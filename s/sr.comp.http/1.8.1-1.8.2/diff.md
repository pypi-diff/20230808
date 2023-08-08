# Comparing `tmp/sr.comp.http-1.8.1.tar.gz` & `tmp/sr.comp.http-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sr.comp.http-1.8.1.tar", last modified: Sat Aug  5 16:21:28 2023, max compression
+gzip compressed data, was "dist/sr.comp.http-1.8.2.tar", last modified: Tue Aug  8 18:12:54 2023, max compression
```

## Comparing `sr.comp.http-1.8.1.tar` & `sr.comp.http-1.8.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3644 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1829 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      405 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1157 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2117 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/sr/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/sr/comp/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/sr/comp/http/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      739 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      529 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      426 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/escaping_formatter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/json_encoder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      178 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/logging-stdout.ini
--rw-r--r--   0 circleci  (1001) circleci  (1002)      365 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/logging-syslog.ini
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3213 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/manager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5184 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/query_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12162 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2023-08-05 16:21:18.000000 sr.comp.http-1.8.1/sr/comp/http/update.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3644 2023-08-05 16:21:27.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      943 2023-08-05 16:21:27.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-05 16:21:27.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-08-05 16:21:27.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-08-05 16:21:27.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/namespace_packages.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-05 16:21:27.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      118 2023-08-05 16:21:27.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2023-08-05 16:21:27.000000 sr.comp.http-1.8.1/sr.comp.http.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/venv/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:28.000000 sr.comp.http-1.8.1/venv/bin/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      625 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2html.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      747 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2html4.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1082 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2html5.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      824 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2latex.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      647 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2man.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      813 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2odt.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      619 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      632 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      668 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2s5.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      904 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2xetex.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      633 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rst2xml.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      701 2023-08-05 16:21:26.000000 sr.comp.http-1.8.1/venv/bin/rstpep2html.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-08-08 18:12:43.000000 sr.comp.http-1.8.2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3644 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1829 2023-08-08 18:12:43.000000 sr.comp.http-1.8.2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      405 2023-08-08 18:12:43.000000 sr.comp.http-1.8.2/docs/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1157 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2117 2023-08-08 18:12:43.000000 sr.comp.http-1.8.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/sr/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/sr/comp/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/sr/comp/http/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-08-08 18:12:43.000000 sr.comp.http-1.8.2/sr/comp/http/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      739 2023-08-08 18:12:43.000000 sr.comp.http-1.8.2/sr/comp/http/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      529 2023-08-08 18:12:43.000000 sr.comp.http-1.8.2/sr/comp/http/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-08-08 18:12:43.000000 sr.comp.http-1.8.2/sr/comp/http/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      426 2023-08-08 18:12:43.000000 sr.comp.http-1.8.2/sr/comp/http/escaping_formatter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-08-08 18:12:43.000000 sr.comp.http-1.8.2/sr/comp/http/json_encoder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      178 2023-08-08 18:12:43.000000 sr.comp.http-1.8.2/sr/comp/http/logging-stdout.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      365 2023-08-08 18:12:43.000000 sr.comp.http-1.8.2/sr/comp/http/logging-syslog.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3213 2023-08-08 18:12:43.000000 sr.comp.http-1.8.2/sr/comp/http/manager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5184 2023-08-08 18:12:43.000000 sr.comp.http-1.8.2/sr/comp/http/query_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12255 2023-08-08 18:12:43.000000 sr.comp.http-1.8.2/sr/comp/http/server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1334 2023-08-08 18:12:43.000000 sr.comp.http-1.8.2/sr/comp/http/update.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/sr.comp.http.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3644 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/sr.comp.http.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      943 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/sr.comp.http.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/sr.comp.http.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/sr.comp.http.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/sr.comp.http.egg-info/namespace_packages.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/sr.comp.http.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      118 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/sr.comp.http.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/sr.comp.http.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/venv/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 18:12:54.000000 sr.comp.http-1.8.2/venv/bin/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      625 2023-08-08 18:12:52.000000 sr.comp.http-1.8.2/venv/bin/rst2html.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      747 2023-08-08 18:12:52.000000 sr.comp.http-1.8.2/venv/bin/rst2html4.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1082 2023-08-08 18:12:52.000000 sr.comp.http-1.8.2/venv/bin/rst2html5.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      824 2023-08-08 18:12:52.000000 sr.comp.http-1.8.2/venv/bin/rst2latex.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      647 2023-08-08 18:12:52.000000 sr.comp.http-1.8.2/venv/bin/rst2man.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      813 2023-08-08 18:12:52.000000 sr.comp.http-1.8.2/venv/bin/rst2odt.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      619 2023-08-08 18:12:52.000000 sr.comp.http-1.8.2/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      632 2023-08-08 18:12:52.000000 sr.comp.http-1.8.2/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      668 2023-08-08 18:12:52.000000 sr.comp.http-1.8.2/venv/bin/rst2s5.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      904 2023-08-08 18:12:52.000000 sr.comp.http-1.8.2/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      633 2023-08-08 18:12:52.000000 sr.comp.http-1.8.2/venv/bin/rst2xml.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      701 2023-08-08 18:12:52.000000 sr.comp.http-1.8.2/venv/bin/rstpep2html.py
```

### Comparing `sr.comp.http-1.8.1/PKG-INFO` & `sr.comp.http-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sr.comp.http
-Version: 1.8.1
+Version: 1.8.2
 Summary: HTTP API for Student Robotics Competition Software
 Home-page: https://github.com/PeterJCLaw/srcomp-http
 Author: Student Robotics Competition Software SIG
 Author-email: srobo-devel@googlegroups.com
 License: UNKNOWN
 Project-URL: Documentation, https://srcomp-http.readthedocs.org/
 Project-URL: Code, https://github.com/PeterJCLaw/srcomp-http
```

### Comparing `sr.comp.http-1.8.1/README.rst` & `sr.comp.http-1.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/setup.cfg` & `sr.comp.http-1.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/setup.py` & `sr.comp.http-1.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_namespace_packages, setup
 
 with open('README.rst') as f:
     long_description = f.read()
 
 setup(
     name='sr.comp.http',
-    version='1.8.1',
+    version='1.8.2',
     url='https://github.com/PeterJCLaw/srcomp-http',
     project_urls={
         'Documentation': 'https://srcomp-http.readthedocs.org/',
         'Code': 'https://github.com/PeterJCLaw/srcomp-http',
         'Issue tracker': 'https://github.com/PeterJCLaw/srcomp-http/issues',
     },
     packages=find_namespace_packages(exclude=('tests',)),
```

### Comparing `sr.comp.http-1.8.1/sr/comp/http/__main__.py` & `sr.comp.http-1.8.2/sr/comp/http/__main__.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/sr/comp/http/config.py` & `sr.comp.http-1.8.2/sr/comp/http/config.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/sr/comp/http/json_encoder.py` & `sr.comp.http-1.8.2/sr/comp/http/json_encoder.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/sr/comp/http/manager.py` & `sr.comp.http-1.8.2/sr/comp/http/manager.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/sr/comp/http/query_utils.py` & `sr.comp.http-1.8.2/sr/comp/http/query_utils.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/sr/comp/http/server.py` & `sr.comp.http-1.8.2/sr/comp/http/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,17 +379,19 @@
             if time > staging_times['closes']:
                 # Already done staging
                 continue
 
             if staging_times['opens'] <= time:
                 staging_matches.append(match_json_info(comp, match))
 
-            first_signal = min(staging_times['signal_shepherds'].values())
-            if first_signal <= time:
-                shepherding_matches.append(match_json_info(comp, match))
+            signal_shepherds = staging_times['signal_shepherds']
+            if signal_shepherds:
+                first_signal = min(signal_shepherds.values())
+                if first_signal <= time:
+                    shepherding_matches.append(match_json_info(comp, match))
 
     return jsonify(
         delay=delay_seconds,
         time=time.isoformat(),
         matches=matches,
         staging_matches=staging_matches,
         shepherding_matches=shepherding_matches,
```

### Comparing `sr.comp.http-1.8.1/sr/comp/http/update.py` & `sr.comp.http-1.8.2/sr/comp/http/update.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/sr.comp.http.egg-info/PKG-INFO` & `sr.comp.http-1.8.2/sr.comp.http.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sr.comp.http
-Version: 1.8.1
+Version: 1.8.2
 Summary: HTTP API for Student Robotics Competition Software
 Home-page: https://github.com/PeterJCLaw/srcomp-http
 Author: Student Robotics Competition Software SIG
 Author-email: srobo-devel@googlegroups.com
 License: UNKNOWN
 Project-URL: Documentation, https://srcomp-http.readthedocs.org/
 Project-URL: Code, https://github.com/PeterJCLaw/srcomp-http
```

### Comparing `sr.comp.http-1.8.1/sr.comp.http.egg-info/SOURCES.txt` & `sr.comp.http-1.8.2/sr.comp.http.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/venv/bin/rst2html.py` & `sr.comp.http-1.8.2/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/venv/bin/rst2html4.py` & `sr.comp.http-1.8.2/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/venv/bin/rst2html5.py` & `sr.comp.http-1.8.2/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/venv/bin/rst2latex.py` & `sr.comp.http-1.8.2/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/venv/bin/rst2man.py` & `sr.comp.http-1.8.2/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/venv/bin/rst2odt.py` & `sr.comp.http-1.8.2/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/venv/bin/rst2odt_prepstyles.py` & `sr.comp.http-1.8.2/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/venv/bin/rst2pseudoxml.py` & `sr.comp.http-1.8.2/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/venv/bin/rst2s5.py` & `sr.comp.http-1.8.2/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/venv/bin/rst2xetex.py` & `sr.comp.http-1.8.2/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/venv/bin/rst2xml.py` & `sr.comp.http-1.8.2/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `sr.comp.http-1.8.1/venv/bin/rstpep2html.py` & `sr.comp.http-1.8.2/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

