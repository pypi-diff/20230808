# Comparing `tmp/taskiq_dependencies-1.3.0.tar.gz` & `tmp/taskiq_dependencies-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_dependencies-1.3.0.tar", max compression
+gzip compressed data, was "taskiq_dependencies-1.3.1.tar", max compression
```

## Comparing `taskiq_dependencies-1.3.0.tar` & `taskiq_dependencies-1.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6368 2023-06-11 13:36:41.851076 taskiq_dependencies-1.3.0/README.md
--rw-r--r--   0        0        0     1618 2023-06-11 13:36:41.855076 taskiq_dependencies-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      386 2023-06-11 13:36:41.855076 taskiq_dependencies-1.3.0/taskiq_dependencies/__init__.py
--rw-r--r--   0        0        0    11773 2023-06-11 13:36:41.855076 taskiq_dependencies-1.3.0/taskiq_dependencies/ctx.py
--rw-r--r--   0        0        0     3273 2023-06-11 13:36:41.855076 taskiq_dependencies-1.3.0/taskiq_dependencies/dependency.py
--rw-r--r--   0        0        0     9626 2023-06-11 13:36:41.855076 taskiq_dependencies-1.3.0/taskiq_dependencies/graph.py
--rw-r--r--   0        0        0        0 2023-06-11 13:36:41.855076 taskiq_dependencies-1.3.0/taskiq_dependencies/py.typed
--rw-r--r--   0        0        0      573 2023-06-11 13:36:41.855076 taskiq_dependencies-1.3.0/taskiq_dependencies/utils.py
--rw-r--r--   0        0        0     7205 1970-01-01 00:00:00.000000 taskiq_dependencies-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     7845 2023-08-07 23:08:24.916518 taskiq_dependencies-1.3.1/README.md
+-rw-r--r--   0        0        0     1618 2023-08-07 23:08:24.920518 taskiq_dependencies-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      386 2023-08-07 23:08:24.920518 taskiq_dependencies-1.3.1/taskiq_dependencies/__init__.py
+-rw-r--r--   0        0        0    11773 2023-08-07 23:08:24.920518 taskiq_dependencies-1.3.1/taskiq_dependencies/ctx.py
+-rw-r--r--   0        0        0     3273 2023-08-07 23:08:24.920518 taskiq_dependencies-1.3.1/taskiq_dependencies/dependency.py
+-rw-r--r--   0        0        0    10345 2023-08-07 23:08:24.920518 taskiq_dependencies-1.3.1/taskiq_dependencies/graph.py
+-rw-r--r--   0        0        0        0 2023-08-07 23:08:24.920518 taskiq_dependencies-1.3.1/taskiq_dependencies/py.typed
+-rw-r--r--   0        0        0      573 2023-08-07 23:08:24.920518 taskiq_dependencies-1.3.1/taskiq_dependencies/utils.py
+-rw-r--r--   0        0        0     8682 1970-01-01 00:00:00.000000 taskiq_dependencies-1.3.1/PKG-INFO
```

### Comparing `taskiq_dependencies-1.3.0/README.md` & `taskiq_dependencies-1.3.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -256,7 +256,56 @@
 
 This code will is going to print:
 
 ```
 strstr
 100
 ```
+
+## Dependencies replacement
+
+You can replace dependencies in runtime, it will recalculate graph
+and will execute your function with updated dependencies.
+
+**!!! This functionality tremendously slows down dependency resolution.**
+
+Use this functionality only for tests. Otherwise, you will end up building dependency graphs on every resolution request. Which is very slow.
+
+But for tests it may be a game changer, since you don't want to change your code, but some dependencies instead.
+
+Here's an example. Imagine you have a built graph for a specific function, like this:
+
+```python
+from taskiq_dependencies import DependencyGraph, Depends
+
+
+def dependency() -> int:
+    return 1
+
+
+def target(dep_value: int = Depends(dependency)) -> None:
+    assert dep_value == 1
+
+graph = DependencyGraph(target)
+```
+
+Normally, you would call the target, by writing something like this:
+
+```python
+with graph.sync_ctx() as ctx:
+    target(**ctx.resolve_kwargs())
+```
+
+But what if you want to replace dependency in runtime, just
+before resolving kwargs? The solution is to add `replaced_deps`
+parameter to the context method. For example:
+
+```python
+def replaced() -> int:
+    return 2
+
+
+with graph.sync_ctx(replaced_deps={dependency: replaced}) as ctx:
+    target(**ctx.resolve_kwargs())
+```
+
+Furthermore, the new dependency can depend on other dependencies. Or you can change type of your dependency, like generator instead of plain return. Everything should work as you would expect it.
```

### Comparing `taskiq_dependencies-1.3.0/pyproject.toml` & `taskiq_dependencies-1.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq-dependencies"
-version = "1.3.0"
+version = "1.3.1"
 description = "FastAPI like dependency injection implementation"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 packages = [{include = "taskiq_dependencies"}]
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
```

### Comparing `taskiq_dependencies-1.3.0/taskiq_dependencies/ctx.py` & `taskiq_dependencies-1.3.1/taskiq_dependencies/ctx.py`

 * *Files identical despite different names*

### Comparing `taskiq_dependencies-1.3.0/taskiq_dependencies/dependency.py` & `taskiq_dependencies-1.3.1/taskiq_dependencies/dependency.py`

 * *Files identical despite different names*

### Comparing `taskiq_dependencies-1.3.0/taskiq_dependencies/graph.py` & `taskiq_dependencies-1.3.1/taskiq_dependencies/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,70 +16,82 @@
     """Class to build dependency graph from a function."""
 
     dep_graph = True
 
     def __init__(
         self,
         target: Callable[..., Any],
+        replaced_deps: Optional[Dict[Any, Any]] = None,
     ) -> None:
         self.target = target
         # Ordinary dependencies with cache.
         self.dependencies: Dict[Any, List[Dependency]] = defaultdict(list)
         # Dependencies without cache.
         # Can be considered as sub graphs.
         self.subgraphs: Dict[Any, DependencyGraph] = {}
         self.ordered_deps: List[Dependency] = []
+        self.replaced_deps = replaced_deps
         self._build_graph()
 
     def is_empty(self) -> bool:
         """
         Checks that target function depends on at least something.
 
         :return: True if depends.
         """
         return len(self.ordered_deps) <= 1
 
     def async_ctx(
         self,
         initial_cache: Optional[Dict[Any, Any]] = None,
+        replaced_deps: Optional[Dict[Any, Any]] = None,
         exception_propagation: bool = True,
     ) -> AsyncResolveContext:
         """
         Create dependency resolver context.
 
         This context is used to actually resolve dependencies.
 
         :param initial_cache: initial cache dict.
         :param exception_propagation: If true, all found errors within
             context will be propagated to dependencies.
+        :param replaced_deps: Dependencies to replace during runtime.
         :return: new resolver context.
         """
+        graph = self
+        if replaced_deps:
+            graph = DependencyGraph(self.target, replaced_deps)
         return AsyncResolveContext(
-            self,
+            graph,
             initial_cache,
             exception_propagation,
         )
 
     def sync_ctx(
         self,
         initial_cache: Optional[Dict[Any, Any]] = None,
+        replaced_deps: Optional[Dict[Any, Any]] = None,
         exception_propagation: bool = True,
     ) -> SyncResolveContext:
         """
         Create dependency resolver context.
 
         This context is used to actually resolve dependencies.
 
         :param initial_cache: initial cache dict.
         :param exception_propagation: If true, all found errors within
             context will be propagated to dependencies.
+        :param replaced_deps: Dependencies to replace during runtime.
         :return: new resolver context.
         """
+        graph = self
+        if replaced_deps:
+            graph = DependencyGraph(self.target, replaced_deps)
         return SyncResolveContext(
-            self,
+            graph,
             initial_cache,
             exception_propagation,
         )
 
     def _build_graph(self) -> None:  # noqa: C901, WPS210
         """
         Builds actual graph.
@@ -98,14 +110,16 @@
         while dep_deque:
             dep = dep_deque.popleft()
             # Skip adding dependency if it's already present.
             if dep in self.dependencies:
                 continue
             if dep.dependency is None:
                 continue
+            if self.replaced_deps and dep.dependency in self.replaced_deps:
+                dep.dependency = self.replaced_deps[dep.dependency]
             # Get signature and type hints.
             origin = getattr(dep.dependency, "__origin__", None)
             if origin is None:
                 origin = dep.dependency
 
             # If we found the typevar.
             # It means, that somebody depend on generic type.
```

### Comparing `taskiq_dependencies-1.3.0/taskiq_dependencies/utils.py` & `taskiq_dependencies-1.3.1/taskiq_dependencies/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq_dependencies-1.3.0/PKG-INFO` & `taskiq_dependencies-1.3.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-dependencies
-Version: 1.3.0
+Version: 1.3.1
 Summary: FastAPI like dependency injection implementation
 Keywords: taskiq,dependencies,injection,async,DI
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -278,7 +278,56 @@
 This code will is going to print:
 
 ```
 strstr
 100
 ```
 
+## Dependencies replacement
+
+You can replace dependencies in runtime, it will recalculate graph
+and will execute your function with updated dependencies.
+
+**!!! This functionality tremendously slows down dependency resolution.**
+
+Use this functionality only for tests. Otherwise, you will end up building dependency graphs on every resolution request. Which is very slow.
+
+But for tests it may be a game changer, since you don't want to change your code, but some dependencies instead.
+
+Here's an example. Imagine you have a built graph for a specific function, like this:
+
+```python
+from taskiq_dependencies import DependencyGraph, Depends
+
+
+def dependency() -> int:
+    return 1
+
+
+def target(dep_value: int = Depends(dependency)) -> None:
+    assert dep_value == 1
+
+graph = DependencyGraph(target)
+```
+
+Normally, you would call the target, by writing something like this:
+
+```python
+with graph.sync_ctx() as ctx:
+    target(**ctx.resolve_kwargs())
+```
+
+But what if you want to replace dependency in runtime, just
+before resolving kwargs? The solution is to add `replaced_deps`
+parameter to the context method. For example:
+
+```python
+def replaced() -> int:
+    return 2
+
+
+with graph.sync_ctx(replaced_deps={dependency: replaced}) as ctx:
+    target(**ctx.resolve_kwargs())
+```
+
+Furthermore, the new dependency can depend on other dependencies. Or you can change type of your dependency, like generator instead of plain return. Everything should work as you would expect it.
+
```

