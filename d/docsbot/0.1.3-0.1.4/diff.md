# Comparing `tmp/docsbot-0.1.3.tar.gz` & `tmp/docsbot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docsbot-0.1.3.tar", last modified: Sun Aug  6 04:18:33 2023, max compression
+gzip compressed data, was "docsbot-0.1.4.tar", last modified: Tue Aug  8 00:59:21 2023, max compression
```

## Comparing `docsbot-0.1.3.tar` & `docsbot-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-06 04:18:33.289890 docsbot-0.1.3/
--rw-r--r--   0 jeffrey    (501) staff       (20)     4818 2023-08-06 04:18:33.289774 docsbot-0.1.3/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)     4629 2023-08-04 13:20:17.000000 docsbot-0.1.3/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-06 04:18:33.289628 docsbot-0.1.3/docsbot.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)     4818 2023-08-06 04:18:33.000000 docsbot-0.1.3/docsbot.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)      206 2023-08-06 04:18:33.000000 docsbot-0.1.3/docsbot.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-06 04:18:33.000000 docsbot-0.1.3/docsbot.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       37 2023-08-06 04:18:33.000000 docsbot-0.1.3/docsbot.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       80 2023-08-06 04:18:33.000000 docsbot-0.1.3/docsbot.egg-info/requires.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-06 04:18:33.000000 docsbot-0.1.3/docsbot.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-08-06 04:18:33.289919 docsbot-0.1.3/setup.cfg
--rw-r--r--   0 jeffrey    (501) staff       (20)      667 2023-08-06 04:18:32.000000 docsbot-0.1.3/setup.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-08 00:59:21.777633 docsbot-0.1.4/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4818 2023-08-08 00:59:21.777522 docsbot-0.1.4/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4629 2023-08-04 13:20:17.000000 docsbot-0.1.4/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-08 00:59:21.777381 docsbot-0.1.4/docsbot.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4818 2023-08-08 00:59:21.000000 docsbot-0.1.4/docsbot.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)      206 2023-08-08 00:59:21.000000 docsbot-0.1.4/docsbot.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-08 00:59:21.000000 docsbot-0.1.4/docsbot.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       37 2023-08-08 00:59:21.000000 docsbot-0.1.4/docsbot.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       80 2023-08-08 00:59:21.000000 docsbot-0.1.4/docsbot.egg-info/requires.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-08 00:59:21.000000 docsbot-0.1.4/docsbot.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-08-08 00:59:21.777665 docsbot-0.1.4/setup.cfg
+-rw-r--r--   0 jeffrey    (501) staff       (20)      667 2023-08-08 00:59:06.000000 docsbot-0.1.4/setup.py
```

### Comparing `docsbot-0.1.3/PKG-INFO` & `docsbot-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docsbot
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple chat bot for querying information from your local private documents.
 Author: J
 Description-Content-Type: text/markdown
 
 # DocsBot 使用说明
 
 DocsBot 是一个命令行工具，提供了方便的方式来管理和查询你的资料库。
```

### Comparing `docsbot-0.1.3/README.md` & `docsbot-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `docsbot-0.1.3/docsbot.egg-info/PKG-INFO` & `docsbot-0.1.4/docsbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docsbot
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple chat bot for querying information from your local private documents.
 Author: J
 Description-Content-Type: text/markdown
 
 # DocsBot 使用说明
 
 DocsBot 是一个命令行工具，提供了方便的方式来管理和查询你的资料库。
```

