# Comparing `tmp/regex-2023.5.5.tar.gz` & `tmp/regex-2023.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex-2023.5.5.tar", last modified: Wed May  3 17:28:21 2023, max compression
+gzip compressed data, was "regex-2023.6.3.tar", last modified: Sat Jun  3 17:05:03 2023, max compression
```

## Comparing `regex-2023.5.5.tar` & `regex-2023.6.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:28:21.521021 regex-2023.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-05-03 17:28:20.000000 regex-2023.5.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-03 17:28:20.000000 regex-2023.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    40894 2023-05-03 17:28:21.521021 regex-2023.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39805 2023-05-03 17:28:20.000000 regex-2023.5.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:28:21.517021 regex-2023.5.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   143294 2023-05-03 17:28:20.000000 regex-2023.5.5/docs/Features.html
--rw-r--r--   0 runner    (1001) docker     (123)    29426 2023-05-03 17:28:20.000000 regex-2023.5.5/docs/UnicodeProperties.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 17:28:20.000000 regex-2023.5.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:28:21.517021 regex-2023.5.5/regex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40894 2023-05-03 17:28:21.000000 regex-2023.5.5/regex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-03 17:28:21.000000 regex-2023.5.5/regex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:28:21.000000 regex-2023.5.5/regex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 17:28:21.000000 regex-2023.5.5/regex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:28:21.521021 regex-2023.5.5/regex_3/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-03 17:28:20.000000 regex-2023.5.5/regex_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   824718 2023-05-03 17:28:20.000000 regex-2023.5.5/regex_3/_regex.c
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-03 17:28:20.000000 regex-2023.5.5/regex_3/_regex.h
--rw-r--r--   0 runner    (1001) docker     (123)   141150 2023-05-03 17:28:20.000000 regex-2023.5.5/regex_3/_regex_core.py
--rw-r--r--   0 runner    (1001) docker     (123)  1837887 2023-05-03 17:28:20.000000 regex-2023.5.5/regex_3/_regex_unicode.c
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-05-03 17:28:20.000000 regex-2023.5.5/regex_3/_regex_unicode.h
--rw-r--r--   0 runner    (1001) docker     (123)    32811 2023-05-03 17:28:20.000000 regex-2023.5.5/regex_3/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)   219546 2023-05-03 17:28:20.000000 regex-2023.5.5/regex_3/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 17:28:21.521021 regex-2023.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-03 17:28:20.000000 regex-2023.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:28:21.521021 regex-2023.5.5/tools/
--rw-r--r--   0 runner    (1001) docker     (123)    55247 2023-05-03 17:28:20.000000 regex-2023.5.5/tools/build_regex_unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:05:03.085785 regex-2023.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-06-03 17:05:01.000000 regex-2023.6.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-03 17:05:01.000000 regex-2023.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    40894 2023-06-03 17:05:03.081785 regex-2023.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39805 2023-06-03 17:05:01.000000 regex-2023.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:05:03.077785 regex-2023.6.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   143294 2023-06-03 17:05:01.000000 regex-2023.6.3/docs/Features.html
+-rw-r--r--   0 runner    (1001) docker     (123)    29426 2023-06-03 17:05:01.000000 regex-2023.6.3/docs/UnicodeProperties.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-03 17:05:01.000000 regex-2023.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:05:03.081785 regex-2023.6.3/regex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40894 2023-06-03 17:05:02.000000 regex-2023.6.3/regex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-03 17:05:03.000000 regex-2023.6.3/regex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:05:02.000000 regex-2023.6.3/regex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-03 17:05:02.000000 regex-2023.6.3/regex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:05:03.081785 regex-2023.6.3/regex_3/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-03 17:05:01.000000 regex-2023.6.3/regex_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   825160 2023-06-03 17:05:01.000000 regex-2023.6.3/regex_3/_regex.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-06-03 17:05:01.000000 regex-2023.6.3/regex_3/_regex.h
+-rw-r--r--   0 runner    (1001) docker     (123)   141150 2023-06-03 17:05:01.000000 regex-2023.6.3/regex_3/_regex_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1837887 2023-06-03 17:05:01.000000 regex-2023.6.3/regex_3/_regex_unicode.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-03 17:05:01.000000 regex-2023.6.3/regex_3/_regex_unicode.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32811 2023-06-03 17:05:01.000000 regex-2023.6.3/regex_3/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)   219948 2023-06-03 17:05:01.000000 regex-2023.6.3/regex_3/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 17:05:03.085785 regex-2023.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-03 17:05:01.000000 regex-2023.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:05:03.081785 regex-2023.6.3/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    55247 2023-06-03 17:05:01.000000 regex-2023.6.3/tools/build_regex_unicode.py
```

### Comparing `regex-2023.5.5/LICENSE.txt` & `regex-2023.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `regex-2023.5.5/PKG-INFO` & `regex-2023.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regex
-Version: 2023.5.5
+Version: 2023.6.3
 Summary: Alternative regular expression module, to replace re.
 Home-page: https://github.com/mrabarnett/mrab-regex
 Author: Matthew Barnett
 Author-email: regex@mrabarnett.plus.com
 License: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `regex-2023.5.5/README.rst` & `regex-2023.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `regex-2023.5.5/docs/Features.html` & `regex-2023.6.3/docs/Features.html`

 * *Files identical despite different names*

### Comparing `regex-2023.5.5/docs/UnicodeProperties.rst` & `regex-2023.6.3/docs/UnicodeProperties.rst`

 * *Files identical despite different names*

### Comparing `regex-2023.5.5/regex.egg-info/PKG-INFO` & `regex-2023.6.3/regex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regex
-Version: 2023.5.5
+Version: 2023.6.3
 Summary: Alternative regular expression module, to replace re.
 Home-page: https://github.com/mrabarnett/mrab-regex
 Author: Matthew Barnett
 Author-email: regex@mrabarnett.plus.com
 License: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `regex-2023.5.5/regex_3/_regex.c` & `regex-2023.6.3/regex_3/_regex.c`

 * *Files 0% similar despite different names*

```diff
@@ -287,14 +287,15 @@
 
 /* A pattern node. */
 typedef struct RE_Node {
     RE_NextNode next_1;
     union {
         struct {
             RE_NextNode next_2;
+            struct RE_Node* true_node; /* Used by a CONDITIONAL node. */
         } nonstring;
         struct {
             /* Used only if (node->status & RE_STATUS_STRING) is true. */
             Py_ssize_t* bad_character_offset;
             Py_ssize_t* good_suffix_offset;
         } string;
     };
@@ -15268,15 +15269,15 @@
                  * 'false' branch.
                  */
                 node = conditional->nonstring.next_2.node;
             else
                 /* It's a negative lookaround that's failed. Go to the 'true'
                  * branch.
                  */
-                node = conditional->next_1.node;
+                node = conditional->nonstring.true_node;
 
             goto advance;
         }
         case RE_OP_END_ATOMIC: /* End of an atomic group. */
             TRACE(("%s\n", re_op_text[op]))
 
             /* bstack: captures fuzzy_counts capture_change */
@@ -16986,15 +16987,14 @@
              * bstack: -
              *
              * pstack: -
              */
 
             if (!lookaround->match) {
                 /* It's a negative lookaround that's failed. */
-
                 node = lookaround->nonstring.next_2.node;
                 goto advance;
             }
             break;
         }
         case RE_OP_MATCH_BODY:
         {
@@ -22982,14 +22982,22 @@
             /* Check the second destination. */
             next = node->nonstring.next_2.node;
             if (next && next->op == RE_OP_BRANCH &&
               !next->nonstring.next_2.node) {
                 node->nonstring.next_2.node = next->next_1.node;
                 modified = TRUE;
             }
+
+            /* Check the true branch for CONDITIONAL. */
+            next = node->nonstring.true_node;
+            if (next && next->op == RE_OP_BRANCH &&
+              !next->nonstring.true_node) {
+                node->nonstring.true_node = next->next_1.node;
+                modified = TRUE;
+            }
         }
     } while (modified);
 
     /* The start node might be a 1-way branch. Skip over it because it'll be
      * removed. It might even be the first in a chain.
      */
     while (pattern->start_node->op == RE_OP_BRANCH &&
@@ -24439,14 +24447,15 @@
     end_node = create_node(args->pattern, RE_OP_BRANCH, 0, 0, 0);
     if (!end_node)
         return RE_ERROR_MEMORY;
 
     /* end test node -> true branch -> end node */
     add_node(end_test_node, subargs.start);
     add_node(subargs.end, end_node);
+    test_node->nonstring.true_node = subargs.start;
 
     if (args->code[0] == RE_OP_NEXT) {
         /* There's a false branch. */
         ++args->code;
 
         /* Compile the false branch. */
         subargs.code = args->code;
```

### Comparing `regex-2023.5.5/regex_3/_regex.h` & `regex-2023.6.3/regex_3/_regex.h`

 * *Files identical despite different names*

### Comparing `regex-2023.5.5/regex_3/_regex_core.py` & `regex-2023.6.3/regex_3/_regex_core.py`

 * *Files identical despite different names*

### Comparing `regex-2023.5.5/regex_3/_regex_unicode.c` & `regex-2023.6.3/regex_3/_regex_unicode.c`

 * *Files identical despite different names*

### Comparing `regex-2023.5.5/regex_3/_regex_unicode.h` & `regex-2023.6.3/regex_3/_regex_unicode.h`

 * *Files identical despite different names*

### Comparing `regex-2023.5.5/regex_3/regex.py` & `regex-2023.6.3/regex_3/regex.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
   "sub", "subf", "subfn", "subn", "template", "Scanner", "A", "ASCII", "B",
   "BESTMATCH", "D", "DEBUG", "E", "ENHANCEMATCH", "S", "DOTALL", "F",
   "FULLCASE", "I", "IGNORECASE", "L", "LOCALE", "M", "MULTILINE", "P", "POSIX",
   "R", "REVERSE", "T", "TEMPLATE", "U", "UNICODE", "V0", "VERSION0", "V1",
   "VERSION1", "X", "VERBOSE", "W", "WORD", "error", "Regex", "__version__",
   "__doc__", "RegexFlag"]
 
-__version__ = "2.5.128"
+__version__ = "2.5.129"
 
 # --------------------------------------------------------------------
 # Public interface.
 
 def match(pattern, string, flags=0, pos=None, endpos=None, partial=False,
   concurrent=None, timeout=None, ignore_unused=False, **kwargs):
     """Try to apply the pattern at the start of the string, returning a match
```

### Comparing `regex-2023.5.5/regex_3/test_regex.py` & `regex-2023.6.3/regex_3/test_regex.py`

 * *Files 0% similar despite different names*

```diff
@@ -4328,14 +4328,20 @@
         # Git issue 479: Segmentation fault when using conditional pattern
         self.assertEqual(regex.match(r'(?(?<=A)|(?(?![^B])C|D))', 'A'), None)
         self.assertEqual(regex.search(r'(?(?<=A)|(?(?![^B])C|D))', 'A').span(), (1, 1))
 
         # Git issue 494: Backtracking failure matching regex ^a?(a?)b?c\1$ against string abca
         self.assertEqual(regex.search(r"^a?(a?)b?c\1$", "abca").span(), (0, 4))
 
+        # Git issue 498: Conditional negative lookahead inside positive lookahead fails to match
+        self.assertEqual(regex.match(r"(?(?=a).|..)", "ab").span(), (0, 1))
+        self.assertEqual(regex.match(r"(?(?=b).|..)", "ab").span(), (0, 2))
+        self.assertEqual(regex.match(r"(?(?!a).|..)", "ab").span(), (0, 2))
+        self.assertEqual(regex.match(r"(?(?!b).|..)", "ab").span(), (0, 1))
+
     def test_fuzzy_ext(self):
         self.assertEqual(bool(regex.fullmatch(r'(?r)(?:a){e<=1:[a-z]}', 'e')),
           True)
         self.assertEqual(bool(regex.fullmatch(r'(?:a){e<=1:[a-z]}', 'e')),
           True)
         self.assertEqual(bool(regex.fullmatch(r'(?:a){e<=1:[a-z]}', '-')),
           False)
```

### Comparing `regex-2023.5.5/setup.py` & `regex-2023.6.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os.path import join
 
 with open('README.rst') as file:
     long_description = file.read()
 
 setup(
     name='regex',
-    version='2023.5.5',
+    version='2023.6.3',
     description='Alternative regular expression module, to replace re.',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Matthew Barnett',
     author_email='regex@mrabarnett.plus.com',
     url='https://github.com/mrabarnett/mrab-regex',
     license='Apache Software License',
```

### Comparing `regex-2023.5.5/tools/build_regex_unicode.py` & `regex-2023.6.3/tools/build_regex_unicode.py`

 * *Files identical despite different names*

