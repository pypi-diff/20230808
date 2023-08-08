# Comparing `tmp/tej-tool-api-1.0.6.tar.gz` & `tmp/tej-tool-api-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tej-tool-api-1.0.6.tar", last modified: Wed Jul 19 01:23:24 2023, max compression
+gzip compressed data, was "tej-tool-api-1.0.7.tar", last modified: Tue Aug  8 08:32:49 2023, max compression
```

## Comparing `tej-tool-api-1.0.6.tar` & `tej-tool-api-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 01:23:24.381233 tej-tool-api-1.0.6/
--rw-rw-rw-   0        0        0     5568 2023-07-19 01:23:24.381233 tej-tool-api-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5158 2023-07-19 01:23:01.000000 tej-tool-api-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 01:23:24.365580 tej-tool-api-1.0.6/TejTOolAPI/
--rw-rw-rw-   0        0        0      197 2023-05-19 07:13:38.000000 tej-tool-api-1.0.6/TejTOolAPI/Error.py
--rw-rw-rw-   0        0        0    17814 2023-07-19 01:08:13.000000 tej-tool-api-1.0.6/TejTOolAPI/Map_Dask_API.py
--rw-rw-rw-   0        0        0    11001 2023-07-19 01:08:13.000000 tej-tool-api-1.0.6/TejTOolAPI/TejToolAPI.py
--rw-rw-rw-   0        0        0      582 2023-07-10 09:13:18.000000 tej-tool-api-1.0.6/TejTOolAPI/__init__.py
--rw-rw-rw-   0        0        0     2329 2023-07-10 09:13:18.000000 tej-tool-api-1.0.6/TejTOolAPI/exchange_calendar.py
--rw-rw-rw-   0        0        0     1488 2023-07-12 03:01:58.000000 tej-tool-api-1.0.6/TejTOolAPI/parameters.py
-drwxrwxrwx   0        0        0        0 2023-07-19 01:23:24.349971 tej-tool-api-1.0.6/TejTOolAPI/tables/
--rw-rw-rw-   0        0        0    38860 2023-07-10 09:13:18.000000 tej-tool-api-1.0.6/TejTOolAPI/tables/columns_group.xlsx
--rw-rw-rw-   0        0        0   137941 2023-05-19 07:13:38.000000 tej-tool-api-1.0.6/TejTOolAPI/tables/mktboard.csv
--rw-rw-rw-   0        0        0       42 2023-07-19 01:23:24.381233 tej-tool-api-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1490 2023-07-19 01:23:21.000000 tej-tool-api-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 01:23:24.365580 tej-tool-api-1.0.6/tej_tool_api.egg-info/
--rw-rw-rw-   0        0        0     5568 2023-07-19 01:23:24.000000 tej-tool-api-1.0.6/tej_tool_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-07-19 01:23:24.000000 tej-tool-api-1.0.6/tej_tool_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 01:23:24.000000 tej-tool-api-1.0.6/tej_tool_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-07-19 01:23:24.000000 tej-tool-api-1.0.6/tej_tool_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-19 01:23:24.000000 tej-tool-api-1.0.6/tej_tool_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 08:32:49.902676 tej-tool-api-1.0.7/
+-rw-rw-rw-   0        0        0     5568 2023-08-08 08:32:49.902676 tej-tool-api-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5158 2023-07-19 01:23:01.000000 tej-tool-api-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 08:32:49.887069 tej-tool-api-1.0.7/TejTOolAPI/
+-rw-rw-rw-   0        0        0      197 2023-05-19 07:13:38.000000 tej-tool-api-1.0.7/TejTOolAPI/Error.py
+-rw-rw-rw-   0        0        0    17814 2023-07-19 01:08:13.000000 tej-tool-api-1.0.7/TejTOolAPI/Map_Dask_API.py
+-rw-rw-rw-   0        0        0    11001 2023-07-19 01:08:13.000000 tej-tool-api-1.0.7/TejTOolAPI/TejToolAPI.py
+-rw-rw-rw-   0        0        0      582 2023-07-10 09:13:18.000000 tej-tool-api-1.0.7/TejTOolAPI/__init__.py
+-rw-rw-rw-   0        0        0     2329 2023-07-10 09:13:18.000000 tej-tool-api-1.0.7/TejTOolAPI/exchange_calendar.py
+-rw-rw-rw-   0        0        0     1488 2023-07-12 03:01:58.000000 tej-tool-api-1.0.7/TejTOolAPI/parameters.py
+drwxrwxrwx   0        0        0        0 2023-08-08 08:32:49.871460 tej-tool-api-1.0.7/TejTOolAPI/tables/
+-rw-rw-rw-   0        0        0    38860 2023-07-10 09:13:18.000000 tej-tool-api-1.0.7/TejTOolAPI/tables/columns_group.xlsx
+-rw-rw-rw-   0        0        0   137941 2023-05-19 07:13:38.000000 tej-tool-api-1.0.7/TejTOolAPI/tables/mktboard.csv
+-rw-rw-rw-   0        0        0      165 2023-07-12 03:01:58.000000 tej-tool-api-1.0.7/TejTOolAPI/tables/~$columns_group.xlsx
+-rw-rw-rw-   0        0        0       42 2023-08-08 08:32:49.902676 tej-tool-api-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1518 2023-08-08 08:06:57.000000 tej-tool-api-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 08:32:49.887069 tej-tool-api-1.0.7/tej_tool_api.egg-info/
+-rw-rw-rw-   0        0        0     5568 2023-08-08 08:32:49.000000 tej-tool-api-1.0.7/tej_tool_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-08-08 08:32:49.000000 tej-tool-api-1.0.7/tej_tool_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 08:32:49.000000 tej-tool-api-1.0.7/tej_tool_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-08-08 08:32:49.000000 tej-tool-api-1.0.7/tej_tool_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-08-08 08:32:49.000000 tej-tool-api-1.0.7/tej_tool_api.egg-info/top_level.txt
```

### Comparing `tej-tool-api-1.0.6/PKG-INFO` & `tej-tool-api-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tej-tool-api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Package to fetch a large quantity of data from tejapi.
 Home-page: https://api.tej.com.tw
 Author: tej
 Author-email: tej@tej.com.tw
 Maintainer: tej api Development Team
 Maintainer-email: tej@tej.com
 License: MIT
```

### Comparing `tej-tool-api-1.0.6/README.md` & `tej-tool-api-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.6/TejTOolAPI/Map_Dask_API.py` & `tej-tool-api-1.0.7/TejTOolAPI/Map_Dask_API.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.6/TejTOolAPI/TejToolAPI.py` & `tej-tool-api-1.0.7/TejTOolAPI/TejToolAPI.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.6/TejTOolAPI/__init__.py` & `tej-tool-api-1.0.7/TejTOolAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.6/TejTOolAPI/exchange_calendar.py` & `tej-tool-api-1.0.7/TejTOolAPI/exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.6/TejTOolAPI/parameters.py` & `tej-tool-api-1.0.7/TejTOolAPI/parameters.py`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.6/TejTOolAPI/tables/columns_group.xlsx` & `tej-tool-api-1.0.7/TejTOolAPI/tables/columns_group.xlsx`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.6/TejTOolAPI/tables/mktboard.csv` & `tej-tool-api-1.0.7/TejTOolAPI/tables/mktboard.csv`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.6/setup.py` & `tej-tool-api-1.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 
   
 
 
 install_requires = [
     'dask == 2022.4.1',
     'pandas == 1.2.5',
-    'tejapi >= 0.1.23',
+    'tejapi >= 0.1.27',
     'xlrd >= 1.0.0',
     'openpyxl',
+    'fastparquet <=0.8.3',
 ]
 
 installs_for_two = [
     'pyOpenSSL',
     'ndg-httpsclient',
     'pyasn1'
 ]
@@ -33,15 +34,15 @@
 long_description = (this_directionary/"README.md").read_text(encoding='utf-8')
 setup(
     name='tej-tool-api',
     description='Package to fetch a large quantity of data from tejapi.',
     keywords=['tej', 'big data', 'data', 'financial', 'economic','stock','TEJ',],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.6',
+    version='1.0.7',
     author='tej',
     author_email='tej@tej.com.tw',
     maintainer='tej api Development Team',
     maintainer_email='tej@tej.com',
     url='https://api.tej.com.tw',
     license='MIT',
     install_requires=install_requires,
```

### Comparing `tej-tool-api-1.0.6/tej_tool_api.egg-info/PKG-INFO` & `tej-tool-api-1.0.7/tej_tool_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tej-tool-api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Package to fetch a large quantity of data from tejapi.
 Home-page: https://api.tej.com.tw
 Author: tej
 Author-email: tej@tej.com.tw
 Maintainer: tej api Development Team
 Maintainer-email: tej@tej.com
 License: MIT
```

