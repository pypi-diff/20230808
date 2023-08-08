# Comparing `tmp/geordpy-0.1.tar.gz` & `tmp/geordpy-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geordpy-0.1.tar", last modified: Tue Aug  8 12:41:17 2023, max compression
+gzip compressed data, was "geordpy-1.1.tar", last modified: Tue Aug  8 14:41:59 2023, max compression
```

## Comparing `geordpy-0.1.tar` & `geordpy-1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mein_ns   (1000) mein_ns   (1000)        0 2023-08-08 12:41:17.211201 geordpy-0.1/
--rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)     1068 2023-08-08 08:11:44.000000 geordpy-0.1/LICENSE
--rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)      523 2023-08-08 12:41:17.211201 geordpy-0.1/PKG-INFO
--rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)      265 2023-08-08 08:03:48.000000 geordpy-0.1/README.md
-drwxr-xr-x   0 mein_ns   (1000) mein_ns   (1000)        0 2023-08-08 12:41:17.211201 geordpy-0.1/geordpy/
--rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)      116 2023-08-08 09:59:49.000000 geordpy-0.1/geordpy/__init__.py
--rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)      495 2023-08-08 12:41:17.211201 geordpy-0.1/geordpy/_version.py
--rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)     1670 2023-08-08 12:37:50.000000 geordpy-0.1/geordpy/geordpy.py
-drwxr-xr-x   0 mein_ns   (1000) mein_ns   (1000)        0 2023-08-08 12:41:17.211201 geordpy-0.1/geordpy.egg-info/
--rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)      523 2023-08-08 12:41:17.000000 geordpy-0.1/geordpy.egg-info/PKG-INFO
--rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)      278 2023-08-08 12:41:17.000000 geordpy-0.1/geordpy.egg-info/SOURCES.txt
--rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)        1 2023-08-08 12:41:17.000000 geordpy-0.1/geordpy.egg-info/dependency_links.txt
--rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)       69 2023-08-08 12:41:17.000000 geordpy-0.1/geordpy.egg-info/requires.txt
--rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)        8 2023-08-08 12:41:17.000000 geordpy-0.1/geordpy.egg-info/top_level.txt
--rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)      304 2023-08-08 08:03:48.000000 geordpy-0.1/pyproject.toml
--rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)      676 2023-08-08 12:41:17.211201 geordpy-0.1/setup.cfg
--rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)     1006 2023-08-08 08:52:12.000000 geordpy-0.1/setup.py
--rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)    86677 2023-08-08 09:35:37.000000 geordpy-0.1/versioneer.py
+drwxr-xr-x   0 mein_ns   (1000) mein_ns   (1000)        0 2023-08-08 14:41:59.141138 geordpy-1.1/
+-rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)     1068 2023-08-08 08:11:44.000000 geordpy-1.1/LICENSE
+-rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)     3118 2023-08-08 14:41:59.141138 geordpy-1.1/PKG-INFO
+-rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)     2746 2023-08-08 14:32:07.000000 geordpy-1.1/README.md
+drwxr-xr-x   0 mein_ns   (1000) mein_ns   (1000)        0 2023-08-08 14:41:59.141138 geordpy-1.1/geordpy/
+-rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)      116 2023-08-08 09:59:49.000000 geordpy-1.1/geordpy/__init__.py
+-rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)      495 2023-08-08 14:41:59.141138 geordpy-1.1/geordpy/_version.py
+-rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)     3203 2023-08-08 13:41:52.000000 geordpy-1.1/geordpy/geordpy.py
+drwxr-xr-x   0 mein_ns   (1000) mein_ns   (1000)        0 2023-08-08 14:41:59.141138 geordpy-1.1/geordpy.egg-info/
+-rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)     3118 2023-08-08 14:41:59.000000 geordpy-1.1/geordpy.egg-info/PKG-INFO
+-rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)      278 2023-08-08 14:41:59.000000 geordpy-1.1/geordpy.egg-info/SOURCES.txt
+-rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)        1 2023-08-08 14:41:59.000000 geordpy-1.1/geordpy.egg-info/dependency_links.txt
+-rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)       69 2023-08-08 14:41:59.000000 geordpy-1.1/geordpy.egg-info/requires.txt
+-rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)        8 2023-08-08 14:41:59.000000 geordpy-1.1/geordpy.egg-info/top_level.txt
+-rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)      304 2023-08-08 08:03:48.000000 geordpy-1.1/pyproject.toml
+-rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)      676 2023-08-08 14:41:59.141138 geordpy-1.1/setup.cfg
+-rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)     1072 2023-08-08 14:40:31.000000 geordpy-1.1/setup.py
+-rw-r--r--   0 mein_ns   (1000) mein_ns   (1000)    86677 2023-08-08 09:35:37.000000 geordpy-1.1/versioneer.py
```

### Comparing `geordpy-0.1/LICENSE` & `geordpy-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geordpy-0.1/setup.cfg` & `geordpy-1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `geordpy-0.1/setup.py` & `geordpy-1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="geordpy",
-    description="",  # TODO: add a short description here
+    description="A Python library for simplifying geodetic-coordinate polylines using the Ramer-Douglas-Peucker algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/avitase/geordpy",
     author="Nis Meinert",
     author_email="mail@nismeinert.name",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
```

### Comparing `geordpy-0.1/versioneer.py` & `geordpy-1.1/versioneer.py`

 * *Files identical despite different names*

