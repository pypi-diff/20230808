# Comparing `tmp/bs_admin_utils-1.1.5-py3-none-any.whl.zip` & `tmp/bs_admin_utils-1.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 209359 bytes, number of entries: 14
+Zip file size: 209365 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx       13 b- defN 23-Apr-07 03:39 bs_admin_utils/__init__.py
 -rw-rw-r--  2.0 unx     4090 b- defN 23-Jun-21 08:15 bs_admin_utils/api.py
 -rw-rw-r--  2.0 unx      636 b- defN 23-Jul-20 10:44 bs_admin_utils/decorators.py
 -rw-rw-r--  2.0 unx     1098 b- defN 23-Jun-17 08:33 bs_admin_utils/model.py
 -rw-rw-r--  2.0 unx     2439 b- defN 23-Jun-14 10:58 bs_admin_utils/vercode.py
--rw-rw-r--  2.0 unx     2926 b- defN 23-Jul-25 02:51 bs_admin_utils/websocket.py
+-rw-rw-r--  2.0 unx     2850 b- defN 23-Aug-08 05:37 bs_admin_utils/websocket.py
 -rwxr-xr-x  2.0 unx   367112 b- defN 23-Apr-07 03:52 bs_admin_utils/static/arial.ttf
 -rwxr-xr-x  2.0 unx     6248 b- defN 23-Jun-14 10:45 bs_admin_utils/static/nstc.ttf
--rwxr-xr-x  2.0 unx     1067 b- defN 23-Jul-25 02:52 bs_admin_utils-1.1.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx      380 b- defN 23-Jul-25 02:52 bs_admin_utils-1.1.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 02:52 bs_admin_utils-1.1.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       20 b- defN 23-Jul-25 02:52 bs_admin_utils-1.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-25 02:52 bs_admin_utils-1.1.5.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1179 b- defN 23-Jul-25 02:52 bs_admin_utils-1.1.5.dist-info/RECORD
-14 files, 387301 bytes uncompressed, 207385 bytes compressed:  46.5%
+-rwxr-xr-x  2.0 unx     1067 b- defN 23-Aug-08 05:40 bs_admin_utils-1.1.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      380 b- defN 23-Aug-08 05:40 bs_admin_utils-1.1.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-08 05:40 bs_admin_utils-1.1.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       20 b- defN 23-Aug-08 05:40 bs_admin_utils-1.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Aug-08 05:40 bs_admin_utils-1.1.6.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1179 b- defN 23-Aug-08 05:40 bs_admin_utils-1.1.6.dist-info/RECORD
+14 files, 387225 bytes uncompressed, 207391 bytes compressed:  46.4%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: bs_admin_utils/static/arial.ttf
 Comment: 
 
 Filename: bs_admin_utils/static/nstc.ttf
 Comment: 
 
-Filename: bs_admin_utils-1.1.5.dist-info/LICENSE
+Filename: bs_admin_utils-1.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: bs_admin_utils-1.1.5.dist-info/METADATA
+Filename: bs_admin_utils-1.1.6.dist-info/METADATA
 Comment: 
 
-Filename: bs_admin_utils-1.1.5.dist-info/WHEEL
+Filename: bs_admin_utils-1.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: bs_admin_utils-1.1.5.dist-info/top_level.txt
+Filename: bs_admin_utils-1.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: bs_admin_utils-1.1.5.dist-info/zip-safe
+Filename: bs_admin_utils-1.1.6.dist-info/zip-safe
 Comment: 
 
-Filename: bs_admin_utils-1.1.5.dist-info/RECORD
+Filename: bs_admin_utils-1.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bs_admin_utils/websocket.py

```diff
@@ -21,17 +21,15 @@
 
 class Websockets:
     def __init__(self):
         self.connections: dict[str, dict[str, WebsocketConnection]] = {}
         self.event_handlers: dict[str, Callable[..., Coroutine]] = {}
 
     def _add_connection(self, user_code: str, connection: WebsocketConnection):
-        if user_code not in self.connections:
-            self.connections[user_code] = {}
-        self.connections[user_code][connection.code] = connection
+        self.connections.setdefault(user_code, {})[connection.code] = connection
 
     def _del_connection(self, user_code: str, connection: WebsocketConnection):
         if user_code in self.connections:
             self.connections[user_code].pop(connection.code, None)
 
             if not len(self.connections[user_code]):
                 self.connections.pop(user_code, None)
```

## Comparing `bs_admin_utils-1.1.5.dist-info/LICENSE` & `bs_admin_utils-1.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bs_admin_utils-1.1.5.dist-info/RECORD` & `bs_admin_utils-1.1.6.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 bs_admin_utils/__init__.py,sha256=da1PTClDMl-IBkrSvq6JC1lnS-K_BASzCvxVhNxN5Ls,13
 bs_admin_utils/api.py,sha256=nQ15WdbjjKV8djnGZ7En3s6DctKit4ygpM_pHN84UrY,4090
 bs_admin_utils/decorators.py,sha256=H6x8ZU-f7ZrNngoyxANDhOyT9zwmeVRIonS089e1RGk,636
 bs_admin_utils/model.py,sha256=-b3qlE6tlobm6mq01j09DHY7Ig25sOfy5q9ogmZTdZU,1098
 bs_admin_utils/vercode.py,sha256=l08RRsQG_n4SzKNkwFBairOhqQ4nxrfpD1FVQm20Lhk,2439
-bs_admin_utils/websocket.py,sha256=AqBndTbw1nSaJL2dwIUqZirxvd3RRdPT_1AR8INZF48,2926
+bs_admin_utils/websocket.py,sha256=LIbuUr5lLAr4OmrxftvbYNz6RCe4M_tCj8Z_GNmz_ms,2850
 bs_admin_utils/static/arial.ttf,sha256=QTx4-RvTnhNPPAuyBLHVqQ8p35793I_SaVCheAWNXXQ,367112
 bs_admin_utils/static/nstc.ttf,sha256=2tSmFfCuO5olGT35eF2kq3QhyR0aiqRedv4WO4rpqlQ,6248
-bs_admin_utils-1.1.5.dist-info/LICENSE,sha256=qmE7pY48Ur85GJoQksvL5vuMovFb2P-4qcjHj6HF8Ag,1067
-bs_admin_utils-1.1.5.dist-info/METADATA,sha256=4DA3TcLgi9Qux8pXdzUMWK9gpqtXcnQR0NqyEh8jT24,380
-bs_admin_utils-1.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-bs_admin_utils-1.1.5.dist-info/top_level.txt,sha256=sUy6z6pEqYADWdTRh6stGJQfcgyhEiLBteEMm283pF8,20
-bs_admin_utils-1.1.5.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-bs_admin_utils-1.1.5.dist-info/RECORD,,
+bs_admin_utils-1.1.6.dist-info/LICENSE,sha256=qmE7pY48Ur85GJoQksvL5vuMovFb2P-4qcjHj6HF8Ag,1067
+bs_admin_utils-1.1.6.dist-info/METADATA,sha256=0rrGj6cSGZCV2VhAQIpLxugSQ41YqvFV38kQbl8zNpE,380
+bs_admin_utils-1.1.6.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+bs_admin_utils-1.1.6.dist-info/top_level.txt,sha256=sUy6z6pEqYADWdTRh6stGJQfcgyhEiLBteEMm283pF8,20
+bs_admin_utils-1.1.6.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+bs_admin_utils-1.1.6.dist-info/RECORD,,
```

