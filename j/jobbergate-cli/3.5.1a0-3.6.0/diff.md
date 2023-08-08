# Comparing `tmp/jobbergate_cli-3.5.1a0.tar.gz` & `tmp/jobbergate_cli-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_cli-3.5.1a0.tar", max compression
+gzip compressed data, was "jobbergate_cli-3.6.0.tar", max compression
```

## Comparing `jobbergate_cli-3.5.1a0.tar` & `jobbergate_cli-3.6.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1082 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/LICENSE
--rw-r--r--   0        0        0     1065 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/README.rst
--rw-r--r--   0        0        0      801 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/jobbergate_cli/__init__.py
--rw-r--r--   0        0        0     1112 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/jobbergate_cli/application_base.py
--rw-r--r--   0        0        0    11271 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/jobbergate_cli/auth.py
--rw-r--r--   0        0        0     4414 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/jobbergate_cli/compat.py
--rw-r--r--   0        0        0     4355 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/jobbergate_cli/config.py
--rw-r--r--   0        0        0     1139 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/jobbergate_cli/constants.py
--rw-r--r--   0        0        0     3112 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/jobbergate_cli/exceptions.py
--rw-r--r--   0        0        0     1134 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/jobbergate_cli/jobberappslib.py
--rw-r--r--   0        0        0     1095 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/jobbergate_cli/logging.py
--rw-r--r--   0        0        0     6510 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/jobbergate_cli/main.py
--rw-r--r--   0        0        0     7523 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/jobbergate_cli/render.py
--rw-r--r--   0        0        0     7954 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/jobbergate_cli/requests.py
--rw-r--r--   0        0        0     6118 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/jobbergate_cli/schemas.py
--rw-r--r--   0        0        0       66 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/__init__.py
--rw-r--r--   0        0        0       66 2023-08-08 14:41:41.649298 jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/applications/__init__.py
--rw-r--r--   0        0        0    11778 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/applications/app.py
--rw-r--r--   0        0        0     1725 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/applications/application_base.py
--rw-r--r--   0        0        0     1558 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/applications/application_helpers.py
--rw-r--r--   0        0        0    13800 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/applications/questions.py
--rw-r--r--   0        0        0    11471 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/applications/tools.py
--rw-r--r--   0        0        0       61 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/clusters/__init__.py
--rw-r--r--   0        0        0      728 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/clusters/app.py
--rw-r--r--   0        0        0     3284 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/clusters/tools.py
--rw-r--r--   0        0        0       64 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/job_scripts/__init__.py
--rw-r--r--   0        0        0    11693 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/job_scripts/app.py
--rw-r--r--   0        0        0     6750 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/job_scripts/tools.py
--rw-r--r--   0        0        0       68 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/job_submissions/__init__.py
--rw-r--r--   0        0        0     7123 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/job_submissions/app.py
--rw-r--r--   0        0        0     4167 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/job_submissions/tools.py
--rw-r--r--   0        0        0     1370 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/jobbergate_cli/text_tools.py
--rw-r--r--   0        0        0     3524 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/jobbergate_cli/time_loop.py
--rw-r--r--   0        0        0     2499 2023-08-08 14:41:41.653298 jobbergate_cli-3.5.1a0/pyproject.toml
--rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 jobbergate_cli-3.5.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/LICENSE
+-rw-r--r--   0        0        0     1065 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/README.rst
+-rw-r--r--   0        0        0      801 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/__init__.py
+-rw-r--r--   0        0        0     1112 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/application_base.py
+-rw-r--r--   0        0        0    11271 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/auth.py
+-rw-r--r--   0        0        0     4414 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/compat.py
+-rw-r--r--   0        0        0     4355 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/config.py
+-rw-r--r--   0        0        0     1139 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/constants.py
+-rw-r--r--   0        0        0     3112 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/exceptions.py
+-rw-r--r--   0        0        0     1134 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/jobberappslib.py
+-rw-r--r--   0        0        0     1095 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/logging.py
+-rw-r--r--   0        0        0     6510 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/main.py
+-rw-r--r--   0        0        0     7523 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/render.py
+-rw-r--r--   0        0        0     7954 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/requests.py
+-rw-r--r--   0        0        0     6118 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/schemas.py
+-rw-r--r--   0        0        0       66 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/subapps/__init__.py
+-rw-r--r--   0        0        0       66 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/subapps/applications/__init__.py
+-rw-r--r--   0        0        0    11778 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/subapps/applications/app.py
+-rw-r--r--   0        0        0     1725 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/subapps/applications/application_base.py
+-rw-r--r--   0        0        0     1558 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/subapps/applications/application_helpers.py
+-rw-r--r--   0        0        0    13800 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/subapps/applications/questions.py
+-rw-r--r--   0        0        0    11471 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/subapps/applications/tools.py
+-rw-r--r--   0        0        0       61 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/subapps/clusters/__init__.py
+-rw-r--r--   0        0        0      728 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/subapps/clusters/app.py
+-rw-r--r--   0        0        0     3284 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/subapps/clusters/tools.py
+-rw-r--r--   0        0        0       64 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/subapps/job_scripts/__init__.py
+-rw-r--r--   0        0        0    11693 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/subapps/job_scripts/app.py
+-rw-r--r--   0        0        0     6750 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/subapps/job_scripts/tools.py
+-rw-r--r--   0        0        0       68 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/subapps/job_submissions/__init__.py
+-rw-r--r--   0        0        0     7123 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/subapps/job_submissions/app.py
+-rw-r--r--   0        0        0     4167 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/subapps/job_submissions/tools.py
+-rw-r--r--   0        0        0     1370 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/text_tools.py
+-rw-r--r--   0        0        0     3524 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/jobbergate_cli/time_loop.py
+-rw-r--r--   0        0        0     2523 2023-07-30 04:37:48.161388 jobbergate_cli-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 jobbergate_cli-3.6.0/PKG-INFO
```

### Comparing `jobbergate_cli-3.5.1a0/LICENSE` & `jobbergate_cli-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/README.rst` & `jobbergate_cli-3.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/__init__.py` & `jobbergate_cli-3.6.0/jobbergate_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/application_base.py` & `jobbergate_cli-3.6.0/jobbergate_cli/application_base.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/auth.py` & `jobbergate_cli-3.6.0/jobbergate_cli/auth.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/compat.py` & `jobbergate_cli-3.6.0/jobbergate_cli/compat.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/config.py` & `jobbergate_cli-3.6.0/jobbergate_cli/config.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/constants.py` & `jobbergate_cli-3.6.0/jobbergate_cli/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/exceptions.py` & `jobbergate_cli-3.6.0/jobbergate_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/jobberappslib.py` & `jobbergate_cli-3.6.0/jobbergate_cli/jobberappslib.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/logging.py` & `jobbergate_cli-3.6.0/jobbergate_cli/logging.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/main.py` & `jobbergate_cli-3.6.0/jobbergate_cli/main.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/render.py` & `jobbergate_cli-3.6.0/jobbergate_cli/render.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/requests.py` & `jobbergate_cli-3.6.0/jobbergate_cli/requests.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/schemas.py` & `jobbergate_cli-3.6.0/jobbergate_cli/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/applications/app.py` & `jobbergate_cli-3.6.0/jobbergate_cli/subapps/applications/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/applications/application_base.py` & `jobbergate_cli-3.6.0/jobbergate_cli/subapps/applications/application_base.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/applications/application_helpers.py` & `jobbergate_cli-3.6.0/jobbergate_cli/subapps/applications/application_helpers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/applications/questions.py` & `jobbergate_cli-3.6.0/jobbergate_cli/subapps/applications/questions.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/applications/tools.py` & `jobbergate_cli-3.6.0/jobbergate_cli/subapps/applications/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/clusters/app.py` & `jobbergate_cli-3.6.0/jobbergate_cli/subapps/clusters/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/clusters/tools.py` & `jobbergate_cli-3.6.0/jobbergate_cli/subapps/clusters/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/job_scripts/app.py` & `jobbergate_cli-3.6.0/jobbergate_cli/subapps/job_scripts/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/job_scripts/tools.py` & `jobbergate_cli-3.6.0/jobbergate_cli/subapps/job_scripts/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/job_submissions/app.py` & `jobbergate_cli-3.6.0/jobbergate_cli/subapps/job_submissions/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/subapps/job_submissions/tools.py` & `jobbergate_cli-3.6.0/jobbergate_cli/subapps/job_submissions/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/text_tools.py` & `jobbergate_cli-3.6.0/jobbergate_cli/text_tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/jobbergate_cli/time_loop.py` & `jobbergate_cli-3.6.0/jobbergate_cli/time_loop.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-3.5.1a0/pyproject.toml` & `jobbergate_cli-3.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "jobbergate-cli"
-version = "3.5.1a0"
+version = "3.6.0"
 description = "Jobbergate CLI Client"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/jobbergate"
-packages = [{ include = "jobbergate_cli" }]
+packages = [ { include = "jobbergate_cli" } ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Development Status :: 5 - Production/Stable",
     "Topic :: Scientific/Engineering",
 ]
@@ -19,15 +19,15 @@
 "Bug Tracker" = "https://github.com/omnivector-solutions/jobbergate/issues"
 "Changelog" = "https://github.com/omnivector-solutions/jobbergate/blob/main/jobbergate-cli/CHANGELOG.rst"
 
 [tool.poetry.dependencies]
 python = "^3.6.2"
 click = "^8.0.1"
 inquirer = "^2.7.0"
-PyYAML = "6.*"
+PyYAML = "^5.4.1"
 python-dotenv = "^0.19.0"
 sentry-sdk = "^1.4.3"
 boto3 = "^1.18.64"
 loguru = "^0.6.0"
 python-jose = "^3.3.0"
 pydantic = "^1.8.2"
 yarl = "^1.7.2"
@@ -45,15 +45,15 @@
 pytest-cov = "^3.0.0"
 pytest-random-order = "^1.0.4"
 pytest-freezegun = "^0.4.2"
 pytest-responsemock = "^1.0.1"
 isort = "^5.9.3"
 pytest-env = "^0.6.2"
 respx = "^0.19.2"
-plummet = { extras = ["time-machine"], version = "^1.1.0" }
+plummet = {extras = ["time-machine"], version = "^1.1.0"}
 pyproject-flake8 = "^0.0.1-alpha.2"
 mypy = "^0.931"
 pytest-mock = "^3.6.0"
 types-PyYAML = "^6.0.4"
 ipython = "^7.10"
 
 [tool.poetry.scripts]
@@ -87,13 +87,19 @@
 include_trailing_comma = true
 
 [tool.flake8]
 max-line-length = 120
 max-complexity = 40
 
 [[tool.mypy.overrides]]
-module = ["urllib3", "pyperclip", "inquirer.*", "jose.*", "pep562"]
+module = [
+    "urllib3",
+    "pyperclip",
+    "inquirer.*",
+    "jose.*",
+    "pep562",
+]
 ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `jobbergate_cli-3.5.1a0/PKG-INFO` & `jobbergate_cli-3.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-cli
-Version: 3.5.1a0
+Version: 3.6.0
 Summary: Jobbergate CLI Client
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: PyYAML (>=6.0.0,<7.0.0)
+Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
 Requires-Dist: boto3 (>=1.18.64,<2.0.0)
 Requires-Dist: click (>=8.0.1,<9.0.0)
 Requires-Dist: httpx (>=0.22.0,<0.23.0)
 Requires-Dist: importlib-metadata (>=4.2,<5.0)
 Requires-Dist: inquirer (>=2.7.0,<3.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
```

