# Comparing `tmp/lightning-graphcore-0.1.0rc3.tar.gz` & `tmp/lightning-graphcore-0.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-graphcore-0.1.0rc3.tar", last modified: Wed May 24 18:22:16 2023, max compression
+gzip compressed data, was "lightning-graphcore-0.1.0rc4.tar", last modified: Tue Aug  8 07:29:38 2023, max compression
```

## Comparing `lightning-graphcore-0.1.0rc3.tar` & `lightning-graphcore-0.1.0rc4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:16.314093 lightning-graphcore-0.1.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-24 18:22:02.000000 lightning-graphcore-0.1.0rc3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-05-24 18:22:02.000000 lightning-graphcore-0.1.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-24 18:22:02.000000 lightning-graphcore-0.1.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-24 18:22:16.314093 lightning-graphcore-0.1.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-24 18:22:02.000000 lightning-graphcore-0.1.0rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 18:22:02.000000 lightning-graphcore-0.1.0rc3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 18:22:16.314093 lightning-graphcore-0.1.0rc3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4162 2023-05-24 18:22:02.000000 lightning-graphcore-0.1.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:16.310093 lightning-graphcore-0.1.0rc3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:16.314093 lightning-graphcore-0.1.0rc3/src/lightning_graphcore/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-24 18:22:02.000000 lightning-graphcore-0.1.0rc3/src/lightning_graphcore/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-24 18:22:02.000000 lightning-graphcore-0.1.0rc3/src/lightning_graphcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-24 18:22:02.000000 lightning-graphcore-0.1.0rc3/src/lightning_graphcore/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-24 18:22:02.000000 lightning-graphcore-0.1.0rc3/src/lightning_graphcore/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-05-24 18:22:02.000000 lightning-graphcore-0.1.0rc3/src/lightning_graphcore/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-24 18:22:02.000000 lightning-graphcore-0.1.0rc3/src/lightning_graphcore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:16.314093 lightning-graphcore-0.1.0rc3/src/lightning_graphcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-24 18:22:16.000000 lightning-graphcore-0.1.0rc3/src/lightning_graphcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-24 18:22:16.000000 lightning-graphcore-0.1.0rc3/src/lightning_graphcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:22:16.000000 lightning-graphcore-0.1.0rc3/src/lightning_graphcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:22:16.000000 lightning-graphcore-0.1.0rc3/src/lightning_graphcore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-24 18:22:16.000000 lightning-graphcore-0.1.0rc3/src/lightning_graphcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 18:22:16.000000 lightning-graphcore-0.1.0rc3/src/lightning_graphcore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:29:38.371776 lightning-graphcore-0.1.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-08 07:29:27.000000 lightning-graphcore-0.1.0rc4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-08-08 07:29:27.000000 lightning-graphcore-0.1.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-08 07:29:27.000000 lightning-graphcore-0.1.0rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-08-08 07:29:38.371776 lightning-graphcore-0.1.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-08-08 07:29:27.000000 lightning-graphcore-0.1.0rc4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-08 07:29:27.000000 lightning-graphcore-0.1.0rc4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 07:29:38.371776 lightning-graphcore-0.1.0rc4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4162 2023-08-08 07:29:27.000000 lightning-graphcore-0.1.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:29:38.367776 lightning-graphcore-0.1.0rc4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:29:38.371776 lightning-graphcore-0.1.0rc4/src/lightning_graphcore/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-08 07:29:27.000000 lightning-graphcore-0.1.0rc4/src/lightning_graphcore/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-08 07:29:27.000000 lightning-graphcore-0.1.0rc4/src/lightning_graphcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-08 07:29:27.000000 lightning-graphcore-0.1.0rc4/src/lightning_graphcore/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-08-08 07:29:27.000000 lightning-graphcore-0.1.0rc4/src/lightning_graphcore/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-08-08 07:29:27.000000 lightning-graphcore-0.1.0rc4/src/lightning_graphcore/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-08-08 07:29:27.000000 lightning-graphcore-0.1.0rc4/src/lightning_graphcore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:29:38.371776 lightning-graphcore-0.1.0rc4/src/lightning_graphcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-08-08 07:29:38.000000 lightning-graphcore-0.1.0rc4/src/lightning_graphcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-08 07:29:38.000000 lightning-graphcore-0.1.0rc4/src/lightning_graphcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:29:38.000000 lightning-graphcore-0.1.0rc4/src/lightning_graphcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:29:38.000000 lightning-graphcore-0.1.0rc4/src/lightning_graphcore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-08 07:29:38.000000 lightning-graphcore-0.1.0rc4/src/lightning_graphcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-08 07:29:38.000000 lightning-graphcore-0.1.0rc4/src/lightning_graphcore.egg-info/top_level.txt
```

### Comparing `lightning-graphcore-0.1.0rc3/LICENSE` & `lightning-graphcore-0.1.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc3/MANIFEST.in` & `lightning-graphcore-0.1.0rc4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc3/PKG-INFO` & `lightning-graphcore-0.1.0rc4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-graphcore
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: Lightning support for GraphCore accelerators
 Home-page: https://github.com/Lightning-AI/lightning-graphcore
 Download-URL: https://github.com/Lightning-AI/lightning-graphcore
 Author: Lightning-AI et al.
 Author-email: name@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-graphcore/issues
@@ -23,14 +23,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: typing
+Provides-Extra: lightning
+Provides-Extra: pytorch-lightning
 License-File: LICENSE
 
 # Lightning ⚡ GraphCore
 
 **Audience:** Users looking to save money and run large models faster using single or multiple IPU devices.
 
 [![lightning](https://img.shields.io/badge/-Lightning_2.0+-792ee5?logo=pytorchlightning&logoColor=white)](https://lightning.ai/)
@@ -50,15 +53,15 @@
 See the [Graphcore Glossary](https://docs.graphcore.ai/projects/graphcore-glossary/) for the definitions of other IPU-specific terminology.
 
 ______________________________________________________________________
 
 ## Installation
 
 ```bash
-pip install -U lightning-graphcore
+pip install -U lightning-graphcore[lightning]
 ```
 
 ## Run on IPU
 
 To enable PyTorch Lightning to utilize the IPU accelerator, simply provide `accelerator="ipu"` parameter to the Trainer class.
 
 To use multiple IPUs set the devices to a number that is a power of 2 (i.e: 2, 4, 8, 16, ...)
```

### Comparing `lightning-graphcore-0.1.0rc3/README.md` & `lightning-graphcore-0.1.0rc4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 See the [Graphcore Glossary](https://docs.graphcore.ai/projects/graphcore-glossary/) for the definitions of other IPU-specific terminology.
 
 ______________________________________________________________________
 
 ## Installation
 
 ```bash
-pip install -U lightning-graphcore
+pip install -U lightning-graphcore[lightning]
 ```
 
 ## Run on IPU
 
 To enable PyTorch Lightning to utilize the IPU accelerator, simply provide `accelerator="ipu"` parameter to the Trainer class.
 
 To use multiple IPUs set the devices to a number that is a power of 2 (i.e: 2, 4, 8, 16, ...)
```

### Comparing `lightning-graphcore-0.1.0rc3/setup.py` & `lightning-graphcore-0.1.0rc4/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc3/src/lightning_graphcore/accelerator.py` & `lightning-graphcore-0.1.0rc4/src/lightning_graphcore/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc3/src/lightning_graphcore/precision.py` & `lightning-graphcore-0.1.0rc4/src/lightning_graphcore/precision.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Any, Callable, Literal, Union, cast
+from typing import Any, Callable, List, Literal, Tuple, Union, cast
 
 from lightning_utilities.core.imports import package_available
 from torch import Tensor
+from torch.nn import Module
 from torch.optim import LBFGS, Optimizer
 from typing_extensions import get_args
 
 if package_available("lightning"):
     from lightning.fabric.utilities.types import Optimizable
     from lightning.pytorch import LightningModule
     from lightning.pytorch.plugins.precision.precision_plugin import PrecisionPlugin
@@ -35,36 +36,47 @@
     from pytorch_lightning.utilities.model_helpers import is_overridden
     from pytorch_lightning.utilities.rank_zero import WarningCache
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 
 warning_cache = WarningCache()
 
-_PRECISION_INPUT = Literal["32-true", "16-mixed"]
+_PRECISION_INPUT = Literal["32-true", "16-mixed", "16-true"]
 
 
 class IPUPrecision(PrecisionPlugin):
     """Precision plugin for IPU integration.
 
     .. warning::  This is an :ref:`experimental <versioning:Experimental API>` feature.
 
     Raises:
         ValueError:
-            If the precision is neither 16-mixed nor 32-true.
+            If the precision is neither 16-true, 16-mixed nor 32-true.
     """
 
-    def __init__(self, precision: Literal["32-true", "16-mixed"]) -> None:
+    def __init__(self, precision: Literal["32-true", "16-mixed", "16-true"]) -> None:
         supported_precision = get_args(_PRECISION_INPUT)
         if precision not in supported_precision:
             raise ValueError(
                 f"`Trainer(accelerator='ipu', precision={precision!r})` is not supported."
                 f" `precision` must be one of: {supported_precision}."
             )
         self.precision = cast(_PRECISION_INPUT, str(precision))
 
+    def convert_module(self, module: Module) -> Module:
+        if self.precision == "16-true":
+            module = module.half()
+        return super().convert_module(module)
+
+    def connect(
+        self, model: Module, optimizers: List[Optimizer], lr_schedulers: List[Any]
+    ) -> Tuple[Module, List[Optimizer], List[Any]]:
+        model = self.convert_module(model)
+        return super().connect(model, optimizers, lr_schedulers)
+
     def backward(
         self,
         tensor: Tensor,
         model: LightningModule,
         *args: Any,
         **kwargs: Any,
     ) -> None:
```

### Comparing `lightning-graphcore-0.1.0rc3/src/lightning_graphcore/strategy.py` & `lightning-graphcore-0.1.0rc4/src/lightning_graphcore/strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     from lightning.fabric.plugins import CheckpointIO, ClusterEnvironment
     from lightning.fabric.utilities.cloud_io import get_filesystem
     from lightning.pytorch import Trainer
     from lightning.pytorch.accelerators import Accelerator
     from lightning.pytorch.plugins.precision import PrecisionPlugin
     from lightning.pytorch.strategies.parallel import ParallelStrategy
     from lightning.pytorch.strategies.strategy import TBroadcast
-    from lightning.pytorch.strategies.utils import _fp_to_half
     from lightning.pytorch.trainer.states import RunningStage, TrainerFn
     from lightning.pytorch.utilities import rank_zero_warn
     from lightning.pytorch.utilities.data import _get_dataloader_init_args_and_kwargs, _reinstantiate_wrapped_cls
     from lightning.pytorch.utilities.exceptions import MisconfigurationException
     from lightning.pytorch.utilities.model_helpers import is_overridden
     from lightning.pytorch.utilities.types import STEP_OUTPUT
 elif package_available("pytorch_lightning"):
@@ -42,26 +41,25 @@
     from lightning_fabric.plugins import CheckpointIO, ClusterEnvironment
     from lightning_fabric.utilities.cloud_io import get_filesystem
     from pytorch_lightning import Trainer
     from pytorch_lightning.accelerators import Accelerator
     from pytorch_lightning.plugins.precision import PrecisionPlugin
     from pytorch_lightning.strategies.parallel import ParallelStrategy
     from pytorch_lightning.strategies.strategy import TBroadcast
-    from pytorch_lightning.strategies.utils import _fp_to_half
     from pytorch_lightning.trainer.states import RunningStage, TrainerFn
     from pytorch_lightning.utilities import rank_zero_warn
     from pytorch_lightning.utilities.data import _get_dataloader_init_args_and_kwargs, _reinstantiate_wrapped_cls
     from pytorch_lightning.utilities.exceptions import MisconfigurationException
     from pytorch_lightning.utilities.model_helpers import is_overridden
     from pytorch_lightning.utilities.types import STEP_OUTPUT
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 
 from lightning_graphcore.accelerator import _IPU_AVAILABLE, _POPTORCH_AVAILABLE
-from lightning_graphcore.utils import _LightningModuleWrapperBase
+from lightning_graphcore.utils import _fp_to_half, _LightningModuleWrapperBase
 
 if _POPTORCH_AVAILABLE:
     import poptorch
 else:
     poptorch = None
 
 
@@ -229,18 +227,15 @@
             # the user is returning the `poptorch.DataLoader` directly, don't change anything.
             return dataloader
 
         dl_args, dl_kwargs = _get_dataloader_init_args_and_kwargs(
             dataloader, sampler, mode, self.replication_factor > 1
         )
         opts = self.training_opts if mode == RunningStage.TRAINING else self.inference_opts
-        dataloader = _reinstantiate_wrapped_cls(
-            dataloader, opts, *dl_args, explicit_cls=poptorch.DataLoader, **dl_kwargs
-        )
-        return dataloader
+        return _reinstantiate_wrapped_cls(dataloader, opts, *dl_args, explicit_cls=poptorch.DataLoader, **dl_kwargs)
 
     @property
     def _n_replicate(self) -> int:
         assert self.lightning_module is not None
         opts = self.training_opts if self.lightning_module.training else self.inference_opts
         accumulate_grad_batches = opts.Training.gradient_accumulation
         device_iterations = opts.device_iterations
```

### Comparing `lightning-graphcore-0.1.0rc3/src/lightning_graphcore/utils.py` & `lightning-graphcore-0.1.0rc4/src/lightning_graphcore/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Any, Union
+from typing import Any, Literal, Union
 
 import torch
 from lightning_utilities.core.imports import package_available
+from torch import Tensor
 
 if package_available("lightning"):
     from lightning.fabric.utilities.device_dtype_mixin import _DeviceDtypeModuleMixin
     from lightning.pytorch import LightningModule
     from lightning.pytorch.overrides.base import _LightningPrecisionModuleWrapperBase
 elif package_available("pytorch_lightning"):
     from lightning_fabric.utilities.device_dtype_mixin import _DeviceDtypeModuleMixin
@@ -62,7 +63,27 @@
             if trainer.testing:
                 return self._forward_module.test_step(*inputs, **kwargs)
             if trainer.sanity_checking or trainer.validating:
                 return self._forward_module.validation_step(*inputs, **kwargs)
             if trainer.predicting:
                 return self._forward_module.predict_step(*inputs, **kwargs)
         return self._forward_module(*inputs, **kwargs)
+
+
+def _fp_to_half(
+    tensor: Tensor,
+    precision: Literal[
+        "64-true",
+        "32-true",
+        "16-mixed",
+        "bf16-mixed",
+    ],
+) -> Tensor:
+    if str(precision) == "16-mixed":
+        return _convert_fp_tensor(tensor, torch.half)
+    if precision == "bf16-mixed":
+        return _convert_fp_tensor(tensor, torch.bfloat16)
+    return tensor
+
+
+def _convert_fp_tensor(tensor: Tensor, dst_type: Union[str, torch.dtype]) -> Tensor:
+    return tensor.to(dst_type) if torch.is_floating_point(tensor) else tensor
```

### Comparing `lightning-graphcore-0.1.0rc3/src/lightning_graphcore.egg-info/PKG-INFO` & `lightning-graphcore-0.1.0rc4/src/lightning_graphcore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-graphcore
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: Lightning support for GraphCore accelerators
 Home-page: https://github.com/Lightning-AI/lightning-graphcore
 Download-URL: https://github.com/Lightning-AI/lightning-graphcore
 Author: Lightning-AI et al.
 Author-email: name@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-graphcore/issues
@@ -23,14 +23,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: typing
+Provides-Extra: lightning
+Provides-Extra: pytorch-lightning
 License-File: LICENSE
 
 # Lightning ⚡ GraphCore
 
 **Audience:** Users looking to save money and run large models faster using single or multiple IPU devices.
 
 [![lightning](https://img.shields.io/badge/-Lightning_2.0+-792ee5?logo=pytorchlightning&logoColor=white)](https://lightning.ai/)
@@ -50,15 +53,15 @@
 See the [Graphcore Glossary](https://docs.graphcore.ai/projects/graphcore-glossary/) for the definitions of other IPU-specific terminology.
 
 ______________________________________________________________________
 
 ## Installation
 
 ```bash
-pip install -U lightning-graphcore
+pip install -U lightning-graphcore[lightning]
 ```
 
 ## Run on IPU
 
 To enable PyTorch Lightning to utilize the IPU accelerator, simply provide `accelerator="ipu"` parameter to the Trainer class.
 
 To use multiple IPUs set the devices to a number that is a power of 2 (i.e: 2, 4, 8, 16, ...)
```

### Comparing `lightning-graphcore-0.1.0rc3/src/lightning_graphcore.egg-info/SOURCES.txt` & `lightning-graphcore-0.1.0rc4/src/lightning_graphcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

