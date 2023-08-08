# Comparing `tmp/somatorioInteiros-0.0.4.tar.gz` & `tmp/somatorioInteiros-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somatorioInteiros-0.0.4.tar", last modified: Tue Aug  8 14:03:04 2023, max compression
+gzip compressed data, was "somatorioInteiros-0.0.5.tar", last modified: Tue Aug  8 14:23:45 2023, max compression
```

## Comparing `somatorioInteiros-0.0.4.tar` & `somatorioInteiros-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 14:03:04.111215 somatorioInteiros-0.0.4/
--rw-rw-rw-   0        0        0     1094 2023-08-08 14:00:28.000000 somatorioInteiros-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      586 2023-08-08 14:03:04.109248 somatorioInteiros-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-08-08 13:18:15.000000 somatorioInteiros-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-08-08 14:03:04.114148 somatorioInteiros-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      480 2023-08-08 14:02:10.000000 somatorioInteiros-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-08 14:03:04.091343 somatorioInteiros-0.0.4/somatorioInteiros.egg-info/
--rw-rw-rw-   0        0        0      586 2023-08-08 14:03:03.000000 somatorioInteiros-0.0.4/somatorioInteiros.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-08-08 14:03:03.000000 somatorioInteiros-0.0.4/somatorioInteiros.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 14:03:03.000000 somatorioInteiros-0.0.4/somatorioInteiros.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-08-08 14:03:03.000000 somatorioInteiros-0.0.4/somatorioInteiros.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-08 14:03:04.103703 somatorioInteiros-0.0.4/src/
--rw-rw-rw-   0        0        0       40 2023-08-08 13:53:28.000000 somatorioInteiros-0.0.4/src/__init__.py
--rw-rw-rw-   0        0        0      234 2023-08-08 11:50:42.000000 somatorioInteiros-0.0.4/src/somatorio.py
+drwxrwxrwx   0        0        0        0 2023-08-08 14:23:45.944851 somatorioInteiros-0.0.5/
+-rw-rw-rw-   0        0        0     1094 2023-08-08 14:00:28.000000 somatorioInteiros-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      586 2023-08-08 14:23:45.943845 somatorioInteiros-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-08-08 13:18:15.000000 somatorioInteiros-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-08 14:23:45.944851 somatorioInteiros-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      454 2023-08-08 14:23:18.000000 somatorioInteiros-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 14:23:45.934909 somatorioInteiros-0.0.5/somatorioInteiros.egg-info/
+-rw-rw-rw-   0        0        0      586 2023-08-08 14:23:45.000000 somatorioInteiros-0.0.5/somatorioInteiros.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-08-08 14:23:45.000000 somatorioInteiros-0.0.5/somatorioInteiros.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 14:23:45.000000 somatorioInteiros-0.0.5/somatorioInteiros.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-08-08 14:23:45.000000 somatorioInteiros-0.0.5/somatorioInteiros.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 14:23:45.942361 somatorioInteiros-0.0.5/src/
+-rw-rw-rw-   0        0        0       40 2023-08-08 14:22:56.000000 somatorioInteiros-0.0.5/src/__init__.py
+-rw-rw-rw-   0        0        0      234 2023-08-08 11:50:42.000000 somatorioInteiros-0.0.5/src/somatorio.py
```

### Comparing `somatorioInteiros-0.0.4/LICENSE` & `somatorioInteiros-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `somatorioInteiros-0.0.4/PKG-INFO` & `somatorioInteiros-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somatorioInteiros
-Version: 0.0.4
+Version: 0.0.5
 Summary: Somador de numeros inteiros em uma lista
 Author: Joao Neto
 Author-email: joaonetoprivado2001@ufpi.edu.br
 License: MIT License
 Keywords: soma inteiros
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `somatorioInteiros-0.0.4/somatorioInteiros.egg-info/PKG-INFO` & `somatorioInteiros-0.0.5/somatorioInteiros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somatorioInteiros
-Version: 0.0.4
+Version: 0.0.5
 Summary: Somador de numeros inteiros em uma lista
 Author: Joao Neto
 Author-email: joaonetoprivado2001@ufpi.edu.br
 License: MIT License
 Keywords: soma inteiros
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

