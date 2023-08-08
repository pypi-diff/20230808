# Comparing `tmp/opendataval-1.0.0.tar.gz` & `tmp/opendataval-1.1.0.tar.gz`

## Comparing `opendataval-1.0.0.tar` & `opendataval-1.1.0.tar`

### file list

```diff
@@ -1,56 +1,61 @@
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/__init__.py
--rw-r--r--   0        0        0     9859 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/__main__.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/metrics.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/presets.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/util.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataloader/__init__.py
--rw-r--r--   0        0        0    18712 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataloader/fetcher.py
--rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataloader/noisify.py
--rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataloader/register.py
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataloader/util.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataloader/datasets/__init__.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataloader/datasets/challenge.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataloader/datasets/cleanlab.py
--rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataloader/datasets/datasets.py
--rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataloader/datasets/imagesets.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataloader/datasets/nlpsets.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/__init__.py
--rw-r--r--   0        0        0    10108 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/api.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/ame/__init__.py
--rw-r--r--   0        0        0     6662 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/ame/ame.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/dvrl/__init__.py
--rw-r--r--   0        0        0    16699 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/dvrl/dvrl.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/influence/__init__.py
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/influence/influence.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/knnshap/__init__.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/knnshap/knnshap.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/margcontrib/__init__.py
--rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/margcontrib/banzhaf.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/margcontrib/betashap.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/margcontrib/datashap.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/margcontrib/loo.py
--rw-r--r--   0        0        0    11187 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/margcontrib/shap.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/oob/__init__.py
--rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/oob/oob.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/random/__init__.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/dataval/random/random.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/experiment/__init__.py
--rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/experiment/api.py
--rw-r--r--   0        0        0    14509 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/experiment/exper_methods.py
--rw-r--r--   0        0        0     6020 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/model/__init__.py
--rw-r--r--   0        0        0    18049 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/model/api.py
--rw-r--r--   0        0        0     9344 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/model/bert.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/model/lenet.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/model/logistic_regression.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 opendataval-1.0.0/opendataval/model/mlp.py
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 opendataval-1.0.0/test/test_dataevaluator.py
--rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 opendataval-1.0.0/test/test_dataloader.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 opendataval-1.0.0/test/test_dataval.py
--rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 opendataval-1.0.0/test/test_exper_methods.py
--rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 opendataval-1.0.0/test/test_experiment.py
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 opendataval-1.0.0/test/test_register.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 opendataval-1.0.0/.gitignore
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 opendataval-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0    13236 2020-02-02 00:00:00.000000 opendataval-1.0.0/README.md
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 opendataval-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    14797 2020-02-02 00:00:00.000000 opendataval-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/__init__.py
+-rw-r--r--   0        0        0     9859 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/__main__.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/metrics.py
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/util.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataloader/__init__.py
+-rw-r--r--   0        0        0    20984 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataloader/fetcher.py
+-rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataloader/noisify.py
+-rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataloader/register.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataloader/util.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataloader/datasets/__init__.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataloader/datasets/challenge.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataloader/datasets/cleanlab.py
+-rw-r--r--   0        0        0     8533 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataloader/datasets/datasets.py
+-rw-r--r--   0        0        0     8866 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataloader/datasets/imagesets.py
+-rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataloader/datasets/nlpsets.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/__init__.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/api.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/ame/__init__.py
+-rw-r--r--   0        0        0     6725 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/ame/ame.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/dvrl/__init__.py
+-rw-r--r--   0        0        0    16747 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/dvrl/dvrl.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/influence/__init__.py
+-rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/influence/influence.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/knnshap/__init__.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/knnshap/knnshap.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/lava/__init__.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/lava/lava.py
+-rw-r--r--   0        0        0    16822 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/lava/otdd.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/margcontrib/__init__.py
+-rw-r--r--   0        0        0     7304 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/margcontrib/banzhaf.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/margcontrib/betashap.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/margcontrib/datashap.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/margcontrib/loo.py
+-rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/margcontrib/shap.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/oob/__init__.py
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/oob/oob.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/random/__init__.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/random/random.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/volume/__init__.py
+-rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/dataval/volume/rvs.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/experiment/__init__.py
+-rw-r--r--   0        0        0    16220 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/experiment/api.py
+-rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/experiment/exper_methods.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/experiment/util.py
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/model/__init__.py
+-rw-r--r--   0        0        0    18168 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/model/api.py
+-rw-r--r--   0        0        0     9388 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/model/bert.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/model/lenet.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/model/logistic_regression.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 opendataval-1.1.0/opendataval/model/mlp.py
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 opendataval-1.1.0/test/test_dataevaluator.py
+-rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 opendataval-1.1.0/test/test_dataloader.py
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 opendataval-1.1.0/test/test_dataval.py
+-rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 opendataval-1.1.0/test/test_exper_methods.py
+-rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 opendataval-1.1.0/test/test_experiment.py
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 opendataval-1.1.0/test/test_register.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 opendataval-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 opendataval-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0    13327 2020-02-02 00:00:00.000000 opendataval-1.1.0/README.md
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 opendataval-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    14915 2020-02-02 00:00:00.000000 opendataval-1.1.0/PKG-INFO
```

### Comparing `opendataval-1.0.0/opendataval/__init__.py` & `opendataval-1.1.0/opendataval/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,9 +30,9 @@
 .. autosummary::
     :toctree: generated/
 
     ~opendataval.util.set_random_state
     ~opendataval.util.load_mediator_output
     __version__
 """
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 """Version release number."""
```

### Comparing `opendataval-1.0.0/opendataval/__main__.py` & `opendataval-1.1.0/opendataval/__main__.py`

 * *Files identical despite different names*

### Comparing `opendataval-1.0.0/opendataval/metrics.py` & `opendataval-1.1.0/opendataval/metrics.py`

 * *Files identical despite different names*

### Comparing `opendataval-1.0.0/opendataval/util.py` & `opendataval-1.1.0/opendataval/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import itertools
 import time
 from datetime import timedelta
 from enum import Enum
 from functools import update_wrapper
-from typing import Callable, Generic, TypeVar
+from typing import Callable, Generic, Optional, TypeVar
 
 import numpy as np
 import pandas as pd
 import torch
 import tqdm
 from numpy.random import RandomState
 from sklearn.utils import check_random_state
 
 
 def load_mediator_output(filepath: str):
     """Loads output of Pandas DataFrame csv generated by ExperimentMediator."""
     return pd.read_csv(filepath, index_col=[0])
 
 
-def set_random_state(random_state: RandomState = None) -> RandomState:
+def set_random_state(random_state: Optional[RandomState] = None) -> RandomState:
     """Set the random state of opendataval, useful for recreation of results."""
     print(f"Initial random seed is: {random_state}.")
     torch.manual_seed(check_random_state(random_state).tomaxint())
     random_state = check_random_state(random_state)
     return random_state
 
 
@@ -42,15 +42,15 @@
         return name.lower()
 
 
 X, Y = TypeVar("X"), TypeVar("Y")
 
 
 class wrapper(str, Generic[X, Y]):
-    def __new__(cls, function: Callable[[X, ...], Y], name: str = None):
+    def __new__(cls, function: Callable[[X, ...], Y], name: Optional[str] = None):
         """Wrapper is a walks and talks like a str but can be called with the func."""
         out = str.__new__(cls, function.__name__ if name is None else name)
         out.function = function
         update_wrapper(out, function)
         return out
 
     def __call__(self, *args, **kwargs) -> Y:
@@ -60,17 +60,17 @@
         return self
 
 
 class FuncEnum(StrEnum):
     """Creating a Enum of functions identifiable by a string."""
 
     @staticmethod
-    def wrap(function: Callable[[X, ...], Y], name: str = None) -> wrapper[X, Y]:
+    def wrap(func: Callable[[X, ...], Y], name: Optional[str] = None) -> wrapper[X, Y]:
         """Function wrapper: class functions are seen as methods and str conversion."""
-        return wrapper(function, name)
+        return wrapper(func, name)
 
     def __call__(self, *args, **kwargs) -> Y:
         """Redirecting the function call."""
         return self.value(*args, **kwargs)
 
 
 class MeanStdTime:
```

### Comparing `opendataval-1.0.0/opendataval/dataloader/__init__.py` & `opendataval-1.1.0/opendataval/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `opendataval-1.0.0/opendataval/dataloader/fetcher.py` & `opendataval-1.1.0/opendataval/dataloader/fetcher.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+import json
 import warnings
 from itertools import accumulate, chain
-from typing import Any, Callable, Sequence, TypeVar, Union
+from pathlib import Path
+from typing import Any, Callable, Optional, Sequence, TypeVar, Union
 
 import numpy as np
+import pandas as pd
 import torch
 from numpy.random import RandomState
 from sklearn.utils import check_random_state
-from torch.utils.data import Dataset, Subset
+from torch.utils.data import DataLoader, Dataset, Subset
 
 from opendataval.dataloader.register import Register
+from opendataval.dataloader.util import CatDataset
 
 Self = TypeVar("Self")
 
 
 class DataFetcher:
     """Load data for an experiment from an input data set name.
 
@@ -67,17 +71,17 @@
     ValueError
         Specified indices must not repeat and must not be outside range of the data set
     """
 
     def __init__(
         self,
         dataset_name: str,
-        cache_dir: str = None,
+        cache_dir: Optional[str] = None,
         force_download: bool = False,
-        random_state: RandomState = None,
+        random_state: Optional[RandomState] = None,
     ):
         if dataset_name not in Register.Datasets:
             raise KeyError(
                 "Must register data set in register_dataset."
                 "Ensure the data set is imported and optional dependencies installed."
             )
 
@@ -122,22 +126,22 @@
         """Get set of available data set names."""
         return set(Register.Datasets.keys())
 
     @classmethod
     def setup(
         cls,
         dataset_name: str,
-        cache_dir: str = None,
+        cache_dir: Optional[str] = None,
         force_download: bool = False,
-        random_state: RandomState = None,
+        random_state: Optional[RandomState] = None,
         train_count: Union[int, float] = 0,
         valid_count: Union[int, float] = 0,
         test_count: Union[int, float] = 0,
-        add_noise: Callable[[Self, Any, ...], dict[str, Any]] = None,
-        noise_kwargs: dict[str, Any] = None,
+        add_noise: Optional[Callable[[Self, Any, ...], dict[str, Any]]] = None,
+        noise_kwargs: Optional[dict[str, Any]] = None,
     ):
         """Create, split, and add noise to DataFetcher from input arguments."""
         noise_kwargs = {} if noise_kwargs is None else noise_kwargs
 
         split_types = (type(train_count), type(valid_count), type(test_count))
         if split_types == (int, int, int):
             return (
@@ -159,15 +163,15 @@
 
     @classmethod
     def from_data(
         cls,
         covar: Union[Dataset, np.ndarray],
         labels: np.ndarray,
         one_hot: bool,
-        random_state: RandomState = None,
+        random_state: Optional[RandomState] = None,
     ):
         """Return DataFetcher from input Covariates and Labels.
 
         Parameters
         ----------
         covar : Union[Dataset, np.ndarray]
             Input covariates
@@ -199,15 +203,15 @@
         x_train: Union[Dataset, np.ndarray],
         y_train: np.ndarray,
         x_valid: Union[Dataset, np.ndarray],
         y_valid: np.ndarray,
         x_test: Union[Dataset, np.ndarray],
         y_test: np.ndarray,
         one_hot: bool,
-        random_state: RandomState = None,
+        random_state: Optional[RandomState] = None,
     ):
         """Return DataFetcher from already split data.
 
         Parameters
         ----------
         x_train : Union[Dataset, np.ndarray]
             Input training covariates
@@ -254,15 +258,17 @@
         (torch.Tensor | Dataset, torch.Tensor)
             Validation Covariates, Valid Labels
         (torch.Tensor | Dataset, torch.Tensor)
             Test Covariates, Test Labels
         """
         x_trn, x_val, x_test = self.x_train, self.x_valid, self.x_test
 
-        if not isinstance(self.x_train, Dataset):  # Turns arrays -> cpu tensors
+        if not isinstance(self.x_train, Dataset) and not isinstance(
+            self.x_train, torch.Tensor
+        ):  # Turns arrays -> cpu tensors
             x_trn = torch.tensor(x_trn, dtype=torch.float).view(-1, *self.covar_dim)
             x_val = torch.tensor(x_val, dtype=torch.float).view(-1, *self.covar_dim)
             x_test = torch.tensor(x_test, dtype=torch.float).view(-1, *self.covar_dim)
 
         y_trn = torch.tensor(self.y_train, dtype=torch.float).view(-1, *self.label_dim)
         y_val = torch.tensor(self.y_valid, dtype=torch.float).view(-1, *self.label_dim)
         y_test = torch.tensor(self.y_test, dtype=torch.float).view(-1, *self.label_dim)
@@ -362,17 +368,17 @@
         self.y_valid = self.labels[self.valid_indices]
         self.y_test = self.labels[self.test_indices]
 
         return self
 
     def split_dataset_by_indices(
         self,
-        train_indices: Sequence[int] = None,
-        valid_indices: Sequence[int] = None,
-        test_indices: Sequence[int] = None,
+        train_indices: Optional[Sequence[int]] = None,
+        valid_indices: Optional[Sequence[int]] = None,
+        test_indices: Optional[Sequence[int]] = None,
     ):
         """Split the covariates and labels to the specified indices.
 
         Parameters
         ----------
         train_indices : Sequence[int]
             Indices of training data set
@@ -422,15 +428,15 @@
         self.valid_indices = np.array(valid_indices, dtype=int)
         self.test_indices = np.array(test_indices, dtype=int)
 
         return self
 
     def noisify(
         self,
-        add_noise: Union[Callable[[Self, Any, ...], dict[str, Any]], str] = None,
+        add_noise: Union[Callable[[Self, Any, ...], dict[str, Any]], str, None] = None,
         *noise_args,
         **noise_kwargs,
     ):
         """Add noise to the data points.
 
         Adds noise to the data set and saves the indices of the noisy data.
         Return object of `add_noise` is a dict with keys to signify how the
@@ -477,7 +483,55 @@
         self.x_valid = noisy_data.get("x_valid", self.x_valid)
         self.y_valid = noisy_data.get("y_valid", self.y_valid)
         self.x_test = noisy_data.get("x_test", self.x_test)
         self.y_test = noisy_data.get("y_test", self.y_test)
         self.noisy_train_indices = noisy_data.get("noisy_train_indices", np.array([]))
 
         return self
+
+    def export_dataset(
+        self,
+        covariates_names: list[str],
+        labels_names: list[str],
+        output_directory: Path = Path.cwd(),
+    ):
+        if isinstance(covariates_names, str):
+            covariates_names = [covariates_names]
+        if isinstance(labels_names, str):
+            labels_names = [labels_names]
+        if not isinstance(output_directory, Path):
+            output_directory = Path(output_directory)
+        if not output_directory.exists():
+            output_directory.mkdir(parents=True)
+
+        columns = covariates_names + labels_names
+        x_train, x_valid, x_test = self.x_train, self.x_valid, self.x_test
+        y_train, y_valid, y_test = self.y_train, self.y_valid, self.y_test
+
+        if self.one_hot:
+            y_train = np.argmax(y_train, axis=1, keepdims=True) if y_train.size else []
+            y_valid = np.argmax(y_valid, axis=1, keepdims=True) if y_valid.size else []
+            y_test = np.argmax(y_test, axis=1, keepdims=True) if y_test.size else []
+
+        def generate_data(covariates, labels):
+            data = CatDataset(covariates, labels)
+            for cov, lab in DataLoader(data, batch_size=1, shuffle=False):
+                yield from np.hstack((cov, lab))
+
+        def save_to_csv(data, file_name):
+            file_path = output_directory / file_name
+            pd.DataFrame(data, columns=columns).to_csv(file_path, index=False)
+
+        save_to_csv(generate_data(x_train, y_train), "train.csv")
+        save_to_csv(generate_data(x_valid, y_valid), "valid.csv")
+        save_to_csv(generate_data(x_test, y_test), "test.csv")
+
+        noisy_indices = (
+            self.noisy_train_indices.tolist()
+            if hasattr(self, "noisy_train_indices")
+            else []
+        )
+        out_path = output_directory / f"noisy-indices-{self.dataset.dataset_name}.json"
+        with open(out_path, "w+") as f:
+            json.dump(noisy_indices, f)
+
+        return
```

### Comparing `opendataval-1.0.0/opendataval/dataloader/noisify.py` & `opendataval-1.1.0/opendataval/dataloader/noisify.py`

 * *Files identical despite different names*

### Comparing `opendataval-1.0.0/opendataval/dataloader/register.py` & `opendataval-1.1.0/opendataval/dataloader/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import warnings
 from functools import lru_cache, partial
 from pathlib import Path
-from typing import Callable, Sequence, TypeVar, Union
+from typing import Callable, ClassVar, Optional, Sequence, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 import requests
 import tqdm
 from torch.utils.data import Dataset
 
@@ -16,15 +16,18 @@
 
 @lru_cache()
 def _request_session():
     return requests.Session()
 
 
 def cache(
-    url: str, cache_dir: Path, file_name: str = None, force_download: bool = False
+    url: str,
+    cache_dir: Path,
+    file_name: Optional[str] = None,
+    force_download: bool = False,
 ) -> Path:
     """Download a file if it it is not present and returns the filepath.
 
     Parameters
     ----------
     url : str
         URL of the file to be downloaded
@@ -124,15 +127,15 @@
         :py:class:`Register` keeps track of all data set names registered and all must
         be unique. If there are any duplicates, warns user.
     """
 
     CACHE_DIR = "data_files"
     """Default directory to cache downloads to."""
 
-    Datasets: dict[str, Self] = {}
+    Datasets: ClassVar[dict[str, Self]] = {}
     """Creates a directory for all registered/downloadable data set functions."""
 
     def __init__(
         self,
         dataset_name: str,
         one_hot: bool = False,
         cacheable: bool = False,
@@ -166,22 +169,21 @@
         return self
 
     def from_numpy(self, array: np.ndarray, label_columns: Union[int, Sequence[int]]):
         """Register data set from covariate and label numpy array."""
         self.covar_label_func = lambda: _from_numpy(array, label_columns)
         return self
 
-    def from_data(self, covar: np.ndarray, label: np.ndarray, one_hot: bool = None):
+    def from_data(self, covar: np.ndarray, label: np.ndarray, one_hot: bool = False):
         """Register data set from covariate and label numpy array."""
         self.covar_label_func = lambda: (covar, label)
-        # Overrides default one_hot if specified
-        if one_hot is not None:
-            self.one_hot = one_hot
-            self.cacheable = False
-            self.label_transform = one_hot_encode if one_hot else self.label_transform
+        self.cacheable = False
+
+        self.one_hot = one_hot
+        self.label_transform = one_hot_encode if one_hot else self.label_transform
 
         return self
 
     def __call__(self, func: DatasetFunc, *args, **kwargs) -> DatasetFunc:
         """Majority of provided datasets are in `from_covar_label_func` format."""
         return self.from_covar_label_func(func, *args, **kwargs)
 
@@ -207,15 +209,15 @@
 
     def add_label_transform(self, transform: Callable[[np.ndarray], np.ndarray]):
         """Add label transform after data is fetched."""
         self.label_transform = transform
         return self
 
     def load_data(
-        self, cache_dir: str = None, force_download: bool = False
+        self, cache_dir: Optional[str] = None, force_download: bool = False
     ) -> tuple[Dataset, np.ndarray]:
         """Retrieve data from specified data input functions.
 
         Loads the covariates and labels from the registered callables, applies
         transformations, and returns the covariates and labels.
 
         Parameters
```

### Comparing `opendataval-1.0.0/opendataval/dataloader/util.py` & `opendataval-1.1.0/opendataval/dataloader/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Sequence, TypeVar
+from typing import Any, Callable, Optional, Sequence, TypeVar
 
 from torch.utils.data import Dataset
 
 T_co = TypeVar("T_co", covariant=True)
 
 
 class CatDataset(Dataset[tuple[Dataset, ...]]):
@@ -49,15 +49,15 @@
         the specific transform per index, by default None which is no transform.
 
     """
 
     def __init__(
         self,
         dataset: Dataset[T_co],
-        index_transformation: Callable[[T_co, int], T_co] = None,
+        index_transformation: Optional[Callable[[T_co, int], T_co]] = None,
     ):
         self.dataset = dataset
         self._transform = index_transformation
 
     @property
     def transform(self) -> Callable[[T_co, int], T_co]:
         """Gets the transform function, if None, no transformation applied."""
```

### Comparing `opendataval-1.0.0/opendataval/dataloader/datasets/challenge.py` & `opendataval-1.1.0/opendataval/dataloader/datasets/challenge.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 def _challenge_ids(challenge: str) -> list[dict[str, str]]:
     """Get challenge ids from the opendataval backend."""
     return requests.get(f"{CHALLENGE_URL}/{challenge}").json()
 
 
-def download_drive(name: str, drive_id: str, cache_dir: Path, force_download: str):
+def download_drive(name: str, drive_id: str, cache_dir: Path, force_download: bool):
     """Downloads file from google drive with set retry attempts."""
     download_url = _dataset_url(drive_id)
     cache_dir = Path(cache_dir)
 
     for i in range(RETRY_ATTEMPTS):
         try:
             return cache(download_url, cache_dir, name, force_download)
@@ -43,15 +43,15 @@
 def basename(file_name: str):
     """Get basename of file."""
     return str(Path(file_name).with_suffix(""))
 
 
 @Register("challenge-iris", cacheable=True, one_hot=True, presplit=True)
 def iris_challenge(cache_dir: str, force_download: bool):
-    drive_ids = _challenge_ids("challenge-iris")
+    drive_ids = _challenge_ids("ChallengeIris")
 
     data = {}
     for row in drive_ids:
         filepath = download_drive(row["name"], row["id"], cache_dir, force_download)
 
         df = pd.read_csv(filepath)
         df["species"] = df["species"].astype("category").cat.codes
```

### Comparing `opendataval-1.0.0/opendataval/dataloader/datasets/cleanlab.py` & `opendataval-1.1.0/opendataval/dataloader/datasets/cleanlab.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 These data sets are NOT 100% perfect, nor are they intended to be.
 
 References
 ----------
 .. [1] C. G. Northcutt, A. Athalye, and J. Mueller,
     Pervasive Label Errors in Test Sets Destabilize Machine Learning Benchmarks
     arXiv.org, 2021. [Online]. Available: https://arxiv.org/abs/2103.14749.
+
+UNDER CONSTRUCTION
 """
 import glob
 import tarfile
 
 from torchvision.datasets import CIFAR10, CIFAR100, ImageNet
 
 from opendataval.dataloader.datasets.imagesets import ResnetEmbeding, VisionAdapter
@@ -65,15 +67,15 @@
 
 imagenet_embed = Register("imagenet-val-embeddings", True, True)(ResnetEmbeding(CleanLabImagenet))
 """Vision Classification registered as ``"imagenet-val-embeddings"`` ResNet50 embeddings"""
 
 cifar10 = Register("cifar10-val", True, True)(VisionAdapter(CIFAR10), train=False)
 """Vision Classification registered as ``"cifar10-val"``, from TorchVision."""
 
-cifar10_embed = Register("cifar10-val-embeddings", True, True)(ResnetEmbeding(CIFAR100), train=False)
+cifar10_embed = Register("cifar10-val-embeddings", True, True)(ResnetEmbeding(CIFAR10), train=False)
 """Vision Classification registered as ``"cifar10-val-embeddings"`` ResNet50 embeddings"""
 
-cifar100 = Register("cifar100-val", True, True)(VisionAdapter(CIFAR10), train=False)
+cifar100 = Register("cifar100-val", True, True)(VisionAdapter(CIFAR100), train=False)
 """Vision Classification registered as ``"cifar100-val"``, from TorchVision."""
 
 cifar100_embed = Register("cifar100-val-embeddings", True, True)(ResnetEmbeding(CIFAR100), train=False)
 """Vision Classification registered as ``"cifar100-val-embeddings"`` ResNet50 embeddings"""
```

### Comparing `opendataval-1.0.0/opendataval/dataloader/datasets/datasets.py` & `opendataval-1.1.0/opendataval/dataloader/datasets/datasets.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,30 +6,36 @@
 import sklearn.datasets as ds
 from sklearn.datasets import fetch_openml
 from sklearn.preprocessing import StandardScaler, minmax_scale
 
 from opendataval.dataloader.register import Register, cache
 
 
-def load_openml(data_id: int):
+def load_openml(data_id: int, is_classification=True):
     """load openml datasets.
 
     A help function to load openml datasets with OpenML ID.
     """
     dataset = fetch_openml(data_id=data_id, as_frame=False)
     category_list = list(dataset["categories"].keys())
     if len(category_list) > 0:
         category_indices = [dataset["feature_names"].index(x) for x in category_list]
         noncategory_indices = [
             i for i in range(len(dataset["feature_names"])) if i not in category_indices
         ]
         X, y = dataset["data"][:, noncategory_indices], dataset["target"]
     else:
         X, y = dataset["data"], dataset["target"]
-    list_of_classes, y = np.unique(y, return_inverse=True)
+
+    # label transformation
+    if is_classification is True:
+        list_of_classes, y = np.unique(y, return_inverse=True)
+    else:
+        y = (y - np.mean(y)) / (np.std(y) + 1e-8)
+
     X = (X - np.mean(X, axis=0)) / (np.std(X, axis=0) + 1e-8)  # standardization
     return X, y
 
 
 @Register("gaussian_classifier", one_hot=True)
 def gaussian_classifier(n: int = 10000, input_dim: int = 10):
     """Binary category data set registered as ``"gaussian_classifier"``.
@@ -141,15 +147,15 @@
 def download_digits():
     """Categorical data set registered as ``"digits"``."""
     return ds.load_digits(return_X_y=True)
 
 
 @Register("breast_cancer", True).add_covar_transform(minmax_scale)
 def download_breast_cancer():
-    """Categorical data set registered as ``"digits"``."""
+    """Categorical data set registered as ``"breast_cancer"``."""
     return ds.load_breast_cancer(return_X_y=True)
 
 
 @Register("election", one_hot=True, cacheable=True)
 def download_election(cache_dir: str, force_download: bool):
     """Categorical data set registered as ``"election"``.
 
@@ -202,15 +208,15 @@
 
 @Register("linnerud")
 def download_linnerud():
     """Regression data set registered as ``"linnerud"``."""
     return ds.load_linnerud(return_X_y=True)
 
 
-# OpenML Datasets
+# OpenML Classification Datasets
 @Register("2dplanes", one_hot=True)
 def download_2dplanes():
     """Categorical data set registered as ``"2dplanes"``."""
     return load_openml(data_id=727)
 
 
 @Register("electricity", one_hot=True)
@@ -244,7 +250,37 @@
 
 
 @Register("creditcard", one_hot=True)
 def download_creditcard():
     """Categorical data set registered as ``"creditcard"``."""
     return load_openml(data_id=42477)
 
+
+# OpenML Regression Datasets
+@Register("wave_energy")
+def download_wave_energy():
+    """Regression data set registered as ``"wave_energy"``."""
+    return load_openml(data_id=44975, is_classification=False)
+
+
+@Register("lowbwt")
+def download_lowbwt():
+    """Regression data set registered as ``"lowbwt"``."""
+    return load_openml(data_id=1193, is_classification=False)
+
+
+@Register("mv")
+def download_mv():
+    """Regression data set registered as ``"mv"``."""
+    return load_openml(data_id=344, is_classification=False)
+
+
+@Register("stock")
+def download_stock():
+    """Regression data set registered as ``"stock"``."""
+    return load_openml(data_id=1200, is_classification=False)
+
+
+@Register("echoMonths")
+def download_echoMonths():
+    """Regression data set registered as ``"echoMonths"``."""
+    return load_openml(data_id=1199, is_classification=False)
```

### Comparing `opendataval-1.0.0/opendataval/dataloader/datasets/imagesets.py` & `opendataval-1.1.0/opendataval/dataloader/datasets/imagesets.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         )
         cache_dir = Path(cache_dir)
         embed_file_name = f"{dataset_class.__name__}_{MAX_DATASET_SIZE}_embed.pt"
         embed_path = cache_dir / embed_file_name
 
         # Resnet inputs expect `img2vec_transforms`ed images as input
         dataset = dataset_class(
-            root=cache_dir.replace("-embeddings", ""),  # Uses original embedding cache
+            root=cache_dir,
             download=force_download or not cache_dir.exists(),
             transform=img2vec_transforms,
             *args,
             **kwargs,
         )
         subset = np.random.RandomState(10).permutation(len(dataset))
```

### Comparing `opendataval-1.0.0/opendataval/dataloader/datasets/nlpsets.py` & `opendataval-1.1.0/opendataval/dataloader/datasets/nlpsets.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import pandas as pd
 import torch
 
 from opendataval.dataloader.register import Register, cache
 from opendataval.dataloader.util import ListDataset
 
-MAX_DATASET_SIZE = 10000
+MAX_DATASET_SIZE = 2000
 """Data Valuation algorithms can take a long time for large data sets, thus cap size."""
 
 
 def BertEmbeddings(func: Callable[[str, bool], tuple[ListDataset, np.ndarray]]):
     """Convert text data into pooled embeddings with DistilBERT model.
 
     Given a data set with a list of string, such as NLP data set function (see below),
@@ -53,23 +53,34 @@
         if embed_path.exists():
             nlp_embeddings = torch.load(embed_path)
             return nlp_embeddings, labels[subset[: len(nlp_embeddings)]]
 
         labels = labels[subset[:MAX_DATASET_SIZE]]
         entries = [entry for entry in dataset[subset[:MAX_DATASET_SIZE]]]
 
+        # Slow down on gpu vs cpu is quite substantial, uses gpu accel if available
+        device = torch.device(
+            "cuda"
+            if torch.cuda.is_available()
+            else "mps"
+            if torch.backends.mps.is_available()
+            else "cpu"
+        )
+
         tokenizer = DistilBertTokenizerFast.from_pretrained(BERT_PRETRAINED_NAME)
-        bert_model = DistilBertModel.from_pretrained(BERT_PRETRAINED_NAME)
+        bert_model = DistilBertModel.from_pretrained(BERT_PRETRAINED_NAME).to(device)
 
         res = tokenizer.__call__(
             entries, max_length=200, padding=True, truncation=True, return_tensors="pt"
-        )
+        ).to(device)
 
         with torch.no_grad():
-            pooled_embeddings = bert_model(res.input_ids, res.attention_mask)[0][:, 0]
+            pooled_embeddings = (
+                (bert_model(res.input_ids, res.attention_mask)[0]).detach().cpu()[:, 0]
+            )
 
         torch.save(pooled_embeddings.detach(), embed_path)
         return pooled_embeddings, np.array(labels)
 
     return wrapper
```

### Comparing `opendataval-1.0.0/opendataval/dataval/__init__.py` & `opendataval-1.1.0/opendataval/dataval/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,25 +23,30 @@
     DVRL
     InfluenceFunctionEval
     KNNShapley
     DataOob
     DataBanzhaf
     BetaShapley
     DataShapley
+    LavaEvaluator
     LeaveOneOut
     ShapEvaluator
     RandomEvaluator
+    RobustVolumeShapley
 """
 from opendataval.dataval.ame import AME
 from opendataval.dataval.api import DataEvaluator
 from opendataval.dataval.dvrl import DVRL
 from opendataval.dataval.influence import InfluenceFunctionEval
 from opendataval.dataval.knnshap import KNNShapley
+from opendataval.dataval.lava import LavaEvaluator
 from opendataval.dataval.margcontrib import (
     BetaShapley,
     DataBanzhaf,
+    DataBanzhafMargContrib,
     DataShapley,
     LeaveOneOut,
     ShapEvaluator,
 )
 from opendataval.dataval.oob import DataOob
 from opendataval.dataval.random import RandomEvaluator
+from opendataval.dataval.volume import RobustVolumeShapley
```

### Comparing `opendataval-1.0.0/opendataval/dataval/api.py` & `opendataval-1.1.0/opendataval/dataval/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from functools import cached_property
-from typing import Callable, TypeVar, Union
+from typing import Callable, ClassVar, Optional, TypeVar, Union
 
 import numpy as np
 import torch
 import torch.nn.functional as F
 from numpy.random import RandomState
 from sklearn.utils import check_random_state
 from torch.utils.data import Dataset
@@ -52,17 +52,17 @@
     ----------
     pred_model : Model
         Prediction model to find how much each training datum contributes towards it.
     data_values: np.array
         Cached data values, used by :py:mod:`opendataval.experiment.exper_methods`
     """
 
-    Evaluators: dict[str, Self] = {}
+    Evaluators: ClassVar[dict[str, Self]] = {}
 
-    def __init__(self, random_state: RandomState = None, *args, **kwargs):
+    def __init__(self, random_state: Optional[RandomState] = None, *args, **kwargs):
         self.random_state = check_random_state(random_state)
 
     def __init_subclass__(cls, *args, **kwargs):
         """Registers DataEvaluator types, used as part of the CLI."""
         super().__init_subclass__(*args, **kwargs)
         cls.Evaluators[cls.__name__.lower()] = cls
 
@@ -159,15 +159,15 @@
 
         return self
 
     def setup(
         self,
         fetcher: DataFetcher,
         pred_model: Model,
-        metric: Callable[[torch.Tensor, torch.Tensor], float] = None,
+        metric: Optional[Callable[[torch.Tensor, torch.Tensor], float]] = None,
     ):
         """Iputs model, metric and data into Data Evaluator.
 
         Parameters
         ----------
         fetcher : DataFetcher
             DataFetcher containing the training and validation data set.
@@ -197,15 +197,15 @@
         self.input_model(pred_model).input_metric(metric)
         return self
 
     def train(
         self,
         fetcher: DataFetcher,
         pred_model: Model,
-        metric: Callable[[torch.Tensor, torch.Tensor], float] = None,
+        metric: Optional[Callable[[torch.Tensor, torch.Tensor], float]] = None,
         *args,
         **kwargs,
     ):
         """Store and transform data, then train model to predict data values.
 
         Trains the Data Evaluator and the underlying prediction model. Wrapper for
         ``self.input_data`` and ``self.train_data_values`` under one method.
```

### Comparing `opendataval-1.0.0/opendataval/dataval/ame/ame.py` & `opendataval-1.1.0/opendataval/dataval/ame/ame.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 import numpy as np
 import torch
 import tqdm
 from numpy.random import RandomState
 from scipy.stats import zscore
 from sklearn.linear_model import LassoCV
 from sklearn.utils import check_random_state
@@ -24,15 +26,17 @@
     ----------
     num_models : int, optional
         Number of models to bag/aggregate, by default 1000
     random_state : RandomState, optional
         Random initial state, by default None
     """
 
-    def __init__(self, num_models: int = 1000, random_state: RandomState = None):
+    def __init__(
+        self, num_models: int = 1000, random_state: Optional[RandomState] = None
+    ):
         self.num_models = num_models
         self.random_state = check_random_state(random_state)
 
     def train_data_values(self, *args, **kwargs):
         """Trains model to predict data values.
 
         Trains the AME model by fitting bagging models on different proportions
@@ -103,15 +107,15 @@
         Random initial state, by default None
     """
 
     def __init__(
         self,
         num_models: int = 1000,
         proportion: float = 1.0,
-        random_state: RandomState = None,
+        random_state: Optional[RandomState] = None,
     ):
         self.num_models = num_models
         self.proportion = proportion
         self.random_state = check_random_state(random_state)
 
     def input_data(
         self,
```

### Comparing `opendataval-1.0.0/opendataval/dataval/dvrl/dvrl.py` & `opendataval-1.1.0/opendataval/dataval/dvrl/dvrl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections import OrderedDict
+from typing import Optional
 
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import tqdm
 from numpy.random import RandomState
@@ -53,15 +54,15 @@
         layer_number: int = 5,
         comb_dim: int = 10,
         rl_epochs: int = 1000,
         rl_batch_size: int = 32,
         lr: float = 0.01,
         threshold: float = 0.9,
         device: torch.device = torch.device("cpu"),
-        random_state: RandomState = None,
+        random_state: Optional[RandomState] = None,
     ):
         # Value estimator parameters
         self.hidden_dim = hidden_dim
         self.layer_number = layer_number
         self.comb_dim = comb_dim
         self.device = device
 
@@ -317,15 +318,15 @@
     def __init__(
         self,
         x_dim: int,
         y_dim: int,
         hidden_dim: int,
         layer_number: int,
         comb_dim: int,
-        random_state: RandomState = None,
+        random_state: Optional[RandomState] = None,
     ):
         super().__init__()
 
         if random_state is not None:  # Can't pass generators to nn.Module layers
             torch.manual_seed(check_random_state(random_state).tomaxint())
 
         mlp_layers = OrderedDict()
```

### Comparing `opendataval-1.0.0/opendataval/dataval/influence/influence.py` & `opendataval-1.1.0/opendataval/dataval/influence/influence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 import numpy as np
 import torch
 import tqdm
 from numpy.random import RandomState
 from sklearn.utils import check_random_state
 from torch.utils.data import Subset
 
@@ -32,15 +34,15 @@
         Random initial state, by default None
     """
 
     def __init__(
         self,
         num_models: int = 1000,
         proportion: float = 0.7,
-        random_state: RandomState = None,
+        random_state: Optional[RandomState] = None,
     ):
         self.num_models = num_models
         self.proportion = proportion
         self.random_state = check_random_state(random_state)
 
     def input_data(
         self,
```

### Comparing `opendataval-1.0.0/opendataval/dataval/knnshap/knnshap.py` & `opendataval-1.1.0/opendataval/dataval/knnshap/knnshap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 import numpy as np
 import torch
 import tqdm
 from numpy.random import RandomState
 from sklearn.utils import check_random_state
 from torch.utils.data import DataLoader
 
@@ -34,16 +36,16 @@
         Random initial state, by default None
     """
 
     def __init__(
         self,
         k_neighbors: int = 10,
         batch_size: int = 32,
-        embedding_model: Model = None,
-        random_state: RandomState = None,
+        embedding_model: Optional[Model] = None,
+        random_state: Optional[RandomState] = None,
     ):
         self.k_neighbors = k_neighbors
         self.batch_size = batch_size
         self.embedding_model = embedding_model
         self.random_state = check_random_state(random_state)
 
     def match(self, y: torch.Tensor) -> torch.Tensor:
@@ -78,25 +80,25 @@
         dist = torch.cat(dist_list, dim=0)
 
         # Arranges by distances
         sort_indices = torch.argsort(dist, dim=0, stable=True)
         y_train_sort = self.y_train[sort_indices]
 
         score = torch.zeros_like(dist)
-        score[sort_indices[m - 1], range(m)] = self.match(y_train_sort[n - 1]) / n
+        score[sort_indices[n - 1], range(m)] = self.match(y_train_sort[n - 1]) / n
 
         # fmt: off
         for i in tqdm.tqdm(range(n - 2, -1, -1)):
             score[sort_indices[i], range(m)] = (
                 score[sort_indices[i + 1], range(m)]
                 + min(self.k_neighbors, i + 1) / (self.k_neighbors * (i + 1))
                 * (self.match(y_train_sort[i]) - self.match(y_train_sort[i + 1]))
             )
 
-        self.data_values = score.mean(axis=1)
+        self.data_values = score.mean(axis=1).detach().numpy()
 
         return self
 
     def evaluate_data_values(self) -> np.ndarray:
         """Return data values for each training data point.
 
         Compute data values using KNN Shapley data valuation
```

### Comparing `opendataval-1.0.0/opendataval/dataval/margcontrib/banzhaf.py` & `opendataval-1.1.0/opendataval/dataval/margcontrib/banzhaf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from itertools import accumulate
+from typing import Optional
 
 import numpy as np
 import torch
 import tqdm
 from numpy.random import RandomState
 from sklearn.utils import check_random_state
 from torch.utils.data import Subset
@@ -24,15 +25,17 @@
     ----------
     num_models : int, optional
         Number of models to take to compute Banzhaf values, by default 1000
     random_state : RandomState, optional
         Random initial state, by default None
     """
 
-    def __init__(self, num_models: int = 1000, random_state: RandomState = None):
+    def __init__(
+        self, num_models: int = 1000, random_state: Optional[RandomState] = None
+    ):
         self.num_models = num_models
         self.random_state = check_random_state(random_state)
 
     def input_data(
         self,
         x_train: torch.Tensor,
         y_train: torch.Tensor,
@@ -160,16 +163,16 @@
 
     def __init__(
         self,
         gr_threshold: float = 1.05,
         max_mc_epochs: int = 100,
         models_per_iteration: int = 100,
         mc_epochs: int = 1000,
-        cache_name: str = None,
-        random_state: RandomState = None,
+        cache_name: Optional[str] = None,
+        random_state: Optional[RandomState] = None,
     ):
         super().__init__(
             gr_threshold=gr_threshold,
             max_mc_epochs=max_mc_epochs,
             models_per_iteration=models_per_iteration,
             mc_epochs=mc_epochs,
             cache_name=cache_name,
```

### Comparing `opendataval-1.0.0/opendataval/dataval/margcontrib/betashap.py` & `opendataval-1.1.0/opendataval/dataval/margcontrib/betashap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 import numpy as np
 from numpy.random import RandomState
 from scipy.special import beta
 
 from opendataval.dataval.margcontrib.shap import ShapEvaluator
 
 
@@ -41,18 +43,18 @@
 
     def __init__(
         self,
         gr_threshold: float = 1.05,
         max_mc_epochs: int = 100,
         models_per_iteration: int = 100,
         mc_epochs: int = 1000,
-        cache_name: str = None,
+        cache_name: Optional[str] = None,
         alpha: int = 4,
         beta: int = 1,
-        random_state: RandomState = None,
+        random_state: Optional[RandomState] = None,
     ):
         super().__init__(
             gr_threshold=gr_threshold,
             max_mc_epochs=max_mc_epochs,
             models_per_iteration=models_per_iteration,
             mc_epochs=mc_epochs,
             cache_name=cache_name,
```

### Comparing `opendataval-1.0.0/opendataval/dataval/margcontrib/datashap.py` & `opendataval-1.1.0/opendataval/dataval/margcontrib/datashap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 import numpy as np
 from numpy.random import RandomState
 
 from opendataval.dataval.margcontrib.shap import ShapEvaluator
 
 
 class DataShapley(ShapEvaluator):
@@ -33,16 +35,16 @@
 
     def __init__(
         self,
         gr_threshold: float = 1.05,
         max_mc_epochs: int = 100,
         models_per_iteration: int = 100,
         mc_epochs: int = 1000,
-        cache_name: str = None,
-        random_state: RandomState = None,
+        cache_name: Optional[str] = None,
+        random_state: Optional[RandomState] = None,
     ):
         super().__init__(
             gr_threshold=gr_threshold,
             max_mc_epochs=max_mc_epochs,
             models_per_iteration=models_per_iteration,
             mc_epochs=mc_epochs,
             cache_name=cache_name,
```

### Comparing `opendataval-1.0.0/opendataval/dataval/margcontrib/loo.py` & `opendataval-1.1.0/opendataval/dataval/margcontrib/loo.py`

 * *Files identical despite different names*

### Comparing `opendataval-1.0.0/opendataval/dataval/margcontrib/shap.py` & `opendataval-1.1.0/opendataval/dataval/margcontrib/shap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from abc import ABC, abstractmethod
+from typing import ClassVar, Optional
 
 import numpy as np
 import torch
 import tqdm
 from numpy.random import RandomState
 from sklearn.utils import check_random_state
 from torch.utils.data import Subset
 
 from opendataval.dataval.api import DataEvaluator
 
 
 class ShapEvaluator(DataEvaluator, ABC):
-    """Abstract class for all Shapley-based methods of computing data values.
+    """Abstract class for all semivalue-based methods of computing data values.
 
     References
     ----------
     .. [1]  A. Ghorbani and J. Zou,
         Data Shapley: Equitable Valuation of Data for Machine Learning,
         arXiv.org, 2019. Available: https://arxiv.org/abs/1904.02868.
 
@@ -38,27 +39,27 @@
         Minimum samples before checking MCMC convergence, by default 1000
     cache_name : str, optional
         Unique cache_name of the model, caches marginal contributions, by default None
     random_state : RandomState, optional
         Random initial state, by default None
     """
 
-    CACHE = {}
+    CACHE: ClassVar[dict[str, np.ndarray]] = {}
     """Cached marginal contributions."""
     GR_MAX = 100
     """Default maximum Gelman-Rubin statistic. Used for burn-in."""
 
     def __init__(
         self,
         gr_threshold: float = 1.05,
         max_mc_epochs: int = 100,
         models_per_iteration: int = 100,
         mc_epochs: int = 1000,
-        cache_name: str = None,
-        random_state: RandomState = None,
+        cache_name: Optional[str] = None,
+        random_state: Optional[RandomState] = None,
     ):
         self.max_mc_epochs = max_mc_epochs
         self.gr_threshold = gr_threshold
         self.models_per_iteration = models_per_iteration
         self.mc_epochs = mc_epochs
 
         self.cache_name = cache_name
@@ -85,15 +86,15 @@
     def input_data(
         self,
         x_train: torch.Tensor,
         y_train: torch.Tensor,
         x_valid: torch.Tensor,
         y_valid: torch.Tensor,
     ):
-        """Store and transform input data for Shapley-based predictors.
+        """Store and transform input data for semivalue-based predictors.
 
         Parameters
         ----------
         x_train : torch.Tensor
             Data covariates
         y_train : torch.Tensor
             Data labels
@@ -183,15 +184,15 @@
         Returns
         -------
         np.ndarray
             An array of marginal increments when one data point is added.
         """
         # for each iteration, we use random permutation for our MCMC
         subset = self.random_state.permutation(self.num_points)
-        marginal_increment = np.zeros(self.num_points) + 1e-12  # Prevents overflow
+        marginal_increment = np.zeros(self.num_points) + 1e-8  # Prevents overflow
         coalition = list(subset[:min_cardinality])
         truncation_counter = 0
 
         # Baseline at minimal cardinality
         prev_perf = curr_perf = self._evaluate_model(coalition, *args, **kwargs)
 
         for cutoff, idx in enumerate(subset[min_cardinality:], start=min_cardinality):
@@ -199,23 +200,19 @@
             coalition.append(idx)
             curr_perf = self._evaluate_model(coalition, *args, **kwargs)
             marginal_increment[idx] = curr_perf - prev_perf
 
             # When the cardinality of random set is 'n',
             self.marginal_contrib_sum[idx, cutoff] += curr_perf - prev_perf
             self.marginal_count[idx, cutoff] += 1
-
-            # if a new increment is not large enough, we terminate the valuation.
-            distance = abs(curr_perf - prev_perf) / np.sum(marginal_increment)
-
-            # update prev_perf
             prev_perf = curr_perf
 
+            # If a new increment is not large enough, we terminate the valuation.
             # If updates are too small then we assume it contributes 0.
-            if distance < 1e-8:
+            if abs(curr_perf - prev_perf) / np.sum(marginal_increment) < 1e-8:
                 truncation_counter += 1
             else:
                 truncation_counter = 0
 
             if truncation_counter == 10:  # If enter space without changes to model
                 break
```

### Comparing `opendataval-1.0.0/opendataval/dataval/oob/oob.py` & `opendataval-1.1.0/opendataval/dataval/oob/oob.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections import defaultdict
+from typing import Optional
 
 import numpy as np
 import torch
 import tqdm
 from numpy.random import RandomState
 from sklearn.utils import check_random_state
 from torch.utils.data import Subset
@@ -33,15 +34,15 @@
         Random initial state, by default None
     """
 
     def __init__(
         self,
         num_models: int = 1000,
         proportion: int = 1.0,
-        random_state: RandomState = None,
+        random_state: Optional[RandomState] = None,
     ):
         self.num_models = num_models
         self.proportion = proportion
         self.random_state = check_random_state(random_state)
 
     def input_data(
         self,
```

### Comparing `opendataval-1.0.0/opendataval/dataval/random/random.py` & `opendataval-1.1.0/opendataval/dataval/random/random.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 import numpy as np
 from numpy.random import RandomState
 from sklearn.utils import check_random_state
 
 from opendataval.dataval.api import DataEvaluator
 
 
@@ -12,15 +14,15 @@
 
     Parameters
     ----------
     random_state : RandomState, optional
         Random initial state, by default None
     """
 
-    def __init__(self, random_state: RandomState = None):
+    def __init__(self, random_state: Optional[RandomState] = None):
         self.random_state = check_random_state(random_state)
 
     def train_data_values(self, *args, **kwargs):
         """RandomEval does not train to find the training values."""
         pass
 
     def evaluate_data_values(self) -> np.ndarray:
```

### Comparing `opendataval-1.0.0/opendataval/experiment/__init__.py` & `opendataval-1.1.0/opendataval/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `opendataval-1.0.0/opendataval/experiment/api.py` & `opendataval-1.1.0/opendataval/experiment/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 import pathlib
 import time
 import warnings
 from datetime import timedelta
-from typing import Any, Callable, Union
+from typing import Any, Callable, Optional, Union
 
 import pandas as pd
 import torch
 from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from numpy.random import RandomState
@@ -43,17 +43,17 @@
         Output directory of experiments
     """
 
     def __init__(
         self,
         fetcher: DataFetcher,
         pred_model: Model,
-        train_kwargs: dict[str, Any] = None,
-        metric_name: str = None,
-        output_dir: Union[str, pathlib.Path] = None,
+        train_kwargs: Optional[dict[str, Any]] = None,
+        metric_name: Optional[str] = None,
+        output_dir: Optional[Union[str, pathlib.Path]] = None,
     ):
         self.fetcher = fetcher
         self.pred_model = pred_model
         self.train_kwargs = {} if train_kwargs is None else train_kwargs
 
         if metric_name is not None:
             self.metric = Metrics(metric_name)
@@ -65,26 +65,26 @@
             self.set_output_directory(output_dir)
         self.timings = {}
 
     @classmethod
     def setup(
         cls,
         dataset_name: str,
-        cache_dir: Union[str, pathlib.Path] = None,
+        cache_dir: Optional[Union[str, pathlib.Path]] = None,
         force_download: bool = False,
         train_count: Union[int, float] = 0,
         valid_count: Union[int, float] = 0,
         test_count: Union[int, float] = 0,
         add_noise: Union[Callable[[DataFetcher], dict[str, Any]], str] = mix_labels,
-        noise_kwargs: dict[str, Any] = None,
-        random_state: RandomState = None,
-        pred_model: Model = None,
-        train_kwargs: dict[str, Any] = None,
-        metric_name: str = None,
-        output_dir: Union[str, pathlib.Path] = None,
+        noise_kwargs: Optional[dict[str, Any]] = None,
+        random_state: Optional[RandomState] = None,
+        pred_model: Optional[Model] = None,
+        train_kwargs: Optional[dict[str, Any]] = None,
+        metric_name: Optional[str] = None,
+        output_dir: Optional[Union[str, pathlib.Path]] = None,
     ):
         """Create a DataFetcher from args and passes it into the init."""
         random_state = check_random_state(random_state)
         noise_kwargs = {} if noise_kwargs is None else noise_kwargs
 
         fetcher = DataFetcher.setup(
             dataset_name=dataset_name,
@@ -106,27 +106,27 @@
             output_dir=output_dir,
         )
 
     @classmethod
     def model_factory_setup(
         cls,
         dataset_name: str,
-        cache_dir: Union[str, pathlib.Path] = None,
+        cache_dir: Optional[Union[str, pathlib.Path]] = None,
         force_download: bool = False,
         train_count: Union[int, float] = 0,
         valid_count: Union[int, float] = 0,
         test_count: Union[int, float] = 0,
         add_noise: Union[Callable[[DataFetcher], dict[str, Any]], str] = mix_labels,
-        noise_kwargs: dict[str, Any] = None,
-        random_state: RandomState = None,
-        model_name: str = None,
+        noise_kwargs: Optional[dict[str, Any]] = None,
+        random_state: Optional[RandomState] = None,
+        model_name: Optional[str] = None,
         device: torch.device = torch.device("cpu"),
-        train_kwargs: dict[str, Any] = None,
-        metric_name: str = None,
-        output_dir: Union[str, pathlib.Path] = None,
+        train_kwargs: Optional[dict[str, Any]] = None,
+        metric_name: Optional[str] = None,
+        output_dir: Optional[Union[str, pathlib.Path]] = None,
     ):
         """Set up ExperimentMediator from ModelFactory using an input string.
 
         Return a ExperimentMediator initialized with
         py:function`~opendataval.model.ModelFactory`
 
         Parameters
@@ -314,16 +314,16 @@
         if save_output:
             self.save_output(f"{exper_func.__name__}.csv", df_resp)
         return df_resp
 
     def plot(
         self,
         exper_func: Callable[[DataEvaluator, DataFetcher, Axes, ...], dict[str, Any]],
-        figure: Figure = None,
-        row: int = None,
+        figure: Optional[Figure] = None,
+        row: Optional[int] = None,
         col: int = 2,
         include_train: bool = False,
         save_output: bool = False,
         **exper_kwargs,
     ) -> tuple[pd.DataFrame, Figure]:
         """Evaluate `exper_func` on each DataEvaluator and plots result in `fig`.
```

### Comparing `opendataval-1.0.0/opendataval/experiment/exper_methods.py` & `opendataval-1.1.0/opendataval/experiment/exper_methods.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,95 +1,96 @@
 """Experiments to test :py:class:`~opendataval.dataval.api.DataEvaluator`.
 
 Experiments pass into :py:meth:`~opendataval.experiment.api.ExperimentMediator.evaluate`
 and :py:meth:`~opendataval.experiment.api.ExperimentMediator.plot` evaluate performance
 of one :py:class:`~opendataval.dataval.api.DataEvaluator` at a time.
 """
-from typing import Any
+from pathlib import Path
+from typing import Any, Optional
 
 import numpy as np
 import pandas as pd
 from matplotlib.axes import Axes
 from mpl_toolkits.axes_grid1.axes_divider import make_axes_locatable
-from sklearn.cluster import KMeans
-from sklearn.metrics import f1_score
 from torch.utils.data import Subset
 
 from opendataval.dataloader import DataFetcher
 from opendataval.dataval import DataEvaluator
+from opendataval.experiment.util import f1_score, oned_twonn_clustering
 
 
-def noisy_detection(evaluator: DataEvaluator, fetcher: DataFetcher) -> dict[str, float]:
+def noisy_detection(
+    evaluator: DataEvaluator,
+    fetcher: DataFetcher = None,
+    indices: Optional[list[int]] = None,
+) -> dict[str, float]:
     """Evaluate ability to identify noisy indices.
 
     Compute F1 score (of 2NN classifier) of the data evaluator
-    on the noisy indices. Noisy indices will be labeled 1 for the positives,
-    while non-Noisy are labeled zero. KMeans labels are random, but because
-    of the convexity the highest data point and lowest data point have different
-    labels and belong to the most valuable/least valuable group. Thus, the least
-    valuable group will be set to 1 and most valuable to zero for the F1 score.
+    on the noisy indices. KMeans labels are random, but because of the convexity of
+    KMeans, the highest data point and lowest data point have different labels and
+    belong to the most valuable/least valuable group. Thus, the least valuable group
+    will be in one group and most valuable to zero for the F1 score.
 
     Parameters
     ----------
     evaluator : DataEvaluator
         DataEvaluator to be tested
-    fetcher : DataFetcher
+    fetcher : DataFetcher, optional
         DataFetcher containing noisy indices
+    indices : list[int], optional
+        Alternatively, pass in noisy indices instead of DataFetcher, by default None
 
     Returns
     -------
     dict[str, float]
 
         - **"kmeans_f1"** -- F1 score performance of a 1D KNN binary classifier
             of the data points. Classifies the lower data value data points as
             corrupted, and the higher value data points as correct.
     """
     data_values = evaluator.data_values
-    noisy_train_indices = fetcher.noisy_train_indices
-
-    num_points = len(data_values)
-    sorted_indices = np.argsort(data_values)
-
-    # Computes F1 of a KMeans(k=2) classifier of the data values
-    kmeans = KMeans(n_clusters=2, n_init="auto").fit(data_values.reshape(-1, 1))
-
-    # Because of the convexity of KMeans classification, the least valuable data point
-    # will always belong to one cluster, while the most valuable will belong to another.
-    labels = (  # If the least valuable group isn't labeled as 1, flips the labels
-        kmeans.labels_ if kmeans.labels_[sorted_indices[0]] == 1 else 1 - kmeans.labels_
+    noisy_train_indices = (
+        fetcher.noisy_train_indices if isinstance(fetcher, DataFetcher) else indices
     )
 
-    # Noisy group is what we're trying to detect, which is why it's set to the positives
-    validation = np.zeros(shape=(num_points,))
-    validation[noisy_train_indices] = 1
-
-    f1_kmeans_label = f1_score(labels, validation)
+    unvaluable, _ = oned_twonn_clustering(data_values.flatten())
+    f1_kmeans_label = f1_score(unvaluable, noisy_train_indices, len(data_values))
 
     return {"kmeans_f1": f1_kmeans_label}
 
 
 def remove_high_low(
     evaluator: DataEvaluator,
     fetcher: DataFetcher,
+    data: Optional[dict[str, Any]] = None,
     percentile: float = 0.05,
-    plot: Axes = None,
+    plot: Optional[Axes] = None,
     metric_name: str = "accuracy",
-    train_kwargs: dict[str, Any] = None,
+    train_kwargs: Optional[dict[str, Any]] = None,
 ) -> dict[str, list[float]]:
     """Evaluate performance after removing high/low points determined by data valuator.
 
     Repeatedly removes ``percentile`` of most valuable/least valuable data points
     and computes the performance of the metric.
 
     Parameters
     ----------
     evaluator : DataEvaluator
         DataEvaluator to be tested
-    fetcher : DataFetcher
-        DataFetcher containing training and valid data points
+    fetcher : DataFetcher, optional
+        DataFetcher containing training and testing data points
+    data : dict[str, Any], optional
+        Alternatively, pass in dictionary instead of a DataFetcher with the training and
+        test data with the following keys:
+
+        - **"x_train"** Training covariates
+        - **"y_train"** Training labels
+        - **"x_test"** Testing covariates
+        - **"y_test"** Testing labels
     percentile : float, optional
         Percentile of data points to remove per iteration, by default 0.05
     plot : Axes, optional
         Matplotlib Axes to plot data output, by default None
     metric_name : str, optional
         Name of DataEvaluator defined performance metric, by default assumed "accuracy"
     train_kwargs : dict[str, Any], optional
@@ -103,15 +104,20 @@
 
         - **"axis"** -- Proportion of data values removed currently
         - **f"remove_least_influential_first_{metric_name}"** -- Performance of model
             after removing a proportion of the data points with the lowest data values
         - **"f"remove_most_influential_first_{metric_name}""** -- Performance of model
             after removing a proportion of the data points with the highest data values
     """
-    x_train, y_train, *_, x_test, y_test = fetcher.datapoints
+    if isinstance(fetcher, DataFetcher):
+        x_train, y_train, *_, x_test, y_test = fetcher.datapoints
+    else:
+        x_train, y_train = data["x_train"], data["y_train"]
+        x_test, y_test = data["x_test"], data["y_test"]
+
     data_values = evaluator.data_values
     curr_model = evaluator.pred_model.clone()
 
     num_points = len(x_train)
     num_period = max(round(num_points * percentile), 5)  # Add at least 5/bin
     num_bins = int(num_points // num_period)
     sorted_value_list = np.argsort(data_values)
@@ -171,28 +177,34 @@
 
     return eval_results
 
 
 def discover_corrupted_sample(
     evaluator: DataEvaluator,
     fetcher: DataFetcher,
+    data: Optional[dict[str, Any]] = None,
     percentile: float = 0.05,
-    plot: Axes = None,
+    plot: Optional[Axes] = None,
 ) -> dict[str, list[float]]:
     """Evaluate discovery of noisy indices in low data value points.
 
     Repeatedly explores ``percentile`` of the data values and determines
     if within that total percentile, what proportion of the noisy indices are found.
 
     Parameters
     ----------
     evaluator : DataEvaluator
         DataEvaluator to be tested
     fetcher : DataFetcher
         DataFetcher containing noisy indices
+    data : dict[str, Any], optional
+        Alternatively, pass in dictionary instead of a DataFetcher with the training and
+        test data with the following keys:
+
+        - **"x_train"** Training covariates
     percentile : float, optional
         Percentile of data points to additionally search per iteration, by default .05
     plot : Axes, optional
         Matplotlib Axes to plot data output, by default None
 
     Returns
     -------
@@ -206,15 +218,18 @@
         - **"optimal"** -- Optimal proportion of corrupted values found currently
             meaning if the inspected **only** contained corrupted samples until
             the number of corrupted samples are completely exhausted.
         - **"random"** -- Random proportion of corrupted samples found, meaning
             if the data points were explored randomly, we'd expect to find
             corrupted_samples in proportion to the number of corruption in the data set.
     """
-    x_train, *_ = fetcher.datapoints
+    if isinstance(fetcher, DataFetcher):
+        x_train, *_ = fetcher.datapoints
+    else:
+        x_train = data["x_train"]
     noisy_train_indices = fetcher.noisy_train_indices
     data_values = evaluator.data_values
 
     num_points = len(x_train)
     num_period = max(round(num_points * percentile), 5)  # Add at least 5 per bin
     num_bins = int(num_points // num_period) + 1
 
@@ -254,36 +269,44 @@
 
         plot.set_title(str(evaluator))
 
     # Returns True Positive Rate of corrupted label discovery
     return eval_results
 
 
-def save_dataval(evaluator: DataEvaluator, fetcher: DataFetcher, output_path: str = ""):
+def save_dataval(
+    evaluator: DataEvaluator,
+    fetcher: DataFetcher = None,
+    indices: Optional[list[int]] = None,
+    output_path: Path = Path("dataval.csv"),
+):
     """Save the indices and the respective data values of the DataEvaluator."""
-    train_indices = fetcher.train_indices
+    train_indices = (
+        fetcher.train_indices if isinstance(fetcher, DataFetcher) else indices
+    )
     data_values = evaluator.data_values
 
     data = {"indices": train_indices, "data_values": data_values}
 
     if output_path:
         df_data = {str(evaluator): data}
         df = pd.DataFrame.from_dict(df_data, "index")
         df.explode(list(df.columns)).to_csv(output_path)
 
     return data
 
 
 def increasing_bin_removal(
     evaluator: DataEvaluator,
-    fetcher: DataFetcher,
+    fetcher: DataFetcher = None,
+    data: Optional[dict[str, Any]] = None,
     bin_size: int = 1,
-    plot: Axes = None,
+    plot: Optional[Axes] = None,
     metric_name: str = "accuracy",
-    train_kwargs: dict[str, Any] = None,
+    train_kwargs: Optional[dict[str, Any]] = None,
 ) -> dict[str, list[float]]:
     """Evaluate accuracy after removing data points with data values above threshold.
 
     For each subplot, displays the proportion of the data set with data values less
     than the specified data value (x-axis) and the performance of the model when all
     data values greater than the specified data value is removed. This implementation
     was inspired by V. Feldman and C. Zhang in their paper [1] where the same principle
@@ -298,14 +321,22 @@
 
     Parameters
     ----------
     evaluator : DataEvaluator
         DataEvaluator to be tested
     fetcher : DataFetcher
         DataFetcher containing training and valid data points
+    data : dict[str, Any], optional
+        Alternatively, pass in dictionary instead of a DataFetcher with the training and
+        test data with the following keys:
+
+        - **"x_train"** Training covariates
+        - **"y_train"** Training labels
+        - **"x_test"** Testing covariates
+        - **"y_test"** Testing labels
     bin_size : float, optional
         We look at bins of equal size and find the data values cutoffs for the x-axis,
         by default 1
     plot : Axes, optional
         Matplotlib Axes to plot data output, by default None
     metric_name : str, optional
         Name of DataEvaluator defined performance metric, by default assumed "accuracy"
@@ -323,15 +354,19 @@
         - **"frac_datapoints_explored"** -- Proportion of data points with data values
             below the specified threshold
         - **f"{metric_name}_at_datavalues"** -- Performance metric when data values
             above the specified threshold are removed
     """
     data_values = evaluator.data_values
     curr_model = evaluator.pred_model
-    x_train, y_train, *_, x_test, y_test = fetcher.datapoints
+    if isinstance(fetcher, DataFetcher):
+        x_train, y_train, *_, x_test, y_test = fetcher.datapoints
+    else:
+        x_train, y_train = data["x_train"], data["y_train"]
+        x_test, y_test = data["x_test"], data["y_test"]
 
     num_points = len(data_values)
 
     # Starts with 10 data points
     bins_indices = [*range(5, num_points - 1, bin_size), num_points - 1]
     frac_datapoints_explored = [(i + 1) / num_points for i in bins_indices]
```

### Comparing `opendataval-1.0.0/opendataval/model/__init__.py` & `opendataval-1.1.0/opendataval/model/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,16 @@
         & \mbox{learning rate} & 0.01 & \mbox{yes} \\
         & \mbox{optimizer} & \mbox{ADAM} & \mbox{no} \\
         & \mbox{loss function} & \mbox{Mean Square Error} & \mbox{no} \\
     \hline
     \end{array}
 """
 # Model Factory imports
+from typing import Optional
+
 import torch
 from sklearn.linear_model import LinearRegression
 from sklearn.linear_model import LogisticRegression as SkLogReg
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.neural_network import MLPClassifier
 
 from opendataval.dataloader import DataFetcher
@@ -104,15 +106,15 @@
 from opendataval.model.lenet import LeNet
 from opendataval.model.logistic_regression import LogisticRegression
 from opendataval.model.mlp import ClassifierMLP, RegressionMLP
 
 
 def ModelFactory(
     model_name: str,
-    fetcher: DataFetcher = None,
+    fetcher: Optional[DataFetcher] = None,
     device: torch.device = torch.device("cpu"),
     *args,
     **kwargs,
 ) -> Model:
     """Factory to create prediction models from specified presets
 
     Model Factory that creates a specified mode, based on the input parameters, it is
@@ -170,10 +172,10 @@
             MLPClassifier, label_dim[0], *args, **kwargs
         )
     elif model_name == "skknn":
         return ClassifierUnweightedSkLearnWrapper(
             KNeighborsClassifier, label_dim[0], label_dim[0], *args, **kwargs
         )
     elif model_name == "sklinreg":
-        return RegressionSkLearnWrapper(LinearRegression, label_dim[0], *args, **kwargs)
+        return RegressionSkLearnWrapper(LinearRegression, *args, **kwargs)
     else:
         raise ValueError(f"{model_name} is not a valid predefined model")
```

### Comparing `opendataval-1.0.0/opendataval/model/api.py` & `opendataval-1.1.0/opendataval/model/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 import warnings
 from abc import ABC, abstractmethod
-from typing import TypeVar, Union
+from typing import ClassVar, Optional, TypeVar, Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from sklearn.dummy import DummyClassifier, DummyRegressor
 from torch.utils.data import DataLoader, Dataset, default_collate
@@ -14,28 +14,28 @@
 
 Self = TypeVar("Self")
 
 
 class Model(ABC):
     """Abstract class of Models. Provides a template for models."""
 
-    Models: dict[str, Self] = {}
+    Models: ClassVar[dict[str, Self]] = {}
 
     def __init_subclass__(cls, *args, **kwargs):
         """Registers Model types, used as part of the CLI."""
         super().__init_subclass__(*args, **kwargs)
         cls.Models[cls.__name__.lower()] = cls
 
     @abstractmethod
     def fit(
         self,
         x_train: Union[torch.Tensor, Dataset],
         y_train: Union[torch.Tensor, Dataset],
         *args,
-        sample_weights: torch.Tensor = None,
+        sample_weights: Optional[torch.Tensor] = None,
         **kwargs
     ) -> Self:
         """Fits the model on the training data.
 
         Parameters
         ----------
         x_train : torch.Tensor | Dataset
@@ -95,15 +95,15 @@
     def device(self):
         return next(self.parameters()).device
 
     def fit(
         self,
         x_train: Union[torch.Tensor, Dataset],
         y_train: Union[torch.Tensor, Dataset],
-        sample_weight: torch.Tensor = None,
+        sample_weight: Optional[torch.Tensor] = None,
         batch_size: int = 32,
         epochs: int = 1,
         lr: float = 0.01,
     ):
         """Fits the model on the training data.
 
         Fits a torch classifier Model object using ADAM optimizer and cross
@@ -162,15 +162,15 @@
     def device(self):
         return next(self.parameters()).device
 
     def fit(
         self,
         x_train: Union[torch.Tensor, Dataset],
         y_train: Union[torch.Tensor, Dataset],
-        sample_weight: torch.Tensor = None,
+        sample_weight: Optional[torch.Tensor] = None,
         batch_size: int = 32,
         epochs: int = 1,
         lr: float = 0.01,
     ):
         """Fits the regression model on the training data.
 
         Fits a torch regression Model object using ADAM optimizer and MSE loss.
@@ -280,15 +280,15 @@
         self.num_classes = num_classes
 
     def fit(
         self,
         x_train: Union[torch.Tensor, Dataset],
         y_train: Union[torch.Tensor, Dataset],
         *args,
-        sample_weight: torch.Tensor = None,
+        sample_weight: Optional[torch.Tensor] = None,
         **kwargs
     ):
         """Fits the model on the training data.
 
         Fits a sk-learn wrapped classifier Model. If there are less classes in the
         sample than num_classes, uses dummy model.
         ::
@@ -381,15 +381,15 @@
     """
 
     def fit(
         self,
         x_train: Union[torch.Tensor, Dataset],
         y_train: Union[torch.Tensor, Dataset],
         *args,
-        sample_weight: torch.Tensor = None,
+        sample_weight: Optional[torch.Tensor] = None,
         **kwargs
     ):
         """Fits the model on the training data.
 
         Fits a sk-learn wrapped classifier Model without sample weight.
 
         Parameters
@@ -455,21 +455,22 @@
     ----------
     base_model : BaseModel
         Any sk-learn model that supports ``sample_weights``
     """
 
     def __init__(self, base_model, *args, **kwargs):
         self.model = base_model(*args, **kwargs)
+        self.num_classes = 1
 
     def fit(
         self,
         x_train: Union[torch.Tensor, Dataset],
         y_train: Union[torch.Tensor, Dataset],
         *args,
-        sample_weight: torch.Tensor = None,
+        sample_weight: Optional[torch.Tensor] = None,
         **kwargs
     ):
         """Fits the model on the training data.
 
         Fits a sk-learn wrapped regression Model. If there is insufficient data to fit
         a regression (such as len(x_train)==0), will use DummyRegressor that predicts
         np.zeros((num_samples, self.num_classes))
```

### Comparing `opendataval-1.0.0/opendataval/model/bert.py` & `opendataval-1.1.0/opendataval/model/bert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import OrderedDict
-from typing import Sequence, Union
+from typing import Optional, Sequence, Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.utils.data import DataLoader, Dataset, TensorDataset
 from transformers import (
     DistilBertModel,
@@ -71,15 +71,17 @@
         for param in self.bert.embeddings.parameters():
             param.requires_grad = False
 
         for layer in self.bert.transformer.layer[: -max(num_train_layers, 1)]:
             for param in layer.parameters():
                 param.requires_grad = False
 
-    def forward(self, input_ids: torch.Tensor, attention_mask: torch.Tensor = None):
+    def forward(
+        self, input_ids: torch.Tensor, attention_mask: Optional[torch.Tensor] = None
+    ):
         """Forward pass through DistilBert with inputs from DistilBERT tokenizer output.
 
         NOTE this is only applicable for a DistilBERT model that doesn't require
         ``token_type_ids``.
 
         Parameters
         ----------
@@ -147,15 +149,15 @@
 
         return TensorDataset(batch_encoding.input_ids, batch_encoding.attention_mask)
 
     def fit(
         self,
         x_train: Dataset[Union[str, list[str]]],
         y_train: torch.Tensor,
-        sample_weight: torch.Tensor = None,
+        sample_weight: Optional[torch.Tensor] = None,
         batch_size: int = 32,
         epochs: int = 1,
         lr: float = 0.001,
     ):
         """Fit the model on the training data.
 
         Fine tunes a pre-trained BERT model on an input Sequence[str] by tokenizing the
```

### Comparing `opendataval-1.0.0/opendataval/model/lenet.py` & `opendataval-1.1.0/opendataval/model/lenet.py`

 * *Files identical despite different names*

### Comparing `opendataval-1.0.0/opendataval/model/logistic_regression.py` & `opendataval-1.1.0/opendataval/model/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `opendataval-1.0.0/opendataval/model/mlp.py` & `opendataval-1.1.0/opendataval/model/mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import OrderedDict
-from typing import Callable
+from typing import Callable, Optional
 
 import torch
 import torch.nn as nn
 
 from opendataval.model.api import (
     TorchClassMixin,
     TorchPredictMixin,
@@ -30,15 +30,15 @@
 
     def __init__(
         self,
         input_dim: int,
         num_classes: int,
         layers: int = 5,
         hidden_dim: int = 25,
-        act_fn: Callable = None,
+        act_fn: Optional[Callable] = None,
     ):
         super().__init__()
 
         act_fn = nn.ReLU() if act_fn is None else act_fn
         self.num_classes = num_classes
 
         mlp_layers = OrderedDict()
@@ -88,18 +88,18 @@
     act_fn : Callable, optional
         Activation function for MLP, if none, set to nn.ReLU, by default None
     """
 
     def __init__(
         self,
         input_dim: int,
-        num_classes: int,
+        num_classes: int = 1,
         layers: int = 5,
         hidden_dim: int = 25,
-        act_fn: Callable = None,
+        act_fn: Optional[Callable] = None,
     ):
         super().__init__()
 
         act_fn = nn.ReLU() if act_fn is None else act_fn
 
         mlp_layers = OrderedDict()
```

### Comparing `opendataval-1.0.0/test/test_dataevaluator.py` & `opendataval-1.1.0/test/test_dataevaluator.py`

 * *Files identical despite different names*

### Comparing `opendataval-1.0.0/test/test_dataloader.py` & `opendataval-1.1.0/test/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `opendataval-1.0.0/test/test_exper_methods.py` & `opendataval-1.1.0/test/test_exper_methods.py`

 * *Files identical despite different names*

### Comparing `opendataval-1.0.0/test/test_experiment.py` & `opendataval-1.1.0/test/test_experiment.py`

 * *Files identical despite different names*

### Comparing `opendataval-1.0.0/test/test_register.py` & `opendataval-1.1.0/test/test_register.py`

 * *Files identical despite different names*

### Comparing `opendataval-1.0.0/.gitignore` & `opendataval-1.1.0/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -85,7 +85,12 @@
 
 # Data
 data_files/
 tmp_*/
 tmp/
 csv/
 kaggle.json
+
+demo/
+demo*.ipynb
+.DS_STORE
+
```

### Comparing `opendataval-1.0.0/LICENSE.txt` & `opendataval-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opendataval-1.0.0/README.md` & `opendataval-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 | Feature | Status | Links | Notes |
 |---------|--------|-------|-------|
 | **[Datasets](https://github.com/opendataval/opendataval/tree/main/opendataval/dataloader/readme.md)** | Stable | [Docs](https://opendataval.github.io/opendataval.dataloader.datasets.html#opendataval-dataloader-datasets-package) | Embeddings available for image/NLP datasets |
 | **[Models](https://github.com/opendataval/opendataval/tree/main/opendataval/model/readme.md)** | Stable | [Docs](https://opendataval.github.io/opendataval.model.html#module-opendataval.model) | Support available for sk-learn models |
 | **[Data Evaluators](https://github.com/opendataval/opendataval/tree/main/opendataval/dataval/readme.md)** | Stable | [Docs](https://opendataval.github.io/opendataval.dataval.html#module-opendataval.dataval) | |
 | **[Experiments](https://github.com/opendataval/opendataval/tree/main/opendataval/experiment/readme.md)** | Stable | [Docs](https://opendataval.github.io/opendataval.experiment.html#module-opendataval.experiment) | |
+| **[Examples](https://github.com/opendataval/opendataval/tree/main/examples/readme.md)** | Stable | | |
 | **[CLI](https://github.com/opendataval/opendataval/tree/main/opendataval/__main__.py)** | Experimental | `opendataval --help` | No support for null values |
 
 <p align="right">(<a href="#readme-top">Back to top</a>)</p>
 
 ## :hourglass_flowing_sand: Installation options
 1. Install with pip
     ```sh
@@ -238,10 +239,10 @@
 [PyTorch-url]: https://pytorch.org/
 [scikit-learn-shield]: https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white
 [scikit-learn-url]: https://scikit-learn.org/stable/
 [numpy-url]: https://numpy.org/
 [numpy-shield]: https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white\
 [release-shield]: https://img.shields.io/github/v/release/opendataval/opendataval?style=for-the-badge
 [release-url]: https://github.com/opendataval/opendataval/releases
-<!-- Pytest Coverage Comment:Begin -->
-[coverage_badge]: https://img.shields.io/badge/Coverage-82%25-green.svg?style=for-the-badge
-<!-- Pytest Coverage Comment:End -->
+<!-- Coverage Comment:Begin -->
+[coverage_badge]: https://img.shields.io/badge/Coverage-80%25-green.svg?style=for-the-badge
+<!-- Coverage Comment:End -->
```

#### html2text {}

```diff
@@ -28,17 +28,19 @@
 [Docs](https://opendataval.github.io/opendataval.model.html#module-
 opendataval.model) | Support available for sk-learn models | | **[Data
 Evaluators](https://github.com/opendataval/opendataval/tree/main/opendataval/
 dataval/readme.md)** | Stable | [Docs](https://opendataval.github.io/
 opendataval.dataval.html#module-opendataval.dataval) | | | **[Experiments]
 (https://github.com/opendataval/opendataval/tree/main/opendataval/experiment/
 readme.md)** | Stable | [Docs](https://opendataval.github.io/
-opendataval.experiment.html#module-opendataval.experiment) | | | **[CLI](https:
-//github.com/opendataval/opendataval/tree/main/opendataval/__main__.py)** |
-Experimental | `opendataval --help` | No support for null values |
+opendataval.experiment.html#module-opendataval.experiment) | | | **[Examples]
+(https://github.com/opendataval/opendataval/tree/main/examples/readme.md)** |
+Stable | | | | **[CLI](https://github.com/opendataval/opendataval/tree/main/
+opendataval/__main__.py)** | Experimental | `opendataval --help` | No support
+for null values |
                                                                   (Back_to_top)
 ## :hourglass_flowing_sand: Installation options 1. Install with pip ```sh pip
 install opendataval ``` 2. Clone the repo and install ```sh git clone https://
 github.com/opendataval/opendataval.git make install ``` a. Install optional
 dependencies if you're [contributing](https://github.com/opendataval/
 opendataval/blob/main/CONTRIBUTING.md) ```sh make install-dev ``` b. If you
 want to pull in kaggle datasets, I'd reccomend looking how to add a kaggle
@@ -163,8 +165,8 @@
 img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-
 badge&logo=scikit-learn&logoColor=white [scikit-learn-url]: https://scikit-
 learn.org/stable/ [numpy-url]: https://numpy.org/ [numpy-shield]: https://
 img.shields.io/badge/numpy-%23013243.svg?style=for-the-
 badge&logo=numpy&logoColor=white\ [release-shield]: https://img.shields.io/
 github/v/release/opendataval/opendataval?style=for-the-badge [release-url]:
 https://github.com/opendataval/opendataval/releases  [coverage_badge]: https://
-img.shields.io/badge/Coverage-82%25-green.svg?style=for-the-badge
+img.shields.io/badge/Coverage-80%25-green.svg?style=for-the-badge
```

### Comparing `opendataval-1.0.0/pyproject.toml` & `opendataval-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -19,19 +19,20 @@
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development",
     "Topic :: Scientific/Engineering",
 
 ]
 dependencies = [
+    "geomloss~=0.2.6",
     "matplotlib~=3.7.1",
     "numpy~=1.24",
-    "opendatasets~=0.1.22",
     "pandas~=2.0",
     "pandera~=0.15.1",
+    "pykeops~=2.1.2",
     "requests~=2.31.0",
     "scipy~=1.10",
     "scikit-learn~=1.2",
     "torch~=2.0.0",
     "torchvision~=0.15",
     "tqdm~=4.64",
     "transformers~=4.30.1",
@@ -49,15 +50,15 @@
 
 [project.optional-dependencies]
 dev = [
     "black~=22.10",
     "hatch~=1.7.0",
     "pip-tools~=6.13.0",
     "pre-commit~=3.2",
-    "ruff~=0.0.2",
+    "ruff~=0.0.275",
     "sphinx~=6.1"
 ]
 test = [
     "pytest~=7.2.2",
     "pytest-cov~=4.0.0"
 ]
 
@@ -101,15 +102,14 @@
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
 [tool.ruff.isort]
 known-first-party = ["opendataval"]
 known-third-party = [
     "numpy",
-    "opendatasets",
     "pandas",
     "pandera",
     "requests",
     "scipy",
     "sklearn",
     "matplotlib",
     "torch",
```

### Comparing `opendataval-1.0.0/PKG-INFO` & `opendataval-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: opendataval
-Version: 1.0.0
+Version: 1.1.0
 Summary: Transparent Data Valuation
 Project-URL: Documentation, https://opendataval.github.io
 Project-URL: Source code, https://github.com/opendataval/opendataval
 Author-email: Anonymous Author 1 <opendataval+1@gmail.com>, Anonymous Author 2 <opendataval+2@gmail.com>, Anonymous Author 3 <opendataval+3@gmail.com>, Anonymous Author 4 <opendataval+4@gmail.com>
 License: MIT
 License-File: LICENSE.txt
 Keywords: Data Centric,Data Valuation,Machine Learning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9.0
+Requires-Dist: geomloss~=0.2.6
 Requires-Dist: matplotlib~=3.7.1
 Requires-Dist: numpy~=1.24
-Requires-Dist: opendatasets~=0.1.22
 Requires-Dist: pandas~=2.0
 Requires-Dist: pandera~=0.15.1
+Requires-Dist: pykeops~=2.1.2
 Requires-Dist: requests~=2.31.0
 Requires-Dist: scikit-learn~=1.2
 Requires-Dist: scipy~=1.10
 Requires-Dist: torchvision~=0.15
 Requires-Dist: torch~=2.0.0
 Requires-Dist: tqdm~=4.64
 Requires-Dist: transformers~=4.30.1
 Requires-Dist: typer~=0.9
 Provides-Extra: dev
 Requires-Dist: black~=22.10; extra == 'dev'
 Requires-Dist: hatch~=1.7.0; extra == 'dev'
 Requires-Dist: pip-tools~=6.13.0; extra == 'dev'
 Requires-Dist: pre-commit~=3.2; extra == 'dev'
-Requires-Dist: ruff~=0.0.2; extra == 'dev'
+Requires-Dist: ruff~=0.0.275; extra == 'dev'
 Requires-Dist: sphinx~=6.1; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest-cov~=4.0.0; extra == 'test'
 Requires-Dist: pytest~=7.2.2; extra == 'test'
 Description-Content-Type: text/markdown
 
 <a name="readme-top" id="readme-top"></a>
@@ -75,14 +76,15 @@
 
 | Feature | Status | Links | Notes |
 |---------|--------|-------|-------|
 | **[Datasets](https://github.com/opendataval/opendataval/tree/main/opendataval/dataloader/readme.md)** | Stable | [Docs](https://opendataval.github.io/opendataval.dataloader.datasets.html#opendataval-dataloader-datasets-package) | Embeddings available for image/NLP datasets |
 | **[Models](https://github.com/opendataval/opendataval/tree/main/opendataval/model/readme.md)** | Stable | [Docs](https://opendataval.github.io/opendataval.model.html#module-opendataval.model) | Support available for sk-learn models |
 | **[Data Evaluators](https://github.com/opendataval/opendataval/tree/main/opendataval/dataval/readme.md)** | Stable | [Docs](https://opendataval.github.io/opendataval.dataval.html#module-opendataval.dataval) | |
 | **[Experiments](https://github.com/opendataval/opendataval/tree/main/opendataval/experiment/readme.md)** | Stable | [Docs](https://opendataval.github.io/opendataval.experiment.html#module-opendataval.experiment) | |
+| **[Examples](https://github.com/opendataval/opendataval/tree/main/examples/readme.md)** | Stable | | |
 | **[CLI](https://github.com/opendataval/opendataval/tree/main/opendataval/__main__.py)** | Experimental | `opendataval --help` | No support for null values |
 
 <p align="right">(<a href="#readme-top">Back to top</a>)</p>
 
 ## :hourglass_flowing_sand: Installation options
 1. Install with pip
     ```sh
@@ -278,10 +280,10 @@
 [PyTorch-url]: https://pytorch.org/
 [scikit-learn-shield]: https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white
 [scikit-learn-url]: https://scikit-learn.org/stable/
 [numpy-url]: https://numpy.org/
 [numpy-shield]: https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white\
 [release-shield]: https://img.shields.io/github/v/release/opendataval/opendataval?style=for-the-badge
 [release-url]: https://github.com/opendataval/opendataval/releases
-<!-- Pytest Coverage Comment:Begin -->
-[coverage_badge]: https://img.shields.io/badge/Coverage-82%25-green.svg?style=for-the-badge
-<!-- Pytest Coverage Comment:End -->
+<!-- Coverage Comment:Begin -->
+[coverage_badge]: https://img.shields.io/badge/Coverage-80%25-green.svg?style=for-the-badge
+<!-- Coverage Comment:End -->
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: opendataval Version: 1.0.0 Summary: Transparent
+Metadata-Version: 2.1 Name: opendataval Version: 1.1.0 Summary: Transparent
 Data Valuation Project-URL: Documentation, https://opendataval.github.io
 Project-URL: Source code, https://github.com/opendataval/opendataval Author-
 email: Anonymous Author 1
 1@gmail.com>, Anonymous Author 2
 2@gmail.com>, Anonymous Author 3
 3@gmail.com>, Anonymous Author 4
 4@gmail.com> License: MIT License-File: LICENSE.txt Keywords: Data Centric,Data
 Valuation,Machine Learning Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering Classifier: Topic :: Software Development Requires-
-Python: >=3.9.0 Requires-Dist: matplotlib~=3.7.1 Requires-Dist: numpy~=1.24
-Requires-Dist: opendatasets~=0.1.22 Requires-Dist: pandas~=2.0 Requires-Dist:
-pandera~=0.15.1 Requires-Dist: requests~=2.31.0 Requires-Dist: scikit-
-learn~=1.2 Requires-Dist: scipy~=1.10 Requires-Dist: torchvision~=0.15
-Requires-Dist: torch~=2.0.0 Requires-Dist: tqdm~=4.64 Requires-Dist:
-transformers~=4.30.1 Requires-Dist: typer~=0.9 Provides-Extra: dev Requires-
-Dist: black~=22.10; extra == 'dev' Requires-Dist: hatch~=1.7.0; extra == 'dev'
-Requires-Dist: pip-tools~=6.13.0; extra == 'dev' Requires-Dist: pre-
-commit~=3.2; extra == 'dev' Requires-Dist: ruff~=0.0.2; extra == 'dev'
+Python: >=3.9.0 Requires-Dist: geomloss~=0.2.6 Requires-Dist: matplotlib~=3.7.1
+Requires-Dist: numpy~=1.24 Requires-Dist: pandas~=2.0 Requires-Dist:
+pandera~=0.15.1 Requires-Dist: pykeops~=2.1.2 Requires-Dist: requests~=2.31.0
+Requires-Dist: scikit-learn~=1.2 Requires-Dist: scipy~=1.10 Requires-Dist:
+torchvision~=0.15 Requires-Dist: torch~=2.0.0 Requires-Dist: tqdm~=4.64
+Requires-Dist: transformers~=4.30.1 Requires-Dist: typer~=0.9 Provides-Extra:
+dev Requires-Dist: black~=22.10; extra == 'dev' Requires-Dist: hatch~=1.7.0;
+extra == 'dev' Requires-Dist: pip-tools~=6.13.0; extra == 'dev' Requires-Dist:
+pre-commit~=3.2; extra == 'dev' Requires-Dist: ruff~=0.0.275; extra == 'dev'
 Requires-Dist: sphinx~=6.1; extra == 'dev' Provides-Extra: test Requires-Dist:
 pytest-cov~=4.0.0; extra == 'test' Requires-Dist: pytest~=7.2.2; extra ==
 'test' Description-Content-Type: text/markdown   ___[Logo_toggles_light_and
 dark_mode]_ # OpenDataVal: a Unified Benchmark for Data Valuation  Assessing
 the quality of individual data points is critical for improving model
 performance and mitigating biases. However, there is no way to systematically
 benchmark different algorithims. **OpenDataVal** is an open-source initiative
@@ -51,17 +51,19 @@
 [Docs](https://opendataval.github.io/opendataval.model.html#module-
 opendataval.model) | Support available for sk-learn models | | **[Data
 Evaluators](https://github.com/opendataval/opendataval/tree/main/opendataval/
 dataval/readme.md)** | Stable | [Docs](https://opendataval.github.io/
 opendataval.dataval.html#module-opendataval.dataval) | | | **[Experiments]
 (https://github.com/opendataval/opendataval/tree/main/opendataval/experiment/
 readme.md)** | Stable | [Docs](https://opendataval.github.io/
-opendataval.experiment.html#module-opendataval.experiment) | | | **[CLI](https:
-//github.com/opendataval/opendataval/tree/main/opendataval/__main__.py)** |
-Experimental | `opendataval --help` | No support for null values |
+opendataval.experiment.html#module-opendataval.experiment) | | | **[Examples]
+(https://github.com/opendataval/opendataval/tree/main/examples/readme.md)** |
+Stable | | | | **[CLI](https://github.com/opendataval/opendataval/tree/main/
+opendataval/__main__.py)** | Experimental | `opendataval --help` | No support
+for null values |
                                                                   (Back_to_top)
 ## :hourglass_flowing_sand: Installation options 1. Install with pip ```sh pip
 install opendataval ``` 2. Clone the repo and install ```sh git clone https://
 github.com/opendataval/opendataval.git make install ``` a. Install optional
 dependencies if you're [contributing](https://github.com/opendataval/
 opendataval/blob/main/CONTRIBUTING.md) ```sh make install-dev ``` b. If you
 want to pull in kaggle datasets, I'd reccomend looking how to add a kaggle
@@ -186,8 +188,8 @@
 img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-
 badge&logo=scikit-learn&logoColor=white [scikit-learn-url]: https://scikit-
 learn.org/stable/ [numpy-url]: https://numpy.org/ [numpy-shield]: https://
 img.shields.io/badge/numpy-%23013243.svg?style=for-the-
 badge&logo=numpy&logoColor=white\ [release-shield]: https://img.shields.io/
 github/v/release/opendataval/opendataval?style=for-the-badge [release-url]:
 https://github.com/opendataval/opendataval/releases  [coverage_badge]: https://
-img.shields.io/badge/Coverage-82%25-green.svg?style=for-the-badge
+img.shields.io/badge/Coverage-80%25-green.svg?style=for-the-badge
```

