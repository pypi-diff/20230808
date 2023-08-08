# Comparing `tmp/thatway-0.1.0.tar.gz` & `tmp/thatway-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thatway-0.1.0.tar", last modified: Mon Aug  7 18:11:05 2023, max compression
+gzip compressed data, was "thatway-0.4.0.tar", last modified: Tue Aug  8 15:50:09 2023, max compression
```

## Comparing `thatway-0.1.0.tar` & `thatway-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-07 18:11:05.453171 thatway-0.1.0/
--rw-r--r--   0 jlorieau   (501) staff       (20)     1071 2023-08-07 18:07:13.000000 thatway-0.1.0/LICENSE
--rw-r--r--   0 jlorieau   (501) staff       (20)      416 2023-08-07 18:11:05.452804 thatway-0.1.0/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)       39 2023-08-07 18:07:13.000000 thatway-0.1.0/README.md
--rw-r--r--   0 jlorieau   (501) staff       (20)      738 2023-08-07 18:10:50.000000 thatway-0.1.0/pyproject.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-08-07 18:11:05.453282 thatway-0.1.0/setup.cfg
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-07 18:11:05.449026 thatway-0.1.0/tests/
--rw-r--r--   0 jlorieau   (501) staff       (20)      769 2023-08-07 18:08:32.000000 thatway-0.1.0/tests/test_config.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-07 18:11:05.450269 thatway-0.1.0/thatway/
--rw-r--r--   0 jlorieau   (501) staff       (20)       80 2023-08-07 18:07:13.000000 thatway-0.1.0/thatway/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     4726 2023-08-07 18:07:13.000000 thatway-0.1.0/thatway/config.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      785 2023-08-07 18:07:13.000000 thatway-0.1.0/thatway/test.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-07 18:11:05.452289 thatway-0.1.0/thatway.egg-info/
--rw-r--r--   0 jlorieau   (501) staff       (20)      416 2023-08-07 18:11:05.000000 thatway-0.1.0/thatway.egg-info/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)      261 2023-08-07 18:11:05.000000 thatway-0.1.0/thatway.egg-info/SOURCES.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-08-07 18:11:05.000000 thatway-0.1.0/thatway.egg-info/dependency_links.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)       57 2023-08-07 18:11:05.000000 thatway-0.1.0/thatway.egg-info/requires.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        8 2023-08-07 18:11:05.000000 thatway-0.1.0/thatway.egg-info/top_level.txt
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 15:50:09.352532 thatway-0.4.0/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1071 2023-08-07 18:07:13.000000 thatway-0.4.0/LICENSE
+-rw-r--r--   0 jlorieau   (501) staff       (20)      376 2023-08-08 15:50:09.352319 thatway-0.4.0/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)     5630 2023-08-08 15:49:41.000000 thatway-0.4.0/README.rst
+-rw-r--r--   0 jlorieau   (501) staff       (20)      818 2023-08-07 21:51:39.000000 thatway-0.4.0/pyproject.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-08-08 15:50:09.352596 thatway-0.4.0/setup.cfg
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 15:50:09.350189 thatway-0.4.0/tests/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6020 2023-08-08 15:17:21.000000 thatway-0.4.0/tests/test_base.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 15:50:09.350724 thatway-0.4.0/thatway/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      123 2023-08-08 15:46:14.000000 thatway-0.4.0/thatway/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)    11450 2023-08-08 14:44:07.000000 thatway-0.4.0/thatway/base.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 15:50:09.352031 thatway-0.4.0/thatway.egg-info/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      376 2023-08-08 15:50:09.000000 thatway-0.4.0/thatway.egg-info/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)      242 2023-08-08 15:50:09.000000 thatway-0.4.0/thatway.egg-info/SOURCES.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-08-08 15:50:09.000000 thatway-0.4.0/thatway.egg-info/dependency_links.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)       57 2023-08-08 15:50:09.000000 thatway-0.4.0/thatway.egg-info/requires.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        8 2023-08-08 15:50:09.000000 thatway-0.4.0/thatway.egg-info/top_level.txt
```

### Comparing `thatway-0.1.0/LICENSE` & `thatway-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thatway-0.1.0/pyproject.toml` & `thatway-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -26,7 +26,10 @@
 
 dev = [  # For development
     "pytest>=7.4",  # Testing framework
     "twine>=4.0",  # Manage package uploads
     "build",  # Manage package builds
     "black[d]",  # Code formatter
     ]
+
+[tool.pytest.ini_options]
+addopts = "--doctest-modules --doctest-glob='*.rst'"
```

