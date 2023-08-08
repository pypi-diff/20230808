# Comparing `tmp/unused_attributes-0.1.8.tar.gz` & `tmp/unused_attributes-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unused_attributes-0.1.8.tar", last modified: Mon Aug  7 18:39:43 2023, max compression
+gzip compressed data, was "unused_attributes-0.1.9.tar", last modified: Tue Aug  8 19:14:01 2023, max compression
```

## Comparing `unused_attributes-0.1.8.tar` & `unused_attributes-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 xor       (1000) xor       (1000)        0 2023-08-07 18:39:43.723037 unused_attributes-0.1.8/
--rw-rw-r--   0 xor       (1000) xor       (1000)    35149 2023-08-06 12:07:32.000000 unused_attributes-0.1.8/LICENSE
--rw-rw-r--   0 xor       (1000) xor       (1000)      803 2023-08-07 18:39:43.719037 unused_attributes-0.1.8/PKG-INFO
--rw-rw-r--   0 xor       (1000) xor       (1000)       20 2023-08-06 22:14:00.000000 unused_attributes-0.1.8/README.md
--rw-rw-r--   0 xor       (1000) xor       (1000)     1051 2023-08-07 18:39:25.000000 unused_attributes-0.1.8/pyproject.toml
--rw-rw-r--   0 xor       (1000) xor       (1000)       38 2023-08-07 18:39:43.723037 unused_attributes-0.1.8/setup.cfg
-drwxrwxr-x   0 xor       (1000) xor       (1000)        0 2023-08-07 18:39:43.719037 unused_attributes-0.1.8/unused_attributes.egg-info/
--rw-rw-r--   0 xor       (1000) xor       (1000)      803 2023-08-07 18:39:43.000000 unused_attributes-0.1.8/unused_attributes.egg-info/PKG-INFO
--rw-rw-r--   0 xor       (1000) xor       (1000)      261 2023-08-07 18:39:43.000000 unused_attributes-0.1.8/unused_attributes.egg-info/SOURCES.txt
--rw-rw-r--   0 xor       (1000) xor       (1000)        1 2023-08-07 18:39:43.000000 unused_attributes-0.1.8/unused_attributes.egg-info/dependency_links.txt
--rw-rw-r--   0 xor       (1000) xor       (1000)       61 2023-08-07 18:39:43.000000 unused_attributes-0.1.8/unused_attributes.egg-info/entry_points.txt
--rw-rw-r--   0 xor       (1000) xor       (1000)       18 2023-08-07 18:39:43.000000 unused_attributes-0.1.8/unused_attributes.egg-info/top_level.txt
--rwxrwxr-x   0 xor       (1000) xor       (1000)     4489 2023-08-07 18:13:33.000000 unused_attributes-0.1.8/unused_attributes.py
+drwxrwxr-x   0 xor       (1000) xor       (1000)        0 2023-08-08 19:14:01.742454 unused_attributes-0.1.9/
+-rw-rw-r--   0 xor       (1000) xor       (1000)    35149 2023-08-06 12:07:32.000000 unused_attributes-0.1.9/LICENSE
+-rw-rw-r--   0 xor       (1000) xor       (1000)     1356 2023-08-08 19:14:01.742454 unused_attributes-0.1.9/PKG-INFO
+-rw-rw-r--   0 xor       (1000) xor       (1000)      463 2023-08-08 19:11:26.000000 unused_attributes-0.1.9/README.md
+-rw-rw-r--   0 xor       (1000) xor       (1000)     1150 2023-08-08 19:11:57.000000 unused_attributes-0.1.9/pyproject.toml
+-rw-rw-r--   0 xor       (1000) xor       (1000)       38 2023-08-08 19:14:01.742454 unused_attributes-0.1.9/setup.cfg
+drwxrwxr-x   0 xor       (1000) xor       (1000)        0 2023-08-08 19:14:01.742454 unused_attributes-0.1.9/unused_attributes.egg-info/
+-rw-rw-r--   0 xor       (1000) xor       (1000)     1356 2023-08-08 19:14:01.000000 unused_attributes-0.1.9/unused_attributes.egg-info/PKG-INFO
+-rw-rw-r--   0 xor       (1000) xor       (1000)      261 2023-08-08 19:14:01.000000 unused_attributes-0.1.9/unused_attributes.egg-info/SOURCES.txt
+-rw-rw-r--   0 xor       (1000) xor       (1000)        1 2023-08-08 19:14:01.000000 unused_attributes-0.1.9/unused_attributes.egg-info/dependency_links.txt
+-rw-rw-r--   0 xor       (1000) xor       (1000)       61 2023-08-08 19:14:01.000000 unused_attributes-0.1.9/unused_attributes.egg-info/entry_points.txt
+-rw-rw-r--   0 xor       (1000) xor       (1000)       18 2023-08-08 19:14:01.000000 unused_attributes-0.1.9/unused_attributes.egg-info/top_level.txt
+-rwxrwxr-x   0 xor       (1000) xor       (1000)     4489 2023-08-07 18:13:33.000000 unused_attributes-0.1.9/unused_attributes.py
```

### Comparing `unused_attributes-0.1.8/LICENSE` & `unused_attributes-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unused_attributes-0.1.8/pyproject.toml` & `unused_attributes-0.1.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unused_attributes"
-version = "0.1.8"
+version = "0.1.9"
 description = "Find class unused attributes"
 authors = [
     {name = "xor2003", email = "xor2003@gmx.com"},
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
@@ -19,14 +19,16 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Quality Assurance"
 ]
 
 [project.urls]
 Homepage = "https://github.com/xor2003/unused_attributes"
 [tool.distutils.egg_info]
 tag-build = ""
 tag-date = 0
```

### Comparing `unused_attributes-0.1.8/unused_attributes.py` & `unused_attributes-0.1.9/unused_attributes.py`

 * *Files identical despite different names*

