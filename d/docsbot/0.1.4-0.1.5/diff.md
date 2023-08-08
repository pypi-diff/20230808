# Comparing `tmp/docsbot-0.1.4.tar.gz` & `tmp/docsbot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docsbot-0.1.4.tar", last modified: Tue Aug  8 00:59:21 2023, max compression
+gzip compressed data, was "docsbot-0.1.5.tar", last modified: Tue Aug  8 01:05:47 2023, max compression
```

## Comparing `docsbot-0.1.4.tar` & `docsbot-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-08 00:59:21.777633 docsbot-0.1.4/
--rw-r--r--   0 jeffrey    (501) staff       (20)     4818 2023-08-08 00:59:21.777522 docsbot-0.1.4/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)     4629 2023-08-04 13:20:17.000000 docsbot-0.1.4/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-08 00:59:21.777381 docsbot-0.1.4/docsbot.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)     4818 2023-08-08 00:59:21.000000 docsbot-0.1.4/docsbot.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)      206 2023-08-08 00:59:21.000000 docsbot-0.1.4/docsbot.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-08 00:59:21.000000 docsbot-0.1.4/docsbot.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       37 2023-08-08 00:59:21.000000 docsbot-0.1.4/docsbot.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       80 2023-08-08 00:59:21.000000 docsbot-0.1.4/docsbot.egg-info/requires.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-08 00:59:21.000000 docsbot-0.1.4/docsbot.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-08-08 00:59:21.777665 docsbot-0.1.4/setup.cfg
--rw-r--r--   0 jeffrey    (501) staff       (20)      667 2023-08-08 00:59:06.000000 docsbot-0.1.4/setup.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-08 01:05:47.994429 docsbot-0.1.5/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4821 2023-08-08 01:05:47.994324 docsbot-0.1.5/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4629 2023-08-04 13:20:17.000000 docsbot-0.1.5/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-08 01:05:47.994188 docsbot-0.1.5/docsbot.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4821 2023-08-08 01:05:47.000000 docsbot-0.1.5/docsbot.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)      206 2023-08-08 01:05:47.000000 docsbot-0.1.5/docsbot.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-08 01:05:47.000000 docsbot-0.1.5/docsbot.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       37 2023-08-08 01:05:47.000000 docsbot-0.1.5/docsbot.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       87 2023-08-08 01:05:47.000000 docsbot-0.1.5/docsbot.egg-info/requires.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-08 01:05:47.000000 docsbot-0.1.5/docsbot.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-08-08 01:05:47.994460 docsbot-0.1.5/setup.cfg
+-rw-r--r--   0 jeffrey    (501) staff       (20)      677 2023-08-08 01:05:46.000000 docsbot-0.1.5/setup.py
```

### Comparing `docsbot-0.1.4/PKG-INFO` & `docsbot-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: docsbot
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple chat bot for querying information from your local private documents.
-Author: J
+Author: Jeff
 Description-Content-Type: text/markdown
 
 # DocsBot 使用说明
 
 DocsBot 是一个命令行工具，提供了方便的方式来管理和查询你的资料库。
 
 ## 快速开始 Quick Start
```

### Comparing `docsbot-0.1.4/README.md` & `docsbot-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `docsbot-0.1.4/docsbot.egg-info/PKG-INFO` & `docsbot-0.1.5/docsbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: docsbot
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple chat bot for querying information from your local private documents.
-Author: J
+Author: Jeff
 Description-Content-Type: text/markdown
 
 # DocsBot 使用说明
 
 DocsBot 是一个命令行工具，提供了方便的方式来管理和查询你的资料库。
 
 ## 快速开始 Quick Start
```

### Comparing `docsbot-0.1.4/setup.py` & `docsbot-0.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name='docsbot',
-    version='0.1.4',
+    version='0.1.5',
     description='A simple chat bot for querying information from your local private documents.',
-    author='J',
+    author='Jeff',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         'console_scripts': [
             'docsbot = cli:main',
         ]
     },
     install_requires = [
-        "chromadb",
+        "chromadb==0.4.5",
         "prettytable",
         "langchain",
         "qdrant-client",
         "unstructured_inference",
         "pytesseract",
     ]
 )
```

