# Comparing `tmp/ez_cqrs-2.5.1.tar.gz` & `tmp/ez_cqrs-2.5.2.tar.gz`

## Comparing `ez_cqrs-2.5.1.tar` & `ez_cqrs-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/ez_cqrs/components.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/ez_cqrs/error.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/ez_cqrs/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/ez_cqrs/py.typed
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/ez_cqrs/framework/__init__.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/ez_cqrs/framework/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/ez_cqrs/utilities/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/ez_cqrs/utilities/cli.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/requirements/core.txt
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/tests/conftest.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/tests/test_acid_exec.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/tests/test_framework.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/README.md
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/pyproject.toml
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/ez_cqrs/error.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/ez_cqrs/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/ez_cqrs/py.typed
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/ez_cqrs/framework/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/ez_cqrs/framework/testing.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/ez_cqrs/utils/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/ez_cqrs/utils/cli.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/ez_cqrs/utils/dates.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/ez_cqrs/utils/models.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/requirements/core.txt
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/tests/conftest.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/tests/test_acid_exec.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/tests/test_framework.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/README.md
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-2.5.2/PKG-INFO
```

### Comparing `ez_cqrs-2.5.1/.github/workflows/release.yml` & `ez_cqrs-2.5.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.5.1/.github/workflows/test.yml` & `ez_cqrs-2.5.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.5.1/.vscode/settings.json` & `ez_cqrs-2.5.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.5.1/ez_cqrs/acid_exec.py` & `ez_cqrs-2.5.2/ez_cqrs/acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.5.1/ez_cqrs/components.py` & `ez_cqrs-2.5.2/ez_cqrs/components.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.5.1/ez_cqrs/error.py` & `ez_cqrs-2.5.2/ez_cqrs/error.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.5.1/ez_cqrs/handler.py` & `ez_cqrs-2.5.2/ez_cqrs/handler.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.5.1/ez_cqrs/framework/__init__.py` & `ez_cqrs-2.5.2/ez_cqrs/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.5.1/ez_cqrs/framework/testing.py` & `ez_cqrs-2.5.2/ez_cqrs/framework/testing.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.5.1/ez_cqrs/utilities/cli.py` & `ez_cqrs-2.5.2/ez_cqrs/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.5.1/scripts/new_release.py` & `ez_cqrs-2.5.2/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.5.1/tests/conftest.py` & `ez_cqrs-2.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.5.1/tests/test_acid_exec.py` & `ez_cqrs-2.5.2/tests/test_acid_exec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 """Test ACID execution."""
 from __future__ import annotations
 
-from typing import Any
-
 import pytest
 
 from ez_cqrs.acid_exec import OpsRegistry
 
 
 @pytest.mark.unit()
 class TestOpsRegistry:
     """Test ops registry."""
 
     def test_is_empty(self) -> None:
         """Test ops registry is empty on creation."""
-        ops_registry = OpsRegistry[Any](max_lenght=1)
+        ops_registry = OpsRegistry[int](max_lenght=1)
         assert ops_registry.is_empty()
 
     def test_add(self) -> None:
         """Test adding values to ops registry."""
-        ops_registry = OpsRegistry[Any](max_lenght=1)
+        ops_registry = OpsRegistry[int](max_lenght=1)
         ops_registry.add(value=1)
         assert not ops_registry.is_empty()
         assert ops_registry.storage_length() == 1
 
     def test_prune_state(self) -> None:
         """Test prune state clears the storage."""
-        ops_registry = OpsRegistry[Any](max_lenght=1)
+        ops_registry = OpsRegistry[int](max_lenght=1)
         ops_registry.add(value=1)
         assert not ops_registry.is_empty()
         assert ops_registry.storage_length() == 1
         ops_registry.prune_storage()
         assert ops_registry.is_empty()
 
     def test_cannot_add_more_that_length(self) -> None:
         """Test adding more values that configured length."""
-        ops_registry = OpsRegistry[Any](max_lenght=0)
+        ops_registry = OpsRegistry[int](max_lenght=0)
         with pytest.raises(RuntimeError):
             ops_registry.add(value=1)
 
     def test_storage_snapshot_new_object(self) -> None:
         """Test get storage snapshot returns a new objected."""
-        ops_registry = OpsRegistry[Any](max_lenght=1)
+        ops_registry = OpsRegistry[int](max_lenght=1)
         ops_registry.add(value=1)
         snapshot = ops_registry.storage_snapshot()
         assert id(snapshot) != id(ops_registry.storage_length())
         snapshot.append(10)
         assert len(snapshot) != ops_registry.storage_length()
         assert not ops_registry.is_empty()
         assert ops_registry.storage_length() == 1
```

### Comparing `ez_cqrs-2.5.1/tests/test_framework.py` & `ez_cqrs-2.5.2/tests/test_framework.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.5.1/.gitignore` & `ez_cqrs-2.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.5.1/LICENSE` & `ez_cqrs-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.5.1/pyproject.toml` & `ez_cqrs-2.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "2.5.1"
+version = "2.5.2"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
```

### Comparing `ez_cqrs-2.5.1/PKG-INFO` & `ez_cqrs-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 2.5.1
+Version: 2.5.2
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

