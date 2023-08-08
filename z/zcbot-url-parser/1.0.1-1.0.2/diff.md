# Comparing `tmp/zcbot-url-parser-1.0.1.tar.gz` & `tmp/zcbot-url-parser-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zcbot-url-parser-1.0.1.tar", last modified: Thu Jul 27 05:02:08 2023, max compression
+gzip compressed data, was "dist\zcbot-url-parser-1.0.2.tar", last modified: Tue Aug  8 04:02:55 2023, max compression
```

## Comparing `zcbot-url-parser-1.0.1.tar` & `zcbot-url-parser-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 05:02:08.695875 zcbot-url-parser-1.0.1/
--rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-url-parser-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      379 2023-07-27 05:02:08.694875 zcbot-url-parser-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      135 2023-05-30 07:06:49.000000 zcbot-url-parser-1.0.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-27 05:02:08.695875 zcbot-url-parser-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      591 2023-07-27 05:01:28.000000 zcbot-url-parser-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 05:02:08.685878 zcbot-url-parser-1.0.1/zcbot_url_parser/
--rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-url-parser-1.0.1/zcbot_url_parser/__init__.py
--rw-rw-rw-   0        0        0      604 2023-07-27 04:57:32.000000 zcbot-url-parser-1.0.1/zcbot_url_parser/constant.py
--rw-rw-rw-   0        0        0     3531 2023-07-27 04:00:15.000000 zcbot-url-parser-1.0.1/zcbot_url_parser/parser.py
--rw-rw-rw-   0        0        0     2935 2023-07-27 04:49:25.000000 zcbot-url-parser-1.0.1/zcbot_url_parser/rule.py
--rw-rw-rw-   0        0        0     3511 2023-07-27 04:59:09.000000 zcbot-url-parser-1.0.1/zcbot_url_parser/spider.py
--rw-rw-rw-   0        0        0      597 2023-07-27 03:12:39.000000 zcbot-url-parser-1.0.1/zcbot_url_parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 05:02:08.692874 zcbot-url-parser-1.0.1/zcbot_url_parser.egg-info/
--rw-rw-rw-   0        0        0      379 2023-07-27 05:02:08.000000 zcbot-url-parser-1.0.1/zcbot_url_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-07-27 05:02:08.000000 zcbot-url-parser-1.0.1/zcbot_url_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 05:02:08.000000 zcbot-url-parser-1.0.1/zcbot_url_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-27 05:02:08.000000 zcbot-url-parser-1.0.1/zcbot_url_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-27 05:02:08.000000 zcbot-url-parser-1.0.1/zcbot_url_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 04:02:55.445649 zcbot-url-parser-1.0.2/
+-rw-rw-rw-   0        0        0        0 2023-06-12 03:07:51.000000 zcbot-url-parser-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      424 2023-08-08 04:02:55.445649 zcbot-url-parser-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      135 2023-06-12 03:07:51.000000 zcbot-url-parser-1.0.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-08 04:02:55.445649 zcbot-url-parser-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-08-08 03:48:09.000000 zcbot-url-parser-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 04:02:55.438604 zcbot-url-parser-1.0.2/zcbot_url_parser/
+-rw-rw-rw-   0        0        0       40 2023-06-12 03:07:51.000000 zcbot-url-parser-1.0.2/zcbot_url_parser/__init__.py
+-rw-rw-rw-   0        0        0      604 2023-08-03 07:56:52.000000 zcbot-url-parser-1.0.2/zcbot_url_parser/constant.py
+-rw-rw-rw-   0        0        0     3538 2023-08-08 03:47:02.000000 zcbot-url-parser-1.0.2/zcbot_url_parser/parser.py
+-rw-rw-rw-   0        0        0     2935 2023-08-03 07:56:52.000000 zcbot-url-parser-1.0.2/zcbot_url_parser/rule.py
+-rw-rw-rw-   0        0        0     3511 2023-08-03 07:56:52.000000 zcbot-url-parser-1.0.2/zcbot_url_parser/spider.py
+-rw-rw-rw-   0        0        0      597 2023-08-03 07:56:52.000000 zcbot-url-parser-1.0.2/zcbot_url_parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-08 04:02:55.443642 zcbot-url-parser-1.0.2/zcbot_url_parser.egg-info/
+-rw-rw-rw-   0        0        0      424 2023-08-08 04:02:55.000000 zcbot-url-parser-1.0.2/zcbot_url_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-08-08 04:02:55.000000 zcbot-url-parser-1.0.2/zcbot_url_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 04:02:55.000000 zcbot-url-parser-1.0.2/zcbot_url_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-08 04:02:55.000000 zcbot-url-parser-1.0.2/zcbot_url_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-08 04:02:55.000000 zcbot-url-parser-1.0.2/zcbot_url_parser.egg-info/top_level.txt
```

### Comparing `zcbot-url-parser-1.0.1/setup.py` & `zcbot-url-parser-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(name='zcbot-url-parser',
-      version='1.0.1',
+      version='1.0.2',
       description='zcbot url parser for zsodata',
       long_description=long_description,
       author='zsodata',
       author_email='team@zso.io',
       url='http://www.zsodata.com',
       install_requires=['pymongo'],
       python_requires='>=3.7',
```

### Comparing `zcbot-url-parser-1.0.1/zcbot_url_parser/constant.py` & `zcbot-url-parser-1.0.2/zcbot_url_parser/constant.py`

 * *Files identical despite different names*

### Comparing `zcbot-url-parser-1.0.1/zcbot_url_parser/parser.py` & `zcbot-url-parser-1.0.2/zcbot_url_parser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,12 +114,12 @@
             for param in sku_param:
                 if param in params and params.get(param)[0].strip():
                     rs_list.append(str(params.get(param)[0].strip()))
 
             if token:
                 return token.join(rs_list)
             else:
-                return rs_list
+                return tuple(rs_list)
     except Exception as e:
         LOGGER.error('match sku error[parse_sku_by_param]: url=%s, ex=%s' % (url, e))
 
     return ''
```

### Comparing `zcbot-url-parser-1.0.1/zcbot_url_parser/rule.py` & `zcbot-url-parser-1.0.2/zcbot_url_parser/rule.py`

 * *Files identical despite different names*

### Comparing `zcbot-url-parser-1.0.1/zcbot_url_parser/spider.py` & `zcbot-url-parser-1.0.2/zcbot_url_parser/spider.py`

 * *Files identical despite different names*

### Comparing `zcbot-url-parser-1.0.1/zcbot_url_parser/utils.py` & `zcbot-url-parser-1.0.2/zcbot_url_parser/utils.py`

 * *Files identical despite different names*

