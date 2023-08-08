# Comparing `tmp/waypaper-1.0.3.tar.gz` & `tmp/waypaper-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waypaper-1.0.3.tar", last modified: Tue Aug  8 03:48:43 2023, max compression
+gzip compressed data, was "waypaper-1.0.4.tar", last modified: Tue Aug  8 03:52:19 2023, max compression
```

## Comparing `waypaper-1.0.3.tar` & `waypaper-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-08-08 03:48:43.893036 waypaper-1.0.3/
--rw-r--r--   0 r         (1000) r         (1000)    35149 2023-08-08 02:44:17.000000 waypaper-1.0.3/LICENSE
--rw-r--r--   0 r         (1000) r         (1000)     1778 2023-08-08 03:48:43.893036 waypaper-1.0.3/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)      996 2023-08-08 03:43:56.000000 waypaper-1.0.3/README.md
--rw-r--r--   0 r         (1000) r         (1000)       91 2022-11-27 00:35:48.000000 waypaper-1.0.3/pyproject.toml
--rw-r--r--   0 r         (1000) r         (1000)       38 2023-08-08 03:48:43.893036 waypaper-1.0.3/setup.cfg
--rw-r--r--   0 r         (1000) r         (1000)     1406 2023-08-08 03:48:27.000000 waypaper-1.0.3/setup.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-08-08 03:48:43.893036 waypaper-1.0.3/waypaper/
--rw-r--r--   0 r         (1000) r         (1000)      472 2023-08-08 03:48:33.000000 waypaper-1.0.3/waypaper/__main__.py
--rw-r--r--   0 r         (1000) r         (1000)     8455 2023-08-08 03:11:39.000000 waypaper-1.0.3/waypaper/app.py
--rw-r--r--   0 r         (1000) r         (1000)      409 2023-08-08 03:10:14.000000 waypaper-1.0.3/waypaper/changer.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-08-08 03:48:43.893036 waypaper-1.0.3/waypaper.egg-info/
--rw-r--r--   0 r         (1000) r         (1000)     1778 2023-08-08 03:48:43.000000 waypaper-1.0.3/waypaper.egg-info/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)      292 2023-08-08 03:48:43.000000 waypaper-1.0.3/waypaper.egg-info/SOURCES.txt
--rw-r--r--   0 r         (1000) r         (1000)        1 2023-08-08 03:48:43.000000 waypaper-1.0.3/waypaper.egg-info/dependency_links.txt
--rw-r--r--   0 r         (1000) r         (1000)       51 2023-08-08 03:48:43.000000 waypaper-1.0.3/waypaper.egg-info/entry_points.txt
--rw-r--r--   0 r         (1000) r         (1000)       10 2023-08-08 03:48:43.000000 waypaper-1.0.3/waypaper.egg-info/requires.txt
--rw-r--r--   0 r         (1000) r         (1000)        9 2023-08-08 03:48:43.000000 waypaper-1.0.3/waypaper.egg-info/top_level.txt
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-08-08 03:52:19.448256 waypaper-1.0.4/
+-rw-r--r--   0 r         (1000) r         (1000)    35149 2023-08-08 02:44:17.000000 waypaper-1.0.4/LICENSE
+-rw-r--r--   0 r         (1000) r         (1000)     1830 2023-08-08 03:52:19.448256 waypaper-1.0.4/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)      996 2023-08-08 03:43:56.000000 waypaper-1.0.4/README.md
+-rw-r--r--   0 r         (1000) r         (1000)       91 2022-11-27 00:35:48.000000 waypaper-1.0.4/pyproject.toml
+-rw-r--r--   0 r         (1000) r         (1000)       38 2023-08-08 03:52:19.448256 waypaper-1.0.4/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1000)     1457 2023-08-08 03:51:54.000000 waypaper-1.0.4/setup.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-08-08 03:52:19.448256 waypaper-1.0.4/waypaper/
+-rw-r--r--   0 r         (1000) r         (1000)      472 2023-08-08 03:52:11.000000 waypaper-1.0.4/waypaper/__main__.py
+-rw-r--r--   0 r         (1000) r         (1000)     8455 2023-08-08 03:11:39.000000 waypaper-1.0.4/waypaper/app.py
+-rw-r--r--   0 r         (1000) r         (1000)      409 2023-08-08 03:10:14.000000 waypaper-1.0.4/waypaper/changer.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-08-08 03:52:19.448256 waypaper-1.0.4/waypaper.egg-info/
+-rw-r--r--   0 r         (1000) r         (1000)     1830 2023-08-08 03:52:19.000000 waypaper-1.0.4/waypaper.egg-info/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)      292 2023-08-08 03:52:19.000000 waypaper-1.0.4/waypaper.egg-info/SOURCES.txt
+-rw-r--r--   0 r         (1000) r         (1000)        1 2023-08-08 03:52:19.000000 waypaper-1.0.4/waypaper.egg-info/dependency_links.txt
+-rw-r--r--   0 r         (1000) r         (1000)       51 2023-08-08 03:52:19.000000 waypaper-1.0.4/waypaper.egg-info/entry_points.txt
+-rw-r--r--   0 r         (1000) r         (1000)       10 2023-08-08 03:52:19.000000 waypaper-1.0.4/waypaper.egg-info/requires.txt
+-rw-r--r--   0 r         (1000) r         (1000)        9 2023-08-08 03:52:19.000000 waypaper-1.0.4/waypaper.egg-info/top_level.txt
```

### Comparing `waypaper-1.0.3/LICENSE` & `waypaper-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `waypaper-1.0.3/PKG-INFO` & `waypaper-1.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: waypaper
-Version: 1.0.3
+Version: 1.0.4
 Summary: GUI wallpaper setter for Wayland
 Home-page: https://github.com/anufrievroman/waypaper
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
-Requires-Python: ~=3.8
+Requires-Python: >3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Waypaper
 
 GUI wallpaper setter for Wayland-based window managers such as Hyprland or Sway.
```

### Comparing `waypaper-1.0.3/README.md` & `waypaper-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `waypaper-1.0.3/setup.py` & `waypaper-1.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,23 +20,24 @@
     entry_points={
         "console_scripts": [
             "waypaper = waypaper.__main__:run"
         ]
     },
     install_requires=["PyGObject"],
     version=version,
-    python_requires='~=3.8',
+    python_requires='>3.10',
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Environment :: Console",
         "Natural Language :: English",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Utilities",
     ],
     packages=["waypaper"],
     include_package_data=True,
 )
```

### Comparing `waypaper-1.0.3/waypaper/app.py` & `waypaper-1.0.4/waypaper/app.py`

 * *Files identical despite different names*

### Comparing `waypaper-1.0.3/waypaper.egg-info/PKG-INFO` & `waypaper-1.0.4/waypaper.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: waypaper
-Version: 1.0.3
+Version: 1.0.4
 Summary: GUI wallpaper setter for Wayland
 Home-page: https://github.com/anufrievroman/waypaper
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
-Requires-Python: ~=3.8
+Requires-Python: >3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Waypaper
 
 GUI wallpaper setter for Wayland-based window managers such as Hyprland or Sway.
```

