# Comparing `tmp/somatorioInteiros-0.0.0.1.tar.gz` & `tmp/somatorioInteiros-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somatorioInteiros-0.0.0.1.tar", last modified: Tue Aug  8 12:44:59 2023, max compression
+gzip compressed data, was "somatorioInteiros-0.0.0.2.tar", last modified: Tue Aug  8 13:10:47 2023, max compression
```

## Comparing `somatorioInteiros-0.0.0.1.tar` & `somatorioInteiros-0.0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 12:44:59.852802 somatorioInteiros-0.0.0.1/
--rw-rw-rw-   0        0        0     1096 2023-08-08 12:21:35.000000 somatorioInteiros-0.0.0.1/LICENSE
--rw-rw-rw-   0        0        0      718 2023-08-08 12:44:59.852802 somatorioInteiros-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-08-08 11:51:28.000000 somatorioInteiros-0.0.0.1/README.md
--rw-rw-rw-   0        0        0      106 2023-08-08 12:06:17.000000 somatorioInteiros-0.0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      565 2023-08-08 12:44:59.852802 somatorioInteiros-0.0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-08 12:44:59.817908 somatorioInteiros-0.0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-08 12:44:59.849134 somatorioInteiros-0.0.0.1/src/somatorioInteiros.egg-info/
--rw-rw-rw-   0        0        0      718 2023-08-08 12:44:59.000000 somatorioInteiros-0.0.0.1/src/somatorioInteiros.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-08-08 12:44:59.000000 somatorioInteiros-0.0.0.1/src/somatorioInteiros.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 12:44:59.000000 somatorioInteiros-0.0.0.1/src/somatorioInteiros.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 12:44:59.000000 somatorioInteiros-0.0.0.1/src/somatorioInteiros.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 13:10:47.483384 somatorioInteiros-0.0.0.2/
+-rw-rw-rw-   0        0        0     1096 2023-08-08 12:21:35.000000 somatorioInteiros-0.0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      720 2023-08-08 13:10:47.483384 somatorioInteiros-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-08-08 11:51:28.000000 somatorioInteiros-0.0.0.2/README.md
+-rw-rw-rw-   0        0        0      106 2023-08-08 12:06:17.000000 somatorioInteiros-0.0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      567 2023-08-08 13:10:47.484982 somatorioInteiros-0.0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 13:10:47.454972 somatorioInteiros-0.0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 13:10:47.483384 somatorioInteiros-0.0.0.2/src/somatorioInteiros.egg-info/
+-rw-rw-rw-   0        0        0      720 2023-08-08 13:10:47.000000 somatorioInteiros-0.0.0.2/src/somatorioInteiros.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-08-08 13:10:47.000000 somatorioInteiros-0.0.0.2/src/somatorioInteiros.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 13:10:47.000000 somatorioInteiros-0.0.0.2/src/somatorioInteiros.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 13:10:47.000000 somatorioInteiros-0.0.0.2/src/somatorioInteiros.egg-info/top_level.txt
```

### Comparing `somatorioInteiros-0.0.0.1/LICENSE` & `somatorioInteiros-0.0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `somatorioInteiros-0.0.0.1/PKG-INFO` & `somatorioInteiros-0.0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: somatorioInteiros
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: Pacote para somar numeros inteiros de uma lista
 Author: Joao Neto
-Author-email: joaonetoprivado2001@gmail.com
+Author-email: joaonetoprivado2001@ufpi.edu.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `somatorioInteiros-0.0.0.1/setup.cfg` & `somatorioInteiros-0.0.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6f6d 6174 6f72 696f 496e 7465   = somatorioInte
 00000020: 6972 6f73 0d0a 7665 7273 696f 6e20 3d20  iros..version = 
-00000030: 302e 302e 302e 310d 0a61 7574 686f 7220  0.0.0.1..author 
+00000030: 302e 302e 302e 320d 0a61 7574 686f 7220  0.0.0.2..author 
 00000040: 3d20 4a6f 616f 204e 6574 6f0d 0a61 7574  = Joao Neto..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6a6f 616f  hor_email = joao
 00000060: 6e65 746f 7072 6976 6164 6f32 3030 3140  netoprivado2001@
-00000070: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
-00000080: 6970 7469 6f6e 203d 2050 6163 6f74 6520  iption = Pacote 
-00000090: 7061 7261 2073 6f6d 6172 206e 756d 6572  para somar numer
-000000a0: 6f73 2069 6e74 6569 726f 7320 6465 2075  os inteiros de u
-000000b0: 6d61 206c 6973 7461 0d0a 6c6f 6e67 5f64  ma lista..long_d
-000000c0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-000000d0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
-000000e0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
-000000f0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
-00000100: 7874 2f6d 6172 6b64 6f77 6e0d 0a63 6c61  xt/markdown..cla
-00000110: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
-00000120: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000130: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000140: 330d 0a09 4c69 6365 6e73 6520 3a3a 204f  3...License :: O
-00000150: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-00000160: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
-00000170: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000180: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
-00000190: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
-000001a0: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
-000001b0: 2073 7263 0d0a 7061 636b 6167 6573 203d   src..packages =
-000001c0: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
-000001d0: 6571 7569 7265 7320 3d20 3e3d 332e 380d  equires = >=3.8.
-000001e0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-000001f0: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
-00000200: 6520 3d20 7372 630d 0a0d 0a5b 6567 675f  e = src....[egg_
-00000210: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000220: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000230: 300d 0a0d 0a                             0....
+00000070: 7566 7069 2e65 6475 2e62 720d 0a64 6573  ufpi.edu.br..des
+00000080: 6372 6970 7469 6f6e 203d 2050 6163 6f74  cription = Pacot
+00000090: 6520 7061 7261 2073 6f6d 6172 206e 756d  e para somar num
+000000a0: 6572 6f73 2069 6e74 6569 726f 7320 6465  eros inteiros de
+000000b0: 2075 6d61 206c 6973 7461 0d0a 6c6f 6e67   uma lista..long
+000000c0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+000000d0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
+000000e0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000f0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+00000100: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a63  text/markdown..c
+00000110: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+00000120: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000130: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000140: 3a20 330d 0a09 4c69 6365 6e73 6520 3a3a  : 3...License ::
+00000150: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+00000160: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
+00000170: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000180: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+00000190: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
+000001a0: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
+000001b0: 093d 2073 7263 0d0a 7061 636b 6167 6573  .= src..packages
+000001c0: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
+000001d0: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
+000001e0: 380d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  8....[options.pa
+000001f0: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
+00000200: 6572 6520 3d20 7372 630d 0a0d 0a5b 6567  ere = src....[eg
+00000210: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000220: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000230: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `somatorioInteiros-0.0.0.1/src/somatorioInteiros.egg-info/PKG-INFO` & `somatorioInteiros-0.0.0.2/src/somatorioInteiros.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: somatorioInteiros
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: Pacote para somar numeros inteiros de uma lista
 Author: Joao Neto
-Author-email: joaonetoprivado2001@gmail.com
+Author-email: joaonetoprivado2001@ufpi.edu.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

