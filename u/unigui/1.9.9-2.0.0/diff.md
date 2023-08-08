# Comparing `tmp/unigui-1.9.9.tar.gz` & `tmp/unigui-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.9.9.tar", last modified: Thu Aug  3 18:47:43 2023, max compression
+gzip compressed data, was "dist/unigui-2.0.0.tar", last modified: Tue Aug  8 17:05:45 2023, max compression
```

## Comparing `unigui-1.9.9.tar` & `unigui-2.0.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-03 18:47:43.000000 unigui-1.9.9/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-03 18:47:43.000000 unigui-1.9.9/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)     5345 2023-07-31 07:12:00.000000 unigui-1.9.9/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     3531 2023-07-26 16:18:00.000000 unigui-1.9.9/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)     4181 2023-07-28 17:59:21.000000 unigui-1.9.9/unigui/tables.py
--rw-rw-r--   0 george    (1000) george    (1000)      128 2023-07-25 04:04:00.000000 unigui-1.9.9/unigui/__init__.py
--rw-rw-r--   0 george    (1000) george    (1000)     7796 2023-07-29 16:08:30.000000 unigui-1.9.9/unigui/autotest.py
--rw-r--r--   0 george    (1000) george    (1000)     2669 2023-07-31 07:45:36.000000 unigui-1.9.9/unigui/utils.py
--rw-rw-r--   0 george    (1000) george    (1000)     5573 2023-07-26 17:26:38.000000 unigui-1.9.9/unigui/reloader.py
--rw-rw-r--   0 george    (1000) george    (1000)     8755 2023-08-03 14:56:50.000000 unigui-1.9.9/unigui/users.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-03 18:47:43.000000 unigui-1.9.9/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-03 18:47:43.000000 unigui-1.9.9/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/css/vendor.f747ec02.css
--rw-rw-r--   0 george    (1000) george    (1000)     2691 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/css/768.30396533.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-03 18:47:43.000000 unigui-1.9.9/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-03 18:47:43.000000 unigui-1.9.9/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-03 18:47:43.000000 unigui-1.9.9/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)    50573 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/js/768.89ad69c0.js
--rw-rw-r--   0 george    (1000) george    (1000)  1445576 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/js/vendor.8cb03aaa.js
--rw-rw-r--   0 george    (1000) george    (1000)     5923 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/js/app.c32942a4.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-08-03 18:41:39.000000 unigui-1.9.9/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.9.9/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      642 2023-08-03 18:47:28.000000 unigui-1.9.9/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    18773 2023-08-03 18:47:43.000000 unigui-1.9.9/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-08-03 18:47:43.000000 unigui-1.9.9/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    18468 2023-07-30 04:54:06.000000 unigui-1.9.9/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.9.9/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-03 18:47:43.000000 unigui-1.9.9/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       63 2023-08-03 18:47:42.000000 unigui-1.9.9/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-08-03 18:47:42.000000 unigui-1.9.9/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    18773 2023-08-03 18:47:42.000000 unigui-1.9.9/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.9.9/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1258 2023-08-03 18:47:42.000000 unigui-1.9.9/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-08-03 18:47:42.000000 unigui-1.9.9/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-08 17:05:45.000000 unigui-2.0.0/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-08 17:05:45.000000 unigui-2.0.0/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)     5345 2023-07-31 07:12:00.000000 unigui-2.0.0/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3531 2023-07-26 16:18:00.000000 unigui-2.0.0/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)     4181 2023-08-05 08:04:27.000000 unigui-2.0.0/unigui/tables.py
+-rw-rw-r--   0 george    (1000) george    (1000)      128 2023-07-25 04:04:00.000000 unigui-2.0.0/unigui/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)     7809 2023-08-08 14:39:14.000000 unigui-2.0.0/unigui/autotest.py
+-rw-r--r--   0 george    (1000) george    (1000)     2669 2023-07-31 07:45:36.000000 unigui-2.0.0/unigui/utils.py
+-rw-rw-r--   0 george    (1000) george    (1000)     5573 2023-07-26 17:26:38.000000 unigui-2.0.0/unigui/reloader.py
+-rw-rw-r--   0 george    (1000) george    (1000)     8755 2023-08-03 14:56:50.000000 unigui-2.0.0/unigui/users.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-08 17:05:45.000000 unigui-2.0.0/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-08 17:05:45.000000 unigui-2.0.0/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/css/vendor.f747ec02.css
+-rw-rw-r--   0 george    (1000) george    (1000)     2691 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/css/737.bedc790c.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-08 17:05:45.000000 unigui-2.0.0/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-08 17:05:45.000000 unigui-2.0.0/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-08 17:05:45.000000 unigui-2.0.0/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)    51662 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/js/737.229a004a.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5923 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/js/app.39deedc9.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1444614 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/js/vendor.bc1bae42.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-08-08 16:51:58.000000 unigui-2.0.0/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-2.0.0/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      651 2023-08-08 16:58:52.000000 unigui-2.0.0/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    18195 2023-08-08 17:05:45.000000 unigui-2.0.0/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-08-08 17:05:45.000000 unigui-2.0.0/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    17890 2023-08-08 16:59:14.000000 unigui-2.0.0/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-2.0.0/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-08 17:05:45.000000 unigui-2.0.0/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       70 2023-08-08 17:05:45.000000 unigui-2.0.0/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-08-08 17:05:45.000000 unigui-2.0.0/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    18195 2023-08-08 17:05:45.000000 unigui-2.0.0/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-2.0.0/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1258 2023-08-08 17:05:45.000000 unigui-2.0.0/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-08-08 17:05:45.000000 unigui-2.0.0/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.9.9/unigui/guielements.py` & `unigui-2.0.0/unigui/guielements.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/server.py` & `unigui-2.0.0/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/tables.py` & `unigui-2.0.0/unigui/tables.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/autotest.py` & `unigui-2.0.0/unigui/autotest.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,26 +179,26 @@
     errors = []
     for module in user.screens:
         errors += check_screen(module)
     if errors:
         errors.insert(0, f'\n!!----Unigui detected errors in screens:')
         print('\n'.join(errors), '\n')
     elif user.screens:
-        print(f'\n----Screens definitions are correct. ')
+        print(f'\n----The screen definitions are correct.-----\n')
         
     files = config.autotest
     ok = True
     process = False
     if os.path.exists(testdir):
         for file in os.listdir(testdir):
             if not os.path.isdir(file) and (files == '*' or file in files):
                 process = True
                 if not test(file,user):
                     ok = False
     if process and ok:
-        print('-----Autotests successfully passed.-----')
+        print('\n-----Autotests successfully passed.-----\n')
     User.last_user = None
     User.toolbar.append(button)
```

### Comparing `unigui-1.9.9/unigui/utils.py` & `unigui-2.0.0/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/reloader.py` & `unigui-2.0.0/unigui/reloader.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/users.py` & `unigui-2.0.0/unigui/users.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/favicon.ico` & `unigui-2.0.0/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/css/vendor.f747ec02.css` & `unigui-2.0.0/unigui/web/css/vendor.f747ec02.css`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/icons/favicon-96x96.png` & `unigui-2.0.0/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/icons/favicon-16x16.png` & `unigui-2.0.0/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/icons/favicon-32x32.png` & `unigui-2.0.0/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/icons/favicon-128x128.png` & `unigui-2.0.0/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `unigui-2.0.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-2.0.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-2.0.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-2.0.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-2.0.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-2.0.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-2.0.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-2.0.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/js/430.591e9a73.js` & `unigui-2.0.0/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/js/768.89ad69c0.js` & `unigui-2.0.0/unigui/web/js/737.229a004a.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [768], {
-        9768: (e, t, a) => {
+    [737], {
+        4737: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => sa
             });
             var s = a(3673),
                 l = a(2323);
             const i = (0, s._)("div", {
                     class: "q-pa-md"
@@ -17,31 +17,31 @@
             function o(e, t, a, o, d, r) {
                 const c = (0, s.up)("q-item-label"),
                     h = (0, s.up)("element"),
                     u = (0, s.up)("q-tab"),
                     p = (0, s.up)("q-tabs"),
                     m = (0, s.up)("q-space"),
                     g = (0, s.up)("q-tooltip"),
-                    f = (0, s.up)("q-btn"),
-                    y = (0, s.up)("q-toolbar"),
+                    y = (0, s.up)("q-btn"),
+                    f = (0, s.up)("q-toolbar"),
                     w = (0, s.up)("q-header"),
                     b = (0, s.up)("zone"),
                     k = (0, s.up)("q-page"),
                     v = (0, s.up)("q-page-container"),
                     x = (0, s.up)("q-layout");
                 return (0, s.wg)(), (0, s.j4)(x, {
                     view: "lHh Lpr lFf"
                 }, {
                     default: (0, s.w5)((() => [(0, s.Wm)(w, {
                         elevated: "",
                         class: (0, l.C_)({
                             "bg-deep-purple-9": e.Dark.isActive
                         })
                     }, {
-                        default: (0, s.w5)((() => [(0, s.Wm)(y, null, {
+                        default: (0, s.w5)((() => [(0, s.Wm)(f, null, {
                             default: (0, s.w5)((() => [(0, s.Wm)(c, {
                                 class: "text-h5"
                             }, {
                                 default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.screen.header ? e.screen.header : ""), 1)])),
                                 _: 1
                             }), i, ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.left_toolbar, (t => ((0, s.wg)(), (0, s.j4)(h, {
                                 class: (0, l.C_)(["q-ma-xs", {
@@ -81,15 +81,15 @@
                             }, 8, ["modelValue"]), (0, s.Wm)(m), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.right_toolbar, (t => ((0, s.wg)(), (0, s.j4)(h, {
                                 class: (0, l.C_)(["q-ma-xs", {
                                     "bg-blue-grey-7": e.Dark.isActive,
                                     "bg-blue-5": !e.Dark.isActive
                                 }]),
                                 data: t,
                                 pdata: e.tooldata
-                            }, null, 8, ["class", "data", "pdata"])))), 256)), (0, s.Wm)(f, {
+                            }, null, 8, ["class", "data", "pdata"])))), 256)), (0, s.Wm)(y, {
                                 class: (0, l.C_)(["q-ma-xs", {
                                     "bg-blue-grey-9": e.Dark.isActive
                                 }]),
                                 dense: "",
                                 round: "",
                                 icon: e.Dark.isActive ? "light_mode" : "dark_mode",
                                 onClick: e.switchTheme
@@ -155,23 +155,23 @@
             var r = a(698),
                 c = a(8603);
             let h = null,
                 u = {};
             var p;
             const m = !1;
             let g = m;
-            const f = ["graph", "textarea", "chart", "block"];
-            const y = window.location.host,
-                w = `${window.location.protocol}//${y}`;
+            const y = ["graph", "textarea", "chart", "block"];
+            const f = window.location.host,
+                w = `${window.location.protocol}//${f}`;
             let b = {},
                 k = {},
                 v = {};
 
             function C(e) {
-                p = new WebSocket(m ? "ws://localhost:8000/ws" : `ws://${y}/ws`), p.onopen = () => e.statusConnect = !0, p.onmessage = t => {
+                p = new WebSocket(m ? "ws://localhost:8000/ws" : `ws://${f}/ws`), p.onopen = () => e.statusConnect = !0, p.onmessage = t => {
                     g && console.log("incoming message", t.data), h.designCycle = 0, e.processMessage(JSON.parse(t.data))
                 }, p.onerror = t => e.error(t), p.onclose = t => {
                     t.wasClean ? e.info("Connection was finished by the server.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, g && console.info("close code : " + t.code + " reason: " + t.reason)
                 }, h = e
             }
 
             function _(e) {
@@ -231,15 +231,15 @@
                 for (let s of e) s instanceof Array ? t.push(s) : t.push([s]);
                 let a = t.shift();
                 return t.reduce(((e, t) => e.flatMap((e => t.map((t => e instanceof Array ? [...e, t] : [e, t]))))), a)
             }
 
             function E(e = !1) {
                 for (let t of Object.values(k))
-                    if (t.expanding && (!e || f.includes(t.type))) {
+                    if (t.expanding && (!e || y.includes(t.type))) {
                         t.has_recalc = !0;
                         let e = t.$el;
                         if (e.getBoundingClientRect) {
                             let e = t.$el.getBoundingClientRect();
                             window.innerHeight < e.top + e.height && (t.styleSize = null)
                         }
                     }(0, s.Y3)((() => {
@@ -277,19 +277,19 @@
                             }
                         } else if (e.name == t.data.name) {
                         d = t;
                         break
                     }
                     let p = n;
                     p /= o;
-                    let m = e || f.includes(t.type) || t.has_recalc,
+                    let m = e || y.includes(t.type) || t.has_recalc,
                         g = m && !t.only_fixed_elems ? `width:${Math.ceil(c.clientWidth+p)}px` : "",
-                        y = s.startsWith("_scroll@") ? r.inner.clientHeight : c.clientHeight;
-                    y < 0 && (y = 20);
-                    let w = `height: ${y+l}px; ${g}`;
+                        f = s.startsWith("_scroll@") ? r.inner.clientHeight : c.clientHeight;
+                    f < 0 && (f = 20);
+                    let w = `height: ${f+l}px; ${g}`;
                     w != t.styleSize && (t.styleSize = w), t.has_recalc = !1
                 }
             }
 
             function O(e) {
                 const t = h.screen.blocks;
                 let a = window.innerHeight;
@@ -390,15 +390,15 @@
                     let t = Array.isArray(d) ? d[d.length - 1] : d,
                         a = b[t.name].$el.getBoundingClientRect().right;
                     t = Array.isArray(d) ? d[0] : d;
                     let l = b[t.name].$el.getBoundingClientRect().left,
                         i = s - a + l - 10;
                     const r = [];
                     for (let [s, n] of Object.entries(k))
-                        if (n.expanding_width && (n.fullname.startsWith("_scroll@") || e || f.includes(n.type))) {
+                        if (n.expanding_width && (n.fullname.startsWith("_scroll@") || e || y.includes(n.type))) {
                             let e = s.split("@")[1];
                             if (d.find((t => t.name == e))) {
                                 let e = !0,
                                     t = n.geom().left;
                                 for (let [a, s] of r.entries())
                                     if (s !== n && s.geom().left == t) {
                                         s.geom().scrollWidth < n.geom().scrollWidth ? (r[a] = n, o.set(s.fullname, n.fullname)) : o.set(n.fullname, s.fullname), e = !1;
@@ -587,74 +587,76 @@
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"]))], 8, se)))), 256))])),
                     _: 1
                 }, 8, ["style"])
             }
             var ne = a(8880);
-            const oe = e => ((0, s.dD)("data-v-d4b5cc5e"), e = e(), (0, s.Cn)(), e),
+            const oe = e => ((0, s.dD)("data-v-905c4cee"), e = e(), (0, s.Cn)(), e),
                 de = {
                     key: 4,
                     class: "{'bg-blue-grey-9': Dark.isActive}"
                 },
-                re = ["src"],
-                ce = {
+                re = {
+                    key: 10
+                },
+                ce = ["src"],
+                he = {
                     key: 18,
                     class: "web-camera-container"
                 },
-                he = {
+                ue = {
                     class: "camera-button"
                 },
-                ue = {
+                pe = {
                     key: 0
                 },
-                pe = {
+                me = {
                     key: 1
                 },
-                me = {
+                ge = {
                     class: "camera-loading"
                 },
-                ge = oe((() => (0, s._)("ul", {
+                ye = oe((() => (0, s._)("ul", {
                     class: "loader-circle"
                 }, [(0, s._)("li"), (0, s._)("li"), (0, s._)("li")], -1))),
-                fe = [ge],
-                ye = ["height"],
+                fe = [ye],
                 we = ["height"],
-                be = {
+                be = ["height"],
+                ke = {
                     key: 1,
                     class: "camera-shoot"
                 },
-                ke = oe((() => (0, s._)("img", {
+                ve = oe((() => (0, s._)("img", {
                     src: "https://img.icons8.com/material-outlined/50/000000/camera--v2.png"
                 }, null, -1))),
-                ve = [ke],
-                xe = {
+                xe = [ve],
+                Ce = {
                     key: 2,
                     class: "camera-download"
                 };
 
-            function Ce(e, t, a, i, n, o) {
+            function _e(e, t, a, i, n, o) {
                 const d = (0, s.up)("q-icon"),
                     r = (0, s.up)("q-img"),
-                    c = (0, s.up)("q-badge"),
-                    h = (0, s.up)("q-select"),
-                    u = (0, s.up)("q-checkbox"),
-                    p = (0, s.up)("q-toggle"),
-                    m = (0, s.up)("q-btn"),
-                    g = (0, s.up)("q-btn-toggle"),
-                    f = (0, s.up)("utable"),
+                    c = (0, s.up)("q-select"),
+                    h = (0, s.up)("q-checkbox"),
+                    u = (0, s.up)("q-toggle"),
+                    p = (0, s.up)("q-btn"),
+                    m = (0, s.up)("q-btn-toggle"),
+                    g = (0, s.up)("utable"),
                     y = (0, s.up)("linechart"),
-                    w = (0, s.up)("q-input"),
-                    b = (0, s.up)("q-tree"),
-                    k = (0, s.up)("q-scroll-area"),
-                    v = (0, s.up)("q-separator"),
-                    x = (0, s.up)("q-uploader"),
-                    C = (0, s.up)("cgraph"),
-                    _ = (0, s.up)("q-tooltip"),
-                    q = (0, s.up)("q-spinner-ios");
+                    f = (0, s.up)("q-input"),
+                    w = (0, s.up)("q-tree"),
+                    b = (0, s.up)("q-scroll-area"),
+                    k = (0, s.up)("q-separator"),
+                    v = (0, s.up)("q-uploader"),
+                    x = (0, s.up)("cgraph"),
+                    C = (0, s.up)("q-tooltip"),
+                    _ = (0, s.up)("q-spinner-ios");
                 return "image" == e.type ? ((0, s.wg)(), (0, s.j4)(r, {
                     key: 0,
                     src: e.data.url,
                     "spinner-color": "blue",
                     onClick: (0, ne.iM)(e.switchValue, ["stop"]),
                     fit: "cover",
                     style: (0, l.j5)(e.elemSize)
@@ -672,201 +674,211 @@
                         style: {
                             "font-size": "2em",
                             top: "8px",
                             left: "8px"
                         }
                     })) : (0, s.kq)("", !0)])),
                     _: 1
-                }, 8, ["src", "onClick", "style"])) : "select" == e.type ? ((0, s.wg)(), (0, s.j4)(h, {
+                }, 8, ["src", "onClick", "style"])) : "select" == e.type ? ((0, s.wg)(), (0, s.j4)(c, {
                     key: 1,
                     "transition-show": "flip-up",
+                    readonly: 0 == e.data.edit,
                     "transition-hide": "flip-down",
                     dense: "",
                     modelValue: e.value,
                     "onUpdate:modelValue": t[1] || (t[1] = t => e.value = t),
                     options: e.data.options
                 }, (0, s.Nv)({
                     _: 2
                 }, [e.showname ? {
                     name: "prepend",
-                    fn: (0, s.w5)((() => [(0, s.Wm)(c, {
-                        color: "secondary"
-                    }, {
-                        default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.name), 1)])),
-                        _: 1
-                    })])),
+                    fn: (0, s.w5)((() => [(0, s._)("p", {
+                        class: (0, l.C_)(["text-subtitle1 q-ma-sm", {
+                            white: e.Dark.isActive,
+                            black: !e.Dark.isActive
+                        }])
+                    }, (0, l.zw)(e.name), 3)])),
                     key: "0"
-                } : void 0]), 1032, ["modelValue", "options"])) : "check" == e.type ? ((0, s.wg)(), (0, s.j4)(u, {
+                } : void 0]), 1032, ["readonly", "modelValue", "options"])) : "check" == e.type ? ((0, s.wg)(), (0, s.j4)(h, {
                     key: 2,
                     "left-label": "",
+                    disable: 0 == e.data.edit,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[2] || (t[2] = t => e.value = t),
                     label: e.nameLabel,
                     "checked-icon": "task_alt",
                     "unchecked-icon": "highlight_off"
-                }, null, 8, ["modelValue", "label"])) : "switch" == e.type ? ((0, s.wg)(), (0, s.j4)(p, {
+                }, null, 8, ["disable", "modelValue", "label"])) : "switch" == e.type ? ((0, s.wg)(), (0, s.j4)(u, {
                     key: 3,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[3] || (t[3] = t => e.value = t),
+                    disable: 0 == e.data.edit,
                     color: "primary",
                     label: e.nameLabel,
                     "left-label": ""
-                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, s.wg)(), (0, s.iD)("div", de, [e.showname ? ((0, s.wg)(), (0, s.j4)(m, {
+                }, null, 8, ["modelValue", "disable", "label"])) : "radio" == e.type ? ((0, s.wg)(), (0, s.iD)("div", de, [e.showname ? ((0, s.wg)(), (0, s.j4)(p, {
                     key: 0,
                     ripple: !1,
                     color: "indigo-10",
                     disable: "",
                     label: e.name,
                     "no-caps": ""
-                }, null, 8, ["label"])) : (0, s.kq)("", !0), (0, s.Wm)(g, {
+                }, null, 8, ["label"])) : (0, s.kq)("", !0), (0, s.Wm)(m, {
                     modelValue: e.value,
                     "onUpdate:modelValue": t[4] || (t[4] = t => e.value = t),
+                    readonly: 0 == e.data.edit,
                     class: (0, l.C_)({
                         "bg-blue-grey-9": e.Dark.isActive
                     }),
                     "no-caps": "",
                     options: e.data.options.map((e => ({
                         label: e,
                         value: e
                     })))
-                }, null, 8, ["modelValue", "class", "options"])])) : "table" == e.type ? ((0, s.wg)(), (0, s.j4)(f, {
+                }, null, 8, ["modelValue", "readonly", "class", "options"])])) : "table" == e.type ? ((0, s.wg)(), (0, s.j4)(g, {
                     key: 5,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.styleSize
                 }, null, 8, ["data", "pdata", "styleSize"])) : "chart" == e.type ? ((0, s.wg)(), (0, s.j4)(y, {
                     key: 6,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.styleSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "edit" == e.type ? ((0, s.wg)(), (0, s.j4)(w, {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "edit" == e.type ? ((0, s.wg)(), (0, s.j4)(f, {
                     key: 7,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[5] || (t[5] = t => e.value = t),
                     label: e.name,
                     ref: "inputRef",
                     autogrow: e.data.autogrow,
                     dense: "",
                     onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"]),
-                    readonly: !1 === e.data.edit
-                }, null, 8, ["modelValue", "label", "autogrow", "onKeyup", "readonly"])) : "number" == e.type ? ((0, s.wg)(), (0, s.j4)(w, {
+                    readonly: 0 == e.data.edit
+                }, null, 8, ["modelValue", "label", "autogrow", "onKeyup", "readonly"])) : "number" == e.type ? ((0, s.wg)(), (0, s.j4)(f, {
                     key: 8,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[6] || (t[6] = t => e.value = t),
                     modelModifiers: {
                         number: !0
                     },
                     label: e.name,
                     ref: "inputRef",
                     dense: "",
                     onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"]),
                     type: "number",
-                    readonly: !1 === e.data.edit
-                }, null, 8, ["modelValue", "label", "onKeyup", "readonly"])) : "autoedit" == e.type ? ((0, s.wg)(), (0, s.j4)(h, {
+                    readonly: 0 == e.data.edit
+                }, null, 8, ["modelValue", "label", "onKeyup", "readonly"])) : "autoedit" == e.type ? ((0, s.wg)(), (0, s.j4)(c, {
                     key: 9,
                     dense: "",
+                    readonly: 0 == e.data.edit,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[7] || (t[7] = t => e.value = t),
                     "use-input": "",
                     "hide-selected": "",
                     borderless: "",
                     outlined: "",
                     "hide-bottom-space": "",
                     "fill-input": "",
                     "input-debounce": "0",
                     options: e.options,
                     onFilter: e.complete,
                     label: e.name,
                     onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"])
-                }, null, 8, ["modelValue", "options", "onFilter", "label", "onKeyup"])) : "tree" == e.type || "list" == e.type ? ((0, s.wg)(), (0, s.j4)(k, {
-                    key: 10,
+                }, null, 8, ["readonly", "modelValue", "options", "onFilter", "label", "onKeyup"])) : "tree" == e.type || "list" == e.type ? ((0, s.wg)(), (0, s.iD)("div", re, [e.showname ? ((0, s.wg)(), (0, s.iD)("p", {
+                    key: 0,
+                    class: (0, l.C_)(["text-subtitle1 q-ma-sm text-grey-7", {
+                        "text-white": e.Dark.isActive,
+                        "text-indigo-10": !e.Dark.isActive
+                    }])
+                }, (0, l.zw)(e.name), 3)) : (0, s.kq)("", !0), (0, s.Wm)(b, {
                     style: (0, l.j5)(e.styleSize),
                     "thumb-style": e.thumbStyle,
                     "bar-style": e.barStyle
                 }, {
-                    default: (0, s.w5)((() => [(0, s.Wm)(b, {
+                    default: (0, s.w5)((() => [(0, s.Wm)(w, {
                         nodes: e.treeNodes,
-                        "selected-color": e.Dark.isActive ? "blue-3" : "indigo",
+                        "selected-color": e.Dark.isActive ? "blue-3" : "blue-9",
                         dense: e.data.dense,
                         selected: e.value,
                         "onUpdate:selected": t[8] || (t[8] = t => e.value = t),
                         expanded: e.expandedKeys,
                         "onUpdate:expanded": t[9] || (t[9] = t => e.expandedKeys = t),
                         "node-key": "label",
                         "default-expand-all": ""
                     }, null, 8, ["nodes", "selected-color", "dense", "selected", "expanded"])])),
                     _: 1
-                }, 8, ["style", "thumb-style", "bar-style"])) : "textarea" == e.type ? (0, s.wy)(((0, s.wg)(), (0, s.iD)("textarea", {
+                }, 8, ["style", "thumb-style", "bar-style"])])) : "textarea" == e.type ? (0, s.wy)(((0, s.wg)(), (0, s.iD)("textarea", {
                     key: 11,
                     class: (0, l.C_)(["textarea", {
                         "bg-grey-10": e.Dark.isActive,
                         "text-white": e.Dark.isActive
                     }]),
                     "onUpdate:modelValue": t[10] || (t[10] = t => e.value = t),
                     filled: "",
                     type: "textarea",
                     style: (0, l.j5)(e.elemSize)
                 }, null, 6)), [
                     [ne.nr, e.value]
-                ]) : "line" == e.type ? ((0, s.wg)(), (0, s.j4)(v, {
+                ]) : "line" == e.type ? ((0, s.wg)(), (0, s.j4)(k, {
                     key: 12,
                     color: "green"
                 })) : "text" == e.type ? ((0, s.wg)(), (0, s.iD)("p", {
                     key: 13,
                     class: (0, l.C_)(["q-ma-sm", {
                         white: e.Dark.isActive,
                         black: !e.Dark.isActive
                     }])
                 }, (0, l.zw)(e.value), 3)) : "video" == e.type ? ((0, s.wg)(), (0, s.iD)("video", {
                     key: e.fullname,
                     controls: ""
                 }, [(0, s._)("source", {
                     src: e.data.url,
                     type: "video/mp4"
-                }, null, 8, re)])) : "uploader" == e.type ? ((0, s.wg)(), (0, s.j4)(x, {
+                }, null, 8, ce)])) : "uploader" == e.type ? ((0, s.wg)(), (0, s.j4)(v, {
                     key: 15,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: e.host_path,
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
                     style: (0, l.j5)(e.elemSize),
                     ref: "uploaderRef",
                     flat: "",
                     class: (0, l.C_)({
                         "bg-grey-9": e.Dark.isActive
                     })
-                }, null, 8, ["label", "url", "onUploaded", "onAdded", "style", "class"])) : "image_uploader" == e.type ? ((0, s.wg)(), (0, s.j4)(x, {
+                }, null, 8, ["label", "url", "onUploaded", "onAdded", "style", "class"])) : "image_uploader" == e.type ? ((0, s.wg)(), (0, s.j4)(v, {
                     key: 16,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: e.host_path,
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
                     ref: "uploaderRef",
                     flat: "",
                     class: (0, l.C_)({
                         "bg-grey-10": e.Dark.isActive
                     }),
                     color: e.Dark.isActive ? "purple-10" : "blue"
-                }, null, 8, ["label", "url", "onUploaded", "onAdded", "class", "color"])) : "graph" == e.type ? ((0, s.wg)(), (0, s.j4)(C, {
+                }, null, 8, ["label", "url", "onUploaded", "onAdded", "class", "color"])) : "graph" == e.type ? ((0, s.wg)(), (0, s.j4)(x, {
                     key: 17,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.elemSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, s.wg)(), (0, s.iD)("div", ce, [(0, s._)("div", he, [(0, s._)("button", {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, s.wg)(), (0, s.iD)("div", he, [(0, s._)("div", ue, [(0, s._)("button", {
                     class: (0, l.C_)(["button is-rounded", {
                         "is-primary": !e.isCameraOpen,
                         "is-danger": e.isCameraOpen
                     }]),
                     type: "button",
                     onClick: t[11] || (t[11] = (...t) => e.toggleCamera && e.toggleCamera(...t))
-                }, [e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("span", pe, "Close Camera")) : ((0, s.wg)(), (0, s.iD)("span", ue, "Open Camera"))], 2)]), (0, s.wy)((0, s._)("div", me, fe, 512), [
+                }, [e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("span", me, "Close Camera")) : ((0, s.wg)(), (0, s.iD)("span", pe, "Open Camera"))], 2)]), (0, s.wy)((0, s._)("div", ge, fe, 512), [
                     [ne.F8, e.isCameraOpen && e.isLoading]
                 ]), e.isCameraOpen ? (0, s.wy)(((0, s.wg)(), (0, s.iD)("div", {
                     key: 0,
                     class: (0, l.C_)(["camera-box", {
                         flash: e.isShotPhoto
                     }])
                 }, [(0, s._)("div", {
@@ -874,129 +886,132 @@
                         flash: e.isShotPhoto
                     }])
                 }, null, 2), (0, s.wy)((0, s._)("video", {
                     ref: "camera",
                     width: 450,
                     height: 337.5,
                     autoplay: ""
-                }, null, 8, ye), [
+                }, null, 8, we), [
                     [ne.F8, !e.isPhotoTaken]
                 ]), (0, s.wy)((0, s._)("canvas", {
                     id: "photoTaken",
                     ref: "canvas",
                     width: 450,
                     height: 337.5
-                }, null, 8, we), [
+                }, null, 8, be), [
                     [ne.F8, e.isPhotoTaken]
                 ])], 2)), [
                     [ne.F8, !e.isLoading]
-                ]) : (0, s.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, s.wg)(), (0, s.iD)("div", be, [(0, s._)("button", {
+                ]) : (0, s.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, s.wg)(), (0, s.iD)("div", ke, [(0, s._)("button", {
                     class: "button",
                     type: "button",
                     onClick: t[12] || (t[12] = (...t) => e.takePhoto && e.takePhoto(...t))
-                }, ve)])) : (0, s.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("div", xe, [(0, s.Wm)(m, {
+                }, xe)])) : (0, s.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("div", Ce, [(0, s.Wm)(p, {
                     onClick: e.downloadImage,
                     label: "Send"
-                }, null, 8, ["onClick"])])) : (0, s.kq)("", !0)])) : "" != e.showname ? ((0, s.wg)(), (0, s.j4)(m, {
+                }, null, 8, ["onClick"])])) : (0, s.kq)("", !0)])) : "" != e.showname ? ((0, s.wg)(), (0, s.j4)(p, {
                     key: 19,
                     "no-caps": "",
+                    disable: 0 == e.data.edit,
                     class: (0, l.C_)({
                         "bg-blue-grey-8": e.Dark.isActive
                     }),
                     label: e.name,
                     icon: e.data.icon,
                     onClick: e.sendValue
                 }, {
-                    default: (0, s.w5)((() => [e.data.tooltip ? ((0, s.wg)(), (0, s.j4)(_, {
+                    default: (0, s.w5)((() => [e.data.tooltip ? ((0, s.wg)(), (0, s.j4)(C, {
                         key: 0,
                         class: "text-body2"
                     }, {
                         default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, s.kq)("", !0)])),
                     _: 1
-                }, 8, ["class", "label", "icon", "onClick"])) : e.data.spinner ? ((0, s.wg)(), (0, s.j4)(m, {
+                }, 8, ["disable", "class", "label", "icon", "onClick"])) : e.data.spinner ? ((0, s.wg)(), (0, s.j4)(p, {
                     key: 21,
                     "no-caps": "",
                     dense: "",
+                    disable: 0 == e.data.edit,
                     round: "",
                     class: (0, l.C_)({
                         "bg-blue-grey-8": e.Dark.isActive
                     }),
                     onClick: e.sendValue
                 }, {
-                    default: (0, s.w5)((() => [(0, s.Wm)(q, {
+                    default: (0, s.w5)((() => [(0, s.Wm)(_, {
                         color: e.Dark.isActive ? "white" : "black"
-                    }, null, 8, ["color"]), e.data.tooltip ? ((0, s.wg)(), (0, s.j4)(_, {
+                    }, null, 8, ["color"]), e.data.tooltip ? ((0, s.wg)(), (0, s.j4)(C, {
                         key: 0,
                         class: "text-body2"
                     }, {
                         default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, s.kq)("", !0)])),
                     _: 1
-                }, 8, ["class", "onClick"])) : ((0, s.wg)(), (0, s.j4)(m, {
+                }, 8, ["disable", "class", "onClick"])) : ((0, s.wg)(), (0, s.j4)(p, {
                     key: 20,
                     "no-caps": "",
+                    disable: 0 == e.data.edit,
                     dense: "",
                     round: "",
                     class: (0, l.C_)({
                         "bg-blue-grey-8": e.Dark.isActive
                     }),
                     icon: e.data.icon,
                     onClick: e.sendValue
                 }, {
-                    default: (0, s.w5)((() => [e.data.tooltip ? ((0, s.wg)(), (0, s.j4)(_, {
+                    default: (0, s.w5)((() => [e.data.tooltip ? ((0, s.wg)(), (0, s.j4)(C, {
                         key: 0,
                         class: "text-body2"
                     }, {
                         default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, s.kq)("", !0)])),
                     _: 1
-                }, 8, ["class", "icon", "onClick"]))
+                }, 8, ["disable", "class", "icon", "onClick"]))
             }
-            const _e = {
+            const qe = {
                     key: 0
                 },
-                qe = {
+                Ae = {
                     class: "row"
                 },
-                Ae = ["onClick"];
+                De = ["onClick"];
 
-            function De(e, t, a, i, n, o) {
+            function Se(e, t, a, i, n, o) {
                 const d = (0, s.up)("q-icon"),
                     r = (0, s.up)("q-tooltip"),
                     c = (0, s.up)("q-input"),
                     h = (0, s.up)("q-btn"),
                     u = (0, s.up)("q-th"),
                     p = (0, s.up)("q-tr"),
                     m = (0, s.up)("q-checkbox"),
                     g = (0, s.up)("q-select"),
-                    f = (0, s.up)("q-td"),
-                    y = (0, s.up)("q-table");
-                return (0, s.wg)(), (0, s.j4)(y, {
+                    y = (0, s.up)("q-td"),
+                    f = (0, s.up)("q-table");
+                return (0, s.wg)(), (0, s.j4)(f, {
                     "virtual-scroll": "",
                     dense: e.data.dense,
-                    style: (0, l.j5)(e.styleSize),
+                    style: (0, l.j5)(e.styleSize ? e.styleSize : e.currentStyle()),
                     flat: "",
                     filter: e.search,
                     ref: "table",
                     virtualScrollSliceSize: "100",
                     "rows-per-page-options": [0],
                     "virtual-scroll-sticky-size-start": 48,
                     "row-key": "iiid",
                     title: e.name,
                     rows: e.rows,
                     columns: e.columns,
                     selection: e.singleMode ? "single" : "multiple",
                     selected: e.selected,
                     "onUpdate:selected": t[2] || (t[2] = t => e.selected = t)
                 }, {
-                    "top-right": (0, s.w5)((() => [!1 !== e.data.tools ? ((0, s.wg)(), (0, s.iD)("div", _e, [(0, s._)("div", qe, [(0, s.Wm)(c, {
+                    "top-right": (0, s.w5)((() => [!1 !== e.data.tools ? ((0, s.wg)(), (0, s.iD)("div", qe, [(0, s._)("div", Ae, [(0, s.Wm)(c, {
                         modelValue: e.search,
                         "onUpdate:modelValue": t[1] || (t[1] = t => e.search = t),
                         label: "Search",
                         dense: "",
                         ref: "searchField"
                     }, (0, s.Nv)({
                         append: (0, s.w5)((() => ["" != e.search ? ((0, s.wg)(), (0, s.j4)(d, {
@@ -1165,15 +1180,15 @@
                         }, 1032, ["class", "props"])))), 128))])),
                         _: 2
                     }, 1032, ["props"])])),
                     body: (0, s.w5)((t => [(0, s.Wm)(p, {
                         props: t,
                         onClick: e => t.selected = !t.selected
                     }, {
-                        default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.columns, ((a, i) => ((0, s.wg)(), (0, s.j4)(f, {
+                        default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.columns, ((a, i) => ((0, s.wg)(), (0, s.j4)(y, {
                             key: a.name,
                             props: t
                         }, {
                             default: (0, s.w5)((() => ["boolean" == typeof t.row[a.name] ? ((0, s.wg)(), (0, s.j4)(m, {
                                 key: 0,
                                 modelValue: t.row[a.name],
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, s => e.change_switcher(t.row, a.name, i)],
@@ -1201,35 +1216,35 @@
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, e.change],
                                 dense: "",
                                 onKeydown: e.keyInput,
                                 autofocus: ""
                             }, null, 8, ["modelValue", "onUpdate:modelValue", "onKeydown"])) : ((0, s.wg)(), (0, s.iD)("div", {
                                 key: 3,
                                 onClick: a => e.select(t.row.iiid, i)
-                            }, (0, l.zw)(t.row[a.name]), 9, Ae))])),
+                            }, (0, l.zw)(t.row[a.name]), 9, De))])),
                             _: 2
                         }, 1032, ["props"])))), 128))])),
                         _: 2
                     }, 1032, ["props", "onClick"])])),
                     _: 1
                 }, 8, ["dense", "style", "filter", "title", "rows", "columns", "selection", "selected"])
             }
-            var Se = a(1959),
-                je = a(9058);
+            var je = a(1959),
+                ze = a(9058);
 
-            function ze(e, t) {
+            function Ze(e, t) {
                 return e.length === t.length && e.every(((e, a) => t[a] && e.iiid == t[a].iiid))
             }
-            const Ze = (0, s.aZ)({
+            const $e = (0, s.aZ)({
                 name: "utable",
                 setup(e) {
                     const {
                         data: t,
                         pdata: a
-                    } = (0, Se.BK)(e);
+                    } = (0, je.BK)(e);
                     let l = (0, s.Fl)((() => {
                             let e = [],
                                 a = t.value;
                             const s = a.headers,
                                 l = s.length,
                                 i = a.rows,
                                 n = i.length;
@@ -1243,17 +1258,17 @@
                         })),
                         i = () => {
                             let e = t.value,
                                 a = null === e.value || 0 == l.value.length ? [] : Array.isArray(e.value) ? e.value.map((e => l.value[e])) : [l.value[e.value]];
                             return a
                         },
                         n = i(),
-                        o = (0, Se.iH)(n),
-                        d = (0, Se.iH)(n),
-                        r = (0, Se.iH)(!Array.isArray(t.value.value)),
+                        o = (0, je.iH)(n),
+                        d = (0, je.iH)(n),
+                        r = (0, je.iH)(!Array.isArray(t.value.value)),
                         c = (e, s) => {
                             _([a.value.name, t.value.name, e, s])
                         },
                         h = (0, s.Fl)((() => r.value ? d.value.length > 0 ? d.value[0].iiid : null : d.value.map((e => e.iiid)))),
                         u = (0, s.Fl)((() => t.value.value));
                     return (0, s.YP)(l, ((e, t) => {
                         d.value = i(), o.value = d.value
@@ -1267,22 +1282,31 @@
                         sendMessage: c,
                         datavalue: u,
                         updated: o
                     }
                 },
                 data() {
                     return {
-                        Dark: je.Z,
+                        Dark: ze.Z,
                         search: "",
                         editMode: !1,
                         options: [],
                         cedit: null
                     }
                 },
                 methods: {
+                    currentStyle() {
+                        let e = this.data.tablerect;
+                        if (e) {
+                            let t = e.width,
+                                a = e.height;
+                            return `width: ${t}px; height: ${a}px`
+                        }
+                        return null
+                    },
                     select(e, t) {
                         this.editMode && (this.cedit = t, g && console.log("selected", e, this.cedit))
                     },
                     change_switcher(e, t, a) {
                         if (console.log(e, t, a, e[t]), this.editMode) {
                             this.cedit = a;
                             const s = e.iiid;
@@ -1373,15 +1397,15 @@
                         }
                     },
                     deselectAll() {
                         this.selected = [], this.sendMessage("changed", this.value)
                     },
                     chart() {
                         let e = this.data;
-                        e.type = "chart"
+                        e.type = "chart", e.tablerect = this.$refs.table.$el.getBoundingClientRect(), k[this.fullname].styleSize = this.currentStyle()
                     },
                     switchMode() {
                         this.singleMode = !this.singleMode, this.singleMode && this.selected.length > 1 && this.selected.splice(1)
                     },
                     switchEdit() {
                         this.editMode = !this.editMode, this.editMode && !this.singleMode && this.switchMode()
                     },
@@ -1396,22 +1420,25 @@
                         }
                         this.selected = []
                     }
                 },
                 watch: {
                     selected(e) {
                         const t = this.data;
-                        if (!ze(this.updated, this.selected)) {
+                        if (!Ze(this.updated, this.selected)) {
                             let e = this.selected.length;
                             t.value = this.singleMode ? 1 == e ? this.selected[0].iiid : null : this.selected.map((e => e.iiid)), this.sendMessage("changed", t.value), this.updated = this.selected
                         }
                         t.show && (this.showSelected(), t.show = !1)
                     }
                 },
                 computed: {
+                    fullname() {
+                        return `${this.data.name}@${this.pdata.name}`
+                    },
                     redit() {
                         return this.editMode && this.selected.length ? this.selected[0].iiid : null
                     },
                     editable() {
                         return 0 != this.data["edit"]
                     },
                     name() {
@@ -1429,52 +1456,52 @@
                 },
                 props: {
                     data: Object,
                     pdata: Object,
                     styleSize: String
                 }
             });
-            var $e = a(9267),
-                Me = a(4842),
-                We = a(8870),
-                Ee = a(2165),
-                Ve = a(8186),
-                Ke = a(2414),
-                Oe = a(3884),
-                He = a(5735),
-                Qe = a(7208);
-            const Ue = (0, U.Z)(Ze, [
-                    ["render", De]
+            var Me = a(9267),
+                We = a(4842),
+                Ee = a(8870),
+                Ve = a(2165),
+                Ke = a(8186),
+                Oe = a(2414),
+                He = a(3884),
+                Qe = a(5735),
+                Ue = a(7208);
+            const Ne = (0, U.Z)($e, [
+                    ["render", Se]
                 ]),
-                Ne = Ue;
-            R()(Ze, "components", {
-                QTable: $e.Z,
-                QInput: Me.Z,
+                Pe = Ne;
+            R()($e, "components", {
+                QTable: Me.Z,
+                QInput: We.Z,
                 QIcon: T.Z,
-                QTooltip: We.Z,
-                QBtn: Ee.Z,
-                QTr: Ve.Z,
-                QTh: Ke.Z,
-                QTd: Oe.Z,
-                QCheckbox: He.Z,
-                QSelect: Qe.Z
+                QTooltip: Ee.Z,
+                QBtn: Ve.Z,
+                QTr: Ke.Z,
+                QTh: Oe.Z,
+                QTd: He.Z,
+                QCheckbox: Qe.Z,
+                QSelect: Ue.Z
             });
-            const Pe = ["nodes", "edges"];
+            const Te = ["nodes", "edges"];
 
-            function Te(e, t, a, i, n, o) {
+            function Fe(e, t, a, i, n, o) {
                 return (0, s.wg)(), (0, s.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, l.j5)(e.styleSize),
                     ref: "cy"
-                }, null, 12, Pe)
+                }, null, 12, Te)
             }
-            var Fe = a(2393),
-                Ie = a.n(Fe);
-            const Re = Ie().stylesheet().selector("node").css({
+            var Ie = a(2393),
+                Re = a.n(Ie);
+            const Le = Re().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#26A69A",
                     "font-size": "14px"
                 }).selector(".selected").css({
                     "background-color": "#4286f4",
                     "border-color": "#ff5555",
                     "font-size": "14px"
@@ -1500,45 +1527,45 @@
                     label: "data(label)",
                     "text-rotation": "autorotate",
                     "text-margin-x": "-8px",
                     "text-margin-y": "-8px",
                     color: "#388E3C",
                     "font-size": "12px"
                 }),
-                Le = {
+                Be = {
                     animate: !0,
                     randomize: !0
                 };
 
-            function Be(e, t) {
+            function Ye(e, t) {
                 if (e.length != t.length) return !0;
                 for (let a = 0; a < e.length; a++)
                     if (e[a].id != t[a].id || e[a].label != t[a].label) return !0;
                 return !1
             }
-            const Ye = (0, s.aZ)({
+            const Xe = (0, s.aZ)({
                     name: "cgraph",
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
                         return {
                             cy: null,
-                            style: Re,
-                            layoutOptions: Le,
+                            style: Le,
+                            layoutOptions: Be,
                             selectedNodes: [],
                             selectedEdges: [],
                             oldNodes: [],
                             oldEdges: []
                         }
                     },
                     mounted() {
-                        let e = Ie()({
+                        let e = Re()({
                                 container: this.$refs.cy,
                                 elements: {
                                     nodes: this.nodes,
                                     edges: this.edges
                                 },
                                 style: this.style
                             }),
@@ -1654,15 +1681,15 @@
                                 for (let t of e) a.edges("[id='" + t + "']").addClass("highlighted")
                             }
                         },
                         data: {
                             handler(e, t) {
                                 let a = e.value,
                                     s = !1;
-                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Be(e.nodes, this.oldNodes) && (s = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Be(e.edges, this.oldEdges) && (s = !0, this.oldEdges = e.edges), s && null != this.cy) {
+                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Ye(e.nodes, this.oldNodes) && (s = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Ye(e.edges, this.oldEdges) && (s = !0, this.oldEdges = e.edges), s && null != this.cy) {
                                     this.cy.json({
                                         elements: {
                                             nodes: this.nodes,
                                             edges: this.edges
                                         }
                                     });
                                     let e = this.data.method;
@@ -1679,55 +1706,56 @@
                             this.cy.style(e)
                         },
                         layoutOptions(e) {
                             this.cy.layout(e).run()
                         }
                     }
                 }),
-                Xe = (0, U.Z)(Ye, [
-                    ["render", Te]
+                Ge = (0, U.Z)(Xe, [
+                    ["render", Fe]
                 ]),
-                Ge = Xe;
+                Je = Ge;
 
-            function Je(e, t, a, i, n, o) {
+            function et(e, t, a, i, n, o) {
                 const d = (0, s.up)("v-chart");
-                return (0, s.wg)(), (0, s.j4)(d, {
+                return (0, s.wg)(), (0, s.iD)("div", {
+                    style: (0, l.j5)(a.styleSize ? a.styleSize : o.currentStyle())
+                }, [(0, s.Wm)(d, {
                     ref: "chart",
                     "manual-update": !0,
                     onClick: o.clicked,
-                    style: (0, l.j5)(a.styleSize ? a.styleSize : "width: 300px; height: 200px"),
                     autoresize: !0
-                }, null, 8, ["onClick", "style"])
+                }, null, 8, ["onClick"])], 4)
             }
-            var et = a(7559),
-                tt = a(6938),
-                at = a(1006),
-                st = a(6080),
-                lt = a(3526),
-                it = a(763),
-                nt = a(546),
-                ot = a(6902),
-                dt = a(2826),
-                rt = a(5256),
-                ct = a(3825),
-                ht = a(8825);
-            (0, it.D)([tt.N, at.N, lt.N, st.N]), (0, it.D)([nt.N, ot.N, dt.N, rt.N, ct.N]);
-            let ut = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"];
-            const pt = {
+            var tt = a(7559),
+                at = a(6938),
+                st = a(1006),
+                lt = a(6080),
+                it = a(3526),
+                nt = a(763),
+                ot = a(546),
+                dt = a(6902),
+                rt = a(2826),
+                ct = a(5256),
+                ht = a(3825),
+                ut = a(8825);
+            (0, nt.D)([at.N, st.N, it.N, lt.N]), (0, nt.D)([ot.N, dt.N, rt.N, ct.N, ht.N]);
+            let pt = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"];
+            const mt = {
                     name: "linechart",
                     components: {
-                        VChart: et.ZP
+                        VChart: tt.ZP
                     },
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
-                        const e = (0, ht.Z)();
+                        const e = (0, ut.Z)();
                         return {
                             $q: e,
                             model: !1,
                             animation: null,
                             markPoint: null,
                             options: {
                                 responsive: !0,
@@ -1773,19 +1801,29 @@
                                     start: 0,
                                     end: 10
                                 }],
                                 series: []
                             }
                         }
                     },
-                    computed: {},
+                    computed: {
+                        fullname() {
+                            return `${this.data.name}@${this.pdata.name}`
+                        }
+                    },
                     methods: {
                         setOptions() {
                             this.$refs.chart.setOption(this.options)
                         },
+                        currentStyle() {
+                            let e = this.data.tablerect,
+                                t = e ? e.width : 300,
+                                a = e ? e.height : 200;
+                            return `width: ${t}px; height: ${a}px`
+                        },
                         processCoord(e, t, a) {
                             let s = null;
                             for (let l of t)
                                 if (e[0] == l.coord[0]) {
                                     s = l;
                                     break
                                 } a ? s ? t.splice(t.indexOf(s), 1) : t.push({
@@ -1808,15 +1846,15 @@
                         calcSeries() {
                             this.options.toolbox.feature.mySwitcher = {
                                 show: !0,
                                 title: "Switch view to the table",
                                 icon: "image:M0 2a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V2zm15 2h-4v3h4V4zm0 4h-4v3h4V8zm0 4h-4v3h3a1 1 0 0 0 1-1v-2zm-5 3v-3H6v3h4zm-5 0v-3H1v2a1 1 0 0 0 1 1h3zm-4-4h4V8H1v3zm0-4h4V4H1v3zm5-3v3h4V4H6zm4 4H6v3h4V8z",
                                 onclick: () => {
                                     let e = this.data;
-                                    e.type = "table"
+                                    e.type = "table", e.tablerect = this.$refs.chart.$el.getBoundingClientRect(), k[this.fullname].styleSize = this.currentStyle()
                                 }
                             };
                             let e = this.data.view,
                                 t = this.data.headers;
                             "_" != this.data.name[0] && (this.options.title.text = this.data.name);
                             let a = e.split("-"),
                                 s = a[1].split(",");
@@ -1825,15 +1863,15 @@
                             for (let n = 0; n < s.length; n++) s[n] = "i" == s[n] ? -1 : parseInt(s[n]), l.push([]), n && (this.options.series.push({
                                 name: t[s[n]],
                                 type: "line",
                                 symbol: "circle",
                                 symbolSize: 10,
                                 sampling: "lttb",
                                 itemStyle: {
-                                    color: ut[n]
+                                    color: pt[n]
                                 },
                                 data: l[n]
                             }), this.options.legend.data.push(t[s[n]]));
                             this.options.xAxis.data = l[0];
                             let i = this.data.rows;
                             for (let n = 0; n < i.length; n++)
                                 for (let e = 0; e < s.length; e++) l[e].push(-1 == s[e] ? n : i[n][s[e]]);
@@ -1863,33 +1901,33 @@
                         this.calcSeries();
                         let e = this;
                         this.$refs.chart.chart.on("datazoom", (function(t) {
                             (t.start || t.end) && (e.animation = t)
                         }))
                     }
                 },
-                mt = (0, U.Z)(pt, [
-                    ["render", Je]
+                gt = (0, U.Z)(mt, [
+                    ["render", et]
                 ]),
-                gt = mt;
+                yt = gt;
 
             function ft(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
                 a.open("POST", w, !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
-            const yt = (0, s.aZ)({
+            const wt = (0, s.aZ)({
                 name: "element",
                 components: {
-                    utable: Ne,
-                    cgraph: Ge,
-                    linechart: gt
+                    utable: Pe,
+                    cgraph: Je,
+                    linechart: yt
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
                     onAdded(e) {
                         0 !== e.length && (0 !== this.fileArr.length ? (this.$refs.uploaderRef.removeFile(this.fileArr[0]), this.fileArr.splice(0, 1, e[0])) : this.fileArr.push(e[0]))
@@ -1958,21 +1996,21 @@
                         document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(ft, "image/jpeg")
                     },
                     rect() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         return e.getBoundingClientRect()
                     },
                     geom() {
-                        let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
-                        e || (e = this.$el.previousElementSibling, e = "clientHeight" in e ? e : e.nextElementSibling);
-                        let t = this.type;
-                        const a = "textarea" == t || "graph" == t || "chart" == t ? e : e.querySelector("table" == t ? ".scroll" : ".q-tree"),
-                            s = e.getBoundingClientRect();
+                        let e = this.type,
+                            t = this.$el;
+                        t = "tree" == e || "list" == e ? t.querySelector(".scroll") : "clientHeight" in t ? t : t.nextElementSibling, t || (t = this.$el.previousElementSibling, t = "clientHeight" in t ? t : t.nextElementSibling);
+                        const a = "textarea" == e || "graph" == e || "chart" == e ? t : t.querySelector("table" == e ? ".scroll" : ".q-tree"),
+                            s = t.getBoundingClientRect();
                         return {
-                            el: e,
+                            el: t,
                             inner: a,
                             left: s.left,
                             right: s.right,
                             top: s.top,
                             scrollHeight: a.scrollHeight,
                             scrollWidth: a.scrollWidth
                         }
@@ -1982,17 +2020,17 @@
                     k[this.fullname] = this
                 },
                 mounted() {
                     k[this.fullname] = this, this.data.focus && this.$refs.inputRef.$el.focus()
                 },
                 data() {
                     return {
-                        Dark: je.Z,
+                        Dark: ze.Z,
                         value: this.data.value,
-                        styleSize: h.visibility ? S(this) : null,
+                        styleSize: A ? S(this) : null,
                         has_recalc: !0,
                         host_path: w,
                         options: [],
                         expandedKeys: [],
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
@@ -2103,58 +2141,56 @@
                         0 == a.length && (a = t.getElementsByTagName("input")), a[0].setSelectionRange(e[0], e[1])
                     },
                     data(e, t) {
                         this.styleSize || (this.styleSize = ""), this.value = this.data.value, this.updated = this.value, k[this.fullname] = this
                     }
                 }
             });
-            var wt = a(4027),
-                bt = a(9721),
+            var bt = a(4027),
                 kt = a(8886),
                 vt = a(8761),
                 xt = a(1232),
                 Ct = a(5551),
                 _t = a(5869),
                 qt = a(1745),
                 At = a(8506);
-            const Dt = (0, U.Z)(yt, [
-                    ["render", Ce],
-                    ["__scopeId", "data-v-d4b5cc5e"]
+            const Dt = (0, U.Z)(wt, [
+                    ["render", _e],
+                    ["__scopeId", "data-v-905c4cee"]
                 ]),
                 St = Dt;
 
             function jt(e) {
                 let t = e.type;
                 return "tree" == t || "table" == t || "list" == t || "textarea" == t || "graph" == t || "chart" == t
             }
-            R()(yt, "components", {
-                QImg: wt.Z,
+            R()(wt, "components", {
+                QImg: bt.Z,
                 QIcon: T.Z,
-                QSelect: Qe.Z,
-                QBadge: bt.Z,
-                QCheckbox: He.Z,
+                QSelect: Ue.Z,
+                QCheckbox: Qe.Z,
                 QToggle: kt.Z,
-                QBtn: Ee.Z,
+                QBtn: Ve.Z,
                 QBtnToggle: vt.Z,
-                QInput: Me.Z,
+                QInput: We.Z,
                 QScrollArea: xt.Z,
                 QTree: Ct.Z,
                 QSeparator: _t.Z,
                 QUploader: qt.Z,
-                QTooltip: We.Z,
+                QTooltip: Ee.Z,
                 QSpinnerIos: At.Z
             });
             const zt = (0, s.aZ)({
                 name: "block",
                 components: {
                     element: St
                 },
                 data() {
                     return {
-                        Dark: je.Z,
+                        Dark: ze.Z,
                         styleSize: null,
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
                             width: "4px",
                             opacity: .75
@@ -2367,28 +2403,28 @@
                 ]),
                 Tt = Pt;
             R()(Qt, "components", {
                 QDialog: Ut.Z,
                 QCard: Zt.Z,
                 QItemLabel: F.Z,
                 QSpace: Nt.Z,
-                QBtn: Ee.Z
+                QBtn: Ve.Z
             });
             var Ft = a(589);
             let It = "theme";
             try {
-                je.Z.set(Ft.Z.getItem(It))
+                ze.Z.set(Ft.Z.getItem(It))
             } catch (la) {}
             let Rt = null;
             const Lt = (0, s.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
-                        Dark: je.Z,
+                        Dark: ze.Z,
                         menu: [],
                         tab: "",
                         tooldata: {
                             name: "toolbar"
                         },
                         localServer: !0,
                         statusConnect: !1,
@@ -2418,15 +2454,15 @@
                     },
                     right_toolbar() {
                         return this.screen.toolbar.filter((e => e.right))
                     }
                 },
                 methods: {
                     switchTheme() {
-                        je.Z.set(!je.Z.isActive), Ft.Z.set(It, je.Z.isActive)
+                        ze.Z.set(!ze.Z.isActive), Ft.Z.set(It, ze.Z.isActive)
                     },
                     toggleLeftDrawer() {
                         this.leftDrawerOpen = !this.leftDrawerOpen
                     },
                     tabclick(e) {
                         _(["root", e])
                     },
@@ -2544,19 +2580,19 @@
                     ["render", o]
                 ]),
                 sa = aa;
             R()(Lt, "components", {
                 QLayout: Bt.Z,
                 QHeader: Yt.Z,
                 QToolbar: Xt.Z,
-                QBtn: Ee.Z,
+                QBtn: Ve.Z,
                 QItemLabel: F.Z,
                 QTabs: Gt.Z,
                 QTab: Jt.Z,
                 QSpace: Nt.Z,
-                QTooltip: We.Z,
+                QTooltip: Ee.Z,
                 QPageContainer: ea.Z,
                 QPage: ta.Z
             })
         }
     }
 ]);
```

### Comparing `unigui-1.9.9/unigui/web/js/vendor.8cb03aaa.js` & `unigui-2.0.0/unigui/web/js/vendor.bc1bae42.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4495,58 +4495,14 @@
                 oe = e => {
                     const t = z(e) ? Number(e) : NaN;
                     return isNaN(t) ? e : t
                 };
             let ae;
             const se = () => ae || (ae = "undefined" !== typeof globalThis ? globalThis : "undefined" !== typeof self ? self : "undefined" !== typeof window ? window : "undefined" !== typeof n.g ? n.g : {})
         },
-        9721: (e, t, n) => {
-            "use strict";
-            n.d(t, {
-                Z: () => s
-            });
-            var r = n(3673),
-                i = n(908),
-                o = n(7657);
-            const a = ["top", "middle", "bottom"],
-                s = (0, i.L)({
-                    name: "QBadge",
-                    props: {
-                        color: String,
-                        textColor: String,
-                        floating: Boolean,
-                        transparent: Boolean,
-                        multiLine: Boolean,
-                        outline: Boolean,
-                        rounded: Boolean,
-                        label: [Number, String],
-                        align: {
-                            type: String,
-                            validator: e => a.includes(e)
-                        }
-                    },
-                    setup(e, {
-                        slots: t
-                    }) {
-                        const n = (0, r.Fl)((() => void 0 !== e.align ? {
-                                verticalAlign: e.align
-                            } : null)),
-                            i = (0, r.Fl)((() => {
-                                const t = !0 === e.outline && e.color || e.textColor;
-                                return `q-badge flex inline items-center no-wrap q-badge--${!0===e.multiLine?"multi":"single"}-line` + (!0 === e.outline ? " q-badge--outline" : void 0 !== e.color ? ` bg-${e.color}` : "") + (void 0 !== t ? ` text-${t}` : "") + (!0 === e.floating ? " q-badge--floating" : "") + (!0 === e.rounded ? " q-badge--rounded" : "") + (!0 === e.transparent ? " q-badge--transparent" : "")
-                            }));
-                        return () => (0, r.h)("div", {
-                            class: i.value,
-                            style: n.value,
-                            role: "status",
-                            "aria-label": e.label
-                        }, (0, o.vs)(t.default, void 0 !== e.label ? [e.label] : []))
-                    }
-                })
-        },
         8761: (e, t, n) => {
             "use strict";
             n.d(t, {
                 Z: () => c
             });
             var r = n(3673),
                 i = n(2165),
```

### Comparing `unigui-1.9.9/unigui/web/js/app.c32942a4.js` & `unigui-2.0.0/unigui/web/js/app.39deedc9.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(768)]).then(r.bind(r, 9768)),
+                        component: () => Promise.all([r.e(736), r.e(737)]).then(r.bind(r, 4737)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -164,24 +164,24 @@
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, o) => (r.f[o](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "283445be",
             430: "591e9a73",
-            768: "89ad69c0"
+            737: "229a004a"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
             736: "f747ec02",
-            768: "30396533"
+            737: "bedc790c"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
@@ -264,15 +264,15 @@
                 e(o, l, n, a)
             })),
             n = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                768: 1
+                737: 1
             };
             n[e] ? t.push(n[e]) : 0 !== n[e] && r[e] && t.push(n[e] = o(e).then((() => {
                 n[e] = 0
             }), (t => {
                 throw delete n[e], t
             })))
         }
```

### Comparing `unigui-1.9.9/unigui/web/js/193.283445be.js` & `unigui-2.0.0/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/unigui/web/index.html` & `unigui-2.0.0/unigui/web/index.html`

 * *Files 11% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.8cb03aaa.js></script><script defer src=js/app.c32942a4.js></script><link href=css/vendor.f747ec02.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.bc1bae42.js></script><script defer src=js/app.39deedc9.js></script><link href=css/vendor.f747ec02.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.9.9/LICENSE` & `unigui-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.9.9/setup.py` & `unigui-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.9.9',      
+      version='2.0.0',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
       url="https://github.com/Claus1/unigui" ,      
       include_package_data=True,
       install_requires=[
-          'websockets','jsonpickle', 'aiohttp', 'watchdog', 'jsoncomparison', 'requests'
+          'websockets','jsonpickle', 'aiohttp', 'watchdog', 'jsoncomparison', 'requests','pandas'
       ],
       zip_safe=False)
```

### Comparing `unigui-1.9.9/PKG-INFO` & `unigui-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.9.9
+Version: 2.0.0
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# unigui #
+# unigui 2 #
 Universal GUI Framework and Protocol (Python)
 
 ### Purpose ###
 Provide a programming technology that does not require front-end programming, for a server written in any language, for displaying on any device, in any resolution, without any tuning. 
 
 ### Installing ###
 ```
 pip install unigui
 ```
 
 ### How it works inside ###
 The exchange protocol for the solution is JSON as the most universally accessible, readable, and popular format for Web. The server sends JSON data to the front-end unigui which has built-in tools (autodesigner) and automatically builds a standart Google Material Design GUI for the user data. No markup, drawing instructions and the other dull job are required. From the constructed Unigui screen the server receives a JSON message flow which fully describes what the user did. The message format is ["Block", "Elem", "type of action", value], where "Block"and "Elem"are the names of the block and its element, "value" is the JSON value of the action/event that has happened. The server can either accept the change or roll it back by sending an info window about an inconsistency. The server can open a dialog box, send popup Warning, Error,.. or an entirely new screen. Unigui instantly and automatically displays actual server state. 
 
 ### Programming ###
-Unigui is the language and platform independent technology. This repo explains how to work with Unigui using Python and the tiny but optimal framework for that. Unigui web version is included in this library. Unigui for Go is accessible in https://github.com/Claus1/unigui-go
+Unigui is the language and platform independent technology. This repo explains how to work with Unigui using Python and the tiny but optimal framework for that. Unigui web version is included in this library.  Supports Python 3.6 and up.
+
 
 ### High level - Screen ###
 The program directory has to contain a screens folder which contains all screens which Unigui has to show.
 
 Screen example tests/screens/main.py
 ```
 name = "Main"
@@ -378,21 +379,15 @@
 ```
 Update window message 
 ```
 user.progress(" 1% is done..")
 ```
 Close window user.progress(None) or automatically when the handler returns something.
 
-### Other subtle benefits of a Unigui protocol and technology. ###
-1. Possible to work with any set of unigui resources as with a single system, within the same GUI user space, carries out any available operations, including crossing, on the fly.
-2. Reproduces and saves sequences of the user interaction with the system without programming. It can be used for complex testing, supporting of security protocols and more.
-3. Possible to mirror a session to other users, works simultaneously in one session for many users.
-
-
-### Milti-user programming? You don't need it! ###
+### Milti-user programming.###
 Unigui automatically creates and serves an environment for every user.
 The management class is User contains all required methods for processing and handling the user activity. A programmer can redefine methods in the inherited class, point it as system user class and that is all. Such methods suit for history navigation, undo/redo and initial operations. The screen folder contains screens which are recreated for every user. The same about blocks. The code and modules outside that folders are common for all users as usual. By default Unigui use the system User class and you do not need to point it. 
 ```
 class Hello_user(unigui.User):
     def __init__(self):
         super().__init__()
         print('New Hello user connected and created!')
```

### Comparing `unigui-1.9.9/README.md` & `unigui-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-# unigui #
+# unigui 2 #
 Universal GUI Framework and Protocol (Python)
 
 ### Purpose ###
 Provide a programming technology that does not require front-end programming, for a server written in any language, for displaying on any device, in any resolution, without any tuning. 
 
 ### Installing ###
 ```
 pip install unigui
 ```
 
 ### How it works inside ###
 The exchange protocol for the solution is JSON as the most universally accessible, readable, and popular format for Web. The server sends JSON data to the front-end unigui which has built-in tools (autodesigner) and automatically builds a standart Google Material Design GUI for the user data. No markup, drawing instructions and the other dull job are required. From the constructed Unigui screen the server receives a JSON message flow which fully describes what the user did. The message format is ["Block", "Elem", "type of action", value], where "Block"and "Elem"are the names of the block and its element, "value" is the JSON value of the action/event that has happened. The server can either accept the change or roll it back by sending an info window about an inconsistency. The server can open a dialog box, send popup Warning, Error,.. or an entirely new screen. Unigui instantly and automatically displays actual server state. 
 
 ### Programming ###
-Unigui is the language and platform independent technology. This repo explains how to work with Unigui using Python and the tiny but optimal framework for that. Unigui web version is included in this library. Unigui for Go is accessible in https://github.com/Claus1/unigui-go
+Unigui is the language and platform independent technology. This repo explains how to work with Unigui using Python and the tiny but optimal framework for that. Unigui web version is included in this library.  Supports Python 3.6 and up.
+
 
 ### High level - Screen ###
 The program directory has to contain a screens folder which contains all screens which Unigui has to show.
 
 Screen example tests/screens/main.py
 ```
 name = "Main"
@@ -366,21 +367,15 @@
 ```
 Update window message 
 ```
 user.progress(" 1% is done..")
 ```
 Close window user.progress(None) or automatically when the handler returns something.
 
-### Other subtle benefits of a Unigui protocol and technology. ###
-1. Possible to work with any set of unigui resources as with a single system, within the same GUI user space, carries out any available operations, including crossing, on the fly.
-2. Reproduces and saves sequences of the user interaction with the system without programming. It can be used for complex testing, supporting of security protocols and more.
-3. Possible to mirror a session to other users, works simultaneously in one session for many users.
-
-
-### Milti-user programming? You don't need it! ###
+### Milti-user programming.###
 Unigui automatically creates and serves an environment for every user.
 The management class is User contains all required methods for processing and handling the user activity. A programmer can redefine methods in the inherited class, point it as system user class and that is all. Such methods suit for history navigation, undo/redo and initial operations. The screen folder contains screens which are recreated for every user. The same about blocks. The code and modules outside that folders are common for all users as usual. By default Unigui use the system User class and you do not need to point it. 
 ```
 class Hello_user(unigui.User):
     def __init__(self):
         super().__init__()
         print('New Hello user connected and created!')
```

### Comparing `unigui-1.9.9/unigui.egg-info/PKG-INFO` & `unigui-2.0.0/unigui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.9.9
+Version: 2.0.0
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# unigui #
+# unigui 2 #
 Universal GUI Framework and Protocol (Python)
 
 ### Purpose ###
 Provide a programming technology that does not require front-end programming, for a server written in any language, for displaying on any device, in any resolution, without any tuning. 
 
 ### Installing ###
 ```
 pip install unigui
 ```
 
 ### How it works inside ###
 The exchange protocol for the solution is JSON as the most universally accessible, readable, and popular format for Web. The server sends JSON data to the front-end unigui which has built-in tools (autodesigner) and automatically builds a standart Google Material Design GUI for the user data. No markup, drawing instructions and the other dull job are required. From the constructed Unigui screen the server receives a JSON message flow which fully describes what the user did. The message format is ["Block", "Elem", "type of action", value], where "Block"and "Elem"are the names of the block and its element, "value" is the JSON value of the action/event that has happened. The server can either accept the change or roll it back by sending an info window about an inconsistency. The server can open a dialog box, send popup Warning, Error,.. or an entirely new screen. Unigui instantly and automatically displays actual server state. 
 
 ### Programming ###
-Unigui is the language and platform independent technology. This repo explains how to work with Unigui using Python and the tiny but optimal framework for that. Unigui web version is included in this library. Unigui for Go is accessible in https://github.com/Claus1/unigui-go
+Unigui is the language and platform independent technology. This repo explains how to work with Unigui using Python and the tiny but optimal framework for that. Unigui web version is included in this library.  Supports Python 3.6 and up.
+
 
 ### High level - Screen ###
 The program directory has to contain a screens folder which contains all screens which Unigui has to show.
 
 Screen example tests/screens/main.py
 ```
 name = "Main"
@@ -378,21 +379,15 @@
 ```
 Update window message 
 ```
 user.progress(" 1% is done..")
 ```
 Close window user.progress(None) or automatically when the handler returns something.
 
-### Other subtle benefits of a Unigui protocol and technology. ###
-1. Possible to work with any set of unigui resources as with a single system, within the same GUI user space, carries out any available operations, including crossing, on the fly.
-2. Reproduces and saves sequences of the user interaction with the system without programming. It can be used for complex testing, supporting of security protocols and more.
-3. Possible to mirror a session to other users, works simultaneously in one session for many users.
-
-
-### Milti-user programming? You don't need it! ###
+### Milti-user programming.###
 Unigui automatically creates and serves an environment for every user.
 The management class is User contains all required methods for processing and handling the user activity. A programmer can redefine methods in the inherited class, point it as system user class and that is all. Such methods suit for history navigation, undo/redo and initial operations. The screen folder contains screens which are recreated for every user. The same about blocks. The code and modules outside that folders are common for all users as usual. By default Unigui use the system User class and you do not need to point it. 
 ```
 class Hello_user(unigui.User):
     def __init__(self):
         super().__init__()
         print('New Hello user connected and created!')
```

### Comparing `unigui-1.9.9/unigui.egg-info/SOURCES.txt` & `unigui-2.0.0/unigui.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/768.30396533.css
+unigui/web/css/737.bedc790c.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.f747ec02.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -31,10 +31,10 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.283445be.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/768.89ad69c0.js
-unigui/web/js/app.c32942a4.js
-unigui/web/js/vendor.8cb03aaa.js
+unigui/web/js/737.229a004a.js
+unigui/web/js/app.39deedc9.js
+unigui/web/js/vendor.bc1bae42.js
```

