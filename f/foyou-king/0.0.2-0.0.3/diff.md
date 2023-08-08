# Comparing `tmp/foyou-king-0.0.2.tar.gz` & `tmp/foyou-king-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foyou-king-0.0.2.tar", last modified: Wed Feb  8 11:30:39 2023, max compression
+gzip compressed data, was "foyou-king-0.0.3.tar", last modified: Tue Aug  8 08:28:48 2023, max compression
```

## Comparing `foyou-king-0.0.2.tar` & `foyou-king-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 11:30:39.921274 foyou-king-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-08 11:30:32.000000 foyou-king-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-02-08 11:30:39.921274 foyou-king-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-02-08 11:30:32.000000 foyou-king-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-02-08 11:30:32.000000 foyou-king-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-08 11:30:32.000000 foyou-king-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 11:30:39.921274 foyou-king-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 11:30:39.917274 foyou-king-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 11:30:39.917274 foyou-king-0.0.2/src/foyou_king.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-02-08 11:30:39.000000 foyou-king-0.0.2/src/foyou_king.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-02-08 11:30:39.000000 foyou-king-0.0.2/src/foyou_king.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 11:30:39.000000 foyou-king-0.0.2/src/foyou_king.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-08 11:30:39.000000 foyou-king-0.0.2/src/foyou_king.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-08 11:30:39.000000 foyou-king-0.0.2/src/foyou_king.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-08 11:30:39.000000 foyou-king-0.0.2/src/foyou_king.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 11:30:39.921274 foyou-king-0.0.2/src/king/
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-02-08 11:30:32.000000 foyou-king-0.0.2/src/king/CompleteSearchResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-02-08 11:30:32.000000 foyou-king-0.0.2/src/king/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-02-08 11:30:32.000000 foyou-king-0.0.2/src/king/DataClass.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-08 11:30:32.000000 foyou-king-0.0.2/src/king/Diy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-02-08 11:30:32.000000 foyou-king-0.0.2/src/king/Downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-08 11:30:32.000000 foyou-king-0.0.2/src/king/Image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-02-08 11:30:32.000000 foyou-king-0.0.2/src/king/King.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-08 11:30:32.000000 foyou-king-0.0.2/src/king/MusicInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-08 11:30:32.000000 foyou-king-0.0.2/src/king/TipResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-08 11:30:32.000000 foyou-king-0.0.2/src/king/Tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-08 11:30:39.000000 foyou-king-0.0.2/src/king/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-02-08 11:30:32.000000 foyou-king-0.0.2/src/king/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-02-08 11:30:32.000000 foyou-king-0.0.2/src/king/yinxiao.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:28:48.862095 foyou-king-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-08 08:28:41.000000 foyou-king-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-08-08 08:28:48.862095 foyou-king-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-08-08 08:28:41.000000 foyou-king-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-08 08:28:41.000000 foyou-king-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-08 08:28:41.000000 foyou-king-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 08:28:48.862095 foyou-king-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:28:48.858095 foyou-king-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:28:48.862095 foyou-king-0.0.3/src/foyou_king.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-08-08 08:28:48.000000 foyou-king-0.0.3/src/foyou_king.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-08 08:28:48.000000 foyou-king-0.0.3/src/foyou_king.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 08:28:48.000000 foyou-king-0.0.3/src/foyou_king.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-08 08:28:48.000000 foyou-king-0.0.3/src/foyou_king.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-08 08:28:48.000000 foyou-king-0.0.3/src/foyou_king.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 08:28:48.000000 foyou-king-0.0.3/src/foyou_king.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:28:48.862095 foyou-king-0.0.3/src/king/
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-08-08 08:28:41.000000 foyou-king-0.0.3/src/king/CompleteSearchResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-08 08:28:41.000000 foyou-king-0.0.3/src/king/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-08-08 08:28:41.000000 foyou-king-0.0.3/src/king/DataClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-08 08:28:41.000000 foyou-king-0.0.3/src/king/Diy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-08-08 08:28:41.000000 foyou-king-0.0.3/src/king/Downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-08 08:28:41.000000 foyou-king-0.0.3/src/king/Image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-08-08 08:28:41.000000 foyou-king-0.0.3/src/king/King.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-08 08:28:41.000000 foyou-king-0.0.3/src/king/MusicInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-08 08:28:41.000000 foyou-king-0.0.3/src/king/TipResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-08 08:28:41.000000 foyou-king-0.0.3/src/king/Tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-08 08:28:48.000000 foyou-king-0.0.3/src/king/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-08-08 08:28:41.000000 foyou-king-0.0.3/src/king/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-08-08 08:28:41.000000 foyou-king-0.0.3/src/king/yinxiao.py
```

### Comparing `foyou-king-0.0.2/LICENSE` & `foyou-king-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `foyou-king-0.0.2/PKG-INFO` & `foyou-king-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foyou-king
-Version: 0.0.2
+Version: 0.0.3
 Summary: search & download kugou-rings
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/foyou-king
 Project-URL: Homepage, https://github.com/foyoux/foyou-king
 Project-URL: Bug Tracker, https://github.com/foyoux/foyou-king/issues
 Keywords: foyou-king
 Classifier: Programming Language :: Python
```

### Comparing `foyou-king-0.0.2/README.md` & `foyou-king-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `foyou-king-0.0.2/pyproject.toml` & `foyou-king-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `foyou-king-0.0.2/src/foyou_king.egg-info/PKG-INFO` & `foyou-king-0.0.3/src/foyou_king.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foyou-king
-Version: 0.0.2
+Version: 0.0.3
 Summary: search & download kugou-rings
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/foyou-king
 Project-URL: Homepage, https://github.com/foyoux/foyou-king
 Project-URL: Bug Tracker, https://github.com/foyoux/foyou-king/issues
 Keywords: foyou-king
 Classifier: Programming Language :: Python
```

### Comparing `foyou-king-0.0.2/src/foyou_king.egg-info/SOURCES.txt` & `foyou-king-0.0.3/src/foyou_king.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foyou-king-0.0.2/src/king/CompleteSearchResponse.py` & `foyou-king-0.0.3/src/king/CompleteSearchResponse.py`

 * *Files identical despite different names*

### Comparing `foyou-king-0.0.2/src/king/DataClass.py` & `foyou-king-0.0.3/src/king/DataClass.py`

 * *Files identical despite different names*

### Comparing `foyou-king-0.0.2/src/king/Diy.py` & `foyou-king-0.0.3/src/king/Diy.py`

 * *Files identical despite different names*

### Comparing `foyou-king-0.0.2/src/king/Downloader.py` & `foyou-king-0.0.3/src/king/Downloader.py`

 * *Files identical despite different names*

### Comparing `foyou-king-0.0.2/src/king/King.py` & `foyou-king-0.0.3/src/king/King.py`

 * *Files identical despite different names*

### Comparing `foyou-king-0.0.2/src/king/MusicInfo.py` & `foyou-king-0.0.3/src/king/MusicInfo.py`

 * *Files identical despite different names*

### Comparing `foyou-king-0.0.2/src/king/main.py` & `foyou-king-0.0.3/src/king/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Tuple
 
 import fire
 import urllib3
 from urllib3.exceptions import InsecureRequestWarning
 
 from king import __version__, King
+from king.MusicInfo import MusicInfo
 from king.yinxiao import YinXiao
 
 urllib3.disable_warnings(InsecureRequestWarning)
 
 
 class CLI:
 
@@ -38,25 +39,31 @@
         """
         king = King()
         print('{:^10}{:8}{:<30}'.format('热度', '', '搜索词'))
         for tip in king.get_tip_list(q, pn):
             print('{:>8}{:8}{:<30}'.format(tip.Hot, '', tip.HintInfo))
 
     @staticmethod
-    def down(q: str, p=1, pn=10, n: Tuple[int] = None, d='.'):
+    def down(q: str, p=1, pn=10, n: Tuple[int] = None, d='.', complex: bool = False):
         """下载铃声
 
         q: 关键词
         p: 页码
         pn: 分页大小（获取多少条）
         n: 需要下载的序号，-n 1 或者 -n 2,5,7
         d: 下载目录
         """
         king = King(d)
-        rings = king.all_search(q, p=p, pn=pn)
+        if complex:
+            results = king.complex_search(q)
+            rings = []
+            rings.extend([MusicInfo(ringName=i.ringName, url=i.url) for i in results.crbt_list])
+            rings.extend([MusicInfo(ringName=i.ringName, url=i.url) for i in results.audio_list])
+        else:
+            rings = king.all_search(q, p=p, pn=pn)
         if n is None:
             for ring in rings:
                 king.download_ring(ring.ringName, ring.url)
         else:
             if isinstance(n, int):
                 n = (n,)
             for i in n:
```

### Comparing `foyou-king-0.0.2/src/king/yinxiao.py` & `foyou-king-0.0.3/src/king/yinxiao.py`

 * *Files identical despite different names*

