# Comparing `tmp/easy-google-docs-0.2.3.tar.gz` & `tmp/easy-google-docs-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easy-google-docs-0.2.3.tar", last modified: Tue Jul 26 19:17:27 2022, max compression
+gzip compressed data, was "easy-google-docs-0.2.4.tar", last modified: Tue Aug  8 16:49:52 2023, max compression
```

## Comparing `easy-google-docs-0.2.3.tar` & `easy-google-docs-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-07-26 19:17:27.000000 easy-google-docs-0.2.3/
--rw-r--r--   0 david      (501) staff       (20)      906 2022-07-26 19:17:27.000000 easy-google-docs-0.2.3/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)     4342 2020-12-14 17:55:11.000000 easy-google-docs-0.2.3/README.md
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-07-26 19:17:27.000000 easy-google-docs-0.2.3/easy_google_docs.egg-info/
--rw-r--r--   0 david      (501) staff       (20)      906 2022-07-26 19:17:27.000000 easy-google-docs-0.2.3/easy_google_docs.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      244 2022-07-26 19:17:27.000000 easy-google-docs-0.2.3/easy_google_docs.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2022-07-26 19:17:27.000000 easy-google-docs-0.2.3/easy_google_docs.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)       47 2022-07-26 19:17:27.000000 easy-google-docs-0.2.3/easy_google_docs.egg-info/requires.txt
--rw-r--r--   0 david      (501) staff       (20)       15 2022-07-26 19:17:27.000000 easy-google-docs-0.2.3/easy_google_docs.egg-info/top_level.txt
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-07-26 19:17:27.000000 easy-google-docs-0.2.3/easygoogledocs/
--rw-r--r--   0 david      (501) staff       (20)    32687 2022-07-26 19:17:02.000000 easy-google-docs-0.2.3/easygoogledocs/__init__.py
--rw-r--r--   0 david      (501) staff       (20)       38 2022-07-26 19:17:27.000000 easy-google-docs-0.2.3/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)     8146 2022-07-26 19:17:25.000000 easy-google-docs-0.2.3/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-08-08 16:49:52.508998 easy-google-docs-0.2.4/
+-rw-rw-r--   0 david     (1000) david     (1000)      850 2023-08-08 16:49:52.508998 easy-google-docs-0.2.4/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     4342 2023-08-08 16:48:19.000000 easy-google-docs-0.2.4/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-08-08 16:49:52.508998 easy-google-docs-0.2.4/easy_google_docs.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)      850 2023-08-08 16:49:52.000000 easy-google-docs-0.2.4/easy_google_docs.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      244 2023-08-08 16:49:52.000000 easy-google-docs-0.2.4/easy_google_docs.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-08-08 16:49:52.000000 easy-google-docs-0.2.4/easy_google_docs.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       47 2023-08-08 16:49:52.000000 easy-google-docs-0.2.4/easy_google_docs.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       15 2023-08-08 16:49:52.000000 easy-google-docs-0.2.4/easy_google_docs.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-08-08 16:49:52.508998 easy-google-docs-0.2.4/easygoogledocs/
+-rw-rw-r--   0 david     (1000) david     (1000)    32924 2023-08-08 16:48:51.000000 easy-google-docs-0.2.4/easygoogledocs/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-08-08 16:49:52.508998 easy-google-docs-0.2.4/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     8146 2023-08-08 16:49:05.000000 easy-google-docs-0.2.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `easy-google-docs-0.2.3/PKG-INFO` & `easy-google-docs-0.2.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: easy-google-docs
-Version: 0.2.3
+Version: 0.2.4
 Summary: Additional functionality for the google-api-python-client centered around Google Docs and Google Sheets
 Home-page: https://github.com/david-pettifor-nd/easy-google-docs
 Author: David W Pettifor
 Author-email: David.W.Pettifor.1@nd.edu
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/david-pettifor-nd/easy-google-docs/issues
 Project-URL: Source, https://github.com/david-pettifor-nd/easy-google-docs
-Description: UNKNOWN
 Keywords: google api sheets docs
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
```

### Comparing `easy-google-docs-0.2.3/README.md` & `easy-google-docs-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `easy-google-docs-0.2.3/easy_google_docs.egg-info/PKG-INFO` & `easy-google-docs-0.2.4/easy_google_docs.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: easy-google-docs
-Version: 0.2.3
+Version: 0.2.4
 Summary: Additional functionality for the google-api-python-client centered around Google Docs and Google Sheets
 Home-page: https://github.com/david-pettifor-nd/easy-google-docs
 Author: David W Pettifor
 Author-email: David.W.Pettifor.1@nd.edu
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/david-pettifor-nd/easy-google-docs/issues
 Project-URL: Source, https://github.com/david-pettifor-nd/easy-google-docs
-Description: UNKNOWN
 Keywords: google api sheets docs
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
```

### Comparing `easy-google-docs-0.2.3/easygoogledocs/__init__.py` & `easy-google-docs-0.2.4/easygoogledocs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,16 +375,20 @@
             workbook = openpyxl.load_workbook(filename=fh)
             wb_sheet = None
             if tab_index != None:
                 wb_sheet = workbook.worksheets[tab_index]
             else:
                 wb_sheet = workbook[tab_name]
             
-            csv_file = open(os.path.join(download_location, os.path.basename(output_file)+'.csv'), 'w')
-            csv_writer = csv.writer(csv_file)
+            if format == FORMAT_TSV:
+                csv_file = open(os.path.join(download_location, os.path.basename(output_file)+'.tsv'), 'w')
+                csv_writer = csv.writer(csv_file, delimiter='\t')
+            else:
+                csv_file = open(os.path.join(download_location, os.path.basename(output_file)+'.csv'), 'w')
+                csv_writer = csv.writer(csv_file)
             for row in wb_sheet.iter_rows():
                 csv_row = []
                 for cell in row:
                     csv_row.append(cell.value)
                 csv_writer.writerow(csv_row)
             csv_file.close()
```

### Comparing `easy-google-docs-0.2.3/setup.py` & `easy-google-docs-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.2.3',  # Required
+    version='0.2.4',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Additional functionality for the google-api-python-client '
                 'centered around Google Docs and Google Sheets',  # Required
```

