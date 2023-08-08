# Comparing `tmp/perms-1.0.tar.gz` & `tmp/perms-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perms-1.0.tar", last modified: Mon Aug  7 11:37:09 2023, max compression
+gzip compressed data, was "perms-1.1.tar", last modified: Tue Aug  8 13:53:20 2023, max compression
```

## Comparing `perms-1.0.tar` & `perms-1.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 peraugust   (501) staff       (20)        0 2023-08-07 11:37:09.970456 perms-1.0/
--rw-r--r--   0 peraugust   (501) staff       (20)       11 2023-07-14 12:31:38.000000 perms-1.0/MANIFEST.in
--rw-r--r--   0 peraugust   (501) staff       (20)      964 2023-08-07 11:37:09.970528 perms-1.0/PKG-INFO
--rw-r--r--   0 peraugust   (501) staff       (20)      325 2023-08-07 11:23:51.000000 perms-1.0/README.md
--rw-r--r--   0 peraugust   (501) staff       (20)     3468 2023-07-16 15:52:26.000000 perms-1.0/get_alphabetagamma.c
--rw-r--r--   0 peraugust   (501) staff       (20)    10362 2023-08-07 11:19:02.000000 perms-1.0/get_log_permanent.c
--rw-r--r--   0 peraugust   (501) staff       (20)     4270 2023-07-16 23:31:49.000000 perms-1.0/header.h
--rw-r--r--   0 peraugust   (501) staff       (20)     6770 2023-08-07 09:32:47.000000 perms-1.0/help_functions.c
--rw-r--r--   0 peraugust   (501) staff       (20)    19601 2023-08-07 09:33:50.000000 perms-1.0/methods.c
--rw-r--r--   0 peraugust   (501) staff       (20)    12828 2023-08-07 09:32:14.000000 perms-1.0/methods_sparse.c
-drwxr-xr-x   0 peraugust   (501) staff       (20)        0 2023-08-07 11:37:09.970354 perms-1.0/perms.egg-info/
--rw-r--r--   0 peraugust   (501) staff       (20)      964 2023-08-07 11:37:09.000000 perms-1.0/perms.egg-info/PKG-INFO
--rw-r--r--   0 peraugust   (501) staff       (20)      320 2023-08-07 11:37:09.000000 perms-1.0/perms.egg-info/SOURCES.txt
--rw-r--r--   0 peraugust   (501) staff       (20)        1 2023-08-07 11:37:09.000000 perms-1.0/perms.egg-info/dependency_links.txt
--rw-r--r--   0 peraugust   (501) staff       (20)        6 2023-08-07 11:37:09.000000 perms-1.0/perms.egg-info/requires.txt
--rw-r--r--   0 peraugust   (501) staff       (20)       12 2023-08-07 11:37:09.000000 perms-1.0/perms.egg-info/top_level.txt
--rw-r--r--   0 peraugust   (501) staff       (20)      568 2023-08-07 11:24:33.000000 perms-1.0/pyproject.toml
--rw-r--r--   0 peraugust   (501) staff       (20)       79 2023-08-07 11:37:09.970745 perms-1.0/setup.cfg
--rw-r--r--   0 peraugust   (501) staff       (20)     1087 2023-08-07 11:24:59.000000 perms-1.0/setup.py
--rw-r--r--   0 peraugust   (501) staff       (20)     1251 2023-08-07 09:57:03.000000 perms-1.0/test2.py
--rw-r--r--   0 peraugust   (501) staff       (20)     1855 2023-07-13 23:55:41.000000 perms-1.0/xxhash.c
--rw-r--r--   0 peraugust   (501) staff       (20)   241969 2023-07-13 23:55:41.000000 perms-1.0/xxhash.h
+drwxr-xr-x   0 peraugust   (501) staff       (20)        0 2023-08-08 13:53:20.482850 perms-1.1/
+-rw-r--r--   0 peraugust   (501) staff       (20)       11 2023-07-14 12:31:38.000000 perms-1.1/MANIFEST.in
+-rw-r--r--   0 peraugust   (501) staff       (20)     1001 2023-08-08 13:53:20.482927 perms-1.1/PKG-INFO
+-rw-r--r--   0 peraugust   (501) staff       (20)      360 2023-08-07 12:20:47.000000 perms-1.1/README.md
+-rw-r--r--   0 peraugust   (501) staff       (20)     3468 2023-07-16 15:52:26.000000 perms-1.1/get_alphabetagamma.c
+-rw-r--r--   0 peraugust   (501) staff       (20)    35063 2023-08-08 13:49:21.000000 perms-1.1/get_log_permanent.c
+-rw-r--r--   0 peraugust   (501) staff       (20)     4325 2023-08-08 11:28:20.000000 perms-1.1/header.h
+-rw-r--r--   0 peraugust   (501) staff       (20)     6770 2023-08-07 09:32:47.000000 perms-1.1/help_functions.c
+-rw-r--r--   0 peraugust   (501) staff       (20)    19601 2023-08-07 09:33:50.000000 perms-1.1/methods.c
+-rw-r--r--   0 peraugust   (501) staff       (20)    12828 2023-08-07 09:32:14.000000 perms-1.1/methods_sparse.c
+drwxr-xr-x   0 peraugust   (501) staff       (20)        0 2023-08-08 13:53:20.482748 perms-1.1/perms.egg-info/
+-rw-r--r--   0 peraugust   (501) staff       (20)     1001 2023-08-08 13:53:20.000000 perms-1.1/perms.egg-info/PKG-INFO
+-rw-r--r--   0 peraugust   (501) staff       (20)      311 2023-08-08 13:53:20.000000 perms-1.1/perms.egg-info/SOURCES.txt
+-rw-r--r--   0 peraugust   (501) staff       (20)        1 2023-08-08 13:53:20.000000 perms-1.1/perms.egg-info/dependency_links.txt
+-rw-r--r--   0 peraugust   (501) staff       (20)        6 2023-08-08 13:53:20.000000 perms-1.1/perms.egg-info/requires.txt
+-rw-r--r--   0 peraugust   (501) staff       (20)        6 2023-08-08 13:53:20.000000 perms-1.1/perms.egg-info/top_level.txt
+-rw-r--r--   0 peraugust   (501) staff       (20)      568 2023-08-08 13:50:27.000000 perms-1.1/pyproject.toml
+-rw-r--r--   0 peraugust   (501) staff       (20)       79 2023-08-08 13:53:20.483142 perms-1.1/setup.cfg
+-rw-r--r--   0 peraugust   (501) staff       (20)     1139 2023-08-08 13:51:33.000000 perms-1.1/setup.py
+-rw-r--r--   0 peraugust   (501) staff       (20)     1855 2023-07-13 23:55:41.000000 perms-1.1/xxhash.c
+-rw-r--r--   0 peraugust   (501) staff       (20)   241969 2023-07-13 23:55:41.000000 perms-1.1/xxhash.h
```

### Comparing `perms-1.0/PKG-INFO` & `perms-1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: perms
-Version: 1.0
+Version: 1.1
 Summary: perms
 Home-page: https://github.com/peraugustmoen/perms
-Download-URL: https://github.com/peraugustmoen/fastperm/archive/refs/tags/v_1.tar.gz
+Download-URL: https://github.com/peraugustmoen/fastperm/archive/refs/tags/v_1_1.tar.gz
 Author: Dennis Christensen, Per August Jarval Moen
 Author-email: Dennis Christensen <dennis.christensen@ffi.no>, Per August Jarval Moen <pamoen@math.uio.no>
 License: MIT
 Project-URL: Homepage, https://github.com/peraugustmoen/perms
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,14 @@
 Description-Content-Type: text/markdown
 
 
 # perms
 
 
 
-The *perms* package implements the algorithm proposed by [[1]](#1) for computing the permanent of a block rectangular matrix. 
+The perms package implements the algorithm proposed by [[1]](#1) for computing permanents of block rectangular matrices. 
 
 ## References
 <a id="1">[1]</a> 
-Christensen, D (2022). 
-Inference for Bayesian Nonparametric Models with Binary Response Data via Permutation Counting. 
-Bayesian Analysis, 1(1), 1-26.
+Christensen, D (2023). 
+Inference for Bayesian nonparametric models with binary response data via permutation counting. 
+Bayesian Analysis, Advance online publication, DOI: 10.1214/22-BA1353.
```

### Comparing `perms-1.0/get_alphabetagamma.c` & `perms-1.1/get_alphabetagamma.c`

 * *Files identical despite different names*

### Comparing `perms-1.0/header.h` & `perms-1.1/header.h`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 double Clog_sum_exp(double *, int, double);
 void print_matrix(int, int , double * );
 void print_int_vector(int ,  int * );
 void print_float_vector(int ,  double * );
 
 static PyObject *C_get_log_permanents(PyObject *, PyObject *);
 static PyObject *log_sum_exp(PyObject *, PyObject *);
+static PyObject *C_get_log_ML(PyObject *, PyObject *);
 
 double Clog_sum_exp(double * , int, double );
 double Csparse_log_sum_exp(dictionary *);
 
 
 int nonzero_perm(double * , double * , double * , int );
```

### Comparing `perms-1.0/help_functions.c` & `perms-1.1/help_functions.c`

 * *Files identical despite different names*

### Comparing `perms-1.0/methods.c` & `perms-1.1/methods.c`

 * *Files identical despite different names*

### Comparing `perms-1.0/methods_sparse.c` & `perms-1.1/methods_sparse.c`

 * *Files identical despite different names*

### Comparing `perms-1.0/perms.egg-info/PKG-INFO` & `perms-1.1/perms.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: perms
-Version: 1.0
+Version: 1.1
 Summary: perms
 Home-page: https://github.com/peraugustmoen/perms
-Download-URL: https://github.com/peraugustmoen/fastperm/archive/refs/tags/v_1.tar.gz
+Download-URL: https://github.com/peraugustmoen/fastperm/archive/refs/tags/v_1_1.tar.gz
 Author: Dennis Christensen, Per August Jarval Moen
 Author-email: Dennis Christensen <dennis.christensen@ffi.no>, Per August Jarval Moen <pamoen@math.uio.no>
 License: MIT
 Project-URL: Homepage, https://github.com/peraugustmoen/perms
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,14 @@
 Description-Content-Type: text/markdown
 
 
 # perms
 
 
 
-The *perms* package implements the algorithm proposed by [[1]](#1) for computing the permanent of a block rectangular matrix. 
+The perms package implements the algorithm proposed by [[1]](#1) for computing permanents of block rectangular matrices. 
 
 ## References
 <a id="1">[1]</a> 
-Christensen, D (2022). 
-Inference for Bayesian Nonparametric Models with Binary Response Data via Permutation Counting. 
-Bayesian Analysis, 1(1), 1-26.
+Christensen, D (2023). 
+Inference for Bayesian nonparametric models with binary response data via permutation counting. 
+Bayesian Analysis, Advance online publication, DOI: 10.1214/22-BA1353.
```

### Comparing `perms-1.0/pyproject.toml` & `perms-1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=58","numpy"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "perms"
-version = "1.0"
+version = "1.1"
 authors = [
   { name="Dennis Christensen", email="dennis.christensen@ffi.no" },
   { name="Per August Jarval Moen", email="pamoen@math.uio.no" }
 ]
 description = "perms"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `perms-1.0/setup.py` & `perms-1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, Extension
 import numpy as np
 
 def main():
     setup(
         license='MIT',
+        extra_compile_args = ["-DNDEBUG", "-O3"],
         description = 'The perms package implements the algorithm proposed by Christensen (Inference for Bayesian Nonparametric Models with Binary Response Data via Permutation Counting, Bayesian Analysis, 1(1), 1-26,2023) for computing the permanent of a block rectangular matrix.',
         author = 'Dennis Christensen, Per August Jarval Moen',                  
         author_email = 'Dennis.Christensen@ffi.no, pamoen@math.uio.no',      
         url = 'https://github.com/peraugustmoen/perms',  
-        download_url = 'https://github.com/peraugustmoen/fastperm/archive/refs/tags/v_1.tar.gz',
+        download_url = 'https://github.com/peraugustmoen/fastperm/archive/refs/tags/v_1_1.tar.gz',
         name="fastperm",
-        version="1.0",
+        version="1.1",
         install_requires=["numpy"],
         include_dirs=[np.get_include()],
         ext_modules=[Extension("perms", ["get_log_permanent.c", "help_functions.c", "get_alphabetagamma.c",\
                 "methods_sparse.c", "methods.c", "xxhash.c"])],
         headers = ["xxhash.h", "header.h"])
```

### Comparing `perms-1.0/xxhash.c` & `perms-1.1/xxhash.c`

 * *Files identical despite different names*

### Comparing `perms-1.0/xxhash.h` & `perms-1.1/xxhash.h`

 * *Files identical despite different names*

