# Comparing `tmp/kaparoo_lightning-0.1.1.tar.gz` & `tmp/kaparoo_lightning-0.1.2.tar.gz`

## Comparing `kaparoo_lightning-0.1.1.tar` & `kaparoo_lightning-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,19 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/common/__init__.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/common/spec.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/common/types.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/data/__init__.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/data/constants.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/data/dataloaders.py
--rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/data/datamodules.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/data/datasets/__init__.py
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/data/datasets/datasets.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/data/datasets/traits.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/data/datasets/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/nn/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/nn/models/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/kaparoo_lightning/nn/models/gan.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/LICENSE
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/README.md
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/kaparoo_lightning/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/kaparoo_lightning/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/kaparoo_lightning/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/kaparoo_lightning/common/__init__.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/kaparoo_lightning/common/spec.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/kaparoo_lightning/common/types.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/kaparoo_lightning/data/__init__.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/kaparoo_lightning/data/constants.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/kaparoo_lightning/data/dataloaders.py
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/kaparoo_lightning/data/datamodules.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/kaparoo_lightning/data/datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/kaparoo_lightning/nn/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/kaparoo_lightning/nn/models/__init__.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/kaparoo_lightning/nn/models/gan.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/README.md
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.2/PKG-INFO
```

### Comparing `kaparoo_lightning-0.1.1/kaparoo_lightning/common/spec.py` & `kaparoo_lightning-0.1.2/kaparoo_lightning/common/spec.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.1/kaparoo_lightning/data/__init__.py` & `kaparoo_lightning-0.1.2/kaparoo_lightning/data/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     # dataloaders
     "DataLoaderSpec",
     # datamodules
     "DataModuleBase",
     "DataModule",
     "TransformableDataModule",
     "LabelTransformableDataModule",
+    # datasets
+    "DoubleDomainDataset",
+    "MultiDomainDataset",
 )
 
 from kaparoo_lightning.data.constants import (
     BATCH_SIZE,
     MAX_WORKERS,
     NUM_WORKERS,
     SUBSETS,
@@ -24,7 +27,8 @@
 from kaparoo_lightning.data.dataloaders import DataLoaderSpec
 from kaparoo_lightning.data.datamodules import (
     DataModule,
     DataModuleBase,
     LabelTransformableDataModule,
     TransformableDataModule,
 )
+from kaparoo_lightning.data.datasets import DoubleDomainDataset, MultiDomainDataset
```

### Comparing `kaparoo_lightning-0.1.1/kaparoo_lightning/data/constants.py` & `kaparoo_lightning-0.1.2/kaparoo_lightning/data/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
-__all__ = ("BATCH_SIZE", "MAX_WORKERS", "NUM_WORKERS", "SUBSETS")
+__all__ = ("BATCH_SIZE", "MAX_WORKERS", "NUM_WORKERS", "STAGES", "SUBSETS")
 
 import os
 from typing import TYPE_CHECKING, Final
 
 from torch import cuda
 
 if TYPE_CHECKING:
@@ -24,8 +24,9 @@
 BATCH_SIZE_3XL: Final[int] = 1024 if _USE_GPU else 256
 BATCH_SIZE: Final[int] = BATCH_SIZE_M
 
 _CPU_COUNT = os.cpu_count()
 MAX_WORKERS: Final[int] = _CPU_COUNT if isinstance(_CPU_COUNT, int) else 0
 NUM_WORKERS: Final[int] = MAX_WORKERS // 2
 
+STAGES: Final[tuple[LiteralString, ...]] = ("fit", "validate", "test", "predict")
 SUBSETS: Final[tuple[LiteralString, ...]] = ("train", "valid", "test", "pred")
```

### Comparing `kaparoo_lightning-0.1.1/kaparoo_lightning/data/dataloaders.py` & `kaparoo_lightning-0.1.2/kaparoo_lightning/data/dataloaders.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.1/kaparoo_lightning/data/datamodules.py` & `kaparoo_lightning-0.1.2/kaparoo_lightning/data/datamodules.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.1/kaparoo_lightning/data/datasets/traits.py` & `kaparoo_lightning-0.1.2/kaparoo_lightning/data/datasets.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,81 +1,105 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
-__all__ = ("MultiDomain", "MultiLabeled")
+__all__ = ("MultiDomainDataset", "DoubleDomainDataset")
 
-from collections.abc import Sequence
-from typing import TYPE_CHECKING, Generic
+from collections.abc import Callable, Sequence
+from typing import TYPE_CHECKING, Generic, TypeVar
+
+from torch.utils.data import Dataset
 
 if TYPE_CHECKING:
-    from kaparoo_lightning.data.datasets.types import DataType, LabelType, TransformType
+    from torch import Tensor
+    from typing_extensions import LiteralString
 
+    from kaparoo_lightning.common.types import TensorFn
 
-def unwrap_transforms(
-    transforms: TransformType | Sequence[TransformType | None] | None,
-    max_transforms: int,
-) -> tuple[TransformType | None, ...]:
-    if not isinstance(max_transforms, int) or max_transforms < 1:
-        raise ValueError(f"`max_transforms` must a positive int (got {max_transforms})")
-
-    def duplicate(
-        transform: TransformType | None, length: int = max_transforms
-    ) -> Sequence[TransformType | None]:
-        return [transform] * length
-
-    if isinstance(transforms, Sequence):
-        if (num_transforms := len(transforms)) == 0:
-            transforms = duplicate(None)
-        elif num_transforms == 1:
-            transforms = duplicate(transforms[0])
-        elif num_transforms < max_transforms:
-            padding = duplicate(None, max_transforms - num_transforms)
-            transforms = [*transforms, *padding]
-        elif num_transforms > max_transforms:
-            transforms = transforms[:max_transforms]
-    else:
-        transforms = duplicate(transforms)
 
-    return tuple(transforms)
+DataType = TypeVar("DataType", bound=Sequence, covariant=True)
+TransformType = TypeVar("TransformType", bound=Callable)
 
 
-class MultiDomain(Generic[DataType, TransformType]):
+class _MultiDomainDataset(Dataset[DataType], Generic[DataType, TransformType]):
     def __init__(
         self,
         num_domains: int,
         transforms: TransformType | Sequence[TransformType | None] | None = None,
     ) -> None:
-        if not isinstance(num_domains, int) or num_domains < 1:
-            raise ValueError(f"`num_domains` must a positive int (got {num_domains})")
-
+        super().__init__()
+        self._transforms = self.validate_transforms(transforms, num_domains)
         self._num_domains = num_domains
-        self._transforms = unwrap_transforms(transforms, num_domains)
+
+    def __str__(self) -> LiteralString:
+        return self.__class__.__name__
 
     @property
     def num_domains(self) -> int:
         return self._num_domains
 
     @property
-    def transforms(self) -> tuple[TransformType | None, ...]:
+    def tranforms(self) -> tuple[TransformType | None, ...]:
         return self._transforms
 
+    @classmethod
+    def validate_transforms(
+        cls,
+        transforms: TransformType | Sequence[TransformType | None] | None,
+        max_transforms: int,
+    ) -> tuple[TransformType | None, ...]:
+        if not isinstance(max_transforms, int) or max_transforms < 1:
+            raise ValueError(
+                f"`max_transforms` must be a positive integer (got {max_transforms})"
+            )
+
+        def duplicate(
+            transform: TransformType | None, length: int = max_transforms
+        ) -> Sequence[TransformType | None]:
+            return [transform] * length
+
+        if isinstance(transforms, Sequence):
+            if (num_transforms := len(transforms)) == 0:
+                transforms = duplicate(None)
+            elif num_transforms == 1:
+                transforms = duplicate(transforms[0])
+            elif num_transforms < max_transforms:
+                padding = duplicate(None, max_transforms - num_transforms)
+                transforms = [*transforms, *padding]
+            elif num_transforms > max_transforms:
+                transforms = transforms[:max_transforms]
+        else:
+            transforms = duplicate(transforms)
+
+        return tuple(transforms)
+
+    @classmethod
+    def apply_transforms(
+        cls, transforms: Sequence[TransformType | None], domains: Sequence
+    ) -> Sequence:
+        if (num_domains := len(domains)) != (num_transforms := len(transforms)):
+            raise ValueError(
+                "`domains` and `transforms` must be the same length"
+                f" (got {num_domains}, {num_transforms})"
+            )
+
+        transformed = []
+        for transform, domain in zip(transforms, domains):
+            transformed.append(transform(domain) if callable(transform) else domain)
+        return transformed
 
-class MultiLabeled(Generic[LabelType, TransformType]):
+
+class MultiDomainDataset(_MultiDomainDataset[tuple[Tensor, ...], TensorFn]):
     def __init__(
         self,
-        num_labels: int,
-        label_transforms: TransformType | Sequence[TransformType | None] | None = None,
+        num_domains: int,
+        transforms: TensorFn | Sequence[TensorFn | None] | None = None,
     ) -> None:
-        if not isinstance(num_labels, int) or num_labels < 1:
-            raise ValueError(f"`num_labels` must a positive int (got {num_labels})")
+        super().__init__(num_domains, transforms)
 
-        self._num_labels = num_labels
-        self._label_transforms = unwrap_transforms(label_transforms, num_labels)
 
-    @property
-    def num_labels(self) -> int:
-        return self._num_labels
-
-    @property
-    def label_transforms(self) -> tuple[TransformType | None, ...]:
-        return self._label_transforms
+class DoubleDomainDataset(_MultiDomainDataset[tuple[Tensor, Tensor], TensorFn]):
+    def __init__(
+        self,
+        transforms: TensorFn | tuple[TensorFn | None, TensorFn | None] | None = None,
+    ) -> None:
+        super().__init__(2, transforms)
```

### Comparing `kaparoo_lightning-0.1.1/kaparoo_lightning/nn/models/gan.py` & `kaparoo_lightning-0.1.2/kaparoo_lightning/nn/models/gan.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,14 +20,10 @@
         self.automatic_optimization = False
 
     @classmethod
     def get_label(cls, pred: Tensor, as_real: bool = True) -> Tensor:
         return torch.ones_like(pred) if as_real else torch.zeros_like(pred)
 
     @classmethod
-    def adversarial_loss(
-        cls, pred: Tensor, as_real: bool = True, as_logit: bool = False
-    ) -> Tensor:
+    def adversarial_loss(cls, pred: Tensor, as_real: bool = True) -> Tensor:
         label = cls.get_label(pred, as_real)
-        if as_logit:
-            return F.binary_cross_entropy_with_logits(pred, label)
         return F.binary_cross_entropy(pred, label)
```

### Comparing `kaparoo_lightning-0.1.1/.gitignore` & `kaparoo_lightning-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.1/LICENSE` & `kaparoo_lightning-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.1/README.md` & `kaparoo_lightning-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.1/pyproject.toml` & `kaparoo_lightning-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.1/PKG-INFO` & `kaparoo_lightning-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaparoo-lightning
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for (personally) common and useful features for PyTorch Lightning.
 Project-URL: GitHub, https://www.github.com/kaparoo/lightning-package
 Author-email: Jaewoo Park <kaparoo2001@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jaewoo Park
```

