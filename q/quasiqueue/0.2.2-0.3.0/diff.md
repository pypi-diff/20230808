# Comparing `tmp/quasiqueue-0.2.2.tar.gz` & `tmp/quasiqueue-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quasiqueue-0.2.2.tar", last modified: Wed Feb  1 04:14:21 2023, max compression
+gzip compressed data, was "quasiqueue-0.3.0.tar", last modified: Tue Aug  8 19:26:16 2023, max compression
```

## Comparing `quasiqueue-0.2.2.tar` & `quasiqueue-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 04:14:21.939861 quasiqueue-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-01 04:13:55.000000 quasiqueue-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-02-01 04:14:21.939861 quasiqueue-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-02-01 04:13:55.000000 quasiqueue-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-01 04:13:55.000000 quasiqueue-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 04:14:21.939861 quasiqueue-0.2.2/quasiqueue/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-01 04:13:55.000000 quasiqueue-0.2.2/quasiqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-01 04:14:21.939861 quasiqueue-0.2.2/quasiqueue/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-02-01 04:13:55.000000 quasiqueue-0.2.2/quasiqueue/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-02-01 04:13:55.000000 quasiqueue-0.2.2/quasiqueue/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-02-01 04:13:55.000000 quasiqueue-0.2.2/quasiqueue/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-02-01 04:13:55.000000 quasiqueue-0.2.2/quasiqueue/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-02-01 04:13:55.000000 quasiqueue-0.2.2/quasiqueue/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 04:14:21.939861 quasiqueue-0.2.2/quasiqueue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-02-01 04:14:21.000000 quasiqueue-0.2.2/quasiqueue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-01 04:14:21.000000 quasiqueue-0.2.2/quasiqueue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 04:14:21.000000 quasiqueue-0.2.2/quasiqueue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-01 04:14:21.000000 quasiqueue-0.2.2/quasiqueue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-01 04:14:21.000000 quasiqueue-0.2.2/quasiqueue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-01 04:14:21.000000 quasiqueue-0.2.2/quasiqueue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-01 04:14:21.939861 quasiqueue-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-01 04:13:55.000000 quasiqueue-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 04:14:21.939861 quasiqueue-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 04:13:55.000000 quasiqueue-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-01 04:13:55.000000 quasiqueue-0.2.2/tests/test_quasiqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:26:16.105544 quasiqueue-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-08 19:25:26.000000 quasiqueue-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-08-08 19:26:16.105544 quasiqueue-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-08-08 19:25:26.000000 quasiqueue-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-08 19:25:26.000000 quasiqueue-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:26:16.105544 quasiqueue-0.3.0/quasiqueue/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-08 19:25:26.000000 quasiqueue-0.3.0/quasiqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-08 19:26:16.109544 quasiqueue-0.3.0/quasiqueue/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-08-08 19:25:26.000000 quasiqueue-0.3.0/quasiqueue/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-08 19:25:26.000000 quasiqueue-0.3.0/quasiqueue/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-08-08 19:25:26.000000 quasiqueue-0.3.0/quasiqueue/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-08-08 19:25:26.000000 quasiqueue-0.3.0/quasiqueue/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-08 19:25:26.000000 quasiqueue-0.3.0/quasiqueue/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:26:16.105544 quasiqueue-0.3.0/quasiqueue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-08-08 19:26:16.000000 quasiqueue-0.3.0/quasiqueue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-08 19:26:16.000000 quasiqueue-0.3.0/quasiqueue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 19:26:16.000000 quasiqueue-0.3.0/quasiqueue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 19:26:16.000000 quasiqueue-0.3.0/quasiqueue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-08 19:26:16.000000 quasiqueue-0.3.0/quasiqueue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-08 19:26:16.000000 quasiqueue-0.3.0/quasiqueue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-08-08 19:26:16.109544 quasiqueue-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-08 19:25:26.000000 quasiqueue-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:26:16.105544 quasiqueue-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:25:26.000000 quasiqueue-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-08 19:25:26.000000 quasiqueue-0.3.0/tests/test_quasiqueue.py
```

### Comparing `quasiqueue-0.2.2/LICENSE` & `quasiqueue-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quasiqueue-0.2.2/PKG-INFO` & `quasiqueue-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quasiqueue
-Version: 0.2.2
+Version: 0.3.0
 Summary: A Simple High Performance Multiprocess Queue
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # QuasiQueue
```

### Comparing `quasiqueue-0.2.2/README.md` & `quasiqueue-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `quasiqueue-0.2.2/pyproject.toml` & `quasiqueue-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quasiqueue-0.2.2/quasiqueue/builder.py` & `quasiqueue-0.3.0/quasiqueue/builder.py`

 * *Files identical despite different names*

### Comparing `quasiqueue-0.2.2/quasiqueue/cli.py` & `quasiqueue-0.3.0/quasiqueue/cli.py`

 * *Files identical despite different names*

### Comparing `quasiqueue-0.2.2/quasiqueue/reader.py` & `quasiqueue-0.3.0/quasiqueue/reader.py`

 * *Files identical despite different names*

### Comparing `quasiqueue-0.2.2/quasiqueue/runner.py` & `quasiqueue-0.3.0/quasiqueue/runner.py`

 * *Files identical despite different names*

### Comparing `quasiqueue-0.2.2/quasiqueue/settings.py` & `quasiqueue-0.3.0/quasiqueue/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from pydantic import BaseSettings, Field
+from pydantic import Field
+from pydantic_settings import BaseSettings
 
 
 class Settings(BaseSettings):
     num_processes: int = Field(default=2, description="The number of reader processes to run.")
     max_queue_size: int = Field(default=300, description="The max allowed six of the queue.")
     prevent_requeuing_time: float = Field(
         default=300, description="The time in seconds that an item will be prevented from being readded to the queue."
```

### Comparing `quasiqueue-0.2.2/quasiqueue.egg-info/PKG-INFO` & `quasiqueue-0.3.0/quasiqueue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quasiqueue
-Version: 0.2.2
+Version: 0.3.0
 Summary: A Simple High Performance Multiprocess Queue
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # QuasiQueue
```

### Comparing `quasiqueue-0.2.2/setup.cfg` & `quasiqueue-0.3.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -21,27 +21,28 @@
 00000140: 3d20 760a 7061 7265 6e74 6469 725f 7072  = v.parentdir_pr
 00000150: 6566 6978 203d 200a 0a5b 6f70 7469 6f6e  efix = ..[option
 00000160: 735d 0a70 6163 6b61 6765 7320 3d20 6669  s].packages = fi
 00000170: 6e64 3a0a 696e 636c 7564 655f 7061 636b  nd:.include_pack
 00000180: 6167 655f 6461 7461 203d 2054 7275 650a  age_data = True.
 00000190: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
 000001a0: 203d 200a 0970 7375 7469 6c0a 0970 7964   = ..psutil..pyd
-000001b0: 616e 7469 630a 0974 7970 6572 0a0a 5b6f  antic..typer..[o
-000001c0: 7074 696f 6e73 2e65 7874 7261 735f 7265  ptions.extras_re
-000001d0: 7175 6972 655d 0a64 6576 203d 200a 0962  quire].dev = ..b
-000001e0: 6c61 636b 0a09 6275 696c 640a 0964 6170  lack..build..dap
-000001f0: 7065 7264 6174 610a 0967 6c6f 6d0a 0969  perdata..glom..i
-00000200: 736f 7274 0a09 6d79 7079 0a09 7079 7465  sort..mypy..pyte
-00000210: 7374 0a09 7079 7465 7374 2d63 6f76 0a09  st..pytest-cov..
-00000220: 7079 7465 7374 2d70 7265 7474 790a 0972  pytest-pretty..r
-00000230: 7561 6d65 6c2e 7961 6d6c 0a09 7479 7065  uamel.yaml..type
-00000240: 732d 7073 7574 696c 0a0a 5b6f 7074 696f  s-psutil..[optio
-00000250: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
-00000260: 0a71 7561 7369 7175 6575 6520 3d20 7079  .quasiqueue = py
-00000270: 2e74 7970 6564 0a0a 5b6f 7074 696f 6e73  .typed..[options
-00000280: 2e65 6e74 7279 5f70 6f69 6e74 735d 0a63  .entry_points].c
-00000290: 6f6e 736f 6c65 5f73 6372 6970 7473 203d  onsole_scripts =
-000002a0: 200a 0971 7561 7369 7175 6575 6520 3d20   ..quasiqueue = 
-000002b0: 7175 6173 6971 7565 7565 2e63 6c69 3a61  quasiqueue.cli:a
-000002c0: 7070 0a0a 5b65 6767 5f69 6e66 6f5d 0a74  pp..[egg_info].t
-000002d0: 6167 5f62 7569 6c64 203d 200a 7461 675f  ag_build = .tag_
-000002e0: 6461 7465 203d 2030 0a0a                 date = 0..
+000001b0: 616e 7469 630a 0970 7964 616e 7469 632d  antic..pydantic-
+000001c0: 7365 7474 696e 6773 0a09 7479 7065 720a  settings..typer.
+000001d0: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
+000001e0: 5f72 6571 7569 7265 5d0a 6465 7620 3d20  _require].dev = 
+000001f0: 0a09 626c 6163 6b0a 0962 7569 6c64 0a09  ..black..build..
+00000200: 6461 7070 6572 6461 7461 0a09 676c 6f6d  dapperdata..glom
+00000210: 0a09 6973 6f72 740a 096d 7970 790a 0970  ..isort..mypy..p
+00000220: 7974 6573 740a 0970 7974 6573 742d 636f  ytest..pytest-co
+00000230: 760a 0970 7974 6573 742d 7072 6574 7479  v..pytest-pretty
+00000240: 0a09 7275 616d 656c 2e79 616d 6c0a 0974  ..ruamel.yaml..t
+00000250: 7970 6573 2d70 7375 7469 6c0a 0a5b 6f70  ypes-psutil..[op
+00000260: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
+00000270: 7461 5d0a 7175 6173 6971 7565 7565 203d  ta].quasiqueue =
+00000280: 2070 792e 7479 7065 640a 0a5b 6f70 7469   py.typed..[opti
+00000290: 6f6e 732e 656e 7472 795f 706f 696e 7473  ons.entry_points
+000002a0: 5d0a 636f 6e73 6f6c 655f 7363 7269 7074  ].console_script
+000002b0: 7320 3d20 0a09 7175 6173 6971 7565 7565  s = ..quasiqueue
+000002c0: 203d 2071 7561 7369 7175 6575 652e 636c   = quasiqueue.cl
+000002d0: 693a 6170 700a 0a5b 6567 675f 696e 666f  i:app..[egg_info
+000002e0: 5d0a 7461 675f 6275 696c 6420 3d20 0a74  ].tag_build = .t
+000002f0: 6167 5f64 6174 6520 3d20 300a 0a         ag_date = 0..
```

