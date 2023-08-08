# Comparing `tmp/outline-cli-1.0.8.tar.gz` & `tmp/outline-cli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outline-cli-1.0.8.tar", last modified: Tue Jan 10 11:50:25 2023, max compression
+gzip compressed data, was "outline-cli-1.0.9.tar", last modified: Tue Aug  8 16:40:03 2023, max compression
```

## Comparing `outline-cli-1.0.8.tar` & `outline-cli-1.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 11:50:25.424262 outline-cli-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 11:50:25.420262 outline-cli-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 11:50:25.420262 outline-cli-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-01-10 11:50:14.000000 outline-cli-1.0.8/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-01-10 11:50:14.000000 outline-cli-1.0.8/.github/workflows/run_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-10 11:50:14.000000 outline-cli-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-10 11:50:14.000000 outline-cli-1.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-10 11:50:14.000000 outline-cli-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-01-10 11:50:25.424262 outline-cli-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-01-10 11:50:14.000000 outline-cli-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-10 11:50:14.000000 outline-cli-1.0.8/example-app.ini
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-01-10 11:50:14.000000 outline-cli-1.0.8/example_email_list.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-10 11:50:14.000000 outline-cli-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-10 11:50:25.424262 outline-cli-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-10 11:50:14.000000 outline-cli-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 11:50:25.424262 outline-cli-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 11:50:25.424262 outline-cli-1.0.8/src/outline_cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-01-10 11:50:14.000000 outline-cli-1.0.8/src/outline_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-01-10 11:50:14.000000 outline-cli-1.0.8/src/outline_cli/gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-01-10 11:50:14.000000 outline-cli-1.0.8/src/outline_cli/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-01-10 11:50:14.000000 outline-cli-1.0.8/src/outline_cli/outline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 11:50:25.424262 outline-cli-1.0.8/src/outline_cli/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 11:50:14.000000 outline-cli-1.0.8/src/outline_cli/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-01-10 11:50:14.000000 outline-cli-1.0.8/src/outline_cli/templates/mail_template.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 11:50:25.424262 outline-cli-1.0.8/src/outline_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-01-10 11:50:25.000000 outline-cli-1.0.8/src/outline_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-01-10 11:50:25.000000 outline-cli-1.0.8/src/outline_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 11:50:25.000000 outline-cli-1.0.8/src/outline_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-10 11:50:25.000000 outline-cli-1.0.8/src/outline_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-10 11:50:25.000000 outline-cli-1.0.8/src/outline_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-10 11:50:25.000000 outline-cli-1.0.8/src/outline_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 11:50:25.000000 outline-cli-1.0.8/src/outline_cli.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-01-10 11:50:14.000000 outline-cli-1.0.8/src/tests.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      398 2023-01-10 11:50:14.000000 outline-cli-1.0.8/test.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 16:40:03.758871 outline-cli-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 16:40:03.754871 outline-cli-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 16:40:03.754871 outline-cli-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1041 2023-08-08 16:39:50.000000 outline-cli-1.0.9/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-08-08 16:39:50.000000 outline-cli-1.0.9/.github/workflows/run_test.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-08-08 16:39:50.000000 outline-cli-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-08-08 16:39:50.000000 outline-cli-1.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-08-08 16:39:50.000000 outline-cli-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1564 2023-08-08 16:40:03.758871 outline-cli-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      929 2023-08-08 16:39:50.000000 outline-cli-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-08-08 16:39:50.000000 outline-cli-1.0.9/example-app.ini
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-08-08 16:39:50.000000 outline-cli-1.0.9/example_email_list.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-08-08 16:39:50.000000 outline-cli-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-08 16:40:03.758871 outline-cli-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-08-08 16:39:50.000000 outline-cli-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 16:40:03.754871 outline-cli-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 16:40:03.754871 outline-cli-1.0.9/src/outline_cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-08-08 16:39:50.000000 outline-cli-1.0.9/src/outline_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-08-08 16:39:50.000000 outline-cli-1.0.9/src/outline_cli/gmail.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-08-08 16:39:50.000000 outline-cli-1.0.9/src/outline_cli/helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-08-08 16:39:50.000000 outline-cli-1.0.9/src/outline_cli/outline.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 16:40:03.758871 outline-cli-1.0.9/src/outline_cli/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 16:39:50.000000 outline-cli-1.0.9/src/outline_cli/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-08-08 16:39:50.000000 outline-cli-1.0.9/src/outline_cli/templates/mail_template.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 16:40:03.758871 outline-cli-1.0.9/src/outline_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1564 2023-08-08 16:40:03.000000 outline-cli-1.0.9/src/outline_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-08-08 16:40:03.000000 outline-cli-1.0.9/src/outline_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-08 16:40:03.000000 outline-cli-1.0.9/src/outline_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-08-08 16:40:03.000000 outline-cli-1.0.9/src/outline_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-08-08 16:40:03.000000 outline-cli-1.0.9/src/outline_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-08-08 16:40:03.000000 outline-cli-1.0.9/src/outline_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-08 16:40:03.000000 outline-cli-1.0.9/src/outline_cli.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     8755 2023-08-08 16:39:50.000000 outline-cli-1.0.9/src/tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      398 2023-08-08 16:39:50.000000 outline-cli-1.0.9/test.sh
```

### Comparing `outline-cli-1.0.8/.github/workflows/publish_to_pypi.yml` & `outline-cli-1.0.9/.github/workflows/publish_to_pypi.yml`

 * *Files 14% similar despite different names*

```diff
@@ -4,30 +4,30 @@
   release:
     types: [created]
     branches:
       - main
 
 jobs:
   build:
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-20.04
     strategy:
       matrix:
         python-version: [3.6, 3.7, 3.8]
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Test
         run: |
           bash test.sh
   deploy:
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-20.04
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
           python-version: '3.8'
       - name: Install dependencies
```

### Comparing `outline-cli-1.0.8/LICENSE.txt` & `outline-cli-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `outline-cli-1.0.8/PKG-INFO` & `outline-cli-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outline-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Jimmy Chen
 Author-email: jimmychen260@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/JMCFTW/outline-cli/issues
 Project-URL: Source Code, https://github.com/JMCFTW/outline-cli/
```

### Comparing `outline-cli-1.0.8/README.md` & `outline-cli-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `outline-cli-1.0.8/setup.py` & `outline-cli-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "Source Code": "https://github.com/JMCFTW/outline-cli/",
     },
     setup_requires=["setuptools_scm"],
     packages=["outline_cli"],
     package_dir={"": "src"},
     entry_points={"console_scripts": ["outline-cli=outline_cli:start_cli"]},
     install_requires=[
-        "certifi==2022.12.7",
+        "certifi==2023.7.22",
         "chardet==3.0.4",
         "idna==2.10",
         "requests-toolbelt==0.9.1",
         "urllib3==1.26.5",
         "PyInquirer==1.0.3",
     ],
     zip_safe=True,
```

### Comparing `outline-cli-1.0.8/src/outline_cli/__init__.py` & `outline-cli-1.0.9/src/outline_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `outline-cli-1.0.8/src/outline_cli/gmail.py` & `outline-cli-1.0.9/src/outline_cli/gmail.py`

 * *Files identical despite different names*

### Comparing `outline-cli-1.0.8/src/outline_cli/helper.py` & `outline-cli-1.0.9/src/outline_cli/helper.py`

 * *Files identical despite different names*

### Comparing `outline-cli-1.0.8/src/outline_cli/outline.py` & `outline-cli-1.0.9/src/outline_cli/outline.py`

 * *Files identical despite different names*

### Comparing `outline-cli-1.0.8/src/outline_cli/templates/mail_template.txt` & `outline-cli-1.0.9/src/outline_cli/templates/mail_template.txt`

 * *Files identical despite different names*

### Comparing `outline-cli-1.0.8/src/outline_cli.egg-info/PKG-INFO` & `outline-cli-1.0.9/src/outline_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outline-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Jimmy Chen
 Author-email: jimmychen260@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/JMCFTW/outline-cli/issues
 Project-URL: Source Code, https://github.com/JMCFTW/outline-cli/
```

### Comparing `outline-cli-1.0.8/src/outline_cli.egg-info/SOURCES.txt` & `outline-cli-1.0.9/src/outline_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `outline-cli-1.0.8/src/tests.py` & `outline-cli-1.0.9/src/tests.py`

 * *Files identical despite different names*

