# Comparing `tmp/mt5-server-0.0.3.tar.gz` & `tmp/mt5-server-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mt5-server-0.0.3.tar", last modified: Tue Aug  8 02:51:41 2023, max compression
+gzip compressed data, was "mt5-server-0.0.4.tar", last modified: Tue Aug  8 14:48:58 2023, max compression
```

## Comparing `mt5-server-0.0.3.tar` & `mt5-server-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:51:41.415988 mt5-server-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 02:51:32.000000 mt5-server-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-08 02:51:32.000000 mt5-server-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-08 02:51:41.415988 mt5-server-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-08 02:51:32.000000 mt5-server-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:51:41.415988 mt5-server-0.0.3/mt5_server/
--rw-r--r--   0 runner    (1001) docker     (123)   167923 2023-08-08 02:51:32.000000 mt5-server-0.0.3/mt5_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-08 02:51:32.000000 mt5-server-0.0.3/mt5_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-08-08 02:51:32.000000 mt5-server-0.0.3/mt5_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:51:41.415988 mt5-server-0.0.3/mt5_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-08 02:51:41.000000 mt5-server-0.0.3/mt5_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-08 02:51:41.000000 mt5-server-0.0.3/mt5_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 02:51:41.000000 mt5-server-0.0.3/mt5_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 02:51:41.000000 mt5-server-0.0.3/mt5_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-08 02:51:41.000000 mt5-server-0.0.3/mt5_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 02:51:41.415988 mt5-server-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-08-08 02:51:32.000000 mt5-server-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:51:41.415988 mt5-server-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-08 02:51:32.000000 mt5-server-0.0.3/tests/test_01.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:48:58.730055 mt5-server-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 14:48:48.000000 mt5-server-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-08 14:48:48.000000 mt5-server-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-08 14:48:58.730055 mt5-server-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-08 14:48:48.000000 mt5-server-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:48:58.730055 mt5-server-0.0.4/mt5_server/
+-rw-r--r--   0 runner    (1001) docker     (123)   167922 2023-08-08 14:48:48.000000 mt5-server-0.0.4/mt5_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-08 14:48:48.000000 mt5-server-0.0.4/mt5_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-08-08 14:48:48.000000 mt5-server-0.0.4/mt5_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:48:58.730055 mt5-server-0.0.4/mt5_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-08 14:48:58.000000 mt5-server-0.0.4/mt5_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-08 14:48:58.000000 mt5-server-0.0.4/mt5_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:48:58.000000 mt5-server-0.0.4/mt5_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 14:48:58.000000 mt5-server-0.0.4/mt5_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-08 14:48:58.000000 mt5-server-0.0.4/mt5_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 14:48:58.730055 mt5-server-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-08-08 14:48:48.000000 mt5-server-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:48:58.730055 mt5-server-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-08 14:48:48.000000 mt5-server-0.0.4/tests/test_01.py
```

### Comparing `mt5-server-0.0.3/LICENSE` & `mt5-server-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mt5-server-0.0.3/LICENSE.txt` & `mt5-server-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mt5-server-0.0.3/PKG-INFO` & `mt5-server-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mt5-server
-Version: 0.0.3
+Version: 0.0.4
 Summary: Servidor
 Home-page: https://github.com/michelmetran/mt5_server
 Author: Michel Metran
 Author-email: michelmetran@gmail.com
 Keywords: python,metatrader
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mt5-server-0.0.3/README.md` & `mt5-server-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mt5-server-0.0.3/mt5_server/__init__.py` & `mt5-server-0.0.4/mt5_server/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,16 +357,16 @@
     # The order is active until the specified date
     ORDER_TIME_SPECIFIED = 2
     # The order is active until 23:59:59 of the specified day. If this time appears to be out of a trading session, the expiration is processed at the nearest trading time.
     ORDER_TIME_SPECIFIED_DAY = 3
 
     def __init__(
         self,
-        # host='localhost',
-        host='192.168.31.251',
+        host='localhost',
+        #host='192.168.31.251',
         port=18812,
     ):
         '''
         host: str
             default = localhost
         port: int
             default = 18812
```

### Comparing `mt5-server-0.0.3/mt5_server/__main__.py` & `mt5-server-0.0.4/mt5_server/__main__.py`

 * *Files identical despite different names*

### Comparing `mt5-server-0.0.3/mt5_server/server.py` & `mt5-server-0.0.4/mt5_server/server.py`

 * *Files identical despite different names*

### Comparing `mt5-server-0.0.3/mt5_server.egg-info/PKG-INFO` & `mt5-server-0.0.4/mt5_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mt5-server
-Version: 0.0.3
+Version: 0.0.4
 Summary: Servidor
 Home-page: https://github.com/michelmetran/mt5_server
 Author: Michel Metran
 Author-email: michelmetran@gmail.com
 Keywords: python,metatrader
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mt5-server-0.0.3/setup.py` & `mt5-server-0.0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 requirements = []
 for line in open('requirements.txt', encoding='utf-8'):
     li = line.strip()
     if not li.startswith('#'):
         requirements.append(line.rstrip())
 
 
-VERSION = (0, 0, 3)
+VERSION = (0, 0, 4)
 __version__ = '.'.join(map(str, VERSION))
 
 
 setup(
     name='mt5-server',
     version=__version__,
     author='Michel Metran',
```

