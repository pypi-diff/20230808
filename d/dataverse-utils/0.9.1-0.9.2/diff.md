# Comparing `tmp/dataverse_utils-0.9.1.tar.gz` & `tmp/dataverse_utils-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse_utils-0.9.1.tar", last modified: Thu Aug  3 21:31:42 2023, max compression
+gzip compressed data, was "dataverse_utils-0.9.2.tar", last modified: Fri Aug  4 21:47:57 2023, max compression
```

## Comparing `dataverse_utils-0.9.1.tar` & `dataverse_utils-0.9.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.118495 dataverse_utils-0.9.1/
--rw-r--r--   0 paul       (501) staff       (20)      144 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/.gitignore
--rw-r--r--   0 paul       (501) staff       (20)     1103 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/LICENCE.md
--rw-r--r--   0 paul       (501) staff       (20)     2052 2023-08-03 21:31:42.117746 dataverse_utils-0.9.1/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)     1163 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/README.md
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.087225 dataverse_utils-0.9.1/docs/
--rw-r--r--   0 paul       (501) staff       (20)    13561 2023-08-03 21:28:11.000000 dataverse_utils-0.9.1/docs/api_ref.md
--rw-r--r--   0 paul       (501) staff       (20)      383 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/docs/credits.md
--rw-r--r--   0 paul       (501) staff       (20)     2932 2021-08-09 17:51:55.000000 dataverse_utils-0.9.1/docs/faq.md
--rw-r--r--   0 paul       (501) staff       (20)     5840 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/docs/index.md
--rw-r--r--   0 paul       (501) staff       (20)    21852 2023-08-03 21:28:11.000000 dataverse_utils-0.9.1/docs/scripts.md
--rw-r--r--   0 paul       (501) staff       (20)     5748 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/docs/windows.md
--rw-r--r--   0 paul       (501) staff       (20)      396 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/mkdocs.yml
--rw-r--r--   0 paul       (501) staff       (20)     2605 2023-08-03 21:28:11.000000 dataverse_utils-0.9.1/pyproject.toml
--rw-r--r--   0 paul       (501) staff       (20)      240 2023-05-11 15:55:17.000000 dataverse_utils-0.9.1/requirements.txt
--rw-r--r--   0 paul       (501) staff       (20)       38 2023-08-03 21:31:42.118665 dataverse_utils-0.9.1/setup.cfg
--rw-r--r--   0 paul       (501) staff       (20)       84 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/setup.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.072110 dataverse_utils-0.9.1/src/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.092537 dataverse_utils-0.9.1/src/dataverse_utils/
--rw-r--r--   0 paul       (501) staff       (20)      253 2023-08-03 21:28:11.000000 dataverse_utils-0.9.1/src/dataverse_utils/__init__.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.099070 dataverse_utils-0.9.1/src/dataverse_utils/data/
--rw-r--r--   0 paul       (501) staff       (20)     1545 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/data/LDC_EULA_general.md
--rw-r--r--   0 paul       (501) staff       (20)    17617 2023-08-03 21:28:11.000000 dataverse_utils-0.9.1/src/dataverse_utils/dataverse_utils.py
--rw-r--r--   0 paul       (501) staff       (20)     7704 2023-08-03 21:28:11.000000 dataverse_utils-0.9.1/src/dataverse_utils/dvdata.py
--rw-r--r--   0 paul       (501) staff       (20)    16047 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/ldc.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.109862 dataverse_utils-0.9.1/src/dataverse_utils/scripts/
--rw-r--r--   0 paul       (501) staff       (20)     4965 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_del.py
--rw-r--r--   0 paul       (501) staff       (20)     5348 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_ldc_uploader.py
--rw-r--r--   0 paul       (501) staff       (20)     5366 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_manifest_gen.py
--rw-r--r--   0 paul       (501) staff       (20)     9076 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_pg_facet_date.py
--rw-r--r--   0 paul       (501) staff       (20)     4385 2023-08-03 21:28:11.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_record_copy.py
--rw-r--r--   0 paul       (501) staff       (20)     8071 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_release.py
--rw-r--r--   0 paul       (501) staff       (20)     4566 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_replace_licence.py
--rw-r--r--   0 paul       (501) staff       (20)     8782 2023-08-03 21:28:11.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_study_migrator.py
--rw-r--r--   0 paul       (501) staff       (20)     2975 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_upload_tsv.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.098008 dataverse_utils-0.9.1/src/dataverse_utils.egg-info/
--rw-r--r--   0 paul       (501) staff       (20)     2052 2023-08-03 21:31:41.000000 dataverse_utils-0.9.1/src/dataverse_utils.egg-info/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)     1101 2023-08-03 21:31:42.000000 dataverse_utils-0.9.1/src/dataverse_utils.egg-info/SOURCES.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2023-08-03 21:31:41.000000 dataverse_utils-0.9.1/src/dataverse_utils.egg-info/dependency_links.txt
--rw-r--r--   0 paul       (501) staff       (20)      641 2023-08-03 21:31:42.000000 dataverse_utils-0.9.1/src/dataverse_utils.egg-info/entry_points.txt
--rw-r--r--   0 paul       (501) staff       (20)      266 2023-08-03 21:31:42.000000 dataverse_utils-0.9.1/src/dataverse_utils.egg-info/requires.txt
--rw-r--r--   0 paul       (501) staff       (20)       16 2023-08-03 21:31:42.000000 dataverse_utils-0.9.1/src/dataverse_utils.egg-info/top_level.txt
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.111752 dataverse_utils-0.9.1/tests/
--rw-r--r--   0 paul       (501) staff       (20)        0 2021-08-09 17:51:55.000000 dataverse_utils-0.9.1/tests/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)     1124 2021-08-09 17:51:55.000000 dataverse_utils-0.9.1/tests/tests_dataverse_utils.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 21:31:42.116236 dataverse_utils-0.9.1/tmp/
--rw-r--r--   0 paul       (501) staff       (20)      324 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/tmp/requirements.txt
--rw-r--r--   0 paul       (501) staff       (20)     2493 2023-05-04 22:06:51.000000 dataverse_utils-0.9.1/tmp/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-04 21:47:57.045990 dataverse_utils-0.9.2/
+-rw-r--r--   0 paul       (501) staff       (20)      144 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/.gitignore
+-rw-r--r--   0 paul       (501) staff       (20)     1103 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/LICENCE.md
+-rw-r--r--   0 paul       (501) staff       (20)     2052 2023-08-04 21:47:57.045004 dataverse_utils-0.9.2/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)     1163 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/README.md
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-04 21:47:57.008715 dataverse_utils-0.9.2/docs/
+-rw-r--r--   0 paul       (501) staff       (20)    13561 2023-08-03 21:28:11.000000 dataverse_utils-0.9.2/docs/api_ref.md
+-rw-r--r--   0 paul       (501) staff       (20)      383 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/docs/credits.md
+-rw-r--r--   0 paul       (501) staff       (20)     2932 2021-08-09 17:51:55.000000 dataverse_utils-0.9.2/docs/faq.md
+-rw-r--r--   0 paul       (501) staff       (20)     5840 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/docs/index.md
+-rw-r--r--   0 paul       (501) staff       (20)    21852 2023-08-03 21:28:11.000000 dataverse_utils-0.9.2/docs/scripts.md
+-rw-r--r--   0 paul       (501) staff       (20)     5748 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/docs/windows.md
+-rw-r--r--   0 paul       (501) staff       (20)      396 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/mkdocs.yml
+-rw-r--r--   0 paul       (501) staff       (20)     2605 2023-08-03 21:28:11.000000 dataverse_utils-0.9.2/pyproject.toml
+-rw-r--r--   0 paul       (501) staff       (20)      240 2023-05-11 15:55:17.000000 dataverse_utils-0.9.2/requirements.txt
+-rw-r--r--   0 paul       (501) staff       (20)       38 2023-08-04 21:47:57.046174 dataverse_utils-0.9.2/setup.cfg
+-rw-r--r--   0 paul       (501) staff       (20)       84 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-04 21:47:56.990085 dataverse_utils-0.9.2/src/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-04 21:47:57.013098 dataverse_utils-0.9.2/src/dataverse_utils/
+-rw-r--r--   0 paul       (501) staff       (20)      253 2023-08-04 21:40:19.000000 dataverse_utils-0.9.2/src/dataverse_utils/__init__.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-04 21:47:57.023771 dataverse_utils-0.9.2/src/dataverse_utils/data/
+-rw-r--r--   0 paul       (501) staff       (20)     1545 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/src/dataverse_utils/data/LDC_EULA_general.md
+-rw-r--r--   0 paul       (501) staff       (20)    17617 2023-08-03 21:28:11.000000 dataverse_utils-0.9.2/src/dataverse_utils/dataverse_utils.py
+-rw-r--r--   0 paul       (501) staff       (20)     7704 2023-08-03 21:28:11.000000 dataverse_utils-0.9.2/src/dataverse_utils/dvdata.py
+-rw-r--r--   0 paul       (501) staff       (20)    16047 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/src/dataverse_utils/ldc.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-04 21:47:57.039923 dataverse_utils-0.9.2/src/dataverse_utils/scripts/
+-rw-r--r--   0 paul       (501) staff       (20)     4965 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_del.py
+-rw-r--r--   0 paul       (501) staff       (20)     5348 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_ldc_uploader.py
+-rw-r--r--   0 paul       (501) staff       (20)     5366 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_manifest_gen.py
+-rw-r--r--   0 paul       (501) staff       (20)     9076 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_pg_facet_date.py
+-rw-r--r--   0 paul       (501) staff       (20)     4385 2023-08-03 21:28:11.000000 dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_record_copy.py
+-rw-r--r--   0 paul       (501) staff       (20)     8071 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_release.py
+-rw-r--r--   0 paul       (501) staff       (20)     4566 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_replace_licence.py
+-rw-r--r--   0 paul       (501) staff       (20)    10457 2023-08-04 21:40:19.000000 dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_study_migrator.py
+-rw-r--r--   0 paul       (501) staff       (20)     2975 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_upload_tsv.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-04 21:47:57.022858 dataverse_utils-0.9.2/src/dataverse_utils.egg-info/
+-rw-r--r--   0 paul       (501) staff       (20)     2052 2023-08-04 21:47:56.000000 dataverse_utils-0.9.2/src/dataverse_utils.egg-info/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)     1101 2023-08-04 21:47:56.000000 dataverse_utils-0.9.2/src/dataverse_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-08-04 21:47:56.000000 dataverse_utils-0.9.2/src/dataverse_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 paul       (501) staff       (20)      641 2023-08-04 21:47:56.000000 dataverse_utils-0.9.2/src/dataverse_utils.egg-info/entry_points.txt
+-rw-r--r--   0 paul       (501) staff       (20)      266 2023-08-04 21:47:56.000000 dataverse_utils-0.9.2/src/dataverse_utils.egg-info/requires.txt
+-rw-r--r--   0 paul       (501) staff       (20)       16 2023-08-04 21:47:56.000000 dataverse_utils-0.9.2/src/dataverse_utils.egg-info/top_level.txt
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-04 21:47:57.041552 dataverse_utils-0.9.2/tests/
+-rw-r--r--   0 paul       (501) staff       (20)        0 2021-08-09 17:51:55.000000 dataverse_utils-0.9.2/tests/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)     1124 2021-08-09 17:51:55.000000 dataverse_utils-0.9.2/tests/tests_dataverse_utils.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-04 21:47:57.043734 dataverse_utils-0.9.2/tmp/
+-rw-r--r--   0 paul       (501) staff       (20)      324 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/tmp/requirements.txt
+-rw-r--r--   0 paul       (501) staff       (20)     2493 2023-05-04 22:06:51.000000 dataverse_utils-0.9.2/tmp/setup.py
```

### Comparing `dataverse_utils-0.9.1/LICENCE.md` & `dataverse_utils-0.9.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/PKG-INFO` & `dataverse_utils-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse_utils
-Version: 0.9.1
+Version: 0.9.2
 Summary: Utilities for the Dataverse data respository system
 Author-email: Paul Lesack <paul.lesack@ubc.ca>
 Project-URL: Homepage, https://ubc-library-rc.github.io/dataverse_utils
 Project-URL: Repository, https://github.com/ubc-library-rc/dataverse_utils.git
 Project-URL: Issue Tracker, https://github.com/ubc-library-rc/dataverse_utils/issues
 Keywords: Harvard Dataverse,Dataverse,research data management,data repository
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dataverse_utils-0.9.1/README.md` & `dataverse_utils-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/docs/api_ref.md` & `dataverse_utils-0.9.2/docs/api_ref.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/docs/faq.md` & `dataverse_utils-0.9.2/docs/faq.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/docs/index.md` & `dataverse_utils-0.9.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/docs/scripts.md` & `dataverse_utils-0.9.2/docs/scripts.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/docs/windows.md` & `dataverse_utils-0.9.2/docs/windows.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/pyproject.toml` & `dataverse_utils-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/src/dataverse_utils/data/LDC_EULA_general.md` & `dataverse_utils-0.9.2/src/dataverse_utils/data/LDC_EULA_general.md`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/src/dataverse_utils/dataverse_utils.py` & `dataverse_utils-0.9.2/src/dataverse_utils/dataverse_utils.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/src/dataverse_utils/dvdata.py` & `dataverse_utils-0.9.2/src/dataverse_utils/dvdata.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/src/dataverse_utils/ldc.py` & `dataverse_utils-0.9.2/src/dataverse_utils/ldc.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_del.py` & `dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_del.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_ldc_uploader.py` & `dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_ldc_uploader.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_manifest_gen.py` & `dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_manifest_gen.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_pg_facet_date.py` & `dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_pg_facet_date.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_record_copy.py` & `dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_record_copy.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_release.py` & `dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_release.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_replace_licence.py` & `dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_replace_licence.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/src/dataverse_utils/scripts/dv_upload_tsv.py` & `dataverse_utils-0.9.2/src/dataverse_utils/scripts/dv_upload_tsv.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/src/dataverse_utils.egg-info/PKG-INFO` & `dataverse_utils-0.9.2/src/dataverse_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-utils
-Version: 0.9.1
+Version: 0.9.2
 Summary: Utilities for the Dataverse data respository system
 Author-email: Paul Lesack <paul.lesack@ubc.ca>
 Project-URL: Homepage, https://ubc-library-rc.github.io/dataverse_utils
 Project-URL: Repository, https://github.com/ubc-library-rc/dataverse_utils.git
 Project-URL: Issue Tracker, https://github.com/ubc-library-rc/dataverse_utils/issues
 Keywords: Harvard Dataverse,Dataverse,research data management,data repository
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dataverse_utils-0.9.1/src/dataverse_utils.egg-info/SOURCES.txt` & `dataverse_utils-0.9.2/src/dataverse_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/src/dataverse_utils.egg-info/entry_points.txt` & `dataverse_utils-0.9.2/src/dataverse_utils.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/tests/tests_dataverse_utils.py` & `dataverse_utils-0.9.2/tests/tests_dataverse_utils.py`

 * *Files identical despite different names*

### Comparing `dataverse_utils-0.9.1/tmp/setup.py` & `dataverse_utils-0.9.2/tmp/setup.py`

 * *Files identical despite different names*

