# Comparing `tmp/practice_japanese-0.0.2.tar.gz` & `tmp/practice_japanese-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "practice_japanese-0.0.2.tar", last modified: Thu Aug  3 13:52:01 2023, max compression
+gzip compressed data, was "practice_japanese-0.1.0.tar", last modified: Tue Aug  8 12:39:00 2023, max compression
```

## Comparing `practice_japanese-0.0.2.tar` & `practice_japanese-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 heather   (1000) heather   (1000)        0 2023-08-03 13:52:01.095422 practice_japanese-0.0.2/
--rw-r--r--   0 heather   (1000) heather   (1000)    18092 2023-08-03 13:07:05.000000 practice_japanese-0.0.2/LICENSE
--rw-r--r--   0 heather   (1000) heather   (1000)       42 2023-08-03 13:44:43.000000 practice_japanese-0.0.2/MANIFEST.in
--rw-r--r--   0 heather   (1000) heather   (1000)     1507 2023-08-03 13:52:01.095422 practice_japanese-0.0.2/PKG-INFO
--rw-r--r--   0 heather   (1000) heather   (1000)     1045 2023-08-03 13:35:58.000000 practice_japanese-0.0.2/README.md
-drwxr-xr-x   0 heather   (1000) heather   (1000)        0 2023-08-03 13:52:01.095422 practice_japanese-0.0.2/practice_japanese/
--rw-r--r--   0 heather   (1000) heather   (1000)        0 2023-08-03 13:07:41.000000 practice_japanese-0.0.2/practice_japanese/__init__.py
-drwxr-xr-x   0 heather   (1000) heather   (1000)        0 2023-08-03 13:52:01.095422 practice_japanese-0.0.2/practice_japanese/character_sets/
--rw-r--r--   0 heather   (1000) heather   (1000)        0 2023-08-03 13:07:41.000000 practice_japanese-0.0.2/practice_japanese/character_sets/__init__.py
--rw-r--r--   0 heather   (1000) heather   (1000)      939 2023-08-03 13:14:07.000000 practice_japanese-0.0.2/practice_japanese/character_sets/hiragana.py
--rwxr-xr-x   0 heather   (1000) heather   (1000)     2895 2023-08-03 13:11:11.000000 practice_japanese-0.0.2/practice_japanese/character_statistics.py
--rw-r--r--   0 heather   (1000) heather   (1000)     1694 2023-08-03 13:50:05.000000 practice_japanese-0.0.2/practice_japanese/command_line.py
--rw-r--r--   0 heather   (1000) heather   (1000)       22 2023-08-03 13:51:06.000000 practice_japanese-0.0.2/practice_japanese/version.py
-drwxr-xr-x   0 heather   (1000) heather   (1000)        0 2023-08-03 13:52:01.095422 practice_japanese-0.0.2/practice_japanese.egg-info/
--rw-r--r--   0 heather   (1000) heather   (1000)     1507 2023-08-03 13:52:01.000000 practice_japanese-0.0.2/practice_japanese.egg-info/PKG-INFO
--rw-r--r--   0 heather   (1000) heather   (1000)      488 2023-08-03 13:52:01.000000 practice_japanese-0.0.2/practice_japanese.egg-info/SOURCES.txt
--rw-r--r--   0 heather   (1000) heather   (1000)        1 2023-08-03 13:52:01.000000 practice_japanese-0.0.2/practice_japanese.egg-info/dependency_links.txt
--rw-r--r--   0 heather   (1000) heather   (1000)       73 2023-08-03 13:52:01.000000 practice_japanese-0.0.2/practice_japanese.egg-info/entry_points.txt
--rw-r--r--   0 heather   (1000) heather   (1000)       18 2023-08-03 13:52:01.000000 practice_japanese-0.0.2/practice_japanese.egg-info/top_level.txt
--rw-r--r--   0 heather   (1000) heather   (1000)        0 2023-08-03 13:43:25.000000 practice_japanese-0.0.2/requirements.txt
--rw-r--r--   0 heather   (1000) heather   (1000)       38 2023-08-03 13:52:01.095422 practice_japanese-0.0.2/setup.cfg
--rw-r--r--   0 heather   (1000) heather   (1000)     1294 2023-08-03 13:44:04.000000 practice_japanese-0.0.2/setup.py
+drwxr-xr-x   0 heather   (1000) heather   (1000)        0 2023-08-08 12:39:00.457477 practice_japanese-0.1.0/
+-rw-r--r--   0 heather   (1000) heather   (1000)    18092 2023-08-03 13:07:05.000000 practice_japanese-0.1.0/LICENSE
+-rw-r--r--   0 heather   (1000) heather   (1000)       42 2023-08-03 13:44:43.000000 practice_japanese-0.1.0/MANIFEST.in
+-rw-r--r--   0 heather   (1000) heather   (1000)     1509 2023-08-08 12:39:00.457477 practice_japanese-0.1.0/PKG-INFO
+-rw-r--r--   0 heather   (1000) heather   (1000)     1047 2023-08-08 12:36:17.000000 practice_japanese-0.1.0/README.md
+drwxr-xr-x   0 heather   (1000) heather   (1000)        0 2023-08-08 12:39:00.453477 practice_japanese-0.1.0/practice_japanese/
+-rw-r--r--   0 heather   (1000) heather   (1000)        0 2023-08-03 13:07:41.000000 practice_japanese-0.1.0/practice_japanese/__init__.py
+drwxr-xr-x   0 heather   (1000) heather   (1000)        0 2023-08-08 12:39:00.457477 practice_japanese-0.1.0/practice_japanese/character_sets/
+-rw-r--r--   0 heather   (1000) heather   (1000)        0 2023-08-03 13:07:41.000000 practice_japanese-0.1.0/practice_japanese/character_sets/__init__.py
+-rw-r--r--   0 heather   (1000) heather   (1000)     1378 2023-08-08 12:37:18.000000 practice_japanese-0.1.0/practice_japanese/character_sets/hiragana.py
+-rwxr-xr-x   0 heather   (1000) heather   (1000)     2895 2023-08-03 13:11:11.000000 practice_japanese-0.1.0/practice_japanese/character_statistics.py
+-rw-r--r--   0 heather   (1000) heather   (1000)     1694 2023-08-03 13:50:05.000000 practice_japanese-0.1.0/practice_japanese/command_line.py
+-rw-r--r--   0 heather   (1000) heather   (1000)       22 2023-08-08 12:37:18.000000 practice_japanese-0.1.0/practice_japanese/version.py
+drwxr-xr-x   0 heather   (1000) heather   (1000)        0 2023-08-08 12:39:00.457477 practice_japanese-0.1.0/practice_japanese.egg-info/
+-rw-r--r--   0 heather   (1000) heather   (1000)     1509 2023-08-08 12:39:00.000000 practice_japanese-0.1.0/practice_japanese.egg-info/PKG-INFO
+-rw-r--r--   0 heather   (1000) heather   (1000)      488 2023-08-08 12:39:00.000000 practice_japanese-0.1.0/practice_japanese.egg-info/SOURCES.txt
+-rw-r--r--   0 heather   (1000) heather   (1000)        1 2023-08-08 12:39:00.000000 practice_japanese-0.1.0/practice_japanese.egg-info/dependency_links.txt
+-rw-r--r--   0 heather   (1000) heather   (1000)       73 2023-08-08 12:39:00.000000 practice_japanese-0.1.0/practice_japanese.egg-info/entry_points.txt
+-rw-r--r--   0 heather   (1000) heather   (1000)       18 2023-08-08 12:39:00.000000 practice_japanese-0.1.0/practice_japanese.egg-info/top_level.txt
+-rw-r--r--   0 heather   (1000) heather   (1000)        0 2023-08-03 13:43:25.000000 practice_japanese-0.1.0/requirements.txt
+-rw-r--r--   0 heather   (1000) heather   (1000)       38 2023-08-08 12:39:00.457477 practice_japanese-0.1.0/setup.cfg
+-rw-r--r--   0 heather   (1000) heather   (1000)     1294 2023-08-03 13:44:04.000000 practice_japanese-0.1.0/setup.py
```

### Comparing `practice_japanese-0.0.2/LICENSE` & `practice_japanese-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `practice_japanese-0.0.2/PKG-INFO` & `practice_japanese-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: practice_japanese
-Version: 0.0.2
+Version: 0.1.0
 Summary: Practice Japanese character sets.
 Home-page: https://github.com/hkeward/practice_japanese
 Author: Heather Ward
 Author-email: heather.ward13@gmail.com
 License: gpl-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -19,15 +19,15 @@
 ## Requirements
 
 - Python3.6+
 
 ## Installation
 
 ```bash
-sudo python3 setup.py install
+python3 setup.py install --user
 ```
 
 This will create a CLI called `practice_japanese` on your PATH.
 
 Alternatively, install via pip:
 
 ```bash
```

### Comparing `practice_japanese-0.0.2/README.md` & `practice_japanese-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ## Requirements
 
 - Python3.6+
 
 ## Installation
 
 ```bash
-sudo python3 setup.py install
+python3 setup.py install --user
 ```
 
 This will create a CLI called `practice_japanese` on your PATH.
 
 Alternatively, install via pip:
 
 ```bash
```

### Comparing `practice_japanese-0.0.2/practice_japanese/character_sets/hiragana.py` & `practice_japanese-0.1.0/practice_japanese/character_sets/hiragana.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,28 @@
 
     t = {"た": "ta", "て": "te", "ち": "chi", "と": "to", "つ": "tsu"}
 
     w = {"わ": "wa", "を": "o"}
 
     y = {"や": "ya", "よ": "yo", "ゆ": "yu"}
 
-    hiragana = {**vowels, **h, **k, **m, **n, **r, **s, **t, **w, **y}
+    # dakuon
+
+    b = {"ば": "ba", "べ": "be", "び": "bi", "ぼ": "bo", "ぶ": "bu"}
+
+    d = {"だ": "da", "で": "de", "ぢ": "di", "ど": "do", "づ": "du"}
+
+    g = {"が": "ga", "げ": "ge", "ぎ": "gi", "ご": "go", "ぐ": "gu"}
+
+    p = {"ぱ": "pa", "ぺ": "pe", "ぴ": "pi", "ぽ": "po", "ぷ": "pu"}
+
+    z = {"ざ": "za", "ぜ": "ze", "じ": "ji", "ぞ": "zo", "ず": "zu"}
+
+    dakuon = {**b, **d, **g, **p, **z}
+
+    hiragana = {**vowels, **h, **k, **m, **n, **r, **s, **t, **w, **y, **dakuon}
 
     def __str__(self):
         return self._name_
 
 
 reverse_hiragana = {v: k for k, v in Hiragana.hiragana.value.items()}
```

### Comparing `practice_japanese-0.0.2/practice_japanese/character_statistics.py` & `practice_japanese-0.1.0/practice_japanese/character_statistics.py`

 * *Files identical despite different names*

### Comparing `practice_japanese-0.0.2/practice_japanese/command_line.py` & `practice_japanese-0.1.0/practice_japanese/command_line.py`

 * *Files identical despite different names*

### Comparing `practice_japanese-0.0.2/practice_japanese.egg-info/PKG-INFO` & `practice_japanese-0.1.0/practice_japanese.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: practice-japanese
-Version: 0.0.2
+Version: 0.1.0
 Summary: Practice Japanese character sets.
 Home-page: https://github.com/hkeward/practice_japanese
 Author: Heather Ward
 Author-email: heather.ward13@gmail.com
 License: gpl-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -19,15 +19,15 @@
 ## Requirements
 
 - Python3.6+
 
 ## Installation
 
 ```bash
-sudo python3 setup.py install
+python3 setup.py install --user
 ```
 
 This will create a CLI called `practice_japanese` on your PATH.
 
 Alternatively, install via pip:
 
 ```bash
```

### Comparing `practice_japanese-0.0.2/setup.py` & `practice_japanese-0.1.0/setup.py`

 * *Files identical despite different names*

