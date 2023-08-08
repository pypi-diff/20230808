# Comparing `tmp/hansken-2023.8.4.tar.gz` & `tmp/hansken-2023.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hansken-2023.8.4.tar", last modified: Fri Aug  4 15:03:30 2023, max compression
+gzip compressed data, was "hansken-2023.8.8.tar", last modified: Tue Aug  8 14:29:10 2023, max compression
```

## Comparing `hansken-2023.8.4.tar` & `hansken-2023.8.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:30.732478 hansken-2023.8.4/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11358 2023-08-04 15:03:22.000000 hansken-2023.8.4/LICENSE
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       78 2023-08-04 15:03:22.000000 hansken-2023.8.4/MANIFEST.in
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1476 2023-08-04 15:03:30.732478 hansken-2023.8.4/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      769 2023-08-04 15:03:22.000000 hansken-2023.8.4/README.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:30.728478 hansken-2023.8.4/hansken/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        8 2023-08-04 15:03:27.000000 hansken-2023.8.4/hansken/VERSION
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2483 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      126 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/abstract_trace.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1306 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/admin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    32028 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/auth.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5898 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/connect.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26248 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/query.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:30.732478 hansken-2023.8.4/hansken/recipes/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/recipes/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21709 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/recipes/export.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:30.732478 hansken-2023.8.4/hansken/recipes/report/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5633 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/recipes/report/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:30.728478 hansken-2023.8.4/hansken/recipes/report/templates/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:30.732478 hansken-2023.8.4/hansken/recipes/report/templates/hansken/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1124 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/recipes/report/templates/hansken/base.html
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      337 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/recipes/report/templates/hansken/default.css
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      922 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/recipes/report/templates/hansken/macros.html
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      157 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/recipes/report/templates/hansken/print.css
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      117 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/recipes/report/templates/hansken/table.html
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)   135700 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/remote.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:30.732478 hansken-2023.8.4/hansken/tool/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    23624 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11560 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/_webhdfs.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11226 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_backup.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12360 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_extract.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3846 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_grant.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7809 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_mount.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11147 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_quickstart.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4160 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_shell.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5470 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_stats.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4028 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_tasks.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1705 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_tools.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20597 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_upload.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5347 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/tool/command_versions.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    59819 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/trace.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20956 2023-08-04 15:03:22.000000 hansken-2023.8.4/hansken/util.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-04 15:03:30.732478 hansken-2023.8.4/hansken.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1476 2023-08-04 15:03:30.000000 hansken-2023.8.4/hansken.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1169 2023-08-04 15:03:30.000000 hansken-2023.8.4/hansken.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-08-04 15:03:30.000000 hansken-2023.8.4/hansken.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       45 2023-08-04 15:03:30.000000 hansken-2023.8.4/hansken.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      299 2023-08-04 15:03:30.000000 hansken-2023.8.4/hansken.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        8 2023-08-04 15:03:30.000000 hansken-2023.8.4/hansken.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-08-04 15:03:30.732478 hansken-2023.8.4/setup.cfg
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1827 2023-08-04 15:03:22.000000 hansken-2023.8.4/setup.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-08 14:29:10.975390 hansken-2023.8.8/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11358 2023-08-08 14:28:59.000000 hansken-2023.8.8/LICENSE
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       78 2023-08-08 14:28:59.000000 hansken-2023.8.8/MANIFEST.in
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1476 2023-08-08 14:29:10.975390 hansken-2023.8.8/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      769 2023-08-08 14:28:59.000000 hansken-2023.8.8/README.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-08 14:29:10.971390 hansken-2023.8.8/hansken/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        8 2023-08-08 14:29:05.000000 hansken-2023.8.8/hansken/VERSION
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2483 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      126 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/abstract_trace.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1306 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/admin.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    32028 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/auth.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5898 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/connect.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26248 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/query.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-08 14:29:10.971390 hansken-2023.8.8/hansken/recipes/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/recipes/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21709 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/recipes/export.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-08 14:29:10.971390 hansken-2023.8.8/hansken/recipes/report/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5633 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/recipes/report/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-08 14:29:10.967390 hansken-2023.8.8/hansken/recipes/report/templates/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-08 14:29:10.975390 hansken-2023.8.8/hansken/recipes/report/templates/hansken/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1124 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/recipes/report/templates/hansken/base.html
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      337 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/recipes/report/templates/hansken/default.css
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      922 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/recipes/report/templates/hansken/macros.html
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      157 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/recipes/report/templates/hansken/print.css
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      117 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/recipes/report/templates/hansken/table.html
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)   136363 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/remote.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-08 14:29:10.975390 hansken-2023.8.8/hansken/tool/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    23624 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/tool/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11560 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/tool/_webhdfs.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11226 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/tool/command_backup.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12360 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/tool/command_extract.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3846 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/tool/command_grant.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7809 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/tool/command_mount.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11147 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/tool/command_quickstart.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4160 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/tool/command_shell.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5470 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/tool/command_stats.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4028 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/tool/command_tasks.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1705 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/tool/command_tools.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20597 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/tool/command_upload.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5347 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/tool/command_versions.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    59819 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/trace.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    20956 2023-08-08 14:28:59.000000 hansken-2023.8.8/hansken/util.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-08-08 14:29:10.971390 hansken-2023.8.8/hansken.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1476 2023-08-08 14:29:10.000000 hansken-2023.8.8/hansken.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1169 2023-08-08 14:29:10.000000 hansken-2023.8.8/hansken.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-08-08 14:29:10.000000 hansken-2023.8.8/hansken.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       45 2023-08-08 14:29:10.000000 hansken-2023.8.8/hansken.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      299 2023-08-08 14:29:10.000000 hansken-2023.8.8/hansken.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        8 2023-08-08 14:29:10.000000 hansken-2023.8.8/hansken.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-08-08 14:29:10.975390 hansken-2023.8.8/setup.cfg
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1827 2023-08-08 14:28:59.000000 hansken-2023.8.8/setup.py
```

### Comparing `hansken-2023.8.4/LICENSE` & `hansken-2023.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/PKG-INFO` & `hansken-2023.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hansken
-Version: 2023.8.4
+Version: 2023.8.8
 Summary: Python API to the Hansken REST endpoint
 Home-page: https://hansken.org/
 Author: Netherlands Forensic Institute
 Author-email: hansken-support@nfi.nl
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `hansken-2023.8.4/README.md` & `hansken-2023.8.8/README.md`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/__init__.py` & `hansken-2023.8.8/hansken/__init__.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/abstract_trace.py` & `hansken-2023.8.8/hansken/abstract_trace.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/admin.py` & `hansken-2023.8.8/hansken/admin.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/auth.py` & `hansken-2023.8.8/hansken/auth.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/connect.py` & `hansken-2023.8.8/hansken/connect.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/query.py` & `hansken-2023.8.8/hansken/query.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/recipes/export.py` & `hansken-2023.8.8/hansken/recipes/export.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/recipes/report/__init__.py` & `hansken-2023.8.8/hansken/recipes/report/__init__.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/recipes/report/templates/hansken/base.html` & `hansken-2023.8.8/hansken/recipes/report/templates/hansken/base.html`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/recipes/report/templates/hansken/macros.html` & `hansken-2023.8.8/hansken/recipes/report/templates/hansken/macros.html`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/remote.py` & `hansken-2023.8.8/hansken/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -768,14 +768,32 @@
                 self.delete_preference(preference['key'], 'project', project_id)
             except HTTPError as e:
                 log.warn('failed to delete preference {}: {}', preference['key'], e.response.text)
                 success = False
 
         return success
 
+    def reindex_project(self, project_id, shards):
+        """
+        Re-indexes a project to a specified number of shards.
+
+        :param project_id: project to be re-indexed
+        :param shards: the desired number of shards for the new index
+        :return: the task_id of the re-index task
+        """
+        response = self._session.post(
+            self.url(self.path.projects, project_id, 'index', 'reindex'),
+            json=omit_empty({
+                'shards': shards,
+            })
+        )
+        with drain(response):
+            response = _expect_ok(response, codes.created, codes.accepted)
+            return _expect_task_id(response)
+
     def clone_project(self, source_id, target_id, filter=None, exclude=None):
         """
         Clones traces of a project identified by *source_id* to a project
         *target_id*. When *filter* (a query) is provided, only traces
         matching the filter are copied.
 
         :param source_id: project to copy traces from
```

### Comparing `hansken-2023.8.4/hansken/tool/__init__.py` & `hansken-2023.8.8/hansken/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/tool/_webhdfs.py` & `hansken-2023.8.8/hansken/tool/_webhdfs.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/tool/command_backup.py` & `hansken-2023.8.8/hansken/tool/command_backup.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/tool/command_extract.py` & `hansken-2023.8.8/hansken/tool/command_extract.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/tool/command_grant.py` & `hansken-2023.8.8/hansken/tool/command_grant.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/tool/command_mount.py` & `hansken-2023.8.8/hansken/tool/command_mount.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/tool/command_quickstart.py` & `hansken-2023.8.8/hansken/tool/command_quickstart.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/tool/command_shell.py` & `hansken-2023.8.8/hansken/tool/command_shell.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/tool/command_stats.py` & `hansken-2023.8.8/hansken/tool/command_stats.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/tool/command_tasks.py` & `hansken-2023.8.8/hansken/tool/command_tasks.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/tool/command_tools.py` & `hansken-2023.8.8/hansken/tool/command_tools.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/tool/command_upload.py` & `hansken-2023.8.8/hansken/tool/command_upload.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/tool/command_versions.py` & `hansken-2023.8.8/hansken/tool/command_versions.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/trace.py` & `hansken-2023.8.8/hansken/trace.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken/util.py` & `hansken-2023.8.8/hansken/util.py`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/hansken.egg-info/PKG-INFO` & `hansken-2023.8.8/hansken.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hansken
-Version: 2023.8.4
+Version: 2023.8.8
 Summary: Python API to the Hansken REST endpoint
 Home-page: https://hansken.org/
 Author: Netherlands Forensic Institute
 Author-email: hansken-support@nfi.nl
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `hansken-2023.8.4/hansken.egg-info/SOURCES.txt` & `hansken-2023.8.8/hansken.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hansken-2023.8.4/setup.py` & `hansken-2023.8.8/setup.py`

 * *Files identical despite different names*

