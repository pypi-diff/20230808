# Comparing `tmp/bounded_pool-0.0.1a0.tar.gz` & `tmp/bounded_pool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bounded_pool-0.0.1a0.tar", last modified: Fri Aug  4 08:54:47 2023, max compression
+gzip compressed data, was "bounded_pool-0.0.2.tar", last modified: Tue Aug  8 20:00:56 2023, max compression
```

## Comparing `bounded_pool-0.0.1a0.tar` & `bounded_pool-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 michaelkrukov   (501) staff       (20)        0 2023-08-04 08:54:47.747297 bounded_pool-0.0.1a0/
--rw-r--r--   0 michaelkrukov   (501) staff       (20)     1072 2023-08-04 08:19:11.000000 bounded_pool-0.0.1a0/LICENSE
--rw-r--r--   0 michaelkrukov   (501) staff       (20)     1689 2023-08-04 08:54:47.747166 bounded_pool-0.0.1a0/PKG-INFO
--rw-r--r--   0 michaelkrukov   (501) staff       (20)     1103 2023-08-04 08:24:32.000000 bounded_pool-0.0.1a0/README.md
-drwxr-xr-x   0 michaelkrukov   (501) staff       (20)        0 2023-08-04 08:54:47.745339 bounded_pool-0.0.1a0/bounded_pool/
--rw-r--r--   0 michaelkrukov   (501) staff       (20)     3373 2023-08-04 08:19:11.000000 bounded_pool-0.0.1a0/bounded_pool/__init__.py
-drwxr-xr-x   0 michaelkrukov   (501) staff       (20)        0 2023-08-04 08:54:47.745994 bounded_pool-0.0.1a0/bounded_pool.egg-info/
--rw-r--r--   0 michaelkrukov   (501) staff       (20)     1689 2023-08-04 08:54:47.000000 bounded_pool-0.0.1a0/bounded_pool.egg-info/PKG-INFO
--rw-r--r--   0 michaelkrukov   (501) staff       (20)      280 2023-08-04 08:54:47.000000 bounded_pool-0.0.1a0/bounded_pool.egg-info/SOURCES.txt
--rw-r--r--   0 michaelkrukov   (501) staff       (20)        1 2023-08-04 08:54:47.000000 bounded_pool-0.0.1a0/bounded_pool.egg-info/dependency_links.txt
--rw-r--r--   0 michaelkrukov   (501) staff       (20)       13 2023-08-04 08:54:47.000000 bounded_pool-0.0.1a0/bounded_pool.egg-info/top_level.txt
--rw-r--r--   0 michaelkrukov   (501) staff       (20)       38 2023-08-04 08:54:47.747338 bounded_pool-0.0.1a0/setup.cfg
--rw-r--r--   0 michaelkrukov   (501) staff       (20)     1119 2023-08-04 08:19:11.000000 bounded_pool-0.0.1a0/setup.py
-drwxr-xr-x   0 michaelkrukov   (501) staff       (20)        0 2023-08-04 08:54:47.746929 bounded_pool-0.0.1a0/tests/
--rw-r--r--   0 michaelkrukov   (501) staff       (20)     1314 2023-08-04 08:50:29.000000 bounded_pool-0.0.1a0/tests/test_basic.py
--rw-r--r--   0 michaelkrukov   (501) staff       (20)      563 2023-08-04 08:19:11.000000 bounded_pool-0.0.1a0/tests/test_defaults.py
--rw-r--r--   0 michaelkrukov   (501) staff       (20)      376 2023-08-04 08:19:11.000000 bounded_pool-0.0.1a0/tests/test_example.py
--rw-r--r--   0 michaelkrukov   (501) staff       (20)      952 2023-08-04 08:19:11.000000 bounded_pool-0.0.1a0/tests/test_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:00:55.998369 bounded_pool-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-08 20:00:25.000000 bounded_pool-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-08-08 20:00:55.998369 bounded_pool-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-08-08 20:00:25.000000 bounded_pool-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:00:55.994369 bounded_pool-0.0.2/bounded_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-08-08 20:00:25.000000 bounded_pool-0.0.2/bounded_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:00:55.994369 bounded_pool-0.0.2/bounded_pool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-08-08 20:00:55.000000 bounded_pool-0.0.2/bounded_pool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-08 20:00:55.000000 bounded_pool-0.0.2/bounded_pool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:00:55.000000 bounded_pool-0.0.2/bounded_pool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 20:00:55.000000 bounded_pool-0.0.2/bounded_pool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 20:00:55.998369 bounded_pool-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-08 20:00:25.000000 bounded_pool-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:00:55.994369 bounded_pool-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-08 20:00:25.000000 bounded_pool-0.0.2/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-08 20:00:25.000000 bounded_pool-0.0.2/tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-08 20:00:25.000000 bounded_pool-0.0.2/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-08 20:00:25.000000 bounded_pool-0.0.2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-08 20:00:25.000000 bounded_pool-0.0.2/tests/test_queue.py
```

### Comparing `bounded_pool-0.0.1a0/LICENSE` & `bounded_pool-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bounded_pool-0.0.1a0/bounded_pool/__init__.py` & `bounded_pool-0.0.2/bounded_pool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import multiprocessing
 import os
 import threading
 from abc import ABC
 from asyncio import Semaphore, Task, create_task
 from concurrent.futures import Executor, ProcessPoolExecutor, ThreadPoolExecutor
-from typing import List, Optional
+from typing import Optional
 
 
 class BoundedExecutor(ABC):
     def __init__(
         self,
         max_workers: Optional[int] = None,
         max_queue_size: int = 0,
@@ -27,35 +27,32 @@
 
 class BoundedAsyncioPoolExecutor(BoundedExecutor):
     @staticmethod
     def _get_default_max_workers():
         return min(32, (os.cpu_count() or 1) + 4)
 
     async def __aenter__(self):
-        self._tasks: List[Task] = []
         self._semaphore = Semaphore(self._semaphore_size)
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
-        while self._tasks:
-            await self._tasks.pop()
+        # make sure no tasks being executed
+        for _ in range(self._semaphore_size):
+            await self._semaphore.acquire()
 
     async def _acquire(self):
         await self._semaphore.acquire()
 
     def _release(self, fut):
-        if fut in self._tasks:
-            self._tasks.remove(fut)
         self._semaphore.release()
 
     async def submit(self, coro, *args, **kwargs) -> Task:
         await self._acquire()
         task = create_task(coro(*args, **kwargs))
         task.add_done_callback(self._release)
-        self._tasks.append(task)
         return task
 
 
 class SyncBoundedExecutor(BoundedExecutor):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._executor: Optional[Executor] = None
```

### Comparing `bounded_pool-0.0.1a0/setup.py` & `bounded_pool-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `bounded_pool-0.0.1a0/tests/test_basic.py` & `bounded_pool-0.0.2/tests/test_queue.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,38 +9,24 @@
     BoundedThreadPoolExecutor,
 )
 
 from .conftest import aassert_takes, assert_takes
 
 
 @pytest.mark.anyio
-async def test_asyncio_executor_sleeps():
-    async with aassert_takes(less=1.5):
-        async with BoundedAsyncioPoolExecutor(2) as pool:
+async def test_asyncio_executor_queues():
+    async with BoundedAsyncioPoolExecutor(1, 1) as pool:
+        async with aassert_takes(more=1, less=2):
             async with aassert_takes(less=0.5):
-                for _ in range(2):
-                    await pool.submit(asyncio.sleep, 1)
-
-        assert not pool._tasks
-
-    async with aassert_takes(more=3.5):
-        async with BoundedAsyncioPoolExecutor(1) as pool:
-            async with aassert_takes(more=3):
-                for _ in range(4):
-                    await pool.submit(asyncio.sleep, 1)
-
-        assert not pool._tasks
+                await pool.submit(asyncio.sleep, 1)
+                await pool.submit(asyncio.sleep, 1)
+            await pool.submit(asyncio.sleep, 1)
 
 
 @pytest.mark.parametrize('cls', [BoundedThreadPoolExecutor, BoundedProcessPoolExecutor])
-def test_sync_executor_sleeps(cls):
-    with assert_takes(less=1.5):
-        with cls(2) as pool:
+def test_sync_executor_queues(cls):
+    with cls(1, 1) as pool:
+        with assert_takes(more=1, less=2):
             with assert_takes(less=0.5):
-                for _ in range(2):
-                    pool.submit(time.sleep, 1)
-
-    with assert_takes(more=3.5):
-        with cls(1) as pool:
-            with assert_takes(more=3):
-                for _ in range(2):
-                    pool.submit(time.sleep, 1)
+                pool.submit(time.sleep, 1)
+                pool.submit(time.sleep, 1)
+            pool.submit(time.sleep, 1)
```

### Comparing `bounded_pool-0.0.1a0/tests/test_defaults.py` & `bounded_pool-0.0.2/tests/test_defaults.py`

 * *Files identical despite different names*

