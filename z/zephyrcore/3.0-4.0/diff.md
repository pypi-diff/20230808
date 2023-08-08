# Comparing `tmp/zephyrcore-3.0.tar.gz` & `tmp/zephyrcore-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zephyrcore-3.0.tar", last modified: Tue Aug  8 18:29:58 2023, max compression
+gzip compressed data, was "zephyrcore-4.0.tar", last modified: Tue Aug  8 18:41:07 2023, max compression
```

## Comparing `zephyrcore-3.0.tar` & `zephyrcore-4.0.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:29:58.284998 zephyrcore-3.0/
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     1241 2023-08-08 18:29:58.284998 zephyrcore-3.0/PKG-INFO
--rw-rw-r--   0 rayan     (1000) rayan     (1000)      985 2023-07-17 12:37:36.000000 zephyrcore-3.0/README.md
-drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:29:58.280998 zephyrcore-3.0/core/
--rw-rw-r--   0 rayan     (1000) rayan     (1000)        0 2023-08-08 12:50:44.000000 zephyrcore-3.0/core/__init__.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)       38 2023-08-08 18:29:58.284998 zephyrcore-3.0/setup.cfg
--rw-rw-r--   0 rayan     (1000) rayan     (1000)      702 2023-08-08 18:29:56.000000 zephyrcore-3.0/setup.py
-drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:29:58.280998 zephyrcore-3.0/zephyrcore.egg-info/
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     1241 2023-08-08 18:29:58.000000 zephyrcore-3.0/zephyrcore.egg-info/PKG-INFO
--rw-rw-r--   0 rayan     (1000) rayan     (1000)      204 2023-08-08 18:29:58.000000 zephyrcore-3.0/zephyrcore.egg-info/SOURCES.txt
--rw-rw-r--   0 rayan     (1000) rayan     (1000)        1 2023-08-08 18:29:58.000000 zephyrcore-3.0/zephyrcore.egg-info/dependency_links.txt
--rw-rw-r--   0 rayan     (1000) rayan     (1000)       30 2023-08-08 18:29:58.000000 zephyrcore-3.0/zephyrcore.egg-info/requires.txt
--rw-rw-r--   0 rayan     (1000) rayan     (1000)        5 2023-08-08 18:29:58.000000 zephyrcore-3.0/zephyrcore.egg-info/top_level.txt
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:41:07.900601 zephyrcore-4.0/
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     1241 2023-08-08 18:41:07.900601 zephyrcore-4.0/PKG-INFO
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)      985 2023-07-17 12:37:36.000000 zephyrcore-4.0/README.md
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)       38 2023-08-08 18:41:07.900601 zephyrcore-4.0/setup.cfg
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)      761 2023-08-08 18:40:41.000000 zephyrcore-4.0/setup.py
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:41:07.900601 zephyrcore-4.0/zephyrcore/
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:41:07.900601 zephyrcore-4.0/zephyrcore/src/
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:41:07.900601 zephyrcore-4.0/zephyrcore/src/zephyrcore/
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     1910 2023-07-31 17:35:09.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore/actions.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     5820 2023-08-08 12:42:10.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore/constants.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)    20585 2023-08-08 12:52:21.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore/create_test_cycles.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     6549 2023-08-08 12:42:10.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore/json_treatment.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     1496 2023-08-08 18:38:16.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore/logger.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     2047 2023-08-03 15:43:40.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore/update_test_case.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     3225 2023-08-08 12:42:10.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore/utils.py
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:41:07.900601 zephyrcore-4.0/zephyrcore/src/zephyrcore.egg-info/
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     1241 2023-08-08 18:41:07.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore.egg-info/PKG-INFO
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)      547 2023-08-08 18:41:07.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)        1 2023-08-08 18:41:07.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)       30 2023-08-08 18:41:07.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore.egg-info/requires.txt
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)       11 2023-08-08 18:41:07.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore.egg-info/top_level.txt
```

### Comparing `zephyrcore-3.0/PKG-INFO` & `zephyrcore-4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zephyrcore
-Version: 3.0
+Version: 4.0
 Summary: Python Distribution Utilities
 Home-page: https://www.python.org/sigs/distutils-sig/
 Author: QM Core Team
 Author-email: business.agility@ab-inbev.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `zephyrcore-3.0/README.md` & `zephyrcore-4.0/README.md`

 * *Files identical despite different names*

### Comparing `zephyrcore-3.0/setup.py` & `zephyrcore-4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python
 
 import setuptools
 
 setuptools.setup(name='zephyrcore',
-                 version='3.0',
+                 version='4.0',
                  description='Python Distribution Utilities',
                  author='QM Core Team',
                  author_email='business.agility@ab-inbev.com',
                  long_description=open('README.md').read(),
                  long_description_content_type='text/markdown',
                  url='https://www.python.org/sigs/distutils-sig/',
                  packages=setuptools.find_packages(),
                  python_requires='>=3.9',
-                 py_modules=["core"],
+                 py_modules=["zephyrcore"],
+                 package_dir={'': 'zephyrcore/src'},
                  install_requires=['requests', 'atlassian-python-api']  # Optional
                  )
```

### Comparing `zephyrcore-3.0/zephyrcore.egg-info/PKG-INFO` & `zephyrcore-4.0/zephyrcore/src/zephyrcore.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zephyrcore
-Version: 3.0
+Version: 4.0
 Summary: Python Distribution Utilities
 Home-page: https://www.python.org/sigs/distutils-sig/
 Author: QM Core Team
 Author-email: business.agility@ab-inbev.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

