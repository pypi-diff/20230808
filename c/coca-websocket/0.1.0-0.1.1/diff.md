# Comparing `tmp/coca_websocket-0.1.0.tar.gz` & `tmp/coca_websocket-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coca_websocket-0.1.0.tar", max compression
+gzip compressed data, was "coca_websocket-0.1.1.tar", max compression
```

## Comparing `coca_websocket-0.1.0.tar` & `coca_websocket-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       72 2023-08-07 19:56:44.699631 coca_websocket-0.1.0/coca_websocket/__init__.py
--rw-r--r--   0        0        0      822 2023-08-07 19:05:51.658697 coca_websocket-0.1.0/coca_websocket/websocket.py
--rw-r--r--   0        0        0      321 2023-08-08 10:27:46.002695 coca_websocket-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      521 2023-08-08 11:18:03.598911 coca_websocket-0.1.0/setup.py
--rw-r--r--   0        0        0      263 2023-08-08 11:18:03.599121 coca_websocket-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-08-08 11:37:06.480250 coca_websocket-0.1.1/coca_websocket/__init__.py
+-rw-r--r--   0        0        0      822 2023-08-07 19:05:51.658697 coca_websocket-0.1.1/coca_websocket/websocket.py
+-rw-r--r--   0        0        0      321 2023-08-08 11:36:55.411688 coca_websocket-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      515 2023-08-08 11:37:37.095645 coca_websocket-0.1.1/setup.py
+-rw-r--r--   0        0        0      307 2023-08-08 11:37:37.095850 coca_websocket-0.1.1/PKG-INFO
```

### Comparing `coca_websocket-0.1.0/coca_websocket/websocket.py` & `coca_websocket-0.1.1/coca_websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `coca_websocket-0.1.0/setup.py` & `coca_websocket-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 ['coca_websocket']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'coca-websocket',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': None,
     'author': 'Hiroyuki Ikuno',
     'author_email': 'sam2kaikaramegusuri@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.9',
 }
 
 
 setup(**setup_kwargs)
```

