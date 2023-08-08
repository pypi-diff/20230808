# Comparing `tmp/mypy_upgrade-0.0.1a4.tar.gz` & `tmp/mypy_upgrade-0.0.1a5.tar.gz`

## Comparing `mypy_upgrade-0.0.1a4.tar` & `mypy_upgrade-0.0.1a5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/__main__.py
--rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/cli.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/editing.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/filter.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/py.typed
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/silence.py
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/mypy_upgrade/utils.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/.gitignore
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/AUTHORS.md
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/LICENSE.txt
--rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/README.md
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/pyproject.toml
--rw-r--r--   0        0        0     7941 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a4/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/mypy_upgrade/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/mypy_upgrade/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/mypy_upgrade/__main__.py
+-rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/mypy_upgrade/cli.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/mypy_upgrade/editing.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/mypy_upgrade/filter.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/mypy_upgrade/parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/mypy_upgrade/py.typed
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/mypy_upgrade/silence.py
+-rw-r--r--   0        0        0     6515 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/mypy_upgrade/utils.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/mypy_upgrade/warnings.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/.gitignore
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/AUTHORS.md
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/LICENSE.txt
+-rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/README.md
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/pyproject.toml
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 mypy_upgrade-0.0.1a5/PKG-INFO
```

### Comparing `mypy_upgrade-0.0.1a4/mypy_upgrade/editing.py` & `mypy_upgrade-0.0.1a5/mypy_upgrade/editing.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,18 @@
         error_codes.extend(e for e in old_error_codes if e not in error_codes)
         comment = old_type_ignore_re.sub("", comment)
 
         # Check for other comments; otherwise, remove comment
         if not re.search(r"[^#\s]", comment):
             comment = ""
         else:
-            comment = f' {comment.lstrip("# ")}'
+            comment = f' # {comment.lstrip("# ")}'
+    elif comment:
+        # format comment
+        comment = f' # {comment.lstrip("# ")}'
 
     sorted_error_codes = ", ".join(sorted(error_codes))
 
     return f"# type: ignore[{sorted_error_codes}]{comment}"
 
 
 def format_type_ignore_comment(comment: str) -> str:
```

### Comparing `mypy_upgrade-0.0.1a4/mypy_upgrade/filter.py` & `mypy_upgrade-0.0.1a5/mypy_upgrade/filter.py`

 * *Files identical despite different names*

### Comparing `mypy_upgrade-0.0.1a4/mypy_upgrade/parsing.py` & `mypy_upgrade-0.0.1a5/mypy_upgrade/parsing.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 import re
 from typing import NamedTuple, TextIO
 
 
 class MypyError(NamedTuple):
     filename: str
-    col_offset: int | None
     line_no: int
+    col_offset: int | None
     message: str
     error_code: str
 
     @staticmethod
     def filename_and_line_number(error: MypyError) -> tuple[str, int]:
         return error.filename, error.line_no
 
@@ -50,16 +50,16 @@
                 col_offset = int(error.group("col_offset"))
             else:
                 col_offset = None
 
             errors.append(
                 MypyError(
                     filename,
-                    col_offset,
                     line_no,
+                    col_offset,
                     message.strip(),
                     error_code,
                 )
             )
 
     return sorted(errors, key=MypyError.filename_and_line_number)
```

### Comparing `mypy_upgrade-0.0.1a4/mypy_upgrade/silence.py` & `mypy_upgrade-0.0.1a5/mypy_upgrade/silence.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,29 +24,30 @@
     description_style: Literal["full", "none"],
     fix_me: str,
 ) -> str:
     """Silences the given error on a line with an error code-specific comment.
 
     Args:
         line: a string containing the line.
-        error: an `Iterable` of `MypyError`s to be silenced.
+        error: an `Iterable` in which each entry is a `MypyError` to be
+            silenced.
         description_style: a string specifying the style of the description of
             errors.
         fix_me: a string specifying a "fix me" message to be appended after the
             silencing comment.
     Returns:
         The line with a type error suppression comment.
     """
     unused_ignore = None
     error_codes = []
     descriptions = []
     for error in errors:
         if error.error_code == "unused-ignore":
             unused_ignore = error  # there should only be one
-        else:
+        elif error.error_code not in error_codes:
             error_codes.append(error.error_code)
             descriptions.append(error.message)
 
     python_code, comment = split_code_and_comment(line.rstrip())
 
     if unused_ignore:
         codes_to_remove = description_to_type_ignore(unused_ignore.message)
@@ -62,13 +63,13 @@
         )
     else:
         final_comment = cleaned_comment
 
     updated_line = f"{python_code}  {final_comment}".rstrip()
 
     if fix_me:
-        updated_line += f" # {fix_me.strip()}"
+        updated_line += f" # {fix_me}"
 
     if description_style == "full" and descriptions:
         updated_line += f" # {', '.join(descriptions)}"
 
     return updated_line + "\n"
```

### Comparing `mypy_upgrade-0.0.1a4/mypy_upgrade/utils.py` & `mypy_upgrade-0.0.1a5/mypy_upgrade/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # remove when dropping Python 3.7-3.9 support
 from __future__ import annotations
 
 import io
-import math
 import tokenize
 from collections.abc import Iterable
 from typing import NamedTuple, TextIO
 
 from mypy_upgrade.parsing import MypyError
 
 
@@ -18,53 +17,21 @@
         start: a 2-tuple representing the start of the unsilenceable region
             whose first entry is the start line (1-indexed) and whose second
             entry is the start column offset.
         end: a 2-tuple representing the end of the unsilenceable region
             whose first entry is the end line (1-indexed) and whose second
             entry is the end column offset.
 
-        Setting any entry of either `start` or `end` to -1 will result in that
-        entry being set to `math.inf` for comparison operations.
+        When start[0] = end[0], it is interpreted that the Unsilenceable
+        region is an explicitly continued line.
     """
 
     start: tuple[int, int]  # line, column
     end: tuple[int, int]  # line, column
 
-    def surrounds(self, error: MypyError) -> bool:
-        """Determines whether a given error is surrounded by the unsilenceable
-        region
-
-        Args:
-            error: a MypyError instance.
-
-        Returns:
-            True if the MypyError lies within the region. False, otherwise.
-            Note that if the column offset is not specified in the error, this
-            function will only return `True` if the error lies on one of the
-            interior lines of the region.
-        """
-        positive_self = self._convert_to_positive_tuple()
-        if error.col_offset is None:
-            return positive_self[0][0] < error.line_no < positive_self[1][0]
-
-        return (
-            positive_self[0]
-            <= (error.line_no, error.col_offset)
-            <= positive_self[1]
-        )
-
-    def _convert_to_positive_tuple(
-        self,
-    ) -> tuple[tuple[float, float], tuple[float, float]]:
-        start_line = math.inf if self.start[0] < 0 else self.start[0]
-        start_column = math.inf if self.start[1] < 0 else self.start[1]
-        end_line = math.inf if self.end[0] < 0 else self.end[0]
-        end_column = math.inf if self.end[1] < 0 else self.end[1]
-        return ((start_line, start_column), (end_line, end_column))
-
 
 def split_code_and_comment(line: str) -> tuple[str, str]:
     """Split a line of code into the code part and comment part."""
     reader = io.StringIO(line).readline
 
     try:
         comment_tokens = []
@@ -99,15 +66,15 @@
     Returns:
         A list of UnsilenceableRegion objects.
 
         Multiline strings are represented by UnsilienceableRegion objects
         whose first entries in their `start` and `end` attributes are
         different. Explicitly continued lines are represented by
         UnsilienceableRegion objects whose first entries in their `start` and
-        `end` attributes are different.
+        `end` attributes are the same.
     """
     all_lines = list(tokenize.generate_tokens(stream.readline))
     unsilenceable_regions = []
     for token in all_lines:
         if (
             token.start[0] != token.end[0]
             and token.exact_type == tokenize.STRING
@@ -118,15 +85,15 @@
     comments = [t for t in all_lines if t.exact_type == tokenize.COMMENT]
 
     for token in all_lines:
         if token.line.rstrip("\r\n").endswith("\\") and not any(
             comment.line == token.line for comment in comments
         ):
             start = token.end[0], 0
-            end = token.end[0], -1
+            end = token.end[0], len(token.line)
             region = UnsilenceableRegion(start, end)
             unsilenceable_regions.append(region)
 
     return unsilenceable_regions
 
 
 def find_safe_end_line(
@@ -134,15 +101,16 @@
 ) -> int:
     """Find a syntax-safe line on which to place an error suppression comment
     for the given error.
 
     Args:
         error: a `MypyError` for which a type error suppression comment is to
             placed.
-        unsilenceable_regions: an `Iterable` of `UnsilenceableRegion`s.
+        unsilenceable_regions: an `Iterable` in which each entry is an
+            `UnsilenceableRegion`.
 
     Returns:
         An integer representing a safe line on which to place an error
         suppression comment if it exists. If no safe line exists, this method
         returns -1.
     """
     new_line = None
@@ -156,15 +124,18 @@
         # can be suppressed if its column number is unknown
         if (
             error.col_offset is None
             and region.start[0] <= error.line_no <= region.end[0]
         ):
             return -1
 
-        if error.col_offset is not None and region.surrounds(error):
+        if (
+            error.col_offset is not None
+            and region.start <= (error.line_no, error.col_offset) <= region.end
+        ):
             return -1
 
         # Error precedes same line multiline string
         if (
             error.line_no == region.start[0]
             and region.start[0] != region.end[0]
         ):
@@ -172,16 +143,16 @@
             new_col_offset = int(region.end[1])
 
     if new_line is None:
         return error.line_no
 
     new_error = MypyError(
         error.filename,
-        new_col_offset,
         new_line,
+        new_col_offset,
         error.message,
         error.error_code,
     )
     return find_safe_end_line(new_error, unsilenceable_regions)
 
 
 def correct_line_numbers(
@@ -191,32 +162,32 @@
 
     Args:
         stream: A text stream from which the line numbers of provided errors
             are to be corrected.
         errors: The errors whose line numbers are to be corrected.
 
     Returns:
-        A 2-tuple whose first entry is a list of MypyErrors from `errors` for
-        which type suppression comments can be added (with line numbers
-        corrected) and whose second entry is a list of the excluded MypyErrors.
+        A 2-tuple whose first entry is a list in which each entry is a
+        `MypyError` from `errors` for which type suppression comments can be
+        added (with line numbers corrected) and whose second entry is a list
+        of each `MypyError` that cannot be silenced.
     """
-    # ? need to copy
     unsilenceable_regions = find_unsilenceable_regions(stream)
     line_corrected_errors = []
-    excluded_errors = []
+    unsilenceable_errors = []
     for error in errors:
         end_line = find_safe_end_line(error, unsilenceable_regions)
 
         if end_line == -1:
-            excluded_errors.append(error)
+            unsilenceable_errors.append(error)
         else:
             line_corrected_errors.append(
                 MypyError(
                     error.filename,
-                    error.col_offset,
                     end_line,
+                    error.col_offset,
                     error.message,
                     error.error_code,
                 )
             )
 
-    return line_corrected_errors, excluded_errors
+    return line_corrected_errors, unsilenceable_errors
```

### Comparing `mypy_upgrade-0.0.1a4/.gitignore` & `mypy_upgrade-0.0.1a5/.gitignore`

 * *Files identical despite different names*

### Comparing `mypy_upgrade-0.0.1a4/LICENSE.txt` & `mypy_upgrade-0.0.1a5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mypy_upgrade-0.0.1a4/README.md` & `mypy_upgrade-0.0.1a5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 You may want to include the error messages provided by `mypy` in the
 suppression comments so that you can fix them later. You can do so using
 the `-d` (or `--description-style`) option
 
     mypy-upgrade --report mypy_report.txt -d full -p package
 
-You also customize the "fix me" message placed after the error suppression
+You can also customize the "fix me" message placed after the error suppression
 comment using the `--fix-me` option
 
     mypy-upgrade --report mypy_report.txt --fix-me "FIX THIS" -p package
 
 To selectively silence errors in packages and modules, use the `-p`
 (`--package`) and `-m` (`--module`) options along with the fully qualified
 module/package name, respectively:
```

### Comparing `mypy_upgrade-0.0.1a4/pyproject.toml` & `mypy_upgrade-0.0.1a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypy_upgrade-0.0.1a4/PKG-INFO` & `mypy_upgrade-0.0.1a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypy-upgrade
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: automatic error suppression for mypy
 Project-URL: Documentation, https://github.com/ugognw/mypy-upgrade#readme
 Project-URL: Issues, https://github.com/ugognw/mypy-upgrade/issues
 Project-URL: Source, https://github.com/ugognw/mypy-upgrade
 Author-email: Ugochukwu Nwosu <ugognw@gmail.com>
 License-Expression: MIT
 License-File: AUTHORS.md
@@ -98,15 +98,15 @@
 
 You may want to include the error messages provided by `mypy` in the
 suppression comments so that you can fix them later. You can do so using
 the `-d` (or `--description-style`) option
 
     mypy-upgrade --report mypy_report.txt -d full -p package
 
-You also customize the "fix me" message placed after the error suppression
+You can also customize the "fix me" message placed after the error suppression
 comment using the `--fix-me` option
 
     mypy-upgrade --report mypy_report.txt --fix-me "FIX THIS" -p package
 
 To selectively silence errors in packages and modules, use the `-p`
 (`--package`) and `-m` (`--module`) options along with the fully qualified
 module/package name, respectively:
```

