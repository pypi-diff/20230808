# Comparing `tmp/rgx-1.3.4.tar.gz` & `tmp/rgx-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgx-1.3.4.tar", max compression
+gzip compressed data, was "rgx-1.4.0.tar", max compression
```

## Comparing `rgx-1.3.4.tar` & `rgx-1.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-06-20 14:04:14.103178 rgx-1.3.4/LICENSE
--rw-r--r--   0        0        0    16342 2023-06-20 14:04:14.103178 rgx-1.3.4/README.md
--rw-r--r--   0        0        0      493 2023-06-20 14:04:14.103178 rgx-1.3.4/pyproject.toml
--rw-r--r--   0        0        0      129 2023-06-20 14:04:14.103178 rgx-1.3.4/rgx/__init__.py
--rw-r--r--   0        0        0    29580 2023-06-20 14:04:14.103178 rgx-1.3.4/rgx/entities.py
--rw-r--r--   0        0        0      933 2023-06-20 14:04:14.103178 rgx-1.3.4/rgx/meta.py
--rw-r--r--   0        0        0      663 2023-06-20 14:04:14.103178 rgx-1.3.4/rgx/unicode_meta.py
--rw-r--r--   0        0        0    17063 1970-01-01 00:00:00.000000 rgx-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-08 00:21:07.393309 rgx-1.4.0/LICENSE
+-rw-r--r--   0        0        0    16342 2023-08-08 00:21:07.393309 rgx-1.4.0/README.md
+-rw-r--r--   0        0        0      565 2023-08-08 00:21:07.393309 rgx-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-08-08 00:21:07.393309 rgx-1.4.0/rgx/__init__.py
+-rw-r--r--   0        0        0    33715 2023-08-08 00:21:07.393309 rgx-1.4.0/rgx/entities.py
+-rw-r--r--   0        0        0      933 2023-08-08 00:21:07.393309 rgx-1.4.0/rgx/meta.py
+-rw-r--r--   0        0        0      663 2023-08-08 00:21:07.393309 rgx-1.4.0/rgx/unicode_meta.py
+-rw-r--r--   0        0        0    17063 1970-01-01 00:00:00.000000 rgx-1.4.0/PKG-INFO
```

### Comparing `rgx-1.3.4/LICENSE` & `rgx-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rgx-1.3.4/README.md` & `rgx-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `rgx-1.3.4/rgx/entities.py` & `rgx-1.4.0/rgx/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from __future__ import annotations
 from typing import (
+    Callable,
     NoReturn,
     Optional,
     Tuple,
+    List,
     Union,
     overload,
     Iterable,
     Sequence,
     TYPE_CHECKING,
 )
 
 if TYPE_CHECKING:
-    from typing import Literal as LiteralType
+    from typing import Literal as LiteralType, Self
+
 
 import itertools
 import re
 
 StrGen = Iterable[str]
 CharType = Union[str, "CharRange", "Literal"]
-LiteralPart = Union["tuple[AnyRegexPattern, ...]", "list[CharType]", str]
+LiteralPart = Union[Tuple["AnyRegexPattern", ...], List[CharType], str]
 AnyRegexPattern = Union[LiteralPart, "RegexPattern"]
+Processor = Callable[["RegexPattern"], "RegexPattern"]
 
 OrResult = Union["Option", "Chars", "ReversedChars"]
 
 priority_step = 1000
 
 
 @overload
@@ -87,39 +91,88 @@
     if contents.priority < other_priority:
         return NonCapturingGroup(contents)
     return contents
 
 
 class RegexPattern:
     priority: int = 100 * priority_step
+    optimized = False
 
     def render(self) -> StrGen:
         """
         Internal method
 
         Returns a generator, that can be joined to get a pattern string representation
         """
         return NotImplemented
 
     def case_insensitive(self) -> RegexPattern:
         return self.set_flags("i")
 
+    def merge_flags(self) -> RegexPattern:
+        return self
+
+    def optimize(self) -> RegexPattern:
+        self = self.merge_flags()
+        self = self.apply(lambda x: x.optimize())
+
+        self.optimized = True
+        return self
+
+    def apply(self, fn: Processor) -> Self:
+        return self
+
+    @staticmethod
+    def merge_flags_abstract(
+        parts: Sequence[RegexPattern],
+    ) -> tuple[Sequence[RegexPattern], set[str]]:
+        common_flags: set[str] | None = None
+
+        for part in parts:
+            if not isinstance(part, LocalFlags):
+                return parts, set()
+
+            flags = set(part.flags)
+
+            if common_flags is None:
+                common_flags = flags
+            else:
+                common_flags &= flags
+
+        if not common_flags:
+            return parts, set()
+
+        new_parts: list[RegexPattern] = []
+
+        for alt in parts:
+            assert isinstance(alt, LocalFlags)
+            new_flags = "".join(f for f in alt.flags if f not in common_flags)
+
+            if new_flags:
+                new_parts.append(LocalFlags(alt, new_flags))
+            else:
+                new_parts.append(alt)
+
+        return new_parts, common_flags
+
     def render_str(self, flags: str = "") -> str:
         """
 
         Renders given pattern into a string with specified global flags.
 
         """
-        contents: Iterable[str]
+
+        parts: list[Iterable[str]] = []
+
         if flags:
-            contents = itertools.chain(GlobalFlags(flags).render(), self.render())
-        else:
-            contents = self.render()
+            parts.append(GlobalFlags(flags).render())
+
+        parts.append(self.optimize().render())
 
-        return "".join(contents)
+        return "".join(itertools.chain(*parts))
 
     def __repr__(self) -> str:
         return self.render_str()
 
     def set_flags(self, flags: str) -> LocalFlags:
         """
         This method adds local flags to given pattern
@@ -400,22 +453,30 @@
 
     def render(self) -> StrGen:
         yield "("
         yield from self.render_prefix()
         yield from self.contents.render()
         yield ")"
 
+    def apply(self, fn: Processor) -> Self:
+        return self.__class__(fn(self.contents))
+
 
 class Group(GroupBase):
     prefix = ""
 
 
 class NonCapturingGroup(GroupBase):
     prefix = "?:"
 
+    def optimize(self) -> RegexPattern:
+        if isinstance(self.contents, NonCapturingGroup):
+            return self.contents.optimize()
+        return super().optimize()
+
 
 class Lookahead(GroupBase):
     prefix = "?="
 
 
 class NegativeLookahead(GroupBase):
     prefix = "?!"
@@ -471,15 +532,15 @@
 
 Bounds = Tuple[int, int]
 
 
 class Chars(RegexPattern):
     non_special = {".", "[", "|", "~", "*", "(", ")", "+", "$", "&", "?", "#"}
 
-    def __init__(self, contents: Sequence[CharType], is_reversed: bool = False):
+    def __init__(self, contents: Sequence[CharType]):
         self.contents = list(merge_chars(contents))
 
     def render(self) -> StrGen:
         if len(self.contents) == 1:
             contents = self.contents[0]
             if contents.is_single_char():
                 yield from contents.render_literal()
@@ -745,56 +806,96 @@
     return Chars([CharRange(start, stop)])
 
 
 class Concat(RegexPattern):
     priority = 2 * priority_step
 
     def __init__(self, *contents: AnyRegexPattern) -> None:
+        if len(contents) >= 3:
+            contents = (contents[0], Concat(*contents[1:]))
+
         self.contents = [respect_priority(part, self.priority) for part in contents]
 
     def __add__(self, other: AnyRegexPattern) -> Concat:
         return Concat(*self.contents, other)
 
     def case_insensitive(self):
         new = Concat()
         new.contents = [part.case_insensitive() for part in self.contents]
         return new
 
     def render(self) -> StrGen:
         for part in self.contents:
             yield from part.render()
 
+    def merge_flags(self) -> LocalFlags | Concat:
+        self = self.apply(lambda x: x.merge_flags())
+
+        processed, common_flags = self.merge_flags_abstract(self.contents)
+
+        new = Concat(*processed)
+
+        if not common_flags:
+            return new
+
+        return LocalFlags(new, "".join(common_flags))
+
+    def apply(self, fn: Processor) -> Self:
+        return self.__class__(*map(fn, self.contents))
+
 
 class Option(RegexPattern):
     priority = 0 * priority_step
 
     def __init__(self, *alternatives: AnyRegexPattern):
+        if len(alternatives) >= 3:
+            alternatives = (alternatives[0], Option(*alternatives[1:]))
+
         self.alternatives = [
             respect_priority(alternative, self.priority) for alternative in alternatives
         ]
 
     def case_insensitive(self) -> RegexPattern:
         new = Option()
-        new.alternatives = [part.case_insensitive() for part in self.alternatives]
+        alts = [part.case_insensitive() for part in self.alternatives]
+
+        if all(isinstance(alt, LocalFlags) and "i" in alt.flags for alt in alts):
+            pass
+
         return new
 
+    def merge_flags(self) -> LocalFlags | Option:
+        self = self.apply(lambda x: x.merge_flags())
+
+        processed, common_flags = self.merge_flags_abstract(self.alternatives)
+
+        new = Option(*processed)
+
+        if not common_flags:
+            return new
+
+        return LocalFlags(new, "".join(common_flags))
+
     def render(self) -> StrGen:
         if not self.alternatives:
             return
         yield from self.alternatives[0].render()
         for alternative in self.alternatives[1:]:
             yield "|"
             yield from alternative.render()
 
     def __or__(self, other: AnyRegexPattern) -> Option:
         return Option(*self.alternatives, other)
 
     def __ror__(self, other: AnyRegexPattern) -> Option:
         return Option(other, *self.alternatives)
 
+    def apply(self, fn: Processor) -> Self:
+        return self.__class__(*map(fn, self.alternatives))
+
 
 class LocalFlags(RegexPattern):
     def __init__(self, contents: AnyRegexPattern, flags: str):
         self.contents = pattern(contents)
         self.flags = flags
 
     def case_insensitive(self) -> RegexPattern:
@@ -803,14 +904,17 @@
     def render(self) -> StrGen:
         yield "(?"
         yield self.flags
         yield ":"
         yield from self.contents.render()
         yield ")"
 
+    def apply(self, fn: Processor) -> Self:
+        return self.__class__(fn(self.contents), self.flags)
+
 
 class GlobalFlags(GroupBase):
     prefix = "?"
 
     def __init__(self, contents: str):
         self.contents = Literal(contents)
 
@@ -942,14 +1046,33 @@
             return
 
         yield from self.render_quantifier()
 
         if self.lazy and self.min_count != self.max_count:
             yield "?"
 
+    def merge_flags(self) -> LocalFlags | Range:
+        processed, common_flags = self.merge_flags_abstract([self.contents])
+
+        if not common_flags:
+            return self
+
+        return LocalFlags(
+            self.apply(lambda _: processed[0]),
+            "".join(common_flags),
+        )
+
+    def apply(self, fn: Processor) -> Self:
+        return self.__class__(
+            fn(self.contents),
+            min_count=self.min_count,
+            max_count=self.max_count,
+            lazy=self.lazy,
+        )
+
 
 class NamedPattern(RegexPattern):
     """
 
     Named capturing group.
 
     If `contents` are omitted, generates a reference, otherwise a named group definition.
@@ -976,14 +1099,37 @@
             yield ">"
             yield from self.contents.render()
         else:
             yield "="
             yield self.name
         yield ")"
 
+    def merge_flags(self) -> LocalFlags | NamedPattern:
+        if self.contents is None:
+            return self
+
+        processed, common_flags = self.merge_flags_abstract([self.contents])
+
+        if not common_flags:
+            return self
+
+        return LocalFlags(
+            self.apply(lambda _: processed[0]),
+            "".join(common_flags),
+        )
+
+    def apply(self, fn: Processor) -> Self:
+        if self.contents is None:
+            return self
+
+        return self.__class__(
+            self.name,
+            fn(self.contents),
+        )
+
 
 class ConditionalPattern(RegexPattern):
     """
     Use to match different patterns depending on whether another group matched or not.
 
     Next two snippets produce effectively the same result:
 
@@ -1027,27 +1173,37 @@
         yield str(self.group)
         yield ")"
         yield from self.true_option.render()
         yield "|"
         yield from self.false_option.render()
         yield ")"
 
+    def apply(self, fn: Processor) -> Self:
+        return self.__class__(
+            self.group,
+            fn(self.true_option),
+            fn(self.false_option),
+        )
+
 
 class Literal(RegexPattern):
     def __init__(self, contents: str) -> None:
         self.contents: str = contents
         if len(self.contents) != 1:
             self.priority = 2 * priority_step
 
     def to(self, other: str | Literal | Chars) -> Chars:
         return Chars([self]).to(other)
 
     def render(self) -> StrGen:
         yield re.escape(self.contents)
 
+    def apply(self, fn: Processor) -> Self:
+        return self
+
 
 class UnescapedLiteral(Literal):
     """
 
     Unescaped literal. Renders into whatever is passed (as long as it is a string)
 
     """
```

### Comparing `rgx-1.3.4/rgx/meta.py` & `rgx-1.4.0/rgx/meta.py`

 * *Files identical despite different names*

### Comparing `rgx-1.3.4/rgx/unicode_meta.py` & `rgx-1.4.0/rgx/unicode_meta.py`

 * *Files identical despite different names*

### Comparing `rgx-1.3.4/PKG-INFO` & `rgx-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgx
-Version: 1.3.4
+Version: 1.4.0
 Summary: Typed, simple and readable regexp generation
 Home-page: https://github.com/evtn/rgx
 License: MIT
 Keywords: regex,regexp,regular expressions
 Author: Dmitry Gritsenko
 Author-email: rgx@evtn.ru
 Requires-Python: >=3.7,<4.0
```

