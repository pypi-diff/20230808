# Comparing `tmp/yeref-0.3.0.tar.gz` & `tmp/yeref-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.3.0.tar", last modified: Tue Aug  8 17:16:58 2023, max compression
+gzip compressed data, was "yeref-0.3.1.tar", last modified: Tue Aug  8 17:33:43 2023, max compression
```

## Comparing `yeref-0.3.0.tar` & `yeref-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 17:16:58.617169 yeref-0.3.0/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-08-08 17:16:58.617388 yeref-0.3.0/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-08 17:16:58.618262 yeref-0.3.0/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1553 2023-08-08 17:16:43.000000 yeref-0.3.0/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 17:16:58.611652 yeref-0.3.0/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.3.0/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   583683 2023-08-06 16:53:26.000000 yeref-0.3.0/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   238926 2023-08-08 16:30:08.000000 yeref-0.3.0/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 17:16:58.616655 yeref-0.3.0/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-08-08 17:16:58.000000 yeref-0.3.0/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-08-08 17:16:58.000000 yeref-0.3.0/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-08 17:16:58.000000 yeref-0.3.0/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-08-08 17:16:58.000000 yeref-0.3.0/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 17:33:43.581299 yeref-0.3.1/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-08-08 17:33:43.581456 yeref-0.3.1/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-08 17:33:43.582206 yeref-0.3.1/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1553 2023-08-08 17:33:22.000000 yeref-0.3.1/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 17:33:43.578369 yeref-0.3.1/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.3.1/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   583683 2023-08-06 16:53:26.000000 yeref-0.3.1/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   239024 2023-08-08 17:33:22.000000 yeref-0.3.1/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 17:33:43.580925 yeref-0.3.1/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-08-08 17:33:43.000000 yeref-0.3.1/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-08-08 17:33:43.000000 yeref-0.3.1/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-08 17:33:43.000000 yeref-0.3.1/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-08-08 17:33:43.000000 yeref-0.3.1/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.3.0/setup.py` & `yeref-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.3.00',
+      version='0.3.01',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.3.0/yeref/l_.py` & `yeref-0.3.1/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.3.0/yeref/yeref.py` & `yeref-0.3.1/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -5348,14 +5348,16 @@
 
             m_html = f'''<div class="media-wrapper">{add_number}{add_media}{add_prev}{add_next}{add_dots}</div>'''
         print(m_html)
 
         txt_html = ''
         if msg_text and msg_text.strip() != '' and msg_text != str_empty:
             msg_text = msg_text.strip()
+            if ENT_TYPE == 'MSG':
+                msg_text = await convert_tgmd_to_html(msg_text)
             msg_arr = re.split(r'\s+', msg_text)
             # print(msg_arr)
 
             for msg_item in msg_arr:
                 if msg_item.startswith('#') or msg_item.startswith('$'):
                     msg_text = msg_text.replace(msg_item, f"<span>{msg_item}</span>")
             txt_html = f'<div class="text">{msg_text}</div>'
```

