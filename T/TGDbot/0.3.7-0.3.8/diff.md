# Comparing `tmp/TGDbot-0.3.7-py3-none-any.whl.zip` & `tmp/TGDbot-0.3.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 20732 bytes, number of entries: 9
--rwxrwxrwx  2.0 unx    54820 b- defN 23-Aug-02 10:22 TGDbot/__init__.py
+Zip file size: 20730 bytes, number of entries: 9
+-rwxrwxrwx  2.0 unx    54820 b- defN 23-Aug-08 12:07 TGDbot/__init__.py
 -rwxrwxrwx  2.0 unx    44441 b- defN 23-Apr-12 06:25 schbot/__init__.py
--rwxrwxrwx  2.0 unx       10 b- defN 23-Aug-02 10:23 TGDbot-0.3.7.dist-info/DESCRIPTION.rst
--rwxrwxrwx  2.0 unx       47 b- defN 23-Aug-02 10:23 TGDbot-0.3.7.dist-info/dependency_links.txt
--rwxrwxrwx  2.0 unx      619 b- defN 23-Aug-02 10:23 TGDbot-0.3.7.dist-info/metadata.json
--rwxrwxrwx  2.0 unx        7 b- defN 23-Aug-02 10:23 TGDbot-0.3.7.dist-info/top_level.txt
--rwxrwxrwx  2.0 unx       92 b- defN 23-Aug-02 10:23 TGDbot-0.3.7.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      531 b- defN 23-Aug-02 10:23 TGDbot-0.3.7.dist-info/METADATA
--rwxrwxrwx  2.0 unx      736 b- defN 23-Aug-02 10:23 TGDbot-0.3.7.dist-info/RECORD
-9 files, 101303 bytes uncompressed, 19472 bytes compressed:  80.8%
+-rwxrwxrwx  2.0 unx       10 b- defN 23-Aug-08 12:08 TGDbot-0.3.8.dist-info/DESCRIPTION.rst
+-rwxrwxrwx  2.0 unx       47 b- defN 23-Aug-08 12:08 TGDbot-0.3.8.dist-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx      619 b- defN 23-Aug-08 12:08 TGDbot-0.3.8.dist-info/metadata.json
+-rwxrwxrwx  2.0 unx        7 b- defN 23-Aug-08 12:08 TGDbot-0.3.8.dist-info/top_level.txt
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Aug-08 12:08 TGDbot-0.3.8.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      531 b- defN 23-Aug-08 12:08 TGDbot-0.3.8.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      736 b- defN 23-Aug-08 12:08 TGDbot-0.3.8.dist-info/RECORD
+9 files, 101303 bytes uncompressed, 19470 bytes compressed:  80.8%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: TGDbot/__init__.py
 Comment: 
 
 Filename: schbot/__init__.py
 Comment: 
 
-Filename: TGDbot-0.3.7.dist-info/DESCRIPTION.rst
+Filename: TGDbot-0.3.8.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: TGDbot-0.3.7.dist-info/dependency_links.txt
+Filename: TGDbot-0.3.8.dist-info/dependency_links.txt
 Comment: 
 
-Filename: TGDbot-0.3.7.dist-info/metadata.json
+Filename: TGDbot-0.3.8.dist-info/metadata.json
 Comment: 
 
-Filename: TGDbot-0.3.7.dist-info/top_level.txt
+Filename: TGDbot-0.3.8.dist-info/top_level.txt
 Comment: 
 
-Filename: TGDbot-0.3.7.dist-info/WHEEL
+Filename: TGDbot-0.3.8.dist-info/WHEEL
 Comment: 
 
-Filename: TGDbot-0.3.7.dist-info/METADATA
+Filename: TGDbot-0.3.8.dist-info/METADATA
 Comment: 
 
-Filename: TGDbot-0.3.7.dist-info/RECORD
+Filename: TGDbot-0.3.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## TGDbot/__init__.py

```diff
@@ -247,15 +247,15 @@
         self.session = aiohttp.ClientSession()
 
         self.skin = "CID_028_Athena_Commando_F"
         self.backpack = "BID_138_Celestial"
         self.pickaxe = "Pickaxe_Lockjaw"
         self.banner = "otherbanner51"
         self.bn_color = "defaultcolor22"
-        self.level = 667
+        self.level = 100
         self.tier = 100
         
         self.sanic_app = sanic_app
         self.server = server
 
         self.rst = "F"
         self.vr = "0.0"
```

## Comparing `TGDbot-0.3.7.dist-info/metadata.json` & `TGDbot-0.3.8.dist-info/metadata.json`

 * *Files 24% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'0.3.8'"}*

```diff
@@ -34,9 +34,9 @@
                 "crayons",
                 "fortnitepy (==3.6.7)",
                 "sanic (==21.6.2)"
             ]
         }
     ],
     "summary": "Lobby bot.",
-    "version": "0.3.7"
+    "version": "0.3.8"
 }
```

## Comparing `TGDbot-0.3.7.dist-info/METADATA` & `TGDbot-0.3.8.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: TGDbot
-Version: 0.3.7
+Version: 0.3.8
 Summary: Lobby bot.
 Home-page: https://www.youtube.com/
 Author: Aeroz
 Author-email: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

