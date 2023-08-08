# Comparing `tmp/sihl-0.0.3.dev5.tar.gz` & `tmp/sihl-0.0.3.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sihl-0.0.3.dev5.tar", max compression
+gzip compressed data, was "sihl-0.0.3.dev6.tar", max compression
```

## Comparing `sihl-0.0.3.dev5.tar` & `sihl-0.0.3.dev6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1063 2023-08-07 00:26:21.459815 sihl-0.0.3.dev5/LICENSE
--rw-r--r--   0        0        0      894 2023-08-07 00:26:21.459815 sihl-0.0.3.dev5/README.md
--rw-r--r--   0        0        0     1568 2023-08-07 00:26:39.580005 sihl-0.0.3.dev5/pyproject.toml
--rw-r--r--   0        0        0   402648 2023-08-07 00:26:21.463815 sihl-0.0.3.dev5/src/sihl/NotoSansMono-Bold.ttf
--rw-r--r--   0        0        0      448 2023-08-07 00:26:21.463815 sihl-0.0.3.dev5/src/sihl/__init__.py
--rw-r--r--   0        0        0      289 2023-08-07 00:26:21.463815 sihl-0.0.3.dev5/src/sihl/heads/__init__.py
--rw-r--r--   0        0        0     3241 2023-08-07 00:26:39.580005 sihl-0.0.3.dev5/src/sihl/heads/binary_classification.py
--rw-r--r--   0        0        0     3962 2023-08-07 00:26:39.580005 sihl-0.0.3.dev5/src/sihl/heads/multiclass_classification.py
--rw-r--r--   0        0        0     4942 2023-08-07 00:26:39.580005 sihl-0.0.3.dev5/src/sihl/heads/multilabel_classification.py
--rw-r--r--   0        0        0    14319 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/heads/object_detection.py
--rw-r--r--   0        0        0      189 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/layers/__init__.py
--rw-r--r--   0        0        0     1553 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/layers/convblocks.py
--rw-r--r--   0        0        0     2711 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/layers/fpn.py
--rw-r--r--   0        0        0      514 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/layers/scalers.py
--rw-r--r--   0        0        0     5215 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/lightning_module.py
--rw-r--r--   0        0        0      549 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/sihl_model.py
--rw-r--r--   0        0        0     2797 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/timm_backbone.py
--rw-r--r--   0        0        0     6509 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/torchvision_backbone.py
--rw-r--r--   0        0        0     1740 2023-08-07 00:26:21.467815 sihl-0.0.3.dev5/src/sihl/utils.py
--rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 sihl-0.0.3.dev5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-08 11:26:39.341832 sihl-0.0.3.dev6/LICENSE
+-rw-r--r--   0        0        0      894 2023-08-08 11:26:39.341832 sihl-0.0.3.dev6/README.md
+-rw-r--r--   0        0        0     1568 2023-08-08 11:26:53.582009 sihl-0.0.3.dev6/pyproject.toml
+-rw-r--r--   0        0        0   402648 2023-08-08 11:26:39.349832 sihl-0.0.3.dev6/src/sihl/NotoSansMono-Bold.ttf
+-rw-r--r--   0        0        0      448 2023-08-08 11:26:39.349832 sihl-0.0.3.dev6/src/sihl/__init__.py
+-rw-r--r--   0        0        0      289 2023-08-08 11:26:39.349832 sihl-0.0.3.dev6/src/sihl/heads/__init__.py
+-rw-r--r--   0        0        0     3326 2023-08-08 11:26:53.582009 sihl-0.0.3.dev6/src/sihl/heads/binary_classification.py
+-rw-r--r--   0        0        0     4094 2023-08-08 11:26:53.582009 sihl-0.0.3.dev6/src/sihl/heads/multiclass_classification.py
+-rw-r--r--   0        0        0     5086 2023-08-08 11:26:53.582009 sihl-0.0.3.dev6/src/sihl/heads/multilabel_classification.py
+-rw-r--r--   0        0        0    14568 2023-08-08 11:26:53.582009 sihl-0.0.3.dev6/src/sihl/heads/object_detection.py
+-rw-r--r--   0        0        0      189 2023-08-08 11:26:39.349832 sihl-0.0.3.dev6/src/sihl/layers/__init__.py
+-rw-r--r--   0        0        0     1553 2023-08-08 11:26:39.349832 sihl-0.0.3.dev6/src/sihl/layers/convblocks.py
+-rw-r--r--   0        0        0     2711 2023-08-08 11:26:39.349832 sihl-0.0.3.dev6/src/sihl/layers/fpn.py
+-rw-r--r--   0        0        0      514 2023-08-08 11:26:39.349832 sihl-0.0.3.dev6/src/sihl/layers/scalers.py
+-rw-r--r--   0        0        0     5215 2023-08-08 11:26:39.349832 sihl-0.0.3.dev6/src/sihl/lightning_module.py
+-rw-r--r--   0        0        0      549 2023-08-08 11:26:39.349832 sihl-0.0.3.dev6/src/sihl/sihl_model.py
+-rw-r--r--   0        0        0     2797 2023-08-08 11:26:39.349832 sihl-0.0.3.dev6/src/sihl/timm_backbone.py
+-rw-r--r--   0        0        0     6509 2023-08-08 11:26:39.349832 sihl-0.0.3.dev6/src/sihl/torchvision_backbone.py
+-rw-r--r--   0        0        0     1740 2023-08-08 11:26:39.349832 sihl-0.0.3.dev6/src/sihl/utils.py
+-rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 sihl-0.0.3.dev6/PKG-INFO
```

### Comparing `sihl-0.0.3.dev5/LICENSE` & `sihl-0.0.3.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev5/README.md` & `sihl-0.0.3.dev6/README.md`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev5/pyproject.toml` & `sihl-0.0.3.dev6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sihl"
-version = "0.0.3-dev5"
+version = "0.0.3-dev6"
 description = "Simple Image Heads and Layers"
 authors = ["jonregef <jon.regef@pm.me>"]
 readme = "README.md"
 license = "MIT"
 # homepage = "https://github.com/sihlAI/sihl"
 # repository = "https://github.com/sihlAI/sihl"
```

### Comparing `sihl-0.0.3.dev5/src/sihl/NotoSansMono-Bold.ttf` & `sihl-0.0.3.dev6/src/sihl/NotoSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev5/src/sihl/heads/binary_classification.py` & `sihl-0.0.3.dev6/src/sihl/heads/binary_classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     ) -> None:
         super().__init__()
         self.level = level
         self.net = nn.Sequential(
             nn.AdaptiveAvgPool2d(1), nn.Flatten(), nn.Linear(in_channels[self.level], 1)
         )
         self.question = question
+        self.output_shapes = {"scores": ("batch_size",), "classes": ("batch_size",)}
 
     def forward(self, inputs: list[Tensor]) -> tuple[Tensor, Tensor]:
         scores = torch.sigmoid(self.net(inputs[self.level])).squeeze(-1)
         return scores, scores > 0.5
 
     def training_step(
         self, inputs: list[Tensor], labels: Tensor
```

### Comparing `sihl-0.0.3.dev5/src/sihl/heads/multiclass_classification.py` & `sihl-0.0.3.dev6/src/sihl/heads/multiclass_classification.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,18 @@
         self.label_weights = torch.tensor(label_weights) if label_weights else None
         self.label_smoothing = label_smoothing
         self.net = nn.Sequential(
             nn.AdaptiveAvgPool2d(1),
             nn.Flatten(),
             nn.Linear(in_channels[self.level], num_classes),
         )
+        self.output_shapes = {
+            "scores": ("batch_size", num_classes),
+            "classes": ("batch_size",),
+        }
 
     def forward(self, inputs: list[Tensor]) -> tuple[Tensor, Tensor]:
         scores, classes = torch.max(
             torch.nn.functional.softmax(self.net(inputs[self.level]), dim=1), dim=1
         )
         return scores, classes
```

### Comparing `sihl-0.0.3.dev5/src/sihl/heads/multilabel_classification.py` & `sihl-0.0.3.dev6/src/sihl/heads/multilabel_classification.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,18 @@
         assert len(self.class_names) == self.num_classes
         self.label_weights = torch.tensor(label_weights) if label_weights else None
         self.net = nn.Sequential(
             nn.AdaptiveAvgPool2d(1),
             nn.Flatten(),
             nn.Linear(in_channels[self.level], num_classes),
         )
+        self.output_shapes = {
+            "scores": ("batch_size", num_classes),
+            "classes": ("batch_size", num_classes),
+        }
 
     def forward(self, inputs: list[Tensor]) -> tuple[Tensor, Tensor]:
         scores, classes = torch.sort(
             torch.sigmoid(self.net(inputs[self.level])), descending=True
         )
         return scores, classes
```

### Comparing `sihl-0.0.3.dev5/src/sihl/heads/object_detection.py` & `sihl-0.0.3.dev6/src/sihl/heads/object_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,20 @@
         )
         self.box_head.append(nn.Conv2d(num_channels, 4, 3, padding=1))
         self.box_head.append(nn.ReLU())
         self.apply(init_weights)
         self.tal_alpha, self.tal_beta, self.tal_topk, self.loss_gamma = 1, 6, 13, 2
         self.register_buffer("thresh", torch.tensor(0.5))
         self.register_buffer("signs", torch.tensor([-1, -1, 1, 1]).reshape(1, 1, 4))
+        self.output_shapes = {
+            "num_instances": ("batch_size",),
+            "scores": ("batch_size", max_instances),
+            "classes": ("batch_size", max_instances),
+            "boxes": ("batch_size", max_instances, 4),
+        }
 
     def forward_single_level(self, input: Tensor, level: int) -> tuple[Tensor, Tensor]:
         """Forward pass for a single level.
 
         Args:
             input (Tensor): Level features
             level (int): Level index
```

### Comparing `sihl-0.0.3.dev5/src/sihl/layers/convblocks.py` & `sihl-0.0.3.dev6/src/sihl/layers/convblocks.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev5/src/sihl/layers/fpn.py` & `sihl-0.0.3.dev6/src/sihl/layers/fpn.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev5/src/sihl/layers/scalers.py` & `sihl-0.0.3.dev6/src/sihl/layers/scalers.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev5/src/sihl/lightning_module.py` & `sihl-0.0.3.dev6/src/sihl/lightning_module.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev5/src/sihl/sihl_model.py` & `sihl-0.0.3.dev6/src/sihl/sihl_model.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev5/src/sihl/timm_backbone.py` & `sihl-0.0.3.dev6/src/sihl/timm_backbone.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev5/src/sihl/torchvision_backbone.py` & `sihl-0.0.3.dev6/src/sihl/torchvision_backbone.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev5/src/sihl/utils.py` & `sihl-0.0.3.dev6/src/sihl/utils.py`

 * *Files identical despite different names*

### Comparing `sihl-0.0.3.dev5/PKG-INFO` & `sihl-0.0.3.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sihl
-Version: 0.0.3.dev5
+Version: 0.0.3.dev6
 Summary: Simple Image Heads and Layers
 License: MIT
 Author: jonregef
 Author-email: jon.regef@pm.me
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

