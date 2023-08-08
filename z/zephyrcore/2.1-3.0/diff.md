# Comparing `tmp/zephyrcore-2.1.tar.gz` & `tmp/zephyrcore-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zephyrcore-2.1.tar", last modified: Tue Aug  8 18:21:14 2023, max compression
+gzip compressed data, was "zephyrcore-3.0.tar", last modified: Tue Aug  8 18:29:58 2023, max compression
```

## Comparing `zephyrcore-2.1.tar` & `zephyrcore-3.0.tar`

### file list

```diff
@@ -1,20 +1,13 @@
-drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:21:14.800401 zephyrcore-2.1/
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     1241 2023-08-08 18:21:14.800401 zephyrcore-2.1/PKG-INFO
--rw-rw-r--   0 rayan     (1000) rayan     (1000)      985 2023-07-17 12:37:36.000000 zephyrcore-2.1/README.md
-drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:21:14.800401 zephyrcore-2.1/core/
--rw-rw-r--   0 rayan     (1000) rayan     (1000)        0 2023-08-08 12:50:44.000000 zephyrcore-2.1/core/__init__.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     1910 2023-07-31 17:35:09.000000 zephyrcore-2.1/core/actions.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     5820 2023-08-08 12:42:10.000000 zephyrcore-2.1/core/constants.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)    20585 2023-08-08 12:52:21.000000 zephyrcore-2.1/core/create_test_cycles.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     6549 2023-08-08 12:42:10.000000 zephyrcore-2.1/core/json_treatment.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     1497 2023-08-08 12:52:21.000000 zephyrcore-2.1/core/logger.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     2047 2023-08-03 15:43:40.000000 zephyrcore-2.1/core/update_test_case.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     3225 2023-08-08 12:42:10.000000 zephyrcore-2.1/core/utils.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)       38 2023-08-08 18:21:14.800401 zephyrcore-2.1/setup.cfg
--rw-rw-r--   0 rayan     (1000) rayan     (1000)      708 2023-08-08 18:21:12.000000 zephyrcore-2.1/setup.py
-drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:21:14.800401 zephyrcore-2.1/zephyrcore.egg-info/
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     1241 2023-08-08 18:21:14.000000 zephyrcore-2.1/zephyrcore.egg-info/PKG-INFO
--rw-rw-r--   0 rayan     (1000) rayan     (1000)      342 2023-08-08 18:21:14.000000 zephyrcore-2.1/zephyrcore.egg-info/SOURCES.txt
--rw-rw-r--   0 rayan     (1000) rayan     (1000)        1 2023-08-08 18:21:14.000000 zephyrcore-2.1/zephyrcore.egg-info/dependency_links.txt
--rw-rw-r--   0 rayan     (1000) rayan     (1000)       30 2023-08-08 18:21:14.000000 zephyrcore-2.1/zephyrcore.egg-info/requires.txt
--rw-rw-r--   0 rayan     (1000) rayan     (1000)       16 2023-08-08 18:21:14.000000 zephyrcore-2.1/zephyrcore.egg-info/top_level.txt
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:29:58.284998 zephyrcore-3.0/
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     1241 2023-08-08 18:29:58.284998 zephyrcore-3.0/PKG-INFO
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)      985 2023-07-17 12:37:36.000000 zephyrcore-3.0/README.md
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:29:58.280998 zephyrcore-3.0/core/
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)        0 2023-08-08 12:50:44.000000 zephyrcore-3.0/core/__init__.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)       38 2023-08-08 18:29:58.284998 zephyrcore-3.0/setup.cfg
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)      702 2023-08-08 18:29:56.000000 zephyrcore-3.0/setup.py
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:29:58.280998 zephyrcore-3.0/zephyrcore.egg-info/
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     1241 2023-08-08 18:29:58.000000 zephyrcore-3.0/zephyrcore.egg-info/PKG-INFO
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)      204 2023-08-08 18:29:58.000000 zephyrcore-3.0/zephyrcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)        1 2023-08-08 18:29:58.000000 zephyrcore-3.0/zephyrcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)       30 2023-08-08 18:29:58.000000 zephyrcore-3.0/zephyrcore.egg-info/requires.txt
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)        5 2023-08-08 18:29:58.000000 zephyrcore-3.0/zephyrcore.egg-info/top_level.txt
```

### Comparing `zephyrcore-2.1/PKG-INFO` & `zephyrcore-3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zephyrcore
-Version: 2.1
+Version: 3.0
 Summary: Python Distribution Utilities
 Home-page: https://www.python.org/sigs/distutils-sig/
 Author: QM Core Team
 Author-email: business.agility@ab-inbev.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `zephyrcore-2.1/README.md` & `zephyrcore-3.0/README.md`

 * *Files identical despite different names*

### Comparing `zephyrcore-2.1/setup.py` & `zephyrcore-3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 import setuptools
 
 setuptools.setup(name='zephyrcore',
-                 version='2.1',
+                 version='3.0',
                  description='Python Distribution Utilities',
                  author='QM Core Team',
                  author_email='business.agility@ab-inbev.com',
                  long_description=open('README.md').read(),
                  long_description_content_type='text/markdown',
                  url='https://www.python.org/sigs/distutils-sig/',
                  packages=setuptools.find_packages(),
                  python_requires='>=3.9',
-                 py_modules=["zephyrcore"],
+                 py_modules=["core"],
                  install_requires=['requests', 'atlassian-python-api']  # Optional
                  )
```

### Comparing `zephyrcore-2.1/zephyrcore.egg-info/PKG-INFO` & `zephyrcore-3.0/zephyrcore.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zephyrcore
-Version: 2.1
+Version: 3.0
 Summary: Python Distribution Utilities
 Home-page: https://www.python.org/sigs/distutils-sig/
 Author: QM Core Team
 Author-email: business.agility@ab-inbev.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

