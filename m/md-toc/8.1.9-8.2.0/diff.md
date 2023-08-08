# Comparing `tmp/md_toc-8.1.9.tar.gz` & `tmp/md_toc-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md_toc-8.1.9.tar", last modified: Fri Feb 10 17:14:11 2023, max compression
+gzip compressed data, was "md_toc-8.2.0.tar", last modified: Tue Aug  8 17:09:15 2023, max compression
```

## Comparing `md_toc-8.1.9.tar` & `md_toc-8.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vm        (1019) vm        (1019)        0 2023-02-10 17:14:11.881694 md_toc-8.1.9/
--rw-r--r--   0 vm        (1019) vm        (1019)       76 2023-02-10 17:08:44.000000 md_toc-8.1.9/CONTRIBUTING.md
--rw-r--r--   0 vm        (1019) vm        (1019)    35147 2023-02-10 17:08:44.000000 md_toc-8.1.9/LICENSE.txt
--rw-r--r--   0 vm        (1019) vm        (1019)      270 2023-02-10 17:08:44.000000 md_toc-8.1.9/MANIFEST.in
--rw-r--r--   0 vm        (1019) vm        (1019)     8411 2023-02-10 17:14:11.881694 md_toc-8.1.9/PKG-INFO
--rw-r--r--   0 vm        (1019) vm        (1019)     7577 2023-02-10 17:08:49.000000 md_toc-8.1.9/README.md
-drwxr-xr-x   0 vm        (1019) vm        (1019)        0 2023-02-10 17:14:11.881694 md_toc-8.1.9/md_toc/
--rw-r--r--   0 vm        (1019) vm        (1019)     1733 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/__init__.py
--rwxr-xr-x   0 vm        (1019) vm        (1019)     1291 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/__main__.py
--rw-r--r--   0 vm        (1019) vm        (1019)    59946 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/api.py
--rw-r--r--   0 vm        (1019) vm        (1019)    14338 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/cli.py
-drwxr-xr-x   0 vm        (1019) vm        (1019)        0 2023-02-10 17:14:11.881694 md_toc-8.1.9/md_toc/cmark/
--rw-r--r--   0 vm        (1019) vm        (1019)      817 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/cmark/__init__.py
--rw-r--r--   0 vm        (1019) vm        (1019)     8533 2023-02-10 17:08:49.000000 md_toc-8.1.9/md_toc/cmark/buffer_c.py
--rw-r--r--   0 vm        (1019) vm        (1019)     1569 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/cmark/buffer_h.py
--rw-r--r--   0 vm        (1019) vm        (1019)     2603 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/cmark/chunk_h.py
--rw-r--r--   0 vm        (1019) vm        (1019)     1552 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/cmark/cmark_ctype_c.py
--rw-r--r--   0 vm        (1019) vm        (1019)     2673 2023-02-10 17:08:49.000000 md_toc-8.1.9/md_toc/cmark/cmark_h.py
--rw-r--r--   0 vm        (1019) vm        (1019)     1132 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/cmark/houdini_h.py
--rw-r--r--   0 vm        (1019) vm        (1019)     5674 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/cmark/houdini_html_u_c.py
--rw-r--r--   0 vm        (1019) vm        (1019)    60427 2023-02-10 17:08:49.000000 md_toc-8.1.9/md_toc/cmark/inlines_c.py
--rw-r--r--   0 vm        (1019) vm        (1019)     8542 2023-02-10 17:08:49.000000 md_toc-8.1.9/md_toc/cmark/node_c.py
--rw-r--r--   0 vm        (1019) vm        (1019)     3869 2023-02-10 17:08:49.000000 md_toc-8.1.9/md_toc/cmark/node_h.py
--rw-r--r--   0 vm        (1019) vm        (1019)     4499 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/cmark/references_c.py
--rw-r--r--   0 vm        (1019) vm        (1019)     1892 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/cmark/references_h.py
--rw-r--r--   0 vm        (1019) vm        (1019)     5194 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/cmark/scanners_c.py
--rw-r--r--   0 vm        (1019) vm        (1019)     2217 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/cmark/scanners_h.py
--rw-r--r--   0 vm        (1019) vm        (1019)     4710 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/cmark/utf8_c.py
--rw-r--r--   0 vm        (1019) vm        (1019)    26242 2023-02-10 17:08:49.000000 md_toc-8.1.9/md_toc/constants.py
--rw-r--r--   0 vm        (1019) vm        (1019)     1620 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/exceptions.py
--rw-r--r--   0 vm        (1019) vm        (1019)     7710 2023-02-10 17:08:44.000000 md_toc-8.1.9/md_toc/generic.py
-drwxr-xr-x   0 vm        (1019) vm        (1019)        0 2023-02-10 17:14:11.881694 md_toc-8.1.9/md_toc.egg-info/
--rw-r--r--   0 vm        (1019) vm        (1019)     8411 2023-02-10 17:14:11.000000 md_toc-8.1.9/md_toc.egg-info/PKG-INFO
--rw-r--r--   0 vm        (1019) vm        (1019)      652 2023-02-10 17:14:11.000000 md_toc-8.1.9/md_toc.egg-info/SOURCES.txt
--rw-r--r--   0 vm        (1019) vm        (1019)       89 2023-02-10 17:08:44.000000 md_toc-8.1.9/pyproject.toml
--rw-r--r--   0 vm        (1019) vm        (1019)     1263 2023-02-10 17:14:11.881694 md_toc-8.1.9/setup.cfg
--rw-r--r--   0 vm        (1019) vm        (1019)     1014 2023-02-10 17:08:44.000000 md_toc-8.1.9/setup.py
+drwxr-xr-x   0 vm        (1019) vm        (1019)        0 2023-08-08 17:09:15.196436 md_toc-8.2.0/
+-rw-r--r--   0 vm        (1019) vm        (1019)       76 2023-08-08 16:20:18.000000 md_toc-8.2.0/CONTRIBUTING.md
+-rw-r--r--   0 vm        (1019) vm        (1019)    35147 2023-08-08 16:20:18.000000 md_toc-8.2.0/LICENSE.txt
+-rw-r--r--   0 vm        (1019) vm        (1019)      270 2023-08-08 16:20:18.000000 md_toc-8.2.0/MANIFEST.in
+-rw-r--r--   0 vm        (1019) vm        (1019)     8542 2023-08-08 17:09:15.196436 md_toc-8.2.0/PKG-INFO
+-rw-r--r--   0 vm        (1019) vm        (1019)     7708 2023-08-08 16:20:31.000000 md_toc-8.2.0/README.md
+drwxr-xr-x   0 vm        (1019) vm        (1019)        0 2023-08-08 17:09:15.196436 md_toc-8.2.0/md_toc/
+-rw-r--r--   0 vm        (1019) vm        (1019)     1749 2023-08-08 16:20:31.000000 md_toc-8.2.0/md_toc/__init__.py
+-rwxr-xr-x   0 vm        (1019) vm        (1019)     1394 2023-08-08 16:20:31.000000 md_toc-8.2.0/md_toc/__main__.py
+-rw-r--r--   0 vm        (1019) vm        (1019)    59939 2023-08-08 16:20:31.000000 md_toc-8.2.0/md_toc/api.py
+-rw-r--r--   0 vm        (1019) vm        (1019)    15111 2023-08-08 16:20:31.000000 md_toc-8.2.0/md_toc/cli.py
+drwxr-xr-x   0 vm        (1019) vm        (1019)        0 2023-08-08 17:09:15.196436 md_toc-8.2.0/md_toc/cmark/
+-rw-r--r--   0 vm        (1019) vm        (1019)      817 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/cmark/__init__.py
+-rw-r--r--   0 vm        (1019) vm        (1019)     8533 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/cmark/buffer_c.py
+-rw-r--r--   0 vm        (1019) vm        (1019)     1569 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/cmark/buffer_h.py
+-rw-r--r--   0 vm        (1019) vm        (1019)     2603 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/cmark/chunk_h.py
+-rw-r--r--   0 vm        (1019) vm        (1019)     1552 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/cmark/cmark_ctype_c.py
+-rw-r--r--   0 vm        (1019) vm        (1019)     2673 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/cmark/cmark_h.py
+-rw-r--r--   0 vm        (1019) vm        (1019)     1132 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/cmark/houdini_h.py
+-rw-r--r--   0 vm        (1019) vm        (1019)     5674 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/cmark/houdini_html_u_c.py
+-rw-r--r--   0 vm        (1019) vm        (1019)    60427 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/cmark/inlines_c.py
+-rw-r--r--   0 vm        (1019) vm        (1019)     8542 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/cmark/node_c.py
+-rw-r--r--   0 vm        (1019) vm        (1019)     3869 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/cmark/node_h.py
+-rw-r--r--   0 vm        (1019) vm        (1019)     4499 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/cmark/references_c.py
+-rw-r--r--   0 vm        (1019) vm        (1019)     1892 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/cmark/references_h.py
+-rw-r--r--   0 vm        (1019) vm        (1019)     5194 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/cmark/scanners_c.py
+-rw-r--r--   0 vm        (1019) vm        (1019)     2217 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/cmark/scanners_h.py
+-rw-r--r--   0 vm        (1019) vm        (1019)     4710 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/cmark/utf8_c.py
+-rw-r--r--   0 vm        (1019) vm        (1019)    26242 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/constants.py
+-rw-r--r--   0 vm        (1019) vm        (1019)     1620 2023-08-08 16:20:19.000000 md_toc-8.2.0/md_toc/exceptions.py
+-rw-r--r--   0 vm        (1019) vm        (1019)    11684 2023-08-08 16:20:31.000000 md_toc-8.2.0/md_toc/generic.py
+drwxr-xr-x   0 vm        (1019) vm        (1019)        0 2023-08-08 17:09:15.196436 md_toc-8.2.0/md_toc.egg-info/
+-rw-r--r--   0 vm        (1019) vm        (1019)     8542 2023-08-08 17:09:15.000000 md_toc-8.2.0/md_toc.egg-info/PKG-INFO
+-rw-r--r--   0 vm        (1019) vm        (1019)      652 2023-08-08 17:09:15.000000 md_toc-8.2.0/md_toc.egg-info/SOURCES.txt
+-rw-r--r--   0 vm        (1019) vm        (1019)       89 2023-08-08 16:20:19.000000 md_toc-8.2.0/pyproject.toml
+-rw-r--r--   0 vm        (1019) vm        (1019)     1263 2023-08-08 17:09:15.200436 md_toc-8.2.0/setup.cfg
+-rw-r--r--   0 vm        (1019) vm        (1019)     1014 2023-08-08 16:20:19.000000 md_toc-8.2.0/setup.py
```

### Comparing `md_toc-8.1.9/LICENSE.txt` & `md_toc-8.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/PKG-INFO` & `md_toc-8.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md_toc
-Version: 8.1.9
+Version: 8.2.0
 Summary: Automatically generate and add an accurate table of contents to markdown files
 Home-page: https://blog.franco.net.eu.org/software/#md-toc
 Author: Franco Masotti
 Author-email: franco.masotti@tutanota.com
 License: GPLv3+,
 Keywords: markdown,toc,text,table-of-contents,documentation
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,15 +48,15 @@
   - [Changelog and trusted source](#changelog-and-trusted-source)
   - [Crypto donations](#crypto-donations)
 
 <!--TOC-->
 
 ## Video
 
-[![image](https://asciinema.org/a/452384.png)](https://asciinema.org/a/452384)
+[![image](./assets/md-toc_youtube_video_thumbnail.png)](https://www.youtube.com/watch?v=guyVdPNmC0A&t=49s)
 
 ## Description
 
 The table of contents (a.k.a: TOC) generated by this program is designed
 to work with several markdown parsers such as the ones used by GitHub
 and GitLab.
 
@@ -75,28 +75,29 @@
   called `Table of contents` to its Gitlab Flavored Mardown
 
 ## Features
 
 - works offline
 - edits file in place using a TOC marker (default `<!--TOC-->`) or
   output to standard output
-- selection of indentation level
+- maximum heading level selection (1 to 6)
 - list indentation based on heading, which can optionally be disabled
-- outputs an ordered or unordered TOC list
+- outputs an ordered or unordered TOC list with list marker selection
 - creates anchor links to markdown headings by default or a plain list
   as alternative
 - checks if heading level is coherent: this avoid creating an
   erroneous TOC. This feature can be disabled if needed
 - skip any number lines before generating the TOC
 - can read content from standard input
 - handles multiple files at once
 - selection of newline string
-- selection of list marker
+- check if there is difference between existing TOC in file and newly generated
+  one
 - supports GitHub, GitLab, Commonmark, Redcarpet and others
-- [pre-commit](https://pre-commit.com/)
+- [pre-commit](https://pre-commit.com/) md-toc
   [hook](https://docs.franco.net.eu.org/md-toc/pre_commit_hook.html)
 
 And more! See the
 [feature comparison table](https://docs.franco.net.eu.org/md-toc/features.html)
 
 ## Examples
```

### Comparing `md_toc-8.1.9/README.md` & `md_toc-8.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   - [Changelog and trusted source](#changelog-and-trusted-source)
   - [Crypto donations](#crypto-donations)
 
 <!--TOC-->
 
 ## Video
 
-[![image](https://asciinema.org/a/452384.png)](https://asciinema.org/a/452384)
+[![image](./assets/md-toc_youtube_video_thumbnail.png)](https://www.youtube.com/watch?v=guyVdPNmC0A&t=49s)
 
 ## Description
 
 The table of contents (a.k.a: TOC) generated by this program is designed
 to work with several markdown parsers such as the ones used by GitHub
 and GitLab.
 
@@ -54,28 +54,29 @@
   called `Table of contents` to its Gitlab Flavored Mardown
 
 ## Features
 
 - works offline
 - edits file in place using a TOC marker (default `<!--TOC-->`) or
   output to standard output
-- selection of indentation level
+- maximum heading level selection (1 to 6)
 - list indentation based on heading, which can optionally be disabled
-- outputs an ordered or unordered TOC list
+- outputs an ordered or unordered TOC list with list marker selection
 - creates anchor links to markdown headings by default or a plain list
   as alternative
 - checks if heading level is coherent: this avoid creating an
   erroneous TOC. This feature can be disabled if needed
 - skip any number lines before generating the TOC
 - can read content from standard input
 - handles multiple files at once
 - selection of newline string
-- selection of list marker
+- check if there is difference between existing TOC in file and newly generated
+  one
 - supports GitHub, GitLab, Commonmark, Redcarpet and others
-- [pre-commit](https://pre-commit.com/)
+- [pre-commit](https://pre-commit.com/) md-toc
   [hook](https://docs.franco.net.eu.org/md-toc/pre_commit_hook.html)
 
 And more! See the
 [feature comparison table](https://docs.franco.net.eu.org/md-toc/features.html)
 
 ## Examples
```

### Comparing `md_toc-8.1.9/md_toc/__init__.py` & `md_toc-8.2.0/md_toc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     is_closing_code_fence,
     is_opening_code_fence,
     is_valid_code_fence_indent,
     remove_emphasis,
     remove_html_tags,
     replace_and_split_newlines,
     toc_renders_as_coherent_list,
+    tocs_equal,
     write_string_on_file_between_markers,
     write_strings_on_files_between_markers,
 )
 from .cli import CliInterface
 from .exceptions import (
     CannotTreatUnicodeString,
     GithubEmptyLinkLabel,
```

### Comparing `md_toc-8.1.9/md_toc/__main__.py` & `md_toc-8.2.0/md_toc/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,17 +30,22 @@
 def main(args=None):
     """Call the CLI interface and wait for the result."""
     retcode = 0
     try:
         ci = CliInterface()
         args = ci.parser.parse_args()
         result = args.func(args)
-        if result is not None:
+        if result is not None and not isinstance(result, bool):
             print(result)
         retcode = 0
+
+        # TOC differs.
+        if result:
+            retcode = 128
+
     except Exception:
         retcode = 1
         traceback.print_exc()
     sys.exit(retcode)
 
 
 if __name__ == '__main__':
```

### Comparing `md_toc-8.1.9/md_toc/api.py` & `md_toc-8.2.0/md_toc/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,146 +38,145 @@
     GithubOverflowOrderedListMarker,
     StdinIsNotAFileToBeWritten,
     StringCannotContainNewlines,
     TocDoesNotRenderAsCoherentList,
 )
 
 
+def tocs_equal(current_toc: str, filename: str, marker: str) -> bool:
+    r"""Check if the TOC already present in a file is the samw of the one passed to this function.
+
+    :parameter current_toc: the new or current TOC. Do not include the ``<!--TOC-->\n\n`` and ``\n\n<!--TOC-->``.
+    :parameter filename: the filename with the TOC for the comparison already present in the file.
+    :parameter marker: the TOC marker.
+    :type current_toc: str
+    :type filename: str
+    :type marker: str
+    :returns: ``True`` if the two TOCs are the same, ``False`` otherwise
+    :rtype: bool
+    :raises: a built-in exception.
+    """
+    tocs_equal: bool = False
+    r: tuple = generic._get_existing_toc(filename, marker)
+    old_toc: str = r[0]
+    if current_toc.strip() == old_toc:
+        tocs_equal = True
+    return tocs_equal
+
+
 def write_string_on_file_between_markers(
     filename: str,
     string: str,
     marker: str,
     newline_string: str = common_defaults['newline string'],
-):
+) -> bool:
     r"""Write the table of contents on a single file.
 
     :parameter filename: the file that needs to be read or modified.
     :parameter string: the string that will be written on the file.
     :parameter marker: a marker that will identify the start
          and the end of the string.
     :parameter newline_string: the new line separator.
          Defaults to ``os.linesep``.
-    :type filenames: str
+    :type filename: str
     :type string: str
     :type marker: str
     :type newline_string: str
-    :returns: None
-    :rtype: None
+    :returns: ``True`` if new TOC is the same as the exising one, ``False`` otherwise.
+    :rtype: bool
     :raises: StdinIsNotAFileToBeWritten or an fpyutils exception
          or a built-in exception.
     """
     if filename == '-':
         raise StdinIsNotAFileToBeWritten
 
-    final_string = ''.join([
+    # TOC that is written to the file.
+    final_toc_string: str = ''.join([
         marker, newline_string, newline_string,
         string.rstrip(), newline_string, newline_string, marker, newline_string
     ])
-    marker_line_positions, lines = fpyutils.filelines.get_line_matches(
-        filename,
-        marker,
-        0,
-        loose_matching=True,
-        keep_all_lines=True,
-    )
-    marker_line_positions_length: int = len(marker_line_positions)
-
-    first_marker: int = 1
-    second_marker: int = 2
-    in_loop: bool = False
-    done: bool = False
-    first_marker_position: int = 0
-
-    if marker_line_positions_length > 0:
-        first_marker_position = marker_line_positions[first_marker]
-
-    # Find appropriate TOC markers.
-    while not done and marker_line_positions_length >= 2:
-        interval: str = generic._read_line_interval(
-            lines, marker_line_positions[first_marker] + 1,
-            marker_line_positions[second_marker] - 1)
-        interval_with_offset: str = generic._read_line_interval(
-            lines, marker_line_positions[first_marker] + 2,
-            marker_line_positions[second_marker] - 2)
-        # TODO: add code fence detection.
-        if generic._detect_toc_list(
-                interval_with_offset) or generic._string_empty(interval):
-            fpyutils.filelines.remove_line_interval(
-                filename,
-                marker_line_positions[first_marker],
-                marker_line_positions[second_marker],
-                filename,
-            )
-            first_marker_position = marker_line_positions[first_marker]
-            done = True
-
-        first_marker += 1
-        second_marker += 1
-        marker_line_positions_length -= 1
-        in_loop = True
 
-    if not in_loop and marker_line_positions_length == 1:
-        fpyutils.filelines.remove_line_interval(
-            filename,
-            marker_line_positions[1],
-            marker_line_positions[1],
-            filename,
-        )
+    (
+        old_toc,
+        lines_to_delete,
+        two_or_more_markers,
+        marker_line_positions_length,
+        marker_line_positions,
+        first_marker_line_number,
+    ) = generic._get_existing_toc(filename, marker)
+
+    equal: bool = False
+    if string.strip() == old_toc:
+        equal = True
+
+    generic._remove_line_intervals(filename, lines_to_delete)
+
+    # Only 1 pre-existing marker.
+    if not two_or_more_markers and marker_line_positions_length == 1:
+        generic._remove_line_intervals(
+            filename, [[marker_line_positions[1], marker_line_positions[1]]])
 
+    # 2 or more pre-existing markers.
     if marker_line_positions_length >= 1:
         fpyutils.filelines.insert_string_at_line(
             filename,
-            final_string,
-            first_marker_position,
+            final_toc_string,
+            first_marker_line_number,
             filename,
             append=False,
             newline_character=newline_string,
         )
 
+    return equal
+
 
 def write_strings_on_files_between_markers(
     filenames: list,
     strings: list,
     marker: str,
     newline_string: str = common_defaults['newline string'],
-):
+) -> bool:
     r"""Write the table of contents on multiple files.
 
     :parameter filenames: the files that needs to be read or modified.
     :parameter strings: the strings that will be written on the file. Each
          string is associated with one file.
     :parameter marker: a marker that will identify the start
          and the end of the string.
     :parameter newline_string: the new line separator.
          Defaults to ``os.linesep``.
     :type filenames: list
     :type strings: list
     :type marker: str
     :type newline_string: str
-    :returns: None
-    :rtype: None
+    :returns: ``True`` if all TOCs are the same as the existing ones, ``False``
+         otherwise.
+    :rtype: bool
     :raises: an fpyutils exception or a built-in exception.
     """
     if not len(filenames) == len(strings):
         raise ValueError
     if len(filenames) > 0:
         for f in filenames:
             if not isinstance(f, str):
                 raise TypeError
     if len(strings) > 0:
         for s in strings:
             if not isinstance(s, str):
                 raise TypeError
 
     file_id = 0
+    equal: bool = True
     for f in filenames:
-        write_string_on_file_between_markers(f, strings[file_id], marker,
-                                             newline_string)
+        equal &= write_string_on_file_between_markers(f, strings[file_id],
+                                                      marker, newline_string)
         file_id += 1
 
+    return equal
+
 
 def build_toc(
     filename: str,
     ordered: bool = False,
     no_links: bool = False,
     no_indentation: bool = False,
     no_list_coherence: bool = False,
```

### Comparing `md_toc-8.1.9/md_toc/cli.py` & `md_toc-8.2.0/md_toc/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,38 +28,43 @@
 # See
 # https://packaging.python.org/en/latest/guides/single-sourcing-package-version/
 if sys.version_info >= (3, 8):
     from importlib import metadata
 else:
     import importlib_metadata as metadata
 
-from .api import build_multiple_tocs, write_strings_on_files_between_markers
+from . import generic
+from .api import (
+    build_multiple_tocs,
+    tocs_equal,
+    write_strings_on_files_between_markers,
+)
 from .constants import common_defaults
 from .constants import parser as md_parser
 
 PROGRAM_DESCRIPTION = 'Markdown Table Of Contents: Automatically generate a compliant table\nof contents for a markdown file to improve document readability.'
 VERSION_NAME = 'md_toc'
 
 try:
     dist = metadata.distribution('md_toc')
     VERSION_NUMBER = dist.version
 except metadata.PackageNotFoundError:
     VERSION_NUMBER = 'vDevel'
 
 VERSION_COPYRIGHT = 'Copyright (C) 2017-2023 Franco Masotti, frnmst'
 VERSION_LICENSE = 'License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>\nThis is free software: you are free to change and redistribute it.\nThere is NO WARRANTY, to the extent permitted by law.'
-RETURN_VALUES = 'Return values: 0 ok, 1 error, 2 invalid command'
+RETURN_VALUES = 'Return values: 0 ok, 1 error, 2 invalid command, 128 TOC differs from the one in the file (see --diff option)'
 ADVICE = 'Please read the documentation to understand how each parser works'
 PROGRAM_EPILOG = ADVICE + '\n\n' + RETURN_VALUES + '\n\n' + VERSION_COPYRIGHT + '\n' + VERSION_LICENSE
 
 
 class CliToApi():
     """An interface between the CLI and API functions."""
 
-    def write_toc(self, args):
+    def write_toc(self, args) -> bool:
         """Write the table of contents."""
         ordered = False
         if args.ordered_list_marker is not None:
             list_marker = args.ordered_list_marker
             ordered = True
         elif args.unordered_list_marker is not None:
             list_marker = args.unordered_list_marker
@@ -80,24 +85,37 @@
             keep_header_levels=args.header_levels,
             parser=args.parser,
             list_marker=list_marker,
             skip_lines=args.skip_lines,
             constant_ordered_list=args.constant_ordered_list,
             newline_string=newline_string,
         )
+
+        equal: bool = True
+
         if args.in_place:
-            write_strings_on_files_between_markers(
+            equal = write_strings_on_files_between_markers(
                 filenames=args.filename,
                 strings=toc_struct,
                 marker=args.toc_marker,
                 newline_string=newline_string,
             )
         else:
-            for toc in toc_struct:
+            for i, toc in enumerate(toc_struct):
                 print(toc, end='')
+                if args.diff:
+                    equal &= tocs_equal(toc, args.filename[i], args.toc_marker)
+
+        diff: bool = False
+        if equal is False:
+            diff = True
+
+        # Return that the TOC(s) is differing only if the `--diff` argument
+        # was selected, i.e.: `args.diff`.
+        return diff & args.diff
 
 
 class CliInterface():
     """The interface exposed to the final user."""
 
     def __init__(self):
         """Set the parser variable that will be used instead of using create_parser."""
@@ -311,14 +329,22 @@
             '-i',
             '--no-indentation',
             action='store_true',
             help='avoids adding indentations to the TOC',
         )
 
         parser.add_argument(
+            '-d',
+            '--diff',
+            action='store_true',
+            help=(
+                'returns 128 if the newly generated TOC differs from the one \
+                  already existing in the file'),
+        )
+        parser.add_argument(
             '-l',
             '--no-links',
             action='store_true',
             help='avoids adding links to the TOC',
         )
         parser.add_argument(
             '-m',
```

### Comparing `md_toc-8.1.9/md_toc/cmark/__init__.py` & `md_toc-8.2.0/md_toc/cmark/__init__.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/cmark/buffer_c.py` & `md_toc-8.2.0/md_toc/cmark/buffer_c.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/cmark/buffer_h.py` & `md_toc-8.2.0/md_toc/cmark/buffer_h.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/cmark/chunk_h.py` & `md_toc-8.2.0/md_toc/cmark/chunk_h.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/cmark/cmark_ctype_c.py` & `md_toc-8.2.0/md_toc/cmark/cmark_ctype_c.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/cmark/cmark_h.py` & `md_toc-8.2.0/md_toc/cmark/cmark_h.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/cmark/houdini_h.py` & `md_toc-8.2.0/md_toc/cmark/houdini_h.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/cmark/houdini_html_u_c.py` & `md_toc-8.2.0/md_toc/cmark/houdini_html_u_c.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/cmark/inlines_c.py` & `md_toc-8.2.0/md_toc/cmark/inlines_c.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/cmark/node_c.py` & `md_toc-8.2.0/md_toc/cmark/node_c.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/cmark/node_h.py` & `md_toc-8.2.0/md_toc/cmark/node_h.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/cmark/references_c.py` & `md_toc-8.2.0/md_toc/cmark/references_c.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/cmark/references_h.py` & `md_toc-8.2.0/md_toc/cmark/references_h.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/cmark/scanners_c.py` & `md_toc-8.2.0/md_toc/cmark/scanners_c.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/cmark/scanners_h.py` & `md_toc-8.2.0/md_toc/cmark/scanners_h.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/cmark/utf8_c.py` & `md_toc-8.2.0/md_toc/cmark/utf8_c.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/constants.py` & `md_toc-8.2.0/md_toc/constants.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/exceptions.py` & `md_toc-8.2.0/md_toc/exceptions.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/md_toc/generic.py` & `md_toc-8.2.0/md_toc/generic.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 # You should have received a copy of the GNU General Public License
 # along with md-toc.  If not, see <http://www.gnu.org/licenses/>.
 #
 """Generic functions."""
 
 import re
 
+import fpyutils
+
 
 # _ctoi and _isascii taken from cpython source Lib/curses/ascii.py
 # See:
 # https://github.com/python/cpython/blob/283de2b9c18e38c9a573526d6c398ade7dd6f8e9/Lib/curses/ascii.py#L48
 # https://github.com/python/cpython/blob/283de2b9c18e38c9a573526d6c398ade7dd6f8e9/Lib/curses/ascii.py#L56
 #
 # These two functions are released under the
@@ -43,36 +45,152 @@
     return retval
 
 
 def _isascii(c):
     return 0 <= _ctoi(c) <= 127
 
 
+def _extract_lines(input_file: str, start: int, end: int) -> str:
+    r"""Extract lines from file between start and end line numbers, with line numbers starting from 1."""
+    if start > end or start < 1 or end < 1:
+        raise ValueError
+
+    lines: list = list()
+    line_counter: int = 1
+
+    with open(input_file, 'r') as f:
+        line = f.readline()
+        while line:
+            if line_counter >= start and line_counter <= end:
+                lines.append(line)
+            line = f.readline()
+            line_counter += 1
+
+    return ''.join(lines)
+
+
+def _remove_line_intervals(filename: str, line_intervals: list):
+    # A nested list of integers divided in couples is expected.
+    # Example: [[1, 4], [8, 9]]
+    for interval in line_intervals:
+        if len(interval) != 2 or interval[0] < 1 or interval[
+                1] < 1 or interval[0] > interval[1]:
+            raise ValueError
+
+        fpyutils.filelines.remove_line_interval(
+            filename,
+            interval[0],
+            interval[1],
+            filename,
+        )
+
+
+def _get_existing_toc(filename: str, marker: str) -> tuple:
+    r"""Get the existing TOC in a file and return other important data about the TOC and its markers."""
+    # TOC marker positions.
+    marker_line_positions, lines = fpyutils.filelines.get_line_matches(
+        filename,
+        marker,
+        0,
+        loose_matching=True,
+        keep_all_lines=True,
+    )
+    marker_line_positions_length: int = len(marker_line_positions)
+
+    old_toc: str = str()
+    first_marker: int = 1
+    second_marker: int = 2
+    two_or_more_markers: bool = False
+    done: bool = False
+    first_marker_line_number: int = 0
+    lines_to_delete: list = list()
+
+    if marker_line_positions_length > 0:
+        first_marker_line_number = marker_line_positions[first_marker]
+
+    # Possible pre-existing TOC.
+    while not done and marker_line_positions_length >= 2:
+
+        interval: str = _read_line_interval(
+            lines, marker_line_positions[first_marker] + 1,
+            marker_line_positions[second_marker] - 1)
+
+        # Line intervals excluding the newline after the first <!--TOC-->
+        # and before the last <!--TOC-->.
+        interval_with_newline: str = _read_line_interval(
+            lines, marker_line_positions[first_marker] + 2,
+            marker_line_positions[second_marker] - 2)
+
+        # TODO: add code fence detection.
+        if _detect_toc_list(interval_with_newline) or _string_empty(interval):
+
+            # Skip the opening and closing TOC markers.
+            start_line: int = marker_line_positions[first_marker] + 1
+            end_line: int = marker_line_positions[second_marker] - 1
+
+            if start_line <= end_line:
+                # Real TOC detected.
+                old_toc = _extract_lines(filename, start_line,
+                                         end_line).strip()
+            else:
+                old_toc = str()
+
+            lines_to_delete.append([
+                marker_line_positions[first_marker],
+                marker_line_positions[second_marker]
+            ])
+
+            first_marker_line_number = marker_line_positions[first_marker]
+            done = True
+
+        first_marker += 1
+        second_marker += 1
+        marker_line_positions_length -= 1
+        two_or_more_markers = True
+
+    # Only 1 pre-existing marker. TOC is just the marker.
+    if not two_or_more_markers and marker_line_positions_length == 1:
+        old_toc = marker
+
+    return old_toc, lines_to_delete, two_or_more_markers, marker_line_positions_length, marker_line_positions, first_marker_line_number
+
+
 def _replace_substring(source: str, replacement: str, start: int,
                        end: int) -> str:
-    r"""Given a string called source, replace it with a string called replacement between the start ~ end interval."""
+    r"""Given a string called source, replace it with a string called replacement between the start and end indices interval."""
+    # Avoid possibility to pass lists to this function which the program would
+    # happily process.
+    if not isinstance(source, str):
+        raise TypeError
+    if not isinstance(replacement, str):
+        raise TypeError
+
+    if start > end:
+        raise ValueError
+
     replaced: list = list()
     replaced_str: str
     was_replaced: bool = False
     i: int = 0
 
     while i < len(source):
         if i < start or i > end:
             replaced.append(source[i])
         elif not was_replaced:
+            # Only one replacement is possible.
             replaced.append(replacement)
             was_replaced = True
         i += 1
 
     replaced_str = ''.join(replaced)
     return replaced_str
 
 
-# A weaker version of C's strncmp: this one does not count the characters
-# it just notify if there are differences.
+# A weaker version of C's strncmp: this one does not count the characters,
+# it just notifies if there are differences.
 def _strncmp(s1: str, s2: str, length: int) -> int:
     i: int = 0
     retval: int = 0
     process: bool = True
 
     s1_prime: str = s1[:length]
     s2_prime: str = s2[:length]
```

### Comparing `md_toc-8.1.9/md_toc.egg-info/PKG-INFO` & `md_toc-8.2.0/md_toc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md-toc
-Version: 8.1.9
+Version: 8.2.0
 Summary: Automatically generate and add an accurate table of contents to markdown files
 Home-page: https://blog.franco.net.eu.org/software/#md-toc
 Author: Franco Masotti
 Author-email: franco.masotti@tutanota.com
 License: GPLv3+,
 Keywords: markdown,toc,text,table-of-contents,documentation
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,15 +48,15 @@
   - [Changelog and trusted source](#changelog-and-trusted-source)
   - [Crypto donations](#crypto-donations)
 
 <!--TOC-->
 
 ## Video
 
-[![image](https://asciinema.org/a/452384.png)](https://asciinema.org/a/452384)
+[![image](./assets/md-toc_youtube_video_thumbnail.png)](https://www.youtube.com/watch?v=guyVdPNmC0A&t=49s)
 
 ## Description
 
 The table of contents (a.k.a: TOC) generated by this program is designed
 to work with several markdown parsers such as the ones used by GitHub
 and GitLab.
 
@@ -75,28 +75,29 @@
   called `Table of contents` to its Gitlab Flavored Mardown
 
 ## Features
 
 - works offline
 - edits file in place using a TOC marker (default `<!--TOC-->`) or
   output to standard output
-- selection of indentation level
+- maximum heading level selection (1 to 6)
 - list indentation based on heading, which can optionally be disabled
-- outputs an ordered or unordered TOC list
+- outputs an ordered or unordered TOC list with list marker selection
 - creates anchor links to markdown headings by default or a plain list
   as alternative
 - checks if heading level is coherent: this avoid creating an
   erroneous TOC. This feature can be disabled if needed
 - skip any number lines before generating the TOC
 - can read content from standard input
 - handles multiple files at once
 - selection of newline string
-- selection of list marker
+- check if there is difference between existing TOC in file and newly generated
+  one
 - supports GitHub, GitLab, Commonmark, Redcarpet and others
-- [pre-commit](https://pre-commit.com/)
+- [pre-commit](https://pre-commit.com/) md-toc
   [hook](https://docs.franco.net.eu.org/md-toc/pre_commit_hook.html)
 
 And more! See the
 [feature comparison table](https://docs.franco.net.eu.org/md-toc/features.html)
 
 ## Examples
```

### Comparing `md_toc-8.1.9/md_toc.egg-info/SOURCES.txt` & `md_toc-8.2.0/md_toc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `md_toc-8.1.9/setup.cfg` & `md_toc-8.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = md_toc
-version = 8.1.9
+version = 8.2.0
 license = GPLv3+,
 description = Automatically generate and add an accurate table of contents to markdown files
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Franco Masotti
 author_email = franco.masotti@tutanota.com
 keywords =
```

### Comparing `md_toc-8.1.9/setup.py` & `md_toc-8.2.0/setup.py`

 * *Files identical despite different names*

