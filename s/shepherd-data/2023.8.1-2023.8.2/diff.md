# Comparing `tmp/shepherd_data-2023.8.1.tar.gz` & `tmp/shepherd_data-2023.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_data-2023.8.1.tar", last modified: Mon Aug  7 13:55:33 2023, max compression
+gzip compressed data, was "shepherd_data-2023.8.2.tar", last modified: Tue Aug  8 09:07:29 2023, max compression
```

## Comparing `shepherd_data-2023.8.1.tar` & `shepherd_data-2023.8.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:33.541836 shepherd_data-2023.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-08-07 13:55:33.541836 shepherd_data-2023.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-08-07 13:55:33.541836 shepherd_data-2023.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:33.533836 shepherd_data-2023.8.1/shepherd_data/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/shepherd_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/shepherd_data/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/shepherd_data/debug_resampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/shepherd_data/ivonne.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/shepherd_data/mppt.py
--rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/shepherd_data/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:33.541836 shepherd_data-2023.8.1/shepherd_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-08-07 13:55:33.000000 shepherd_data-2023.8.1/shepherd_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-07 13:55:33.000000 shepherd_data-2023.8.1/shepherd_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:55:33.000000 shepherd_data-2023.8.1/shepherd_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-07 13:55:33.000000 shepherd_data-2023.8.1/shepherd_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-07 13:55:33.000000 shepherd_data-2023.8.1/shepherd_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 13:55:33.000000 shepherd_data-2023.8.1/shepherd_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:55:33.000000 shepherd_data-2023.8.1/shepherd_data.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:33.537836 shepherd_data-2023.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/tests/test_cli_downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/tests/test_cli_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/tests/test_cli_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/tests/test_cli_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/tests/test_ivonne.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-07 13:55:05.000000 shepherd_data-2023.8.1/tests/test_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:07:29.419007 shepherd_data-2023.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-08-08 09:07:29.419007 shepherd_data-2023.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-08-08 09:07:29.419007 shepherd_data-2023.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:07:29.419007 shepherd_data-2023.8.2/shepherd_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/shepherd_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/shepherd_data/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/shepherd_data/debug_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/shepherd_data/ivonne.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/shepherd_data/mppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/shepherd_data/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:07:29.419007 shepherd_data-2023.8.2/shepherd_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-08-08 09:07:29.000000 shepherd_data-2023.8.2/shepherd_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-08 09:07:29.000000 shepherd_data-2023.8.2/shepherd_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 09:07:29.000000 shepherd_data-2023.8.2/shepherd_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-08 09:07:29.000000 shepherd_data-2023.8.2/shepherd_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-08 09:07:29.000000 shepherd_data-2023.8.2/shepherd_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-08 09:07:29.000000 shepherd_data-2023.8.2/shepherd_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 09:07:29.000000 shepherd_data-2023.8.2/shepherd_data.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:07:29.419007 shepherd_data-2023.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/tests/test_cli_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/tests/test_cli_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/tests/test_cli_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/tests/test_cli_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/tests/test_ivonne.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-08 09:07:00.000000 shepherd_data-2023.8.2/tests/test_reader.py
```

### Comparing `shepherd_data-2023.8.1/PKG-INFO` & `shepherd_data-2023.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_data
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-data/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
```

### Comparing `shepherd_data-2023.8.1/README.md` & `shepherd_data-2023.8.2/README.md`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.8.1/setup.cfg` & `shepherd_data-2023.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.8.1/shepherd_data/cli.py` & `shepherd_data-2023.8.2/shepherd_data/cli.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.8.1/shepherd_data/debug_resampler.py` & `shepherd_data-2023.8.2/shepherd_data/debug_resampler.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.8.1/shepherd_data/ivonne.py` & `shepherd_data-2023.8.2/shepherd_data/ivonne.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.8.1/shepherd_data/mppt.py` & `shepherd_data-2023.8.2/shepherd_data/mppt.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.8.1/shepherd_data/reader.py` & `shepherd_data-2023.8.2/shepherd_data/reader.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.8.1/shepherd_data.egg-info/PKG-INFO` & `shepherd_data-2023.8.2/shepherd_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd-data
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-data/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
```

### Comparing `shepherd_data-2023.8.1/shepherd_data.egg-info/SOURCES.txt` & `shepherd_data-2023.8.2/shepherd_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.8.1/tests/conftest.py` & `shepherd_data-2023.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.8.1/tests/test_cli_downsample.py` & `shepherd_data-2023.8.2/tests/test_cli_downsample.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.8.1/tests/test_cli_extract.py` & `shepherd_data-2023.8.2/tests/test_cli_extract.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.8.1/tests/test_cli_plot.py` & `shepherd_data-2023.8.2/tests/test_cli_plot.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.8.1/tests/test_examples.py` & `shepherd_data-2023.8.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.8.1/tests/test_ivonne.py` & `shepherd_data-2023.8.2/tests/test_ivonne.py`

 * *Files identical despite different names*

