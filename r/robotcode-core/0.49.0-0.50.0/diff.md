# Comparing `tmp/robotcode_core-0.49.0.tar.gz` & `tmp/robotcode_core-0.50.0.tar.gz`

## Comparing `robotcode_core-0.49.0.tar` & `robotcode_core-0.50.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/__version__.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/async_cache.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/async_itertools.py
--rw-r--r--   0        0        0    21626 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/async_tools.py
--rw-r--r--   0        0        0    15582 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/dataclasses.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/event.py
--rw-r--r--   0        0        0    15851 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/logging.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/py.typed
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/types.py
--rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/uri.py
--rw-r--r--   0        0        0   233349 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/lsp/types.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/utils/debugpy.py
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/utils/glob_path.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/utils/inspect.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/utils/net.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/utils/path.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/utils/process.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/utils/safe_eval.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/src/robotcode/core/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/LICENSE.txt
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/README.md
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/pyproject.toml
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 robotcode_core-0.49.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/__version__.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/async_cache.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/async_itertools.py
+-rw-r--r--   0        0        0    21626 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/async_tools.py
+-rw-r--r--   0        0        0    15492 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/dataclasses.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/event.py
+-rw-r--r--   0        0        0    15851 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/logging.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/py.typed
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/types.py
+-rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/uri.py
+-rw-r--r--   0        0        0   233349 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/lsp/types.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/utils/debugpy.py
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/utils/glob_path.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/utils/inspect.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/utils/net.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/utils/path.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/utils/process.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/utils/safe_eval.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/src/robotcode/core/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/LICENSE.txt
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/README.md
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/pyproject.toml
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 robotcode_core-0.50.0/PKG-INFO
```

### Comparing `robotcode_core-0.49.0/src/robotcode/core/async_cache.py` & `robotcode_core-0.50.0/src/robotcode/core/async_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/src/robotcode/core/async_itertools.py` & `robotcode_core-0.50.0/src/robotcode/core/async_itertools.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/src/robotcode/core/async_tools.py` & `robotcode_core-0.50.0/src/robotcode/core/async_tools.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/src/robotcode/core/dataclasses.py` & `robotcode_core-0.50.0/src/robotcode/core/dataclasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,19 +101,14 @@
 @runtime_checkable
 class HasCaseDecoder(Protocol):
     @classmethod
     def _decode_case(cls, s: str) -> str:  # pragma: no cover
         ...
 
 
-@runtime_checkable
-class ConfigBase(HasCaseDecoder, HasCaseEncoder, Protocol):
-    pass
-
-
 _T = TypeVar("_T")
 
 
 class DefaultConfig:
     @classmethod
     def _encode_case(cls, s: str) -> str:
         return s
```

### Comparing `robotcode_core-0.49.0/src/robotcode/core/event.py` & `robotcode_core-0.50.0/src/robotcode/core/event.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/src/robotcode/core/logging.py` & `robotcode_core-0.50.0/src/robotcode/core/logging.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/src/robotcode/core/uri.py` & `robotcode_core-0.50.0/src/robotcode/core/uri.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/src/robotcode/core/lsp/types.py` & `robotcode_core-0.50.0/src/robotcode/core/lsp/types.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/src/robotcode/core/utils/debugpy.py` & `robotcode_core-0.50.0/src/robotcode/core/utils/debugpy.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/src/robotcode/core/utils/glob_path.py` & `robotcode_core-0.50.0/src/robotcode/core/utils/glob_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/src/robotcode/core/utils/inspect.py` & `robotcode_core-0.50.0/src/robotcode/core/utils/inspect.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import inspect
-from typing import Any, Callable, Coroutine, Iterator, List, Optional
+from typing import Any, Callable, Coroutine, Iterator, Optional
 
 
 def iter_methods(
     obj: Any, predicate: Optional[Callable[[Callable[..., Any]], bool]] = None
 ) -> Iterator[Callable[..., Any]]:
     is_cls = inspect.isclass(obj)
     cls = obj if is_cls else type(obj)
@@ -18,21 +18,14 @@
                 if not inspect.ismethod(m):
                     continue
 
             if predicate is None or predicate(m):
                 yield m
 
 
-def get_methods(
-    instance_or_type: Any,
-    predicate: Optional[Callable[[Callable[..., Any]], bool]] = None,
-) -> List[Callable[..., Any]]:
-    return list(iter_methods(instance_or_type, predicate))
-
-
 _lambda_type = type(lambda: 0)
 _lambda_name = (lambda: 0).__name__
 
 
 def is_lambda(v: Any) -> bool:
     return isinstance(v, _lambda_type) and v.__name__ == _lambda_name
```

### Comparing `robotcode_core-0.49.0/src/robotcode/core/utils/net.py` & `robotcode_core-0.50.0/src/robotcode/core/utils/net.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/src/robotcode/core/utils/process.py` & `robotcode_core-0.50.0/src/robotcode/core/utils/process.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/src/robotcode/core/utils/safe_eval.py` & `robotcode_core-0.50.0/src/robotcode/core/utils/safe_eval.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/src/robotcode/core/utils/version.py` & `robotcode_core-0.50.0/src/robotcode/core/utils/version.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/.gitignore` & `robotcode_core-0.50.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/LICENSE.txt` & `robotcode_core-0.50.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/README.md` & `robotcode_core-0.50.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/pyproject.toml` & `robotcode_core-0.50.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.49.0/PKG-INFO` & `robotcode_core-0.50.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-core
-Version: 0.49.0
+Version: 0.50.0
 Summary: Some core classes for RobotCode
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
```

