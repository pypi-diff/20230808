# Comparing `tmp/intelmo-1.0.0.tar.gz` & `tmp/intelmo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intelmo-1.0.0.tar", last modified: Sat Aug  5 18:36:10 2023, max compression
+gzip compressed data, was "intelmo-1.0.1.tar", last modified: Mon Aug  7 23:20:28 2023, max compression
```

## Comparing `intelmo-1.0.0.tar` & `intelmo-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-05 18:36:10.288877 intelmo-1.0.0/
--rw-r--r--   0 chunxuyang   (501) staff       (20)      347 2023-08-05 18:36:10.288780 intelmo-1.0.0/PKG-INFO
--rw-r--r--   0 chunxuyang   (501) staff       (20)       62 2023-07-11 20:32:46.000000 intelmo-1.0.0/README.md
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-05 18:36:10.284708 intelmo-1.0.0/intelmo.egg-info/
--rw-r--r--   0 chunxuyang   (501) staff       (20)      347 2023-08-05 18:36:10.000000 intelmo-1.0.0/intelmo.egg-info/PKG-INFO
--rw-r--r--   0 chunxuyang   (501) staff       (20)      705 2023-08-05 18:36:10.000000 intelmo-1.0.0/intelmo.egg-info/SOURCES.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-08-05 18:36:10.000000 intelmo-1.0.0/intelmo.egg-info/dependency_links.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)       54 2023-08-05 18:36:10.000000 intelmo-1.0.0/intelmo.egg-info/requires.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)       15 2023-08-05 18:36:10.000000 intelmo-1.0.0/intelmo.egg-info/top_level.txt
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-05 18:36:10.285291 intelmo-1.0.0/interactivenlp/
--rw-r--r--   0 chunxuyang   (501) staff       (20)      218 2023-07-27 01:07:04.000000 intelmo-1.0.0/interactivenlp/__init__.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-05 18:36:10.286070 intelmo-1.0.0/interactivenlp/controllers/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 intelmo-1.0.0/interactivenlp/controllers/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     6794 2023-07-29 21:47:39.000000 intelmo-1.0.0/interactivenlp/controllers/reader_controller.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      818 2023-07-27 01:10:19.000000 intelmo-1.0.0/interactivenlp/controllers/rss_controller.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-05 18:36:10.287291 intelmo-1.0.0/interactivenlp/models/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 intelmo-1.0.0/interactivenlp/models/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      520 2023-08-03 23:26:35.000000 intelmo-1.0.0/interactivenlp/models/article.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     2199 2023-07-29 22:24:21.000000 intelmo-1.0.0/interactivenlp/models/block.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      868 2023-07-24 23:42:14.000000 intelmo-1.0.0/interactivenlp/models/form.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1028 2023-08-03 23:23:01.000000 intelmo-1.0.0/interactivenlp/models/rss.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     5350 2023-08-03 23:26:42.000000 intelmo-1.0.0/interactivenlp/models/task.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1034 2023-07-29 20:32:23.000000 intelmo-1.0.0/interactivenlp/server.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-05 18:36:10.288245 intelmo-1.0.0/interactivenlp/types/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 intelmo-1.0.0/interactivenlp/types/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     2579 2023-07-29 21:07:20.000000 intelmo-1.0.0/interactivenlp/types/model.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-17 20:45:05.000000 intelmo-1.0.0/interactivenlp/types/server.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-05 18:36:10.288529 intelmo-1.0.0/interactivenlp/utils/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 intelmo-1.0.0/interactivenlp/utils/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      607 2023-07-27 01:11:10.000000 intelmo-1.0.0/interactivenlp/utils/extraction.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)       38 2023-08-05 18:36:10.288915 intelmo-1.0.0/setup.cfg
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1333 2023-08-05 18:35:41.000000 intelmo-1.0.0/setup.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:20:28.564512 intelmo-1.0.1/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      661 2023-08-07 23:20:28.564360 intelmo-1.0.1/PKG-INFO
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      376 2023-08-07 18:59:23.000000 intelmo-1.0.1/README.md
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:20:28.556784 intelmo-1.0.1/intelmo/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      218 2023-07-27 01:07:04.000000 intelmo-1.0.1/intelmo/__init__.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:20:28.559924 intelmo-1.0.1/intelmo/controllers/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 intelmo-1.0.1/intelmo/controllers/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     6828 2023-08-05 20:52:12.000000 intelmo-1.0.1/intelmo/controllers/reader_controller.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      818 2023-07-27 01:10:19.000000 intelmo-1.0.1/intelmo/controllers/rss_controller.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:20:28.561964 intelmo-1.0.1/intelmo/models/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 intelmo-1.0.1/intelmo/models/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      520 2023-08-03 23:26:35.000000 intelmo-1.0.1/intelmo/models/article.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     2199 2023-07-29 22:24:21.000000 intelmo-1.0.1/intelmo/models/block.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      868 2023-07-24 23:42:14.000000 intelmo-1.0.1/intelmo/models/form.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1027 2023-08-07 21:56:20.000000 intelmo-1.0.1/intelmo/models/rss.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     5260 2023-08-05 20:51:38.000000 intelmo-1.0.1/intelmo/models/task.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1034 2023-07-29 20:32:23.000000 intelmo-1.0.1/intelmo/server.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:20:28.562940 intelmo-1.0.1/intelmo/types/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 intelmo-1.0.1/intelmo/types/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     2579 2023-07-29 21:07:20.000000 intelmo-1.0.1/intelmo/types/model.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-17 20:45:05.000000 intelmo-1.0.1/intelmo/types/server.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:20:28.563930 intelmo-1.0.1/intelmo/utils/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 intelmo-1.0.1/intelmo/utils/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      607 2023-07-27 01:11:10.000000 intelmo-1.0.1/intelmo/utils/extraction.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:20:28.559184 intelmo-1.0.1/intelmo.egg-info/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      661 2023-08-07 23:20:28.000000 intelmo-1.0.1/intelmo.egg-info/PKG-INFO
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      593 2023-08-07 23:20:28.000000 intelmo-1.0.1/intelmo.egg-info/SOURCES.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-08-07 23:20:28.000000 intelmo-1.0.1/intelmo.egg-info/dependency_links.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       54 2023-08-07 23:20:28.000000 intelmo-1.0.1/intelmo.egg-info/requires.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        8 2023-08-07 23:20:28.000000 intelmo-1.0.1/intelmo.egg-info/top_level.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       38 2023-08-07 23:20:28.564597 intelmo-1.0.1/setup.cfg
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1327 2023-08-07 23:20:25.000000 intelmo-1.0.1/setup.py
```

### Comparing `intelmo-1.0.0/interactivenlp/controllers/reader_controller.py` & `intelmo-1.0.1/intelmo/controllers/reader_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,14 +156,15 @@
     return render_template('reader.html', **context)
 
 
 @reader_page.route('/set_form', methods=['POST'])
 def set_form():
     args = request.args
     function_id = args.get('id', default=None, type=str)
+    print(request.form.to_dict())
     function_forms[function_id] = request.form.to_dict()
     # return to the same page
     return redirect(request.referrer)
 
 
 @reader_page.route('/toggle_function')
 def toggle_function():
```

### Comparing `intelmo-1.0.0/interactivenlp/controllers/rss_controller.py` & `intelmo-1.0.1/intelmo/controllers/rss_controller.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.0/interactivenlp/models/article.py` & `intelmo-1.0.1/intelmo/models/article.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.0/interactivenlp/models/block.py` & `intelmo-1.0.1/intelmo/models/block.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.0/interactivenlp/models/form.py` & `intelmo-1.0.1/intelmo/models/form.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.0/interactivenlp/models/rss.py` & `intelmo-1.0.1/intelmo/models/rss.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,8 +41,7 @@
 
 class RSS:
     def __init__(self, id, name, url):
         self.id = id
         self.name = name
         self.url = url
         self.feed = parse(url)
-
```

### Comparing `intelmo-1.0.0/interactivenlp/models/task.py` & `intelmo-1.0.1/intelmo/models/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,15 +72,14 @@
             # [{"position": 1, "content": "hello world"}, {"position": 3, "content": "hello world"}]
             for index, paragraph in enumerate(old_paragraphs):
                 new_paragraphs.append(
                     Block(BlockLevelEnum.Paragraph, BlockTypeEnum.Normal, paragraph.content, None,
                           BlockStatusEnum.Untouched))
                 for insert_res in insert_func_res:
                     if insert_res["position"] == index:
-                        print("inserting", insert_res["position"], insert_res["content"])
                         new_paragraphs.append(
                             Block(BlockLevelEnum.Paragraph, BlockTypeEnum.Quote, insert_res["content"], None,
                                   BlockStatusEnum.New))
 
             new_article.blocks = new_paragraphs
             return new_article
```

### Comparing `intelmo-1.0.0/interactivenlp/server.py` & `intelmo-1.0.1/intelmo/server.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.0/interactivenlp/types/model.py` & `intelmo-1.0.1/intelmo/types/model.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.0/interactivenlp/utils/extraction.py` & `intelmo-1.0.1/intelmo/utils/extraction.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.0/setup.py` & `intelmo-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,43 +3,43 @@
 from setuptools.command.install import install
 
 
 class PostInstallCommand(install):
     """Post-installation for installation mode."""
 
     def run(self):
+        install.run(self)
         # Install nltk punkt
         import nltk
         nltk.download('punkt')
-        install.run(self)
 
 
 with open('README.md', "r") as f:
     long_description = f.read()
 
 print(find_packages(
-    exclude=["examples", "tests"],
+    exclude=["examples", "tests", "docs"],
 ))
 
 
 setup(
     name='intelmo',
-    version='1.0.0',
+    version='1.0.1',
     description='Interface Toolkit for Extensive Language Models',
     long_description=long_description,
     author="Chunxu Yang",
     author_email="chunxuyang@ucla.edu",
     # include_package_data=True,
     packages=find_packages(
         exclude=["examples", "tests"],
     ),
     include_package_data=True,
     package_data={
-        'templates': ["interactivenlp/templates/*"],
-        'static': ["interactivenlp/static/*"],
+        'templates': ["intelmo/templates/*"],
+        'static': ["intelmo/static/*"],
     },
     zipSafe=False,
     install_requires=[
         'flask',
         'flask-cors',
         'newspaper3k',
         'nltk',
```

