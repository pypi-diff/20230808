# Comparing `tmp/nbcpu-0.6.0.tar.gz` & `tmp/nbcpu-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbcpu-0.6.0.tar", max compression
+gzip compressed data, was "nbcpu-0.7.0.tar", max compression
```

## Comparing `nbcpu-0.6.0.tar` & `nbcpu-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1071 2023-08-04 09:10:49.582825 nbcpu-0.6.0/LICENSE
--rw-r--r--   0        0        0     3306 2023-08-04 09:10:49.582825 nbcpu-0.6.0/README.md
--rw-r--r--   0        0        0     3006 2023-08-04 09:11:22.114725 nbcpu-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      180 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/__cli__.py
--rw-r--r--   0        0        0      484 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/__init__.py
--rw-r--r--   0        0        0       22 2023-08-04 09:11:22.070725 nbcpu-0.6.0/src/nbcpu/_version.py
--rw-r--r--   0        0        0        0 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/conf/__init__.py
--rw-r--r--   0        0        0      275 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/conf/about/nbcpu.yaml
--rw-r--r--   0        0        0      676 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/conf/fetcher/khmer.yaml
--rw-r--r--   0        0        0      698 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/conf/fetcher/phnompenh.yaml
--rw-r--r--   0        0        0        0 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/fetcher/__init__.py
--rw-r--r--   0        0        0    11793 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/fetcher/base.py
--rw-r--r--   0        0        0     4049 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/fetcher/khmer.py
--rw-r--r--   0        0        0     4704 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/fetcher/phnompenh.py
--rw-r--r--   0        0        0        0 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/py.typed
--rw-r--r--   0        0        0     4091 1970-01-01 00:00:00.000000 nbcpu-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-08 19:07:05.180958 nbcpu-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3306 2023-08-08 19:07:05.180958 nbcpu-0.7.0/README.md
+-rw-r--r--   0        0        0     3006 2023-08-08 19:07:37.733461 nbcpu-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      180 2023-08-08 19:07:05.184958 nbcpu-0.7.0/src/nbcpu/__cli__.py
+-rw-r--r--   0        0        0      484 2023-08-08 19:07:05.184958 nbcpu-0.7.0/src/nbcpu/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-08 19:07:37.689460 nbcpu-0.7.0/src/nbcpu/_version.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:07:05.184958 nbcpu-0.7.0/src/nbcpu/conf/__init__.py
+-rw-r--r--   0        0        0      275 2023-08-08 19:07:05.184958 nbcpu-0.7.0/src/nbcpu/conf/about/nbcpu.yaml
+-rw-r--r--   0        0        0      675 2023-08-08 19:07:05.184958 nbcpu-0.7.0/src/nbcpu/conf/fetcher/khmer.yaml
+-rw-r--r--   0        0        0      698 2023-08-08 19:07:05.184958 nbcpu-0.7.0/src/nbcpu/conf/fetcher/phnompenh.yaml
+-rw-r--r--   0        0        0        0 2023-08-08 19:07:05.184958 nbcpu-0.7.0/src/nbcpu/fetcher/__init__.py
+-rw-r--r--   0        0        0    11793 2023-08-08 19:07:05.184958 nbcpu-0.7.0/src/nbcpu/fetcher/base.py
+-rw-r--r--   0        0        0     4049 2023-08-08 19:07:05.184958 nbcpu-0.7.0/src/nbcpu/fetcher/khmer.py
+-rw-r--r--   0        0        0     4704 2023-08-08 19:07:05.184958 nbcpu-0.7.0/src/nbcpu/fetcher/phnompenh.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:07:05.184958 nbcpu-0.7.0/src/nbcpu/py.typed
+-rw-r--r--   0        0        0     4091 1970-01-01 00:00:00.000000 nbcpu-0.7.0/PKG-INFO
```

### Comparing `nbcpu-0.6.0/LICENSE` & `nbcpu-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nbcpu-0.6.0/README.md` & `nbcpu-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `nbcpu-0.6.0/pyproject.toml` & `nbcpu-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "nbcpu"
-version = "0.6.0"
+version = "0.7.0"
 description = "Quantifying Central Bank Policy Uncertainty in a Highly Dollarized Economy: A Topic Modeling Approach"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.github.io/nbcpu"
 repository = "https://github.com/entelecheia/nbcpu"
 readme = "README.md"
 packages = [{ include = "nbcpu", from = "src" }]
 
 [tool.poetry.scripts]
 nbcpu = 'nbcpu.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 click = "^8.1.3"
-hyfi = "^1.18.1"
+hyfi = "^1.25.0"
 # hyfi = { path = "../hyfi", develop = true }
-lexikanon = "^0.4.2"
+lexikanon = "^0.5.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `nbcpu-0.6.0/src/nbcpu/conf/fetcher/khmer.yaml` & `nbcpu-0.7.0/src/nbcpu/conf/fetcher/phnompenh.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-_target_: nbcpu.fetcher.khmer.KhmerFetcher
-_config_name_: khmer
+_target_: nbcpu.fetcher.phnompenh.PhnompenhFetcher
+_config_name_: phnompenh
 _config_group_: /fetcher
-search_url: https://www.khmertimeskh.com/page/{page}/?s={keyword}
+search_url: https://phnompenhpost.com/search/node/{keyword}?page={page}
 search_keywords:
 - NBC
 - Exchange Rate
 - De-dollarization
 - Inflation
 - GDP
 - Monetary Policy
@@ -17,19 +17,19 @@
 - Policy
 - Financial
 - Riel
 - Bank
 - Economy
 - Securities Exchange
 - National Bank of Cambodia
-start_page: 1
+start_page: 0
 max_num_pages: 2
 max_num_articles: 10
-output_dir: workspace/datasets//fetcher/khmer
+output_dir: workspace/datasets/fetcher/phnompenh
 link_filename: links.jsonl
 article_filename: articles.jsonl
 overwrite_existing: false
 key_field: url
-delay_between_requests: 0.0
+delay_between_requests: 20.0
 num_workers: 1
 print_every: 10
 verbose: true
```

### Comparing `nbcpu-0.6.0/src/nbcpu/conf/fetcher/phnompenh.yaml` & `nbcpu-0.7.0/src/nbcpu/conf/fetcher/khmer.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-_target_: nbcpu.fetcher.phnompenh.PhnompenhFetcher
-_config_name_: phnompenh
+_target_: nbcpu.fetcher.khmer.KhmerFetcher
+_config_name_: khmer
 _config_group_: /fetcher
-search_url: https://phnompenhpost.com/search/node/{keyword}?page={page}
+search_url: https://www.khmertimeskh.com/page/{page}/?s={keyword}
 search_keywords:
 - NBC
 - Exchange Rate
 - De-dollarization
 - Inflation
 - GDP
 - Monetary Policy
@@ -17,19 +17,19 @@
 - Policy
 - Financial
 - Riel
 - Bank
 - Economy
 - Securities Exchange
 - National Bank of Cambodia
-start_page: 0
+start_page: 1
 max_num_pages: 2
 max_num_articles: 10
-output_dir: workspace/datasets/fetcher/phnompenh
+output_dir: workspace/datasets/fetcher/khmer
 link_filename: links.jsonl
 article_filename: articles.jsonl
 overwrite_existing: false
 key_field: url
-delay_between_requests: 20.0
+delay_between_requests: 0.0
 num_workers: 1
 print_every: 10
 verbose: true
```

### Comparing `nbcpu-0.6.0/src/nbcpu/fetcher/base.py` & `nbcpu-0.7.0/src/nbcpu/fetcher/base.py`

 * *Files identical despite different names*

### Comparing `nbcpu-0.6.0/src/nbcpu/fetcher/khmer.py` & `nbcpu-0.7.0/src/nbcpu/fetcher/khmer.py`

 * *Files identical despite different names*

### Comparing `nbcpu-0.6.0/src/nbcpu/fetcher/phnompenh.py` & `nbcpu-0.7.0/src/nbcpu/fetcher/phnompenh.py`

 * *Files identical despite different names*

### Comparing `nbcpu-0.6.0/PKG-INFO` & `nbcpu-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nbcpu
-Version: 0.6.0
+Version: 0.7.0
 Summary: Quantifying Central Bank Policy Uncertainty in a Highly Dollarized Economy: A Topic Modeling Approach
 Home-page: https://entelecheia.github.io/nbcpu
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: hyfi (>=1.18.1,<2.0.0)
-Requires-Dist: lexikanon (>=0.4.2,<0.5.0)
+Requires-Dist: hyfi (>=1.25.0,<2.0.0)
+Requires-Dist: lexikanon (>=0.5.2,<0.6.0)
 Project-URL: Repository, https://github.com/entelecheia/nbcpu
 Description-Content-Type: text/markdown
 
 # Measuring Central Bank Policy Uncertainty
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
```

