# Comparing `tmp/openhexa.toolbox-0.1.4.tar.gz` & `tmp/openhexa.toolbox-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhexa.toolbox-0.1.4.tar", last modified: Wed Aug  2 13:02:00 2023, max compression
+gzip compressed data, was "openhexa.toolbox-0.1.5.tar", last modified: Tue Aug  8 12:19:25 2023, max compression
```

## Comparing `openhexa.toolbox-0.1.4.tar` & `openhexa.toolbox-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:02:00.911547 openhexa.toolbox-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-02 13:02:00.911547 openhexa.toolbox-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:02:00.907546 openhexa.toolbox-0.1.4/openhexa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:02:00.911547 openhexa.toolbox-0.1.4/openhexa/toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/openhexa/toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:02:00.911547 openhexa.toolbox-0.1.4/openhexa/toolbox/dhis2/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/openhexa/toolbox/dhis2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/openhexa/toolbox/dhis2/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29336 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/openhexa/toolbox/dhis2/dhis2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/openhexa/toolbox/dhis2/periods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:02:00.911547 openhexa.toolbox-0.1.4/openhexa.toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-02 13:02:00.000000 openhexa.toolbox-0.1.4/openhexa.toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-02 13:02:00.000000 openhexa.toolbox-0.1.4/openhexa.toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:02:00.000000 openhexa.toolbox-0.1.4/openhexa.toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-02 13:02:00.000000 openhexa.toolbox-0.1.4/openhexa.toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 13:02:00.000000 openhexa.toolbox-0.1.4/openhexa.toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 13:02:00.911547 openhexa.toolbox-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:02:00.911547 openhexa.toolbox-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 13:01:33.000000 openhexa.toolbox-0.1.4/tests/test_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:19:25.975348 openhexa.toolbox-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-08 12:18:55.000000 openhexa.toolbox-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-08 12:19:25.975348 openhexa.toolbox-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 12:18:55.000000 openhexa.toolbox-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:19:25.967348 openhexa.toolbox-0.1.5/openhexa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:19:25.971348 openhexa.toolbox-0.1.5/openhexa/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:18:55.000000 openhexa.toolbox-0.1.5/openhexa/toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:19:25.971348 openhexa.toolbox-0.1.5/openhexa/toolbox/dhis2/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-08 12:18:55.000000 openhexa.toolbox-0.1.5/openhexa/toolbox/dhis2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-08-08 12:18:55.000000 openhexa.toolbox-0.1.5/openhexa/toolbox/dhis2/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29384 2023-08-08 12:18:55.000000 openhexa.toolbox-0.1.5/openhexa/toolbox/dhis2/dhis2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-08-08 12:18:55.000000 openhexa.toolbox-0.1.5/openhexa/toolbox/dhis2/periods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:19:25.971348 openhexa.toolbox-0.1.5/openhexa.toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-08 12:19:25.000000 openhexa.toolbox-0.1.5/openhexa.toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-08 12:19:25.000000 openhexa.toolbox-0.1.5/openhexa.toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:19:25.000000 openhexa.toolbox-0.1.5/openhexa.toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-08 12:19:25.000000 openhexa.toolbox-0.1.5/openhexa.toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 12:19:25.000000 openhexa.toolbox-0.1.5/openhexa.toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-08 12:18:55.000000 openhexa.toolbox-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:19:25.975348 openhexa.toolbox-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:19:25.975348 openhexa.toolbox-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:18:55.000000 openhexa.toolbox-0.1.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:19:25.975348 openhexa.toolbox-0.1.5/tests/dhis2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-08-08 12:18:55.000000 openhexa.toolbox-0.1.5/tests/dhis2/test_dhis2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-08-08 12:18:55.000000 openhexa.toolbox-0.1.5/tests/dhis2/test_dhis2_periods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 12:18:55.000000 openhexa.toolbox-0.1.5/tests/test_lib.py
```

### Comparing `openhexa.toolbox-0.1.4/LICENSE` & `openhexa.toolbox-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.1.4/PKG-INFO` & `openhexa.toolbox-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.toolbox
-Version: 0.1.4
+Version: 0.1.5
 Summary: A set of tools to acquire & process data from various sources
 Author-email: Bluesquare <dev@bluesquarehub.com>
 Maintainer-email: Bluesquare <dev@bluesquarehub.com>
 License: MIT License
         
         Copyright (c) 2023 Bluesquare
```

### Comparing `openhexa.toolbox-0.1.4/openhexa/toolbox/dhis2/api.py` & `openhexa.toolbox-0.1.5/openhexa/toolbox/dhis2/api.py`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.1.4/openhexa/toolbox/dhis2/dhis2.py` & `openhexa.toolbox-0.1.5/openhexa/toolbox/dhis2/dhis2.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,16 @@
         cache_dir : str, optional
             Cache directory. Actual cache data will be stored under a sub-directory
             named after the DHIS2 instance domain.
         """
         self.api = Api(connection)
         if cache_dir:
             self.cache_dir = self.setup_cache(cache_dir)
+        else:
+            self.cache_dir = None
         self.meta = Metadata(self)
         self.version = self.meta.system_info().get("version")
         self.data_value_sets = DataValueSets(self)
         self.analytics = Analytics(self)
 
     def setup_cache(self, cache_dir: str):
         """Initialize diskcache."""
```

### Comparing `openhexa.toolbox-0.1.4/openhexa/toolbox/dhis2/periods.py` & `openhexa.toolbox-0.1.5/openhexa/toolbox/dhis2/periods.py`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.1.4/openhexa.toolbox.egg-info/PKG-INFO` & `openhexa.toolbox-0.1.5/openhexa.toolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.toolbox
-Version: 0.1.4
+Version: 0.1.5
 Summary: A set of tools to acquire & process data from various sources
 Author-email: Bluesquare <dev@bluesquarehub.com>
 Maintainer-email: Bluesquare <dev@bluesquarehub.com>
 License: MIT License
         
         Copyright (c) 2023 Bluesquare
```

### Comparing `openhexa.toolbox-0.1.4/pyproject.toml` & `openhexa.toolbox-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openhexa.toolbox"
-version = "0.1.4"
+version = "0.1.5"
 description = "A set of tools to acquire & process data from various sources"
-authors = [
-    { name = "Bluesquare", email = "dev@bluesquarehub.com"}
-]
-maintainers = [
-    { name = "Bluesquare", email = "dev@bluesquarehub.com" }
-]
+authors = [{ name = "Bluesquare", email = "dev@bluesquarehub.com" }]
+maintainers = [{ name = "Bluesquare", email = "dev@bluesquarehub.com" }]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent"
+    "Operating System :: OS Independent",
 ]
 requires-python = ">=3.8"
-dependencies = [
-    "requests",
-    "python-dateutil",
-    "pandas",
-    "polars",
-    "diskcache"
-]
+dependencies = ["requests", "python-dateutil", "pandas", "polars", "diskcache"]
 
 [project.optional-dependencies]
-dev = ["ruff~=0.0.278", "pytest~=7.3.0", "build~=0.10.0", "pytest-cov~=4.0.0" , "black~=23.7.0", "pre-commit"]
+dev = [
+    "ruff~=0.0.278",
+    "pytest~=7.3.0",
+    "build~=0.10.0",
+    "pytest-cov~=4.0.0",
+    "black~=23.7.0",
+    "pre-commit",
+    "responses",
+]
 
 [tool.setuptools.packages.find]
 where = ["."]
 namespaces = true
 
 [project.urls]
 "Homepage" = "https://github.com/blsq/openhexa-toolbox"
@@ -43,7 +41,10 @@
 line-length = 120
 
 [tool.ruff]
 line-length = 120
 
 [tool.ruff.pycodestyle]
 max-doc-length = 120
+
+[tool.pytest.ini_options]
+addopts = ["--import-mode=importlib"]
```

