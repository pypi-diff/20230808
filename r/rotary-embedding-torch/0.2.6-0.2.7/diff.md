# Comparing `tmp/rotary-embedding-torch-0.2.6.tar.gz` & `tmp/rotary-embedding-torch-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotary-embedding-torch-0.2.6.tar", last modified: Fri Aug  4 17:16:25 2023, max compression
+gzip compressed data, was "rotary-embedding-torch-0.2.7.tar", last modified: Tue Aug  8 15:09:10 2023, max compression
```

## Comparing `rotary-embedding-torch-0.2.6.tar` & `rotary-embedding-torch-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:16:25.023728 rotary-embedding-torch-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 17:16:15.000000 rotary-embedding-torch-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-04 17:16:25.023728 rotary-embedding-torch-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-08-04 17:16:15.000000 rotary-embedding-torch-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:16:25.023728 rotary-embedding-torch-0.2.6/rotary_embedding_torch/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-04 17:16:15.000000 rotary-embedding-torch-0.2.6/rotary_embedding_torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-08-04 17:16:15.000000 rotary-embedding-torch-0.2.6/rotary_embedding_torch/rotary_embedding_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:16:25.023728 rotary-embedding-torch-0.2.6/rotary_embedding_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-04 17:16:25.000000 rotary-embedding-torch-0.2.6/rotary_embedding_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-04 17:16:25.000000 rotary-embedding-torch-0.2.6/rotary_embedding_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 17:16:25.000000 rotary-embedding-torch-0.2.6/rotary_embedding_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 17:16:25.000000 rotary-embedding-torch-0.2.6/rotary_embedding_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 17:16:25.000000 rotary-embedding-torch-0.2.6/rotary_embedding_torch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 17:16:25.023728 rotary-embedding-torch-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-08-04 17:16:15.000000 rotary-embedding-torch-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:09:10.044198 rotary-embedding-torch-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-08 15:08:55.000000 rotary-embedding-torch-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-08 15:09:10.044198 rotary-embedding-torch-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-08-08 15:08:55.000000 rotary-embedding-torch-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:09:10.040198 rotary-embedding-torch-0.2.7/rotary_embedding_torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-08 15:08:55.000000 rotary-embedding-torch-0.2.7/rotary_embedding_torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-08-08 15:08:55.000000 rotary-embedding-torch-0.2.7/rotary_embedding_torch/rotary_embedding_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:09:10.044198 rotary-embedding-torch-0.2.7/rotary_embedding_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-08 15:09:10.000000 rotary-embedding-torch-0.2.7/rotary_embedding_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-08 15:09:10.000000 rotary-embedding-torch-0.2.7/rotary_embedding_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:09:10.000000 rotary-embedding-torch-0.2.7/rotary_embedding_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 15:09:10.000000 rotary-embedding-torch-0.2.7/rotary_embedding_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 15:09:10.000000 rotary-embedding-torch-0.2.7/rotary_embedding_torch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 15:09:10.044198 rotary-embedding-torch-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-08-08 15:08:55.000000 rotary-embedding-torch-0.2.7/setup.py
```

### Comparing `rotary-embedding-torch-0.2.6/LICENSE` & `rotary-embedding-torch-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rotary-embedding-torch-0.2.6/PKG-INFO` & `rotary-embedding-torch-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotary-embedding-torch
-Version: 0.2.6
+Version: 0.2.7
 Summary: Rotary Embedding - Pytorch
 Home-page: https://github.com/lucidrains/rotary-embedding-torch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,positional embedding
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rotary-embedding-torch-0.2.6/README.md` & `rotary-embedding-torch-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `rotary-embedding-torch-0.2.6/rotary_embedding_torch/rotary_embedding_torch.py` & `rotary-embedding-torch-0.2.7/rotary_embedding_torch/rotary_embedding_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
     def get_seq_pos(self, seq_len, device, dtype, offset = 0):
         return (torch.arange(seq_len, device = device, dtype = dtype) + offset) / self.interpolate_factor
 
     def rotate_queries_or_keys(self, t, seq_dim = -2, offset = 0):
         assert not self.use_xpos, 'you must use `.rotate_queries_and_keys` method instead and pass in both queries and keys, for length extrapolatable rotary embeddings'
         device, dtype, seq_len = t.device, t.dtype, t.shape[seq_dim]
-        freqs = self.forward(lambda: self.get_seq_pos(seq_len, device = device, dtype = dtype, offset = offset), cache_key = f'freqs:{seq_len}')
+        freqs = self.forward(lambda: self.get_seq_pos(seq_len, device = device, dtype = dtype, offset = offset), cache_key = f'freqs:{seq_len}|offset:{offset}')
         return apply_rotary_emb(freqs, t)
 
     def rotate_queries_and_keys(self, q, k, seq_dim = -2):
         assert self.use_xpos
         device, dtype, seq_len = q.device, q.dtype, q.shape[seq_dim]
         seq = self.get_seq_pos(seq_len, dtype = dtype, device = device)
         freqs = self.forward(lambda: seq, cache_key = f'freqs:{seq_len}')
```

### Comparing `rotary-embedding-torch-0.2.6/rotary_embedding_torch.egg-info/PKG-INFO` & `rotary-embedding-torch-0.2.7/rotary_embedding_torch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotary-embedding-torch
-Version: 0.2.6
+Version: 0.2.7
 Summary: Rotary Embedding - Pytorch
 Home-page: https://github.com/lucidrains/rotary-embedding-torch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,positional embedding
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rotary-embedding-torch-0.2.6/setup.py` & `rotary-embedding-torch-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'rotary-embedding-torch',
   packages = find_packages(),
-  version = '0.2.6',
+  version = '0.2.7',
   license='MIT',
   description = 'Rotary Embedding - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/rotary-embedding-torch',
   keywords = [
```

