# Comparing `tmp/era_5g_client-0.4.1.tar.gz` & `tmp/era_5g_client-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "era_5g_client-0.4.1.tar", last modified: Wed Jul 19 09:49:01 2023, max compression
+gzip compressed data, was "era_5g_client-0.4.2.tar", last modified: Mon Aug  7 12:09:12 2023, max compression
```

## Comparing `era_5g_client-0.4.1.tar` & `era_5g_client-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:49:01.439323 era_5g_client-0.4.1/
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       12 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/MANIFEST.in
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      414 2023-07-19 09:49:01.439323 era_5g_client-0.4.1/PKG-INFO
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      749 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/backend_shim.py
-drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:49:01.439323 era_5g_client-0.4.1/era_5g_client/
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client/__init__.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)    11708 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client/client.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     8643 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client/client_base.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      523 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client/dataclasses.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      662 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client/exceptions.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     2715 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client/middleware_resource_checker.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client/py.typed
-drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:49:01.439323 era_5g_client-0.4.1/era_5g_client.egg-info/
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      414 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client.egg-info/PKG-INFO
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      470 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client.egg-info/SOURCES.txt
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        1 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client.egg-info/dependency_links.txt
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        1 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client.egg-info/namespace_packages.txt
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      127 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client.egg-info/requires.txt
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       14 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client.egg-info/top_level.txt
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       38 2023-07-19 09:49:01.439323 era_5g_client-0.4.1/setup.cfg
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1009 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/setup.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-08-07 12:09:12.985364 era_5g_client-0.4.2/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-08-07 12:09:11.000000 era_5g_client-0.4.2/MANIFEST.in
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      414 2023-08-07 12:09:12.985364 era_5g_client-0.4.2/PKG-INFO
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      749 2023-08-07 12:09:11.000000 era_5g_client-0.4.2/backend_shim.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-08-07 12:09:12.981364 era_5g_client-0.4.2/era_5g_client/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-08-07 12:09:11.000000 era_5g_client-0.4.2/era_5g_client/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)    11708 2023-08-07 12:09:11.000000 era_5g_client-0.4.2/era_5g_client/client.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     8643 2023-08-07 12:09:11.000000 era_5g_client-0.4.2/era_5g_client/client_base.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      523 2023-08-07 12:09:11.000000 era_5g_client-0.4.2/era_5g_client/dataclasses.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      662 2023-08-07 12:09:11.000000 era_5g_client-0.4.2/era_5g_client/exceptions.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2715 2023-08-07 12:09:11.000000 era_5g_client-0.4.2/era_5g_client/middleware_resource_checker.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-08-07 12:09:11.000000 era_5g_client-0.4.2/era_5g_client/py.typed
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-08-07 12:09:12.981364 era_5g_client-0.4.2/era_5g_client.egg-info/
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      414 2023-08-07 12:09:12.000000 era_5g_client-0.4.2/era_5g_client.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      470 2023-08-07 12:09:12.000000 era_5g_client-0.4.2/era_5g_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-08-07 12:09:12.000000 era_5g_client-0.4.2/era_5g_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-08-07 12:09:12.000000 era_5g_client-0.4.2/era_5g_client.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      135 2023-08-07 12:09:12.000000 era_5g_client-0.4.2/era_5g_client.egg-info/requires.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       14 2023-08-07 12:09:12.000000 era_5g_client-0.4.2/era_5g_client.egg-info/top_level.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-08-07 12:09:12.985364 era_5g_client-0.4.2/setup.cfg
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1017 2023-08-07 12:09:11.000000 era_5g_client-0.4.2/setup.py
```

### Comparing `era_5g_client-0.4.1/backend_shim.py` & `era_5g_client-0.4.2/backend_shim.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.4.1/era_5g_client/client.py` & `era_5g_client-0.4.2/era_5g_client/client.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.4.1/era_5g_client/client_base.py` & `era_5g_client-0.4.2/era_5g_client/client_base.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.4.1/era_5g_client/dataclasses.py` & `era_5g_client-0.4.2/era_5g_client/dataclasses.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.4.1/era_5g_client/exceptions.py` & `era_5g_client-0.4.2/era_5g_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.4.1/era_5g_client/middleware_resource_checker.py` & `era_5g_client-0.4.2/era_5g_client/middleware_resource_checker.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.4.1/setup.py` & `era_5g_client-0.4.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         'Intended Audience :: Developers',
     ],
     'description': 'A client for 5G-ERA NetApps',
     'install_requires': (
         'era-5g-interface~=0.4.1',
         'numpy>=1.24.2',
         'opencv-python>=4.6.0.66',
-        'python-socketio>=5.8.0',
+        'python-socketio[client]>=5.8.0',
         'requests>=2.28.2',
         'types-requests==2.31.0.1',
     ),
     'license': 'LGPL',
     'name': 'era_5g_client',
     'namespace_packages': (
     ),
@@ -31,9 +31,9 @@
             'py.typed',
         ),
     },
     'packages': (
         'era_5g_client',
     ),
     'python_requires': '>=3.8',
-    'version': '0.4.1',
+    'version': '0.4.2',
 })
```

