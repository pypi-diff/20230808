# Comparing `tmp/LIV-robotics-0.1.0.tar.gz` & `tmp/LIV-robotics-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LIV-robotics-0.1.0.tar", last modified: Mon Jul 31 23:51:26 2023, max compression
+gzip compressed data, was "LIV-robotics-0.1.2.tar", last modified: Mon Aug  7 23:56:49 2023, max compression
```

## Comparing `LIV-robotics-0.1.0.tar` & `LIV-robotics-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:51:26.105502 LIV-robotics-0.1.0/
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)    19346 2023-07-28 00:25:56.000000 LIV-robotics-0.1.0/LICENSE
-drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:51:26.105502 LIV-robotics-0.1.0/LIV_robotics.egg-info/
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     6157 2023-07-31 23:51:26.000000 LIV-robotics-0.1.0/LIV_robotics.egg-info/PKG-INFO
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)      666 2023-07-31 23:51:26.000000 LIV-robotics-0.1.0/LIV_robotics.egg-info/SOURCES.txt
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)        1 2023-07-31 23:51:26.000000 LIV-robotics-0.1.0/LIV_robotics.egg-info/dependency_links.txt
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)      229 2023-07-31 23:51:26.000000 LIV-robotics-0.1.0/LIV_robotics.egg-info/requires.txt
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)        4 2023-07-31 23:51:26.000000 LIV-robotics-0.1.0/LIV_robotics.egg-info/top_level.txt
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     6157 2023-07-31 23:51:26.105502 LIV-robotics-0.1.0/PKG-INFO
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     5598 2023-07-28 00:25:56.000000 LIV-robotics-0.1.0/README.md
-drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:51:26.101502 LIV-robotics-0.1.0/liv/
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     1995 2023-07-31 23:49:50.000000 LIV-robotics-0.1.0/liv/__init__.py
-drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:51:26.101502 LIV-robotics-0.1.0/liv/models/
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)       36 2023-07-28 00:25:57.000000 LIV-robotics-0.1.0/liv/models/__init__.py
-drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:51:26.101502 LIV-robotics-0.1.0/liv/models/clip/
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:23:28.000000 LIV-robotics-0.1.0/liv/models/clip/__init__.py
-drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:51:26.105502 LIV-robotics-0.1.0/liv/models/clip/clip/
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)       20 2023-07-28 00:25:57.000000 LIV-robotics-0.1.0/liv/models/clip/clip/__init__.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)  1356917 2023-07-28 00:25:57.000000 LIV-robotics-0.1.0/liv/models/clip/clip/bpe_simple_vocab_16e6.txt.gz
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     9445 2023-07-28 00:25:57.000000 LIV-robotics-0.1.0/liv/models/clip/clip/clip.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)    17411 2023-07-28 00:25:57.000000 LIV-robotics-0.1.0/liv/models/clip/clip/model.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     4632 2023-07-28 00:25:57.000000 LIV-robotics-0.1.0/liv/models/clip/clip/simple_tokenizer.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     3683 2023-07-31 22:57:04.000000 LIV-robotics-0.1.0/liv/models/model_liv.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     6835 2023-07-28 00:25:57.000000 LIV-robotics-0.1.0/liv/train_liv.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     4635 2023-07-28 00:25:57.000000 LIV-robotics-0.1.0/liv/trainer.py
-drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:51:26.105502 LIV-robotics-0.1.0/liv/utils/
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)      262 2023-07-28 00:25:57.000000 LIV-robotics-0.1.0/liv/utils/__init__.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     5928 2023-07-28 00:25:57.000000 LIV-robotics-0.1.0/liv/utils/data_loaders.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     5934 2023-07-28 00:25:57.000000 LIV-robotics-0.1.0/liv/utils/logger.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     5591 2023-07-28 00:25:57.000000 LIV-robotics-0.1.0/liv/utils/plotter.py
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     4777 2023-07-28 00:25:57.000000 LIV-robotics-0.1.0/liv/utils/utils.py
--rw-r--r--   0 haonanyu  (1000) haonanyu  (1000)      616 2023-07-31 23:51:13.000000 LIV-robotics-0.1.0/pyproject.toml
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)       38 2023-07-31 23:51:26.105502 LIV-robotics-0.1.0/setup.cfg
--rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     1154 2023-07-31 23:51:18.000000 LIV-robotics-0.1.0/setup.py
+drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-08-07 23:56:49.438046 LIV-robotics-0.1.2/
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)    19346 2023-07-28 00:25:56.000000 LIV-robotics-0.1.2/LICENSE
+drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-08-07 23:56:49.438046 LIV-robotics-0.1.2/LIV_robotics.egg-info/
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     6157 2023-08-07 23:56:49.000000 LIV-robotics-0.1.2/LIV_robotics.egg-info/PKG-INFO
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)      666 2023-08-07 23:56:49.000000 LIV-robotics-0.1.2/LIV_robotics.egg-info/SOURCES.txt
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)        1 2023-08-07 23:56:49.000000 LIV-robotics-0.1.2/LIV_robotics.egg-info/dependency_links.txt
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)      230 2023-08-07 23:56:49.000000 LIV-robotics-0.1.2/LIV_robotics.egg-info/requires.txt
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)        4 2023-08-07 23:56:49.000000 LIV-robotics-0.1.2/LIV_robotics.egg-info/top_level.txt
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     6157 2023-08-07 23:56:49.438046 LIV-robotics-0.1.2/PKG-INFO
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     5598 2023-07-28 00:25:56.000000 LIV-robotics-0.1.2/README.md
+drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-08-07 23:56:49.438046 LIV-robotics-0.1.2/liv/
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     1995 2023-07-31 23:53:09.000000 LIV-robotics-0.1.2/liv/__init__.py
+drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-08-07 23:56:49.438046 LIV-robotics-0.1.2/liv/models/
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)       36 2023-07-28 00:25:57.000000 LIV-robotics-0.1.2/liv/models/__init__.py
+drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-08-07 23:56:49.438046 LIV-robotics-0.1.2/liv/models/clip/
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)        0 2023-07-31 23:23:28.000000 LIV-robotics-0.1.2/liv/models/clip/__init__.py
+drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-08-07 23:56:49.438046 LIV-robotics-0.1.2/liv/models/clip/clip/
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)       20 2023-07-28 00:25:57.000000 LIV-robotics-0.1.2/liv/models/clip/clip/__init__.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)  1356917 2023-07-28 00:25:57.000000 LIV-robotics-0.1.2/liv/models/clip/clip/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     9482 2023-08-04 03:15:08.000000 LIV-robotics-0.1.2/liv/models/clip/clip/clip.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)    17895 2023-08-04 03:29:35.000000 LIV-robotics-0.1.2/liv/models/clip/clip/model.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     4632 2023-07-28 00:25:57.000000 LIV-robotics-0.1.2/liv/models/clip/clip/simple_tokenizer.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     3969 2023-08-04 00:40:05.000000 LIV-robotics-0.1.2/liv/models/model_liv.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     6835 2023-07-28 00:25:57.000000 LIV-robotics-0.1.2/liv/train_liv.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     4635 2023-07-28 00:25:57.000000 LIV-robotics-0.1.2/liv/trainer.py
+drwxrwxr-x   0 haonanyu  (1000) haonanyu  (1000)        0 2023-08-07 23:56:49.438046 LIV-robotics-0.1.2/liv/utils/
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)      262 2023-07-28 00:25:57.000000 LIV-robotics-0.1.2/liv/utils/__init__.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     5928 2023-07-28 00:25:57.000000 LIV-robotics-0.1.2/liv/utils/data_loaders.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     5934 2023-07-28 00:25:57.000000 LIV-robotics-0.1.2/liv/utils/logger.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     5591 2023-07-28 00:25:57.000000 LIV-robotics-0.1.2/liv/utils/plotter.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     4777 2023-07-28 00:25:57.000000 LIV-robotics-0.1.2/liv/utils/utils.py
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)      616 2023-08-07 23:56:29.000000 LIV-robotics-0.1.2/pyproject.toml
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)       38 2023-08-07 23:56:49.438046 LIV-robotics-0.1.2/setup.cfg
+-rw-rw-r--   0 haonanyu  (1000) haonanyu  (1000)     1155 2023-08-07 23:56:34.000000 LIV-robotics-0.1.2/setup.py
```

### Comparing `LIV-robotics-0.1.0/LICENSE` & `LIV-robotics-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.1.0/LIV_robotics.egg-info/PKG-INFO` & `LIV-robotics-0.1.2/LIV_robotics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LIV-robotics
-Version: 0.1.0
+Version: 0.1.2
 Summary: LIV: Language-Image Representations and Rewards for Robotic Control
 Author: Jason Ma
 Author-email: Jason Ma <jasonyma@seas.upenn.edu>
 Project-URL: Homepage, https://github.com/penn-pal-lab/LIV
 Project-URL: Bug Tracker, https://github.com/penn-pal-lab/LIV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LIV-robotics-0.1.0/LIV_robotics.egg-info/SOURCES.txt` & `LIV-robotics-0.1.2/LIV_robotics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.1.0/PKG-INFO` & `LIV-robotics-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LIV-robotics
-Version: 0.1.0
+Version: 0.1.2
 Summary: LIV: Language-Image Representations and Rewards for Robotic Control
 Author: Jason Ma
 Author-email: Jason Ma <jasonyma@seas.upenn.edu>
 Project-URL: Homepage, https://github.com/penn-pal-lab/LIV
 Project-URL: Bug Tracker, https://github.com/penn-pal-lab/LIV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LIV-robotics-0.1.0/README.md` & `LIV-robotics-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.1.0/liv/__init__.py` & `LIV-robotics-0.1.2/liv/__init__.py`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.1.0/liv/models/clip/clip/bpe_simple_vocab_16e6.txt.gz` & `LIV-robotics-0.1.2/liv/models/clip/clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.1.0/liv/models/clip/clip/clip.py` & `LIV-robotics-0.1.2/liv/models/clip/clip/clip.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,18 +47,19 @@
     expected_sha256 = url.split("/")[-2]
     download_target = os.path.join(root, filename)
 
     if os.path.exists(download_target) and not os.path.isfile(download_target):
         raise RuntimeError(f"{download_target} exists and is not a regular file")
 
     if os.path.isfile(download_target):
-        if hashlib.sha256(open(download_target, "rb").read()).hexdigest() == expected_sha256:
-            return download_target
-        else:
-            warnings.warn(f"{download_target} exists, but the SHA256 checksum does not match; re-downloading the file")
+        with open(download_target, "rb") as f:
+            if hashlib.sha256(f.read()).hexdigest() == expected_sha256:
+                return download_target
+            else:
+                warnings.warn(f"{download_target} exists, but the SHA256 checksum does not match; re-downloading the file")
 
     with urllib.request.urlopen(url) as source, open(download_target, "wb") as output:
         with tqdm(total=int(source.info().get("Content-Length")), ncols=80, unit='iB', unit_scale=True, unit_divisor=1024) as loop:
             while True:
                 buffer = source.read(8192)
                 if not buffer:
                     break
```

### Comparing `LIV-robotics-0.1.0/liv/models/clip/clip/model.py` & `LIV-robotics-0.1.2/liv/models/clip/clip/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,30 +130,34 @@
 
         self._inplanes = planes * Bottleneck.expansion
         for _ in range(1, blocks):
             layers.append(Bottleneck(self._inplanes, planes))
 
         return nn.Sequential(*layers)
 
-    def forward(self, x):
+    def features_forward(self, x):
         def stem(x):
             x = self.relu1(self.bn1(self.conv1(x)))
             x = self.relu2(self.bn2(self.conv2(x)))
             x = self.relu3(self.bn3(self.conv3(x)))
             x = self.avgpool(x)
             return x
 
         x = x.type(self.conv1.weight.dtype)
         x = stem(x)
         x = self.layer1(x)
         x = self.layer2(x)
         x = self.layer3(x)
         x = self.layer4(x)
-        x = self.attnpool(x)
+        # [B,2048,7,7]
+        return x
 
+    def forward(self, x):
+        x = self.features_forward(x)
+        x = self.attnpool(x)
         return x
 
 
 class LayerNorm(nn.LayerNorm):
     """Subclass torch's LayerNorm to handle fp16."""
 
     def forward(self, x: torch.Tensor):
@@ -178,16 +182,21 @@
             ("gelu", QuickGELU()),
             ("c_proj", nn.Linear(d_model * 4, d_model))
         ]))
         self.ln_2 = LayerNorm(d_model)
         self.attn_mask = attn_mask
 
     def attention(self, x: torch.Tensor):
-        self.attn_mask = self.attn_mask.to(dtype=x.dtype, device=x.device) if self.attn_mask is not None else None
-        return self.attn(x, x, x, need_weights=False, attn_mask=self.attn_mask)[0]
+        cxt_len = x.shape[0]
+        if self.attn_mask is not None:
+            attn_mask = self.attn_mask.to(dtype=x.dtype, device=x.device)
+            attn_mask = attn_mask[:cxt_len, :cxt_len]
+        else:
+            attn_mask = None
+        return self.attn(x, x, x, need_weights=False, attn_mask=attn_mask)[0]
 
     def forward(self, x: torch.Tensor):
         x = x + self.attention(self.ln_1(x))
         x = x + self.mlp(self.ln_2(x))
         return x
 
 
@@ -336,16 +345,15 @@
     def dtype(self):
         return self.visual.conv1.weight.dtype
 
     def encode_image(self, image):
         return self.visual(image.type(self.dtype))
 
     def encode_text(self, text):
-        x = self.token_embedding(text).type(self.dtype)  # [batch_size, n_ctx, d_model]
-        x = x + self.positional_embedding.type(self.dtype)
+        x = self.encode_text_as_embeddings(text)
         x = x.permute(1, 0, 2)  # NLD -> LND
         x = self.transformer(x)
         x = x.permute(1, 0, 2)  # LND -> NLD
         x = self.ln_final(x).type(self.dtype)
 
         # x.shape = [batch_size, n_ctx, transformer.width]
         # take features from the eot embedding (eot_token is the highest number in each sequence)
@@ -364,14 +372,23 @@
         logit_scale = self.logit_scale.exp()
         logits_per_image = logit_scale * image_features @ text_features.t()
         logits_per_text = logits_per_image.t()
 
         # shape = [global_batch_size, global_batch_size]
         return logits_per_image, logits_per_text
 
+    def encode_image_as_features(self, image):
+        return self.visual.features_forward(image)
+
+    def encode_text_as_embeddings(self, text):
+        x = self.token_embedding(text).type(self.dtype)  # [batch_size, n_ctx, d_model]
+        n_ctx = x.shape[1]
+        x = x + self.positional_embedding.type(self.dtype)[:n_ctx, ...]
+        return x
+
 
 def convert_weights(model: nn.Module):
     """Convert applicable model parameters to fp16"""
 
     def _convert_weights_to_fp16(l):
         if isinstance(l, (nn.Conv1d, nn.Conv2d, nn.Linear)):
             l.weight.data = l.weight.data.half()
```

### Comparing `LIV-robotics-0.1.0/liv/models/clip/clip/simple_tokenizer.py` & `LIV-robotics-0.1.2/liv/models/clip/clip/simple_tokenizer.py`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.1.0/liv/models/model_liv.py` & `LIV-robotics-0.1.2/liv/models/model_liv.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,14 +78,22 @@
                 with torch.no_grad():
                     features = self.model.encode_text(b_token)
         else:
             raise NotImplementedError
 
         return features
 
+    def encode_image_as_features(self, img):
+        img = self.transforms_tensor(img).to(self.device)
+        # [B,C,H,W]
+        return self.model.encode_image_as_features(img)
+
+    def encode_text_as_embeddings(self, text):
+        return self.model.encode_text_as_embeddings(text)
+
     def sim(self, tensor1, tensor2):
         if type(tensor1) == np.ndarray:
             tensor1 = torch.from_numpy(tensor1).to(self.device)
             tensor2 = torch.from_numpy(tensor2).to(self.device)
         if self.metric == 'l2':
             d = -torch.linalg.norm(tensor1 - tensor2, dim = -1)
         elif self.metric == 'cos':
```

### Comparing `LIV-robotics-0.1.0/liv/train_liv.py` & `LIV-robotics-0.1.2/liv/train_liv.py`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.1.0/liv/trainer.py` & `LIV-robotics-0.1.2/liv/trainer.py`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.1.0/liv/utils/data_loaders.py` & `LIV-robotics-0.1.2/liv/utils/data_loaders.py`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.1.0/liv/utils/logger.py` & `LIV-robotics-0.1.2/liv/utils/logger.py`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.1.0/liv/utils/plotter.py` & `LIV-robotics-0.1.2/liv/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.1.0/liv/utils/utils.py` & `LIV-robotics-0.1.2/liv/utils/utils.py`

 * *Files identical despite different names*

### Comparing `LIV-robotics-0.1.0/pyproject.toml` & `LIV-robotics-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "LIV-robotics"
-version = "0.1.0"
+version = "0.1.2"
 authors = [
   { name="Jason Ma", email="jasonyma@seas.upenn.edu" },
 ]
 description = "LIV: Language-Image Representations and Rewards for Robotic Control"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `LIV-robotics-0.1.0/setup.py` & `LIV-robotics-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name='liv',
-    version='0.1.0',
+    version='0.1.2',
     packages=find_packages(),
     description='LIV: Language-Image Representations and Rewards for Robotic Control',
     long_description=read('README.md'),
     author='Jason Ma',
     install_requires=[
         'torch',
         'torchvision>=0.8.2',
         'omegaconf==2.1.1',
         'hydra-core==1.1.1',
-        'pillow==9.0.1',
+        'pillow==10.0.0',
         'opencv-python',
         'matplotlib',
         'flatten_dict',
         'gdown',
         'huggingface_hub',
         'tabulate',
         'pandas',
```

