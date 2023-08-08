# Comparing `tmp/yeref-0.2.90.tar.gz` & `tmp/yeref-0.2.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.2.90.tar", last modified: Tue Aug  8 13:30:03 2023, max compression
+gzip compressed data, was "yeref-0.2.91.tar", last modified: Tue Aug  8 13:34:54 2023, max compression
```

## Comparing `yeref-0.2.90.tar` & `yeref-0.2.91.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 13:30:03.321142 yeref-0.2.90/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 13:30:03.321284 yeref-0.2.90/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-08 13:30:03.321869 yeref-0.2.90/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1552 2023-08-08 13:29:34.000000 yeref-0.2.90/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 13:30:03.314963 yeref-0.2.90/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.90/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   583683 2023-08-06 16:53:26.000000 yeref-0.2.90/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   232838 2023-08-08 13:29:34.000000 yeref-0.2.90/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 13:30:03.320782 yeref-0.2.90/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 13:30:03.000000 yeref-0.2.90/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-08-08 13:30:03.000000 yeref-0.2.90/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-08 13:30:03.000000 yeref-0.2.90/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-08-08 13:30:03.000000 yeref-0.2.90/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 13:34:54.877581 yeref-0.2.91/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 13:34:54.877857 yeref-0.2.91/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-08 13:34:54.879194 yeref-0.2.91/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1552 2023-08-08 13:34:35.000000 yeref-0.2.91/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 13:34:54.869992 yeref-0.2.91/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.91/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   583683 2023-08-06 16:53:26.000000 yeref-0.2.91/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   232848 2023-08-08 13:34:35.000000 yeref-0.2.91/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 13:34:54.876447 yeref-0.2.91/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 13:34:54.000000 yeref-0.2.91/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-08-08 13:34:54.000000 yeref-0.2.91/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-08 13:34:54.000000 yeref-0.2.91/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-08-08 13:34:54.000000 yeref-0.2.91/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.2.90/setup.py` & `yeref-0.2.91/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.2.90',
+      version='0.2.91',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.2.90/yeref/l_.py` & `yeref-0.2.91/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.2.90/yeref/yeref.py` & `yeref-0.2.91/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
             await updateMedia();
             const roundedMedia = document.querySelectorAll('.rounded-media');
             for (let i = 0; i < roundedMedia.length; i++) roundedMedia[i].style.width = "auto";
         }})
         async function fetchData(url) {{
             try {{
                 const response = await fetch(url);
-                console.log('dd:', data)
+                console.log('response:', response)
             }} catch (error) {{
                 console.log('Error fetching data:', error);
                 return null;
             }}
         }}
 
         async function handleButtonClick(button) {{
```

