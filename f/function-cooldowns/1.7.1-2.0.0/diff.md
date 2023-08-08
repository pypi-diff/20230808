# Comparing `tmp/function-cooldowns-1.7.1.tar.gz` & `tmp/function-cooldowns-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function-cooldowns-1.7.1.tar", last modified: Thu Apr 27 10:17:41 2023, max compression
+gzip compressed data, was "function-cooldowns-2.0.0.tar", last modified: Tue Aug  8 01:24:31 2023, max compression
```

## Comparing `function-cooldowns-1.7.1.tar` & `function-cooldowns-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,36 @@
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-27 10:17:41.307673 function-cooldowns-1.7.1/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1211 2022-06-02 07:37:26.000000 function-cooldowns-1.7.1/LICENSE
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1680 2023-04-27 10:17:41.307673 function-cooldowns-1.7.1/PKG-INFO
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-27 10:17:41.303673 function-cooldowns-1.7.1/cooldowns/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1415 2023-04-27 10:17:31.000000 function-cooldowns-1.7.1/cooldowns/__init__.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-27 10:17:41.303673 function-cooldowns-1.7.1/cooldowns/buckets/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      182 2022-06-02 07:37:26.000000 function-cooldowns-1.7.1/cooldowns/buckets/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2154 2022-10-30 10:38:23.000000 function-cooldowns-1.7.1/cooldowns/buckets/hashable_arguments.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      911 2022-06-02 07:37:26.000000 function-cooldowns-1.7.1/cooldowns/buckets/main.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1134 2022-06-02 07:37:26.000000 function-cooldowns-1.7.1/cooldowns/buckets/slash.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    13914 2023-04-27 09:26:19.000000 function-cooldowns-1.7.1/cooldowns/cooldown.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     3640 2023-04-27 10:13:38.000000 function-cooldowns-1.7.1/cooldowns/cooldown_times_per.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2202 2023-02-14 11:31:54.000000 function-cooldowns-1.7.1/cooldowns/exceptions.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2905 2023-04-27 10:17:31.000000 function-cooldowns-1.7.1/cooldowns/persistence.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-27 10:17:41.303673 function-cooldowns-1.7.1/cooldowns/protocols/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       82 2022-06-02 07:37:26.000000 function-cooldowns-1.7.1/cooldowns/protocols/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      359 2022-06-02 07:37:26.000000 function-cooldowns-1.7.1/cooldowns/protocols/bucket.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     6139 2023-02-14 11:31:54.000000 function-cooldowns-1.7.1/cooldowns/static_cooldown.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2273 2023-02-14 11:31:54.000000 function-cooldowns-1.7.1/cooldowns/static_times_per.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     9214 2023-02-14 11:31:54.000000 function-cooldowns-1.7.1/cooldowns/utils.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-04-27 10:17:41.307673 function-cooldowns-1.7.1/function_cooldowns.egg-info/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1680 2023-04-27 10:17:40.000000 function-cooldowns-1.7.1/function_cooldowns.egg-info/PKG-INFO
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      572 2023-04-27 10:17:41.000000 function-cooldowns-1.7.1/function_cooldowns.egg-info/SOURCES.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)        1 2023-04-27 10:17:40.000000 function-cooldowns-1.7.1/function_cooldowns.egg-info/dependency_links.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       10 2023-04-27 10:17:41.000000 function-cooldowns-1.7.1/function_cooldowns.egg-info/top_level.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       38 2023-04-27 10:17:41.307673 function-cooldowns-1.7.1/setup.cfg
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1496 2022-06-02 07:37:26.000000 function-cooldowns-1.7.1/setup.py
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-08-08 01:24:31.241922 function-cooldowns-2.0.0/
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1211 2023-08-08 00:53:33.000000 function-cooldowns-2.0.0/LICENSE
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1643 2023-08-08 01:24:31.241922 function-cooldowns-2.0.0/PKG-INFO
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-08-08 01:24:31.241922 function-cooldowns-2.0.0/cooldowns/
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1527 2023-08-08 01:21:56.000000 function-cooldowns-2.0.0/cooldowns/__init__.py
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-08-08 01:24:31.241922 function-cooldowns-2.0.0/cooldowns/buckets/
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      182 2023-08-08 00:53:33.000000 function-cooldowns-2.0.0/cooldowns/buckets/__init__.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2154 2023-08-08 00:53:33.000000 function-cooldowns-2.0.0/cooldowns/buckets/hashable_arguments.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      911 2023-08-08 00:53:33.000000 function-cooldowns-2.0.0/cooldowns/buckets/main.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1134 2023-08-08 00:53:33.000000 function-cooldowns-2.0.0/cooldowns/buckets/slash.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    14372 2023-08-08 01:21:56.000000 function-cooldowns-2.0.0/cooldowns/cooldown.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     3665 2023-08-08 01:21:56.000000 function-cooldowns-2.0.0/cooldowns/cooldown_times_per.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      319 2023-08-08 01:21:56.000000 function-cooldowns-2.0.0/cooldowns/date_util.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2218 2023-08-08 01:21:56.000000 function-cooldowns-2.0.0/cooldowns/exceptions.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2862 2023-08-08 01:21:56.000000 function-cooldowns-2.0.0/cooldowns/persistence.py
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-08-08 01:24:31.241922 function-cooldowns-2.0.0/cooldowns/protocols/
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      141 2023-08-08 01:21:56.000000 function-cooldowns-2.0.0/cooldowns/protocols/__init__.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      701 2023-08-08 01:21:56.000000 function-cooldowns-2.0.0/cooldowns/protocols/bucket.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     6284 2023-08-08 01:21:56.000000 function-cooldowns-2.0.0/cooldowns/static_cooldown.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2289 2023-08-08 01:21:56.000000 function-cooldowns-2.0.0/cooldowns/static_times_per.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     9452 2023-08-08 01:21:56.000000 function-cooldowns-2.0.0/cooldowns/utils.py
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-08-08 01:24:31.241922 function-cooldowns-2.0.0/function_cooldowns.egg-info/
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1643 2023-08-08 01:24:31.000000 function-cooldowns-2.0.0/function_cooldowns.egg-info/PKG-INFO
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      792 2023-08-08 01:24:31.000000 function-cooldowns-2.0.0/function_cooldowns.egg-info/SOURCES.txt
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)        1 2023-08-08 01:24:31.000000 function-cooldowns-2.0.0/function_cooldowns.egg-info/dependency_links.txt
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       10 2023-08-08 01:24:31.000000 function-cooldowns-2.0.0/function_cooldowns.egg-info/top_level.txt
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       38 2023-08-08 01:24:31.241922 function-cooldowns-2.0.0/setup.cfg
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1496 2023-08-08 00:53:33.000000 function-cooldowns-2.0.0/setup.py
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-08-08 01:24:31.241922 function-cooldowns-2.0.0/tests/
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      900 2023-08-08 00:53:33.000000 function-cooldowns-2.0.0/tests/test_callable_on_cooldown.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     9804 2023-08-08 01:21:56.000000 function-cooldowns-2.0.0/tests/test_cooldown.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1750 2023-08-08 00:53:33.000000 function-cooldowns-2.0.0/tests/test_cooldown_times_per.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     3846 2023-08-08 01:21:56.000000 function-cooldowns-2.0.0/tests/test_persistence.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    10398 2023-08-08 01:21:56.000000 function-cooldowns-2.0.0/tests/test_static_cooldown.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     5813 2023-08-08 01:21:56.000000 function-cooldowns-2.0.0/tests/test_static_times_per.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     3870 2023-08-08 01:21:56.000000 function-cooldowns-2.0.0/tests/test_util.py
```

### Comparing `function-cooldowns-1.7.1/LICENSE` & `function-cooldowns-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `function-cooldowns-1.7.1/PKG-INFO` & `function-cooldowns-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: function-cooldowns
-Version: 1.7.1
+Version: 2.0.0
 Summary: A simplistic decorator based approach to rate limiting function calls.
 Author: Skelmis
 Author-email: ethan@koldfusion.xyz
-License: UNKNOWN
 Project-URL: Issue tracker, https://github.com/Skelmis/Function-Cooldowns/issues
 Project-URL: Documentation, https://function-cooldowns.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/Skelmis/Function-Cooldowns
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -60,9 +58,7 @@
 ---
 
 ### Funding
 
 Want a feature added quickly? Want me to help build your software using this?
 
 Sponsor me [here](https://github.com/sponsors/Skelmis)
-
-
```

### Comparing `function-cooldowns-1.7.1/cooldowns/__init__.py` & `function-cooldowns-2.0.0/cooldowns/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import namedtuple
 
 from .buckets import CooldownBucket, SlashBucket
-from .protocols import CooldownBucketProtocol
+from .protocols import CooldownBucketProtocol, AsyncCooldownBucketProtocol
 from .cooldown import Cooldown, cooldown, shared_cooldown
 from .static_cooldown import StaticCooldown, static_cooldown
 from .cooldown_times_per import CooldownTimesPer
 from .static_times_per import StaticTimesPer
 from .exceptions import (
     CallableOnCooldown,
     NoRegisteredCooldowns,
@@ -17,19 +17,21 @@
     reset_cooldown,
     reset_cooldowns,
     reset_bucket,
     get_cooldown,
     define_shared_cooldown,
     get_shared_cooldown,
     define_shared_static_cooldown,
+    get_all_cooldowns,
 )
 
 __all__ = (
     "CooldownBucket",
     "SlashBucket",
+    "AsyncCooldownBucketProtocol",
     "Cooldown",
     "cooldown",
     "shared_cooldown",
     "CooldownTimesPer",
     "CooldownBucketProtocol",
     "CallableOnCooldown",
     "NoRegisteredCooldowns",
@@ -42,12 +44,13 @@
     "get_cooldown",
     "define_shared_cooldown",
     "get_shared_cooldown",
     "StaticTimesPer",
     "StaticCooldown",
     "static_cooldown",
     "define_shared_static_cooldown",
+    "get_all_cooldowns",
 )
 
-__version__ = "1.7.1"
+__version__ = "2.0.0"
 VersionInfo = namedtuple("VersionInfo", "major minor micro releaselevel serial")
-version_info = VersionInfo(major=1, minor=7, micro=1, releaselevel="final", serial=0)
+version_info = VersionInfo(major=0, minor=0, micro=0, releaselevel="final", serial=0)
```

### Comparing `function-cooldowns-1.7.1/cooldowns/buckets/hashable_arguments.py` & `function-cooldowns-2.0.0/cooldowns/buckets/hashable_arguments.py`

 * *Files identical despite different names*

### Comparing `function-cooldowns-1.7.1/cooldowns/buckets/main.py` & `function-cooldowns-2.0.0/cooldowns/buckets/main.py`

 * *Files identical despite different names*

### Comparing `function-cooldowns-1.7.1/cooldowns/buckets/slash.py` & `function-cooldowns-2.0.0/cooldowns/buckets/slash.py`

 * *Files identical despite different names*

### Comparing `function-cooldowns-1.7.1/cooldowns/cooldown.py` & `function-cooldowns-2.0.0/cooldowns/cooldown.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,41 +14,41 @@
     MaybeCoro,
     maybe_coro,
     default_check,
     COOLDOWN_ID,
 )
 from . import CooldownBucket, utils
 from .buckets import _HashableArguments
-from .protocols import CooldownBucketProtocol
+from .protocols import CooldownBucketProtocol, AsyncCooldownBucketProtocol
 
 logger = getLogger(__name__)
 
 T = TypeVar("T", bound=_HashableArguments)
 TP = TypeVar("TP", bound=CooldownTimesPer)
 
 
 def cooldown(
     limit: int,
     time_period: Union[float, datetime.timedelta],
-    bucket: CooldownBucketProtocol,
+    bucket: Union[CooldownBucketProtocol, AsyncCooldownBucketProtocol],
     check: Optional[MaybeCoro] = default_check,
     *,
     cooldown_id: Optional[COOLDOWN_ID] = None,
 ):
     """
     Wrap this Callable in a cooldown.
 
     Parameters
     ----------
     limit: int
         How many call's can be made in the time
         period specified by ``time_period``
     time_period: Union[float, datetime.timedelta]
         The time period related to ``limit``. This is seconds.
-    bucket: CooldownBucketProtocol
+    bucket: Union[CooldownBucketProtocol, AsyncCooldownBucketProtocol]
         The :class:`Bucket` implementation to use
         as a bucket to separate cooldown buckets.
     check: Optional[MaybeCoro]
         A Callable which dictates whether
         to apply the cooldown on current invoke.
 
         If this Callable returns a truthy value,
@@ -172,29 +172,31 @@
 class Cooldown:
     """Represents a cooldown for any given :type:`Callable`."""
 
     def __init__(
         self,
         limit: int,
         time_period: Union[float, datetime.timedelta],
-        bucket: Optional[CooldownBucketProtocol] = None,
+        bucket: Optional[
+            Union[CooldownBucketProtocol, AsyncCooldownBucketProtocol]
+        ] = None,
         func: Optional[Callable] = None,
         *,
         cooldown_id: Optional[Union[int, str]] = None,
         check: Optional[MaybeCoro] = default_check,
     ) -> None:
         """
         Parameters
         ----------
         limit: int
             How many call's can be made in the time
             period specified by ``time_period``
         time_period: Union[float, datetime.timedelta]
             The time period related to ``limit``. This is seconds.
-        bucket: Optional[CooldownBucketProtocol]
+        bucket: Optional[Union[CooldownBucketProtocol, AsyncCooldownBucketProtocol]]
             The :class:`Bucket` implementation to use
             as a bucket to separate cooldown buckets.
 
             Defaults to :class:`CooldownBucket.all`
         func: Optional[Callable]
             The function this cooldown is attached to
         cooldown_id: Optional[Union[int, str]]
@@ -223,17 +225,19 @@
             if isinstance(time_period, (float, int))
             else time_period.total_seconds()
         )
         self.check: MaybeCoro = check
         self.cooldown_id: Optional[Union[int, str]] = cooldown_id
 
         self._func: Optional[Callable] = func
-        self._bucket: CooldownBucketProtocol = bucket
+        self._bucket: Union[
+            CooldownBucketProtocol, AsyncCooldownBucketProtocol
+        ] = bucket
         self.pending_reset: bool = False
-        self._last_bucket: Optional[_HashableArguments] = None
+        self._raw_last_bucket: dict = {"args": [], "kwargs": {}}
 
         self._cache: Dict[_HashableArguments, TP] = {}
 
         # How long to sleep between attempt cache clean calls
         self._cache_clean_eagerness: int = 250
         self._clean_task: Optional[asyncio.Task] = None
         # self._clean_task = asyncio.create_task(self._keep_buckets_clear())
@@ -241,23 +245,26 @@
         if cooldown_id:
             utils.shared_cooldown_refs[cooldown_id] = self
 
     async def __aenter__(self) -> "Cooldown":
         if not self._clean_task:
             self._clean_task = asyncio.create_task(self._keep_buckets_clear())
 
-        bucket: TP = self._get_cooldown_for_bucket(self._last_bucket)
+        last_bucket = await self.get_bucket(
+            *self._raw_last_bucket["args"], **self._raw_last_bucket["kwargs"]
+        )
+        bucket: TP = self._get_cooldown_for_bucket(last_bucket)
         async with bucket:
             return self
 
     async def __aexit__(self, *_) -> None:
         ...
 
     def __call__(self, *args, **kwargs):
-        self._last_bucket = self.get_bucket(*args, **kwargs)
+        self._raw_last_bucket = {"args": args, "kwargs": kwargs}
         return self
 
     def _get_cooldown_for_bucket(
         self, bucket: _HashableArguments, *, raise_on_create: bool = False
     ) -> TP:
         try:
             return self._cache[bucket]
@@ -286,15 +293,15 @@
             The internal :py:class:`CooldownTimesPer` object
         """
         try:
             return self._get_cooldown_for_bucket(bucket, raise_on_create=True)
         except NonExistent:
             return None
 
-    def get_bucket(self, *args, **kwargs) -> _HashableArguments:
+    async def get_bucket(self, *args, **kwargs) -> _HashableArguments:
         """
         Return the given bucket for some given arguments.
 
         This uses the underlying :class:`CooldownBucket`
         and will return a :class:`_HashableArguments`
         instance which is inline with how Cooldown's function.
 
@@ -309,15 +316,15 @@
         -------
         _HashableArguments
             An internally correct representation
             of a bucket for the given arguments.
 
             This can then be used in :meth:`Cooldown.clear` calls.
         """
-        data = self._bucket.process(*args, **kwargs)
+        data = await maybe_coro(self._bucket.process, *args, **kwargs)
         if self._bucket is CooldownBucket.all:
             return _HashableArguments(*data[0], **data[1])
 
         elif self._bucket is CooldownBucket.args:
             return _HashableArguments(*data)
 
         elif self._bucket is CooldownBucket.kwargs:
@@ -367,15 +374,15 @@
             # is not tracking anything
             _bucket: TP = self._cache[bucket]
             if not _bucket.has_cooldown or force_evict:
                 del self._cache[bucket]
         except KeyError:
             pass
 
-    def remaining_calls(self, *args, **kwargs) -> int:
+    async def remaining_calls(self, *args, **kwargs) -> int:
         """
         Given a :type:`Callable`, return the amount of remaining
         available calls before these arguments will result
         in the callable being rate-limited.
 
         Parameters
         ----------
@@ -386,15 +393,15 @@
 
         Returns
         -------
         int
             How many more times this :type:`Callable`
             can be called without being rate-limited.
         """
-        bucket: _HashableArguments = self.get_bucket(*args, **kwargs)
+        bucket: _HashableArguments = await self.get_bucket(*args, **kwargs)
         try:
             cooldown_times_per: TP = self._get_cooldown_for_bucket(
                 bucket, raise_on_create=True
             )
         except NonExistent:
             return self.limit
 
@@ -426,15 +433,15 @@
         """
         _unpickle_cooldown(self, state)
 
     def __repr__(self) -> str:
         return f"Cooldown(limit={self.limit}, time_period={self.time_period}, func={self._func})"
 
     @property
-    def bucket(self) -> CooldownBucketProtocol:
+    def bucket(self) -> Union[CooldownBucketProtocol, AsyncCooldownBucketProtocol]:
         """Returns the underlying bucket to process cooldowns against."""
         return self._bucket
 
     @property
     def func(self) -> Optional[Callable]:
         """Returns the wrapped function."""
         return self._func
```

### Comparing `function-cooldowns-1.7.1/cooldowns/cooldown_times_per.py` & `function-cooldowns-2.0.0/cooldowns/cooldown_times_per.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import datetime
 import pickle
 from asyncio import get_event_loop, AbstractEventLoop, Queue
 from typing import TYPE_CHECKING, Optional, Dict, TypeVar, TypedDict
 
 from cooldowns.exceptions import CallableOnCooldown
+from cooldowns.date_util import _utc_now
 
 if TYPE_CHECKING:
     from cooldowns import Cooldown
 
 
 class CooldownTimesPer:
     def __init__(
@@ -50,15 +51,15 @@
             raise CallableOnCooldown(
                 self._cooldown.func, self._cooldown, self.next_reset
             )
 
         self.current -= 1
 
         self._next_reset.put_nowait(
-            datetime.datetime.utcnow() + datetime.timedelta(seconds=self.time_period)
+            _utc_now() + datetime.timedelta(seconds=self.time_period)
         )
         self.loop.call_later(self.time_period, self._reset_invoke)
 
         return self
 
     async def __aexit__(self, *_) -> None:
         ...
```

### Comparing `function-cooldowns-1.7.1/cooldowns/exceptions.py` & `function-cooldowns-2.0.0/cooldowns/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 import datetime
-from typing import Callable, TYPE_CHECKING, Optional
+from typing import Callable, TYPE_CHECKING
+
+from cooldowns.date_util import _utc_now
 
 if TYPE_CHECKING:
     from cooldowns import Cooldown
 
 
 class BaseCooldownException(Exception):
     """A base exception handler."""
@@ -78,13 +80,13 @@
         float
             How many seconds before you can retry this
 
             .. note::
 
                 This will be 0 if you can retry now
         """
-        now = datetime.datetime.utcnow()
+        now = _utc_now()
         if now > self.resets_at:
             return 0
 
         gap: datetime.timedelta = self.resets_at - now
         return gap.total_seconds()
```

### Comparing `function-cooldowns-1.7.1/cooldowns/persistence.py` & `function-cooldowns-2.0.0/cooldowns/persistence.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import pickle
 import typing
 from asyncio import Queue
 import datetime
 from typing import TypedDict, Union, Optional, Dict, List
 
+from cooldowns.date_util import _utc_now, _utc_from_timestamp
+
 if typing.TYPE_CHECKING:
     from cooldowns import Cooldown, CooldownTimesPer
 
 
 class CTPState(TypedDict):
     limit: int
     time_period: float
@@ -52,15 +54,15 @@
         "cache": cache,
     }
     return state
 
 
 def _check_expired(time: datetime.datetime) -> bool:
     """Returns `True` if in the past, `False` otherwise"""
-    return datetime.datetime.utcnow() > time
+    return _utc_now() > time
 
 
 def _unpickle_cooldown(cooldown: Cooldown, state: State) -> None:
     from cooldowns import CooldownTimesPer
 
     cooldown.limit = state["limit"]
     cooldown.cooldown_id = state["cooldown_id"]
@@ -75,23 +77,21 @@
             limit=v["limit"],
             time_period=v["time_period"],
             _cooldown=cooldown,
         )
         cooldown_times_per.current = v["current"]
 
         for epoch in v["next_reset"]:
-            epoch_time = datetime.datetime.utcfromtimestamp(
-                epoch,  # tz=datetime.timezone.utc
-            )
+            epoch_time = _utc_from_timestamp(epoch)
             if _check_expired(epoch_time):
                 # No longer relevant
                 cooldown_times_per.current += 1
                 continue
 
-            current_time = datetime.datetime.utcnow()
+            current_time = _utc_now()
             cooldown_times_per._next_reset.put_nowait(epoch_time)
             cooldown_times_per.loop.call_later(
                 (epoch_time - current_time).total_seconds(),
                 cooldown_times_per._reset_invoke,
             )
 
         cache[hashable_arguments] = cooldown_times_per
```

### Comparing `function-cooldowns-1.7.1/cooldowns/static_cooldown.py` & `function-cooldowns-2.0.0/cooldowns/static_cooldown.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import asyncio
 import datetime
 import functools
 from typing import List, Callable, Optional, Union
 
-from . import Cooldown, CooldownBucketProtocol, utils
+from . import Cooldown, utils
 from .buckets import _HashableArguments
 from .cooldown import TP
 from .exceptions import NonExistent
+from .protocols import AsyncCooldownBucketProtocol, CooldownBucketProtocol
 from .static_times_per import StaticTimesPer
 from .utils import MaybeCoro, default_check, COOLDOWN_ID, maybe_coro
 
 
 def static_cooldown(
     limit: int,
     reset_times: Union[datetime.time, List[datetime.time]],
-    bucket: CooldownBucketProtocol,
+    bucket: Union[CooldownBucketProtocol, AsyncCooldownBucketProtocol],
     check: Optional[MaybeCoro] = default_check,
     *,
     cooldown_id: Optional[COOLDOWN_ID] = None,
 ):
     """
     Parameters
     ----------
@@ -111,15 +112,17 @@
 class StaticCooldown(Cooldown):
     """A cooldown which implements a set amount of cooldown reset times per day."""
 
     def __init__(
         self,
         limit: int,
         reset_times: Union[datetime.time, List[datetime.time]],
-        bucket: Optional[CooldownBucketProtocol] = None,
+        bucket: Optional[
+            Union[CooldownBucketProtocol, AsyncCooldownBucketProtocol]
+        ] = None,
         func: Optional[Callable] = None,
         *,
         cooldown_id: Optional[Union[int, str]] = None,
         check: Optional[MaybeCoro] = default_check,
     ) -> None:
         """
         Parameters
```

### Comparing `function-cooldowns-1.7.1/cooldowns/static_times_per.py` & `function-cooldowns-2.0.0/cooldowns/static_times_per.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import datetime
 from typing import TYPE_CHECKING, List
 
 from .cooldown_times_per import CooldownTimesPer
 from .exceptions import CallableOnCooldown
+from .date_util import _utc_now
 
 if TYPE_CHECKING:
     from cooldowns import Cooldown
 
 
 class StaticTimesPer(CooldownTimesPer):
     """A cooldown which implements a set amount of cooldown reset times."""
@@ -66,14 +67,14 @@
         if self.current == 0:
             raise CallableOnCooldown(
                 self._cooldown.func, self._cooldown, self.next_reset
             )
 
         self.current -= 1
 
-        now = datetime.datetime.utcnow()
+        now = _utc_now()
         reset: datetime.datetime = self.get_next_reset(now)
 
         self._next_reset.put_nowait(reset)
         self.loop.call_later((reset - now).total_seconds(), self._reset_invoke)
 
         return self
```

### Comparing `function-cooldowns-1.7.1/cooldowns/utils.py` & `function-cooldowns-2.0.0/cooldowns/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 from cooldowns.exceptions import (
     NoRegisteredCooldowns,
     NonExistent,
     CooldownAlreadyExists,
 )
 
 if TYPE_CHECKING:
-    from cooldowns import Cooldown, CooldownBucketProtocol, StaticCooldown
+    from cooldowns import (
+        Cooldown,
+        CooldownBucketProtocol,
+        AsyncCooldownBucketProtocol,
+        StaticCooldown,
+    )
 
     CooldownT = Union[Cooldown, StaticCooldown]
 
 # hA! Hey you, come say hi :O
 COOLDOWN_ID = Union[int, str]
 # A 'global state' of sorts
 shared_cooldown_refs: Dict[COOLDOWN_ID, CooldownT] = {}
@@ -38,15 +43,15 @@
     cooldowns: List[CooldownT] = getattr(func, "_cooldowns")
     if not cooldowns:
         raise NoRegisteredCooldowns
 
     return cooldowns
 
 
-def get_remaining_calls(func: MaybeCoro, *args, **kwargs) -> int:
+async def get_remaining_calls(func: MaybeCoro, *args, **kwargs) -> int:
     """
     Given a `Callable`, return the amount of remaining
     available calls before these arguments will result
     in the callable being rate-limited.
 
     Parameters
     ----------
@@ -72,15 +77,15 @@
     -----
     This aggregates all attached cooldowns
     and returns the lowest remaining amount.
     """
     cooldowns: List[CooldownT] = _get_cooldowns_or_raise(func)
 
     remaining: List[int] = [
-        cooldown.remaining_calls(*args, **kwargs) for cooldown in cooldowns
+        await cooldown.remaining_calls(*args, **kwargs) for cooldown in cooldowns
     ]
     return min(remaining)
 
 
 def reset_cooldowns(func: MaybeCoro):
     """
     Reset all cooldown's on this `Callable`
@@ -98,15 +103,15 @@
         The func has no cooldown's attached.
     """
     cooldowns: List[CooldownT] = _get_cooldowns_or_raise(func)
     for cooldown in cooldowns:
         cooldown.clear(force_evict=True)
 
 
-def reset_bucket(func: MaybeCoro, *args, **kwargs):
+async def reset_bucket(func: MaybeCoro, *args, **kwargs):
     """
     Reset all buckets matching the provided arguments.
 
     Parameters
     ----------
     func: MaybeCoro
         The func with cooldowns we should reset.
@@ -117,15 +122,15 @@
 
     Notes
     -----
     Does nothing if it resets nothing.
     """
     cooldowns: List[CooldownT] = _get_cooldowns_or_raise(func)
     for cooldown in cooldowns:
-        bucket = cooldown.get_bucket(*args, **kwargs)
+        bucket = await cooldown.get_bucket(*args, **kwargs)
         try:
             cooldown._get_cooldown_for_bucket(bucket, raise_on_create=True)
         except NonExistent:
             continue
         else:
             cooldown.clear(bucket, force_evict=True)
 
@@ -207,15 +212,15 @@
     """
     return _get_cooldowns_or_raise(func)
 
 
 def define_shared_cooldown(
     limit: int,
     time_period: float,
-    bucket: CooldownBucketProtocol,
+    bucket: Union[CooldownBucketProtocol, AsyncCooldownBucketProtocol],
     cooldown_id: COOLDOWN_ID,
     *,
     check: Optional[MaybeCoro] = default_check,
 ):
     """
     Define a global cooldown which can be used to ratelimit
     1 or more callables under the same situations.
@@ -225,15 +230,15 @@
     Parameters
     ----------
     limit: int
         How many call's can be made in the time
         period specified by ``time_period``
     time_period: float
         The time period related to ``limit``
-    bucket: CooldownBucketProtocol
+    bucket: Union[CooldownBucketProtocol, AsyncCooldownBucketProtocol]
         The :class:`Bucket` implementation to use
         as a bucket to separate cooldown buckets.
     cooldown_id: Union[int, str]
         The ID used to refer to this when defining a shared_cooldown
 
         This should be unique globally,
         behaviour is not guaranteed if not unique.
@@ -270,15 +275,15 @@
     )
     shared_cooldown_refs[cooldown_id] = cooldown
 
 
 def define_shared_static_cooldown(
     limit: int,
     reset_times: Union[datetime.time, List[datetime.time]],
-    bucket: CooldownBucketProtocol,
+    bucket: Union[CooldownBucketProtocol, AsyncCooldownBucketProtocol],
     cooldown_id: COOLDOWN_ID,
     *,
     check: Optional[MaybeCoro] = default_check,
 ):
     """
     Define a global cooldown which can be used to ratelimit
     1 or more callables under the same situations.
@@ -289,15 +294,15 @@
     ----------
     limit: int
         How many call's can be made in the time
         period specified by ``time_period``
     reset_times: Union[datetime.time, List[datetime.time]]
         A time or list of the possible
         times in the day to reset cooldowns at
-    bucket: CooldownBucketProtocol
+    bucket: Union[CooldownBucketProtocol, AsyncCooldownBucketProtocol]
         The :class:`Bucket` implementation to use
         as a bucket to separate cooldown buckets.
     cooldown_id: Union[int, str]
         The ID used to refer to this when defining a shared_cooldown
 
         This should be unique globally,
         behaviour is not guaranteed if not unique.
```

### Comparing `function-cooldowns-1.7.1/function_cooldowns.egg-info/PKG-INFO` & `function-cooldowns-2.0.0/function_cooldowns.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: function-cooldowns
-Version: 1.7.1
+Version: 2.0.0
 Summary: A simplistic decorator based approach to rate limiting function calls.
 Author: Skelmis
 Author-email: ethan@koldfusion.xyz
-License: UNKNOWN
 Project-URL: Issue tracker, https://github.com/Skelmis/Function-Cooldowns/issues
 Project-URL: Documentation, https://function-cooldowns.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/Skelmis/Function-Cooldowns
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -60,9 +58,7 @@
 ---
 
 ### Funding
 
 Want a feature added quickly? Want me to help build your software using this?
 
 Sponsor me [here](https://github.com/sponsors/Skelmis)
-
-
```

### Comparing `function-cooldowns-1.7.1/setup.py` & `function-cooldowns-2.0.0/setup.py`

 * *Files identical despite different names*

