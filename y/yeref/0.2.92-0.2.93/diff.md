# Comparing `tmp/yeref-0.2.92.tar.gz` & `tmp/yeref-0.2.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.2.92.tar", last modified: Tue Aug  8 14:05:22 2023, max compression
+gzip compressed data, was "yeref-0.2.93.tar", last modified: Tue Aug  8 14:07:35 2023, max compression
```

## Comparing `yeref-0.2.92.tar` & `yeref-0.2.93.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 14:05:22.948347 yeref-0.2.92/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 14:05:22.948594 yeref-0.2.92/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-08 14:05:22.950618 yeref-0.2.92/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1552 2023-08-08 14:05:02.000000 yeref-0.2.92/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 14:05:22.939282 yeref-0.2.92/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.92/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   583683 2023-08-06 16:53:26.000000 yeref-0.2.92/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   237498 2023-08-08 14:05:02.000000 yeref-0.2.92/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 14:05:22.947462 yeref-0.2.92/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 14:05:22.000000 yeref-0.2.92/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-08-08 14:05:22.000000 yeref-0.2.92/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-08 14:05:22.000000 yeref-0.2.92/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-08-08 14:05:22.000000 yeref-0.2.92/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 14:07:35.305098 yeref-0.2.93/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 14:07:35.305510 yeref-0.2.93/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-08 14:07:35.306820 yeref-0.2.93/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1552 2023-08-08 14:07:11.000000 yeref-0.2.93/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 14:07:35.293695 yeref-0.2.93/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.93/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   583683 2023-08-06 16:53:26.000000 yeref-0.2.93/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   237486 2023-08-08 14:07:11.000000 yeref-0.2.93/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 14:07:35.304118 yeref-0.2.93/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 14:07:35.000000 yeref-0.2.93/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-08-08 14:07:35.000000 yeref-0.2.93/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-08 14:07:35.000000 yeref-0.2.93/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-08-08 14:07:35.000000 yeref-0.2.93/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.2.92/setup.py` & `yeref-0.2.93/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.2.92',
+      version='0.2.93',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.2.92/yeref/l_.py` & `yeref-0.2.93/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.2.92/yeref/yeref.py` & `yeref-0.2.93/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -5335,15 +5335,15 @@
             txt_html = f'<div class="text">{msg_text.strip()}</div>'
 
         btn_html = ''
         if POST_BUTTON:
             extra_id = 0
             btns_html = ''
             row_html = '<div class="buttons-row">'
-            dic_btns = await check_buttons(bot, my_tid, POST_BUTTON, True)
+            dic_btns = await check_buttons2(POST_BUTTON, True)
 
             for k, v in dic_btns.items():
                 if not v[0] or (len(v) > 0 and v[-1] is None):
                     if len(row_html) > len('<div class="buttons-row">'):
                         btns_html = f"{btns_html}{row_html}</div>"
                         row_html = '<div class="buttons-row">'
                     continue
```

