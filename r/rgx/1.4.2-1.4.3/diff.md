# Comparing `tmp/rgx-1.4.2.tar.gz` & `tmp/rgx-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgx-1.4.2.tar", max compression
+gzip compressed data, was "rgx-1.4.3.tar", max compression
```

## Comparing `rgx-1.4.2.tar` & `rgx-1.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-08-08 01:35:17.115732 rgx-1.4.2/LICENSE
--rw-r--r--   0        0        0    16342 2023-08-08 01:35:17.115732 rgx-1.4.2/README.md
--rw-r--r--   0        0        0      586 2023-08-08 01:35:17.115732 rgx-1.4.2/pyproject.toml
--rw-r--r--   0        0        0      129 2023-08-08 01:35:17.115732 rgx-1.4.2/rgx/__init__.py
--rw-r--r--   0        0        0    33247 2023-08-08 01:35:17.115732 rgx-1.4.2/rgx/entities.py
--rw-r--r--   0        0        0      933 2023-08-08 01:35:17.115732 rgx-1.4.2/rgx/meta.py
--rw-r--r--   0        0        0      663 2023-08-08 01:35:17.115732 rgx-1.4.2/rgx/unicode_meta.py
--rw-r--r--   0        0        0    17063 1970-01-01 00:00:00.000000 rgx-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-08 02:27:28.840202 rgx-1.4.3/LICENSE
+-rw-r--r--   0        0        0    16342 2023-08-08 02:27:28.840202 rgx-1.4.3/README.md
+-rw-r--r--   0        0        0      585 2023-08-08 02:27:28.840202 rgx-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-08-08 02:27:28.840202 rgx-1.4.3/rgx/__init__.py
+-rw-r--r--   0        0        0    33328 2023-08-08 02:27:28.840202 rgx-1.4.3/rgx/entities.py
+-rw-r--r--   0        0        0      933 2023-08-08 02:27:28.840202 rgx-1.4.3/rgx/meta.py
+-rw-r--r--   0        0        0      663 2023-08-08 02:27:28.840202 rgx-1.4.3/rgx/unicode_meta.py
+-rw-r--r--   0        0        0    17063 1970-01-01 00:00:00.000000 rgx-1.4.3/PKG-INFO
```

### Comparing `rgx-1.4.2/LICENSE` & `rgx-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rgx-1.4.2/README.md` & `rgx-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `rgx-1.4.2/pyproject.toml` & `rgx-1.4.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rgx"
-version = "1.4.2"
+version = "1.4.3"
 description = "Typed, simple and readable regexp generation"
 authors = ["Dmitry Gritsenko <rgx@evtn.ru>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/evtn/rgx"
 homepage = "https://github.com/evtn/rgx"
 keywords = ["regex", "regexp", "regular expressions"]
@@ -13,12 +13,12 @@
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 mypy = "^1.4.1"
-coveralls = "^3.3.1"
+coverage = "^7.2.7"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rgx-1.4.2/rgx/entities.py` & `rgx-1.4.3/rgx/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,18 +82,23 @@
             return pattern(literal[0])
         return NonCapturingGroup(Concat(*literal))
 
     if isinstance(literal, list):
         return Chars(literal)
 
 
-def respect_priority(contents_: AnyRegexPattern, other_priority: int) -> RegexPattern:
-    contents: RegexPattern = pattern(contents_)
+def respect_priority(contents: AnyRegexPattern, other_priority: int) -> RegexPattern:
+    contents = pattern(contents)
+
+    if isinstance(contents, NonCapturingGroup):
+        return respect_priority(contents.contents, other_priority)
+
     if contents.priority < other_priority:
         return NonCapturingGroup(contents)
+
     return contents
 
 
 class RegexPattern:
     priority: int = 100 * priority_step
     optimized = False
 
@@ -108,16 +113,16 @@
     def case_insensitive(self) -> RegexPattern:
         return self.set_flags("i")
 
     def merge_flags(self) -> RegexPattern:
         return self
 
     def optimize(self) -> RegexPattern:
-        self = self.merge_flags()
         self = self.apply(lambda x: x.optimize())
+        self = self.merge_flags()
 
         self.optimized = True
         return self
 
     def apply(self, fn: Processor) -> Self:
         return self
 
@@ -143,16 +148,18 @@
 
         new_parts: list[RegexPattern] = []
 
         for alt in parts:
             assert isinstance(alt, LocalFlags)
             new_flags = "".join(f for f in alt.flags if f not in common_flags)
 
-            if new_flags:
-                new_parts.append(LocalFlags(alt, new_flags))
+            if not new_flags:
+                new_parts.append(alt.contents)
+            elif new_flags != alt.flags:
+                new_parts.append(LocalFlags(alt.contents, new_flags))
             else:
                 new_parts.append(alt)
 
         return new_parts, common_flags
 
     def render_str(self, flags: str = "") -> str:
         """
@@ -822,16 +829,14 @@
         return self.apply(lambda x: x.case_insensitive())
 
     def render(self) -> StrGen:
         for part in self.contents:
             yield from part.render()
 
     def merge_flags(self) -> LocalFlags | Concat:
-        self = self.apply(lambda x: x.merge_flags())
-
         processed, common_flags = self.merge_flags_abstract(self.contents)
 
         new = Concat(*processed)
 
         if not common_flags:
             return new
 
@@ -852,16 +857,14 @@
             respect_priority(alternative, self.priority) for alternative in alternatives
         ]
 
     def case_insensitive(self) -> RegexPattern:
         return self.apply(lambda x: x.case_insensitive())
 
     def merge_flags(self) -> LocalFlags | Option:
-        self = self.apply(lambda x: x.merge_flags())
-
         processed, common_flags = self.merge_flags_abstract(self.alternatives)
 
         new = Option(*processed)
 
         if not common_flags:
             return new
 
@@ -887,15 +890,15 @@
 
 class LocalFlags(RegexPattern):
     def __init__(self, contents: AnyRegexPattern, flags: str):
         self.contents = pattern(contents)
         self.flags = flags
 
     def case_insensitive(self) -> RegexPattern:
-        return LocalFlags(self.contents.case_insensitive(), self.flags)
+        return self.apply(lambda x: x.case_insensitive())
 
     def render(self) -> StrGen:
         yield "(?"
         yield self.flags
         yield ":"
         yield from self.contents.render()
         yield ")"
```

### Comparing `rgx-1.4.2/rgx/meta.py` & `rgx-1.4.3/rgx/meta.py`

 * *Files identical despite different names*

### Comparing `rgx-1.4.2/rgx/unicode_meta.py` & `rgx-1.4.3/rgx/unicode_meta.py`

 * *Files identical despite different names*

### Comparing `rgx-1.4.2/PKG-INFO` & `rgx-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgx
-Version: 1.4.2
+Version: 1.4.3
 Summary: Typed, simple and readable regexp generation
 Home-page: https://github.com/evtn/rgx
 License: MIT
 Keywords: regex,regexp,regular expressions
 Author: Dmitry Gritsenko
 Author-email: rgx@evtn.ru
 Requires-Python: >=3.7,<4.0
```

