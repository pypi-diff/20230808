# Comparing `tmp/zep_python-1.0.tar.gz` & `tmp/zep_python-1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_python-1.0.tar", max compression
+gzip compressed data, was "zep_python-1.0b0.tar", max compression
```

## Comparing `zep_python-1.0.tar` & `zep_python-1.0b0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-08-08 04:19:03.921157 zep_python-1.0/LICENSE
--rw-r--r--   0        0        0      877 2023-08-08 04:19:03.921157 zep_python-1.0/README.md
--rw-r--r--   0        0        0     1072 2023-08-08 04:19:03.925157 zep_python-1.0/pyproject.toml
--rw-r--r--   0        0        0      952 2023-08-08 04:19:03.929157 zep_python-1.0/zep_python/__init__.py
--rw-r--r--   0        0        0      168 2023-08-08 04:19:03.929157 zep_python-1.0/zep_python/document/__init__.py
--rw-r--r--   0        0        0    13320 2023-08-08 04:19:03.929157 zep_python-1.0/zep_python/document/client.py
--rw-r--r--   0        0        0    18469 2023-08-08 04:19:03.929157 zep_python-1.0/zep_python/document/collections.py
--rw-r--r--   0        0        0     3764 2023-08-08 04:19:03.929157 zep_python-1.0/zep_python/document/models.py
--rw-r--r--   0        0        0     2608 2023-08-08 04:19:03.929157 zep_python-1.0/zep_python/exceptions.py
--rw-r--r--   0        0        0        0 2023-08-08 04:19:03.929157 zep_python-1.0/zep_python/experimental/__init__.py
--rw-r--r--   0        0        0       74 2023-08-08 04:19:03.929157 zep_python-1.0/zep_python/experimental/langchain/__init__.py
--rw-r--r--   0        0        0    20276 2023-08-08 04:19:03.929157 zep_python-1.0/zep_python/experimental/langchain/zep_vectorstore.py
--rw-r--r--   0        0        0      268 2023-08-08 04:19:03.929157 zep_python-1.0/zep_python/memory/__init__.py
--rw-r--r--   0        0        0    17816 2023-08-08 04:19:03.929157 zep_python-1.0/zep_python/memory/client.py
--rw-r--r--   0        0        0     5883 2023-08-08 04:19:03.929157 zep_python-1.0/zep_python/memory/models.py
--rw-r--r--   0        0        0        0 2023-08-08 04:19:03.929157 zep_python-1.0/zep_python/py.typed
--rw-r--r--   0        0        0      375 2023-08-08 04:19:03.929157 zep_python-1.0/zep_python/utils.py
--rw-r--r--   0        0        0     8486 2023-08-08 04:19:03.929157 zep_python-1.0/zep_python/zep_client.py
--rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 zep_python-1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-02 23:20:19.775943 zep_python-1.0b0/LICENSE
+-rw-r--r--   0        0        0      877 2023-08-02 23:20:19.775943 zep_python-1.0b0/README.md
+-rw-r--r--   0        0        0     1074 2023-08-02 23:20:19.779943 zep_python-1.0b0/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/__init__.py
+-rw-r--r--   0        0        0      168 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/document/__init__.py
+-rw-r--r--   0        0        0    13320 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/document/client.py
+-rw-r--r--   0        0        0    18469 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/document/collections.py
+-rw-r--r--   0        0        0     3764 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/document/models.py
+-rw-r--r--   0        0        0     2608 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/experimental/__init__.py
+-rw-r--r--   0        0        0       74 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/experimental/langchain/__init__.py
+-rw-r--r--   0        0        0    20276 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/experimental/langchain/zep_vectorstore.py
+-rw-r--r--   0        0        0      268 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/memory/__init__.py
+-rw-r--r--   0        0        0    17816 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/memory/client.py
+-rw-r--r--   0        0        0     5883 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/memory/models.py
+-rw-r--r--   0        0        0        0 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/py.typed
+-rw-r--r--   0        0        0      375 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/utils.py
+-rw-r--r--   0        0        0     8486 2023-08-02 23:20:19.779943 zep_python-1.0b0/zep_python/zep_client.py
+-rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 zep_python-1.0b0/PKG-INFO
```

### Comparing `zep_python-1.0/LICENSE` & `zep_python-1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `zep_python-1.0/README.md` & `zep_python-1.0b0/README.md`

 * *Files identical despite different names*

### Comparing `zep_python-1.0/pyproject.toml` & `zep_python-1.0b0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zep-python"
-version = "1.0"
+version = "1.0b0"
 description = "Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service."
 authors = ["Daniel Chalef <daniel.chalef@private.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9.0,<4"
 httpx = "^0.24.0"
```

### Comparing `zep_python-1.0/zep_python/__init__.py` & `zep_python-1.0b0/zep_python/__init__.py`

 * *Files identical despite different names*

### Comparing `zep_python-1.0/zep_python/document/client.py` & `zep_python-1.0b0/zep_python/document/client.py`

 * *Files identical despite different names*

### Comparing `zep_python-1.0/zep_python/document/collections.py` & `zep_python-1.0b0/zep_python/document/collections.py`

 * *Files identical despite different names*

### Comparing `zep_python-1.0/zep_python/document/models.py` & `zep_python-1.0b0/zep_python/document/models.py`

 * *Files identical despite different names*

### Comparing `zep_python-1.0/zep_python/exceptions.py` & `zep_python-1.0b0/zep_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `zep_python-1.0/zep_python/experimental/langchain/zep_vectorstore.py` & `zep_python-1.0b0/zep_python/experimental/langchain/zep_vectorstore.py`

 * *Files identical despite different names*

### Comparing `zep_python-1.0/zep_python/memory/client.py` & `zep_python-1.0b0/zep_python/memory/client.py`

 * *Files identical despite different names*

### Comparing `zep_python-1.0/zep_python/memory/models.py` & `zep_python-1.0b0/zep_python/memory/models.py`

 * *Files identical despite different names*

### Comparing `zep_python-1.0/zep_python/zep_client.py` & `zep_python-1.0b0/zep_python/zep_client.py`

 * *Files identical despite different names*

### Comparing `zep_python-1.0/PKG-INFO` & `zep_python-1.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zep-python
-Version: 1.0
+Version: 1.0b0
 Summary: Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service.
 Author: Daniel Chalef
 Author-email: daniel.chalef@private.org
 Requires-Python: >=3.9.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

