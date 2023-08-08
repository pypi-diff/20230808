# Comparing `tmp/test-pypi-uploads-0.1.0rc3.tar.gz` & `tmp/test-pypi-uploads-0.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-pypi-uploads-0.1.0rc3.tar", last modified: Tue Aug  8 04:15:08 2023, max compression
+gzip compressed data, was "test-pypi-uploads-0.1.0rc4.tar", last modified: Tue Aug  8 04:17:52 2023, max compression
```

## Comparing `test-pypi-uploads-0.1.0rc3.tar` & `test-pypi-uploads-0.1.0rc4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 04:15:08.746658 test-pypi-uploads-0.1.0rc3/
--rw-r--r--   0 root         (0) root         (0)      558 2023-08-08 04:15:08.746658 test-pypi-uploads-0.1.0rc3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       32 2023-08-08 04:14:44.000000 test-pypi-uploads-0.1.0rc3/README.md
--rw-r--r--   0 root         (0) root         (0)      358 2023-08-08 04:15:03.000000 test-pypi-uploads-0.1.0rc3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 04:15:08.746658 test-pypi-uploads-0.1.0rc3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      905 2023-08-08 04:15:03.000000 test-pypi-uploads-0.1.0rc3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 04:15:08.746658 test-pypi-uploads-0.1.0rc3/test_pypi_uploads/
--rw-r--r--   0 root         (0) root         (0)       56 2023-08-08 03:58:09.000000 test-pypi-uploads-0.1.0rc3/test_pypi_uploads/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 04:15:08.746658 test-pypi-uploads-0.1.0rc3/test_pypi_uploads.egg-info/
--rw-r--r--   0 root         (0) root         (0)      558 2023-08-08 04:15:08.000000 test-pypi-uploads-0.1.0rc3/test_pypi_uploads.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-08-08 04:15:08.000000 test-pypi-uploads-0.1.0rc3/test_pypi_uploads.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 04:15:08.000000 test-pypi-uploads-0.1.0rc3/test_pypi_uploads.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-08-08 04:15:08.000000 test-pypi-uploads-0.1.0rc3/test_pypi_uploads.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 04:17:52.578648 test-pypi-uploads-0.1.0rc4/
+-rw-r--r--   0 root         (0) root         (0)      558 2023-08-08 04:17:52.578648 test-pypi-uploads-0.1.0rc4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       32 2023-08-08 04:14:44.000000 test-pypi-uploads-0.1.0rc4/README.md
+-rw-r--r--   0 root         (0) root         (0)      358 2023-08-08 04:16:48.000000 test-pypi-uploads-0.1.0rc4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 04:17:52.578648 test-pypi-uploads-0.1.0rc4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      905 2023-08-08 04:16:50.000000 test-pypi-uploads-0.1.0rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 04:17:52.578648 test-pypi-uploads-0.1.0rc4/test_pypi_uploads/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-08-08 03:58:09.000000 test-pypi-uploads-0.1.0rc4/test_pypi_uploads/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 04:17:52.578648 test-pypi-uploads-0.1.0rc4/test_pypi_uploads.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      558 2023-08-08 04:17:52.000000 test-pypi-uploads-0.1.0rc4/test_pypi_uploads.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-08-08 04:17:52.000000 test-pypi-uploads-0.1.0rc4/test_pypi_uploads.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 04:17:52.000000 test-pypi-uploads-0.1.0rc4/test_pypi_uploads.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-08 04:17:52.000000 test-pypi-uploads-0.1.0rc4/test_pypi_uploads.egg-info/top_level.txt
```

### Comparing `test-pypi-uploads-0.1.0rc3/PKG-INFO` & `test-pypi-uploads-0.1.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-pypi-uploads
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: Package for testing PyPi uploads.
 Author: angrybayblade
 License: MIT
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `test-pypi-uploads-0.1.0rc3/setup.py` & `test-pypi-uploads-0.1.0rc4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import find_packages, setup
 
 if __name__ == "__main__":
     setup(
         name="test-pypi-uploads",
         description="Package for testing PyPi uploads.",
-        version="0.1.0.rc3",
+        version="0.1.0.rc4",
         author="angrybayblade",
         long_description="Package for testing PyPi uploads.",
         long_description_content_type="text/markdown",
         packages=find_packages(include=["test_pypi_uploads*"]),
         classifiers=[
             "Operating System :: MacOS",
             "Operating System :: Microsoft",
```

### Comparing `test-pypi-uploads-0.1.0rc3/test_pypi_uploads.egg-info/PKG-INFO` & `test-pypi-uploads-0.1.0rc4/test_pypi_uploads.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-pypi-uploads
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: Package for testing PyPi uploads.
 Author: angrybayblade
 License: MIT
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.7
```

