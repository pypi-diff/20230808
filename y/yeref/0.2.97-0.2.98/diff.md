# Comparing `tmp/yeref-0.2.97.tar.gz` & `tmp/yeref-0.2.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.2.97.tar", last modified: Tue Aug  8 16:19:22 2023, max compression
+gzip compressed data, was "yeref-0.2.98.tar", last modified: Tue Aug  8 16:24:16 2023, max compression
```

## Comparing `yeref-0.2.97.tar` & `yeref-0.2.98.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 16:19:22.928993 yeref-0.2.97/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 16:19:22.929237 yeref-0.2.97/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-08 16:19:22.930151 yeref-0.2.97/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1552 2023-08-08 16:18:49.000000 yeref-0.2.97/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 16:19:22.920324 yeref-0.2.97/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.97/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   583683 2023-08-06 16:53:26.000000 yeref-0.2.97/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   238932 2023-08-08 16:16:45.000000 yeref-0.2.97/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 16:19:22.928145 yeref-0.2.97/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 16:19:22.000000 yeref-0.2.97/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-08-08 16:19:22.000000 yeref-0.2.97/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-08 16:19:22.000000 yeref-0.2.97/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-08-08 16:19:22.000000 yeref-0.2.97/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 16:24:16.263089 yeref-0.2.98/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 16:24:16.263363 yeref-0.2.98/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-08 16:24:16.264334 yeref-0.2.98/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1552 2023-08-08 16:23:51.000000 yeref-0.2.98/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 16:24:16.248842 yeref-0.2.98/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.98/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   583683 2023-08-06 16:53:26.000000 yeref-0.2.98/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   238924 2023-08-08 16:23:51.000000 yeref-0.2.98/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 16:24:16.262010 yeref-0.2.98/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 16:24:16.000000 yeref-0.2.98/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-08-08 16:24:16.000000 yeref-0.2.98/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-08 16:24:16.000000 yeref-0.2.98/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-08-08 16:24:16.000000 yeref-0.2.98/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.2.97/setup.py` & `yeref-0.2.98/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.2.97',
+      version='0.2.98',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.2.97/yeref/l_.py` & `yeref-0.2.98/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.2.97/yeref/yeref.py` & `yeref-0.2.98/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -5301,25 +5301,25 @@
         return result
 
 
 # endregion
 
 
 # region web
-async def region_web(BOT_TID, POST_ID, POST_TYPE, POST_TEXT, POST_LNK, POST_BUTTON, ENT_TYPE, MEDIA_D, BASE_D,
+async def region_web(BOT_TID, BOT_LC, POST_ID, POST_TYPE, POST_TEXT, POST_LNK, POST_BUTTON, ENT_TYPE, MEDIA_D, BASE_D,
                      bot_username):
     result = None
     try:
         POST_TEXT = POST_TEXT.replace('<tg-spoiler>', '').replace('</tg-spoiler>', '')
         BASE_BOT = os.path.join(MEDIA_D, str(BOT_TID), f"{str(BOT_TID)}.db")
         os.makedirs(os.path.join(MEDIA_D, str(BOT_TID)), exist_ok=True, mode=0o777)
         await db_bot_create(BASE_BOT)
-        sql = "SELECT BOT_TOKENTGPH, BOT_USERNAME, BOT_FIRSTNAME, BOT_LC FROM BOT WHERE BOT_TID=?"
+        sql = "SELECT BOT_TOKENTGPH, BOT_USERNAME, BOT_FIRSTNAME FROM BOT WHERE BOT_TID=?"
         data_bot = await db_select(sql, (BOT_TID,), BASE_D)
-        BOT_TOKENTGPH, BOT_USERNAME, BOT_FIRSTNAME, BOT_LC = data_bot[0]
+        BOT_TOKENTGPH, BOT_USERNAME, BOT_FIRSTNAME = data_bot[0]
 
         WEB_D = os.path.join(MEDIA_D, str(BOT_TID), 'WEB')
         os.makedirs(WEB_D, exist_ok=True, mode=0o777)
         file_html = os.path.join(WEB_D, f"{POST_ID}.html")
         msg_text = POST_TEXT
 
         m_html = ''
```

