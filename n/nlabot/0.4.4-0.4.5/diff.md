# Comparing `tmp/nlabot-0.4.4-py3-none-any.whl.zip` & `tmp/nlabot-0.4.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10788 bytes, number of entries: 8
--rwxrwxrwx  2.0 unx    45146 b- defN 23-Aug-02 10:04 nlaftn/__init__.py
--rwxrwxrwx  2.0 unx       10 b- defN 23-Aug-02 10:04 nlabot-0.4.4.dist-info/DESCRIPTION.rst
--rwxrwxrwx  2.0 unx       47 b- defN 23-Aug-02 10:04 nlabot-0.4.4.dist-info/dependency_links.txt
--rwxrwxrwx  2.0 unx      619 b- defN 23-Aug-02 10:04 nlabot-0.4.4.dist-info/metadata.json
--rwxrwxrwx  2.0 unx        7 b- defN 23-Aug-02 10:04 nlabot-0.4.4.dist-info/top_level.txt
--rwxrwxrwx  2.0 unx       92 b- defN 23-Aug-02 10:04 nlabot-0.4.4.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      531 b- defN 23-Aug-02 10:04 nlabot-0.4.4.dist-info/METADATA
--rwxrwxrwx  2.0 unx      659 b- defN 23-Aug-02 10:04 nlabot-0.4.4.dist-info/RECORD
-8 files, 47111 bytes uncompressed, 9640 bytes compressed:  79.5%
+Zip file size: 10919 bytes, number of entries: 8
+-rwxrwxrwx  2.0 unx    46176 b- defN 23-Aug-08 14:58 nlaftn/__init__.py
+-rwxrwxrwx  2.0 unx       10 b- defN 23-Aug-08 14:59 nlabot-0.4.5.dist-info/DESCRIPTION.rst
+-rwxrwxrwx  2.0 unx       47 b- defN 23-Aug-08 14:59 nlabot-0.4.5.dist-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx      619 b- defN 23-Aug-08 14:59 nlabot-0.4.5.dist-info/metadata.json
+-rwxrwxrwx  2.0 unx        7 b- defN 23-Aug-08 14:59 nlabot-0.4.5.dist-info/top_level.txt
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Aug-08 14:59 nlabot-0.4.5.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      531 b- defN 23-Aug-08 14:59 nlabot-0.4.5.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      659 b- defN 23-Aug-08 14:59 nlabot-0.4.5.dist-info/RECORD
+8 files, 48141 bytes uncompressed, 9771 bytes compressed:  79.7%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: nlaftn/__init__.py
 Comment: 
 
-Filename: nlabot-0.4.4.dist-info/DESCRIPTION.rst
+Filename: nlabot-0.4.5.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: nlabot-0.4.4.dist-info/dependency_links.txt
+Filename: nlabot-0.4.5.dist-info/dependency_links.txt
 Comment: 
 
-Filename: nlabot-0.4.4.dist-info/metadata.json
+Filename: nlabot-0.4.5.dist-info/metadata.json
 Comment: 
 
-Filename: nlabot-0.4.4.dist-info/top_level.txt
+Filename: nlabot-0.4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: nlabot-0.4.4.dist-info/WHEEL
+Filename: nlabot-0.4.5.dist-info/WHEEL
 Comment: 
 
-Filename: nlabot-0.4.4.dist-info/METADATA
+Filename: nlabot-0.4.5.dist-info/METADATA
 Comment: 
 
-Filename: nlabot-0.4.4.dist-info/RECORD
+Filename: nlabot-0.4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nlaftn/__init__.py

```diff
@@ -1019,8 +1019,36 @@
 
         if self.friends in friend.display_name:
             name = friend.display_name
             if any(word in name for word in self.ban_player):
                 try:
                     await friend.remove()
                     print(f' Friend {friend.display_name} Removed Corectly')
-                except: pass
+                except: pass
+
+
+    async def verify(self):
+        try:
+        global code
+          
+        if len(self.friends) >= 0 and len(self.friends) <= 200:
+          await self.set_presence('💔 {party_size}/16 use code 667')
+          await asyncio.sleep(3)
+          await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
+
+        elif len(self.friends) >= 201 and len(self.friends) <= 600:
+          await self.set_presence('🧡 {party_size}/16 use code 667')
+          await asyncio.sleep(3)
+          await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
+
+        elif len(self.friends) >= 601 and len(self.friends) <= 1100:
+          await self.set_presence('💚 {party_size}/16 use code 667')
+          await asyncio.sleep(3)
+          await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
+
+        else:
+          await self.set_presence('💚 {party_size}/16 use code 667')
+          await asyncio.sleep(3)
+          await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
+          
+      except:
+        pass
```

## Comparing `nlabot-0.4.4.dist-info/metadata.json` & `nlabot-0.4.5.dist-info/metadata.json`

 * *Files 2% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'0.4.5'"}*

```diff
@@ -34,9 +34,9 @@
                 "crayons",
                 "fortnitepy (==3.6.7)",
                 "sanic (==21.6.2)"
             ]
         }
     ],
     "summary": "Lobby bot.",
-    "version": "0.4.4"
+    "version": "0.4.5"
 }
```

## Comparing `nlabot-0.4.4.dist-info/METADATA` & `nlabot-0.4.5.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: nlabot
-Version: 0.4.4
+Version: 0.4.5
 Summary: Lobby bot.
 Home-page: https://www.youtube.com/
 Author: Aeroz
 Author-email: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `nlabot-0.4.4.dist-info/RECORD` & `nlabot-0.4.5.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-nlabot-0.4.4.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
-nlabot-0.4.4.dist-info/METADATA,sha256=r2Ki1eYrM3MZ7n9rDYVsXlKzGXHJl84cSDwSlFQCPMg,531
-nlabot-0.4.4.dist-info/RECORD,,
-nlabot-0.4.4.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
-nlabot-0.4.4.dist-info/dependency_links.txt,sha256=w-iWPDMAaFhNNlD27qG0wZlgCL7bmLrdykt1CAjMpg4,47
-nlabot-0.4.4.dist-info/metadata.json,sha256=qi73f4XnylEDUV2Z7NQLkLKk9Xkku157Ii7fxCKMsE0,619
-nlabot-0.4.4.dist-info/top_level.txt,sha256=Hf6V-zsLXka13-6RurPoKaSDrHpVgxjB9QZCqY0kBo0,7
-nlaftn/__init__.py,sha256=mzHLLPJD1D0w7v3A0XKPKEuVstCLBeYAXrX6w-rXMtg,45146
+nlabot-0.4.5.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
+nlabot-0.4.5.dist-info/METADATA,sha256=BYBOxZq75OtvywTPpbDBySHZUXBqnlqz3YNqvo2U9A8,531
+nlabot-0.4.5.dist-info/RECORD,,
+nlabot-0.4.5.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
+nlabot-0.4.5.dist-info/dependency_links.txt,sha256=w-iWPDMAaFhNNlD27qG0wZlgCL7bmLrdykt1CAjMpg4,47
+nlabot-0.4.5.dist-info/metadata.json,sha256=ZXMzp9RMdFlXzkNrRj652QCCCVudaz7DuyXXiJ-ma88,619
+nlabot-0.4.5.dist-info/top_level.txt,sha256=Hf6V-zsLXka13-6RurPoKaSDrHpVgxjB9QZCqY0kBo0,7
+nlaftn/__init__.py,sha256=jd_8WsXscA5jy3ju6Wca7xxf-L38OLKCErHNpd0j_AM,46176
```

