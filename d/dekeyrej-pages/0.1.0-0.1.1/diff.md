# Comparing `tmp/dekeyrej-pages-0.1.0.tar.gz` & `tmp/dekeyrej-pages-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dekeyrej-pages-0.1.0.tar", last modified: Tue Aug  8 03:20:31 2023, max compression
+gzip compressed data, was "dekeyrej-pages-0.1.1.tar", last modified: Tue Aug  8 03:39:33 2023, max compression
```

## Comparing `dekeyrej-pages-0.1.0.tar` & `dekeyrej-pages-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 03:20:31.104384 dekeyrej-pages-0.1.0/
--rw-rw-rw-   0        0        0     1086 2023-08-08 02:48:33.000000 dekeyrej-pages-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1792 2023-08-08 03:20:31.103383 dekeyrej-pages-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       79 2023-08-08 03:15:27.000000 dekeyrej-pages-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-08 03:20:31.102383 dekeyrej-pages-0.1.0/dekeyrej_pages.egg-info/
--rw-rw-rw-   0        0        0     1792 2023-08-08 03:20:31.000000 dekeyrej-pages-0.1.0/dekeyrej_pages.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-08-08 03:20:31.000000 dekeyrej-pages-0.1.0/dekeyrej_pages.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 03:20:31.000000 dekeyrej-pages-0.1.0/dekeyrej_pages.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-08-08 03:20:31.000000 dekeyrej-pages-0.1.0/dekeyrej_pages.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 03:20:31.000000 dekeyrej-pages-0.1.0/dekeyrej_pages.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1207 2023-08-08 03:16:28.000000 dekeyrej-pages-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-08 03:20:31.104384 dekeyrej-pages-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      385 2023-08-08 03:15:43.000000 dekeyrej-pages-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 03:39:33.112674 dekeyrej-pages-0.1.1/
+-rw-rw-rw-   0        0        0     1086 2023-08-08 02:48:33.000000 dekeyrej-pages-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1792 2023-08-08 03:39:33.111674 dekeyrej-pages-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       79 2023-08-08 03:39:07.000000 dekeyrej-pages-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 03:39:33.100674 dekeyrej-pages-0.1.1/dekeyrej_pages.egg-info/
+-rw-rw-rw-   0        0        0     1792 2023-08-08 03:39:33.000000 dekeyrej-pages-0.1.1/dekeyrej_pages.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-08-08 03:39:33.000000 dekeyrej-pages-0.1.1/dekeyrej_pages.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 03:39:33.000000 dekeyrej-pages-0.1.1/dekeyrej_pages.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-08-08 03:39:33.000000 dekeyrej-pages-0.1.1/dekeyrej_pages.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-08 03:39:33.000000 dekeyrej-pages-0.1.1/dekeyrej_pages.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 03:39:33.110674 dekeyrej-pages-0.1.1/pages/
+-rw-rw-rw-   0        0        0       84 2023-08-08 03:09:12.000000 dekeyrej-pages-0.1.1/pages/__init__.py
+-rw-rw-rw-   0        0        0     6136 2023-08-08 03:13:18.000000 dekeyrej-pages-0.1.1/pages/serverpage.py
+-rw-rw-rw-   0        0        0     1207 2023-08-08 03:39:07.000000 dekeyrej-pages-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 03:39:33.112674 dekeyrej-pages-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      348 2023-08-08 03:39:07.000000 dekeyrej-pages-0.1.1/setup.py
```

### Comparing `dekeyrej-pages-0.1.0/LICENSE` & `dekeyrej-pages-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dekeyrej-pages-0.1.0/PKG-INFO` & `dekeyrej-pages-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dekeyrej-pages
-Version: 0.1.0
+Version: 0.1.1
 Summary: base classes for microservice servers and matrix display pages
 Author: J.DeKeyrel
 Author-email: "J. DeKeyrel" <noneyabusiness@notemail.com>
 License: MIT License
         
         Copyright (c) 2023 dekeyrej
         
@@ -29,9 +29,9 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pages latest {version='0.1.0'}
+# pages latest {version='0.1.1'}
 Matrix - serverpage and displaypage classes
```

### Comparing `dekeyrej-pages-0.1.0/dekeyrej_pages.egg-info/PKG-INFO` & `dekeyrej-pages-0.1.1/dekeyrej_pages.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dekeyrej-pages
-Version: 0.1.0
+Version: 0.1.1
 Summary: base classes for microservice servers and matrix display pages
 Author: J.DeKeyrel
 Author-email: "J. DeKeyrel" <noneyabusiness@notemail.com>
 License: MIT License
         
         Copyright (c) 2023 dekeyrej
         
@@ -29,9 +29,9 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pages latest {version='0.1.0'}
+# pages latest {version='0.1.1'}
 Matrix - serverpage and displaypage classes
```

### Comparing `dekeyrej-pages-0.1.0/pyproject.toml` & `dekeyrej-pages-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 00000030: 2c20 2277 6865 656c 225d 0d0a 6275 696c  , "wheel"]..buil
 00000040: 642d 6261 636b 656e 6420 3d20 2273 6574  d-backend = "set
 00000050: 7570 746f 6f6c 732e 6275 696c 645f 6d65  uptools.build_me
 00000060: 7461 220d 0a0d 0a5b 7072 6f6a 6563 745d  ta"....[project]
 00000070: 0d0a 2020 2020 6e61 6d65 203d 2022 6465  ..    name = "de
 00000080: 6b65 7972 656a 2d70 6167 6573 220d 0a20  keyrej-pages".. 
 00000090: 2020 2076 6572 7369 6f6e 203d 2022 302e     version = "0.
-000000a0: 312e 3022 0d0a 2020 2020 6465 7363 7269  1.0"..    descri
+000000a0: 312e 3122 0d0a 2020 2020 6465 7363 7269  1.1"..    descri
 000000b0: 7074 696f 6e20 3d20 2262 6173 6520 636c  ption = "base cl
 000000c0: 6173 7365 7320 666f 7220 6d69 6372 6f73  asses for micros
 000000d0: 6572 7669 6365 2073 6572 7665 7273 2061  ervice servers a
 000000e0: 6e64 206d 6174 7269 7820 6469 7370 6c61  nd matrix displa
 000000f0: 7920 7061 6765 7322 0d0a 2020 2020 7265  y pages"..    re
 00000100: 6164 6d65 203d 2022 5245 4144 4d45 2e6d  adme = "README.m
 00000110: 6422 0d0a 2020 2020 6175 7468 6f72 7320  d"..    authors 
@@ -40,15 +40,15 @@
 00000270: 736f 7572 6365 222c 0d0a 2020 2020 2020  source",..      
 00000280: 2020 2264 656b 6579 7265 6a2d 7365 6375    "dekeyrej-secu
 00000290: 7265 6469 6374 222c 0d0a 2020 2020 5d0d  redict",..    ].
 000002a0: 0a20 2020 2072 6571 7569 7265 732d 7079  .    requires-py
 000002b0: 7468 6f6e 203d 2022 3e3d 332e 3922 0d0a  thon = ">=3.9"..
 000002c0: 0d0a 5b74 6f6f 6c2e 6275 6d70 7665 725d  ..[tool.bumpver]
 000002d0: 0d0a 6375 7272 656e 745f 7665 7273 696f  ..current_versio
-000002e0: 6e20 3d20 2230 2e31 2e30 220d 0a76 6572  n = "0.1.0"..ver
+000002e0: 6e20 3d20 2230 2e31 2e31 220d 0a76 6572  n = "0.1.1"..ver
 000002f0: 7369 6f6e 5f70 6174 7465 726e 203d 2022  sion_pattern = "
 00000300: 274d 414a 4f52 2e4d 494e 4f52 2e50 4154  'MAJOR.MINOR.PAT
 00000310: 4348 5b50 5954 4147 4e55 4d5d 220d 0a63  CH[PYTAGNUM]"..c
 00000320: 6f6d 6d69 745f 6d65 7373 6167 6520 3d20  ommit_message = 
 00000330: 2262 756d 7020 7665 7273 696f 6e20 7b6f  "bump version {o
 00000340: 6c64 5f76 6572 7369 6f6e 7d20 2d3e 207b  ld_version} -> {
 00000350: 6e65 775f 7665 7273 696f 6e7d 220d 0a74  new_version}"..t
```

