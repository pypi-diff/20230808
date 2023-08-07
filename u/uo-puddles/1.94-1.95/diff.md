# Comparing `tmp/uo_puddles-1.94.tar.gz` & `tmp/uo_puddles-1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uo_puddles-1.94.tar", last modified: Fri Aug  4 19:01:15 2023, max compression
+gzip compressed data, was "uo_puddles-1.95.tar", last modified: Mon Aug  7 22:07:55 2023, max compression
```

## Comparing `uo_puddles-1.94.tar` & `uo_puddles-1.95.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:01:15.184880 uo_puddles-1.94/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-04 19:01:02.000000 uo_puddles-1.94/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-04 19:01:15.180879 uo_puddles-1.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 19:01:02.000000 uo_puddles-1.94/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 19:01:02.000000 uo_puddles-1.94/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 19:01:15.184880 uo_puddles-1.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-04 19:01:02.000000 uo_puddles-1.94/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:01:15.180879 uo_puddles-1.94/uo_puddles/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-04 19:01:02.000000 uo_puddles-1.94/uo_puddles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-08-04 19:01:02.000000 uo_puddles-1.94/uo_puddles/cis423.py
--rw-r--r--   0 runner    (1001) docker     (123)    26639 2023-08-04 19:01:02.000000 uo_puddles-1.94/uo_puddles/good_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)    24737 2023-08-04 19:01:02.000000 uo_puddles-1.94/uo_puddles/good_ai_22.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-08-04 19:01:02.000000 uo_puddles-1.94/uo_puddles/gremcat_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-08-04 19:01:02.000000 uo_puddles-1.94/uo_puddles/gremcat_oo.py
--rw-r--r--   0 runner    (1001) docker     (123)    21672 2023-08-04 19:01:02.000000 uo_puddles-1.94/uo_puddles/mlops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:01:15.180879 uo_puddles-1.94/uo_puddles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-04 19:01:15.000000 uo_puddles-1.94/uo_puddles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-04 19:01:15.000000 uo_puddles-1.94/uo_puddles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:01:15.000000 uo_puddles-1.94/uo_puddles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 19:01:15.000000 uo_puddles-1.94/uo_puddles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:07:55.361454 uo_puddles-1.95/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-07 22:07:46.000000 uo_puddles-1.95/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-07 22:07:55.361454 uo_puddles-1.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-07 22:07:46.000000 uo_puddles-1.95/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-07 22:07:46.000000 uo_puddles-1.95/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 22:07:55.361454 uo_puddles-1.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-07 22:07:46.000000 uo_puddles-1.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:07:55.361454 uo_puddles-1.95/uo_puddles/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-07 22:07:46.000000 uo_puddles-1.95/uo_puddles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-08-07 22:07:46.000000 uo_puddles-1.95/uo_puddles/cis423.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26639 2023-08-07 22:07:46.000000 uo_puddles-1.95/uo_puddles/good_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24737 2023-08-07 22:07:46.000000 uo_puddles-1.95/uo_puddles/good_ai_22.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-08-07 22:07:46.000000 uo_puddles-1.95/uo_puddles/gremcat_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-08-07 22:07:46.000000 uo_puddles-1.95/uo_puddles/gremcat_oo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-08-07 22:07:46.000000 uo_puddles-1.95/uo_puddles/mlops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:07:55.361454 uo_puddles-1.95/uo_puddles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-07 22:07:55.000000 uo_puddles-1.95/uo_puddles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-07 22:07:55.000000 uo_puddles-1.95/uo_puddles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 22:07:55.000000 uo_puddles-1.95/uo_puddles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 22:07:55.000000 uo_puddles-1.95/uo_puddles.egg-info/top_level.txt
```

### Comparing `uo_puddles-1.94/LICENSE.txt` & `uo_puddles-1.95/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.94/setup.py` & `uo_puddles-1.95/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="uo_puddles",
-    version="1.94",    #also change pypi_version variable at top of library
+    version="1.95",    #also change pypi_version variable at top of library
     author="Stephen Fickas",
     author_email="stephenfickas@gmail.com",
     description="for cis423 class",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `uo_puddles-1.94/uo_puddles/cis423.py` & `uo_puddles-1.95/uo_puddles/cis423.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.94/uo_puddles/good_ai.py` & `uo_puddles-1.95/uo_puddles/good_ai.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.94/uo_puddles/good_ai_22.py` & `uo_puddles-1.95/uo_puddles/good_ai_22.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.94/uo_puddles/gremcat_df.py` & `uo_puddles-1.95/uo_puddles/gremcat_df.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.94/uo_puddles/gremcat_oo.py` & `uo_puddles-1.95/uo_puddles/gremcat_oo.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.94/uo_puddles/mlops.py` & `uo_puddles-1.95/uo_puddles/mlops.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,16 +312,16 @@
 
   def transform(self, X):
     assert isinstance(X, pd.core.frame.DataFrame), f'{self.__class__.__name__}.transform expected Dataframe but got {type(X)} instead.'
     assert isinstance(self.iqr, float), f'NotFittedError: This {self.__class__.__name__} instance is not fitted yet. Call "fit" with appropriate arguments before using this estimator.'
     assert self.target_column in X.columns.to_list(), f'{self.__class__.__name__}.transform unrecognizable column {self.target_column}.'
 
     X_ = X.copy()
-    X_[self.target_column] -= med
-    X_[self.target_column] /= iqr
+    X_[self.target_column] -= self.med
+    X_[self.target_column] /= self.iqr
     return X_
 
   def fit_transform(self, X, y = None):
     self.fit(X,y)
     result = self.transform(X)
     return result
```

