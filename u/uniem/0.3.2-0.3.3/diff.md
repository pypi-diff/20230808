# Comparing `tmp/uniem-0.3.2.tar.gz` & `tmp/uniem-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniem-0.3.2.tar", max compression
+gzip compressed data, was "uniem-0.3.3.tar", max compression
```

## Comparing `uniem-0.3.2.tar` & `uniem-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-07-20 03:53:40.653015 uniem-0.3.2/LICENSE
--rw-r--r--   0        0        0     6369 2023-07-20 03:53:40.653015 uniem-0.3.2/README.md
--rw-r--r--   0        0        0      813 2023-07-20 03:53:40.665015 uniem-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       92 2023-07-20 03:53:40.761014 uniem-0.3.2/uniem/__init__.py
--rw-r--r--   0        0        0     7166 2023-07-20 03:53:40.761014 uniem-0.3.2/uniem/criteria.py
--rw-r--r--   0        0        0    12450 2023-07-20 03:53:40.761014 uniem-0.3.2/uniem/data.py
--rw-r--r--   0        0        0     1109 2023-07-20 03:53:40.761014 uniem-0.3.2/uniem/data_structures.py
--rw-r--r--   0        0        0    14419 2023-07-20 03:53:40.761014 uniem-0.3.2/uniem/finetuner.py
--rw-r--r--   0        0        0        0 2023-07-20 03:53:40.761014 uniem-0.3.2/uniem/integration/__init__.py
--rw-r--r--   0        0        0     1339 2023-07-20 03:53:40.761014 uniem-0.3.2/uniem/integration/sentence_transformers_wrapper.py
--rw-r--r--   0        0        0    13360 2023-07-20 03:53:40.765014 uniem-0.3.2/uniem/model.py
--rw-r--r--   0        0        0     6478 2023-07-20 03:53:40.765014 uniem-0.3.2/uniem/trainer.py
--rw-r--r--   0        0        0     3678 2023-07-20 03:53:40.765014 uniem-0.3.2/uniem/training_strategy.py
--rw-r--r--   0        0        0      658 2023-07-20 03:53:40.765014 uniem-0.3.2/uniem/types.py
--rw-r--r--   0        0        0     6193 2023-07-20 03:53:40.765014 uniem-0.3.2/uniem/utils.py
--rw-r--r--   0        0        0       22 2023-07-20 03:53:40.765014 uniem-0.3.2/uniem/version.py
--rw-r--r--   0        0        0     7004 1970-01-01 00:00:00.000000 uniem-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-08 08:02:28.836841 uniem-0.3.3/LICENSE
+-rw-r--r--   0        0        0     6369 2023-08-08 08:02:28.836841 uniem-0.3.3/README.md
+-rw-r--r--   0        0        0      813 2023-08-08 08:02:28.848842 uniem-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0       92 2023-08-08 08:02:28.952844 uniem-0.3.3/uniem/__init__.py
+-rw-r--r--   0        0        0     7166 2023-08-08 08:02:28.952844 uniem-0.3.3/uniem/criteria.py
+-rw-r--r--   0        0        0    12450 2023-08-08 08:02:28.952844 uniem-0.3.3/uniem/data.py
+-rw-r--r--   0        0        0     1109 2023-08-08 08:02:28.952844 uniem-0.3.3/uniem/data_structures.py
+-rw-r--r--   0        0        0    14592 2023-08-08 08:02:28.952844 uniem-0.3.3/uniem/finetuner.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:02:28.952844 uniem-0.3.3/uniem/integration/__init__.py
+-rw-r--r--   0        0        0     1339 2023-08-08 08:02:28.952844 uniem-0.3.3/uniem/integration/sentence_transformers_wrapper.py
+-rw-r--r--   0        0        0    13360 2023-08-08 08:02:28.952844 uniem-0.3.3/uniem/model.py
+-rw-r--r--   0        0        0     8055 2023-08-08 08:02:28.952844 uniem-0.3.3/uniem/trainer.py
+-rw-r--r--   0        0        0     3678 2023-08-08 08:02:28.952844 uniem-0.3.3/uniem/training_strategy.py
+-rw-r--r--   0        0        0      658 2023-08-08 08:02:28.952844 uniem-0.3.3/uniem/types.py
+-rw-r--r--   0        0        0     6193 2023-08-08 08:02:28.952844 uniem-0.3.3/uniem/utils.py
+-rw-r--r--   0        0        0       22 2023-08-08 08:02:28.952844 uniem-0.3.3/uniem/version.py
+-rw-r--r--   0        0        0     7004 1970-01-01 00:00:00.000000 uniem-0.3.3/PKG-INFO
```

### Comparing `uniem-0.3.2/LICENSE` & `uniem-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uniem-0.3.2/README.md` & `uniem-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `uniem-0.3.2/pyproject.toml` & `uniem-0.3.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uniem"
-version = "0.3.2"
+version = "0.3.3"
 description = "unified embedding model"
 authors = ["wangyuxin <wangyuxin@mokahr.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `uniem-0.3.2/uniem/criteria.py` & `uniem-0.3.3/uniem/criteria.py`

 * *Files identical despite different names*

### Comparing `uniem-0.3.2/uniem/data.py` & `uniem-0.3.3/uniem/data.py`

 * *Files identical despite different names*

### Comparing `uniem-0.3.2/uniem/data_structures.py` & `uniem-0.3.3/uniem/data_structures.py`

 * *Files identical despite different names*

### Comparing `uniem-0.3.2/uniem/finetuner.py` & `uniem-0.3.3/uniem/finetuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import os
 from enum import Enum
 from pathlib import Path
-from typing import Callable, Iterable, Sequence, Sized, cast
+from typing import Any, Callable, Iterable, Sequence, Sized, cast
 
 import torch
 from accelerate import Accelerator
 from accelerate.tracking import GeneralTracker
 from accelerate.utils import LoggerType, ProjectConfiguration, set_seed
 from datasets import Dataset as HFDataset
 from datasets import IterableDataset as HFIterableDataset
@@ -231,18 +231,20 @@
         num_warmup_steps: float | None = None,
         # Data
         batch_size: int = 256,
         max_length: int = 512,
         drop_last: bool = False,
         shuffle: bool = False,
         num_workers: int = 0,
-        # Trainer
-        epochs: int = 3,
+        # Aceelerator
         mixed_precision: MixedPrecisionType = MixedPrecisionType.no,
         gradient_accumulation_steps: int = 1,
+        accelerator_kwargs: dict[str, Any] | None = None,
+        # Trainer
+        epochs: int = 3,
         save_on_epoch_end: bool = False,
         num_max_checkpoints: int = 1,
         log_with: str | LoggerType | GeneralTracker | list[str | LoggerType | GeneralTracker] | None = None,
         seed: int = 42,
         epoch_end_callbacks: Sequence[Callable[[Trainer], None]] | None = None,
         output_dir: Path | str | None = None,
     ):
@@ -253,19 +255,21 @@
 
         output_dir = Path(output_dir) if output_dir is not None else Path('finetuned-model')
         project_config = ProjectConfiguration(
             project_dir=str(output_dir),
             automatic_checkpoint_naming=True,
             total_limit=num_max_checkpoints,
         )
+        accelerator_kwargs = accelerator_kwargs or {}
         accelerator = Accelerator(
             mixed_precision=mixed_precision.value,
             gradient_accumulation_steps=gradient_accumulation_steps,
             project_config=project_config,
             log_with=log_with,
+            **accelerator_kwargs,
         )
         self.accelerator = accelerator
         accelerator.init_trackers('uniem')
 
         set_seed(seed)
         accelerator.print(f'Batch size: {batch_size}')
         accelerator.print(f'Start with seed: {seed}')
```

### Comparing `uniem-0.3.2/uniem/integration/sentence_transformers_wrapper.py` & `uniem-0.3.3/uniem/integration/sentence_transformers_wrapper.py`

 * *Files identical despite different names*

### Comparing `uniem-0.3.2/uniem/model.py` & `uniem-0.3.3/uniem/model.py`

 * *Files identical despite different names*

### Comparing `uniem-0.3.2/uniem/trainer.py` & `uniem-0.3.3/uniem/trainer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from __future__ import annotations
 
+import logging
+import os
+import re
+import shutil
 from typing import Any, Callable, Sequence, Sized
 
 import torch
 from accelerate import Accelerator
 from torch.optim import Optimizer
 from torch.utils.data import DataLoader
 from tqdm.auto import tqdm
 
 try:
     from torch.optim.lr_scheduler import LRScheduler
 except ImportError:
     from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 
+logger = logging.getLogger(__name__)
+
 
 class Trainer:
     def __init__(
         self,
         *,
         model: torch.nn.Module,
         train_dataloader: DataLoader,
@@ -85,15 +91,15 @@
                     self.validation_loss_tracker,
                 )
                 validation_metrics = self.add_prefix({'loss': validation_loss}, 'validation')
                 self.accelerator.print(f'Epoch {current_epoch} Validation loss: {validation_loss:.4f}')
                 self.accelerator.log(validation_metrics, step=current_epoch)
 
             if self.save_on_epoch_end:
-                self.accelerator.save_state()
+                self.accelerator.save_state(self.get_checkpoint_dir())
 
             if self.epoch_end_callbacks:
                 for callback in self.epoch_end_callbacks:
                     callback(self)
 
         self.accelerator.end_training()
 
@@ -101,14 +107,42 @@
         self.accelerator.log(metrics, step=step)
         self.progress_bar.show_metrics(metrics)
 
     @staticmethod
     def add_prefix(values: dict[str, Any], prefix: str):
         return {f'{prefix}/{k}': v for k, v in values.items()}
 
+    def get_checkpoint_dir(self):
+        # COPY FROM accelerator to fix Checkpoint bug
+        self.accelerator.project_configuration.automatic_checkpoint_naming = False
+        output_dir = os.path.join(self.accelerator.project_dir, 'checkpoints')
+        if self.accelerator.is_local_main_process:
+            os.makedirs(output_dir, exist_ok=True)
+            folders = [os.path.join(output_dir, folder) for folder in os.listdir(output_dir)]
+            if self.accelerator.project_configuration.total_limit is not None and (
+                len(folders) + 1 > self.accelerator.project_configuration.total_limit
+            ):
+
+                def _inner(folder):
+                    return list(map(int, re.findall(r'[\/]?([0-9]+)(?=[^\/]*$)', folder)))[0]
+
+                folders.sort(key=_inner)
+                logger.warning(
+                    f'Deleting {len(folders) + 1 - self.accelerator.project_configuration.total_limit}'
+                    'checkpoints to make room for new checkpoint.'
+                )
+                for folder in folders[: len(folders) + 1 - self.accelerator.project_configuration.total_limit]:
+                    shutil.rmtree(folder)
+
+        output_dir = os.path.join(output_dir, f'checkpoint_{self.accelerator.save_iteration}')
+        if self.accelerator.is_local_main_process:
+            os.makedirs(output_dir, exist_ok=True)
+        logger.info(f'Saving current state to {output_dir}')
+        return output_dir
+
 
 def evaluate(
     model: torch.nn.Module,
     dataloader: DataLoader,
     loss_tracker: LossTracker | None = None,
 ):
     model = model.eval()
```

### Comparing `uniem-0.3.2/uniem/training_strategy.py` & `uniem-0.3.3/uniem/training_strategy.py`

 * *Files identical despite different names*

### Comparing `uniem-0.3.2/uniem/types.py` & `uniem-0.3.3/uniem/types.py`

 * *Files identical despite different names*

### Comparing `uniem-0.3.2/uniem/utils.py` & `uniem-0.3.3/uniem/utils.py`

 * *Files identical despite different names*

### Comparing `uniem-0.3.2/PKG-INFO` & `uniem-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniem
-Version: 0.3.2
+Version: 0.3.3
 Summary: unified embedding model
 License: MIT
 Author: wangyuxin
 Author-email: wangyuxin@mokahr.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

