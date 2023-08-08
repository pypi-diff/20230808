# Comparing `tmp/wikichangewatcher-0.2.0-py3-none-any.whl.zip` & `tmp/wikichangewatcher-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 11888 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      498 b- defN 23-Aug-06 18:46 wikichangewatcher/__init__.py
--rw-rw-rw-  2.0 fat    12743 b- defN 23-Aug-06 18:09 wikichangewatcher/wikichangewatcher.py
--rw-rw-rw-  2.0 fat    10761 b- defN 23-Aug-06 18:54 wikichangewatcher-0.2.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    16752 b- defN 23-Aug-06 18:54 wikichangewatcher-0.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-06 18:54 wikichangewatcher-0.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-06 18:54 wikichangewatcher-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      619 b- defN 23-Aug-06 18:54 wikichangewatcher-0.2.0.dist-info/RECORD
-7 files, 41483 bytes uncompressed, 10782 bytes compressed:  74.0%
+Zip file size: 13022 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      848 b- defN 23-Aug-07 02:46 wikichangewatcher/__init__.py
+-rw-rw-rw-  2.0 fat    16533 b- defN 23-Aug-07 02:30 wikichangewatcher/wikichangewatcher.py
+-rw-rw-rw-  2.0 fat    10761 b- defN 23-Aug-07 02:52 wikichangewatcher-0.2.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    16706 b- defN 23-Aug-07 02:52 wikichangewatcher-0.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-07 02:52 wikichangewatcher-0.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-07 02:52 wikichangewatcher-0.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      619 b- defN 23-Aug-07 02:52 wikichangewatcher-0.2.1.dist-info/RECORD
+7 files, 45577 bytes uncompressed, 11916 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: wikichangewatcher/__init__.py
 Comment: 
 
 Filename: wikichangewatcher/wikichangewatcher.py
 Comment: 
 
-Filename: wikichangewatcher-0.2.0.dist-info/LICENSE
+Filename: wikichangewatcher-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: wikichangewatcher-0.2.0.dist-info/METADATA
+Filename: wikichangewatcher-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: wikichangewatcher-0.2.0.dist-info/WHEEL
+Filename: wikichangewatcher-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: wikichangewatcher-0.2.0.dist-info/top_level.txt
+Filename: wikichangewatcher-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: wikichangewatcher-0.2.0.dist-info/RECORD
+Filename: wikichangewatcher-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wikichangewatcher/__init__.py

```diff
@@ -1,7 +1,17 @@
-__version__ = "0.2.0"
+__author__ = "Erik Nyquist"
+__license__ = "Apache 2.0"
+__maintainer__ = "Erik Nyquist"
+__version__ = "0.2.1"
+__email__ = "eknyquist@gmail.com"
 
 from wikichangewatcher.wikichangewatcher import FieldFilter, FilterCollection, IpV4Filter, IpV6Filter, WikiChangeWatcher, MatchType
 from wikichangewatcher.wikichangewatcher import FieldStringFilter, FieldRegexMatchFilter, FieldRegexSearchFilter
 from wikichangewatcher.wikichangewatcher import UsernameFilter, UsernameRegexMatchFilter, UsernameRegexSearchFilter
 from wikichangewatcher.wikichangewatcher import PageUrlFilter, PageUrlRegexMatchFilter, PageUrlRegexSearchFilter
 
+import logging
+logging.basicConfig(format="[%(asctime)s][%(levelname)s][%(module)s:%(lineno)s]: %(message)s")
+
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.WARNING)
+logger.info(f"wikichangewatcher {__version__}")
```

## wikichangewatcher/wikichangewatcher.py

```diff
@@ -1,17 +1,20 @@
 import re
 import threading
 import requests
 import json
 import ctypes
+import logging
 from typing import Callable, Type, Self
 
 from sseclient import SSEClient
 
 
+logger = logging.getLogger(__name__)
+
 WIKIMEDIA_URL = 'https://stream.wikimedia.org/v2/stream/recentchange'
 
 
 class FieldFilter(object):
     """
     Generic/abstract class for checking whether a specific field of the "recent changes"
     JSON event data matches some expected format/values.
@@ -19,24 +22,42 @@
     The json_data provided to the on_match callback is an JSON-encoded event from the WikiMedia
     "recent changes" event stream, as described here: https://www.mediawiki.org/wiki/Manual:RCFeed
     """
     def __init__(self):
         self._on_match = None
 
     def on_match(self, on_match_handler: Callable[[dict], None]) -> Self:
+        """
+        Set a function to be called when an edit event matching this filter is seen
+
+        :param on_match_handler: callback function
+        """
         self._on_match = on_match_handler
         return self
 
     def _handler(self, json_data: dict) -> bool:
         raise NotImplementedError
 
     def check_match(self, json_data: dict) -> bool:
+        """
+        Check if an edit event matches this filter
+
+        :param json_data: Edit event to check
+
+        :return: True if match
+        :rtype: bool
+        """
         return self._handler(json_data)
 
     def run_on_match(self, json_data: dict):
+        """
+        Check if edit event matches this filter, and run on_match handler if it does match.
+
+        :param json_data: Edit event to check
+        """
         if self._on_match is not None:
             self._on_match(json_data)
 
 
 class MatchType(object):
     """
     Enumerates all match types handled by a FilterCollection
@@ -47,23 +68,28 @@
 
 class FilterCollection(FieldFilter):
     """
     A Filter object that holds multiple filters, and can run a callback if all or any one
     of the filters matches
     """
     def __init__(self, *filters):
+        """
+        :param filters: one or more filter instances to use
+        """
         super(FilterCollection, self).__init__()
         self._filters = filters
         self._match_type = MatchType.ALL
 
     def set_match_type(self, match_type: int) -> Self:
         """
         Set match type for this collection. If MatchType.ALL, then this collection will
         match only if all contained filters match. If MatchType.ANY, then this collection will
         match if one of the contained filters match.
+
+        :match_type: Match type, must be one of the values defined in wikichangewatcher.MatchType
         """
         self._match_type = match_type
         return self
 
     def _handler(self, json_data: dict) -> bool:
         match = False
 
@@ -81,18 +107,45 @@
         raise ValueError
 
     return intval
 
 
 class IpV4Filter(FieldFilter):
     """
-    FieldWatcher implementation to watch for "user" fields that contain IPv4 addresses
+    FieldFilter implementation to watch for "user" fields that contain IPv4 addresses
     in the specified ranges
     """
     def __init__(self, ip_addr_pattern="*.*.*.*"):
+        """
+        IPv4 address pattern to use. Each of the 4 dot-seperated fields may be one of
+        the following:
+
+        - A decimal integer from 0 through 255, representing exactly and only the written value.
+        - A range of values in the form "0-255" (two decimal integers, both between 0 and 255, separated
+          by a dash), representing any value between and including the two written values.
+        - An asterisk '\*', representing any value from 0 through 255.
+
+        These can be used in combination. For example:
+
+        - "\*.\*.\*.\*" matches any valid IPv4 address
+
+        - "192.88.99.77" matches only one specific IPv4 address, 192.88.99.77
+
+        - "192.88.0-9.\*" matches 2,550 specific IPv4 addresses:
+
+           192.88.0.0
+
+           192.88.0.1
+
+           192.88.0.2
+
+           ...
+
+           And so on, all the way up to 192.88.9.255
+        """
         super(IpV4Filter, self).__init__()
         self.ip_addr_pattern = []
 
         for x in ip_addr_pattern.split("."):
             error = False
 
             if x == "*":
@@ -153,18 +206,45 @@
         raise ValueError
 
     return intval
 
 
 class IpV6Filter(FieldFilter):
     """
-    FieldWatcher implementation to watch for "user" fields that contain IPv6 addresses
+    FieldFilter implementation to watch for "user" fields that contain IPv6 addresses
     in the specified ranges
     """
     def __init__(self, ip_addr_pattern="*:*:*:*:*:*:*:*"):
+        """
+        IPv6 address pattern to use. Each of the 8 dot-seperated fields may be one of
+        the following:
+
+        - A hexadecimal integer from 0 through ffff, representing exactly and only the written value.
+        - A range of values in the form "0-255" (two hexadecimal integers, both between 0 and ffff, separated
+          by a dash), representing any value between and including the two written values.
+        - An asterisk '\*', representing any value from 0 through ffff.
+
+        These can be used in combination. For example:
+
+        - "\*:\*:\*:\*:\*:\*:\*:\*" matches any valid IPv6 address
+
+        - "00.11.22.33.44.55.66.77" matches only one specific IPv6 address, 00.11.22.33.44.55.66.77
+
+        - "00.11.22.33.44.55.0-9.\*" matches 655,350 specific IPv6 addresses:
+
+           00.11.22.33.44.55.0.0
+
+           00.11.22.33.44.55.0.1
+
+           00.11.22.33.44.55.0.2
+
+           ...
+
+           And so on, all the way up to 00.11.22.33.44.55.9.ffff
+        """
         super(IpV6Filter, self).__init__()
         self.ip_addr_pattern = []
 
         for x in ip_addr_pattern.split(":"):
             error = False
 
             if x == "*":
@@ -323,50 +403,76 @@
     Consumes all events from the Wikimedia "recent changes" stream, and
     applies all provided FieldFilter instances to each received event.
     """
     def __init__(self, *filters):
         self._thread = None
         self._stop_event = threading.Event()
         self._filters = filters
+        self._session = None
+        self._client = None
+        self._on_edit_handler = None
+        self._retry_count = 0
+        self._max_retries = 10
+        self._connect()
+
+    def _connect(self):
         self._session = requests.Session()
         self._client = SSEClient(WIKIMEDIA_URL, session=self._session)
-        self._on_edit_handler = None
+        logger.debug(f"connected to {WIKIMEDIA_URL}")
 
     def on_edit(self, on_edit_handler: Callable[[dict], None]) -> Self:
         """
         Sets handler to run whenever any edit event is received (before any filters are processed)
+
+        :param on_edit_handler: Handler to run on edit event
         """
         self._on_edit_handler = on_edit_handler
         return self
 
     def add_filter(self, fltr: Type[FieldFilter]) -> Self:
         """
         Add a new filter to the list of active filters
+
+        :param fltr: filter instance to add
         """
         self._filters.append(fltr)
         return self
 
     def run(self):
         """
-        Start WikiWatcher running in a separate thread
+        Start WikiChangeWatcher running in a separate thread
         """
         if self._thread is not None:
             raise RuntimeError("'run()' has already been called!")
 
         self._thread = threading.Thread(target=self._thread_task)
         self._thread.daemon = True
         self._thread.start()
 
+    def is_running(self):
+        """
+        Returns true if WikiChangeWatcher thread is active
+
+        :return: True if thread is active
+        :rtype: bool
+        """
+        if self._thread is None:
+            return False
+
+        return self._thread.is_alive()
+
     def stop(self):
         """
         Send stop event to the running WikiWatcher thread and wait for it to terminate
         """
         if self._thread is None:
             return
 
+        logger.debug("stopping")
+
         # Use CPython API to inject a SystemExit exception into the WikiWatcher thread.
         # Unfortunately, sseclient lib does not provide any way to terminate waiting for
         # the next event, so this is the only way to stop the thread without having
         # to wait for the next event.
         exception = SystemExit
         target_tid = self._thread.ident
 
@@ -377,18 +483,30 @@
             ctypes.pythonapi.PyThreadState_SetAsyncExc(target_tid, NULL)
             raise SystemError("PyThreadState_SetAsyncExc failed")
 
         self._thread.join()
         self._thread = None
 
     def _thread_task(self):
+        while True:
+            try:
+                self._event_loop()
+            except requests.exceptions.ConnectionError:
+                if self._retry_count >= self._max_retries:
+                    raise RuntimeError(f"failed to re-connect after {self._max_retries} attempts")
+                else:
+                    self._retry_count += 1
+                    logger.warning(f"stream connection failed, retrying {self._retry_count}/{self._max_retries}")
+
+    def _event_loop(self):
         for event in self._client:
             if self._stop_event.is_set():
                 return
 
+            self._retry_count = 0
             if event.event == "message":
                 try:
                     change = json.loads(event.data)
                 except ValueError:
                     continue
 
                 if self._on_edit_handler:
```

## Comparing `wikichangewatcher-0.2.0.dist-info/LICENSE` & `wikichangewatcher-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wikichangewatcher-0.2.0.dist-info/METADATA` & `wikichangewatcher-0.2.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
 Name: wikichangewatcher
-Version: 0.2.0
+Version: 0.2.1
 Summary: Real-time monitoring/filtering of global Wikipedia page edits
 Home-page: http://github.com/eriknyquist/wikichangewatcher
 Author: Erik Nyquist
 Author-email: eknyquist@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: sseclient
 
-WikiChangeWatcher 0.2.0
+WikiChangeWatcher 0.2.1
 =======================
 
-.. image:: images/wikiwatcher_github_banner.png
+.. image:: https://raw.githubusercontent.com/eriknyquist/wikichangewatcher/5f8e204db0af39d0a0ed00e5884a38544e11321a/images/wikiwatcher_github_banner.png
 
 .. contents:: Table of Contents
 
 Introduction
 ============
 
 Wikipedia provides an `SSE Stream <https://en.wikipedia.org/wiki/Server-sent_events>`_  of
```

