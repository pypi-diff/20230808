# Comparing `tmp/github_webhook_server-0.0.0.tar.gz` & `tmp/github_webhook_server-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_webhook_server-0.0.0.tar", max compression
+gzip compressed data, was "github_webhook_server-1.0.6.tar", max compression
```

## Comparing `github_webhook_server-0.0.0.tar` & `github_webhook_server-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-08-07 21:41:21.487013 github_webhook_server-0.0.0/LICENSE
--rw-r--r--   0        0        0     5907 2023-08-07 21:41:21.487013 github_webhook_server-0.0.0/README.md
--rw-r--r--   0        0        0     1542 2023-08-07 21:41:21.488013 github_webhook_server-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-07 21:41:21.489013 github_webhook_server-0.0.0/webhook_server_container/__init__.py
--rw-r--r--   0        0        0     4564 2023-08-07 21:41:21.489013 github_webhook_server-0.0.0/webhook_server_container/app.py
--rw-r--r--   0        0        0        0 2023-08-07 21:41:21.489013 github_webhook_server-0.0.0/webhook_server_container/libs/__init__.py
--rw-r--r--   0        0        0    66847 2023-08-07 21:41:21.489013 github_webhook_server-0.0.0/webhook_server_container/libs/github_api.py
--rw-r--r--   0        0        0     1309 2023-08-07 21:41:21.490013 github_webhook_server-0.0.0/webhook_server_container/libs/sonar_qube.py
--rw-r--r--   0        0        0        0 2023-08-07 21:41:21.490013 github_webhook_server-0.0.0/webhook_server_container/utils/__init__.py
--rw-r--r--   0        0        0     2466 2023-08-07 21:41:21.490013 github_webhook_server-0.0.0/webhook_server_container/utils/constants.py
--rw-r--r--   0        0        0     1876 2023-08-07 21:41:21.490013 github_webhook_server-0.0.0/webhook_server_container/utils/dockerhub_rate_limit.py
--rw-r--r--   0        0        0     8288 2023-08-07 21:41:21.490013 github_webhook_server-0.0.0/webhook_server_container/utils/github_repository_settings.py
--rw-r--r--   0        0        0     6068 2023-08-07 21:41:21.490013 github_webhook_server-0.0.0/webhook_server_container/utils/helpers.py
--rw-r--r--   0        0        0     1154 2023-08-07 21:41:21.490013 github_webhook_server-0.0.0/webhook_server_container/utils/sonar_qube.py
--rw-r--r--   0        0        0     1844 2023-08-07 21:41:21.490013 github_webhook_server-0.0.0/webhook_server_container/utils/webhook.py
--rw-r--r--   0        0        0     7202 1970-01-01 00:00:00.000000 github_webhook_server-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-07 21:56:57.367681 github_webhook_server-1.0.6/LICENSE
+-rw-r--r--   0        0        0     5907 2023-08-07 21:56:57.367681 github_webhook_server-1.0.6/README.md
+-rw-r--r--   0        0        0     1543 2023-08-07 21:57:02.778697 github_webhook_server-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-07 21:56:57.369681 github_webhook_server-1.0.6/webhook_server_container/__init__.py
+-rw-r--r--   0        0        0     4564 2023-08-07 21:56:57.369681 github_webhook_server-1.0.6/webhook_server_container/app.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:56:57.369681 github_webhook_server-1.0.6/webhook_server_container/libs/__init__.py
+-rw-r--r--   0        0        0    66847 2023-08-07 21:56:57.369681 github_webhook_server-1.0.6/webhook_server_container/libs/github_api.py
+-rw-r--r--   0        0        0     1309 2023-08-07 21:56:57.369681 github_webhook_server-1.0.6/webhook_server_container/libs/sonar_qube.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:56:57.369681 github_webhook_server-1.0.6/webhook_server_container/utils/__init__.py
+-rw-r--r--   0        0        0     2466 2023-08-07 21:56:57.369681 github_webhook_server-1.0.6/webhook_server_container/utils/constants.py
+-rw-r--r--   0        0        0     1876 2023-08-07 21:56:57.369681 github_webhook_server-1.0.6/webhook_server_container/utils/dockerhub_rate_limit.py
+-rw-r--r--   0        0        0     8288 2023-08-07 21:56:57.369681 github_webhook_server-1.0.6/webhook_server_container/utils/github_repository_settings.py
+-rw-r--r--   0        0        0     6068 2023-08-07 21:56:57.370681 github_webhook_server-1.0.6/webhook_server_container/utils/helpers.py
+-rw-r--r--   0        0        0     1154 2023-08-07 21:56:57.370681 github_webhook_server-1.0.6/webhook_server_container/utils/sonar_qube.py
+-rw-r--r--   0        0        0     1844 2023-08-07 21:56:57.370681 github_webhook_server-1.0.6/webhook_server_container/utils/webhook.py
+-rw-r--r--   0        0        0     7202 1970-01-01 00:00:00.000000 github_webhook_server-1.0.6/PKG-INFO
```

### Comparing `github_webhook_server-0.0.0/LICENSE` & `github_webhook_server-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `github_webhook_server-0.0.0/README.md` & `github_webhook_server-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `github_webhook_server-0.0.0/pyproject.toml` & `github_webhook_server-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [tool.isort]
 line_length = 88
 profile = "black"
 
 [tool.poetry]
 name = "github-webhook-server"
-version = "0.0.0"
+version = "1.0.6"
 description = "A webhook server to manage Github reposotories and pull requests."
 authors = ["Meni Yakove <myakove@gmail.com>", "Ruth Netser <ruth.netser@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/myakove/github-webhook-server"
 repository = "https://github.com/myakove/github-webhook-server"
 packages = [{include = "webhook_server_container"}]
@@ -48,15 +48,15 @@
 python-sonarqube-api = "^2.0.4"
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "^0.13.13"
 ipython = "*"
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 pattern = "((?P<epoch>\\d+)!)?(?P<base>\\d+(\\.\\d+)*)"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.ruff]
```

### Comparing `github_webhook_server-0.0.0/webhook_server_container/app.py` & `github_webhook_server-1.0.6/webhook_server_container/app.py`

 * *Files identical despite different names*

### Comparing `github_webhook_server-0.0.0/webhook_server_container/libs/github_api.py` & `github_webhook_server-1.0.6/webhook_server_container/libs/github_api.py`

 * *Files identical despite different names*

### Comparing `github_webhook_server-0.0.0/webhook_server_container/libs/sonar_qube.py` & `github_webhook_server-1.0.6/webhook_server_container/libs/sonar_qube.py`

 * *Files identical despite different names*

### Comparing `github_webhook_server-0.0.0/webhook_server_container/utils/constants.py` & `github_webhook_server-1.0.6/webhook_server_container/utils/constants.py`

 * *Files identical despite different names*

### Comparing `github_webhook_server-0.0.0/webhook_server_container/utils/dockerhub_rate_limit.py` & `github_webhook_server-1.0.6/webhook_server_container/utils/dockerhub_rate_limit.py`

 * *Files identical despite different names*

### Comparing `github_webhook_server-0.0.0/webhook_server_container/utils/github_repository_settings.py` & `github_webhook_server-1.0.6/webhook_server_container/utils/github_repository_settings.py`

 * *Files identical despite different names*

### Comparing `github_webhook_server-0.0.0/webhook_server_container/utils/helpers.py` & `github_webhook_server-1.0.6/webhook_server_container/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `github_webhook_server-0.0.0/webhook_server_container/utils/sonar_qube.py` & `github_webhook_server-1.0.6/webhook_server_container/utils/sonar_qube.py`

 * *Files identical despite different names*

### Comparing `github_webhook_server-0.0.0/webhook_server_container/utils/webhook.py` & `github_webhook_server-1.0.6/webhook_server_container/utils/webhook.py`

 * *Files identical despite different names*

### Comparing `github_webhook_server-0.0.0/PKG-INFO` & `github_webhook_server-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-webhook-server
-Version: 0.0.0
+Version: 1.0.6
 Summary: A webhook server to manage Github reposotories and pull requests.
 Home-page: https://github.com/myakove/github-webhook-server
 License: Apache-2.0
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

