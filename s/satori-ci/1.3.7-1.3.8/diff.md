# Comparing `tmp/satori_ci-1.3.7.tar.gz` & `tmp/satori_ci-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_ci-1.3.7.tar", last modified: Thu Aug  3 23:17:00 2023, max compression
+gzip compressed data, was "satori_ci-1.3.8.tar", last modified: Tue Aug  8 20:47:05 2023, max compression
```

## Comparing `satori_ci-1.3.7.tar` & `satori_ci-1.3.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-08-03 23:16:41.897454 satori_ci-1.3.7/LICENSE
--rw-r--r--   0        0        0     7140 2023-08-03 23:16:41.897454 satori_ci-1.3.7/README.md
--rw-r--r--   0        0        0      755 2023-08-03 23:17:00.594571 satori_ci-1.3.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-03 23:16:41.897454 satori_ci-1.3.7/src/satoricli/__init__.py
--rw-r--r--   0        0        0       37 2023-08-03 23:16:41.897454 satori_ci-1.3.7/src/satoricli/__main__.py
--rw-r--r--   0        0        0     4551 2023-08-03 23:16:41.897454 satori_ci-1.3.7/src/satoricli/classes/api.py
--rw-r--r--   0        0        0     1633 2023-08-03 23:16:41.897454 satori_ci-1.3.7/src/satoricli/classes/bundler.py
--rw-r--r--   0        0        0      484 2023-08-03 23:16:41.897454 satori_ci-1.3.7/src/satoricli/classes/models.py
--rw-r--r--   0        0        0     3345 2023-08-03 23:16:41.897454 satori_ci-1.3.7/src/satoricli/classes/playbooks.py
--rw-r--r--   0        0        0    27829 2023-08-03 23:16:41.897454 satori_ci-1.3.7/src/satoricli/classes/satori.py
--rw-r--r--   0        0        0    13678 2023-08-03 23:16:41.897454 satori_ci-1.3.7/src/satoricli/classes/utils.py
--rw-r--r--   0        0        0     1194 2023-08-03 23:16:41.897454 satori_ci-1.3.7/src/satoricli/classes/validations.py
--rwxr-xr-x   0        0        0     9997 2023-08-03 23:16:41.897454 satori_ci-1.3.7/src/satoricli/cli/parser.py
--rw-r--r--   0        0        0    48305 1970-01-01 00:00:00.000000 satori_ci-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-08 20:46:50.372381 satori_ci-1.3.8/LICENSE
+-rw-r--r--   0        0        0     7140 2023-08-08 20:46:50.372381 satori_ci-1.3.8/README.md
+-rw-r--r--   0        0        0      755 2023-08-08 20:47:05.620351 satori_ci-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-08 20:46:50.372381 satori_ci-1.3.8/src/satoricli/__init__.py
+-rw-r--r--   0        0        0       37 2023-08-08 20:46:50.372381 satori_ci-1.3.8/src/satoricli/__main__.py
+-rw-r--r--   0        0        0     4551 2023-08-08 20:46:50.372381 satori_ci-1.3.8/src/satoricli/classes/api.py
+-rw-r--r--   0        0        0     1633 2023-08-08 20:46:50.372381 satori_ci-1.3.8/src/satoricli/classes/bundler.py
+-rw-r--r--   0        0        0      484 2023-08-08 20:46:50.372381 satori_ci-1.3.8/src/satoricli/classes/models.py
+-rw-r--r--   0        0        0     3345 2023-08-08 20:46:50.372381 satori_ci-1.3.8/src/satoricli/classes/playbooks.py
+-rw-r--r--   0        0        0    28140 2023-08-08 20:46:50.372381 satori_ci-1.3.8/src/satoricli/classes/satori.py
+-rw-r--r--   0        0        0    13678 2023-08-08 20:46:50.372381 satori_ci-1.3.8/src/satoricli/classes/utils.py
+-rw-r--r--   0        0        0     1194 2023-08-08 20:46:50.372381 satori_ci-1.3.8/src/satoricli/classes/validations.py
+-rwxr-xr-x   0        0        0     9997 2023-08-08 20:46:50.372381 satori_ci-1.3.8/src/satoricli/cli/parser.py
+-rw-r--r--   0        0        0    48305 1970-01-01 00:00:00.000000 satori_ci-1.3.8/PKG-INFO
```

### Comparing `satori_ci-1.3.7/LICENSE` & `satori_ci-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.7/README.md` & `satori_ci-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.7/pyproject.toml` & `satori_ci-1.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satori-ci"
-version = "1.3.7"
+version = "1.3.8"
 description = "Satori CI - Automated Software Testing Platform"
 authors = [
     { name = "Satori CI CLI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "requests>=2.27.1",
     "pyyaml>=6.0",
```

### Comparing `satori_ci-1.3.7/src/satoricli/classes/api.py` & `satori_ci-1.3.8/src/satoricli/classes/api.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.7/src/satoricli/classes/bundler.py` & `satori_ci-1.3.8/src/satoricli/classes/bundler.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.7/src/satoricli/classes/playbooks.py` & `satori_ci-1.3.8/src/satoricli/classes/playbooks.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.7/src/satoricli/classes/satori.py` & `satori_ci-1.3.8/src/satoricli/classes/satori.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,24 +151,32 @@
         if path.is_dir():
             playbook = path / ".satori.yml"
         elif path.is_file():
             playbook = path
         else:
             puts(FAIL_COLOR, "Playbook file or folder not found")
             sys.exit(1)
+        
+        try:
+            playbook_text = playbook.read_text()
+        except FileNotFoundError:
+            console.print(f"Error: playbook not found", e)
+            sys.exit(1)
 
-        playbook_text = playbook.read_text()
         config = None
 
         try:
             config = yaml.safe_load(playbook_text)
 
             with warnings.catch_warnings(record=True) as w:
-                validate_playbook(config)
-
+                try:
+                    validate_playbook(config)
+                except TypeError:
+                    console.print(f"Error: playbook not found or invalid", e)
+                    sys.exit(1)
             for warning in w:
                 if warning.category == NoLogMonitorWarning:
                     console.print(
                         "[warning]WARNING:[/] No notifications (log, onLogFail or onLogPass) were defined for the Monitor"
                     )
         except yaml.YAMLError as e:
             console.print(f"Error parsing the playbook [bold]{playbook.name}[/]:\n", e)
```

### Comparing `satori_ci-1.3.7/src/satoricli/classes/utils.py` & `satori_ci-1.3.8/src/satoricli/classes/utils.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.7/src/satoricli/classes/validations.py` & `satori_ci-1.3.8/src/satoricli/classes/validations.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.7/src/satoricli/cli/parser.py` & `satori_ci-1.3.8/src/satoricli/cli/parser.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.7/PKG-INFO` & `satori_ci-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satori-ci
-Version: 1.3.7
+Version: 1.3.8
 Summary: Satori CI - Automated Software Testing Platform
 Author-Email: Satori CI CLI <info@satori-ci.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

