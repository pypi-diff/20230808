# Comparing `tmp/tensoul-0.1.3.tar.gz` & `tmp/tensoul-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensoul-0.1.3.tar", max compression
+gzip compressed data, was "tensoul-0.1.4.tar", max compression
```

## Comparing `tensoul-0.1.3.tar` & `tensoul-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      445 2023-06-27 02:49:07.715727 tensoul-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      944 2023-05-25 04:14:31.440763 tensoul-0.1.3/README.md
--rw-r--r--   0        0        0       48 2023-05-24 15:43:55.027885 tensoul-0.1.3/tensoul/__init__.py
--rw-r--r--   0        0        0   168833 2023-05-25 02:49:24.087394 tensoul-0.1.3/tensoul/cfg.json
--rw-r--r--   0        0        0      163 2023-05-24 15:36:34.423992 tensoul-0.1.3/tensoul/cfg.py
--rw-r--r--   0        0        0     2377 2023-05-29 02:03:29.081206 tensoul-0.1.3/tensoul/constants.py
--rw-r--r--   0        0        0     7056 2023-05-25 08:27:21.930832 tensoul-0.1.3/tensoul/downloader.py
--rw-r--r--   0        0        0    10263 2023-06-27 02:49:01.395547 tensoul-0.1.3/tensoul/model.py
--rw-r--r--   0        0        0    14218 2023-05-29 01:57:19.665195 tensoul-0.1.3/tensoul/parser.py
--rw-r--r--   0        0        0      452 2023-05-25 04:10:00.171590 tensoul-0.1.3/tensoul/utils.py
--rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 tensoul-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      445 2023-08-08 14:05:53.142349 tensoul-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      944 2023-05-25 04:14:31.440763 tensoul-0.1.4/README.md
+-rw-r--r--   0        0        0       48 2023-05-24 15:43:55.027885 tensoul-0.1.4/tensoul/__init__.py
+-rw-r--r--   0        0        0   168833 2023-05-25 02:49:24.087394 tensoul-0.1.4/tensoul/cfg.json
+-rw-r--r--   0        0        0      163 2023-05-24 15:36:34.423992 tensoul-0.1.4/tensoul/cfg.py
+-rw-r--r--   0        0        0     2377 2023-05-29 02:03:29.081206 tensoul-0.1.4/tensoul/constants.py
+-rw-r--r--   0        0        0     7056 2023-05-25 08:27:21.930832 tensoul-0.1.4/tensoul/downloader.py
+-rw-r--r--   0        0        0    10283 2023-08-08 14:04:36.617461 tensoul-0.1.4/tensoul/model.py
+-rw-r--r--   0        0        0    14218 2023-05-29 01:57:19.665195 tensoul-0.1.4/tensoul/parser.py
+-rw-r--r--   0        0        0      452 2023-05-25 04:10:00.171590 tensoul-0.1.4/tensoul/utils.py
+-rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 tensoul-0.1.4/PKG-INFO
```

### Comparing `tensoul-0.1.3/README.md` & `tensoul-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.3/tensoul/cfg.json` & `tensoul-0.1.4/tensoul/cfg.json`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.3/tensoul/constants.py` & `tensoul-0.1.4/tensoul/constants.py`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.3/tensoul/downloader.py` & `tensoul-0.1.4/tensoul/downloader.py`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.3/tensoul/model.py` & `tensoul-0.1.4/tensoul/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,21 +225,22 @@
     tsumo_oya: int = 0
     oya: bool = False
 
     @property
     def level(self) -> Optional[AgariPointLevel]:
         judgement = 0
         if self.ron == 0:
+            # 自摸
             if self.oya:
-                judgement = (self.tsumo * 9) >> 2
+                judgement = (self.tsumo * 3) // 1.5
             else:
                 judgement = self.tsumo * 2 + self.tsumo_oya
         else:
             if self.oya:
-                judgement = (self.ron * 3) >> 2
+                judgement = self.ron // 1.5
             else:
                 judgement = self.ron
 
         if judgement >= 32000:
             return AgariPointLevel.yakuman
         elif judgement >= 24000:
             return AgariPointLevel.sanbaiman
```

### Comparing `tensoul-0.1.3/tensoul/parser.py` & `tensoul-0.1.4/tensoul/parser.py`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.3/PKG-INFO` & `tensoul-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensoul
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

