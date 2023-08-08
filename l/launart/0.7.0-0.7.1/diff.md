# Comparing `tmp/launart-0.7.0.tar.gz` & `tmp/launart-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launart-0.7.0.tar", last modified: Sun Aug  6 13:00:28 2023, max compression
+gzip compressed data, was "launart-0.7.1.tar", last modified: Tue Aug  8 12:45:44 2023, max compression
```

## Comparing `launart-0.7.0.tar` & `launart-0.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1071 2023-08-06 13:00:11.757793 launart-0.7.0/LICENSE
--rw-r--r--   0        0        0      929 2023-08-06 13:00:11.757793 launart-0.7.0/README.md
--rw-r--r--   0        0        0      520 2023-08-06 13:00:11.757793 launart-0.7.0/launart/__init__.py
--rw-r--r--   0        0        0      913 2023-08-06 13:00:11.757793 launart-0.7.0/launart/_sideload.py
--rw-r--r--   0        0        0    19050 2023-08-06 13:00:11.757793 launart-0.7.0/launart/manager.py
--rw-r--r--   0        0        0        0 2023-08-06 13:00:11.757793 launart-0.7.0/launart/ryanvk/__init__.py
--rw-r--r--   0        0        0      993 2023-08-06 13:00:11.757793 launart-0.7.0/launart/saya.py
--rw-r--r--   0        0        0     3615 2023-08-06 13:00:11.757793 launart-0.7.0/launart/service.py
--rw-r--r--   0        0        0     3825 2023-08-06 13:00:11.757793 launart-0.7.0/launart/status.py
--rw-r--r--   0        0        0     3259 2023-08-06 13:00:11.757793 launart-0.7.0/launart/utilles.py
--rw-r--r--   0        0        0     1552 2023-08-06 13:00:28.841802 launart-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      122 2023-08-06 13:00:11.757793 launart-0.7.0/tests/_saya_mod/empty_sub.py
--rw-r--r--   0        0        0      129 2023-08-06 13:00:11.757793 launart-0.7.0/tests/_saya_mod/fail_sub.py
--rw-r--r--   0        0        0      662 2023-08-06 13:00:11.757793 launart-0.7.0/tests/_saya_mod/ok_sub.py
--rw-r--r--   0        0        0     1637 2023-08-06 13:00:11.757793 launart-0.7.0/tests/fixture.py
--rw-r--r--   0        0        0     3773 2023-08-06 13:00:11.757793 launart-0.7.0/tests/launchable.py
--rw-r--r--   0        0        0     8666 2023-08-06 13:00:11.757793 launart-0.7.0/tests/manager.py
--rw-r--r--   0        0        0     1085 2023-08-06 13:00:11.757793 launart-0.7.0/tests/saya.py
--rw-r--r--   0        0        0     2462 2023-08-06 13:00:11.757793 launart-0.7.0/tests/sideload.py
--rw-r--r--   0        0        0     1994 2023-08-06 13:00:11.757793 launart-0.7.0/tests/utils.py
--rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 launart-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-08 12:45:32.327569 launart-0.7.1/LICENSE
+-rw-r--r--   0        0        0      929 2023-08-08 12:45:32.327569 launart-0.7.1/README.md
+-rw-r--r--   0        0        0      520 2023-08-08 12:45:32.327569 launart-0.7.1/launart/__init__.py
+-rw-r--r--   0        0        0      913 2023-08-08 12:45:32.327569 launart-0.7.1/launart/_sideload.py
+-rw-r--r--   0        0        0    19078 2023-08-08 12:45:32.327569 launart-0.7.1/launart/manager.py
+-rw-r--r--   0        0        0        0 2023-08-08 12:45:32.327569 launart-0.7.1/launart/ryanvk/__init__.py
+-rw-r--r--   0        0        0      993 2023-08-08 12:45:32.327569 launart-0.7.1/launart/saya.py
+-rw-r--r--   0        0        0     3615 2023-08-08 12:45:32.327569 launart-0.7.1/launart/service.py
+-rw-r--r--   0        0        0     3825 2023-08-08 12:45:32.327569 launart-0.7.1/launart/status.py
+-rw-r--r--   0        0        0     3259 2023-08-08 12:45:32.327569 launart-0.7.1/launart/utilles.py
+-rw-r--r--   0        0        0     1552 2023-08-08 12:45:44.647733 launart-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-08-08 12:45:32.327569 launart-0.7.1/tests/_saya_mod/empty_sub.py
+-rw-r--r--   0        0        0      129 2023-08-08 12:45:32.327569 launart-0.7.1/tests/_saya_mod/fail_sub.py
+-rw-r--r--   0        0        0      662 2023-08-08 12:45:32.327569 launart-0.7.1/tests/_saya_mod/ok_sub.py
+-rw-r--r--   0        0        0     1637 2023-08-08 12:45:32.327569 launart-0.7.1/tests/fixture.py
+-rw-r--r--   0        0        0     3773 2023-08-08 12:45:32.327569 launart-0.7.1/tests/launchable.py
+-rw-r--r--   0        0        0     8666 2023-08-08 12:45:32.327569 launart-0.7.1/tests/manager.py
+-rw-r--r--   0        0        0     1085 2023-08-08 12:45:32.327569 launart-0.7.1/tests/saya.py
+-rw-r--r--   0        0        0     2462 2023-08-08 12:45:32.327569 launart-0.7.1/tests/sideload.py
+-rw-r--r--   0        0        0     1994 2023-08-08 12:45:32.327569 launart-0.7.1/tests/utils.py
+-rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 launart-0.7.1/PKG-INFO
```

### Comparing `launart-0.7.0/LICENSE` & `launart-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `launart-0.7.0/README.md` & `launart-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `launart-0.7.0/launart/__init__.py` & `launart-0.7.1/launart/__init__.py`

 * *Files identical despite different names*

### Comparing `launart-0.7.0/launart/_sideload.py` & `launart-0.7.1/launart/_sideload.py`

 * *Files identical despite different names*

### Comparing `launart-0.7.0/launart/manager.py` & `launart-0.7.1/launart/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         logger.info(
             f"Component {component.id} completed.",
             alt=rf"[green]Component [magenta]{component.id}[/magenta] completed.",
         )
 
         # clean interface
 
-        for k, v in list(self._default_isolate['interface_provide']):
+        for k, v in list(self._default_isolate['interface_provide'].items()):
             if v is component:
                 del self._default_isolate['interface_provide'][k]
 
     async def _component_prepare(self, task: asyncio.Task, component: Service):
         if component.status.stage != "waiting-for-prepare":  # pragma: worst case
             logger.info(f"Wait component {component.id} into preparing.")
             await any_completed(task, component.status.wait_for("waiting-for-prepare"))
@@ -435,15 +435,15 @@
         loop: Optional[asyncio.AbstractEventLoop] = None,
         stop_signal: Iterable[signal.Signals] = (signal.SIGINT,),
     ):
         import contextlib
         import functools
         import threading
 
-        if loop is not None:
+        if loop is not None:  # pragma: no cover
             from warnings import warn
 
             warn(
                 "The loop argument is deprecated since launart 0.6.4, " "and scheduled for removal in launart 0.7.0.",
                 DeprecationWarning,
                 stacklevel=2,
             )
```

### Comparing `launart-0.7.0/launart/saya.py` & `launart-0.7.1/launart/saya.py`

 * *Files identical despite different names*

### Comparing `launart-0.7.0/launart/service.py` & `launart-0.7.1/launart/service.py`

 * *Files identical despite different names*

### Comparing `launart-0.7.0/launart/status.py` & `launart-0.7.1/launart/status.py`

 * *Files identical despite different names*

### Comparing `launart-0.7.0/launart/utilles.py` & `launart-0.7.1/launart/utilles.py`

 * *Files identical despite different names*

### Comparing `launart-0.7.0/pyproject.toml` & `launart-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "launart"
-version = "0.7.0"
+version = "0.7.1"
 description = "Component lifetime manager for runtime."
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
 dependencies = [
     "statv>=0.2.2",
     "loguru>=0.6.0",
```

### Comparing `launart-0.7.0/tests/_saya_mod/ok_sub.py` & `launart-0.7.1/tests/_saya_mod/ok_sub.py`

 * *Files identical despite different names*

### Comparing `launart-0.7.0/tests/fixture.py` & `launart-0.7.1/tests/fixture.py`

 * *Files identical despite different names*

### Comparing `launart-0.7.0/tests/launchable.py` & `launart-0.7.1/tests/launchable.py`

 * *Files identical despite different names*

### Comparing `launart-0.7.0/tests/manager.py` & `launart-0.7.1/tests/manager.py`

 * *Files identical despite different names*

### Comparing `launart-0.7.0/tests/saya.py` & `launart-0.7.1/tests/saya.py`

 * *Files identical despite different names*

### Comparing `launart-0.7.0/tests/sideload.py` & `launart-0.7.1/tests/sideload.py`

 * *Files identical despite different names*

### Comparing `launart-0.7.0/tests/utils.py` & `launart-0.7.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `launart-0.7.0/PKG-INFO` & `launart-0.7.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launart
-Version: 0.7.0
+Version: 0.7.1
 Summary: Component lifetime manager for runtime.
 Author-Email: GreyElaina <GreyElaina@outlook.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: statv>=0.2.2
 Requires-Dist: loguru>=0.6.0
 Requires-Dist: creart>=0.3.0
```

