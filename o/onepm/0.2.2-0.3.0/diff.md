# Comparing `tmp/onepm-0.2.2.tar.gz` & `tmp/onepm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onepm-0.2.2.tar", last modified: Tue Jul 26 03:49:05 2022, max compression
+gzip compressed data, was "onepm-0.3.0.tar", last modified: Tue Aug  8 03:11:52 2023, max compression
```

## Comparing `onepm-0.2.2.tar` & `onepm-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-07-26 03:48:53.049716 onepm-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-07-26 03:48:53.049716 onepm-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-07-26 03:48:53.049716 onepm-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-07-26 03:48:53.049716 onepm-0.2.2/src/onepm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-07-26 03:48:53.049716 onepm-0.2.2/src/onepm/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-07-26 03:48:53.049716 onepm-0.2.2/src/onepm/pdm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2262 2022-07-26 03:48:53.049716 onepm-0.2.2/src/onepm/pip.py
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-07-26 03:48:53.049716 onepm-0.2.2/src/onepm/pipenv.py
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-07-26 03:48:53.049716 onepm-0.2.2/src/onepm/poetry.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 03:48:53.049716 onepm-0.2.2/src/onepm/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-07-26 03:48:53.049716 onepm-0.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-07-26 03:48:53.049716 onepm-0.2.2/tests/test_pdm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2531 2022-07-26 03:48:53.049716 onepm-0.2.2/tests/test_pip.py
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-07-26 03:48:53.049716 onepm-0.2.2/tests/test_pipenv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-07-26 03:48:53.049716 onepm-0.2.2/tests/test_poetry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-07-26 03:48:53.049716 onepm-0.2.2/tests/test_utils.py
--rw-------   0 runner    (1001) docker     (121)     3029 2022-07-26 03:49:05.789746 onepm-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-08 03:11:34.435997 onepm-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1603 2023-08-08 03:11:34.435997 onepm-0.3.0/README.md
+-rw-r--r--   0        0        0     1023 2023-08-08 03:11:52.200246 onepm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1669 2023-08-08 03:11:34.435997 onepm-0.3.0/src/onepm/__init__.py
+-rw-r--r--   0        0        0     1879 2023-08-08 03:11:34.435997 onepm-0.3.0/src/onepm/base.py
+-rw-r--r--   0        0        0      709 2023-08-08 03:11:34.435997 onepm-0.3.0/src/onepm/pdm.py
+-rw-r--r--   0        0        0     2411 2023-08-08 03:11:34.435997 onepm-0.3.0/src/onepm/pip.py
+-rw-r--r--   0        0        0      557 2023-08-08 03:11:34.435997 onepm-0.3.0/src/onepm/pipenv.py
+-rw-r--r--   0        0        0      683 2023-08-08 03:11:34.435997 onepm-0.3.0/src/onepm/poetry.py
+-rw-r--r--   0        0        0        0 2023-08-08 03:11:34.435997 onepm-0.3.0/src/onepm/py.typed
+-rw-r--r--   0        0        0     1400 2023-08-08 03:11:34.435997 onepm-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     1140 2023-08-08 03:11:34.435997 onepm-0.3.0/tests/test_pdm.py
+-rw-r--r--   0        0        0     2371 2023-08-08 03:11:34.435997 onepm-0.3.0/tests/test_pip.py
+-rw-r--r--   0        0        0      929 2023-08-08 03:11:34.435997 onepm-0.3.0/tests/test_pipenv.py
+-rw-r--r--   0        0        0     1053 2023-08-08 03:11:34.435997 onepm-0.3.0/tests/test_poetry.py
+-rw-r--r--   0        0        0     1048 2023-08-08 03:11:34.435997 onepm-0.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2309 1970-01-01 00:00:00.000000 onepm-0.3.0/PKG-INFO
```

### Comparing `onepm-0.2.2/LICENSE` & `onepm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onepm-0.2.2/README.md` & `onepm-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `onepm-0.2.2/pyproject.toml` & `onepm-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
-version = "0.2.2"
+version = "0.3.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/frostming/onepm"
 Changelog = "https://github.com/frostming/onepm/releases"
@@ -40,10 +40,10 @@
 [tool.pdm.dev-dependencies]
 test = [
     "pytest>=7.1.2",
 ]
 
 [build-system]
 requires = [
-    "pdm-pep517>=0.12.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
```

### Comparing `onepm-0.2.2/src/onepm/__init__.py` & `onepm-0.3.0/src/onepm/__init__.py`

 * *Files identical despite different names*

### Comparing `onepm-0.2.2/src/onepm/base.py` & `onepm-0.3.0/src/onepm/base.py`

 * *Files identical despite different names*

### Comparing `onepm-0.2.2/src/onepm/pdm.py` & `onepm-0.3.0/src/onepm/pdm.py`

 * *Files identical despite different names*

### Comparing `onepm-0.2.2/src/onepm/pip.py` & `onepm-0.3.0/src/onepm/pip.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import os
 import sys
-from typing import NoReturn, Optional, List
+from typing import List, NoReturn, Optional
 
 from onepm.base import PackageManager
 
 
 class Pip(PackageManager):
     name = "pip"
 
     def _ensure_virtualenv(self) -> str:
-        if "VIRTUAL_ENV" in os.environ:
-            return os.environ["VIRTUAL_ENV"]
         this_venv = os.path.abspath(".venv")
         if os.path.exists(this_venv) and os.path.exists(
             os.path.join(this_venv, "pyvenv.cfg")
         ):
             return this_venv
-        raise Exception(
-            "To use pip, you must activate a virtualenv or create one at `.venv`."
-        )
+        if "VIRTUAL_ENV" in os.environ:
+            return os.environ["VIRTUAL_ENV"]
+
+        try:
+            import venv
+        except ImportError:
+            raise Exception(
+                "To use pip, you must activate a virtualenv or create one at `.venv`."
+            )
+        venv.create(this_venv, with_pip=True)
+        return this_venv
 
     def _find_requirements_txt(self) -> Optional[str]:
         for filename in ["requirements.txt", "requirements.in"]:
             if os.path.exists(filename):
                 return filename
         return None
```

### Comparing `onepm-0.2.2/src/onepm/pipenv.py` & `onepm-0.3.0/src/onepm/pipenv.py`

 * *Files identical despite different names*

### Comparing `onepm-0.2.2/src/onepm/poetry.py` & `onepm-0.3.0/src/onepm/poetry.py`

 * *Files identical despite different names*

### Comparing `onepm-0.2.2/tests/conftest.py` & `onepm-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `onepm-0.2.2/tests/test_pdm.py` & `onepm-0.3.0/tests/test_pdm.py`

 * *Files identical despite different names*

### Comparing `onepm-0.2.2/tests/test_pip.py` & `onepm-0.3.0/tests/test_pip.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import sys
 
 import pytest
-from onepm import pi, pr, pa, pu, pun
+from onepm import pa, pi, pr, pu, pun
 from onepm.pip import Pip
 
 pytestmark = pytest.mark.usefixtures("pip")
 
 
 @pytest.fixture
 def venv(monkeypatch):
     monkeypatch.setenv("VIRTUAL_ENV", "foo")
 
 
-def test_pip_detect_activated_venv(venv):
+def test_pip_detect_activated_venv(venv, project):
     pm = Pip()
     if sys.platform == "win32":
         assert pm.command == ["foo\\Scripts\\python.exe", "-m", "pip"]
     else:
         assert pm.command == ["foo/bin/python", "-m", "pip"]
 
 
@@ -35,21 +35,14 @@
         assert pm.command == [
             os.path.join(project, ".venv", "bin", "python"),
             "-m",
             "pip",
         ]
 
 
-def test_pip_no_venv_error(project):
-    with pytest.raises(
-        Exception, match="To use pip, you must activate a virtualenv or create one"
-    ):
-        pi([])
-
-
 def test_install_without_args_error(project, venv):
     with pytest.raises(
         Exception, match="No requirements.txt or setup.py/pyproject.toml is found"
     ):
         pi([])
```

### Comparing `onepm-0.2.2/tests/test_pipenv.py` & `onepm-0.3.0/tests/test_pipenv.py`

 * *Files identical despite different names*

### Comparing `onepm-0.2.2/tests/test_poetry.py` & `onepm-0.3.0/tests/test_poetry.py`

 * *Files identical despite different names*

### Comparing `onepm-0.2.2/tests/test_utils.py` & `onepm-0.3.0/tests/test_utils.py`

 * *Files identical despite different names*

