# Comparing `tmp/apache-airflow-providers-redis-3.3.1rc1.tar.gz` & `tmp/apache-airflow-providers-redis-3.3.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-redis-3.3.1rc1.tar", last modified: Fri Aug  4 21:41:34 2023, max compression
+gzip compressed data, was "apache-airflow-providers-redis-3.3.1rc2.tar", last modified: Tue Aug  8 07:21:56 2023, max compression
```

## Comparing `apache-airflow-providers-redis-3.3.1rc1.tar` & `apache-airflow-providers-redis-3.3.1rc2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.663300 apache-airflow-providers-redis-3.3.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-redis-3.3.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:41:33.000000 apache-airflow-providers-redis-3.3.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-redis-3.3.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4384 2023-08-04 21:41:34.663931 apache-airflow-providers-redis-3.3.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2750 2023-08-04 21:41:33.000000 apache-airflow-providers-redis-3.3.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.570393 apache-airflow-providers-redis-3.3.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.571553 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.607362 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/
--rw-r--r--   0 root         (0) root         (0)     1574 2023-08-04 21:33:34.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2707 2023-08-04 21:41:33.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.612912 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2945 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/hooks/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.618810 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/log/
--rw-r--r--   0 root         (0) root         (0)      787 2023-07-26 06:59:50.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3641 2023-07-26 06:59:50.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/log/redis_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.625314 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/operators/redis_publish.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.635533 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1585 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/sensors/redis_key.py
--rw-r--r--   0 root         (0) root         (0)     2660 2023-08-04 10:24:22.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/sensors/redis_pub_sub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.660987 apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4384 2023-08-04 21:41:34.000000 apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      937 2023-08-04 21:41:34.000000 apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:34.000000 apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-08-04 21:41:34.000000 apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:34.000000 apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       40 2023-08-04 21:41:34.000000 apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:41:34.000000 apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-redis-3.3.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1932 2023-08-04 21:41:34.666038 apache-airflow-providers-redis-3.3.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1632 2023-08-04 21:41:33.000000 apache-airflow-providers-redis-3.3.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 07:21:56.476785 apache-airflow-providers-redis-3.3.1rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-redis-3.3.1rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-08 07:21:55.000000 apache-airflow-providers-redis-3.3.1rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-redis-3.3.1rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4384 2023-08-08 07:21:56.477338 apache-airflow-providers-redis-3.3.1rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-08-08 07:21:55.000000 apache-airflow-providers-redis-3.3.1rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 07:21:56.383665 apache-airflow-providers-redis-3.3.1rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 07:21:56.384885 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 07:21:56.423644 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-08-08 06:28:58.000000 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2023-08-08 07:21:55.000000 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 07:21:56.429275 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2945 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/hooks/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 07:21:56.434984 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/log/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-07-26 06:59:50.000000 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2023-07-26 06:59:50.000000 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/log/redis_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 07:21:56.441034 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/operators/redis_publish.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 07:21:56.450180 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/sensors/redis_key.py
+-rw-r--r--   0 root         (0) root         (0)     2673 2023-08-08 06:24:51.000000 apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/sensors/redis_pub_sub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 07:21:56.474157 apache-airflow-providers-redis-3.3.1rc2/apache_airflow_providers_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4384 2023-08-08 07:21:56.000000 apache-airflow-providers-redis-3.3.1rc2/apache_airflow_providers_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      937 2023-08-08 07:21:56.000000 apache-airflow-providers-redis-3.3.1rc2/apache_airflow_providers_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 07:21:56.000000 apache-airflow-providers-redis-3.3.1rc2/apache_airflow_providers_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-08-08 07:21:56.000000 apache-airflow-providers-redis-3.3.1rc2/apache_airflow_providers_redis.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 07:21:56.000000 apache-airflow-providers-redis-3.3.1rc2/apache_airflow_providers_redis.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2023-08-08 07:21:56.000000 apache-airflow-providers-redis-3.3.1rc2/apache_airflow_providers_redis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-08 07:21:56.000000 apache-airflow-providers-redis-3.3.1rc2/apache_airflow_providers_redis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-redis-3.3.1rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1932 2023-08-08 07:21:56.479267 apache-airflow-providers-redis-3.3.1rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-08-08 07:21:55.000000 apache-airflow-providers-redis-3.3.1rc2/setup.py
```

### Comparing `apache-airflow-providers-redis-3.3.1rc1/LICENSE` & `apache-airflow-providers-redis-3.3.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.1rc1/MANIFEST.in` & `apache-airflow-providers-redis-3.3.1rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.1rc1/PKG-INFO` & `apache-airflow-providers-redis-3.3.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-redis
-Version: 3.3.1rc1
+Version: 3.3.1rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-redis package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.1/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-redis``
 
-Release: ``3.3.1rc1``
+Release: ``3.3.1rc2``
 
 
 `Redis <https://redis.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-redis-3.3.1rc1/README.rst` & `apache-airflow-providers-redis-3.3.1rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-redis``
 
-Release: ``3.3.1rc1``
+Release: ``3.3.1rc2``
 
 
 `Redis <https://redis.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/__init__.py` & `apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/get_provider_info.py` & `apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/hooks/__init__.py` & `apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/hooks/redis.py` & `apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/hooks/redis.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/log/__init__.py` & `apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/log/redis_task_handler.py` & `apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/log/redis_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/operators/__init__.py` & `apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/operators/redis_publish.py` & `apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/operators/redis_publish.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/sensors/__init__.py` & `apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/sensors/redis_key.py` & `apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/sensors/redis_key.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/sensors/redis_pub_sub.py` & `apache-airflow-providers-redis-3.3.1rc2/airflow/providers/redis/sensors/redis_pub_sub.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,27 +41,28 @@
     def __init__(self, *, channels: list[str] | str, redis_conn_id: str, **kwargs) -> None:
         super().__init__(**kwargs)
         self.channels = channels
         self.redis_conn_id = redis_conn_id
 
     @cached_property
     def pubsub(self):
-        return RedisHook(redis_conn_id=self.redis_conn_id).get_conn().pubsub()
+        hook = RedisHook(redis_conn_id=self.redis_conn_id).get_conn().pubsub()
+        hook.subscribe(self.channels)
+        return hook
 
     def poke(self, context: Context) -> bool:
         """
         Check for message on subscribed channels and write to xcom the message with key ``message``.
 
         An example of message ``{'type': 'message', 'pattern': None, 'channel': b'test', 'data': b'hello'}``
 
         :param context: the context object
         :return: ``True`` if message (with type 'message') is available or ``False`` if not
         """
         self.log.info("RedisPubSubSensor checking for message on channels: %s", self.channels)
-        self.pubsub.subscribe(self.channels)
         message = self.pubsub.get_message()
         self.log.info("Message %s from channel %s", message, self.channels)
 
         # Process only message types
         if message and message["type"] == "message":
 
             context["ti"].xcom_push(key="message", value=message)
```

### Comparing `apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/PKG-INFO` & `apache-airflow-providers-redis-3.3.1rc2/apache_airflow_providers_redis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-redis
-Version: 3.3.1rc1
+Version: 3.3.1rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-redis package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.1/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-redis``
 
-Release: ``3.3.1rc1``
+Release: ``3.3.1rc2``
 
 
 `Redis <https://redis.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/SOURCES.txt` & `apache-airflow-providers-redis-3.3.1rc2/apache_airflow_providers_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.1rc1/pyproject.toml` & `apache-airflow-providers-redis-3.3.1rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.1rc1/setup.cfg` & `apache-airflow-providers-redis-3.3.1rc2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.redis.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.redis
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-redis-3.3.1rc1/setup.py` & `apache-airflow-providers-redis-3.3.1rc2/setup.py`

 * *Files identical despite different names*

