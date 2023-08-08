# Comparing `tmp/remfile-0.1.0.tar.gz` & `tmp/remfile-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remfile-0.1.0.tar", last modified: Mon Aug  7 13:09:08 2023, max compression
+gzip compressed data, was "remfile-0.1.1.tar", last modified: Mon Aug  7 19:45:55 2023, max compression
```

## Comparing `remfile-0.1.0.tar` & `remfile-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 codespace  (1000) codespace  (1000)        0 2023-08-07 13:09:08.399952 remfile-0.1.0/
--rw-rw-r--   0 codespace  (1000) codespace  (1000)    11357 2023-08-07 12:41:38.000000 remfile-0.1.0/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)    15106 2023-08-07 13:09:08.399952 remfile-0.1.0/PKG-INFO
--rw-r--r--   0 codespace  (1000) codespace  (1000)     1613 2023-08-07 13:07:09.000000 remfile-0.1.0/README.md
--rw-r--r--   0 codespace  (1000) codespace  (1000)      893 2023-08-07 13:04:05.000000 remfile-0.1.0/pyproject.toml
-drwxr-xr-x   0 codespace  (1000) codespace  (1000)        0 2023-08-07 13:09:08.395952 remfile-0.1.0/remfile/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     3790 2023-08-07 13:04:53.000000 remfile-0.1.0/remfile/RemFile.py
--rw-r--r--   0 codespace  (1000) codespace  (1000)       59 2023-08-07 13:04:48.000000 remfile-0.1.0/remfile/__init__.py
-drwxr-xr-x   0 codespace  (1000) codespace  (1000)        0 2023-08-07 13:09:08.399952 remfile-0.1.0/remfile.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)    15106 2023-08-07 13:09:08.000000 remfile-0.1.0/remfile.egg-info/PKG-INFO
--rw-r--r--   0 codespace  (1000) codespace  (1000)      225 2023-08-07 13:09:08.000000 remfile-0.1.0/remfile.egg-info/SOURCES.txt
--rw-r--r--   0 codespace  (1000) codespace  (1000)        1 2023-08-07 13:09:08.000000 remfile-0.1.0/remfile.egg-info/dependency_links.txt
--rw-r--r--   0 codespace  (1000) codespace  (1000)       14 2023-08-07 13:09:08.000000 remfile-0.1.0/remfile.egg-info/requires.txt
--rw-r--r--   0 codespace  (1000) codespace  (1000)        8 2023-08-07 13:09:08.000000 remfile-0.1.0/remfile.egg-info/top_level.txt
--rw-r--r--   0 codespace  (1000) codespace  (1000)       38 2023-08-07 13:09:08.399952 remfile-0.1.0/setup.cfg
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-07 19:45:55.922896 remfile-0.1.1/
+-rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-08-07 12:41:38.000000 remfile-0.1.1/LICENSE
+-rw-rw-r--   0 magland   (1000) magland   (1000)    15245 2023-08-07 19:45:55.922896 remfile-0.1.1/PKG-INFO
+-rw-r--r--   0 magland   (1000) magland   (1000)     1731 2023-08-07 19:45:00.000000 remfile-0.1.1/README.md
+-rw-r--r--   0 magland   (1000) magland   (1000)      959 2023-08-07 19:14:40.000000 remfile-0.1.1/pyproject.toml
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-07 19:45:55.922896 remfile-0.1.1/remfile/
+-rw-r--r--   0 magland   (1000) magland   (1000)     5454 2023-08-07 19:42:37.000000 remfile-0.1.1/remfile/RemFile.py
+-rw-r--r--   0 magland   (1000) magland   (1000)       59 2023-08-07 19:43:40.000000 remfile-0.1.1/remfile/__init__.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-07 19:45:55.922896 remfile-0.1.1/remfile.egg-info/
+-rw-r--r--   0 magland   (1000) magland   (1000)    15245 2023-08-07 19:45:55.000000 remfile-0.1.1/remfile.egg-info/PKG-INFO
+-rw-r--r--   0 magland   (1000) magland   (1000)      244 2023-08-07 19:45:55.000000 remfile-0.1.1/remfile.egg-info/SOURCES.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)        1 2023-08-07 19:45:55.000000 remfile-0.1.1/remfile.egg-info/dependency_links.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)       29 2023-08-07 19:45:55.000000 remfile-0.1.1/remfile.egg-info/requires.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)        8 2023-08-07 19:45:55.000000 remfile-0.1.1/remfile.egg-info/top_level.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       38 2023-08-07 19:45:55.922896 remfile-0.1.1/setup.cfg
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-07 19:45:55.922896 remfile-0.1.1/tests/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      363 2023-08-07 19:14:23.000000 remfile-0.1.1/tests/test_main.py
```

### Comparing `remfile-0.1.0/LICENSE` & `remfile-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `remfile-0.1.0/PKG-INFO` & `remfile-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remfile
-Version: 0.1.0
+Version: 0.1.1
 Summary: File-like object from url of remote file, optimized for use with h5py.
 Author-email: Jeremy Magland <jmagland@flatironinstitute.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -208,14 +208,15 @@
 Project-URL: repository, https://github.com/magland/remfile
 Keywords: hdf5,file-like
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # remfile
 
 Provides a file-like object for reading a remote file over HTTP, optimized for use with h5py.
 
 Example usage:
@@ -224,15 +225,15 @@
 # See examples/example1.py
 
 import h5py
 import remfile
 
 url = 'https://dandiarchive.s3.amazonaws.com/blobs/d86/055/d8605573-4639-4b99-a6d9-e0ac13f9a7df'
 
-file = remfil.File(url)
+file = remfile.File(url)
 
 with h5py.File(file, 'r') as f:
     print(f['/'].keys())
 ```
 
 See [examples/example1.py](examples/example1.py) for a more complete example.
 
@@ -240,21 +241,21 @@
 
 ```bash
 pip install remfile
 ```
 
 ## Why?
 
-The conventional way of reading a remote hdf5 file is to use the fsspec library as in [examples/example1_compare_fsspec.py](examples/example1_compare_fsspec.py). However, this approach is empirically much slower than using remfile. I am not familiar with the inner workings of fsspec, but it does not seem to be optimized for reading hdf5 files. Efficient access of remote hdf5 files requires reading small chunks of data to obtain meta information, and then large chunks of data to obtain the larger data arrays.
+The conventional way of reading a remote hdf5 file is to use the fsspec library as in [examples/example1_compare_fsspec.py](examples/example1_compare_fsspec.py). However, this approach is empirically much slower than using remfile. I am not familiar with the inner workings of fsspec, but it does not seem to be optimized for reading hdf5 files. Efficient access of remote hdf5 files requires reading small chunks of data to obtain meta information, and then large chunks of data, and parallelization, to obtain the larger data arrays.
 
 See a timing comparison betweeen remfile and fsspec in the examples directory.
 
 ## How?
 
-A file-like object is created that reads the remote file in chunks using the requests library. A relatively small default chunk size is used, but when the system detects that a large data array is being accessed, it switches to a larger chunk size.
+A file-like object is created that reads the remote file in chunks using the requests library. A relatively small default chunk size is used, but when the system detects that a large data array is being accessed, it switches to a larger chunk size. For very large data arrays, the system will use multiple threads to read the data in parallel.
 
 ## Caveats
 
 This library is not intended to be a general purpose library for reading remote files. It is optimized for reading hdf5 files.
 
 ## License
```

### Comparing `remfile-0.1.0/README.md` & `remfile-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # See examples/example1.py
 
 import h5py
 import remfile
 
 url = 'https://dandiarchive.s3.amazonaws.com/blobs/d86/055/d8605573-4639-4b99-a6d9-e0ac13f9a7df'
 
-file = remfil.File(url)
+file = remfile.File(url)
 
 with h5py.File(file, 'r') as f:
     print(f['/'].keys())
 ```
 
 See [examples/example1.py](examples/example1.py) for a more complete example.
 
@@ -24,21 +24,21 @@
 
 ```bash
 pip install remfile
 ```
 
 ## Why?
 
-The conventional way of reading a remote hdf5 file is to use the fsspec library as in [examples/example1_compare_fsspec.py](examples/example1_compare_fsspec.py). However, this approach is empirically much slower than using remfile. I am not familiar with the inner workings of fsspec, but it does not seem to be optimized for reading hdf5 files. Efficient access of remote hdf5 files requires reading small chunks of data to obtain meta information, and then large chunks of data to obtain the larger data arrays.
+The conventional way of reading a remote hdf5 file is to use the fsspec library as in [examples/example1_compare_fsspec.py](examples/example1_compare_fsspec.py). However, this approach is empirically much slower than using remfile. I am not familiar with the inner workings of fsspec, but it does not seem to be optimized for reading hdf5 files. Efficient access of remote hdf5 files requires reading small chunks of data to obtain meta information, and then large chunks of data, and parallelization, to obtain the larger data arrays.
 
 See a timing comparison betweeen remfile and fsspec in the examples directory.
 
 ## How?
 
-A file-like object is created that reads the remote file in chunks using the requests library. A relatively small default chunk size is used, but when the system detects that a large data array is being accessed, it switches to a larger chunk size.
+A file-like object is created that reads the remote file in chunks using the requests library. A relatively small default chunk size is used, but when the system detects that a large data array is being accessed, it switches to a larger chunk size. For very large data arrays, the system will use multiple threads to read the data in parallel.
 
 ## Caveats
 
 This library is not intended to be a general purpose library for reading remote files. It is optimized for reading hdf5 files.
 
 ## License
```

### Comparing `remfile-0.1.0/pyproject.toml` & `remfile-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -16,17 +16,22 @@
 requires-python = ">=3.6"
 dynamic = ["version", "readme"]
 dependencies = [
     "requests",
     "h5py"
 ]
 
+[project.optional-dependencies]
+test = [
+    "pytest"
+]
+
 [project.urls]
 repository = "https://github.com/magland/remfile"
 
 [tool.setuptools.packages.find]
 include = ["remfile*"]
-exclude = ["devel"]
+exclude = ["devel", "tests"]
 
 [tool.setuptools.dynamic]
 readme = {file = ["README.md"], content-type = "text/markdown"}
 version = {attr = "remfile.__version__"}
```

### Comparing `remfile-0.1.0/remfile.egg-info/PKG-INFO` & `remfile-0.1.1/remfile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remfile
-Version: 0.1.0
+Version: 0.1.1
 Summary: File-like object from url of remote file, optimized for use with h5py.
 Author-email: Jeremy Magland <jmagland@flatironinstitute.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -208,14 +208,15 @@
 Project-URL: repository, https://github.com/magland/remfile
 Keywords: hdf5,file-like
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # remfile
 
 Provides a file-like object for reading a remote file over HTTP, optimized for use with h5py.
 
 Example usage:
@@ -224,15 +225,15 @@
 # See examples/example1.py
 
 import h5py
 import remfile
 
 url = 'https://dandiarchive.s3.amazonaws.com/blobs/d86/055/d8605573-4639-4b99-a6d9-e0ac13f9a7df'
 
-file = remfil.File(url)
+file = remfile.File(url)
 
 with h5py.File(file, 'r') as f:
     print(f['/'].keys())
 ```
 
 See [examples/example1.py](examples/example1.py) for a more complete example.
 
@@ -240,21 +241,21 @@
 
 ```bash
 pip install remfile
 ```
 
 ## Why?
 
-The conventional way of reading a remote hdf5 file is to use the fsspec library as in [examples/example1_compare_fsspec.py](examples/example1_compare_fsspec.py). However, this approach is empirically much slower than using remfile. I am not familiar with the inner workings of fsspec, but it does not seem to be optimized for reading hdf5 files. Efficient access of remote hdf5 files requires reading small chunks of data to obtain meta information, and then large chunks of data to obtain the larger data arrays.
+The conventional way of reading a remote hdf5 file is to use the fsspec library as in [examples/example1_compare_fsspec.py](examples/example1_compare_fsspec.py). However, this approach is empirically much slower than using remfile. I am not familiar with the inner workings of fsspec, but it does not seem to be optimized for reading hdf5 files. Efficient access of remote hdf5 files requires reading small chunks of data to obtain meta information, and then large chunks of data, and parallelization, to obtain the larger data arrays.
 
 See a timing comparison betweeen remfile and fsspec in the examples directory.
 
 ## How?
 
-A file-like object is created that reads the remote file in chunks using the requests library. A relatively small default chunk size is used, but when the system detects that a large data array is being accessed, it switches to a larger chunk size.
+A file-like object is created that reads the remote file in chunks using the requests library. A relatively small default chunk size is used, but when the system detects that a large data array is being accessed, it switches to a larger chunk size. For very large data arrays, the system will use multiple threads to read the data in parallel.
 
 ## Caveats
 
 This library is not intended to be a general purpose library for reading remote files. It is optimized for reading hdf5 files.
 
 ## License
```

