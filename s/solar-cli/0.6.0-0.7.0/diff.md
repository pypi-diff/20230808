# Comparing `tmp/solar_cli-0.6.0.tar.gz` & `tmp/solar_cli-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solar_cli-0.6.0.tar", max compression
+gzip compressed data, was "solar_cli-0.7.0.tar", max compression
```

## Comparing `solar_cli-0.6.0.tar` & `solar_cli-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     3121 2023-08-08 08:54:08.454260 solar_cli-0.6.0/README.md
--rw-r--r--   0        0        0      612 2023-08-08 08:54:08.454260 solar_cli-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       36 2023-08-08 08:54:08.454260 solar_cli-0.6.0/solar/__init__.py
--rw-r--r--   0        0        0        0 2023-08-08 08:54:08.454260 solar_cli-0.6.0/solar/api/__init__.py
--rw-r--r--   0        0        0     6347 2023-08-08 08:58:23.614207 solar_cli-0.6.0/solar/api/base.py
--rw-r--r--   0        0        0     7900 2023-08-08 08:54:08.454260 solar_cli-0.6.0/solar/api/export.py
--rw-r--r--   0        0        0     7879 2023-08-08 08:57:33.484230 solar_cli-0.6.0/solar/api/import_.py
--rw-r--r--   0        0        0     6152 2023-08-08 08:57:03.184229 solar_cli-0.6.0/solar/cli.py
--rw-r--r--   0        0        0       98 2023-08-08 08:54:08.454260 solar_cli-0.6.0/solar/cmd/__init__.py
--rw-r--r--   0        0        0     2011 2023-08-08 08:58:36.034207 solar_cli-0.6.0/solar/cmd/export.py
--rw-r--r--   0        0        0     1665 2023-08-08 08:58:10.424206 solar_cli-0.6.0/solar/cmd/import_.py
--rw-r--r--   0        0        0        0 2023-08-08 08:54:08.464260 solar_cli-0.6.0/solar/types/__init__.py
--rw-r--r--   0        0        0      481 2023-08-08 08:54:08.464260 solar_cli-0.6.0/solar/types/analysis.py
--rw-r--r--   0        0        0      141 2023-08-08 08:54:08.464260 solar_cli-0.6.0/solar/types/base.py
--rw-r--r--   0        0        0     1278 2023-08-08 08:54:08.464260 solar_cli-0.6.0/solar/types/cluster_status.py
--rw-r--r--   0        0        0      331 2023-08-08 08:54:08.464260 solar_cli-0.6.0/solar/types/config_files.py
--rw-r--r--   0        0        0        0 2023-08-08 08:54:08.464260 solar_cli-0.6.0/solar/utils.py
--rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 solar_cli-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     3121 2023-08-08 08:54:08.454260 solar_cli-0.7.0/README.md
+-rw-r--r--   0        0        0      612 2023-08-08 09:36:56.995778 solar_cli-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-08-08 09:33:57.514927 solar_cli-0.7.0/solar/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:54:08.454260 solar_cli-0.7.0/solar/api/__init__.py
+-rw-r--r--   0        0        0     6347 2023-08-08 08:58:23.614207 solar_cli-0.7.0/solar/api/base.py
+-rw-r--r--   0        0        0     7900 2023-08-08 08:54:08.454260 solar_cli-0.7.0/solar/api/export.py
+-rw-r--r--   0        0        0     7983 2023-08-08 09:35:59.038813 solar_cli-0.7.0/solar/api/import_.py
+-rw-r--r--   0        0        0     6183 2023-08-08 09:34:30.219283 solar_cli-0.7.0/solar/cli.py
+-rw-r--r--   0        0        0       98 2023-08-08 08:54:08.454260 solar_cli-0.7.0/solar/cmd/__init__.py
+-rw-r--r--   0        0        0     2011 2023-08-08 08:58:36.034207 solar_cli-0.7.0/solar/cmd/export.py
+-rw-r--r--   0        0        0     1665 2023-08-08 08:58:10.424206 solar_cli-0.7.0/solar/cmd/import_.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:54:08.464260 solar_cli-0.7.0/solar/types/__init__.py
+-rw-r--r--   0        0        0      481 2023-08-08 08:54:08.464260 solar_cli-0.7.0/solar/types/analysis.py
+-rw-r--r--   0        0        0      141 2023-08-08 08:54:08.464260 solar_cli-0.7.0/solar/types/base.py
+-rw-r--r--   0        0        0     1278 2023-08-08 08:54:08.464260 solar_cli-0.7.0/solar/types/cluster_status.py
+-rw-r--r--   0        0        0      331 2023-08-08 08:54:08.464260 solar_cli-0.7.0/solar/types/config_files.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:54:08.464260 solar_cli-0.7.0/solar/utils.py
+-rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 solar_cli-0.7.0/PKG-INFO
```

### Comparing `solar_cli-0.6.0/README.md` & `solar_cli-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `solar_cli-0.6.0/pyproject.toml` & `solar_cli-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solar-cli"
-version = "0.6.0"
+version = "0.7.0"
 description = "CLI app for Solr"
 authors = ["Andrey S. <andrewsapw@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "solar" },
 ]
```

### Comparing `solar_cli-0.6.0/solar/api/base.py` & `solar_cli-0.7.0/solar/api/base.py`

 * *Files identical despite different names*

### Comparing `solar_cli-0.6.0/solar/api/export.py` & `solar_cli-0.7.0/solar/api/export.py`

 * *Files identical despite different names*

### Comparing `solar_cli-0.6.0/solar/api/import_.py` & `solar_cli-0.7.0/solar/api/import_.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from rich.progress import (
     BarColumn,
     Progress,
     TaskProgressColumn,
     TextColumn,
     TimeRemainingColumn,
 )
+import solar
 
 from solar.api.base import ApiEngine
 
 logger = logging.getLogger("root")
 
 
 def recursive_field_remove(doc: dict, field: str):
@@ -136,18 +137,19 @@
             collection_name = collection
 
         print("Begin import with params:")
         print(f"Source file: [bold]{path}")
         print(f"Batch size: [bold]{batch_size}")
         print(f"Collection: [bold]{collection_name}")
 
-        confirm = input("Correct? (y/n)").lower() == "y"
-        if not confirm:
-            print("[red]Отмена...")
-            return
+        if not solar.FORCE:
+            confirm = input("Correct? (y/n)").lower() == "y"
+            if not confirm:
+                print("[red]Отмена...")
+                return
 
         num_docs = len(upload_docs)
 
         with Progress(
             TextColumn("[progress.description]{task.description}"),
             BarColumn(),
             TaskProgressColumn(),
@@ -212,18 +214,19 @@
         if name is None:
             name = configs_path.name
 
         print("Import params:")
         print(f"Source config: [bold]{name}[/bold]")
         print(f"Overwrite: [bold]{overwrite}[/bold]")
 
-        confirm = input("Correct? (y/n)")
-        if confirm.lower() != "y":
-            print("[red]Stopping...")
-            os._exit(1)
+        if not solar.FORCE:
+            confirm = input("Correct? (y/n)")
+            if confirm.lower() != "y":
+                print("[red]Stopping...")
+                os._exit(1)
 
         if overwrite:
             print("Removing old config...", end=" ")
             await self._remove_config(name=name)
 
         print("Creating new config...")
         upload_url = "/solr/admin/configs"
```

### Comparing `solar_cli-0.6.0/solar/cli.py` & `solar_cli-0.7.0/solar/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pathlib
 import urllib.parse
 from functools import wraps
 
 import click
 from rich import print
 
+import solar
 from solar.api.base import ApiEngine
 from solar.api.export import Exporter
 from solar.api.import_ import Importer
 from solar.types.cluster_status import Collection
 
 
 def coro(f):
@@ -29,19 +30,20 @@
 @click.pass_context
 def cli(ctx, query: str, collection: str, url: str):
     """Solr CLI"""
     url_parsed = urllib.parse.urlparse(url)
     if url_parsed.scheme not in ("http", "https"):
         print(f"[red]Unknown scheme {url_parsed.scheme}")
         exit(1)
-        
 
     username = url_parsed.username
     password = url_parsed.password
 
+    solar.FORCE = False
+
     url_str = f"{url_parsed.scheme}://{url_parsed.hostname}:{url_parsed.port}{url_parsed.path}"
 
     ctx.ensure_object(dict)
     ctx.obj["query"] = query
     ctx.obj["url"] = url_str
     ctx.obj["collection"] = collection
     ctx.obj["username"] = username
```

### Comparing `solar_cli-0.6.0/solar/cmd/export.py` & `solar_cli-0.7.0/solar/cmd/export.py`

 * *Files identical despite different names*

### Comparing `solar_cli-0.6.0/solar/cmd/import_.py` & `solar_cli-0.7.0/solar/cmd/import_.py`

 * *Files identical despite different names*

### Comparing `solar_cli-0.6.0/solar/types/cluster_status.py` & `solar_cli-0.7.0/solar/types/cluster_status.py`

 * *Files identical despite different names*

### Comparing `solar_cli-0.6.0/PKG-INFO` & `solar_cli-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solar-cli
-Version: 0.6.0
+Version: 0.7.0
 Summary: CLI app for Solr
 License: MIT
 Author: Andrey S.
 Author-email: andrewsapw@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

