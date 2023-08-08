# Comparing `tmp/buildstr-0.1.0.tar.gz` & `tmp/buildstr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildstr-0.1.0.tar", max compression
+gzip compressed data, was "buildstr-0.1.1.tar", max compression
```

## Comparing `buildstr-0.1.0.tar` & `buildstr-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      583 2023-03-15 17:42:18.383369 buildstr-0.1.0/LICENSE
--rw-r--r--   0        0        0      905 2023-03-15 18:23:09.467993 buildstr-0.1.0/README.md
--rw-r--r--   0        0        0     2771 2023-03-15 18:23:09.453929 buildstr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       52 2023-03-15 17:59:32.278796 buildstr-0.1.0/src/buildstr/__init__.py
--rw-r--r--   0        0        0     1807 2023-03-15 18:11:18.094379 buildstr-0.1.0/src/buildstr/builder.py
--rw-r--r--   0        0        0     2165 2023-03-15 18:23:09.477712 buildstr-0.1.0/src/buildstr/builder_test.py
--rw-r--r--   0        0        0     1695 1970-01-01 00:00:00.000000 buildstr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-03-15 17:42:18.383369 buildstr-0.1.1/LICENSE
+-rw-r--r--   0        0        0      905 2023-03-15 18:23:09.467993 buildstr-0.1.1/README.md
+-rw-r--r--   0        0        0     2834 2023-08-08 13:22:09.481547 buildstr-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       52 2023-03-15 17:59:32.278796 buildstr-0.1.1/src/buildstr/__init__.py
+-rw-r--r--   0        0        0     1833 2023-08-08 13:01:40.613824 buildstr-0.1.1/src/buildstr/builder.py
+-rw-r--r--   0        0        0     2165 2023-03-15 18:23:09.477712 buildstr-0.1.1/src/buildstr/builder_test.py
+-rw-r--r--   0        0        0     1880 2023-08-08 13:02:45.459033 buildstr-0.1.1/src/buildstr/builder_test_augass.py
+-rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 buildstr-0.1.1/PKG-INFO
```

### Comparing `buildstr-0.1.0/LICENSE` & `buildstr-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `buildstr-0.1.0/README.md` & `buildstr-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `buildstr-0.1.0/pyproject.toml` & `buildstr-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "buildstr"
-version = "0.1.0"
+version = "0.1.1"
 homepage = "https://github.com/abilian/buildstr"
 description = "Fancy Pythonic String Builder."
 authors = ["Abilian SAS <sf@abilian.com>"]
 readme = "README.md"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
@@ -21,24 +21,23 @@
 
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 ## Standard cruft
 abilian-devtools = "*"
 
-# Cruft (project templates management)
 cruft = "*"
 toml = "*"
-
 ## /standard cruft
 
+pyanalyze = "^0.9.0"
 
 
 [tool.isort]
 profile = "black"
 
 
 [build-system]
@@ -119,14 +118,15 @@
 ]
 # Add later: "ANN", "ERA"...
 
 ignore = [
     "S101",  # Use of `assert` detected
     "B019",  # Use of `functools.cache` on methods can lead to memory leaks
     "UP038", # Use `X | Y` in `isinstance` call instead of `(X, Y)`
+    "PLW2901", # `with` statement variable overwritten by assignment target
 ]
 
 
 [tool.pyright]
 exclude = [
     '.tox',
     '.nox',
```

### Comparing `buildstr-0.1.0/src/buildstr/builder.py` & `buildstr-0.1.1/src/buildstr/builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,15 @@
             self._items.extend(other)
         else:
             self._items.append(other)
 
         return self
 
     __ilshift__ = __lshift__
+    __iadd__ = __lshift__
 
     def __call__(self, *args, surround=None, separator=" ", name="sub"):
         root = self._get_root()
         parent = root._stack[-1] if root._stack else root
         sub_builder = Builder(
             *args, surround=surround, separator=separator, parent=parent, name=name
         )
```

### Comparing `buildstr-0.1.0/src/buildstr/builder_test.py` & `buildstr-0.1.1/src/buildstr/builder_test.py`

 * *Files identical despite different names*

### Comparing `buildstr-0.1.0/PKG-INFO` & `buildstr-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Metadata-Version: 2.1
 Name: buildstr
-Version: 0.1.0
+Version: 0.1.1
 Summary: Fancy Pythonic String Builder.
 Home-page: https://github.com/abilian/buildstr
 Author: Abilian SAS
 Author-email: sf@abilian.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # Fancy Pythonic String Builder
 
 [![image](https://img.shields.io/pypi/v/buildstr.svg)](https://pypi.python.org/pypi/buildstr)
 
 [![image](https://img.shields.io/travis/sfermigier/buildstr.svg)](https://travis-ci.com/sfermigier/buildstr)
```

