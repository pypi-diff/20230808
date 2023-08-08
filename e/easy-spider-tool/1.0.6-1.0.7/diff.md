# Comparing `tmp/easy_spider_tool-1.0.6.tar.gz` & `tmp/easy_spider_tool-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\easy_spider_tool-1.0.6.tar", last modified: Sat Jul  1 11:35:45 2023, max compression
+gzip compressed data, was "dist\easy_spider_tool-1.0.7.tar", last modified: Tue Aug  8 14:30:42 2023, max compression
```

## Comparing `easy_spider_tool-1.0.6.tar` & `easy_spider_tool-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 11:35:45.000000 easy_spider_tool-1.0.6/
--rw-rw-rw-   0        0        0     1088 2023-06-07 06:20:35.000000 easy_spider_tool-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     2826 2023-07-01 11:35:45.000000 easy_spider_tool-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2550 2023-06-07 06:29:39.000000 easy_spider_tool-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 11:35:45.000000 easy_spider_tool-1.0.6/easy_spider_tool/
--rw-rw-rw-   0        0        0      381 2023-07-01 11:17:32.000000 easy_spider_tool-1.0.6/easy_spider_tool/__init__.py
--rw-rw-rw-   0        0        0      702 2023-06-07 06:18:05.000000 easy_spider_tool-1.0.6/easy_spider_tool/data.py
--rw-rw-rw-   0        0        0    17323 2023-06-07 06:18:05.000000 easy_spider_tool-1.0.6/easy_spider_tool/date.py
--rw-rw-rw-   0        0        0     1208 2023-06-07 06:18:05.000000 easy_spider_tool-1.0.6/easy_spider_tool/decorator.py
--rw-rw-rw-   0        0        0      290 2023-06-07 06:18:05.000000 easy_spider_tool-1.0.6/easy_spider_tool/hash.py
--rw-rw-rw-   0        0        0     1813 2023-07-01 11:34:11.000000 easy_spider_tool-1.0.6/easy_spider_tool/jsons.py
--rw-rw-rw-   0        0        0      624 2023-06-07 06:18:05.000000 easy_spider_tool-1.0.6/easy_spider_tool/re.py
--rw-rw-rw-   0        0        0      114 2023-06-07 06:18:05.000000 easy_spider_tool-1.0.6/easy_spider_tool/types.py
--rw-rw-rw-   0        0        0     1943 2023-06-07 06:18:05.000000 easy_spider_tool-1.0.6/easy_spider_tool/verify.py
-drwxrwxrwx   0        0        0        0 2023-07-01 11:35:45.000000 easy_spider_tool-1.0.6/easy_spider_tool.egg-info/
--rw-rw-rw-   0        0        0     2826 2023-07-01 11:35:45.000000 easy_spider_tool-1.0.6/easy_spider_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-07-01 11:35:45.000000 easy_spider_tool-1.0.6/easy_spider_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 11:35:45.000000 easy_spider_tool-1.0.6/easy_spider_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-01 11:35:45.000000 easy_spider_tool-1.0.6/easy_spider_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-01 11:35:45.000000 easy_spider_tool-1.0.6/easy_spider_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 11:35:45.000000 easy_spider_tool-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      595 2023-07-01 11:35:36.000000 easy_spider_tool-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 14:30:42.000000 easy_spider_tool-1.0.7/
+-rw-rw-rw-   0        0        0     1088 2023-06-07 06:20:35.000000 easy_spider_tool-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2826 2023-08-08 14:30:42.000000 easy_spider_tool-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2550 2023-06-07 06:29:39.000000 easy_spider_tool-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 14:30:42.000000 easy_spider_tool-1.0.7/easy_spider_tool/
+-rw-rw-rw-   0        0        0      381 2023-07-01 11:17:32.000000 easy_spider_tool-1.0.7/easy_spider_tool/__init__.py
+-rw-rw-rw-   0        0        0      702 2023-06-07 06:18:05.000000 easy_spider_tool-1.0.7/easy_spider_tool/data.py
+-rw-rw-rw-   0        0        0    17323 2023-06-07 06:18:05.000000 easy_spider_tool-1.0.7/easy_spider_tool/date.py
+-rw-rw-rw-   0        0        0     1208 2023-06-07 06:18:05.000000 easy_spider_tool-1.0.7/easy_spider_tool/decorator.py
+-rw-rw-rw-   0        0        0      290 2023-06-07 06:18:05.000000 easy_spider_tool-1.0.7/easy_spider_tool/hash.py
+-rw-rw-rw-   0        0        0     1813 2023-07-01 11:34:11.000000 easy_spider_tool-1.0.7/easy_spider_tool/jsons.py
+-rw-rw-rw-   0        0        0      624 2023-06-07 06:18:05.000000 easy_spider_tool-1.0.7/easy_spider_tool/re.py
+-rw-rw-rw-   0        0        0      114 2023-06-07 06:18:05.000000 easy_spider_tool-1.0.7/easy_spider_tool/types.py
+-rw-rw-rw-   0        0        0     1943 2023-06-07 06:18:05.000000 easy_spider_tool-1.0.7/easy_spider_tool/verify.py
+drwxrwxrwx   0        0        0        0 2023-08-08 14:30:42.000000 easy_spider_tool-1.0.7/easy_spider_tool.egg-info/
+-rw-rw-rw-   0        0        0     2826 2023-08-08 14:30:41.000000 easy_spider_tool-1.0.7/easy_spider_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2023-08-08 14:30:41.000000 easy_spider_tool-1.0.7/easy_spider_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 14:30:41.000000 easy_spider_tool-1.0.7/easy_spider_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-08 14:30:41.000000 easy_spider_tool-1.0.7/easy_spider_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-08 14:30:41.000000 easy_spider_tool-1.0.7/easy_spider_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 14:30:42.000000 easy_spider_tool-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      595 2023-08-08 14:30:31.000000 easy_spider_tool-1.0.7/setup.py
```

### Comparing `easy_spider_tool-1.0.6/LICENSE` & `easy_spider_tool-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_spider_tool-1.0.6/PKG-INFO` & `easy_spider_tool-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_spider_tool
-Version: 1.0.6
+Version: 1.0.7
 Summary: 简易、好用的爬虫工具,减少重复代码与文件冗余
 Author: hanxinkong
 Author-email: xinkonghan@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `easy_spider_tool-1.0.6/README.md` & `easy_spider_tool-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `easy_spider_tool-1.0.6/easy_spider_tool/data.py` & `easy_spider_tool-1.0.7/easy_spider_tool/data.py`

 * *Files identical despite different names*

### Comparing `easy_spider_tool-1.0.6/easy_spider_tool/date.py` & `easy_spider_tool-1.0.7/easy_spider_tool/date.py`

 * *Files identical despite different names*

### Comparing `easy_spider_tool-1.0.6/easy_spider_tool/decorator.py` & `easy_spider_tool-1.0.7/easy_spider_tool/decorator.py`

 * *Files identical despite different names*

### Comparing `easy_spider_tool-1.0.6/easy_spider_tool/jsons.py` & `easy_spider_tool-1.0.7/easy_spider_tool/jsons.py`

 * *Files identical despite different names*

### Comparing `easy_spider_tool-1.0.6/easy_spider_tool/re.py` & `easy_spider_tool-1.0.7/easy_spider_tool/re.py`

 * *Files identical despite different names*

### Comparing `easy_spider_tool-1.0.6/easy_spider_tool/verify.py` & `easy_spider_tool-1.0.7/easy_spider_tool/verify.py`

 * *Files identical despite different names*

### Comparing `easy_spider_tool-1.0.6/easy_spider_tool.egg-info/PKG-INFO` & `easy_spider_tool-1.0.7/easy_spider_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-spider-tool
-Version: 1.0.6
+Version: 1.0.7
 Summary: 简易、好用的爬虫工具,减少重复代码与文件冗余
 Author: hanxinkong
 Author-email: xinkonghan@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `easy_spider_tool-1.0.6/setup.py` & `easy_spider_tool-1.0.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='easy_spider_tool',
-    version='1.0.06',
+    version='1.0.07',
     packages=find_packages(),
     license='MIT',
     author='hanxinkong',
     author_email='xinkonghan@gmail.com',
     description='简易、好用的爬虫工具,减少重复代码与文件冗余',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     install_requires=[
         # List your package's dependencies here
-        "dateparser>=1.1.8",
+        "dateparser>=1.1.3",
         "jsonpath>=0.82",
         "pytz>=2023.3"
     ],
 )
```

