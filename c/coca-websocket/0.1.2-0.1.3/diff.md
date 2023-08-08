# Comparing `tmp/coca_websocket-0.1.2.tar.gz` & `tmp/coca_websocket-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coca_websocket-0.1.2.tar", max compression
+gzip compressed data, was "coca_websocket-0.1.3.tar", max compression
```

## Comparing `coca_websocket-0.1.2.tar` & `coca_websocket-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       72 2023-08-08 11:46:27.857419 coca_websocket-0.1.2/coca_websocket/__init__.py
--rw-r--r--   0        0        0      822 2023-08-07 19:05:51.658697 coca_websocket-0.1.2/coca_websocket/websocket.py
--rw-r--r--   0        0        0      344 2023-08-08 11:46:21.493183 coca_websocket-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      610 2023-08-08 11:46:41.385255 coca_websocket-0.1.2/setup.py
--rw-r--r--   0        0        0      352 2023-08-08 11:46:41.385482 coca_websocket-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-08-08 12:23:20.018232 coca_websocket-0.1.3/coca_websocket/__init__.py
+-rw-r--r--   0        0        0      822 2023-08-08 12:05:45.739310 coca_websocket-0.1.3/coca_websocket/websocket.py
+-rw-r--r--   0        0        0      421 2023-08-08 12:23:10.393798 coca_websocket-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      610 2023-08-08 12:23:57.961960 coca_websocket-0.1.3/setup.py
+-rw-r--r--   0        0        0      352 2023-08-08 12:23:57.962262 coca_websocket-0.1.3/PKG-INFO
```

### Comparing `coca_websocket-0.1.2/coca_websocket/websocket.py` & `coca_websocket-0.1.3/coca_websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `coca_websocket-0.1.2/setup.py` & `coca_websocket-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['websockets>=11.0.3,<12.0.0']
 
 setup_kwargs = {
     'name': 'coca-websocket',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '',
     'long_description': None,
     'author': 'Hiroyuki Ikuno',
     'author_email': 'sam2kaikaramegusuri@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

