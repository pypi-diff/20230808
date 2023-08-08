# Comparing `tmp/remfile-0.1.4.tar.gz` & `tmp/remfile-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remfile-0.1.4.tar", last modified: Tue Aug  8 16:38:55 2023, max compression
+gzip compressed data, was "remfile-0.1.5.tar", last modified: Tue Aug  8 17:23:30 2023, max compression
```

## Comparing `remfile-0.1.4.tar` & `remfile-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 16:38:55.663624 remfile-0.1.4/
--rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-08-07 12:41:38.000000 remfile-0.1.4/LICENSE
--rw-rw-r--   0 magland   (1000) magland   (1000)     2340 2023-08-08 16:38:55.663624 remfile-0.1.4/PKG-INFO
--rw-r--r--   0 magland   (1000) magland   (1000)     2032 2023-08-08 15:51:03.000000 remfile-0.1.4/README.md
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 16:38:55.663624 remfile-0.1.4/remfile/
--rw-r--r--   0 magland   (1000) magland   (1000)    10197 2023-08-08 15:46:29.000000 remfile-0.1.4/remfile/RemFile.py
--rw-r--r--   0 magland   (1000) magland   (1000)      115 2023-08-08 16:35:22.000000 remfile-0.1.4/remfile/__init__.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 16:38:55.663624 remfile-0.1.4/remfile.egg-info/
--rw-r--r--   0 magland   (1000) magland   (1000)     2340 2023-08-08 16:38:55.000000 remfile-0.1.4/remfile.egg-info/PKG-INFO
--rw-r--r--   0 magland   (1000) magland   (1000)      238 2023-08-08 16:38:55.000000 remfile-0.1.4/remfile.egg-info/SOURCES.txt
--rw-r--r--   0 magland   (1000) magland   (1000)        1 2023-08-08 16:38:55.000000 remfile-0.1.4/remfile.egg-info/dependency_links.txt
--rw-r--r--   0 magland   (1000) magland   (1000)       20 2023-08-08 16:38:55.000000 remfile-0.1.4/remfile.egg-info/requires.txt
--rw-r--r--   0 magland   (1000) magland   (1000)        8 2023-08-08 16:38:55.000000 remfile-0.1.4/remfile.egg-info/top_level.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       38 2023-08-08 16:38:55.663624 remfile-0.1.4/setup.cfg
--rw-rw-r--   0 magland   (1000) magland   (1000)      764 2023-08-08 16:35:39.000000 remfile-0.1.4/setup.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 16:38:55.663624 remfile-0.1.4/tests/
--rw-rw-r--   0 magland   (1000) magland   (1000)     1673 2023-08-08 15:43:09.000000 remfile-0.1.4/tests/test_main.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 17:23:30.670187 remfile-0.1.5/
+-rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-08-07 12:41:38.000000 remfile-0.1.5/LICENSE
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2492 2023-08-08 17:23:30.670187 remfile-0.1.5/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2184 2023-08-08 17:19:43.000000 remfile-0.1.5/README.md
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 17:23:30.670187 remfile-0.1.5/remfile/
+-rw-r--r--   0 magland   (1000) magland   (1000)    11553 2023-08-08 17:17:55.000000 remfile-0.1.5/remfile/RemFile.py
+-rw-r--r--   0 magland   (1000) magland   (1000)      115 2023-08-08 16:35:22.000000 remfile-0.1.5/remfile/__init__.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 17:23:30.670187 remfile-0.1.5/remfile.egg-info/
+-rw-r--r--   0 magland   (1000) magland   (1000)     2492 2023-08-08 17:23:30.000000 remfile-0.1.5/remfile.egg-info/PKG-INFO
+-rw-r--r--   0 magland   (1000) magland   (1000)      238 2023-08-08 17:23:30.000000 remfile-0.1.5/remfile.egg-info/SOURCES.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)        1 2023-08-08 17:23:30.000000 remfile-0.1.5/remfile.egg-info/dependency_links.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)       20 2023-08-08 17:23:30.000000 remfile-0.1.5/remfile.egg-info/requires.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)        8 2023-08-08 17:23:30.000000 remfile-0.1.5/remfile.egg-info/top_level.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       38 2023-08-08 17:23:30.670187 remfile-0.1.5/setup.cfg
+-rw-rw-r--   0 magland   (1000) magland   (1000)      764 2023-08-08 17:19:09.000000 remfile-0.1.5/setup.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-08 17:23:30.670187 remfile-0.1.5/tests/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1810 2023-08-08 17:18:04.000000 remfile-0.1.5/tests/test_main.py
```

### Comparing `remfile-0.1.4/LICENSE` & `remfile-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `remfile-0.1.4/PKG-INFO` & `remfile-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: remfile
-Version: 0.1.4
+Version: 0.1.5
 Summary: File-like object from url of remote file, optimized for use with h5py.
 Home-page: https://github.com/magland/remfile
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # remfile
 
 [![latest-release](https://img.shields.io/pypi/v/remfile.svg)](https://pypi.org/project/remfile)
 ![tests](https://github.com/magland/remfile/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/magland/remfile/branch/main/graph/badge.svg)](https://codecov.io/gh/magland/remfile)
 
-
 Provides a file-like object for reading a remote file over HTTP, optimized for use with h5py.
 
 Example usage:
 
 ```python
 # See examples/example1.py
 
@@ -51,14 +50,18 @@
 
 A file-like object is created that reads the remote file in chunks using the requests library. A relatively small default chunk size is used, but when the system detects that a large data array is being accessed, it switches to a larger chunk size. For very large data arrays, the system will use multiple threads to read the data in parallel.
 
 ## Caveats
 
 This library is not intended to be a general purpose library for reading remote files. It is optimized for reading hdf5 files.
 
+At this time, remfile provides only an in-memory cache, not an on-disk cache.
+
+At this time, remfile does not do automatic retries for failed requests.
+
 ## License
 
 Apache 2.0
 
 ## Author
 
 Jeremy Magland, Center for Computational Mathematics, Flatiron Institute
```

### Comparing `remfile-0.1.4/README.md` & `remfile-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # remfile
 
 [![latest-release](https://img.shields.io/pypi/v/remfile.svg)](https://pypi.org/project/remfile)
 ![tests](https://github.com/magland/remfile/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/magland/remfile/branch/main/graph/badge.svg)](https://codecov.io/gh/magland/remfile)
 
-
 Provides a file-like object for reading a remote file over HTTP, optimized for use with h5py.
 
 Example usage:
 
 ```python
 # See examples/example1.py
 
@@ -41,14 +40,18 @@
 
 A file-like object is created that reads the remote file in chunks using the requests library. A relatively small default chunk size is used, but when the system detects that a large data array is being accessed, it switches to a larger chunk size. For very large data arrays, the system will use multiple threads to read the data in parallel.
 
 ## Caveats
 
 This library is not intended to be a general purpose library for reading remote files. It is optimized for reading hdf5 files.
 
+At this time, remfile provides only an in-memory cache, not an on-disk cache.
+
+At this time, remfile does not do automatic retries for failed requests.
+
 ## License
 
 Apache 2.0
 
 ## Author
 
 Jeremy Magland, Center for Computational Mathematics, Flatiron Institute
```

### Comparing `remfile-0.1.4/remfile/RemFile.py` & `remfile-0.1.5/remfile/RemFile.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 from concurrent.futures import ThreadPoolExecutor
 import requests
 
 default_min_chunk_size = 100 * 1024
 default_max_cache_size = 1e8
 default_chunk_increment_factor = 1.7
 default_bytes_per_thread = 4 * 1024 * 1024
@@ -12,34 +13,37 @@
         url: str, *,
         verbose: bool=False,
         _min_chunk_size: int=default_min_chunk_size,
         _max_cache_size: int=default_max_cache_size,
         _chunk_increment_factor: int=default_chunk_increment_factor,
         _bytes_per_thread: int=default_bytes_per_thread,
         _max_threads: int=default_max_threads,
-        _max_chunk_size: int=100 * 1024 * 1024
+        _max_chunk_size: int=100 * 1024 * 1024,
+        _impose_request_failures_for_testing: bool=False
     ):
         """Create a file-like object for reading a remote file. Optimized for reading hdf5 files. The arguments starting with an underscore are for testing and debugging purposes - they may experience breaking changes in the future.
 
         Args:
             url (str): The url of the remote file.
             verbose (bool, optional): Whether to print info for debugging. Defaults to False.
             _min_chunk_size (int, optional): The minimum chunk size. When reading, the chunks will be loaded in multiples of this size.
             _max_cache_size (int, optional): The maximum number of bytes to keep in the cache.
             _chunk_increment_factor (int, optional): The factor by which to increase the number of chunks to load when the system detects that the chunks are being loaded in order.
             _bytes_per_thread (int, optional): The minimum number of bytes to load in each thread.
             _max_threads (int, optional): The maximum number of threads to use when loading the file.
             _max_chunk_size (int, optional): The maximum chunk size. When reading, the chunks will be loaded in multiples of the minimum chunk size up to this size.
+            _impose_request_failures_for_testing (bool, optional): Whether to impose request failures for testing purposes. Defaults to False.
         """
         self._min_chunk_size = _min_chunk_size
         self._max_chunks_in_cache = int(_max_cache_size / _min_chunk_size)
         self._chunk_increment_factor = _chunk_increment_factor
         self._bytes_per_thread = _bytes_per_thread
         self._max_threads = _max_threads
         self._max_chunk_size = _max_chunk_size
+        self._impose_request_failures_for_testing = _impose_request_failures_for_testing
         self._verbose = verbose
         self._chunks = {}
         self._chunk_indices: list[int] = [] # list of chunk indices in order of loading for purposes of cleaning up the cache
         self._url = url
         self._position = 0
         self._smart_loader_last_chunk_index_accessed = -99
         self._smart_loader_chunk_sequence_length = 1
@@ -123,15 +127,23 @@
             self._smart_loader_chunk_sequence_length = 1
         data_start = chunk_index * self._min_chunk_size
         data_end = data_start + self._min_chunk_size * self._smart_loader_chunk_sequence_length - 1
         if self._verbose:
             print(f"Loading {self._smart_loader_chunk_sequence_length} chunks starting at {chunk_index} ({(data_end - data_start + 1)/1e6} million bytes)")
         if data_end >= self.length:
             data_end = self.length - 1
-        x = _get_bytes(self._url, data_start, data_end, verbose=self._verbose, bytes_per_thread=self._bytes_per_thread, max_threads=self._max_threads)
+        x = _get_bytes(
+            self._url,
+            data_start,
+            data_end,
+            verbose=self._verbose,
+            bytes_per_thread=self._bytes_per_thread,
+            max_threads=self._max_threads,
+            _impose_request_failures_for_testing=self._impose_request_failures_for_testing
+        )
         if self._smart_loader_chunk_sequence_length == 1:
             self._chunks[chunk_index] = x
             self._chunk_indices.append(chunk_index)
         else:
             for i in range(self._smart_loader_chunk_sequence_length):
                 self._chunks[chunk_index + i] = x[i * self._min_chunk_size:(i + 1) * self._min_chunk_size]
                 self._chunk_indices.append(chunk_index + i)
@@ -158,15 +170,17 @@
 
     def tell(self):
         return self._position
 
     def close(self):
         pass
 
-def _get_bytes(url: str, start_byte: int, end_byte: int, *, verbose=False, bytes_per_thread: int, max_threads: int):
+_num_request_retries = 8
+
+def _get_bytes(url: str, start_byte: int, end_byte: int, *, verbose=False, bytes_per_thread: int, max_threads: int, _impose_request_failures_for_testing=False):
     """Get bytes from a remote file.
 
     Args:
         url (str): The url of the remote file.
         start_byte (int): The first byte to get.
         end_byte (int): The last byte to get.
         bytes_per_thread (int): The minimum number of bytes to load in each thread.
@@ -175,50 +189,66 @@
 
     Returns:
         _type_: _description_
     """
     num_bytes = end_byte - start_byte + 1
 
     # Function to be used in threads for fetching the byte ranges
-    def fetch_bytes(range_start: int, range_end: int):
+    def fetch_bytes(range_start: int, range_end: int, num_retries: int, verbose: bool):
         """Fetch a range of bytes from a remote file using the range header
 
         Args:
             range_start (int): The first byte to get.
             range_end (int): The last byte to get.
 
         Returns:
             bytes: The bytes fetched.
+            num_retries (int): The number of retries.
         """
-        range_header = f"bytes={range_start}-{range_end}"
-        response = requests.get(url, headers={'Range': range_header})
-        return response.content
+        for try_num in range(num_retries + 1):
+            try:
+                actual_url = url
+                if _impose_request_failures_for_testing:
+                    if try_num == 0:
+                        actual_url = '_error_' + url
+                range_header = f"bytes={range_start}-{range_end}"
+                response = requests.get(actual_url, headers={'Range': range_header})
+                return response.content
+            except Exception as e:
+                if try_num == num_retries:
+                    raise e # pragma: no cover
+                else:
+                    delay = 0.1 * 2 ** try_num
+                    if verbose:
+                        print(f"Retrying after exception: {e}")
+                        print(f'Waiting {delay} seconds')
+                    time.sleep(delay)
 
     if num_bytes < bytes_per_thread * 2:
         # If the number of bytes is less than 2 times the bytes_per_thread,
         # then we can just use a single thread
-        return fetch_bytes(start_byte, end_byte)
+        return fetch_bytes(start_byte, end_byte, _num_request_retries, verbose)
     else:
         num_threads = num_bytes // bytes_per_thread
         if num_threads > max_threads:
             num_threads = max_threads
-        byte_ranges = []
+        thread_args = []
         a = start_byte
         for i in range(num_threads):
             if i == num_threads - 1:
                 b = end_byte
             else:
                 b = a + num_bytes // num_threads - 1
-            byte_ranges.append((a, b))
+            thread_args.append((a, b, _num_request_retries, verbose))
             a = b + 1
         
         if verbose:
             print(f"Fetching {num_bytes} bytes in {num_threads} threads")
 
         # Using ThreadPoolExecutor to manage the threads
         with ThreadPoolExecutor(max_workers=num_threads) as executor:
             # Mapping fetch_bytes function to the byte_ranges
-            results = list(executor.map(lambda r: fetch_bytes(*r), byte_ranges))
+            results = list(executor.map(lambda r: fetch_bytes(*r), thread_args))
 
         # Concatenating the results to form the final content
         final_content = b''.join(results)
         return final_content
```

### Comparing `remfile-0.1.4/remfile.egg-info/PKG-INFO` & `remfile-0.1.5/remfile.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: remfile
-Version: 0.1.4
+Version: 0.1.5
 Summary: File-like object from url of remote file, optimized for use with h5py.
 Home-page: https://github.com/magland/remfile
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # remfile
 
 [![latest-release](https://img.shields.io/pypi/v/remfile.svg)](https://pypi.org/project/remfile)
 ![tests](https://github.com/magland/remfile/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/magland/remfile/branch/main/graph/badge.svg)](https://codecov.io/gh/magland/remfile)
 
-
 Provides a file-like object for reading a remote file over HTTP, optimized for use with h5py.
 
 Example usage:
 
 ```python
 # See examples/example1.py
 
@@ -51,14 +50,18 @@
 
 A file-like object is created that reads the remote file in chunks using the requests library. A relatively small default chunk size is used, but when the system detects that a large data array is being accessed, it switches to a larger chunk size. For very large data arrays, the system will use multiple threads to read the data in parallel.
 
 ## Caveats
 
 This library is not intended to be a general purpose library for reading remote files. It is optimized for reading hdf5 files.
 
+At this time, remfile provides only an in-memory cache, not an on-disk cache.
+
+At this time, remfile does not do automatic retries for failed requests.
+
 ## License
 
 Apache 2.0
 
 ## Author
 
 Jeremy Magland, Center for Computational Mathematics, Flatiron Institute
```

### Comparing `remfile-0.1.4/setup.py` & `remfile-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README.md
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 setup(
     name='remfile',
     version=__version__,
     author="Jeremy Magland",
     author_email="jmagland@flatironinstitute.org",
     url="https://github.com/magland/remfile",
```

### Comparing `remfile-0.1.4/tests/test_main.py` & `remfile-0.1.5/tests/test_main.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,9 +49,14 @@
 
     print(sum0)
     assert sum0 == 110503440
 
 def test_for_coverage():
     url = 'https://dandiarchive.s3.amazonaws.com/blobs/d86/055/d8605573-4639-4b99-a6d9-e0ac13f9a7df'
 
-    f = remfile.File(url)
+    f = remfile.File(url, _impose_request_failures_for_testing=True, verbose=True)
+
+    file = h5py.File(f)
+
+    assert file.attrs['neurodata_type'] == 'NWBFile'
+
     f.close()
```

