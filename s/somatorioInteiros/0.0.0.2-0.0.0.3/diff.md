# Comparing `tmp/somatorioInteiros-0.0.0.2.tar.gz` & `tmp/somatorioInteiros-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somatorioInteiros-0.0.0.2.tar", last modified: Tue Aug  8 13:10:47 2023, max compression
+gzip compressed data, was "somatorioInteiros-0.0.0.3.tar", last modified: Tue Aug  8 13:19:48 2023, max compression
```

## Comparing `somatorioInteiros-0.0.0.2.tar` & `somatorioInteiros-0.0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 13:10:47.483384 somatorioInteiros-0.0.0.2/
--rw-rw-rw-   0        0        0     1096 2023-08-08 12:21:35.000000 somatorioInteiros-0.0.0.2/LICENSE
--rw-rw-rw-   0        0        0      720 2023-08-08 13:10:47.483384 somatorioInteiros-0.0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-08-08 11:51:28.000000 somatorioInteiros-0.0.0.2/README.md
--rw-rw-rw-   0        0        0      106 2023-08-08 12:06:17.000000 somatorioInteiros-0.0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      567 2023-08-08 13:10:47.484982 somatorioInteiros-0.0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-08 13:10:47.454972 somatorioInteiros-0.0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-08-08 13:10:47.483384 somatorioInteiros-0.0.0.2/src/somatorioInteiros.egg-info/
--rw-rw-rw-   0        0        0      720 2023-08-08 13:10:47.000000 somatorioInteiros-0.0.0.2/src/somatorioInteiros.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-08-08 13:10:47.000000 somatorioInteiros-0.0.0.2/src/somatorioInteiros.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 13:10:47.000000 somatorioInteiros-0.0.0.2/src/somatorioInteiros.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 13:10:47.000000 somatorioInteiros-0.0.0.2/src/somatorioInteiros.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 13:19:48.476331 somatorioInteiros-0.0.0.3/
+-rw-rw-rw-   0        0        0     1096 2023-08-08 12:21:35.000000 somatorioInteiros-0.0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      717 2023-08-08 13:19:48.476331 somatorioInteiros-0.0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-08-08 13:18:15.000000 somatorioInteiros-0.0.0.3/README.md
+-rw-rw-rw-   0        0        0      106 2023-08-08 12:06:17.000000 somatorioInteiros-0.0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      567 2023-08-08 13:19:48.476331 somatorioInteiros-0.0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 13:19:48.455946 somatorioInteiros-0.0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 13:19:48.476331 somatorioInteiros-0.0.0.3/src/somatorioInteiros.egg-info/
+-rw-rw-rw-   0        0        0      717 2023-08-08 13:19:48.000000 somatorioInteiros-0.0.0.3/src/somatorioInteiros.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-08-08 13:19:48.000000 somatorioInteiros-0.0.0.3/src/somatorioInteiros.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 13:19:48.000000 somatorioInteiros-0.0.0.3/src/somatorioInteiros.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 13:19:48.000000 somatorioInteiros-0.0.0.3/src/somatorioInteiros.egg-info/top_level.txt
```

### Comparing `somatorioInteiros-0.0.0.2/LICENSE` & `somatorioInteiros-0.0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `somatorioInteiros-0.0.0.2/PKG-INFO` & `somatorioInteiros-0.0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somatorioInteiros
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: Pacote para somar numeros inteiros de uma lista
 Author: Joao Neto
 Author-email: joaonetoprivado2001@ufpi.edu.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -22,9 +22,9 @@
 
 ## Uso:
 
 ```
 import somatorioInteiros as sumint
 lista = [1,2,3,4]
 obj = sumint(lista)
-soma = sumint.somar()
+soma = obj.somar()
 ```
```

### Comparing `somatorioInteiros-0.0.0.2/setup.cfg` & `somatorioInteiros-0.0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6f6d 6174 6f72 696f 496e 7465   = somatorioInte
 00000020: 6972 6f73 0d0a 7665 7273 696f 6e20 3d20  iros..version = 
-00000030: 302e 302e 302e 320d 0a61 7574 686f 7220  0.0.0.2..author 
+00000030: 302e 302e 302e 330d 0a61 7574 686f 7220  0.0.0.3..author 
 00000040: 3d20 4a6f 616f 204e 6574 6f0d 0a61 7574  = Joao Neto..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6a6f 616f  hor_email = joao
 00000060: 6e65 746f 7072 6976 6164 6f32 3030 3140  netoprivado2001@
 00000070: 7566 7069 2e65 6475 2e62 720d 0a64 6573  ufpi.edu.br..des
 00000080: 6372 6970 7469 6f6e 203d 2050 6163 6f74  cription = Pacot
 00000090: 6520 7061 7261 2073 6f6d 6172 206e 756d  e para somar num
 000000a0: 6572 6f73 2069 6e74 6569 726f 7320 6465  eros inteiros de
```

### Comparing `somatorioInteiros-0.0.0.2/src/somatorioInteiros.egg-info/PKG-INFO` & `somatorioInteiros-0.0.0.3/src/somatorioInteiros.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somatorioInteiros
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: Pacote para somar numeros inteiros de uma lista
 Author: Joao Neto
 Author-email: joaonetoprivado2001@ufpi.edu.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -22,9 +22,9 @@
 
 ## Uso:
 
 ```
 import somatorioInteiros as sumint
 lista = [1,2,3,4]
 obj = sumint(lista)
-soma = sumint.somar()
+soma = obj.somar()
 ```
```

