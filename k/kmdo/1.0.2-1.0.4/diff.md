# Comparing `tmp/kmdo-1.0.2.tar.gz` & `tmp/kmdo-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kmdo-1.0.2.tar", last modified: Tue Feb 15 21:29:04 2022, max compression
+gzip compressed data, was "kmdo-1.0.4.tar", last modified: Tue Aug  8 12:34:05 2023, max compression
```

## Comparing `kmdo-1.0.2.tar` & `kmdo-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 21:29:04.000000 kmdo-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     2033 2022-02-15 21:29:04.000000 kmdo-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-02-15 21:28:56.000000 kmdo-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 21:29:04.000000 kmdo-1.0.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3774 2022-02-15 21:28:56.000000 kmdo-1.0.2/bin/kmdo
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 21:29:04.000000 kmdo-1.0.2/kmdo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2033 2022-02-15 21:29:04.000000 kmdo-1.0.2/kmdo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-02-15 21:29:04.000000 kmdo-1.0.2/kmdo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-15 21:29:04.000000 kmdo-1.0.2/kmdo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-15 21:29:04.000000 kmdo-1.0.2/kmdo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-15 21:29:04.000000 kmdo-1.0.2/kmdo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-15 21:29:04.000000 kmdo-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1295 2022-02-15 21:28:56.000000 kmdo-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:05.247286 kmdo-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-08-08 12:33:15.000000 kmdo-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-08-08 12:34:05.247286 kmdo-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-08 12:33:15.000000 kmdo-1.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-08 12:33:15.000000 kmdo-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-08 12:34:05.247286 kmdo-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:33:15.000000 kmdo-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:05.243286 kmdo-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:05.247286 kmdo-1.0.4/src/kmdo/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-08 12:33:15.000000 kmdo-1.0.4/src/kmdo/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3556 2023-08-08 12:33:15.000000 kmdo-1.0.4/src/kmdo/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:05.247286 kmdo-1.0.4/src/kmdo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-08-08 12:34:04.000000 kmdo-1.0.4/src/kmdo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-08 12:34:05.000000 kmdo-1.0.4/src/kmdo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:34:04.000000 kmdo-1.0.4/src/kmdo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-08 12:34:04.000000 kmdo-1.0.4/src/kmdo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:34:04.000000 kmdo-1.0.4/src/kmdo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 12:34:04.000000 kmdo-1.0.4/src/kmdo.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kmdo-1.0.2/PKG-INFO` & `kmdo-1.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: kmdo
-Version: 1.0.2
+Version: 1.0.4
 Summary: Command-line tool for auto generating command output
 Home-page: https://github.com/safl/kmdo
 Author: Simon A. F. Lund
 Author-email: os@safl.dk
-License: Apache License 2.0
+Maintainer: Simon A. F. Lund
+Maintainer-email: os@safl.dk
+License: BSD-3-Clause
+Project-URL: homepage, https://kmdo.readthedocs.io
+Project-URL: documentation, https://kmdo.readthedocs.io
+Project-URL: repository, https://github.com/safl/kmdo
 Description: kmdo - auto-generate command-line usage examples
         ================================================
         
         .. image:: https://img.shields.io/pypi/v/kmdo.svg
            :target: https://pypi.org/project/kmdo
            :alt: PyPI
         
-        .. image:: https://github.com/safl/kmdo/workflows/selftest/badge.svg
+        .. image:: https://github.com/safl/kmdo/workflows/build_check_publish/badge.svg
            :target: https://github.com/safl/kmdo/actions
            :alt: Build Status
         
         .. image:: https://readthedocs.org/projects/kmdo/badge/?version=latest
            :target: https://kmdo.readthedocs.io/en/latest/?badge=latest
            :alt: Documentation Status
         
@@ -39,12 +44,13 @@
         .. _Pull request: https://github.com/safl/kmdo/pulls
         .. _Issue: https://github.com/safl/kmdo/issues
         
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
+Description-Content-Type: text/x-rst
```

### Comparing `kmdo-1.0.2/README.rst` & `kmdo-1.0.4/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 kmdo - auto-generate command-line usage examples
 ================================================
 
 .. image:: https://img.shields.io/pypi/v/kmdo.svg
    :target: https://pypi.org/project/kmdo
    :alt: PyPI
 
-.. image:: https://github.com/safl/kmdo/workflows/selftest/badge.svg
+.. image:: https://github.com/safl/kmdo/workflows/build_check_publish/badge.svg
    :target: https://github.com/safl/kmdo/actions
    :alt: Build Status
 
 .. image:: https://readthedocs.org/projects/kmdo/badge/?version=latest
    :target: https://kmdo.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
```

### Comparing `kmdo-1.0.2/bin/kmdo` & `kmdo-1.0.4/src/kmdo/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 #!/usr/bin/env python3
 """
     Run commands from .cmd files, storing output in .out files
 """
 from __future__ import print_function
-from subprocess import Popen, PIPE
+
 import argparse
-import sys
 import os
-
-VERSION_MAJOR = 1
-VERSION_MINOR = 0
-VERSION_PATCH = 2
-VERSION = "%d.%d.%d" % (VERSION_MAJOR, VERSION_MINOR, VERSION_PATCH)
-__version__ = VERSION
+import sys
+from subprocess import PIPE, Popen
 
 
 def expand_path(path):
     """Expand variables in and provide absolute version of the given 'path'"""
 
     return os.path.abspath(os.path.expanduser(os.path.expandvars(path)))
 
 
 def update_file(fpath, content):
     """Writes 'content' to 'fpath'"""
 
-    with open(fpath, 'w+') as output:
+    with open(fpath, "w+") as output:
         output.write(content)
 
 
 def cmd_run(cmd, args):
     """Execute the given command and return stdout, stderr, and returncode"""
 
     with Popen(
-            cmd, shell=True, stdout=PIPE, stderr=PIPE, executable=args.shell
+        cmd, shell=True, stdout=PIPE, stderr=PIPE, executable=args.shell
     ) as process:
         out, err = process.communicate()
 
     return out, err, process.returncode
 
 
 def cmd_from_file(fpath):
@@ -56,15 +51,14 @@
     return cmds
 
 
 def produce_cmd_output(args):
     """Do the actual work"""
 
     for root, _, fnames in os.walk(args.path):
-
         if args.recursive and root != args.path:
             continue
 
         for fname in sorted(fname for fname in fnames if fname.endswith(".cmd")):
             cmd_fpath = os.sep.join([root, fname])
 
             out_fpath = cmd_fpath.replace(".cmd", ".out")
@@ -87,17 +81,33 @@
             if errored:
                 update_file(err_fpath, "\n".join([o.decode("utf-8") for o in output]))
 
             if not errored or uone:
                 update_file(out_fpath, "\n".join([o.decode("utf-8") for o in output]))
 
 
-def main(args):
+def parse_args():
+    parser = argparse.ArgumentParser(
+        description="Run commands from .cmd files, storing output in .out files"
+    )
+    parser.add_argument("path", type=str, help="Path to DIR containing .cmd files")
+    parser.add_argument("-r", "--recursive", action="store_true", help="go deepah!")
+    parser.add_argument("-s", "--shell", help="Absolute path to the Shell to use")
+
+    args = parser.parse_args()
+    args.path = expand_path(args.path)
+
+    return args
+
+
+def main():
     """Entry point"""
 
+    args = parse_args()
+
     nerrs = 0
 
     try:
         print("args:")
         print("  path: %r" % args.path)
         print("  recursive: %r" % args.recursive)
         print("results:")
@@ -114,31 +124,7 @@
     except OSError as exc:
         print("# err(%s)" % exc)
         return 1
 
     print("nerrs: %r" % nerrs)
 
     return nerrs
-
-if __name__ == "__main__":
-    PRSR = argparse.ArgumentParser(
-        description="Run commands from .cmd files, storing output in .out files"
-    )
-    PRSR.add_argument(
-        "path",
-        type=str,
-        help="Path to DIR containing .cmd files"
-    )
-    PRSR.add_argument(
-        "-r", "--recursive",
-        action="store_true",
-        help="go deepah!"
-    )
-    PRSR.add_argument(
-        "-s", "--shell",
-        help="Absolute path to the Shell to use"
-    )
-
-    ARGS = PRSR.parse_args()
-    ARGS.path = expand_path(ARGS.path)
-
-    sys.exit(main(ARGS))
```

### Comparing `kmdo-1.0.2/kmdo.egg-info/PKG-INFO` & `kmdo-1.0.4/src/kmdo.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: kmdo
-Version: 1.0.2
+Version: 1.0.4
 Summary: Command-line tool for auto generating command output
 Home-page: https://github.com/safl/kmdo
 Author: Simon A. F. Lund
 Author-email: os@safl.dk
-License: Apache License 2.0
+Maintainer: Simon A. F. Lund
+Maintainer-email: os@safl.dk
+License: BSD-3-Clause
+Project-URL: homepage, https://kmdo.readthedocs.io
+Project-URL: documentation, https://kmdo.readthedocs.io
+Project-URL: repository, https://github.com/safl/kmdo
 Description: kmdo - auto-generate command-line usage examples
         ================================================
         
         .. image:: https://img.shields.io/pypi/v/kmdo.svg
            :target: https://pypi.org/project/kmdo
            :alt: PyPI
         
-        .. image:: https://github.com/safl/kmdo/workflows/selftest/badge.svg
+        .. image:: https://github.com/safl/kmdo/workflows/build_check_publish/badge.svg
            :target: https://github.com/safl/kmdo/actions
            :alt: Build Status
         
         .. image:: https://readthedocs.org/projects/kmdo/badge/?version=latest
            :target: https://kmdo.readthedocs.io/en/latest/?badge=latest
            :alt: Documentation Status
         
@@ -39,12 +44,13 @@
         .. _Pull request: https://github.com/safl/kmdo/pulls
         .. _Issue: https://github.com/safl/kmdo/issues
         
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
+Description-Content-Type: text/x-rst
```

