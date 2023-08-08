# Comparing `tmp/kaparoo_lightning-0.1.3.tar.gz` & `tmp/kaparoo_lightning-0.1.3.1.tar.gz`

## Comparing `kaparoo_lightning-0.1.3.tar` & `kaparoo_lightning-0.1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/kaparoo_lightning/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/kaparoo_lightning/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/kaparoo_lightning/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/kaparoo_lightning/common/__init__.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/kaparoo_lightning/common/spec.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/kaparoo_lightning/common/types.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/kaparoo_lightning/data/__init__.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/kaparoo_lightning/data/constants.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/kaparoo_lightning/data/dataloaders.py
--rw-r--r--   0        0        0    10340 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/kaparoo_lightning/data/datamodules.py
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/kaparoo_lightning/data/datasets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/kaparoo_lightning/nn/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/kaparoo_lightning/nn/models/__init__.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/kaparoo_lightning/nn/models/gan.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/LICENSE
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/README.md
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/kaparoo_lightning/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/kaparoo_lightning/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/kaparoo_lightning/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/kaparoo_lightning/common/__init__.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/kaparoo_lightning/common/spec.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/kaparoo_lightning/common/types.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/kaparoo_lightning/data/__init__.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/kaparoo_lightning/data/constants.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/kaparoo_lightning/data/dataloaders.py
+-rw-r--r--   0        0        0    10340 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/kaparoo_lightning/data/datamodules.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/kaparoo_lightning/data/datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/kaparoo_lightning/nn/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/kaparoo_lightning/nn/models/__init__.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/kaparoo_lightning/nn/models/gan.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/LICENSE
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/README.md
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 kaparoo_lightning-0.1.3.1/PKG-INFO
```

### Comparing `kaparoo_lightning-0.1.3/kaparoo_lightning/common/spec.py` & `kaparoo_lightning-0.1.3.1/kaparoo_lightning/common/spec.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.3/kaparoo_lightning/data/__init__.py` & `kaparoo_lightning-0.1.3.1/kaparoo_lightning/data/__init__.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.3/kaparoo_lightning/data/constants.py` & `kaparoo_lightning-0.1.3.1/kaparoo_lightning/data/constants.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.3/kaparoo_lightning/data/dataloaders.py` & `kaparoo_lightning-0.1.3.1/kaparoo_lightning/data/dataloaders.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.3/kaparoo_lightning/data/datamodules.py` & `kaparoo_lightning-0.1.3.1/kaparoo_lightning/data/datamodules.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.3/kaparoo_lightning/data/datasets.py` & `kaparoo_lightning-0.1.3.1/kaparoo_lightning/data/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from __future__ import annotations
 
 __all__ = ("MultiDomainDataset", "DoubleDomainDataset")
 
 from collections.abc import Callable, Sequence
 from typing import TYPE_CHECKING, Generic, TypeVar
 
+from torch import Tensor
 from torch.utils.data import Dataset
 
 from kaparoo_lightning.common.types import TensorFn
 
 if TYPE_CHECKING:
-    from torch import Tensor
     from typing_extensions import LiteralString
 
 
 DataType = TypeVar("DataType", bound=Sequence, covariant=True)
 TransformType = TypeVar("TransformType", bound=Callable)
```

### Comparing `kaparoo_lightning-0.1.3/kaparoo_lightning/nn/models/gan.py` & `kaparoo_lightning-0.1.3.1/kaparoo_lightning/nn/models/gan.py`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.3/.gitignore` & `kaparoo_lightning-0.1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.3/LICENSE` & `kaparoo_lightning-0.1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.3/README.md` & `kaparoo_lightning-0.1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.3/pyproject.toml` & `kaparoo_lightning-0.1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kaparoo_lightning-0.1.3/PKG-INFO` & `kaparoo_lightning-0.1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaparoo-lightning
-Version: 0.1.3
+Version: 0.1.3.1
 Summary: A Python package for (personally) common and useful features for PyTorch Lightning.
 Project-URL: GitHub, https://www.github.com/kaparoo/lightning-package
 Author-email: Jaewoo Park <kaparoo2001@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jaewoo Park
```

