# Comparing `tmp/openprotein_python-0.2.1.post1.tar.gz` & `tmp/openprotein_python-0.2.1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openprotein_python-0.2.1.post1.tar", max compression
+gzip compressed data, was "openprotein_python-0.2.1.post2.tar", max compression
```

## Comparing `openprotein_python-0.2.1.post1.tar` & `openprotein_python-0.2.1.post2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1543 2023-08-07 09:39:52.360055 openprotein_python-0.2.1.post1/LICENSE.txt
--rw-r--r--   0        0        0     4997 2023-08-07 09:51:46.711873 openprotein_python-0.2.1.post1/README.md
--rw-r--r--   0        0        0     2038 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post1/openprotein/__init__.py
--rw-r--r--   0        0        0      215 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post1/openprotein/_version.py
--rw-r--r--   0        0        0      127 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post1/openprotein/api/__init__.py
--rw-r--r--   0        0        0    13237 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post1/openprotein/api/data.py
--rw-r--r--   0        0        0     8533 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post1/openprotein/api/design.py
--rw-r--r--   0        0        0    22209 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post1/openprotein/api/embedding.py
--rw-r--r--   0        0        0    14511 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post1/openprotein/api/jobs.py
--rw-r--r--   0        0        0    41899 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post1/openprotein/api/poet.py
--rw-r--r--   0        0        0    17751 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post1/openprotein/api/predict.py
--rw-r--r--   0        0        0    19453 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post1/openprotein/api/train.py
--rw-r--r--   0        0        0     3069 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post1/openprotein/base.py
--rw-r--r--   0        0        0      170 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post1/openprotein/config.py
--rw-r--r--   0        0        0     1146 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post1/openprotein/errors.py
--rw-r--r--   0        0        0     1055 2023-08-04 09:17:01.541290 openprotein_python-0.2.1.post1/openprotein/fasta.py
--rw-r--r--   0        0        0     8620 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post1/openprotein/models.py
--rw-r--r--   0        0        0      601 2023-08-07 10:05:47.616391 openprotein_python-0.2.1.post1/pyproject.toml
--rw-r--r--   0        0        0     5781 1970-01-01 00:00:00.000000 openprotein_python-0.2.1.post1/PKG-INFO
+-rw-r--r--   0        0        0     1543 2023-08-07 09:39:52.360055 openprotein_python-0.2.1.post2/LICENSE.txt
+-rw-r--r--   0        0        0     4997 2023-08-07 10:27:49.587448 openprotein_python-0.2.1.post2/README.md
+-rw-r--r--   0        0        0     2038 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post2/openprotein/__init__.py
+-rw-r--r--   0        0        0      215 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post2/openprotein/_version.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post2/openprotein/api/__init__.py
+-rw-r--r--   0        0        0    13237 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post2/openprotein/api/data.py
+-rw-r--r--   0        0        0     8533 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post2/openprotein/api/design.py
+-rw-r--r--   0        0        0    22209 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post2/openprotein/api/embedding.py
+-rw-r--r--   0        0        0    14511 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post2/openprotein/api/jobs.py
+-rw-r--r--   0        0        0    41899 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post2/openprotein/api/poet.py
+-rw-r--r--   0        0        0    17751 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post2/openprotein/api/predict.py
+-rw-r--r--   0        0        0    19453 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post2/openprotein/api/train.py
+-rw-r--r--   0        0        0     3069 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post2/openprotein/base.py
+-rw-r--r--   0        0        0      170 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post2/openprotein/config.py
+-rw-r--r--   0        0        0     1146 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post2/openprotein/errors.py
+-rw-r--r--   0        0        0     1055 2023-08-04 09:17:01.541290 openprotein_python-0.2.1.post2/openprotein/fasta.py
+-rw-r--r--   0        0        0     8620 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post2/openprotein/models.py
+-rw-r--r--   0        0        0      601 2023-08-07 10:29:18.079921 openprotein_python-0.2.1.post2/pyproject.toml
+-rw-r--r--   0        0        0     5781 1970-01-01 00:00:00.000000 openprotein_python-0.2.1.post2/PKG-INFO
```

### Comparing `openprotein_python-0.2.1.post1/LICENSE.txt` & `openprotein_python-0.2.1.post2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1.post1/README.md` & `openprotein_python-0.2.1.post2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![PyPI version](https://badge.fury.io/py/openprotein-python.svg)](https://pypi.org/project/openprotein-python/)
 [![Coverage](https://dev.docs.openprotein.ai/api-python/_images/coverage.svg)](https://pypi.org/project/openprotein-python/)
-[![Conda version](https://anaconda.org/openprotein/openprotein_python/badges/version.svg)](https://anaconda.org/openprotein/openprotein_python)
+[![Conda version](https://anaconda.org/openprotein/openprotein-python/badges/version.svg)](https://anaconda.org/openprotein/openprotein-python)
 
 
 # openprotein-python
 The OpenProtein.AI Python Interface provides a user-friendly library to interact with the OpenProtein.AI REST API, enabling various tasks related to protein analysis and modeling.
 
 ## Installation
```

### Comparing `openprotein_python-0.2.1.post1/openprotein/__init__.py` & `openprotein_python-0.2.1.post2/openprotein/__init__.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1.post1/openprotein/api/data.py` & `openprotein_python-0.2.1.post2/openprotein/api/data.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1.post1/openprotein/api/design.py` & `openprotein_python-0.2.1.post2/openprotein/api/design.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1.post1/openprotein/api/embedding.py` & `openprotein_python-0.2.1.post2/openprotein/api/embedding.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1.post1/openprotein/api/jobs.py` & `openprotein_python-0.2.1.post2/openprotein/api/jobs.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1.post1/openprotein/api/poet.py` & `openprotein_python-0.2.1.post2/openprotein/api/poet.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1.post1/openprotein/api/predict.py` & `openprotein_python-0.2.1.post2/openprotein/api/predict.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1.post1/openprotein/api/train.py` & `openprotein_python-0.2.1.post2/openprotein/api/train.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1.post1/openprotein/base.py` & `openprotein_python-0.2.1.post2/openprotein/base.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1.post1/openprotein/errors.py` & `openprotein_python-0.2.1.post2/openprotein/errors.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1.post1/openprotein/fasta.py` & `openprotein_python-0.2.1.post2/openprotein/fasta.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1.post1/openprotein/models.py` & `openprotein_python-0.2.1.post2/openprotein/models.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1.post1/pyproject.toml` & `openprotein_python-0.2.1.post2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "openprotein_python"
 packages = [{include = "openprotein"}]
-version = "0.2.1.post1"
+version = "0.2.1.post2"
 description = "OpenProtein Python interface."
 license = "MIT"
 readme = "README.md"
 homepage = "https://docs.openprotein.ai/"
 authors = ["OpenProtein <info@ne47.bio>"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `openprotein_python-0.2.1.post1/PKG-INFO` & `openprotein_python-0.2.1.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openprotein-python
-Version: 0.2.1.post1
+Version: 0.2.1.post2
 Summary: OpenProtein Python interface.
 Home-page: https://docs.openprotein.ai/
 License: MIT
 Author: OpenProtein
 Author-email: info@ne47.bio
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,15 @@
 Requires-Dist: pydantic (>=1)
 Requires-Dist: requests (>=2)
 Requires-Dist: tqdm (>=4)
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/openprotein-python.svg)](https://pypi.org/project/openprotein-python/)
 [![Coverage](https://dev.docs.openprotein.ai/api-python/_images/coverage.svg)](https://pypi.org/project/openprotein-python/)
-[![Conda version](https://anaconda.org/openprotein/openprotein_python/badges/version.svg)](https://anaconda.org/openprotein/openprotein_python)
+[![Conda version](https://anaconda.org/openprotein/openprotein-python/badges/version.svg)](https://anaconda.org/openprotein/openprotein-python)
 
 
 # openprotein-python
 The OpenProtein.AI Python Interface provides a user-friendly library to interact with the OpenProtein.AI REST API, enabling various tasks related to protein analysis and modeling.
 
 ## Installation
```

