# Comparing `tmp/query_strings_parser-0.1.2.tar.gz` & `tmp/query_strings_parser-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "query_strings_parser-0.1.2.tar", last modified: Fri Jul 14 17:55:51 2023, max compression
+gzip compressed data, was "query_strings_parser-0.1.3.tar", last modified: Tue Aug  8 16:39:03 2023, max compression
```

## Comparing `query_strings_parser-0.1.2.tar` & `query_strings_parser-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 17:55:51.293203 query_strings_parser-0.1.2/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)    11357 2023-07-14 16:38:29.000000 query_strings_parser-0.1.2/LICENSE
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      340 2023-07-14 17:55:51.293203 query_strings_parser-0.1.2/PKG-INFO
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     5878 2023-07-14 17:27:48.000000 query_strings_parser-0.1.2/README.md
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      103 2023-07-14 17:55:51.293203 query_strings_parser-0.1.2/setup.cfg
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      415 2023-07-14 17:27:48.000000 query_strings_parser-0.1.2/setup.py
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 17:55:51.289203 query_strings_parser-0.1.2/src/
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 17:55:51.293203 query_strings_parser-0.1.2/src/query_strings_parser/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 16:38:29.000000 query_strings_parser-0.1.2/src/query_strings_parser/__init__.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3076 2023-07-14 17:27:48.000000 query_strings_parser-0.1.2/src/query_strings_parser/query_parser.py
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 17:55:51.293203 query_strings_parser-0.1.2/src/query_strings_parser.egg-info/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      340 2023-07-14 17:55:51.000000 query_strings_parser-0.1.2/src/query_strings_parser.egg-info/PKG-INFO
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      306 2023-07-14 17:55:51.000000 query_strings_parser-0.1.2/src/query_strings_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2023-07-14 17:55:51.000000 query_strings_parser-0.1.2/src/query_strings_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       21 2023-07-14 17:55:51.000000 query_strings_parser-0.1.2/src/query_strings_parser.egg-info/top_level.txt
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-08-08 16:39:03.293994 query_strings_parser-0.1.3/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)    11357 2023-08-08 16:31:24.000000 query_strings_parser-0.1.3/LICENSE
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      340 2023-08-08 16:39:03.297994 query_strings_parser-0.1.3/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     5878 2023-08-08 16:31:24.000000 query_strings_parser-0.1.3/README.md
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      103 2023-08-08 16:39:03.297994 query_strings_parser-0.1.3/setup.cfg
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      415 2023-08-08 16:36:21.000000 query_strings_parser-0.1.3/setup.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-08-08 16:39:03.293994 query_strings_parser-0.1.3/src/
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-08-08 16:39:03.293994 query_strings_parser-0.1.3/src/query_strings_parser/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        0 2023-08-08 16:31:24.000000 query_strings_parser-0.1.3/src/query_strings_parser/__init__.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3115 2023-08-08 16:36:21.000000 query_strings_parser-0.1.3/src/query_strings_parser/query_parser.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-08-08 16:39:03.293994 query_strings_parser-0.1.3/src/query_strings_parser.egg-info/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      340 2023-08-08 16:39:03.000000 query_strings_parser-0.1.3/src/query_strings_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      306 2023-08-08 16:39:03.000000 query_strings_parser-0.1.3/src/query_strings_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2023-08-08 16:39:03.000000 query_strings_parser-0.1.3/src/query_strings_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       21 2023-08-08 16:39:03.000000 query_strings_parser-0.1.3/src/query_strings_parser.egg-info/top_level.txt
```

### Comparing `query_strings_parser-0.1.2/LICENSE` & `query_strings_parser-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `query_strings_parser-0.1.2/README.md` & `query_strings_parser-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `query_strings_parser-0.1.2/src/query_strings_parser/query_parser.py` & `query_strings_parser-0.1.3/src/query_strings_parser/query_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     elif (value.find(":") != -1):
         return build_comparison_operator(value)
     return value
 
 
 def build_regex(value):
     value = re.sub(r"\*{2,}", "*", value)
+    value = re.sub(r"\+", "\+", value)
     value = add_accent_regex(value)
 
     result = {}
 
     if (not value.startswith("*") and value.endswith("*")):
         result["$regex"] = "^{}".format(value.replace("*", ""))
     elif (value.startswith("*") and not value.endswith("*")):
```

