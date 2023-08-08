# Comparing `tmp/robotcode_jsonrpc2-0.49.0.tar.gz` & `tmp/robotcode_jsonrpc2-0.50.0.tar.gz`

## Comparing `robotcode_jsonrpc2-0.49.0.tar` & `robotcode_jsonrpc2-0.50.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.49.0/src/robotcode/jsonrpc2/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.49.0/src/robotcode/jsonrpc2/__version__.py
--rw-r--r--   0        0        0    30454 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.49.0/src/robotcode/jsonrpc2/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.49.0/src/robotcode/jsonrpc2/py.typed
--rw-r--r--   0        0        0     9709 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.49.0/src/robotcode/jsonrpc2/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.49.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.49.0/LICENSE.txt
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.49.0/README.md
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.49.0/pyproject.toml
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.49.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.50.0/src/robotcode/jsonrpc2/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.50.0/src/robotcode/jsonrpc2/__version__.py
+-rw-r--r--   0        0        0    31054 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.50.0/src/robotcode/jsonrpc2/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.50.0/src/robotcode/jsonrpc2/py.typed
+-rw-r--r--   0        0        0     9709 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.50.0/src/robotcode/jsonrpc2/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.50.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.50.0/LICENSE.txt
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.50.0/README.md
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.50.0/pyproject.toml
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.50.0/PKG-INFO
```

### Comparing `robotcode_jsonrpc2-0.49.0/src/robotcode/jsonrpc2/protocol.py` & `robotcode_jsonrpc2-0.50.0/src/robotcode/jsonrpc2/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,16 @@
     method: Callable[..., Any]
     param_type: Optional[Type[Any]]
     cancelable: bool
 
 
 @runtime_checkable
 class RpcMethod(Protocol):
+    __slots__ = "__rpc_method__"
+
     __rpc_method__: RpcMethodEntry
 
 
 _F = TypeVar("_F", bound=Callable[..., Any])
 
 
 @overload
@@ -260,15 +262,20 @@
                     rpc_method.__rpc_method__.name,
                     method,
                     rpc_method.__rpc_method__.param_type,
                     rpc_method.__rpc_method__.cancelable,
                 )
                 for method, rpc_method in map(
                     lambda m1: (m1, cast(RpcMethod, m1)),
-                    filter(lambda m2: isinstance(m2, RpcMethod), iter_methods(obj)),
+                    iter_methods(
+                        obj,
+                        lambda m2: isinstance(m2, RpcMethod)
+                        or inspect.ismethod(m2)
+                        and isinstance(m2.__func__, RpcMethod),
+                    ),
                 )
             }
 
         if not self.__initialized:
             if inspect.isclass(self.__owner):
                 self.__methods = get_methods(self.__owner)
 
@@ -757,15 +764,21 @@
                 f"Unknown method: {message.method}",
                 id=message.id,
             )
             return
 
         params = self._convert_params(e.method, e.param_type, message.params)
 
-        if isinstance(e.method, HasThreaded) and e.method.__threaded__:
+        if (
+            isinstance(e.method, HasThreaded)
+            and e.method.__threaded__
+            or inspect.ismethod(e.method)
+            and isinstance(e.method.__func__, HasThreaded)
+            and e.method.__func__.__threaded__
+        ):
             task = run_coroutine_in_thread(
                 ensure_coroutine(cast(Callable[..., Any], e.method)), *params[0], **params[1]
             )
         else:
             task = create_sub_task(
                 ensure_coroutine(e.method)(*params[0], **params[1]),
                 name=message.method,
@@ -822,15 +835,21 @@
 
         if e is None or not callable(e.method):
             self.__logger.warning(lambda: f"Unknown method: {message.method}")
             return
         try:
             params = self._convert_params(e.method, e.param_type, message.params)
 
-            if isinstance(e.method, HasThreaded) and e.method.__threaded__:
+            if (
+                isinstance(e.method, HasThreaded)
+                and e.method.__threaded__
+                or inspect.ismethod(e.method)
+                and isinstance(e.method.__func__, HasThreaded)
+                and e.method.__func__.__threaded__
+            ):
                 task = run_coroutine_in_thread(
                     ensure_coroutine(cast(Callable[..., Any], e.method)), *params[0], **params[1]
                 )
             else:
                 task = create_sub_task(
                     ensure_coroutine(e.method)(*params[0], **params[1]),
                     name=message.method,
```

### Comparing `robotcode_jsonrpc2-0.49.0/src/robotcode/jsonrpc2/server.py` & `robotcode_jsonrpc2-0.50.0/src/robotcode/jsonrpc2/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.49.0/.gitignore` & `robotcode_jsonrpc2-0.50.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.49.0/LICENSE.txt` & `robotcode_jsonrpc2-0.50.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.49.0/README.md` & `robotcode_jsonrpc2-0.50.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.49.0/pyproject.toml` & `robotcode_jsonrpc2-0.50.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Operating System :: OS Independent",
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
-dependencies = ["robotcode-core==0.49.0"]
+dependencies = ["robotcode-core==0.50.0"]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
 Documentation = "https://github.com/d-biehl/robotcode#readme"
 Changelog = "https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md"
```

### Comparing `robotcode_jsonrpc2-0.49.0/PKG-INFO` & `robotcode_jsonrpc2-0.50.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-jsonrpc2
-Version: 0.49.0
+Version: 0.50.0
 Summary: JSONRPC Server for RobotCode
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-core==0.49.0
+Requires-Dist: robotcode-core==0.50.0
 Description-Content-Type: text/markdown
 
 # robotcode-jsonrpc2
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-jsonrpc2.svg)](https://pypi.org/project/robotcode-jsonrpc2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-jsonrpc2.svg)](https://pypi.org/project/robotcode-jsonrpc2)
 [![License](https://img.shields.io/github/license/d-biehl/robotcode?style=flat&logo=apache)](https://github.com/d-biehl/robotcode/blob/master/LICENSE.txt)
```

