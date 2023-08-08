# Comparing `tmp/async_wrapper-0.5.1.tar.gz` & `tmp/async_wrapper-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.5.1.tar", max compression
+gzip compressed data, was "async_wrapper-0.5.2.tar", max compression
```

## Comparing `async_wrapper-0.5.1.tar` & `async_wrapper-0.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1070 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/LICENSE
--rw-r--r--   0        0        0     1836 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/README.md
--rw-r--r--   0        0        0     3983 2023-08-06 19:26:55.955239 async_wrapper-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      513 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-08-06 19:26:55.999239 async_wrapper-0.5.1/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0     1668 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/convert/_async.py
--rw-r--r--   0        0        0     4568 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/convert/_sync.py
--rw-r--r--   0        0        0     1226 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0     1560 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/exception.py
--rw-r--r--   0        0        0        0 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/py.typed
--rw-r--r--   0        0        0    12169 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/queue.py
--rw-r--r--   0        0        0      207 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0     7500 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/task_group/task_group.py
--rw-r--r--   0        0        0      866 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/task_group/value.py
--rw-r--r--   0        0        0    11566 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/wait.py
--rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 async_wrapper-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-08 11:04:29.262139 async_wrapper-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1994 2023-08-08 11:04:29.262139 async_wrapper-0.5.2/README.md
+-rw-r--r--   0        0        0     3983 2023-08-08 11:04:42.662216 async_wrapper-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-08-08 11:04:29.262139 async_wrapper-0.5.2/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-08 11:04:42.702219 async_wrapper-0.5.2/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-08-08 11:04:29.262139 async_wrapper-0.5.2/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0     1673 2023-08-08 11:04:29.262139 async_wrapper-0.5.2/src/async_wrapper/convert/_async.py
+-rw-r--r--   0        0        0     4573 2023-08-08 11:04:29.262139 async_wrapper-0.5.2/src/async_wrapper/convert/_sync.py
+-rw-r--r--   0        0        0     1231 2023-08-08 11:04:29.262139 async_wrapper-0.5.2/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0     1699 2023-08-08 11:04:29.262139 async_wrapper-0.5.2/src/async_wrapper/exception.py
+-rw-r--r--   0        0        0        0 2023-08-08 11:04:29.262139 async_wrapper-0.5.2/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0    17607 2023-08-08 11:04:29.262139 async_wrapper-0.5.2/src/async_wrapper/queue.py
+-rw-r--r--   0        0        0      207 2023-08-08 11:04:29.262139 async_wrapper-0.5.2/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0     7528 2023-08-08 11:04:29.262139 async_wrapper-0.5.2/src/async_wrapper/task_group/task_group.py
+-rw-r--r--   0        0        0     1211 2023-08-08 11:04:29.262139 async_wrapper-0.5.2/src/async_wrapper/task_group/value.py
+-rw-r--r--   0        0        0    11599 2023-08-08 11:04:29.262139 async_wrapper-0.5.2/src/async_wrapper/wait.py
+-rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 async_wrapper-0.5.2/PKG-INFO
```

### Comparing `async_wrapper-0.5.1/LICENSE` & `async_wrapper-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.5.1/README.md` & `async_wrapper-0.5.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # async-wrapper
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Documentation Status](https://readthedocs.org/projects/async-wrapper/badge/?version=latest)](https://async-wrapper.readthedocs.io/en/latest/?badge=latest)
 [![github action](https://github.com/phi-friday/async-wrapper/actions/workflows/check.yaml/badge.svg?event=push&branch=main)](#)
 [![codecov](https://codecov.io/gh/phi-friday/async-wrapper/branch/main/graph/badge.svg?token=R1RAQ5F0YD)](https://codecov.io/gh/phi-friday/async-wrapper)
 [![PyPI version](https://badge.fury.io/py/async-wrapper.svg)](https://badge.fury.io/py/async-wrapper)
 [![python version](https://img.shields.io/pypi/pyversions/async_wrapper.svg)](#)
 
 ## how to install
 ```shell
```

### Comparing `async_wrapper-0.5.1/pyproject.toml` & `async_wrapper-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.5.1"
+version = "0.5.2"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://async-wrapper.readthedocs.io/"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
```

### Comparing `async_wrapper-0.5.1/src/async_wrapper/__init__.py` & `async_wrapper-0.5.2/src/async_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.5.1/src/async_wrapper/convert/_async.py` & `async_wrapper-0.5.2/src/async_wrapper/convert/_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 __all__ = ["sync_to_async"]
 
 
 def sync_to_async(
     func: Callable[ParamT, ValueT_co],
 ) -> Callable[ParamT, Coroutine[Any, Any, ValueT_co]]:
-    """Convert a synchronous function to an asynchronous function.
+    """
+    Convert a synchronous function to an asynchronous function.
 
     Args:
         func: The synchronous function to be converted.
 
     Returns:
         An asynchronous function
         that behaves equivalently to the input synchronous function.
```

### Comparing `async_wrapper-0.5.1/src/async_wrapper/convert/_sync.py` & `async_wrapper-0.5.2/src/async_wrapper/convert/_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 current_async_lib_var = ContextVar("current_async_lib", default="asyncio")
 use_uvloop_var = ContextVar("use_uvloop", default=False)
 
 
 def async_to_sync(
     func: Callable[ParamT, Awaitable[ValueT_co]],
 ) -> Callable[ParamT, ValueT_co]:
-    """Convert an awaitable function to a synchronous function.
+    """
+    Convert an awaitable function to a synchronous function.
 
     If used within an asynchronous context, attempts to use the same backend.
     Defaults to asyncio.
 
     Args:
         func: An awaitable function.
```

### Comparing `async_wrapper-0.5.1/src/async_wrapper/convert/main.py` & `async_wrapper-0.5.2/src/async_wrapper/convert/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 ) -> Callable[ParamT, Coroutine[Any, Any, ValueT]]:
     ...  # pragma: no cover
 
 
 def toggle_func(
     func: Callable[ParamT, ValueT] | Callable[ParamT, Coroutine[Any, Any, ValueT]],
 ) -> Callable[ParamT, ValueT] | Callable[ParamT, Coroutine[Any, Any, ValueT]]:
-    """Convert between synchronous and asynchronous functions.
+    """
+    Convert between synchronous and asynchronous functions.
 
     Args:
         func: A function that can be either synchronous or asynchronous.
 
     Returns:
         A function that matches the desired synchronicity,
         either synchronous or asynchronous.
```

### Comparing `async_wrapper-0.5.1/src/async_wrapper/exception.py` & `async_wrapper-0.5.2/src/async_wrapper/exception.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,58 +3,69 @@
 __all__ = [
     "PendingError",
     "QueueError",
     "QueueEmptyError",
     "QueueFullError",
     "QueueClosedError",
     "QueueBrokenError",
+    "QueueRestrictedError",
 ]
 
 
 class PendingError(Exception):
-    """Exception used exclusively for pending values.
+    """
+    Exception used exclusively for pending values.
 
     This exception is used within the context of handling soon values.
     """
 
 
 class QueueError(Exception):
-    """Base exception for queue-related errors.
+    """
+    Base exception for queue-related errors.
 
     This exception serves as the base class for various queue-related exceptions.
     """
 
 
 class QueueEmptyError(QueueError):
-    """Exception raised when attempting to retrieve an item from an empty queue.
+    """
+    Exception raised when attempting to retrieve an item from an empty queue.
 
     This exception occurs when trying to get an item from a queue
     that has no available items.
     """
 
 
 class QueueFullError(QueueError):
-    """Exception raised when attempting to add an item to a full queue.
+    """
+    Exception raised when attempting to add an item to a full queue.
 
     This exception occurs when trying to put an item into a queue
     that has reached its capacity.
     """
 
 
 class QueueClosedError(QueueError):
-    """Error that occurs when attempting to get from or put into a closed queue.
+    """
+    Error that occurs when attempting to get from or put into a closed queue.
 
     This error is different from QueueBrokenError.
         :exc:`QueueBrokenError` is an unintended error.
 
         :exc:`QueueClosedError` is an error deliberately raised.
     """
 
 
 class QueueBrokenError(QueueError):
-    """Error that occurs when trying to get from or put into a closed queue.
+    """
+    Error that occurs when trying to get from or put into a closed queue.
 
     This error is different from QueueClosedError.
         :exc:`QueueClosedError` is an error deliberately raised.
 
         :exc:`QueueBrokenError` is an unintended error.
     """
+
+
+class QueueRestrictedError(QueueError):
+    """queue is restricted but used"""
```

### Comparing `async_wrapper-0.5.1/src/async_wrapper/queue.py` & `async_wrapper-0.5.2/src/async_wrapper/queue.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,25 +7,28 @@
     TYPE_CHECKING,
     Any,
     AsyncContextManager,
     AsyncGenerator,
     ContextManager,
     Generator,
     Generic,
+    Literal,
     TypeVar,
 )
 
 from anyio import WouldBlock, create_memory_object_stream, create_task_group, fail_after
 from anyio.streams.memory import BrokenResourceError, ClosedResourceError, EndOfStream
+from typing_extensions import override
 
 from async_wrapper.exception import (
     QueueBrokenError,
     QueueClosedError,
     QueueEmptyError,
     QueueFullError,
+    QueueRestrictedError,
 )
 
 if sys.version_info < (3, 11):  # pragma: no cover
     from exceptiongroup import ExceptionGroup  # type: ignore
 
 if TYPE_CHECKING:
     from types import TracebackType
@@ -36,18 +39,20 @@
         MemoryObjectStreamStatistics,
     )
     from typing_extensions import Self
 
 __all__ = ["Queue", "create_queue"]
 
 ValueT = TypeVar("ValueT")
+QueueT_co = TypeVar("QueueT_co", covariant=True, bound="Queue")
 
 
 class Queue(Generic[ValueT]):
-    """obtained from :class:`asyncio.Queue`
+    """
+    obtained from :class:`asyncio.Queue`
 
     Example:
         >>> from __future__ import annotations
         >>>
         >>> from typing import Any
         >>>
         >>> import anyio
@@ -62,15 +67,15 @@
         >>>
         >>> async def main() -> None:
         >>>     queue: Queue[Any] = Queue(10)
         >>>
         >>>     async with anyio.create_task_group() as task_group:
         >>>         async with queue.aputter:
         >>>             for i in range(10):
-        >>>                 task_group.start_soon(aput, queue.clone(putter=True), i)
+        >>>                 task_group.start_soon(aput, queue.clone.putter, i)
         >>>
         >>>     async with queue.agetter:
         >>>         result = {x async for x in queue}
         >>>
         >>>     assert result == set(range(10))
         >>>
         >>>
@@ -185,27 +190,29 @@
     def full(self) -> bool:
         """return true if there are maxsize items in the queue."""
         if self.maxsize == math.inf:
             return False
         return self.qsize() >= self.maxsize
 
     async def aget(self, *, timeout: float | None = None) -> ValueT:
-        """remove and return an item from the queue.
+        """
+        remove and return an item from the queue.
 
         Args:
             timeout: error occurs when over timeout. Defaults to None.
 
         Returns:
             item from queue
         """
         with fail_after(timeout):
             return await self._aget()
 
     async def aput(self, value: ValueT, *, timeout: float | None = None) -> None:
-        """put an item into the queue.
+        """
+        put an item into the queue.
 
         Args:
             value: item
             timeout: error occurs when over timeout. Defaults to None.
         """
         with fail_after(timeout):
             await self._aput(value)
@@ -286,37 +293,39 @@
     def _close(self) -> None:
         """close the stream as sync"""
         if self._close_getter:
             self._getter.close()
         if self._close_putter:
             self._putter.close()
 
-    def clone(self, *, putter: bool = False, getter: bool = False) -> Queue[ValueT]:
-        """create clone of this queue.
-
-        Args:
-            putter: if true, clone putter. Defaults to False.
-            getter: if true, clone getter. Defaults to False.
+    @property
+    def clone(self) -> _Clone[ValueT]:
+        """
+        Create a queue factory for generating RestrictedQueue instances.
 
         Returns:
-            clone
+            A queue factory.
+
+        .. versionadded:: 0.5.2
         """
-        try:
-            return self._clone(putter=putter, getter=getter)
-        except (ClosedResourceError, BrokenResourceError) as exc:
-            raise QueueBrokenError from exc
+        return _Clone(self)
 
     def _clone(self, *, putter: bool, getter: bool) -> Queue[ValueT]:
         """create clone of this queue"""
         if self._closed:
             raise QueueClosedError("the queue is already closed")
         if not putter and not getter:
             raise RuntimeError("putter and getter are None.")
-        _putter = self._putter.clone() if putter else self._putter
-        _getter = self._getter.clone() if getter else self._getter
+
+        try:
+            _putter = self._putter.clone() if putter else self._putter
+            _getter = self._getter.clone() if getter else self._getter
+        except (ClosedResourceError, BrokenResourceError) as exc:
+            raise QueueBrokenError from exc
+
         new = Queue(_stream=(_putter, _getter))  # type: ignore
         new._close_putter = putter  # noqa: SLF001
         new._close_getter = getter  # noqa: SLF001
         return new
 
     def statistics(self) -> MemoryObjectStreamStatistics:
         """return statstics from stream"""
@@ -382,20 +391,189 @@
 
     def __len__(self) -> int:
         return self.qsize()
 
     def __repr__(self) -> str:
         max_size = "inf" if self.maxsize == math.inf else self.maxsize
         size = self.qsize()
-        return f"<Queue: max={max_size}, size={size}>"
+        return _render("Queue", max=max_size, size=size)
+
+
+class _RestrictedQueue(Queue[ValueT], Generic[ValueT]):
+    __slots__ = ("_queue", "_do_putter", "_do_getter")
+
+    def __init__(self, queue: Queue[ValueT], *, putter: bool, getter: bool) -> None:
+        self._queue = queue
+        if getter is putter:
+            raise QueueRestrictedError("putter and getter are the same")
+        self._do_putter = putter
+        self._do_getter = getter
+
+    @property
+    def _putter(self) -> MemoryObjectSendStream[ValueT]:
+        self._raise_restricted(putter=True)
+        return self._queue._putter  # noqa: SLF001
+
+    @property
+    def _getter(self) -> MemoryObjectReceiveStream[ValueT]:
+        self._raise_restricted(getter=True)
+        return self._queue._getter  # noqa: SLF001
+
+    @property
+    def _close_getter(self) -> bool:
+        return self._queue._close_getter  # noqa: SLF001
+
+    @property
+    def _close_putter(self) -> bool:
+        return self._queue._close_putter  # noqa: SLF001
+
+    @property
+    def _close_stream(self) -> bool:
+        if self._do_getter:
+            return self._close_getter
+        if self._do_putter:
+            return self._close_putter
+        raise RuntimeError("never")  # pragma: no cover
+
+    @property
+    def _stream(
+        self,
+    ) -> MemoryObjectSendStream[ValueT] | MemoryObjectReceiveStream[ValueT]:
+        if self._do_getter:
+            return self._getter
+        if self._do_putter:
+            return self._putter
+        raise RuntimeError("never")  # pragma: no cover
+
+    @property
+    @override
+    def _closed(self) -> bool:
+        return not self._close_stream or self._stream._closed  # noqa: SLF001
+
+    @override
+    def qsize(self) -> int:
+        return len(self._stream._state.buffer)  # noqa: SLF001
+
+    @property
+    def maxsize(self) -> float:
+        return self._stream._state.max_buffer_size  # noqa: SLF001
+
+    @override
+    async def _aclose(self) -> None:
+        await self._stream.aclose()
+
+    @override
+    def _close(self) -> None:
+        self._stream.close()
+
+    @property
+    @override
+    def clone(self) -> _Clone[Self]:
+        raise TypeError("do not clone restricted queue")
+
+    @override
+    def _clone(self, *, putter: bool, getter: bool) -> Queue[ValueT]:
+        raise TypeError("do not clone restricted queue")
+
+    @override
+    def statistics(self) -> MemoryObjectStreamStatistics:
+        return self._stream.statistics()
+
+    def _raise_restricted(self, *, getter: bool = False, putter: bool = False) -> None:
+        if getter and not self._do_getter:
+            raise QueueRestrictedError("getter is restricted")
+        if putter and not self._do_putter:
+            raise QueueRestrictedError("putter is restricted")
+
+    @override
+    def __exit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
+        try:
+            self.close()
+        finally:
+            self._queue._close_getter = True  # noqa: SLF001
+            self._queue._close_putter = True  # noqa: SLF001
+
+    @override
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
+        try:
+            await self.aclose()
+        finally:
+            self._queue._close_getter = True  # noqa: SLF001
+            self._queue._close_putter = True  # noqa: SLF001
+
+    def __repr__(self) -> str:
+        max_size = "inf" if self.maxsize == math.inf else self.maxsize
+        size = self.qsize()
+        if self._do_getter:
+            where = "getter"
+        elif self._do_putter:
+            where = "putter"
+        else:
+            raise RuntimeError("never")  # pragma: no cover
+        return _render("RestrictedQueue", max=max_size, size=size, where=where)
+
+
+class _Clone(Generic[ValueT]):
+    __slots__ = ("_queue",)
+
+    def __init__(self, queue: Queue[ValueT]) -> None:
+        if queue._closed:  # noqa: SLF001
+            raise QueueClosedError("queue is already closed")
+        self._queue = queue
+
+    def create(self, where: Literal["putter", "getter"]) -> _RestrictedQueue[ValueT]:
+        if where == "putter":
+            return self.putter
+        if where == "getter":
+            return self.getter
+        raise RuntimeError("never")  # pragma: no cover
+
+    @property
+    def putter(self) -> _RestrictedQueue[ValueT]:
+        self._raise_if_closed()
+        new = self._queue._clone(putter=True, getter=False)  # noqa: SLF001
+        return _RestrictedQueue(new, putter=True, getter=False)
+
+    @property
+    def getter(self) -> _RestrictedQueue[ValueT]:
+        self._raise_if_closed()
+        new = self._queue._clone(getter=True, putter=False)  # noqa: SLF001
+        return _RestrictedQueue(new, putter=False, getter=True)
+
+    def _raise_if_closed(self) -> None:
+        if self._queue._closed:  # noqa: SLF001
+            raise QueueClosedError("queue is already closed")
+
+    def __repr__(self) -> str:
+        max_size = "inf" if self._queue.maxsize == math.inf else self._queue.maxsize
+        size = self._queue.qsize()
+        return _render("Clone", max=max_size, size=size)
 
 
 def create_queue(max_size: float | None = None) -> Queue[Any]:
-    """create queue like :class:`asyncio.Queue`
+    """
+    create queue like :class:`asyncio.Queue`
 
     Args:
         max_size: queue size. Defaults to None.
 
     Returns:
         new :obj:`Queue` using :class:`anyio.abc.ObjectStream`
     """
     return Queue(max_size)
+
+
+def _render(name: str, **kwargs: Any) -> str:
+    if kwargs:
+        status = ", ".join(f"{key}={value}" for key, value in kwargs.items())
+        return f"<{name}: {status}>"
+    return f"<{name}>"
```

### Comparing `async_wrapper-0.5.1/src/async_wrapper/task_group/task_group.py` & `async_wrapper-0.5.2/src/async_wrapper/task_group/task_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 ParamT = ParamSpec("ParamT")
 OtherParamT = ParamSpec("OtherParamT")
 
 __all__ = ["TaskGroupWrapper", "create_task_group_wrapper"]
 
 
 class TaskGroupWrapper(_TaskGroup):
-    """wrap :class:`anyio.abc.TaskGroup`
+    """
+    wrap :class:`anyio.abc.TaskGroup`
 
     Example:
         >>> import anyio
         >>>
         >>> from async_wrapper import TaskGroupWrapper
         >>>
         >>>
@@ -117,15 +118,16 @@
     def wrap(
         self,
         func: Callable[ParamT, Awaitable[ValueT_co]],
         semaphore: Semaphore | None = None,
         limiter: CapacityLimiter | None = None,
         lock: Lock | None = None,
     ) -> SoonWrapper[ParamT, ValueT_co]:
-        """Wrap a function to be used within a wrapper.
+        """
+        Wrap a function to be used within a wrapper.
 
         The wrapped function will return a value shortly.
 
         Args:
             func: The target function to be wrapped.
             semaphore: An :obj:`anyio.Semaphore`. Defaults to None.
             limiter: An :obj:`anyio.CapacityLimiter`. Defaults to None.
@@ -203,15 +205,16 @@
 
     def copy(
         self,
         semaphore: Semaphore | None = None,
         limiter: CapacityLimiter | None = None,
         lock: Lock | None = None,
     ) -> Self:
-        """Create a copy of this object.
+        """
+        Create a copy of this object.
 
         Args:
             semaphore: An :obj:`anyio.Semaphore`.
                 If provided, it will overwrite the existing semaphore. Defaults to None.
             limiter: An :obj:`anyio.CapacityLimiter`.
                 If provided, it will overwrite the existing limiter. Defaults to None.
             lock: An :obj:`anyio.Lock`.
@@ -232,15 +235,16 @@
             semaphore=semaphore,
             limiter=limiter,
             lock=lock,
         )
 
 
 def create_task_group_wrapper() -> TaskGroupWrapper:
-    """create new task group wrapper
+    """
+    create new task group wrapper
 
     Returns:
         new :obj:`TaskGroupWrapper`
     """
     return TaskGroupWrapper(_create_task_group())
```

### Comparing `async_wrapper-0.5.1/src/async_wrapper/task_group/value.py` & `async_wrapper-0.5.2/src/async_wrapper/task_group/value.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,29 +8,42 @@
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 Pending = local()
 
 __all__ = ["SoonValue"]
 
 
 class SoonValue(Generic[ValueT_co]):
-    """will get value soon"""
+    """A class representing a value that will be available soon."""
 
     __slots__ = ("_value",)
 
     def __init__(self) -> None:
         self._value: ValueT_co | local = Pending
 
     def __repr__(self) -> str:
         status = "pending" if self._value is Pending else "done"
         return f"<SoonValue: status={status}>"
 
     @property
     def value(self) -> ValueT_co:
-        """soon value"""
+        """
+        Gets the soon-to-be available value.
+
+        Raises:
+            PendingError: Raised if the value is not yet available.
+
+        Returns:
+            The soon-to-be available value.
+        """
         if self._value is Pending:
             raise PendingError
         return self._value  # type: ignore
 
     @property
     def is_ready(self) -> bool:
-        """value status"""
+        """
+        Checks if the value is ready.
+
+        Returns:
+            True if the value is not pending, False otherwise.
+        """
         return self._value is not Pending
```

### Comparing `async_wrapper-0.5.1/src/async_wrapper/wait.py` & `async_wrapper-0.5.2/src/async_wrapper/wait.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 Pending = local()
 
 
 class Waiter(Event):
-    """wait wrapper
+    """
+    wait wrapper
 
     Example:
         >>> import anyio
         >>>
         >>> from async_wrapper import Waiter
         >>>
         >>>
@@ -84,15 +85,16 @@
         )
         return self
 
     def __copy__(self) -> Self:
         return self.copy()
 
     def copy(self, *args: Any, **kwargs: Any) -> Self:
-        """create new event
+        """
+        create new event
 
         Returns:
             new :obj:`Waiter`
         """
         if not args:
             args = tuple(self._args)
         if not kwargs:
@@ -124,15 +126,16 @@
 
     @override
     def statistics(self) -> EventStatistics:
         return self._event.statistics()
 
 
 class Completed:
-    """like :func:`asyncio.as_completed`
+    """
+    like :func:`asyncio.as_completed`
 
     Example:
         >>> from __future__ import annotations
         >>>
         >>> import anyio
         >>>
         >>> from async_wrapper import Completed
@@ -222,15 +225,16 @@
     def start_soon(
         self,
         task_group: TaskGroup | None,
         func: Callable[..., Awaitable[Any]],
         *args: Any,
         name: Any = None,
     ) -> None:
-        """Start a coroutine in a task group,
+        """
+        Start a coroutine in a task group,
         similar to :meth:`anyio.abc.TaskGroup.start_soon`.
 
         If a task group is already provided,
         the task_group parameter should be the same object.
 
         Args:
             task_group: An :class:`anyio.abc.TaskGroup`. Defaults to None.
@@ -301,15 +305,16 @@
 
 async def wait_for(
     event: Event | Iterable[Event],
     func: Callable[ParamT, Awaitable[ValueT_co]],
     *args: ParamT.args,
     **kwargs: ParamT.kwargs,
 ) -> ValueT_co:
-    """Wait for an event before executing an awaitable function.
+    """
+    Wait for an event before executing an awaitable function.
 
     like :func:`asyncio.wait_for`
 
     Args:
         event: An :obj:`anyio.Event` or an iterable of events.
         func: An awaitable function to be executed.
```

### Comparing `async_wrapper-0.5.1/PKG-INFO` & `async_wrapper-0.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.5.1
+Version: 0.5.2
 Summary: async wrapper
 Home-page: https://async-wrapper.readthedocs.io/
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,15 @@
 Requires-Dist: uvloop (>=0.17.0,<0.18.0) ; (platform_system != "Windows") and (extra == "uvloop")
 Project-URL: Repository, https://github.com/phi-friday/async-wrapper
 Description-Content-Type: text/markdown
 
 # async-wrapper
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Documentation Status](https://readthedocs.org/projects/async-wrapper/badge/?version=latest)](https://async-wrapper.readthedocs.io/en/latest/?badge=latest)
 [![github action](https://github.com/phi-friday/async-wrapper/actions/workflows/check.yaml/badge.svg?event=push&branch=main)](#)
 [![codecov](https://codecov.io/gh/phi-friday/async-wrapper/branch/main/graph/badge.svg?token=R1RAQ5F0YD)](https://codecov.io/gh/phi-friday/async-wrapper)
 [![PyPI version](https://badge.fury.io/py/async-wrapper.svg)](https://badge.fury.io/py/async-wrapper)
 [![python version](https://img.shields.io/pypi/pyversions/async_wrapper.svg)](#)
 
 ## how to install
 ```shell
```

