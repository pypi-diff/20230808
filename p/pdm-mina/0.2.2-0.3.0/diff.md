# Comparing `tmp/pdm_mina-0.2.2.tar.gz` & `tmp/pdm_mina-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_mina-0.2.2.tar", last modified: Wed Jun 14 12:12:15 2023, max compression
+gzip compressed data, was "pdm_mina-0.3.0.tar", last modified: Tue Aug  8 08:17:11 2023, max compression
```

## Comparing `pdm_mina-0.2.2.tar` & `pdm_mina-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4153 2023-06-14 12:12:03.795548 pdm_mina-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-06-14 12:12:03.795548 pdm_mina-0.2.2/mina/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 12:12:03.795548 pdm_mina-0.2.2/mina/commands/__init__.py
--rw-r--r--   0        0        0     5621 2023-06-14 12:12:03.795548 pdm_mina-0.2.2/mina/commands/build.py
--rw-r--r--   0        0        0     1160 2023-06-14 12:12:03.795548 pdm_mina-0.2.2/mina/commands/list.py
--rw-r--r--   0        0        0      804 2023-06-14 12:12:03.795548 pdm_mina-0.2.2/mina/plugin.py
--rw-r--r--   0        0        0     1562 2023-06-14 12:12:15.960226 pdm_mina-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4394 1970-01-01 00:00:00.000000 pdm_mina-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4153 2023-08-08 08:16:55.274180 pdm_mina-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-08 08:16:55.274180 pdm_mina-0.3.0/mina/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:16:55.274180 pdm_mina-0.3.0/mina/commands/__init__.py
+-rw-r--r--   0        0        0     5621 2023-08-08 08:16:55.274180 pdm_mina-0.3.0/mina/commands/build.py
+-rw-r--r--   0        0        0     1370 2023-08-08 08:16:55.274180 pdm_mina-0.3.0/mina/commands/list.py
+-rw-r--r--   0        0        0      804 2023-08-08 08:16:55.274180 pdm_mina-0.3.0/mina/plugin.py
+-rw-r--r--   0        0        0     1596 2023-08-08 08:17:11.878402 pdm_mina-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4394 1970-01-01 00:00:00.000000 pdm_mina-0.3.0/PKG-INFO
```

### Comparing `pdm_mina-0.2.2/README.md` & `pdm_mina-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pdm_mina-0.2.2/mina/commands/build.py` & `pdm_mina-0.3.0/mina/commands/build.py`

 * *Files identical despite different names*

### Comparing `pdm_mina-0.2.2/mina/commands/list.py` & `pdm_mina-0.3.0/mina/commands/list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+from pathlib import Path
 from argparse import Namespace
 
 try:
     import tomllib as tomli  # type: ignore
 except ImportError:
     try:
         from pdm.backend._vendor import tomli
@@ -17,14 +18,19 @@
         if not (project.root / "pyproject.toml").exists():
             project.core.ui.echo("No pyproject.toml found.", err=True)
             sys.exit(1)
         pyproj = tomli.loads(
             (project.root / "pyproject.toml").read_text(encoding="utf-8")
         )
         mina_packages = pyproj.get("tool", {}).get("mina", {}).get("packages", [])
+        for i in project.root.glob(".mina/*.toml"):
+            name = i.name[:-5]
+            if name not in mina_packages:
+                mina_packages.append(name)
+                
         if not mina_packages:
             project.core.ui.echo(
                 "No mina packages found, you could add some in pyproject.toml."
             )
             sys.exit(0)
         project.core.ui.echo(
             "\n".join(
```

### Comparing `pdm_mina-0.2.2/mina/plugin.py` & `pdm_mina-0.3.0/mina/plugin.py`

 * *Files identical despite different names*

### Comparing `pdm_mina-0.2.2/pyproject.toml` & `pdm_mina-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pdm-mina"
-version = "0.2.2"
+version = "0.3.0"
 dependencies = [
     "pdm>=2.5.0",
     "mina-build>=0.2.1",
     "tomli>=1.1.0; python_version < \"3.11\"",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
@@ -39,22 +39,23 @@
 includes = [
     "mina/backend",
 ]
 raw-dependencies = []
 
 [tool.mina.packages.backend.project]
 name = "mina-build"
-version = "0.4.0"
+version = "0.5.0"
 description = "build backend for Mina Package Structure"
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
 dependencies = [
     "pdm-backend",
     "tomli",
+    "editables",
 ]
 requires-python = ">=3.9"
 readme = "README.build.md"
 
 [tool.mina.packages.backend.project.license]
 text = "MIT"
 
@@ -64,15 +65,15 @@
 ]
 excludes = [
     "mina/backend",
 ]
 
 [tool.mina.packages.cli-pdm.project]
 name = "pdm-mina"
-version = "0.2.2"
+version = "0.3.0"
 dependencies = [
     "pdm>=2.5.0",
     "mina-build>=0.2.1",
     "tomli>=1.1.0; python_version < \"3.11\"",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
@@ -82,9 +83,10 @@
 
 [tool.mina.packages.cli-pdm.project.entry-points.pdm]
 mina = "mina.plugin:ensure_pdm"
 
 [build-system]
 requires = [
     "mina-build>=0.2.6",
+    "editables",
 ]
 build-backend = "mina.backend"
```

### Comparing `pdm_mina-0.2.2/PKG-INFO` & `pdm_mina-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-mina
-Version: 0.2.2
+Version: 0.3.0
 License: MIT
 Requires-Python: >=3.9
 Requires-Dist: pdm>=2.5.0
 Requires-Dist: mina-build>=0.2.1
 Requires-Dist: tomli>=1.1.0; python_version < "3.11"
 Description-Content-Type: text/markdown
```

