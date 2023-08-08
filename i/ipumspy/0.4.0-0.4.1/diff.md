# Comparing `tmp/ipumspy-0.4.0.tar.gz` & `tmp/ipumspy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipumspy-0.4.0.tar", max compression
+gzip compressed data, was "ipumspy-0.4.1.tar", max compression
```

## Comparing `ipumspy-0.4.0.tar` & `ipumspy-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    16725 2023-03-02 23:47:57.339161 ipumspy-0.4.0/LICENSE
--rw-r--r--   0        0        0     1875 2023-06-24 21:04:23.345033 ipumspy-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       96 2023-03-06 22:01:08.975231 ipumspy-0.4.0/src/ipumspy/__init__.py
--rw-r--r--   0        0        0      184 2023-03-06 17:17:16.405993 ipumspy-0.4.0/src/ipumspy/__version__.py
--rw-r--r--   0        0        0      119 2023-03-06 22:01:08.975231 ipumspy-0.4.0/src/ipumspy/api/__init__.py
--rw-r--r--   0        0        0    21466 2023-04-09 00:12:02.422109 ipumspy-0.4.0/src/ipumspy/api/core.py
--rw-r--r--   0        0        0     1108 2023-03-02 23:47:57.349161 ipumspy-0.4.0/src/ipumspy/api/exceptions.py
--rw-r--r--   0        0        0    25203 2023-04-09 00:12:02.422109 ipumspy-0.4.0/src/ipumspy/api/extract.py
--rw-r--r--   0        0        0     8789 2023-03-27 14:03:52.671184 ipumspy-0.4.0/src/ipumspy/cli.py
--rw-r--r--   0        0        0        0 2023-06-24 20:23:19.621594 ipumspy-0.4.0/src/ipumspy/data/__init__.py
--rw-r--r--   0        0        0    19106 2023-06-24 20:23:19.621594 ipumspy-0.4.0/src/ipumspy/data/nyts.yml.gz
--rw-r--r--   0        0        0    15040 2023-06-24 20:23:19.621594 ipumspy-0.4.0/src/ipumspy/data/yrbss.yml.gz
--rw-r--r--   0        0        0    14372 2023-06-24 20:23:19.621594 ipumspy-0.4.0/src/ipumspy/ddi.py
--rw-r--r--   0        0        0     6009 2023-03-02 23:47:57.349161 ipumspy-0.4.0/src/ipumspy/fileutils.py
--rw-r--r--   0        0        0     4073 2023-06-24 20:23:19.621594 ipumspy-0.4.0/src/ipumspy/noextract.py
--rw-r--r--   0        0        0    17990 2023-06-24 21:04:23.345033 ipumspy-0.4.0/src/ipumspy/readers.py
--rw-r--r--   0        0        0      348 2023-03-02 23:47:57.349161 ipumspy-0.4.0/src/ipumspy/types.py
--rw-r--r--   0        0        0     1236 2023-04-09 00:12:02.422109 ipumspy-0.4.0/src/ipumspy/utilities.py
--rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 ipumspy-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-03-02 23:47:57.339161 ipumspy-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1875 2023-08-08 15:23:32.054917 ipumspy-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-03-06 22:01:08.975231 ipumspy-0.4.1/src/ipumspy/__init__.py
+-rw-r--r--   0        0        0      184 2023-03-06 17:17:16.405993 ipumspy-0.4.1/src/ipumspy/__version__.py
+-rw-r--r--   0        0        0      119 2023-03-06 22:01:08.975231 ipumspy-0.4.1/src/ipumspy/api/__init__.py
+-rw-r--r--   0        0        0    21466 2023-04-09 00:12:02.422109 ipumspy-0.4.1/src/ipumspy/api/core.py
+-rw-r--r--   0        0        0     1108 2023-03-02 23:47:57.349161 ipumspy-0.4.1/src/ipumspy/api/exceptions.py
+-rw-r--r--   0        0        0    25203 2023-04-09 00:12:02.422109 ipumspy-0.4.1/src/ipumspy/api/extract.py
+-rw-r--r--   0        0        0     8789 2023-03-27 14:03:52.671184 ipumspy-0.4.1/src/ipumspy/cli.py
+-rw-r--r--   0        0        0        0 2023-06-24 20:23:19.621594 ipumspy-0.4.1/src/ipumspy/data/__init__.py
+-rw-r--r--   0        0        0    19106 2023-06-24 20:23:19.621594 ipumspy-0.4.1/src/ipumspy/data/nyts.yml.gz
+-rw-r--r--   0        0        0    15040 2023-06-24 20:23:19.621594 ipumspy-0.4.1/src/ipumspy/data/yrbss.yml.gz
+-rw-r--r--   0        0        0    14372 2023-06-24 20:23:19.621594 ipumspy-0.4.1/src/ipumspy/ddi.py
+-rw-r--r--   0        0        0     6009 2023-03-02 23:47:57.349161 ipumspy-0.4.1/src/ipumspy/fileutils.py
+-rw-r--r--   0        0        0     4073 2023-06-24 20:23:19.621594 ipumspy-0.4.1/src/ipumspy/noextract.py
+-rw-r--r--   0        0        0    17990 2023-06-24 21:04:23.345033 ipumspy-0.4.1/src/ipumspy/readers.py
+-rw-r--r--   0        0        0      348 2023-03-02 23:47:57.349161 ipumspy-0.4.1/src/ipumspy/types.py
+-rw-r--r--   0        0        0     1236 2023-04-09 00:12:02.422109 ipumspy-0.4.1/src/ipumspy/utilities.py
+-rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 ipumspy-0.4.1/PKG-INFO
```

### Comparing `ipumspy-0.4.0/LICENSE` & `ipumspy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipumspy-0.4.0/pyproject.toml` & `ipumspy-0.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipumspy"
-version = "0.4.0"
+version = "0.4.1"
 description = "A collection of tools for working with IPUMS data"
 authors = ["Kevin H. Wilson <kevin_wilson@brown.edu>",
            "Renae Rodgers <rodge103@umn.edu>"]
 license = "Mozilla Public License 2.0 (MPL 2.0)"
 packages = [
     { include = "ipumspy", from = "src" }
 ]
@@ -12,15 +12,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "^1.5.2"
 click = "^8.0.0"
 pyarrow = "^10.0.0"
 requests = {extras = ["use_chardet_on_py3"], version = "^2.26.0"}
 importlib-metadata = "^4.13.0"
-PyYAML = "^5.4.1"
+PyYAML = "^6.0.1"
 beautifulsoup4 = "^4.11.1"
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 pylint = "^2.7.4"
 isort = "^5.8.0"
 mypy = "^1.0.1"
```

### Comparing `ipumspy-0.4.0/src/ipumspy/api/core.py` & `ipumspy-0.4.1/src/ipumspy/api/core.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.4.0/src/ipumspy/api/exceptions.py` & `ipumspy-0.4.1/src/ipumspy/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.4.0/src/ipumspy/api/extract.py` & `ipumspy-0.4.1/src/ipumspy/api/extract.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.4.0/src/ipumspy/cli.py` & `ipumspy-0.4.1/src/ipumspy/cli.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.4.0/src/ipumspy/data/nyts.yml.gz` & `ipumspy-0.4.1/src/ipumspy/data/nyts.yml.gz`

 * *Files identical despite different names*

### Comparing `ipumspy-0.4.0/src/ipumspy/data/yrbss.yml.gz` & `ipumspy-0.4.1/src/ipumspy/data/yrbss.yml.gz`

 * *Files identical despite different names*

### Comparing `ipumspy-0.4.0/src/ipumspy/ddi.py` & `ipumspy-0.4.1/src/ipumspy/ddi.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.4.0/src/ipumspy/fileutils.py` & `ipumspy-0.4.1/src/ipumspy/fileutils.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.4.0/src/ipumspy/noextract.py` & `ipumspy-0.4.1/src/ipumspy/noextract.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.4.0/src/ipumspy/readers.py` & `ipumspy-0.4.1/src/ipumspy/readers.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.4.0/src/ipumspy/utilities.py` & `ipumspy-0.4.1/src/ipumspy/utilities.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.4.0/PKG-INFO` & `ipumspy-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ipumspy
-Version: 0.4.0
+Version: 0.4.1
 Summary: A collection of tools for working with IPUMS data
 License: Mozilla Public License 2.0 (MPL 2.0)
 Author: Kevin H. Wilson
 Author-email: kevin_wilson@brown.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
-Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
+Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: importlib-metadata (>=4.13.0,<5.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: pyarrow (>=10.0.0,<11.0.0)
 Requires-Dist: requests[use-chardet-on-py3] (>=2.26.0,<3.0.0)
```

