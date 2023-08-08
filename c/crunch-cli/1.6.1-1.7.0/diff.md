# Comparing `tmp/crunch-cli-1.6.1.tar.gz` & `tmp/crunch-cli-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch-cli-1.6.1.tar", last modified: Fri Aug  4 18:51:19 2023, max compression
+gzip compressed data, was "crunch-cli-1.7.0.tar", last modified: Tue Aug  8 15:35:57 2023, max compression
```

## Comparing `crunch-cli-1.6.1.tar` & `crunch-cli-1.7.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:51:19.608374 crunch-cli-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-04 18:51:19.608374 crunch-cli-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:51:19.604374 crunch-cli-1.6.1/crunch/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:51:19.604374 crunch-cli-1.6.1/crunch/command/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/command/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/command/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/command/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:51:19.604374 crunch-cli-1.6.1/crunch/demo-project/
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/demo-project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/demo-project/files.json
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/demo-project/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/demo-project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/ensure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/crunch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:51:19.608374 crunch-cli-1.6.1/crunch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-04 18:51:19.000000 crunch-cli-1.6.1/crunch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-04 18:51:19.000000 crunch-cli-1.6.1/crunch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 18:51:19.000000 crunch-cli-1.6.1/crunch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-04 18:51:19.000000 crunch-cli-1.6.1/crunch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 18:51:19.000000 crunch-cli-1.6.1/crunch_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-04 18:51:19.000000 crunch-cli-1.6.1/crunch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 18:51:19.000000 crunch-cli-1.6.1/crunch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 18:51:19.608374 crunch-cli-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-04 18:51:14.000000 crunch-cli-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:35:57.246141 crunch-cli-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-08 15:35:57.242141 crunch-cli-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:35:57.242141 crunch-cli-1.7.0/crunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:35:57.242141 crunch-cli-1.7.0/crunch/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/command/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/command/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/command/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:35:57.242141 crunch-cli-1.7.0/crunch/demo-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/demo-project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/demo-project/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/demo-project/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/demo-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/ensure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/crunch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:35:57.242141 crunch-cli-1.7.0/crunch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-08 15:35:57.000000 crunch-cli-1.7.0/crunch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-08 15:35:57.000000 crunch-cli-1.7.0/crunch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:35:57.000000 crunch-cli-1.7.0/crunch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 15:35:57.000000 crunch-cli-1.7.0/crunch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:35:57.000000 crunch-cli-1.7.0/crunch_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-08 15:35:57.000000 crunch-cli-1.7.0/crunch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 15:35:57.000000 crunch-cli-1.7.0/crunch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 15:35:57.246141 crunch-cli-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-08 15:35:51.000000 crunch-cli-1.7.0/setup.py
```

### Comparing `crunch-cli-1.6.1/PKG-INFO` & `crunch-cli-1.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crunch-cli
-Version: 1.6.1
+Version: 1.7.0
 Summary: crunch-cli - CLI of the CrunchDAO Platform
 Home-page: https://github.com/crunchdao/crunch-cli
 Author: Enzo CACERES
 Author-email: enzo.caceres@crunchdao.com
 Keywords: package development template
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `crunch-cli-1.6.1/README.md` & `crunch-cli-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.6.1/crunch/command/convert.py` & `crunch-cli-1.7.0/crunch/command/convert.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.6.1/crunch/command/download.py` & `crunch-cli-1.7.0/crunch/command/download.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.6.1/crunch/command/push.py` & `crunch-cli-1.7.0/crunch/command/push.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os
 import tarfile
 import tempfile
 import shutil
+import pkg_resources
+
 
 import gitignorefile
 
 from .. import constants, utils
 from .setup import _setup_demo
 
 
@@ -59,18 +61,26 @@
 
 
 def push(
     session: utils.CustomSession,
     message: str,
     main_file_path: str,
     model_directory_path: str,
-    export_path: str = None
+    include_installed_packages_version: bool,
+    export_path: str = None,
 ):
     project_name = utils.read_project_name()
     push_token = utils.read_token()
+    
+    installed_packages_version = {}
+    if include_installed_packages_version:
+        installed_packages_version = {
+            package.project_name: package.version
+            for package in pkg_resources.working_set
+        }
 
     fds = []
 
     try:
         if not os.path.exists(constants.DOT_GITIGNORE_FILE):
             _setup_demo(".",  [constants.DOT_GITIGNORE_FILE])
 
@@ -104,15 +114,19 @@
                 submission = session.post(
                     f"/v1/projects/{project_name}/submissions",
                     data={
                         "message": message,
                         "mainFilePath": main_file_path,
                         "modelDirectoryPath": model_directory_path,
                         "pushToken": push_token,
-                        "notebook": False
+                        "notebook": False,
+                        **{
+                            f"preferredPackagesVersion[{key}]": value
+                            for key, value in installed_packages_version.items()
+                        }
                     },
                     files=tuple(files)
                 ).json()
 
                 return submission
     finally:
         for fd in fds:
```

### Comparing `crunch-cli-1.6.1/crunch/command/setup.py` & `crunch-cli-1.7.0/crunch/command/setup.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.6.1/crunch/command/test.py` & `crunch-cli-1.7.0/crunch/command/test.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.6.1/crunch/constants.py` & `crunch-cli-1.7.0/crunch/constants.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.6.1/crunch/demo-project/.gitignore` & `crunch-cli-1.7.0/crunch/demo-project/.gitignore`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.6.1/crunch/demo-project/main.py` & `crunch-cli-1.7.0/crunch/demo-project/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.6.1/crunch/ensure.py` & `crunch-cli-1.7.0/crunch/ensure.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.6.1/crunch/inline.py` & `crunch-cli-1.7.0/crunch/inline.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.6.1/crunch/library.py` & `crunch-cli-1.7.0/crunch/library.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.6.1/crunch/main.py` & `crunch-cli-1.7.0/crunch/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,20 +79,22 @@
     print(f" - To see all of the available commands of the CrunchDAO CLI, run: crunch --help")
 
 
 @cli.command(help="Send the new submission of your code.")
 @click.option("-m", "--message", prompt=True, default="", help="Specify the change of your code. (like a commit message)")
 @click.option("--main-file", "main_file_path", default="main.py", show_default=True, help="Entrypoint of your code.")
 @click.option("--model-directory", "model_directory_path", default="resources", show_default=True, help="Directory where your model is stored.")
-@click.option("--export", "export_path", show_default=True, type=str, help="Copy the `.tar` to the specified file")
+@click.option("--export", "export_path", show_default=True, type=str, help="Copy the `.tar` to the specified file.")
+@click.option("--no-pip-freeze", is_flag=True, help="Do not do a `pip freeze` to know preferred packages version.")
 def push(
     message: str,
     main_file_path: str,
     model_directory_path: str,
     export_path: str,
+    no_pip_freeze: bool,
 ):
     utils.change_root()
 
     converted = False
     if not os.path.exists(main_file_path):
         print(f"missing {main_file_path}")
 
@@ -112,14 +114,15 @@
     try:
         submission = command.push(
             session,
             message=message,
             main_file_path=main_file_path,
             model_directory_path=model_directory_path,
             export_path=export_path,
+            include_installed_packages_version=not no_pip_freeze
         )
 
         if submission:
             command.push_summary(submission, session)
     finally:
         if converted:
             os.unlink(main_file_path)
```

### Comparing `crunch-cli-1.6.1/crunch/tester.py` & `crunch-cli-1.7.0/crunch/tester.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.6.1/crunch/utils.py` & `crunch-cli-1.7.0/crunch/utils.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.6.1/crunch_cli.egg-info/PKG-INFO` & `crunch-cli-1.7.0/crunch_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crunch-cli
-Version: 1.6.1
+Version: 1.7.0
 Summary: crunch-cli - CLI of the CrunchDAO Platform
 Home-page: https://github.com/crunchdao/crunch-cli
 Author: Enzo CACERES
 Author-email: enzo.caceres@crunchdao.com
 Keywords: package development template
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `crunch-cli-1.6.1/crunch_cli.egg-info/SOURCES.txt` & `crunch-cli-1.7.0/crunch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.6.1/setup.py` & `crunch-cli-1.7.0/setup.py`

 * *Files identical despite different names*

