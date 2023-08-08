# Comparing `tmp/kmdo-1.0.4.tar.gz` & `tmp/kmdo-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmdo-1.0.4.tar", last modified: Tue Aug  8 12:34:05 2023, max compression
+gzip compressed data, was "kmdo-1.0.5.tar", last modified: Tue Aug  8 12:54:27 2023, max compression
```

## Comparing `kmdo-1.0.4.tar` & `kmdo-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:05.247286 kmdo-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-08-08 12:33:15.000000 kmdo-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-08-08 12:34:05.247286 kmdo-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-08 12:33:15.000000 kmdo-1.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-08 12:33:15.000000 kmdo-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-08 12:34:05.247286 kmdo-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:33:15.000000 kmdo-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:05.243286 kmdo-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:05.247286 kmdo-1.0.4/src/kmdo/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-08 12:33:15.000000 kmdo-1.0.4/src/kmdo/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3556 2023-08-08 12:33:15.000000 kmdo-1.0.4/src/kmdo/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:05.247286 kmdo-1.0.4/src/kmdo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-08-08 12:34:04.000000 kmdo-1.0.4/src/kmdo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-08 12:34:05.000000 kmdo-1.0.4/src/kmdo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:34:04.000000 kmdo-1.0.4/src/kmdo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-08 12:34:04.000000 kmdo-1.0.4/src/kmdo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:34:04.000000 kmdo-1.0.4/src/kmdo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 12:34:04.000000 kmdo-1.0.4/src/kmdo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:54:27.112393 kmdo-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-08-08 12:53:45.000000 kmdo-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-08-08 12:54:27.112393 kmdo-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-08 12:53:45.000000 kmdo-1.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-08 12:53:45.000000 kmdo-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-08 12:54:27.112393 kmdo-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:53:45.000000 kmdo-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:54:27.112393 kmdo-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:54:27.112393 kmdo-1.0.5/src/kmdo/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-08 12:53:45.000000 kmdo-1.0.5/src/kmdo/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3723 2023-08-08 12:53:45.000000 kmdo-1.0.5/src/kmdo/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:54:27.112393 kmdo-1.0.5/src/kmdo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-08-08 12:54:26.000000 kmdo-1.0.5/src/kmdo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-08 12:54:26.000000 kmdo-1.0.5/src/kmdo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:54:26.000000 kmdo-1.0.5/src/kmdo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-08 12:54:26.000000 kmdo-1.0.5/src/kmdo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:54:26.000000 kmdo-1.0.5/src/kmdo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 12:54:26.000000 kmdo-1.0.5/src/kmdo.egg-info/top_level.txt
```

### Comparing `kmdo-1.0.4/LICENSE` & `kmdo-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kmdo-1.0.4/PKG-INFO` & `kmdo-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmdo
-Version: 1.0.4
+Version: 1.0.5
 Summary: Command-line tool for auto generating command output
 Home-page: https://github.com/safl/kmdo
 Author: Simon A. F. Lund
 Author-email: os@safl.dk
 Maintainer: Simon A. F. Lund
 Maintainer-email: os@safl.dk
 License: BSD-3-Clause
```

### Comparing `kmdo-1.0.4/README.rst` & `kmdo-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `kmdo-1.0.4/setup.cfg` & `kmdo-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `kmdo-1.0.4/src/kmdo/cli.py` & `kmdo-1.0.5/src/kmdo/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,17 @@
     """Do the actual work"""
 
     for root, _, fnames in os.walk(args.path):
         if args.recursive and root != args.path:
             continue
 
         for fname in sorted(fname for fname in fnames if fname.endswith(".cmd")):
+            if args.exclude in args.exclude in fname:
+                continue
+
             cmd_fpath = os.sep.join([root, fname])
 
             out_fpath = cmd_fpath.replace(".cmd", ".out")
             err_fpath = cmd_fpath.replace(".cmd", ".err")
             uone = cmd_fpath.endswith(".uone.cmd")
             output = []
             errored = False
@@ -88,14 +91,15 @@
 def parse_args():
     parser = argparse.ArgumentParser(
         description="Run commands from .cmd files, storing output in .out files"
     )
     parser.add_argument("path", type=str, help="Path to DIR containing .cmd files")
     parser.add_argument("-r", "--recursive", action="store_true", help="go deepah!")
     parser.add_argument("-s", "--shell", help="Absolute path to the Shell to use")
+    parser.add_argument("-x", "--exclude", help="Exclude command-files matching this")
 
     args = parser.parse_args()
     args.path = expand_path(args.path)
 
     return args
```

### Comparing `kmdo-1.0.4/src/kmdo.egg-info/PKG-INFO` & `kmdo-1.0.5/src/kmdo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmdo
-Version: 1.0.4
+Version: 1.0.5
 Summary: Command-line tool for auto generating command output
 Home-page: https://github.com/safl/kmdo
 Author: Simon A. F. Lund
 Author-email: os@safl.dk
 Maintainer: Simon A. F. Lund
 Maintainer-email: os@safl.dk
 License: BSD-3-Clause
```

