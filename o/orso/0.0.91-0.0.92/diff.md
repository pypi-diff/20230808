# Comparing `tmp/orso-0.0.91.tar.gz` & `tmp/orso-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orso-0.0.91.tar", last modified: Wed Aug  2 20:33:31 2023, max compression
+gzip compressed data, was "orso-0.0.92.tar", last modified: Tue Aug  8 20:47:18 2023, max compression
```

## Comparing `orso-0.0.91.tar` & `orso-0.0.92.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:33:31.483908 orso-0.0.91/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-08-02 20:33:17.000000 orso-0.0.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-02 20:33:31.483908 orso-0.0.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-08-02 20:33:17.000000 orso-0.0.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:33:31.475907 orso-0.0.91/orso/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-02 20:33:17.000000 orso-0.0.91/orso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:33:31.475907 orso-0.0.91/orso/bitarray/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 20:33:17.000000 orso-0.0.91/orso/bitarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   375496 2023-08-02 20:33:17.000000 orso-0.0.91/orso/bitarray/cbitarray.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:33:31.479907 orso-0.0.91/orso/cityhash/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 20:33:17.000000 orso-0.0.91/orso/cityhash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19319 2023-08-02 20:33:17.000000 orso-0.0.91/orso/cityhash/city.cc
--rw-r--r--   0 runner    (1001) docker     (123)   237362 2023-08-02 20:33:17.000000 orso-0.0.91/orso/cityhash/cityhash.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-08-02 20:33:17.000000 orso-0.0.91/orso/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14589 2023-08-02 20:33:17.000000 orso-0.0.91/orso/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-08-02 20:33:17.000000 orso-0.0.91/orso/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-08-02 20:33:17.000000 orso-0.0.91/orso/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:33:31.479907 orso-0.0.91/orso/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-02 20:33:17.000000 orso-0.0.91/orso/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-08-02 20:33:17.000000 orso-0.0.91/orso/filters/bloom_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-08-02 20:33:17.000000 orso-0.0.91/orso/filters/cuckoo_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:33:31.479907 orso-0.0.91/orso/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-02 20:33:17.000000 orso-0.0.91/orso/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-08-02 20:33:17.000000 orso-0.0.91/orso/logging/add_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-02 20:33:17.000000 orso-0.0.91/orso/logging/create_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-08-02 20:33:17.000000 orso-0.0.91/orso/logging/google_cloud_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-08-02 20:33:17.000000 orso-0.0.91/orso/logging/levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-08-02 20:33:17.000000 orso-0.0.91/orso/logging/log_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:33:31.479907 orso-0.0.91/orso/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 20:33:17.000000 orso-0.0.91/orso/profiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:33:31.479907 orso-0.0.91/orso/profiler/distogram/
--rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-08-02 20:33:17.000000 orso-0.0.91/orso/profiler/distogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-08-02 20:33:17.000000 orso-0.0.91/orso/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-08-02 20:33:17.000000 orso-0.0.91/orso/row.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-08-02 20:33:17.000000 orso-0.0.91/orso/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-08-02 20:33:17.000000 orso-0.0.91/orso/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-02 20:33:17.000000 orso-0.0.91/orso/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-02 20:33:17.000000 orso-0.0.91/orso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:33:31.475907 orso-0.0.91/orso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-02 20:33:31.000000 orso-0.0.91/orso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-02 20:33:31.000000 orso-0.0.91/orso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:33:31.000000 orso-0.0.91/orso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 20:33:31.000000 orso-0.0.91/orso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 20:33:31.000000 orso-0.0.91/orso.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-02 20:33:17.000000 orso-0.0.91/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:33:31.483908 orso-0.0.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-02 20:33:17.000000 orso-0.0.91/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:33:31.483908 orso-0.0.91/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-02 20:33:17.000000 orso-0.0.91/tests/test_bitarray.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-02 20:33:17.000000 orso-0.0.91/tests/test_cityhash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-08-02 20:33:17.000000 orso-0.0.91/tests/test_converters_arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-02 20:33:17.000000 orso-0.0.91/tests/test_converters_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-02 20:33:17.000000 orso-0.0.91/tests/test_converters_polars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-08-02 20:33:17.000000 orso-0.0.91/tests/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-02 20:33:17.000000 orso-0.0.91/tests/test_fetching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-02 20:33:17.000000 orso-0.0.91/tests/test_filter_bloom_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-02 20:33:17.000000 orso-0.0.91/tests/test_filter_cuckoo_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-02 20:33:17.000000 orso-0.0.91/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-02 20:33:17.000000 orso-0.0.91/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-08-02 20:33:17.000000 orso-0.0.91/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-08-02 20:33:17.000000 orso-0.0.91/tests/test_schema_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-02 20:33:17.000000 orso-0.0.91/tests/test_single_item_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-02 20:33:17.000000 orso-0.0.91/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:47:18.900457 orso-0.0.92/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-08-08 20:46:59.000000 orso-0.0.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-08 20:47:18.900457 orso-0.0.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-08-08 20:46:59.000000 orso-0.0.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:47:18.892457 orso-0.0.92/orso/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-08 20:46:59.000000 orso-0.0.92/orso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:47:18.892457 orso-0.0.92/orso/bitarray/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 20:46:59.000000 orso-0.0.92/orso/bitarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   375496 2023-08-08 20:46:59.000000 orso-0.0.92/orso/bitarray/cbitarray.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:47:18.892457 orso-0.0.92/orso/cityhash/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-08 20:46:59.000000 orso-0.0.92/orso/cityhash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19319 2023-08-08 20:46:59.000000 orso-0.0.92/orso/cityhash/city.cc
+-rw-r--r--   0 runner    (1001) docker     (123)   237362 2023-08-08 20:46:59.000000 orso-0.0.92/orso/cityhash/cityhash.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-08-08 20:46:59.000000 orso-0.0.92/orso/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14589 2023-08-08 20:46:59.000000 orso-0.0.92/orso/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-08-08 20:46:59.000000 orso-0.0.92/orso/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-08 20:46:59.000000 orso-0.0.92/orso/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:47:18.892457 orso-0.0.92/orso/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-08 20:46:59.000000 orso-0.0.92/orso/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-08-08 20:46:59.000000 orso-0.0.92/orso/filters/bloom_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-08-08 20:46:59.000000 orso-0.0.92/orso/filters/cuckoo_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:47:18.896457 orso-0.0.92/orso/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-08 20:46:59.000000 orso-0.0.92/orso/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-08-08 20:46:59.000000 orso-0.0.92/orso/logging/add_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-08 20:46:59.000000 orso-0.0.92/orso/logging/create_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-08-08 20:46:59.000000 orso-0.0.92/orso/logging/google_cloud_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-08-08 20:46:59.000000 orso-0.0.92/orso/logging/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-08-08 20:46:59.000000 orso-0.0.92/orso/logging/log_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:47:18.896457 orso-0.0.92/orso/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 20:46:59.000000 orso-0.0.92/orso/profiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:47:18.896457 orso-0.0.92/orso/profiler/distogram/
+-rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-08-08 20:46:59.000000 orso-0.0.92/orso/profiler/distogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-08-08 20:46:59.000000 orso-0.0.92/orso/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-08-08 20:46:59.000000 orso-0.0.92/orso/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-08-08 20:46:59.000000 orso-0.0.92/orso/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-08-08 20:46:59.000000 orso-0.0.92/orso/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-08 20:46:59.000000 orso-0.0.92/orso/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-08 20:46:59.000000 orso-0.0.92/orso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:47:18.892457 orso-0.0.92/orso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-08 20:47:18.000000 orso-0.0.92/orso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-08 20:47:18.000000 orso-0.0.92/orso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:47:18.000000 orso-0.0.92/orso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 20:47:18.000000 orso-0.0.92/orso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 20:47:18.000000 orso-0.0.92/orso.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-08 20:46:59.000000 orso-0.0.92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 20:47:18.900457 orso-0.0.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-08 20:46:59.000000 orso-0.0.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:47:18.896457 orso-0.0.92/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-08 20:46:59.000000 orso-0.0.92/tests/test_bitarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-08 20:46:59.000000 orso-0.0.92/tests/test_cityhash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-08-08 20:46:59.000000 orso-0.0.92/tests/test_converters_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-08 20:46:59.000000 orso-0.0.92/tests/test_converters_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-08 20:46:59.000000 orso-0.0.92/tests/test_converters_polars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-08-08 20:46:59.000000 orso-0.0.92/tests/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-08 20:46:59.000000 orso-0.0.92/tests/test_fetching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-08 20:46:59.000000 orso-0.0.92/tests/test_filter_bloom_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-08 20:46:59.000000 orso-0.0.92/tests/test_filter_cuckoo_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-08 20:46:59.000000 orso-0.0.92/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-08 20:46:59.000000 orso-0.0.92/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-08-08 20:46:59.000000 orso-0.0.92/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-08-08 20:46:59.000000 orso-0.0.92/tests/test_schema_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-08 20:46:59.000000 orso-0.0.92/tests/test_single_item_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-08 20:46:59.000000 orso-0.0.92/tests/test_types.py
```

### Comparing `orso-0.0.91/LICENSE` & `orso-0.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/PKG-INFO` & `orso-0.0.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orso
-Version: 0.0.91
+Version: 0.0.92
 Summary: 🐻 DataFrame Library
 Home-page: https://github.com/mabel-dev/orso/
 Author-email: justin.joyce@joocer.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
```

### Comparing `orso-0.0.91/README.md` & `orso-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/bitarray/cbitarray.c` & `orso-0.0.92/orso/bitarray/cbitarray.c`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/cityhash/city.cc` & `orso-0.0.92/orso/cityhash/city.cc`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/cityhash/cityhash.cpp` & `orso-0.0.92/orso/cityhash/cityhash.cpp`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/converters.py` & `orso-0.0.92/orso/converters.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/dataframe.py` & `orso-0.0.92/orso/dataframe.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/display.py` & `orso-0.0.92/orso/display.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/exceptions.py` & `orso-0.0.92/orso/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,7 +47,8 @@
         super().__init__(message)
 
 
 class ColumnDefinitionError(DataError):
     def __init__(self, attribute):
         self.attribute = attribute
         message = f"Column is missing attribute {attribute}"
+        super().__init__(message)
```

### Comparing `orso-0.0.91/orso/filters/bloom_filter.py` & `orso-0.0.92/orso/filters/bloom_filter.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/filters/cuckoo_filter.py` & `orso-0.0.92/orso/filters/cuckoo_filter.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/logging/add_level.py` & `orso-0.0.92/orso/logging/add_level.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/logging/create_logger.py` & `orso-0.0.92/orso/logging/create_logger.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/logging/google_cloud_logger.py` & `orso-0.0.92/orso/logging/google_cloud_logger.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/logging/levels.py` & `orso-0.0.92/orso/logging/levels.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/logging/log_formatter.py` & `orso-0.0.92/orso/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/profiler/distogram/__init__.py` & `orso-0.0.92/orso/profiler/distogram/__init__.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/profiler/profiler.py` & `orso-0.0.92/orso/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/row.py` & `orso-0.0.92/orso/row.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/schema.py` & `orso-0.0.92/orso/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,20 @@
                 warn("Column type LIST will be deprecated in a future version, use ARRAY instead.")
                 self.type = OrsoTypes.ARRAY
             elif type_name == "NUMERIC":
                 warn(
                     "Column type NUMERIC will be deprecated in a future version, use DECIMAL, DOUBLE or INTEGER instead. Mapped to DOUBLE, this may not be compatible with all values NUMERIC was compatible with."
                 )
                 self.type = OrsoTypes.DOUBLE
+            elif type_name == "STRING":
+                raise ValueError(
+                    f"Unknown column type '{self.type}' for column '{self.name}'. Did you mean 'VARCHAR'?"
+                )
             elif self.type != 0:
-                raise ValueError(f"Unknown column type {self.type} for column {self.name}")
+                raise ValueError(f"Unknown column type '{self.type}' for column '{self.name}'.")
 
     def __str__(self):
         return self.identity
 
     def materialize(self):
         raise TypeError("Cannot materialize FlatColumns")
```

### Comparing `orso-0.0.91/orso/tools.py` & `orso-0.0.92/orso/tools.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/types.py` & `orso-0.0.92/orso/types.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/orso/version.py` & `orso-0.0.92/orso/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__: str = "0.0.91"
+__version__: str = "0.0.92"
 __author__: str = "@joocer"
```

### Comparing `orso-0.0.91/orso.egg-info/PKG-INFO` & `orso-0.0.92/orso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orso
-Version: 0.0.91
+Version: 0.0.92
 Summary: 🐻 DataFrame Library
 Home-page: https://github.com/mabel-dev/orso/
 Author-email: justin.joyce@joocer.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
```

### Comparing `orso-0.0.91/orso.egg-info/SOURCES.txt` & `orso-0.0.92/orso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/setup.py` & `orso-0.0.92/setup.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/tests/test_bitarray.py` & `orso-0.0.92/tests/test_bitarray.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/tests/test_cityhash.py` & `orso-0.0.92/tests/test_cityhash.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/tests/test_converters_arrow.py` & `orso-0.0.92/tests/test_converters_arrow.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/tests/test_converters_pandas.py` & `orso-0.0.92/tests/test_converters_pandas.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/tests/test_converters_polars.py` & `orso-0.0.92/tests/test_converters_polars.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/tests/test_dataframe.py` & `orso-0.0.92/tests/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/tests/test_fetching.py` & `orso-0.0.92/tests/test_fetching.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/tests/test_filter_bloom_filter.py` & `orso-0.0.92/tests/test_filter_bloom_filter.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/tests/test_filter_cuckoo_filter.py` & `orso-0.0.92/tests/test_filter_cuckoo_filter.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/tests/test_profiler.py` & `orso-0.0.92/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/tests/test_random.py` & `orso-0.0.92/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/tests/test_schema.py` & `orso-0.0.92/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/tests/test_single_item_cache.py` & `orso-0.0.92/tests/test_single_item_cache.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.91/tests/test_types.py` & `orso-0.0.92/tests/test_types.py`

 * *Files identical despite different names*

