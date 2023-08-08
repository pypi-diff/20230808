# Comparing `tmp/yeref-0.2.94.tar.gz` & `tmp/yeref-0.2.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.2.94.tar", last modified: Tue Aug  8 14:39:37 2023, max compression
+gzip compressed data, was "yeref-0.2.95.tar", last modified: Tue Aug  8 15:18:18 2023, max compression
```

## Comparing `yeref-0.2.94.tar` & `yeref-0.2.95.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 14:39:37.944015 yeref-0.2.94/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 14:39:37.944274 yeref-0.2.94/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-08 14:39:37.944992 yeref-0.2.94/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1552 2023-08-08 14:39:25.000000 yeref-0.2.94/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 14:39:37.936132 yeref-0.2.94/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.94/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   583683 2023-08-06 16:53:26.000000 yeref-0.2.94/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   237436 2023-08-08 14:29:18.000000 yeref-0.2.94/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 14:39:37.943290 yeref-0.2.94/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 14:39:37.000000 yeref-0.2.94/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-08-08 14:39:37.000000 yeref-0.2.94/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-08 14:39:37.000000 yeref-0.2.94/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-08-08 14:39:37.000000 yeref-0.2.94/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 15:18:18.045060 yeref-0.2.95/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 15:18:18.045292 yeref-0.2.95/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-08 15:18:18.046454 yeref-0.2.95/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1552 2023-08-08 15:18:05.000000 yeref-0.2.95/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 15:18:18.041149 yeref-0.2.95/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.95/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   583683 2023-08-06 16:53:26.000000 yeref-0.2.95/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   237742 2023-08-08 15:18:05.000000 yeref-0.2.95/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 15:18:18.044467 yeref-0.2.95/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 15:18:18.000000 yeref-0.2.95/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-08-08 15:18:18.000000 yeref-0.2.95/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-08 15:18:18.000000 yeref-0.2.95/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-08-08 15:18:18.000000 yeref-0.2.95/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.2.94/setup.py` & `yeref-0.2.95/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.2.94',
+      version='0.2.95',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.2.94/yeref/l_.py` & `yeref-0.2.95/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.2.94/yeref/yeref.py` & `yeref-0.2.95/yeref/yeref.py`

 * *Files 1% similar despite different names*

```diff
@@ -5328,15 +5328,23 @@
                 add_media = f'<video class="media{add_rounded}" src="{TMP_LNK}" controls autoplay loop muted></video>'
 
             m_html = f'''<div class="media-wrapper">{add_number}{add_media}{add_prev}{add_next}{add_dots}</div>'''
         print(m_html)
 
         txt_html = ''
         if msg_text and msg_text.strip() != '' and msg_text != str_empty:
-            txt_html = f'<div class="text">{msg_text.strip()}</div>'
+            msg_text = msg_text.strip()
+            msg_arr = re.split(r'\s+', msg_text)
+            print(msg_arr)
+
+            for msg_item in msg_arr:
+                if msg_item.startswith('#') or msg_item.startswith('$'):
+                    msg_text = msg_text.replace(msg_item, f"<span>{msg_item}</span>")
+
+            txt_html = f'<div class="text">{msg_text}</div>'
 
         btn_html = ''
         if POST_BUTTON:
             extra_id = 0
             btns_html = ''
             row_html = '<div class="buttons-row">'
             dic_btns = await check_buttons2(POST_BUTTON, True)
```

