# Comparing `tmp/oa_pynput-1.7.6.tar.gz` & `tmp/oa_pynput-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oa_pynput-1.7.6.tar", last modified: Sat Aug  5 01:42:47 2023, max compression
+gzip compressed data, was "oa_pynput-1.7.7.tar", last modified: Tue Aug  8 20:34:04 2023, max compression
```

## Comparing `oa_pynput-1.7.6.tar` & `oa_pynput-1.7.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 01:42:47.349161 oa_pynput-1.7.6/
--rw-rw-rw-   0        0        0     7821 2023-07-24 16:14:16.000000 oa_pynput-1.7.6/COPYING.LGPL
--rw-rw-rw-   0        0        0     1518 2023-08-05 01:42:47.349161 oa_pynput-1.7.6/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-24 16:14:16.000000 oa_pynput-1.7.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-05 01:42:47.225193 oa_pynput-1.7.6/lib/
-drwxrwxrwx   0        0        0        0 2023-08-05 01:42:47.241388 oa_pynput-1.7.6/lib/oa_pynput/
--rw-rw-rw-   0        0        0     1375 2023-07-24 16:14:16.000000 oa_pynput-1.7.6/lib/oa_pynput/__init__.py
--rw-rw-rw-   0        0        0      794 2023-07-24 16:14:16.000000 oa_pynput-1.7.6/lib/oa_pynput/_info.py
-drwxrwxrwx   0        0        0        0 2023-08-05 01:42:47.304381 oa_pynput-1.7.6/lib/oa_pynput/_util/
--rw-rw-rw-   0        0        0    15998 2023-07-24 16:14:16.000000 oa_pynput-1.7.6/lib/oa_pynput/_util/__init__.py
--rw-rw-rw-   0        0        0     9465 2023-07-24 16:14:16.000000 oa_pynput-1.7.6/lib/oa_pynput/_util/darwin.py
--rw-rw-rw-   0        0        0     1591 2023-07-24 16:14:16.000000 oa_pynput-1.7.6/lib/oa_pynput/_util/darwin_vks.py
--rw-rw-rw-   0        0        0     2912 2023-07-24 16:14:16.000000 oa_pynput-1.7.6/lib/oa_pynput/_util/uinput.py
--rw-rw-rw-   0        0        0    18708 2023-07-24 16:14:16.000000 oa_pynput-1.7.6/lib/oa_pynput/_util/win32.py
--rw-rw-rw-   0        0        0     3073 2023-07-24 16:14:16.000000 oa_pynput-1.7.6/lib/oa_pynput/_util/win32_vks.py
--rw-rw-rw-   0        0        0    15772 2023-07-24 16:14:16.000000 oa_pynput-1.7.6/lib/oa_pynput/_util/xorg.py
--rw-rw-rw-   0        0        0    71053 2023-07-24 16:14:16.000000 oa_pynput-1.7.6/lib/oa_pynput/_util/xorg_keysyms.py
-drwxrwxrwx   0        0        0        0 2023-08-05 01:42:47.327118 oa_pynput-1.7.6/lib/oa_pynput/keyboard/
--rw-rw-rw-   0        0        0     7753 2023-08-04 23:26:17.000000 oa_pynput-1.7.6/lib/oa_pynput/keyboard/__init__.py
--rw-rw-rw-   0        0        0    23750 2023-08-04 23:21:29.000000 oa_pynput-1.7.6/lib/oa_pynput/keyboard/_base.py
--rw-rw-rw-   0        0        0    11735 2023-08-04 23:27:12.000000 oa_pynput-1.7.6/lib/oa_pynput/keyboard/_darwin.py
--rw-rw-rw-   0        0        0      918 2023-07-24 16:14:16.000000 oa_pynput-1.7.6/lib/oa_pynput/keyboard/_dummy.py
--rw-rw-rw-   0        0        0    14849 2023-08-04 23:27:32.000000 oa_pynput-1.7.6/lib/oa_pynput/keyboard/_uinput.py
--rw-rw-rw-   0        0        0    11757 2023-08-04 23:27:46.000000 oa_pynput-1.7.6/lib/oa_pynput/keyboard/_win32.py
--rw-rw-rw-   0        0        0    23336 2023-08-04 23:28:17.000000 oa_pynput-1.7.6/lib/oa_pynput/keyboard/_xorg.py
-drwxrwxrwx   0        0        0        0 2023-08-05 01:42:47.346498 oa_pynput-1.7.6/lib/oa_pynput/mouse/
--rw-rw-rw-   0        0        0     2677 2023-08-04 23:28:32.000000 oa_pynput-1.7.6/lib/oa_pynput/mouse/__init__.py
--rw-rw-rw-   0        0        0     9432 2023-08-04 23:28:44.000000 oa_pynput-1.7.6/lib/oa_pynput/mouse/_base.py
--rw-rw-rw-   0        0        0     7010 2023-08-04 23:28:54.000000 oa_pynput-1.7.6/lib/oa_pynput/mouse/_darwin.py
--rw-rw-rw-   0        0        0      896 2023-07-24 16:14:16.000000 oa_pynput-1.7.6/lib/oa_pynput/mouse/_dummy.py
--rw-rw-rw-   0        0        0     7330 2023-08-04 23:29:08.000000 oa_pynput-1.7.6/lib/oa_pynput/mouse/_win32.py
--rw-rw-rw-   0        0        0     5741 2023-08-04 23:29:28.000000 oa_pynput-1.7.6/lib/oa_pynput/mouse/_xorg.py
-drwxrwxrwx   0        0        0        0 2023-08-05 01:42:47.278921 oa_pynput-1.7.6/lib/oa_pynput.egg-info/
--rw-rw-rw-   0        0        0     1518 2023-08-05 01:42:47.000000 oa_pynput-1.7.6/lib/oa_pynput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      973 2023-08-05 01:42:47.000000 oa_pynput-1.7.6/lib/oa_pynput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 01:42:47.000000 oa_pynput-1.7.6/lib/oa_pynput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      196 2023-08-05 01:42:47.000000 oa_pynput-1.7.6/lib/oa_pynput.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-05 01:42:47.000000 oa_pynput-1.7.6/lib/oa_pynput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-08-04 23:51:02.000000 oa_pynput-1.7.6/lib/oa_pynput.egg-info/zip-safe
--rw-rw-rw-   0        0        0      199 2023-08-05 01:42:47.351765 oa_pynput-1.7.6/setup.cfg
--rw-rw-rw-   0        0        0     3157 2023-08-05 01:42:15.000000 oa_pynput-1.7.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:34:04.203419 oa_pynput-1.7.7/
+-rw-rw-rw-   0        0        0     7821 2023-07-24 16:14:16.000000 oa_pynput-1.7.7/COPYING.LGPL
+-rw-rw-rw-   0        0        0     1515 2023-08-08 20:34:04.204571 oa_pynput-1.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-24 16:14:16.000000 oa_pynput-1.7.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-08 20:34:04.101779 oa_pynput-1.7.7/lib/
+drwxrwxrwx   0        0        0        0 2023-08-08 20:34:04.116723 oa_pynput-1.7.7/lib/oa_pynput/
+-rw-rw-rw-   0        0        0     1375 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/__init__.py
+-rw-rw-rw-   0        0        0      794 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/_info.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:34:04.169354 oa_pynput-1.7.7/lib/oa_pynput/_util/
+-rw-rw-rw-   0        0        0    15998 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/_util/__init__.py
+-rw-rw-rw-   0        0        0     9465 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/_util/darwin.py
+-rw-rw-rw-   0        0        0     1591 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/_util/darwin_vks.py
+-rw-rw-rw-   0        0        0     2912 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/_util/uinput.py
+-rw-rw-rw-   0        0        0    18708 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/_util/win32.py
+-rw-rw-rw-   0        0        0     3073 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/_util/win32_vks.py
+-rw-rw-rw-   0        0        0    15772 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/_util/xorg.py
+-rw-rw-rw-   0        0        0    71053 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/_util/xorg_keysyms.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:34:04.186830 oa_pynput-1.7.7/lib/oa_pynput/keyboard/
+-rw-rw-rw-   0        0        0     7753 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/keyboard/__init__.py
+-rw-rw-rw-   0        0        0    23750 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/keyboard/_base.py
+-rw-rw-rw-   0        0        0    11735 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/keyboard/_darwin.py
+-rw-rw-rw-   0        0        0      918 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/keyboard/_dummy.py
+-rw-rw-rw-   0        0        0    14849 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/keyboard/_uinput.py
+-rw-rw-rw-   0        0        0    11757 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/keyboard/_win32.py
+-rw-rw-rw-   0        0        0    23336 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/keyboard/_xorg.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:34:04.201171 oa_pynput-1.7.7/lib/oa_pynput/mouse/
+-rw-rw-rw-   0        0        0     2677 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/mouse/__init__.py
+-rw-rw-rw-   0        0        0     9432 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/mouse/_base.py
+-rw-rw-rw-   0        0        0     7010 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/mouse/_darwin.py
+-rw-rw-rw-   0        0        0      896 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/mouse/_dummy.py
+-rw-rw-rw-   0        0        0     7330 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/mouse/_win32.py
+-rw-rw-rw-   0        0        0     5741 2023-08-08 19:02:27.000000 oa_pynput-1.7.7/lib/oa_pynput/mouse/_xorg.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:34:04.146943 oa_pynput-1.7.7/lib/oa_pynput.egg-info/
+-rw-rw-rw-   0        0        0     1515 2023-08-08 20:34:04.000000 oa_pynput-1.7.7/lib/oa_pynput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      973 2023-08-08 20:34:04.000000 oa_pynput-1.7.7/lib/oa_pynput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 20:34:04.000000 oa_pynput-1.7.7/lib/oa_pynput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      196 2023-08-08 20:34:04.000000 oa_pynput-1.7.7/lib/oa_pynput.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-08 20:34:04.000000 oa_pynput-1.7.7/lib/oa_pynput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-08-04 23:51:02.000000 oa_pynput-1.7.7/lib/oa_pynput.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      199 2023-08-08 20:34:04.206498 oa_pynput-1.7.7/setup.cfg
+-rw-rw-rw-   0        0        0     3140 2023-08-08 20:33:48.000000 oa_pynput-1.7.7/setup.py
```

### Comparing `oa_pynput-1.7.6/COPYING.LGPL` & `oa_pynput-1.7.7/COPYING.LGPL`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/PKG-INFO` & `oa_pynput-1.7.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: oa_pynput
-Version: 1.7.6
+Version: 1.7.7
 Summary: Monitor and control user input devices
 Home-page: https://github.com/OpenAdaptAI/pynput
 Author: Moses Palmér
-Author-email: richard.abrich@mldsai.com
+Author-email: moses.palmer@gmail.com
 License: LGPLv3
 Keywords: control mouse,mouse input,control keyboard,keyboard input
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/__init__.py` & `oa_pynput-1.7.7/lib/oa_pynput/__init__.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/_info.py` & `oa_pynput-1.7.7/lib/oa_pynput/_info.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/_util/__init__.py` & `oa_pynput-1.7.7/lib/oa_pynput/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/_util/darwin.py` & `oa_pynput-1.7.7/lib/oa_pynput/_util/darwin.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/_util/darwin_vks.py` & `oa_pynput-1.7.7/lib/oa_pynput/_util/darwin_vks.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/_util/uinput.py` & `oa_pynput-1.7.7/lib/oa_pynput/_util/uinput.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/_util/win32.py` & `oa_pynput-1.7.7/lib/oa_pynput/_util/win32.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/_util/win32_vks.py` & `oa_pynput-1.7.7/lib/oa_pynput/_util/win32_vks.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/_util/xorg.py` & `oa_pynput-1.7.7/lib/oa_pynput/_util/xorg.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/_util/xorg_keysyms.py` & `oa_pynput-1.7.7/lib/oa_pynput/_util/xorg_keysyms.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/keyboard/__init__.py` & `oa_pynput-1.7.7/lib/oa_pynput/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/keyboard/_base.py` & `oa_pynput-1.7.7/lib/oa_pynput/keyboard/_base.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/keyboard/_darwin.py` & `oa_pynput-1.7.7/lib/oa_pynput/keyboard/_darwin.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/keyboard/_dummy.py` & `oa_pynput-1.7.7/lib/oa_pynput/keyboard/_dummy.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/keyboard/_uinput.py` & `oa_pynput-1.7.7/lib/oa_pynput/keyboard/_uinput.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/keyboard/_win32.py` & `oa_pynput-1.7.7/lib/oa_pynput/keyboard/_win32.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/keyboard/_xorg.py` & `oa_pynput-1.7.7/lib/oa_pynput/keyboard/_xorg.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/mouse/__init__.py` & `oa_pynput-1.7.7/lib/oa_pynput/mouse/__init__.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/mouse/_base.py` & `oa_pynput-1.7.7/lib/oa_pynput/mouse/_base.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/mouse/_darwin.py` & `oa_pynput-1.7.7/lib/oa_pynput/mouse/_darwin.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/mouse/_dummy.py` & `oa_pynput-1.7.7/lib/oa_pynput/mouse/_dummy.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/mouse/_win32.py` & `oa_pynput-1.7.7/lib/oa_pynput/mouse/_win32.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput/mouse/_xorg.py` & `oa_pynput-1.7.7/lib/oa_pynput/mouse/_xorg.py`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/lib/oa_pynput.egg-info/PKG-INFO` & `oa_pynput-1.7.7/lib/oa_pynput.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: oa-pynput
-Version: 1.7.6
+Version: 1.7.7
 Summary: Monitor and control user input devices
 Home-page: https://github.com/OpenAdaptAI/pynput
 Author: Moses Palmér
-Author-email: richard.abrich@mldsai.com
+Author-email: moses.palmer@gmail.com
 License: LGPLv3
 Keywords: control mouse,mouse input,control keyboard,keyboard input
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `oa_pynput-1.7.6/lib/oa_pynput.egg-info/SOURCES.txt` & `oa_pynput-1.7.7/lib/oa_pynput.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oa_pynput-1.7.6/setup.py` & `oa_pynput-1.7.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 #: The name of the main Python package
 MAIN_PACKAGE_NAME = 'oa_pynput'
 
 #: The package URL
 PACKAGE_URL = 'https://github.com/OpenAdaptAI/pynput'
 
 #: The author email
-AUTHOR_EMAIL = 'richard.abrich@mldsai.com'
+AUTHOR_EMAIL = 'moses.palmer@gmail.com'
 
 #: The runtime requirements
 RUNTIME_PACKAGES = [
     'six']
 
 #: Additional requirements used during setup
 SETUP_PACKAGES = [
     'setuptools-lint >=0.5',
-    'sphinx >=1.3.1']
+    'sphinx >=1.3.1',
+    'twine >=4.0']
 
 #: Packages requires for different environments
 EXTRA_PACKAGES = {
     ':sys_platform == "darwin"': [
         'pyobjc-framework-ApplicationServices >=8.0',
         'pyobjc-framework-Quartz >=8.0'],
     ':"linux" in sys_platform': [
@@ -57,15 +58,15 @@
 # Load the read me
 with open("README.md", "r", encoding="utf-8") as fh:
     README = fh.read()
 
 
 setuptools.setup(
     name=PYPI_PACKAGE_NAME,
-    version='.'.join(str(i) for i in INFO['version']),
+    version='1.7.7',
     description='Monitor and control user input devices',
     long_description=README,
     long_description_content_type='text/markdown', 
 
     install_requires=RUNTIME_PACKAGES,
     setup_requires=RUNTIME_PACKAGES + SETUP_PACKAGES,
     extras_require=EXTRA_PACKAGES,
```

