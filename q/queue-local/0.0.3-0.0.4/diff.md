# Comparing `tmp/queue-local-0.0.3.tar.gz` & `tmp/queue-local-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue-local-0.0.3.tar", last modified: Mon Aug  7 16:16:21 2023, max compression
+gzip compressed data, was "queue-local-0.0.4.tar", last modified: Tue Aug  8 12:29:33 2023, max compression
```

## Comparing `queue-local-0.0.3.tar` & `queue-local-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:16:21.939103 queue-local-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-07 16:16:21.939103 queue-local-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-07 16:15:54.000000 queue-local-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-07 16:15:54.000000 queue-local-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:16:21.939103 queue-local-0.0.3/queue_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-07 16:16:21.000000 queue-local-0.0.3/queue_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 16:16:21.000000 queue-local-0.0.3/queue_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:16:21.000000 queue-local-0.0.3/queue_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:16:21.000000 queue-local-0.0.3/queue_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 16:16:21.939103 queue-local-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-07 16:15:54.000000 queue-local-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:29:33.192947 queue-local-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-08 12:29:33.192947 queue-local-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-08 12:29:06.000000 queue-local-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-08 12:29:06.000000 queue-local-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:29:33.192947 queue-local-0.0.4/queue_local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:29:06.000000 queue-local-0.0.4/queue_local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:29:33.192947 queue-local-0.0.4/queue_local/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:29:06.000000 queue-local-0.0.4/queue_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-08-08 12:29:06.000000 queue-local-0.0.4/queue_local/src/database_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-08 12:29:06.000000 queue-local-0.0.4/queue_local/src/our_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:29:33.192947 queue-local-0.0.4/queue_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-08 12:29:33.000000 queue-local-0.0.4/queue_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-08 12:29:33.000000 queue-local-0.0.4/queue_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:29:33.000000 queue-local-0.0.4/queue_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 12:29:33.000000 queue-local-0.0.4/queue_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:29:33.192947 queue-local-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-08 12:29:06.000000 queue-local-0.0.4/setup.py
```

### Comparing `queue-local-0.0.3/README.md` & `queue-local-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # queue-local-python-package
 
 ## Usage:
 
-Install: `pip install queue-local-python-package`  
-(Preferable you add queue-local to requirements.txt)
-If you want to test it, please run `pip install queue-local`
+Install: `pip install queue-local`  
+(Preferable you add queue-local to requirements.txt)  
 
 Use the `DatabaseQueue`:
 ```py
 from queue_local.src.database_queue import DatabaseQueue
 
 q = DatabaseQueue()
 q.push({"item": "test 1", "action_id": 1})
```

### Comparing `queue-local-0.0.3/setup.py` & `queue-local-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 setuptools.setup(
      name='queue-local',
-     version='0.0.3',  # https://pypi.org/project/queue-local-python-package/
+     version='0.0.4',  # https://pypi.org/project/queue-local-python-package/
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles queue Local Python",
      long_description="This is a package for sharing common Queue function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/circles",
      packages=setuptools.find_packages(),
```

