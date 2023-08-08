# Comparing `tmp/rgx-1.4.0.tar.gz` & `tmp/rgx-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgx-1.4.0.tar", max compression
+gzip compressed data, was "rgx-1.4.2.tar", max compression
```

## Comparing `rgx-1.4.0.tar` & `rgx-1.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-08-08 00:21:07.393309 rgx-1.4.0/LICENSE
--rw-r--r--   0        0        0    16342 2023-08-08 00:21:07.393309 rgx-1.4.0/README.md
--rw-r--r--   0        0        0      565 2023-08-08 00:21:07.393309 rgx-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      129 2023-08-08 00:21:07.393309 rgx-1.4.0/rgx/__init__.py
--rw-r--r--   0        0        0    33715 2023-08-08 00:21:07.393309 rgx-1.4.0/rgx/entities.py
--rw-r--r--   0        0        0      933 2023-08-08 00:21:07.393309 rgx-1.4.0/rgx/meta.py
--rw-r--r--   0        0        0      663 2023-08-08 00:21:07.393309 rgx-1.4.0/rgx/unicode_meta.py
--rw-r--r--   0        0        0    17063 1970-01-01 00:00:00.000000 rgx-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-08 01:35:17.115732 rgx-1.4.2/LICENSE
+-rw-r--r--   0        0        0    16342 2023-08-08 01:35:17.115732 rgx-1.4.2/README.md
+-rw-r--r--   0        0        0      586 2023-08-08 01:35:17.115732 rgx-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-08-08 01:35:17.115732 rgx-1.4.2/rgx/__init__.py
+-rw-r--r--   0        0        0    33247 2023-08-08 01:35:17.115732 rgx-1.4.2/rgx/entities.py
+-rw-r--r--   0        0        0      933 2023-08-08 01:35:17.115732 rgx-1.4.2/rgx/meta.py
+-rw-r--r--   0        0        0      663 2023-08-08 01:35:17.115732 rgx-1.4.2/rgx/unicode_meta.py
+-rw-r--r--   0        0        0    17063 1970-01-01 00:00:00.000000 rgx-1.4.2/PKG-INFO
```

### Comparing `rgx-1.4.0/LICENSE` & `rgx-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rgx-1.4.0/README.md` & `rgx-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `rgx-1.4.0/pyproject.toml` & `rgx-1.4.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rgx"
-version = "1.4.0"
+version = "1.4.2"
 description = "Typed, simple and readable regexp generation"
 authors = ["Dmitry Gritsenko <rgx@evtn.ru>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/evtn/rgx"
 homepage = "https://github.com/evtn/rgx"
 keywords = ["regex", "regexp", "regular expressions"]
@@ -13,11 +13,12 @@
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 mypy = "^1.4.1"
+coveralls = "^3.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rgx-1.4.0/rgx/entities.py` & `rgx-1.4.2/rgx/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -445,15 +445,15 @@
     def __init__(self, *contents: AnyRegexPattern):
         self.contents = pattern(contents)
 
     def render_prefix(self) -> StrGen:
         yield self.prefix
 
     def case_insensitive(self):
-        return self.__class__(self.contents.case_insensitive())
+        return self.apply(lambda x: x.case_insensitive())
 
     def render(self) -> StrGen:
         yield "("
         yield from self.render_prefix()
         yield from self.contents.render()
         yield ")"
 
@@ -814,18 +814,16 @@
             contents = (contents[0], Concat(*contents[1:]))
 
         self.contents = [respect_priority(part, self.priority) for part in contents]
 
     def __add__(self, other: AnyRegexPattern) -> Concat:
         return Concat(*self.contents, other)
 
-    def case_insensitive(self):
-        new = Concat()
-        new.contents = [part.case_insensitive() for part in self.contents]
-        return new
+    def case_insensitive(self) -> RegexPattern:
+        return self.apply(lambda x: x.case_insensitive())
 
     def render(self) -> StrGen:
         for part in self.contents:
             yield from part.render()
 
     def merge_flags(self) -> LocalFlags | Concat:
         self = self.apply(lambda x: x.merge_flags())
@@ -851,21 +849,15 @@
             alternatives = (alternatives[0], Option(*alternatives[1:]))
 
         self.alternatives = [
             respect_priority(alternative, self.priority) for alternative in alternatives
         ]
 
     def case_insensitive(self) -> RegexPattern:
-        new = Option()
-        alts = [part.case_insensitive() for part in self.alternatives]
-
-        if all(isinstance(alt, LocalFlags) and "i" in alt.flags for alt in alts):
-            pass
-
-        return new
+        return self.apply(lambda x: x.case_insensitive())
 
     def merge_flags(self) -> LocalFlags | Option:
         self = self.apply(lambda x: x.merge_flags())
 
         processed, common_flags = self.merge_flags_abstract(self.alternatives)
 
         new = Option(*processed)
@@ -944,20 +936,15 @@
             raise ValueError("Quantifier upper bound cannot be less than 0")
 
         self.min_count = min_count
         self.max_count = max_count
         self.lazy = lazy
 
     def case_insensitive(self) -> RegexPattern:
-        new = self.contents.case_insensitive().repeat(self.min_count)
-        if self.max_count is None:
-            new = new.or_more()
-        else:
-            new = new.to(self.max_count)
-        return new
+        return self.apply(lambda x: x.case_insensitive())
 
     def repeat(self, count: int, lazy: bool = False) -> Range:
         """
 
         The logic here should be carefully thought through.
         If we multiply a fixed-size pattern a{X} by Y, we generally DO NOT get a{X*Y}
         If we multiply a .or_less() pattern a{,X} by Y, we get a{,X*Y}
@@ -1157,21 +1144,14 @@
     def __init__(
         self, group: int, true_option: AnyRegexPattern, false_option: AnyRegexPattern
     ) -> None:
         self.group = group
         self.true_option = respect_priority(true_option, Option.priority + 1)
         self.false_option = respect_priority(false_option, Option.priority + 1)
 
-    def case_insensitive(self) -> RegexPattern:
-        return ConditionalPattern(
-            self.group,
-            self.true_option.case_insensitive(),
-            self.false_option.case_insensitive(),
-        )
-
     def render(self) -> StrGen:
         yield "(?("
         yield str(self.group)
         yield ")"
         yield from self.true_option.render()
         yield "|"
         yield from self.false_option.render()
@@ -1180,14 +1160,17 @@
     def apply(self, fn: Processor) -> Self:
         return self.__class__(
             self.group,
             fn(self.true_option),
             fn(self.false_option),
         )
 
+    def case_insensitive(self) -> RegexPattern:
+        return self.apply(lambda x: x.case_insensitive())
+
 
 class Literal(RegexPattern):
     def __init__(self, contents: str) -> None:
         self.contents: str = contents
         if len(self.contents) != 1:
             self.priority = 2 * priority_step
```

### Comparing `rgx-1.4.0/rgx/meta.py` & `rgx-1.4.2/rgx/meta.py`

 * *Files identical despite different names*

### Comparing `rgx-1.4.0/rgx/unicode_meta.py` & `rgx-1.4.2/rgx/unicode_meta.py`

 * *Files identical despite different names*

### Comparing `rgx-1.4.0/PKG-INFO` & `rgx-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgx
-Version: 1.4.0
+Version: 1.4.2
 Summary: Typed, simple and readable regexp generation
 Home-page: https://github.com/evtn/rgx
 License: MIT
 Keywords: regex,regexp,regular expressions
 Author: Dmitry Gritsenko
 Author-email: rgx@evtn.ru
 Requires-Python: >=3.7,<4.0
```

