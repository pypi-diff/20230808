# Comparing `tmp/SharQ-1.2.0.tar.gz` & `tmp/SharQ-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SharQ-1.2.0.tar", last modified: Tue Oct 26 07:11:53 2021, max compression
+gzip compressed data, was "SharQ-1.3.0.tar", last modified: Tue Aug  8 17:34:46 2023, max compression
```

## Comparing `SharQ-1.2.0.tar` & `SharQ-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 manish     (502) staff       (20)        0 2021-10-26 07:11:53.740995 SharQ-1.2.0/
--rw-r--r--   0 manish     (502) staff       (20)     1076 2021-06-08 15:55:01.000000 SharQ-1.2.0/LICENSE.txt
--rw-r--r--   0 manish     (502) staff       (20)       54 2021-06-08 15:55:01.000000 SharQ-1.2.0/MANIFEST.in
--rw-r--r--   0 manish     (502) staff       (20)     7397 2021-10-26 07:11:53.740849 SharQ-1.2.0/PKG-INFO
--rw-r--r--   0 manish     (502) staff       (20)     6750 2021-06-08 15:55:01.000000 SharQ-1.2.0/README.md
-drwxr-xr-x   0 manish     (502) staff       (20)        0 2021-10-26 07:11:53.738028 SharQ-1.2.0/SharQ.egg-info/
--rw-r--r--   0 manish     (502) staff       (20)     7397 2021-10-26 07:11:53.000000 SharQ-1.2.0/SharQ.egg-info/PKG-INFO
--rw-r--r--   0 manish     (502) staff       (20)      434 2021-10-26 07:11:53.000000 SharQ-1.2.0/SharQ.egg-info/SOURCES.txt
--rw-r--r--   0 manish     (502) staff       (20)        1 2021-10-26 07:11:53.000000 SharQ-1.2.0/SharQ.egg-info/dependency_links.txt
--rw-r--r--   0 manish     (502) staff       (20)       39 2021-10-26 07:11:53.000000 SharQ-1.2.0/SharQ.egg-info/requires.txt
--rw-r--r--   0 manish     (502) staff       (20)        6 2021-10-26 07:11:53.000000 SharQ-1.2.0/SharQ.egg-info/top_level.txt
--rw-r--r--   0 manish     (502) staff       (20)       38 2021-10-26 07:11:53.741042 SharQ-1.2.0/setup.cfg
--rw-r--r--   0 manish     (502) staff       (20)     1003 2021-10-26 07:11:02.000000 SharQ-1.2.0/setup.py
-drwxr-xr-x   0 manish     (502) staff       (20)        0 2021-10-26 07:11:53.739089 SharQ-1.2.0/sharq/
--rw-r--r--   0 manish     (502) staff       (20)      133 2021-06-08 15:55:01.000000 SharQ-1.2.0/sharq/__init__.py
--rw-r--r--   0 manish     (502) staff       (20)      185 2021-06-08 15:55:01.000000 SharQ-1.2.0/sharq/exceptions.py
--rw-r--r--   0 manish     (502) staff       (20)    19288 2021-09-21 10:02:20.000000 SharQ-1.2.0/sharq/queue.py
-drwxr-xr-x   0 manish     (502) staff       (20)        0 2021-10-26 07:11:53.736833 SharQ-1.2.0/sharq/scripts/
-drwxr-xr-x   0 manish     (502) staff       (20)        0 2021-10-26 07:11:53.740606 SharQ-1.2.0/sharq/scripts/lua/
--rw-r--r--   0 manish     (502) staff       (20)     4304 2021-06-08 15:55:01.000000 SharQ-1.2.0/sharq/scripts/lua/dequeue.lua
--rw-r--r--   0 manish     (502) staff       (20)     3282 2021-06-08 15:55:01.000000 SharQ-1.2.0/sharq/scripts/lua/enqueue.lua
--rw-r--r--   0 manish     (502) staff       (20)     1504 2021-06-08 15:55:01.000000 SharQ-1.2.0/sharq/scripts/lua/finish.lua
--rw-r--r--   0 manish     (502) staff       (20)      372 2021-06-08 15:55:01.000000 SharQ-1.2.0/sharq/scripts/lua/interval.lua
--rw-r--r--   0 manish     (502) staff       (20)      891 2021-06-08 15:55:01.000000 SharQ-1.2.0/sharq/scripts/lua/metrics.lua
--rw-r--r--   0 manish     (502) staff       (20)     3037 2021-06-08 15:55:01.000000 SharQ-1.2.0/sharq/scripts/lua/requeue.lua
--rw-r--r--   0 manish     (502) staff       (20)     2326 2021-10-26 07:02:56.000000 SharQ-1.2.0/sharq/utils.py
+drwxr-xr-x   0 manish     (502) staff       (20)        0 2023-08-08 17:34:46.239245 SharQ-1.3.0/
+-rw-r--r--   0 manish     (502) staff       (20)     1076 2021-06-08 15:55:01.000000 SharQ-1.3.0/LICENSE.txt
+-rw-r--r--   0 manish     (502) staff       (20)       54 2021-06-08 15:55:01.000000 SharQ-1.3.0/MANIFEST.in
+-rw-r--r--   0 manish     (502) staff       (20)     7377 2023-08-08 17:34:46.239045 SharQ-1.3.0/PKG-INFO
+-rw-r--r--   0 manish     (502) staff       (20)     6750 2021-06-08 15:55:01.000000 SharQ-1.3.0/README.md
+drwxr-xr-x   0 manish     (502) staff       (20)        0 2023-08-08 17:34:46.235250 SharQ-1.3.0/SharQ.egg-info/
+-rw-r--r--   0 manish     (502) staff       (20)     7377 2023-08-08 17:34:46.000000 SharQ-1.3.0/SharQ.egg-info/PKG-INFO
+-rw-r--r--   0 manish     (502) staff       (20)      473 2023-08-08 17:34:46.000000 SharQ-1.3.0/SharQ.egg-info/SOURCES.txt
+-rw-r--r--   0 manish     (502) staff       (20)        1 2023-08-08 17:34:46.000000 SharQ-1.3.0/SharQ.egg-info/dependency_links.txt
+-rw-r--r--   0 manish     (502) staff       (20)       39 2023-08-08 17:34:46.000000 SharQ-1.3.0/SharQ.egg-info/requires.txt
+-rw-r--r--   0 manish     (502) staff       (20)        6 2023-08-08 17:34:46.000000 SharQ-1.3.0/SharQ.egg-info/top_level.txt
+-rw-r--r--   0 manish     (502) staff       (20)       38 2023-08-08 17:34:46.239316 SharQ-1.3.0/setup.cfg
+-rw-r--r--   0 manish     (502) staff       (20)     1003 2023-08-08 10:26:57.000000 SharQ-1.3.0/setup.py
+drwxr-xr-x   0 manish     (502) staff       (20)        0 2023-08-08 17:34:46.236365 SharQ-1.3.0/sharq/
+-rw-r--r--   0 manish     (502) staff       (20)      133 2021-06-08 15:55:01.000000 SharQ-1.3.0/sharq/__init__.py
+-rw-r--r--   0 manish     (502) staff       (20)      185 2021-06-08 15:55:01.000000 SharQ-1.3.0/sharq/exceptions.py
+-rw-r--r--   0 manish     (502) staff       (20)    19947 2023-08-08 10:26:57.000000 SharQ-1.3.0/sharq/queue.py
+drwxr-xr-x   0 manish     (502) staff       (20)        0 2023-08-08 17:34:46.233538 SharQ-1.3.0/sharq/scripts/
+drwxr-xr-x   0 manish     (502) staff       (20)        0 2023-08-08 17:34:46.237762 SharQ-1.3.0/sharq/scripts/lua/
+-rw-r--r--   0 manish     (502) staff       (20)     4304 2021-06-08 15:55:01.000000 SharQ-1.3.0/sharq/scripts/lua/dequeue.lua
+-rw-r--r--   0 manish     (502) staff       (20)     3282 2021-06-08 15:55:01.000000 SharQ-1.3.0/sharq/scripts/lua/enqueue.lua
+-rw-r--r--   0 manish     (502) staff       (20)     1504 2021-06-08 15:55:01.000000 SharQ-1.3.0/sharq/scripts/lua/finish.lua
+-rw-r--r--   0 manish     (502) staff       (20)      372 2021-06-08 15:55:01.000000 SharQ-1.3.0/sharq/scripts/lua/interval.lua
+-rw-r--r--   0 manish     (502) staff       (20)      891 2021-06-08 15:55:01.000000 SharQ-1.3.0/sharq/scripts/lua/metrics.lua
+-rw-r--r--   0 manish     (502) staff       (20)     3037 2021-06-08 15:55:01.000000 SharQ-1.3.0/sharq/scripts/lua/requeue.lua
+-rw-r--r--   0 manish     (502) staff       (20)     2326 2021-10-26 07:02:56.000000 SharQ-1.3.0/sharq/utils.py
+drwxr-xr-x   0 manish     (502) staff       (20)        0 2023-08-08 17:34:46.238495 SharQ-1.3.0/tests/
+-rw-r--r--   0 manish     (502) staff       (20)    73852 2021-06-08 15:55:01.000000 SharQ-1.3.0/tests/test_func.py
+-rw-r--r--   0 manish     (502) staff       (20)    31253 2021-06-08 15:55:01.000000 SharQ-1.3.0/tests/test_queue.py
```

### Comparing `SharQ-1.2.0/LICENSE.txt` & `SharQ-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SharQ-1.2.0/PKG-INFO` & `SharQ-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: SharQ
-Version: 1.2.0
+Version: 1.3.0
 Summary: An API queueing system built at Plivo.
 Home-page: https://github.com/plivo/sharq
 Author: Plivo Team
 Author-email: voice-team@plivo.com
 License: The MIT License (MIT)
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >3.5
@@ -257,9 +256,7 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 ```
-
-
```

### Comparing `SharQ-1.2.0/README.md` & `SharQ-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `SharQ-1.2.0/SharQ.egg-info/PKG-INFO` & `SharQ-1.3.0/SharQ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: SharQ
-Version: 1.2.0
+Version: 1.3.0
 Summary: An API queueing system built at Plivo.
 Home-page: https://github.com/plivo/sharq
 Author: Plivo Team
 Author-email: voice-team@plivo.com
 License: The MIT License (MIT)
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >3.5
@@ -257,9 +256,7 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 ```
-
-
```

### Comparing `SharQ-1.2.0/setup.py` & `SharQ-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2014 Plivo Team. See LICENSE.txt for details.
 from setuptools import setup
 
 setup(
     name='SharQ',
-    version='1.2.0',
+    version='1.3.0',
     url='https://github.com/plivo/sharq',
     author='Plivo Team',
     author_email='voice-team@plivo.com',
     packages=['sharq'],
     package_data={
         'sharq': ['scripts/lua/*.lua']
     },
```

### Comparing `SharQ-1.2.0/sharq/queue.py` & `SharQ-1.3.0/sharq/queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -513,7 +513,25 @@
             pipe.execute()
             response.update({'status': 'Success',
                              'message': 'Successfully removed all queued calls and purged related resources'})
         else:
             # always delete the job queue list
             self._r.delete(job_queue_list)
         return response
+
+    def get_queue_length(self, queue_type, queue_id):
+        """
+        Return the current length present in redis key of type list
+        Redis key structure : key_prefix : queue_type : queue_id
+        """
+
+        # validate all the input
+        if not is_valid_identifier(queue_type):
+            raise BadArgumentException('`queue_type` has an invalid value.')
+
+        if not is_valid_identifier(queue_id):
+            raise BadArgumentException('`queue_id` has an invalid value.')
+
+        redis_key = self._key_prefix + ':' + queue_type + ':' + queue_id
+        current_queue_length = self._r.llen(redis_key)
+        return current_queue_length
+
```

### Comparing `SharQ-1.2.0/sharq/scripts/lua/dequeue.lua` & `SharQ-1.3.0/sharq/scripts/lua/dequeue.lua`

 * *Files identical despite different names*

### Comparing `SharQ-1.2.0/sharq/scripts/lua/enqueue.lua` & `SharQ-1.3.0/sharq/scripts/lua/enqueue.lua`

 * *Files identical despite different names*

### Comparing `SharQ-1.2.0/sharq/scripts/lua/finish.lua` & `SharQ-1.3.0/sharq/scripts/lua/finish.lua`

 * *Files identical despite different names*

### Comparing `SharQ-1.2.0/sharq/scripts/lua/metrics.lua` & `SharQ-1.3.0/sharq/scripts/lua/metrics.lua`

 * *Files identical despite different names*

### Comparing `SharQ-1.2.0/sharq/scripts/lua/requeue.lua` & `SharQ-1.3.0/sharq/scripts/lua/requeue.lua`

 * *Files identical despite different names*

### Comparing `SharQ-1.2.0/sharq/utils.py` & `SharQ-1.3.0/sharq/utils.py`

 * *Files identical despite different names*

