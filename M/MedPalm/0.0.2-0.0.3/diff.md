# Comparing `tmp/MedPalm-0.0.2.tar.gz` & `tmp/MedPalm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MedPalm-0.0.2.tar", last modified: Mon Jul 31 04:24:24 2023, max compression
+gzip compressed data, was "MedPalm-0.0.3.tar", last modified: Tue Aug  8 13:11:43 2023, max compression
```

## Comparing `MedPalm-0.0.2.tar` & `MedPalm-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:24:24.067710 MedPalm-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 04:24:12.000000 MedPalm-0.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:24:24.063710 MedPalm-0.0.2/MedPalm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-31 04:24:24.000000 MedPalm-0.0.2/MedPalm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-31 04:24:24.000000 MedPalm-0.0.2/MedPalm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 04:24:24.000000 MedPalm-0.0.2/MedPalm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-31 04:24:24.000000 MedPalm-0.0.2/MedPalm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 04:24:24.000000 MedPalm-0.0.2/MedPalm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-31 04:24:24.067710 MedPalm-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-31 04:24:12.000000 MedPalm-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:24:24.067710 MedPalm-0.0.2/med_palm/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15166 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)    20650 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/ppo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/reward_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-31 04:24:12.000000 MedPalm-0.0.2/med_palm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 04:24:24.067710 MedPalm-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-31 04:24:12.000000 MedPalm-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:11:43.489018 MedPalm-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-08 13:11:27.000000 MedPalm-0.0.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:11:43.485018 MedPalm-0.0.3/MedPalm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-08 13:11:43.000000 MedPalm-0.0.3/MedPalm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-08 13:11:43.000000 MedPalm-0.0.3/MedPalm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:11:43.000000 MedPalm-0.0.3/MedPalm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-08 13:11:43.000000 MedPalm-0.0.3/MedPalm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 13:11:43.000000 MedPalm-0.0.3/MedPalm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-08 13:11:43.485018 MedPalm-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-08-08 13:11:27.000000 MedPalm-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:11:43.485018 MedPalm-0.0.3/med_palm/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 13:11:27.000000 MedPalm-0.0.3/med_palm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-08-08 13:11:27.000000 MedPalm-0.0.3/med_palm/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-08 13:11:27.000000 MedPalm-0.0.3/med_palm/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16026 2023-08-08 13:11:27.000000 MedPalm-0.0.3/med_palm/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-08 13:11:27.000000 MedPalm-0.0.3/med_palm/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-08-08 13:11:27.000000 MedPalm-0.0.3/med_palm/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20646 2023-08-08 13:11:27.000000 MedPalm-0.0.3/med_palm/ppo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-08 13:11:27.000000 MedPalm-0.0.3/med_palm/reward_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-08-08 13:11:27.000000 MedPalm-0.0.3/med_palm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 13:11:43.489018 MedPalm-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-08 13:11:27.000000 MedPalm-0.0.3/setup.py
```

### Comparing `MedPalm-0.0.2/LICENSE` & `MedPalm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MedPalm-0.0.2/MedPalm.egg-info/PKG-INFO` & `MedPalm-0.0.3/MedPalm.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedPalm
-Version: 0.0.2
+Version: 0.0.3
 Summary: MedPalm - Pytorch
 Home-page: https://github.com/kyegomez/med-palm
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MedPalm-0.0.2/PKG-INFO` & `MedPalm-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedPalm
-Version: 0.0.2
+Version: 0.0.3
 Summary: MedPalm - Pytorch
 Home-page: https://github.com/kyegomez/med-palm
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MedPalm-0.0.2/med_palm/attention.py` & `MedPalm-0.0.3/med_palm/attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import torch
-from torch import nn, einsum
-import torch.nn.functional as F
-
 from collections import namedtuple
 from functools import wraps
-from packaging import version
 
+import torch
+import torch.nn.functional as F
 from einops import rearrange
+from packaging import version
+from torch import einsum, nn
 
 # constants
 
 Config = namedtuple('EfficientAttentionConfig', ['enable_flash', 'enable_math', 'enable_mem_efficient'])
 
 # helpers
```

### Comparing `MedPalm-0.0.2/med_palm/lora.py` & `MedPalm-0.0.3/med_palm/lora.py`

 * *Files identical despite different names*

### Comparing `MedPalm-0.0.2/med_palm/optimizer.py` & `MedPalm-0.0.3/med_palm/optimizer.py`

 * *Files identical despite different names*

### Comparing `MedPalm-0.0.2/med_palm/palm.py` & `MedPalm-0.0.3/med_palm/palm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from pathlib import Path
 from itertools import zip_longest
-
-from tqdm import tqdm
-from beartype import beartype
+from pathlib import Path
 
 import torch
-from torch import nn
 import torch.nn.functional as F
-
-from einops import rearrange, pack, unpack
+from beartype import beartype
+from einops import pack, rearrange, unpack
+from torch import nn
+from tqdm import tqdm
 
 from med_palm.attention import Attention
-from med_palm.utils import top_k, gumbel_sample, eval_decorator
-from med_palm.lora import LoRA
+from med_palm.utils import eval_decorator, gumbel_sample, top_k
+from med_palm.lora import Lora
 
 # functions and decorators
 
 def exists(val):
     return val is not None
 
 def default(val, d):
@@ -340,18 +338,18 @@
         q_inner_dim = heads * dim_head
         kv_inner_dim = dim_head
 
         lora_modules = nn.ModuleList([])
 
         for _ in range(len(self.layers)):
             lora_modules.append(nn.ModuleList([
-                LoRA(dim, q_inner_dim, r = r),   # queries
-                LoRA(dim, kv_inner_dim, r = r),  # keys
-                LoRA(dim, kv_inner_dim, r = r),  # values
-                LoRA(q_inner_dim, dim, r = r)    # wo
+                Lora(dim, q_inner_dim, r = r),   # queries
+                Lora(dim, kv_inner_dim, r = r),  # keys
+                Lora(dim, kv_inner_dim, r = r),  # values
+                Lora(q_inner_dim, dim, r = r)    # wo
             ]))
 
         self.finetune_modules[scope] = lora_modules.to(device)
 
     def remove_finetune_params(self, scope):
         assert scope in self.finetune_modules, f'finetune scope {scope} not found'
         return self.finetune_modules.pop(scope)
```

### Comparing `MedPalm-0.0.2/med_palm/ppo.py` & `MedPalm-0.0.3/med_palm/ppo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,30 @@
-import math
-from pathlib import Path
 import copy
-from tqdm import tqdm
-from functools import partial
+import math
 from collections import deque, namedtuple
+from functools import partial
+from pathlib import Path
 from random import randrange
 
-from beartype import beartype
-from beartype.typing import List, Optional, Callable, Deque
-
 import torch
-from torch import nn
 import torch.nn.functional as F
-
-from torch.utils.data import Dataset, DataLoader
-from torch.nn.utils.rnn import pad_sequence
-
+from accelerate import Accelerator
+from beartype import beartype
+from beartype.typing import Callable, Deque, List, Optional
 from einops import rearrange, repeat
 from einops.layers.torch import Rearrange
+from torch import nn
+from torch.nn.utils.rnn import pad_sequence
+from torch.utils.data import DataLoader, Dataset
+from tqdm import tqdm
 
+from med_palm.optimizer import get_optimizer
 from med_palm.palm import PaLM
 from med_palm.reward import RewardModel
-from med_palm.optimizer import get_optimizer
-from med_palm.utils import masked_mean, eval_decorator
-
-from accelerate import Accelerator
+from med_palm.utils import eval_decorator, masked_mean
 
 # actor critic - PaLM with lora
 
 PPOActionCriticReturn = namedtuple('PPOActionCriticReturn', [
     'actions',
     'sequence',
     'mask',
```

### Comparing `MedPalm-0.0.2/med_palm/reward_model.py` & `MedPalm-0.0.3/med_palm/reward_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import copy
 from pathlib import Path
 
-from beartype import beartype
-
 import torch
-from torch import nn
 import torch.nn.functional as F
-
+from beartype import beartype
 from einops import rearrange, repeat
 from einops.layers.torch import Rearrange
+from torch import nn
 
-from med_palm.utils import masked_mean, gumbel_sample
 from med_palm.palm import PaLM
+from med_palm.utils import gumbel_sample, masked_mean
 
 # helper functions
 
 def exists(val):
     return val is not None
 
 # Reward Model - PaLM with a scalar head
```

### Comparing `MedPalm-0.0.2/med_palm/utils.py` & `MedPalm-0.0.3/med_palm/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import math
 
 import torch
 import torch.nn.functional as F
 from einops import rearrange
 
 
-
 # helpers
 def exists(val):
     return val is not None
 
 
 #decorators
 def eval_decorator(fn):
```

### Comparing `MedPalm-0.0.2/setup.py` & `MedPalm-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MedPalm',
   packages = find_packages(exclude=['examples']),
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT',
   description = 'MedPalm - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   url = 'https://github.com/kyegomez/med-palm',
   long_description_content_type = 'text/markdown',
   keywords = [
     'artificial intelligence',
     'attention mechanism',
     'transformers'
   ],
   install_requires=[
-    "torch"
+    "torch",
     "lion-pytorch",
     "numpy",
     "einops",
     "accelerate",
     "transformers",
     "SentencePiece",
     "datasets",
```

