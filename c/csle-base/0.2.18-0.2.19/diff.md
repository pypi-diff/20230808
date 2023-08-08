# Comparing `tmp/csle_base-0.2.18.tar.gz` & `tmp/csle_base-0.2.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_base-0.2.18.tar", last modified: Fri Jul  7 12:46:44 2023, max compression
+gzip compressed data, was "csle_base-0.2.19.tar", last modified: Tue Aug  8 14:24:28 2023, max compression
```

## Comparing `csle_base-0.2.18.tar` & `csle_base-0.2.19.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-07-07 12:46:44.612839 csle_base-0.2.18/
--rw-r--r--   0 kimham     (501) staff       (20)      664 2023-07-07 12:46:44.612973 csle_base-0.2.18/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     3391 2023-06-28 07:40:45.000000 csle_base-0.2.18/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      670 2023-06-11 13:17:52.000000 csle_base-0.2.18/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1222 2023-07-07 12:46:44.613583 csle_base-0.2.18/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2023-06-11 13:17:52.000000 csle_base-0.2.18/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-07-07 12:46:44.604748 csle_base-0.2.18/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-07-07 12:46:44.610130 csle_base-0.2.18/src/csle_base/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2023-06-11 13:17:52.000000 csle_base-0.2.18/src/csle_base/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       23 2023-07-07 12:46:35.000000 csle_base-0.2.18/src/csle_base/__version__.py
--rw-r--r--   0 kimham     (501) staff       (20)      574 2023-06-16 06:45:51.000000 csle_base-0.2.18/src/csle_base/grpc_serializable.py
--rw-r--r--   0 kimham     (501) staff       (20)     1537 2023-06-11 13:17:52.000000 csle_base-0.2.18/src/csle_base/json_serializable.py
--rw-r--r--   0 kimham     (501) staff       (20)      713 2023-06-16 06:45:51.000000 csle_base-0.2.18/src/csle_base/kafka_serializable.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-07-07 12:46:44.612603 csle_base-0.2.18/src/csle_base.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      664 2023-07-07 12:46:44.000000 csle_base-0.2.18/src/csle_base.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      424 2023-07-07 12:46:44.000000 csle_base-0.2.18/src/csle_base.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-07-07 12:46:44.000000 csle_base-0.2.18/src/csle_base.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-07-07 09:36:52.000000 csle_base-0.2.18/src/csle_base.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      204 2023-07-07 12:46:44.000000 csle_base-0.2.18/src/csle_base.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       10 2023-07-07 12:46:44.000000 csle_base-0.2.18/src/csle_base.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-08-08 14:24:28.571495 csle_base-0.2.19/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      654 2023-08-08 14:24:28.571495 csle_base-0.2.19/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3597 2023-08-08 13:45:05.000000 csle_base-0.2.19/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      670 2023-08-08 13:59:17.000000 csle_base-0.2.19/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1560 2023-08-08 14:24:28.571495 csle_base-0.2.19/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_base-0.2.19/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-08-08 14:24:28.567495 csle_base-0.2.19/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-08-08 14:24:28.571495 csle_base-0.2.19/src/csle_base/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_base-0.2.19/src/csle_base/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       23 2023-08-08 14:24:23.000000 csle_base-0.2.19/src/csle_base/__version__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      574 2023-06-13 15:27:33.000000 csle_base-0.2.19/src/csle_base/grpc_serializable.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1591 2023-07-11 06:36:56.000000 csle_base-0.2.19/src/csle_base/json_serializable.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      713 2023-06-13 15:27:33.000000 csle_base-0.2.19/src/csle_base/kafka_serializable.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-08-08 14:24:28.571495 csle_base-0.2.19/src/csle_base.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      654 2023-08-08 14:24:28.000000 csle_base-0.2.19/src/csle_base.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      424 2023-08-08 14:24:28.000000 csle_base-0.2.19/src/csle_base.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-08-08 14:24:28.000000 csle_base-0.2.19/src/csle_base.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-10 13:43:53.000000 csle_base-0.2.19/src/csle_base.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      333 2023-08-08 14:24:28.000000 csle_base-0.2.19/src/csle_base.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       10 2023-08-08 14:24:28.000000 csle_base-0.2.19/src/csle_base.egg-info/top_level.txt
```

### Comparing `csle_base-0.2.18/PKG-INFO` & `csle_base-0.2.19/src/csle_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
-Name: csle_base
-Version: 0.2.18
+Name: csle-base
+Version: 0.2.19
 Summary: Library with base classes and definitions for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Provides-Extra: testing
-
-UNKNOWN
-
```

### Comparing `csle_base-0.2.18/README.md` & `csle_base-0.2.19/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,23 @@
 
 - Python 3.8+
 
 ## Development Requirements
 
 - Python 3.8+
 - `flake8` (for linting)
+- `flake8-rst-docstrings` (for linting docstrings)
 - `tox` (for automated testing)
 - `pytest` (for unit tests)
 - `pytest-cov` (for unit test coverage)
 - `mypy` (for static typing)
+- `types-paramiko` (for static typing)
+- `types-protobuf` (for static typing)
+- `types-requests` (for static typing)
+- `types-urllib3` (for static typing)
 - `sphinx` (for API documentation)
 - `sphinxcontrib-napoleon` (for API documentation)
 - `sphinx-rtd-theme` (for API documentation)
 - `pytest-mock` (for mocking tests)
 - `pytest-grpc` (for grpc tests)
 
 ## Installation
```

### Comparing `csle_base-0.2.18/pyproject.toml` & `csle_base-0.2.19/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools==62.0.0"]
+requires = ["setuptools==68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 addopts = "--cov=csle_base -p no:warnings"
 testpaths = [
     "tests",
 ]
```

### Comparing `csle_base-0.2.18/setup.cfg` & `csle_base-0.2.19/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -29,28 +29,37 @@
 
 [options.extras_require]
 testing = 
 	pytest>=6.0
 	pytest-cov>=2.0
 	pytest-mock>=3.6.0
 	pytest-grpc>=0.8.0
-	mypy>=1.3.0
+	mypy>=1.4.1
+	types-paramiko>=3.2.0.0
+	types-protobuf>=4.23.0.3
+	types-requests>=2.31.0.1
+	types-urllib3>=1.26.25.13
 	flake8>=3.9
+	flake8-rst-docstrings>=0.3.0
 	tox>=3.24
 	sphinx>=5.3.0
 	sphinxcontrib-napoleon>=0.7
 	sphinx-rtd-theme>=1.1.1
 	twine>=4.0.2
 	build>=0.10.0
 
 [options.package_data]
 csle_ryu = py.typed
 
 [flake8]
 max-line-length = 120
-exclude = .git,__pycache__,docs/source/conf.py,old,build,dist,*_pb2*,*init__*
+exclude = .git,__pycache__,docs/source/conf.py,old,build,dist,*_pb2*,*init__*,.tox
 ignore = E741, W503, W504, F821, W605
+rst-roles = class, func, ref
+rst-directives = envvar, exception
+rst-substitutions = version
+extend-ignore = D401, D400, D100, RST305, RST219, D205, D202, D200, D204, RST206, W293, D403, D402, RST306
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `csle_base-0.2.18/src/csle_base/grpc_serializable.py` & `csle_base-0.2.19/src/csle_base/grpc_serializable.py`

 * *Files identical despite different names*

### Comparing `csle_base-0.2.18/src/csle_base/json_serializable.py` & `csle_base-0.2.19/src/csle_base/json_serializable.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,16 @@
         :return: the converted instance
         """
         pass
 
     @abstractmethod
     def to_dict(self) -> Dict[str, Any]:
         """
+        Converts the object to a dict representation
+
         :return: a dict representation of the object
         """
         pass
 
     @staticmethod
     @abstractmethod
     def from_json_file(json_file_path: str) -> "JSONSerializable":
```

### Comparing `csle_base-0.2.18/src/csle_base/kafka_serializable.py` & `csle_base-0.2.19/src/csle_base/kafka_serializable.py`

 * *Files identical despite different names*

### Comparing `csle_base-0.2.18/src/csle_base.egg-info/PKG-INFO` & `csle_base-0.2.19/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
-Name: csle-base
-Version: 0.2.18
+Name: csle_base
+Version: 0.2.19
 Summary: Library with base classes and definitions for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Provides-Extra: testing
-
-UNKNOWN
-
```

