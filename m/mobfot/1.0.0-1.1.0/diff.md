# Comparing `tmp/mobfot-1.0.0.tar.gz` & `tmp/mobfot-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobfot-1.0.0.tar", last modified: Thu Dec  8 05:51:52 2022, max compression
+gzip compressed data, was "mobfot-1.1.0.tar", last modified: Tue Aug  8 00:07:42 2023, max compression
```

## Comparing `mobfot-1.0.0.tar` & `mobfot-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 05:51:52.507468 mobfot-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2022-12-08 05:51:40.000000 mobfot-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2022-12-08 05:51:52.507468 mobfot-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      977 2022-12-08 05:51:40.000000 mobfot-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 05:51:52.503468 mobfot-1.0.0/mobfot/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-08 05:51:40.000000 mobfot-1.0.0/mobfot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2022-12-08 05:51:40.000000 mobfot-1.0.0/mobfot/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 05:51:52.507468 mobfot-1.0.0/mobfot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2022-12-08 05:51:52.000000 mobfot-1.0.0/mobfot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2022-12-08 05:51:52.000000 mobfot-1.0.0/mobfot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 05:51:52.000000 mobfot-1.0.0/mobfot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-08 05:51:52.000000 mobfot-1.0.0/mobfot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-08 05:51:52.000000 mobfot-1.0.0/mobfot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2022-12-08 05:51:40.000000 mobfot-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 05:51:52.507468 mobfot-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:07:42.126423 mobfot-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-08 00:07:32.000000 mobfot-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-08-08 00:07:42.126423 mobfot-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-08 00:07:32.000000 mobfot-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:07:42.126423 mobfot-1.1.0/mobfot/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 00:07:32.000000 mobfot-1.1.0/mobfot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-08-08 00:07:32.000000 mobfot-1.1.0/mobfot/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:07:42.126423 mobfot-1.1.0/mobfot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-08-08 00:07:42.000000 mobfot-1.1.0/mobfot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-08 00:07:42.000000 mobfot-1.1.0/mobfot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 00:07:42.000000 mobfot-1.1.0/mobfot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-08 00:07:42.000000 mobfot-1.1.0/mobfot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 00:07:42.000000 mobfot-1.1.0/mobfot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-08 00:07:32.000000 mobfot-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 00:07:42.126423 mobfot-1.1.0/setup.cfg
```

### Comparing `mobfot-1.0.0/LICENSE` & `mobfot-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mobfot-1.0.0/PKG-INFO` & `mobfot-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: mobfot
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python wrapper around the unofficial FotMob API
 Author: Brian Greenwood
 License: MIT
-Project-URL: Homepage, https://github.com/bgrnwd/mobfot
+Project-URL: homepage, https://github.com/bgrnwd/mobfot
+Project-URL: repository, https://github.com/bgrnwd/mobfot
 Keywords: fotmob,soccer,api,football
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -16,23 +17,24 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # mobfot
 
 [![license](https://img.shields.io/github/license/bgrnwd/mobfot.svg)](LICENSE)
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
 ![pypi](https://img.shields.io/pypi/v/mobfot?color=green)
+[![PyPI download month](https://img.shields.io/pypi/dm/mobfot.svg)](https://pypi.python.org/pypi/mobfot/)
 ![Python CI](https://github.com/bgrnwd/mobfot/workflows/Python%20CI/badge.svg)
 
 A Python wrapper around the unofficial [FotMob](https://www.fotmob.com/) API
 
 ## Table of Contents
 
 - [mobfot](#mobfot)
```

### Comparing `mobfot-1.0.0/README.md` & `mobfot-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # mobfot
 
 [![license](https://img.shields.io/github/license/bgrnwd/mobfot.svg)](LICENSE)
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
 ![pypi](https://img.shields.io/pypi/v/mobfot?color=green)
+[![PyPI download month](https://img.shields.io/pypi/dm/mobfot.svg)](https://pypi.python.org/pypi/mobfot/)
 ![Python CI](https://github.com/bgrnwd/mobfot/workflows/Python%20CI/badge.svg)
 
 A Python wrapper around the unofficial [FotMob](https://www.fotmob.com/) API
 
 ## Table of Contents
 
 - [mobfot](#mobfot)
```

### Comparing `mobfot-1.0.0/mobfot/client.py` & `mobfot-1.1.0/mobfot/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re
+import urllib.parse
 from logging import getLevelName, getLogger
 from typing import Optional, Union
 
 import requests
 from cachecontrol import CacheControl
 
-VERSION = "1.0.0"
+VERSION = "1.1.0"
 
 
 class MobFot:
     BASE_URL = "https://www.fotmob.com/api"
     LOGGER = getLogger(__name__)
 
     def __init__(
@@ -34,15 +35,17 @@
 
         self.session = CACHE_SESSION
         self.matches_url = f"{self.BASE_URL}/matches?"
         self.leagues_url = f"{self.BASE_URL}/leagues?"
         self.teams_url = f"{self.BASE_URL}/teams?"
         self.player_url = f"{self.BASE_URL}/playerData?"
         self.match_details_url = f"{self.BASE_URL}/matchDetails?"
-        self.search_url = f"{self.BASE_URL}/searchapi/"
+        self.search_url = f"{self.BASE_URL}/searchData?"
+        self.tv_listing_url = f"{self.BASE_URL}/tvlisting?"
+        self.tv_listings_url = f"{self.BASE_URL}/tvlistings?"
 
     def _check_date(self, date: str) -> Union[re.Match, None]:
         pattern = re.compile(r"(20\d{2})(\d{2})(\d{2})")
         return pattern.match(date)
 
     def _execute_query(self, url: str):
         response = self.session.get(url)
@@ -79,7 +82,20 @@
     def get_player(self, id: int):
         url = f"{self.player_url}id={id}"
         return self._execute_query(url)
 
     def get_match_details(self, match_id: int):
         url = f"{self.match_details_url}matchId={match_id}"
         return self._execute_query(url)
+
+    def get_match_tv_listing(self, match_id: int, country_code: str = "GB"):
+        url = f"{self.tv_listing_url}matchId={match_id}&countryCode={country_code}"
+        return self._execute_query(url)
+
+    def get_tv_listings_country(self, country_code: str = "GB"):
+        url = f"{self.tv_listings_url}countryCode={country_code}"
+        return self._execute_query(url)
+
+    def search(self, term: str, user_language: str = "en-GB,en"):
+        searchterm = urllib.parse.quote_plus(term)
+        url = f"{self.search_url}term={searchterm}&userLanguage={user_language}"
+        return self._execute_query(url)
```

### Comparing `mobfot-1.0.0/mobfot.egg-info/PKG-INFO` & `mobfot-1.1.0/mobfot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: mobfot
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python wrapper around the unofficial FotMob API
 Author: Brian Greenwood
 License: MIT
-Project-URL: Homepage, https://github.com/bgrnwd/mobfot
+Project-URL: homepage, https://github.com/bgrnwd/mobfot
+Project-URL: repository, https://github.com/bgrnwd/mobfot
 Keywords: fotmob,soccer,api,football
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -16,23 +17,24 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # mobfot
 
 [![license](https://img.shields.io/github/license/bgrnwd/mobfot.svg)](LICENSE)
 [![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
 ![pypi](https://img.shields.io/pypi/v/mobfot?color=green)
+[![PyPI download month](https://img.shields.io/pypi/dm/mobfot.svg)](https://pypi.python.org/pypi/mobfot/)
 ![Python CI](https://github.com/bgrnwd/mobfot/workflows/Python%20CI/badge.svg)
 
 A Python wrapper around the unofficial [FotMob](https://www.fotmob.com/) API
 
 ## Table of Contents
 
 - [mobfot](#mobfot)
```

### Comparing `mobfot-1.0.0/pyproject.toml` & `mobfot-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mobfot"
 description = "A Python wrapper around the unofficial FotMob API"
+readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">=3.7"
 authors = [
   { name = "Brian Greenwood" },
 ]
 keywords = [
-   	"fotmob",
+    "fotmob",
     "soccer",
     "api",
     "football"
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
@@ -31,37 +32,37 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-	"requests==2.28.1",
-	"CacheControl==0.12.11"
+  "requests==2.31.0",
+  "CacheControl==0.13.1"
 ]
-dynamic = ["readme", "version"]
+dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
     "black",
     "mypy",
     "isort",
     "behave",
     "reformat-gherkin",
     "types-requests"
 ]
 
 [project.urls]
-Homepage = "https://github.com/bgrnwd/mobfot"
+homepage = "https://github.com/bgrnwd/mobfot"
+repository = "https://github.com/bgrnwd/mobfot"
 
 [tool.isort]
 atomic = true
 line_length = 88
 skip_gitignore = true
 
 [tool.setuptools.dynamic]
 version = {attr = "mobfot.client.VERSION"}
-readme = {file = ["README.md"]}
 
 [[tool.mypy.overrides]]
 module = "cachecontrol.*"
 ignore_missing_imports = true
```

