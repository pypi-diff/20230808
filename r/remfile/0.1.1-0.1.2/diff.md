# Comparing `tmp/remfile-0.1.1.tar.gz` & `tmp/remfile-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remfile-0.1.1.tar", last modified: Mon Aug  7 19:45:55 2023, max compression
+gzip compressed data, was "remfile-0.1.2.tar", last modified: Mon Aug  7 23:58:09 2023, max compression
```

## Comparing `remfile-0.1.1.tar` & `remfile-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-07 19:45:55.922896 remfile-0.1.1/
--rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-08-07 12:41:38.000000 remfile-0.1.1/LICENSE
--rw-rw-r--   0 magland   (1000) magland   (1000)    15245 2023-08-07 19:45:55.922896 remfile-0.1.1/PKG-INFO
--rw-r--r--   0 magland   (1000) magland   (1000)     1731 2023-08-07 19:45:00.000000 remfile-0.1.1/README.md
--rw-r--r--   0 magland   (1000) magland   (1000)      959 2023-08-07 19:14:40.000000 remfile-0.1.1/pyproject.toml
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-07 19:45:55.922896 remfile-0.1.1/remfile/
--rw-r--r--   0 magland   (1000) magland   (1000)     5454 2023-08-07 19:42:37.000000 remfile-0.1.1/remfile/RemFile.py
--rw-r--r--   0 magland   (1000) magland   (1000)       59 2023-08-07 19:43:40.000000 remfile-0.1.1/remfile/__init__.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-07 19:45:55.922896 remfile-0.1.1/remfile.egg-info/
--rw-r--r--   0 magland   (1000) magland   (1000)    15245 2023-08-07 19:45:55.000000 remfile-0.1.1/remfile.egg-info/PKG-INFO
--rw-r--r--   0 magland   (1000) magland   (1000)      244 2023-08-07 19:45:55.000000 remfile-0.1.1/remfile.egg-info/SOURCES.txt
--rw-r--r--   0 magland   (1000) magland   (1000)        1 2023-08-07 19:45:55.000000 remfile-0.1.1/remfile.egg-info/dependency_links.txt
--rw-r--r--   0 magland   (1000) magland   (1000)       29 2023-08-07 19:45:55.000000 remfile-0.1.1/remfile.egg-info/requires.txt
--rw-r--r--   0 magland   (1000) magland   (1000)        8 2023-08-07 19:45:55.000000 remfile-0.1.1/remfile.egg-info/top_level.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       38 2023-08-07 19:45:55.922896 remfile-0.1.1/setup.cfg
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-07 19:45:55.922896 remfile-0.1.1/tests/
--rw-rw-r--   0 magland   (1000) magland   (1000)      363 2023-08-07 19:14:23.000000 remfile-0.1.1/tests/test_main.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-07 23:58:09.187381 remfile-0.1.2/
+-rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-08-07 12:41:38.000000 remfile-0.1.2/LICENSE
+-rw-rw-r--   0 magland   (1000) magland   (1000)    15245 2023-08-07 23:58:09.187381 remfile-0.1.2/PKG-INFO
+-rw-r--r--   0 magland   (1000) magland   (1000)     1731 2023-08-07 19:45:00.000000 remfile-0.1.2/README.md
+-rw-r--r--   0 magland   (1000) magland   (1000)      959 2023-08-07 19:14:40.000000 remfile-0.1.2/pyproject.toml
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-07 23:58:09.187381 remfile-0.1.2/remfile/
+-rw-r--r--   0 magland   (1000) magland   (1000)     6549 2023-08-07 23:54:25.000000 remfile-0.1.2/remfile/RemFile.py
+-rw-r--r--   0 magland   (1000) magland   (1000)       59 2023-08-07 23:57:25.000000 remfile-0.1.2/remfile/__init__.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-07 23:58:09.187381 remfile-0.1.2/remfile.egg-info/
+-rw-r--r--   0 magland   (1000) magland   (1000)    15245 2023-08-07 23:58:09.000000 remfile-0.1.2/remfile.egg-info/PKG-INFO
+-rw-r--r--   0 magland   (1000) magland   (1000)      244 2023-08-07 23:58:09.000000 remfile-0.1.2/remfile.egg-info/SOURCES.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)        1 2023-08-07 23:58:09.000000 remfile-0.1.2/remfile.egg-info/dependency_links.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)       29 2023-08-07 23:58:09.000000 remfile-0.1.2/remfile.egg-info/requires.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)        8 2023-08-07 23:58:09.000000 remfile-0.1.2/remfile.egg-info/top_level.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       38 2023-08-07 23:58:09.187381 remfile-0.1.2/setup.cfg
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-08-07 23:58:09.187381 remfile-0.1.2/tests/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      363 2023-08-07 19:14:23.000000 remfile-0.1.2/tests/test_main.py
```

### Comparing `remfile-0.1.1/LICENSE` & `remfile-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `remfile-0.1.1/PKG-INFO` & `remfile-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remfile
-Version: 0.1.1
+Version: 0.1.2
 Summary: File-like object from url of remote file, optimized for use with h5py.
 Author-email: Jeremy Magland <jmagland@flatironinstitute.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `remfile-0.1.1/README.md` & `remfile-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `remfile-0.1.1/pyproject.toml` & `remfile-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `remfile-0.1.1/remfile/RemFile.py` & `remfile-0.1.2/remfile/RemFile.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,76 +1,99 @@
 from concurrent.futures import ThreadPoolExecutor
 import requests
 
+min_chunk_size = 100 * 1024
+max_chunks_in_cache = int(1e8 / min_chunk_size)
+
 class RemFile:
     def __init__(self, url, *, verbose=False):
         self._verbose = verbose
-        self._chunk_size = 100 * 1024
         self._chunks = {}
+        self._chunk_indices: list[int] = [] # list of chunk indices in order of loading for purposes of cleaning up the cache
         self._url = url
         self._position = 0
-        self._smart_loader_last_chunk_index_read = -99
+        self._smart_loader_last_chunk_index_accessed = -99
         self._smart_loader_chunk_sequence_length = 1
         response = requests.head(self._url)
         self.length = int(response.headers['Content-Length'])
 
     def read(self, size=None):
         if size is None:
             raise Exception('The size argument must be provided in remfile')
-        chunk_start_index = self._position // self._chunk_size
-        chunk_end_index = (self._position + size - 1) // self._chunk_size
+        
+        chunk_start_index = self._position // min_chunk_size
+        chunk_end_index = (self._position + size - 1) // min_chunk_size
         for chunk_index in range(chunk_start_index, chunk_end_index + 1):
             self._load_chunk(chunk_index)
         if chunk_end_index == chunk_start_index:
             chunk = self._chunks[chunk_start_index]
-            chunk_offset = self._position % self._chunk_size
+            chunk_offset = self._position % min_chunk_size
             chunk_length = size
             self._position += size
             return chunk[chunk_offset:chunk_offset + chunk_length]
         else:
             pieces_to_concat = []
             for chunk_index in range(chunk_start_index, chunk_end_index + 1):
                 chunk = self._chunks[chunk_index]
                 if chunk_index == chunk_start_index:
-                    chunk_offset = self._position % self._chunk_size
-                    chunk_length = self._chunk_size - chunk_offset
+                    chunk_offset = self._position % min_chunk_size
+                    chunk_length = min_chunk_size - chunk_offset
                 elif chunk_index == chunk_end_index:
                     chunk_offset = 0
                     chunk_length = size - sum([len(p) for p in pieces_to_concat])
                 else:
                     chunk_offset = 0
-                    chunk_length = self._chunk_size
+                    chunk_length = min_chunk_size
                 pieces_to_concat.append(chunk[chunk_offset:chunk_offset + chunk_length])
         ret = b''.join(pieces_to_concat)
         self._position += size
+
+        # clean up the cache
+        if len(self._chunk_indices) > max_chunks_in_cache:
+            if self._verbose:
+                print("Cleaning up cache")
+            for chunk_index in self._chunk_indices[:int(max_chunks_in_cache * 0.5)]:
+                del self._chunks[chunk_index]
+            self._chunk_indices = self._chunk_indices[int(max_chunks_in_cache * 0.5):]
+
         return ret
     
     def _load_chunk(self, chunk_index):
         if chunk_index in self._chunks:
+            self._smart_loader_last_chunk_index_accessed = chunk_index
             return
-        if chunk_index == self._smart_loader_last_chunk_index_read + 1:
+
+        if chunk_index == self._smart_loader_last_chunk_index_accessed + 1:
             # round up to the chunk sequence length times 1.7
             self._smart_loader_chunk_sequence_length = round(self._smart_loader_chunk_sequence_length * 1.7 + 0.5)
-            if self._smart_loader_chunk_sequence_length > 15 * 1024 * 1024 / self._chunk_size:
-                self._smart_loader_chunk_sequence_length = int(15 * 1024 * 1024 / self._chunk_size)
+            if self._smart_loader_chunk_sequence_length > 100 * 1024 * 1024 / min_chunk_size:
+                self._smart_loader_chunk_sequence_length = int(100 * 1024 * 1024 / min_chunk_size)
+            # make sure the chunk sequence length is valid
+            for j in range(1, self._smart_loader_chunk_sequence_length):
+                if chunk_index + j in self._chunks:
+                    # already loaded this chunk
+                    self._smart_loader_chunk_sequence_length = j
+                    break
         else:
             self._smart_loader_chunk_sequence_length = 1
-        data_start = chunk_index * self._chunk_size
-        data_end = data_start + self._chunk_size * self._smart_loader_chunk_sequence_length - 1
+        data_start = chunk_index * min_chunk_size
+        data_end = data_start + min_chunk_size * self._smart_loader_chunk_sequence_length - 1
         if self._verbose:
-            print(f"Loading chunks starting at {chunk_index} ({(data_end - data_start + 1)/1e6} million bytes)")
+            print(f"Loading {self._smart_loader_chunk_sequence_length} chunks starting at {chunk_index} ({(data_end - data_start + 1)/1e6} million bytes)")
         if data_end >= self.length:
             data_end = self.length - 1
         x = _get_bytes(self._url, data_start, data_end, verbose=self._verbose)
         if self._smart_loader_chunk_sequence_length == 1:
             self._chunks[chunk_index] = x
+            self._chunk_indices.append(chunk_index)
         else:
             for i in range(self._smart_loader_chunk_sequence_length):
-                self._chunks[chunk_index + i] = x[i * self._chunk_size:(i + 1) * self._chunk_size]
-        self._smart_loader_last_chunk_index_read = chunk_index + self._smart_loader_chunk_sequence_length - 1
+                self._chunks[chunk_index + i] = x[i * min_chunk_size:(i + 1) * min_chunk_size]
+                self._chunk_indices.append(chunk_index + i)
+        self._smart_loader_last_chunk_index_accessed = chunk_index + self._smart_loader_chunk_sequence_length - 1
 
     def seek(self, offset, whence=0):
         if whence == 0:
             self._position = offset
         elif whence == 1:
             self._position += offset
         elif whence == 2:
@@ -80,16 +103,16 @@
 
     def tell(self):
         return self._position
 
     def close(self):
         pass
 
-bytes_per_thread = 3 * 1024 * 1024
-max_threads = 4
+bytes_per_thread = 4 * 1024 * 1024
+max_threads = 3
 
 def _get_bytes(url: str, start_byte: int, end_byte: int, verbose=False):
     num_bytes = end_byte - start_byte + 1
 
     # Function to be used in threads for fetching the byte ranges
     def fetch_bytes(range_start, range_end):
         range_header = f"bytes={range_start}-{range_end}"
```

### Comparing `remfile-0.1.1/remfile.egg-info/PKG-INFO` & `remfile-0.1.2/remfile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remfile
-Version: 0.1.1
+Version: 0.1.2
 Summary: File-like object from url of remote file, optimized for use with h5py.
 Author-email: Jeremy Magland <jmagland@flatironinstitute.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

