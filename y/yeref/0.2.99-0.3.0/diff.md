# Comparing `tmp/yeref-0.2.99.tar.gz` & `tmp/yeref-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.2.99.tar", last modified: Tue Aug  8 16:30:21 2023, max compression
+gzip compressed data, was "yeref-0.3.0.tar", last modified: Tue Aug  8 17:16:58 2023, max compression
```

## Comparing `yeref-0.2.99.tar` & `yeref-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 16:30:21.808267 yeref-0.2.99/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 16:30:21.808463 yeref-0.2.99/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-08 16:30:21.809628 yeref-0.2.99/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1552 2023-08-08 16:30:08.000000 yeref-0.2.99/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 16:30:21.804727 yeref-0.2.99/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.99/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   583683 2023-08-06 16:53:26.000000 yeref-0.2.99/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   238926 2023-08-08 16:30:08.000000 yeref-0.2.99/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 16:30:21.807619 yeref-0.2.99/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 16:30:21.000000 yeref-0.2.99/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-08-08 16:30:21.000000 yeref-0.2.99/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-08 16:30:21.000000 yeref-0.2.99/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-08-08 16:30:21.000000 yeref-0.2.99/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 17:16:58.617169 yeref-0.3.0/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-08-08 17:16:58.617388 yeref-0.3.0/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-08 17:16:58.618262 yeref-0.3.0/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1553 2023-08-08 17:16:43.000000 yeref-0.3.0/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 17:16:58.611652 yeref-0.3.0/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.3.0/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   583683 2023-08-06 16:53:26.000000 yeref-0.3.0/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   238926 2023-08-08 16:30:08.000000 yeref-0.3.0/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 17:16:58.616655 yeref-0.3.0/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-08-08 17:16:58.000000 yeref-0.3.0/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-08-08 17:16:58.000000 yeref-0.3.0/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-08 17:16:58.000000 yeref-0.3.0/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-08-08 17:16:58.000000 yeref-0.3.0/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.2.99/setup.py` & `yeref-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.2.99',
+      version='0.3.00',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -41,13 +41,13 @@
 
 # python -m build; twine upload --username freey.sitner.ya --password cejwez-nosgin-vaVfe7 dist/* ; python3 -m pip install --upgrade yeref ; python3 -m pip install --upgrade yeref
 # twine upload dist/*
 # freey.sitner.ya
 # cejwez-nosgin-vaVfe7
 
 # python3 -m pip install --upgrade yeref
-
+#
 # python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.99-py3-none-any.whl
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.2.99/yeref/l_.py` & `yeref-0.3.0/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.2.99/yeref/yeref.py` & `yeref-0.3.0/yeref/yeref.py`

 * *Files identical despite different names*

