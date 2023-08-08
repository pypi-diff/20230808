# Comparing `tmp/mdast_cli_core-2023.8.1.tar.gz` & `tmp/mdast_cli_core-2023.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdast_cli_core-2023.8.1.tar", last modified: Tue Aug  1 11:23:01 2023, max compression
+gzip compressed data, was "mdast_cli_core-2023.8.2.tar", last modified: Tue Aug  8 19:35:29 2023, max compression
```

## Comparing `mdast_cli_core-2023.8.1.tar` & `mdast_cli_core-2023.8.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:01.699842 mdast_cli_core-2023.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-08-01 11:23:01.699842 mdast_cli_core-2023.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-01 11:22:48.000000 mdast_cli_core-2023.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:01.699842 mdast_cli_core-2023.8.1/mdast_cli_core/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 11:22:48.000000 mdast_cli_core-2023.8.1/mdast_cli_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-01 11:22:48.000000 mdast_cli_core-2023.8.1/mdast_cli_core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27547 2023-08-01 11:22:48.000000 mdast_cli_core-2023.8.1/mdast_cli_core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-01 11:22:48.000000 mdast_cli_core-2023.8.1/mdast_cli_core/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:01.699842 mdast_cli_core-2023.8.1/mdast_cli_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-08-01 11:23:01.000000 mdast_cli_core-2023.8.1/mdast_cli_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-01 11:23:01.000000 mdast_cli_core-2023.8.1/mdast_cli_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:23:01.000000 mdast_cli_core-2023.8.1/mdast_cli_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 11:23:01.000000 mdast_cli_core-2023.8.1/mdast_cli_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:23:01.000000 mdast_cli_core-2023.8.1/mdast_cli_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:23:01.699842 mdast_cli_core-2023.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-01 11:22:48.000000 mdast_cli_core-2023.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:35:29.216975 mdast_cli_core-2023.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-08-08 19:35:29.216975 mdast_cli_core-2023.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-08 19:35:18.000000 mdast_cli_core-2023.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:35:29.216975 mdast_cli_core-2023.8.2/mdast_cli_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-08 19:35:18.000000 mdast_cli_core-2023.8.2/mdast_cli_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-08 19:35:18.000000 mdast_cli_core-2023.8.2/mdast_cli_core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27850 2023-08-08 19:35:18.000000 mdast_cli_core-2023.8.2/mdast_cli_core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-08 19:35:18.000000 mdast_cli_core-2023.8.2/mdast_cli_core/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:35:29.216975 mdast_cli_core-2023.8.2/mdast_cli_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-08-08 19:35:29.000000 mdast_cli_core-2023.8.2/mdast_cli_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-08 19:35:29.000000 mdast_cli_core-2023.8.2/mdast_cli_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 19:35:29.000000 mdast_cli_core-2023.8.2/mdast_cli_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 19:35:29.000000 mdast_cli_core-2023.8.2/mdast_cli_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-08 19:35:29.000000 mdast_cli_core-2023.8.2/mdast_cli_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 19:35:29.220975 mdast_cli_core-2023.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-08 19:35:18.000000 mdast_cli_core-2023.8.2/setup.py
```

### Comparing `mdast_cli_core-2023.8.1/PKG-INFO` & `mdast_cli_core-2023.8.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdast_cli_core
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: mDast core package
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli-core
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `mdast_cli_core-2023.8.1/mdast_cli_core/api.py` & `mdast_cli_core-2023.8.2/mdast_cli_core/api.py`

 * *Files identical despite different names*

### Comparing `mdast_cli_core-2023.8.1/mdast_cli_core/base.py` & `mdast_cli_core-2023.8.2/mdast_cli_core/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -604,14 +604,22 @@
     def download_report(self, dast_id):
         report = requests.get(f'{self.url}/dasts/{dast_id}/report/',
                               allow_redirects=True,
                               headers=self.headers,
                               verify=False)
         return report
 
+    def download_scan_json_result(self, dast_id):
+        report = requests.get(f'{self.url}/dasts/{dast_id}/report/?output=json',
+                              allow_redirects=True,
+                              headers=self.headers,
+                              verify=False)
+        return report
+
+
     def get_dast_logs(self, dast_id):
         return requests.get(f'{self.url}/dasts/{dast_id}/log/',
                             headers=self.headers,
                             verify=False)
 
     def get_profiles_for_project(self, project_id):
         return requests.get(f'{self.url}/projects/{project_id}/profiles/',
```

### Comparing `mdast_cli_core-2023.8.1/mdast_cli_core/token.py` & `mdast_cli_core-2023.8.2/mdast_cli_core/token.py`

 * *Files identical despite different names*

### Comparing `mdast_cli_core-2023.8.1/mdast_cli_core.egg-info/PKG-INFO` & `mdast_cli_core-2023.8.2/mdast_cli_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdast-cli-core
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: mDast core package
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli-core
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `mdast_cli_core-2023.8.1/setup.py` & `mdast_cli_core-2023.8.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mdast_cli_core",
-    version='2023.08.01',
+    version='2023.08.02',
     author="Dynamic-Mobile-Security",
     description="mDast core package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Dynamic-Mobile-Security/mdast-cli-core",
     packages=find_packages(),
     include_package_data=True,
```

