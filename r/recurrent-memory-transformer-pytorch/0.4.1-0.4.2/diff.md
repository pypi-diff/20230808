# Comparing `tmp/recurrent-memory-transformer-pytorch-0.4.1.tar.gz` & `tmp/recurrent-memory-transformer-pytorch-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurrent-memory-transformer-pytorch-0.4.1.tar", last modified: Sat May 27 01:18:31 2023, max compression
+gzip compressed data, was "recurrent-memory-transformer-pytorch-0.4.2.tar", last modified: Tue Aug  8 15:56:11 2023, max compression
```

## Comparing `recurrent-memory-transformer-pytorch-0.4.1.tar` & `recurrent-memory-transformer-pytorch-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:31.592264 recurrent-memory-transformer-pytorch-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-27 01:18:18.000000 recurrent-memory-transformer-pytorch-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-27 01:18:31.592264 recurrent-memory-transformer-pytorch-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-27 01:18:18.000000 recurrent-memory-transformer-pytorch-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:31.592264 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-27 01:18:18.000000 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-27 01:18:18.000000 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-05-27 01:18:18.000000 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:31.592264 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-27 01:18:31.000000 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-27 01:18:31.000000 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 01:18:31.000000 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-27 01:18:31.000000 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-27 01:18:31.000000 recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 01:18:31.592264 recurrent-memory-transformer-pytorch-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-27 01:18:18.000000 recurrent-memory-transformer-pytorch-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:56:11.530894 recurrent-memory-transformer-pytorch-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-08 15:56:01.000000 recurrent-memory-transformer-pytorch-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-08 15:56:11.530894 recurrent-memory-transformer-pytorch-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-08-08 15:56:01.000000 recurrent-memory-transformer-pytorch-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:56:11.530894 recurrent-memory-transformer-pytorch-0.4.2/recurrent_memory_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-08 15:56:01.000000 recurrent-memory-transformer-pytorch-0.4.2/recurrent_memory_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-08-08 15:56:01.000000 recurrent-memory-transformer-pytorch-0.4.2/recurrent_memory_transformer_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-08-08 15:56:01.000000 recurrent-memory-transformer-pytorch-0.4.2/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:56:11.530894 recurrent-memory-transformer-pytorch-0.4.2/recurrent_memory_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-08 15:56:11.000000 recurrent-memory-transformer-pytorch-0.4.2/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-08 15:56:11.000000 recurrent-memory-transformer-pytorch-0.4.2/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:56:11.000000 recurrent-memory-transformer-pytorch-0.4.2/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 15:56:11.000000 recurrent-memory-transformer-pytorch-0.4.2/recurrent_memory_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-08 15:56:11.000000 recurrent-memory-transformer-pytorch-0.4.2/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 15:56:11.530894 recurrent-memory-transformer-pytorch-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-08 15:56:01.000000 recurrent-memory-transformer-pytorch-0.4.2/setup.py
```

### Comparing `recurrent-memory-transformer-pytorch-0.4.1/LICENSE` & `recurrent-memory-transformer-pytorch-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.4.1/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.4.1
+Version: 0.4.2
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.4.1/README.md` & `recurrent-memory-transformer-pytorch-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <img src="./rmt.png" width="450px"></img>
 
 ## Recurrent Memory Transformer - Pytorch
 
 Implementation of <a href="https://arxiv.org/abs/2207.06881">Recurrent Memory Transformer</a> <a href="https://openreview.net/forum?id=Uynr3iPhksa">(openreview)</a> in Pytorch. They had <a href="https://arxiv.org/abs/2304.11062">a short follow up paper</a> recently that demonstrated it was able to copy information across 1 million tokens at the very least.
 
-There is no doubt in my mind that RMT would make a stronger RL agent than <a href="https://sites.google.com/view/adaptive-agent/">AdA</a>, which is just a Transformer-XL
+There is no doubt in my mind that RMT would make a stronger RL agent than <a href="https://sites.google.com/view/adaptive-agent/">AdA</a>, which is just a Transformer-XL - Update: <a href="https://arxiv.org/abs/2306.09459">Recurrent Memory Decision Transformer</a> 
 
 <a href="https://www.youtube.com/watch?v=4Cclp6yPDuw">Yannic Kilcher paper review</a>
 
 ## Appreciation
 
 - <a href="https://stability.ai/">Stability</a> and <a href="https://huggingface.co/">🤗 Huggingface</a> for their generous sponsorships to work on and open source cutting edge artificial intelligence research
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
 [./rmt.png] ## Recurrent Memory Transformer - Pytorch Implementation of
 Recurrent_Memory_Transformer (openreview) in Pytorch. They had a_short_follow
 up_paper recently that demonstrated it was able to copy information across 1
 million tokens at the very least. There is no doubt in my mind that RMT would
-make a stronger RL agent than AdA, which is just a Transformer-XL Yannic
-Kilcher_paper_review ## Appreciation - Stability and ð¤_Huggingface for their
-generous sponsorships to work on and open source cutting edge artificial
-intelligence research ## Install ```bash $ pip install recurrent-memory-
-transformer-pytorch ``` ## Usage ```python import torch from
-recurrent_memory_transformer_pytorch import RecurrentMemoryTransformer model =
-RecurrentMemoryTransformer( num_tokens = 20000, # number of tokens
-num_memory_tokens = 128, # number of memory tokens, this will determine the
-bottleneck for information being passed to the future dim = 512, # model
-dimensions depth = 6, # transformer depth causal = True, # autoregressive or
-not dim_head = 64, # dimension per head heads = 8, # heads seq_len = 1024, #
-sequence length of a segment use_flash_attn = True # whether to use flash
-attention ) x = torch.randint(0, 256, (1, 1024)) logits1, mem1, _ = model(x) #
-(1, 1024, 20000), (1, 128, 512), None logits2, mem2, _ = model(x, mem1) # (1,
-1024, 20000), (1, 128, 512), None logits3, mem3, _ = model(x, mem2) # (1, 1024,
-20000), (1, 128, 512), None # and so on ... ``` With XL memories ```python
-import torch from recurrent_memory_transformer_pytorch import
+make a stronger RL agent than AdA, which is just a Transformer-XL - Update:
+Recurrent_Memory_Decision_Transformer Yannic_Kilcher_paper_review ##
+Appreciation - Stability and ð¤_Huggingface for their generous sponsorships
+to work on and open source cutting edge artificial intelligence research ##
+Install ```bash $ pip install recurrent-memory-transformer-pytorch ``` ## Usage
+```python import torch from recurrent_memory_transformer_pytorch import
+RecurrentMemoryTransformer model = RecurrentMemoryTransformer( num_tokens =
+20000, # number of tokens num_memory_tokens = 128, # number of memory tokens,
+this will determine the bottleneck for information being passed to the future
+dim = 512, # model dimensions depth = 6, # transformer depth causal = True, #
+autoregressive or not dim_head = 64, # dimension per head heads = 8, # heads
+seq_len = 1024, # sequence length of a segment use_flash_attn = True # whether
+to use flash attention ) x = torch.randint(0, 256, (1, 1024)) logits1, mem1, _
+= model(x) # (1, 1024, 20000), (1, 128, 512), None logits2, mem2, _ = model(x,
+mem1) # (1, 1024, 20000), (1, 128, 512), None logits3, mem3, _ = model(x, mem2)
+# (1, 1024, 20000), (1, 128, 512), None # and so on ... ``` With XL memories
+```python import torch from recurrent_memory_transformer_pytorch import
 RecurrentMemoryTransformer model = RecurrentMemoryTransformer( num_tokens =
 20000, num_memory_tokens = 128, dim = 512, depth = 6, causal = True, dim_head =
 64, heads = 8, seq_len = 1024, use_flash_attn = True, use_xl_memories = True, #
 set this to True xl_mem_len = 512 # can be shorter than the seq len - i think
 just having a bit of the past will prevent much of the RMT memories memorizing
 the immediate preceding text ) x = torch.randint(0, 256, (1, 1024)) logits1,
 mem1, xl_mem1 = model(x) # (1, 1024, 20000), (1, 128, 512), [(2, 1, 512, 512)]
```

### Comparing `recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch/attend.py` & `recurrent-memory-transformer-pytorch-0.4.2/recurrent_memory_transformer_pytorch/attend.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,16 +76,17 @@
 
     def flash_attn(self, q, k, v, mask = None):
         _, heads, q_len, _, k_len, is_cuda = *q.shape, k.shape[-2], q.is_cuda
 
         # Check if mask exists and expand to compatible shape
         # The mask is B L, so it would have to be expanded to B H N L
 
-        if exists(mask) and mask.ndim != 4:
-            mask = rearrange(mask, 'b j -> b 1 1 j')
+        if exists(mask):
+            if mask.ndim != 4:
+                mask = rearrange(mask, 'b j -> b 1 1 j')
             mask = mask.expand(-1, heads, q_len, -1)
 
         # Check if there is a compatible device for flash attention
 
         config = self.cuda_config if is_cuda else self.cpu_config
 
         # pytorch 2.0 flash attn: q, k, v, mask, dropout, causal, softmax_scale
@@ -119,15 +120,16 @@
         # similarity
 
         sim = einsum("b h i d, b h j d -> b h i j", q, k) * scale
 
         # key padding mask
 
         if exists(mask):
-            mask = rearrange(mask, 'b j -> b 1 1 j')
+            if mask.ndim != 4:
+                mask = rearrange(mask, 'b j -> b 1 1 j')
             sim = sim.masked_fill(~mask, -torch.finfo(sim.dtype).max)
 
         # causal mask
 
         if self.causal:
             causal_mask = self.get_mask(n, device)
             sim = sim.masked_fill(causal_mask, -torch.finfo(sim.dtype).max)
```

### Comparing `recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py` & `recurrent-memory-transformer-pytorch-0.4.2/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.4.1/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.4.2/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.4.1
+Version: 0.4.2
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.4.1/setup.py` & `recurrent-memory-transformer-pytorch-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'recurrent-memory-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.4.1',
+  version = '0.4.2',
   license='MIT',
   description = 'Recurrent Memory Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/recurrent-memory-transformer-pytorch',
   keywords = [
```

