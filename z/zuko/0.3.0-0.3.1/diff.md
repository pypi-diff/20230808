# Comparing `tmp/zuko-0.3.0.tar.gz` & `tmp/zuko-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zuko-0.3.0.tar", last modified: Wed Aug  2 20:01:55 2023, max compression
+gzip compressed data, was "zuko-0.3.1.tar", last modified: Tue Aug  8 17:41:20 2023, max compression
```

## Comparing `zuko-0.3.0.tar` & `zuko-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-08-02 20:01:55.282693 zuko-0.3.0/
--rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2022-12-13 12:43:25.000000 zuko-0.3.0/LICENSE
--rw-rw-r--   0 francois  (1001) francois  (1001)     5377 2023-08-02 20:01:55.282693 zuko-0.3.0/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1001)     4648 2023-08-02 20:00:36.000000 zuko-0.3.0/README.md
--rw-rw-r--   0 francois  (1001) francois  (1001)       28 2023-07-09 09:28:21.000000 zuko-0.3.0/requirements.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)      823 2023-08-02 20:01:55.282693 zuko-0.3.0/setup.cfg
--rw-rw-r--   0 francois  (1001) francois  (1001)       72 2023-07-09 09:28:21.000000 zuko-0.3.0/setup.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-08-02 20:01:55.278693 zuko-0.3.0/tests/
--rw-rw-r--   0 francois  (1001) francois  (1001)     1550 2023-07-09 09:28:21.000000 zuko-0.3.0/tests/test_distributions.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     2966 2023-08-02 20:00:36.000000 zuko-0.3.0/tests/test_flows.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     1138 2023-07-09 09:28:21.000000 zuko-0.3.0/tests/test_nn.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     3167 2023-08-02 20:00:36.000000 zuko-0.3.0/tests/test_transforms.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     2792 2023-07-13 11:22:12.000000 zuko-0.3.0/tests/test_utils.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-08-02 20:01:55.278693 zuko-0.3.0/zuko/
--rw-rw-r--   0 francois  (1001) francois  (1001)      177 2023-08-02 20:01:09.000000 zuko-0.3.0/zuko/__init__.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    20790 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/distributions.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-08-02 20:01:55.282693 zuko-0.3.0/zuko/flows/
--rw-rw-r--   0 francois  (1001) francois  (1001)      273 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/__init__.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     7482 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/autoregressive.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     3959 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/continuous.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     4057 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/core.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     4964 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/coupling.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     4199 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/gaussianization.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     1989 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/mixture.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     9948 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/neural.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     1359 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/polynomial.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     3060 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/spline.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     9073 2023-07-13 20:10:54.000000 zuko-0.3.0/zuko/nn.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    28089 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/transforms.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    13559 2023-08-01 12:27:42.000000 zuko-0.3.0/zuko/utils.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-08-02 20:01:55.282693 zuko-0.3.0/zuko.egg-info/
--rw-rw-r--   0 francois  (1001) francois  (1001)     5377 2023-08-02 20:01:55.000000 zuko-0.3.0/zuko.egg-info/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1001)      623 2023-08-02 20:01:55.000000 zuko-0.3.0/zuko.egg-info/SOURCES.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-08-02 20:01:55.000000 zuko-0.3.0/zuko.egg-info/dependency_links.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)       28 2023-08-02 20:01:55.000000 zuko-0.3.0/zuko.egg-info/requires.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)        5 2023-08-02 20:01:55.000000 zuko-0.3.0/zuko.egg-info/top_level.txt
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-08-08 17:41:20.322286 zuko-0.3.1/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2022-12-13 12:43:25.000000 zuko-0.3.1/LICENSE
+-rw-rw-r--   0 francois  (1001) francois  (1001)     5309 2023-08-08 17:41:20.322286 zuko-0.3.1/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4580 2023-08-08 17:38:40.000000 zuko-0.3.1/README.md
+-rw-rw-r--   0 francois  (1001) francois  (1001)       28 2023-07-09 09:28:21.000000 zuko-0.3.1/requirements.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)      823 2023-08-08 17:41:20.322286 zuko-0.3.1/setup.cfg
+-rw-rw-r--   0 francois  (1001) francois  (1001)       72 2023-07-09 09:28:21.000000 zuko-0.3.1/setup.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-08-08 17:41:20.322286 zuko-0.3.1/tests/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1550 2023-07-09 09:28:21.000000 zuko-0.3.1/tests/test_distributions.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2966 2023-08-02 20:00:36.000000 zuko-0.3.1/tests/test_flows.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1138 2023-07-09 09:28:21.000000 zuko-0.3.1/tests/test_nn.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     3167 2023-08-02 20:00:36.000000 zuko-0.3.1/tests/test_transforms.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2792 2023-07-13 11:22:12.000000 zuko-0.3.1/tests/test_utils.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-08-08 17:41:20.322286 zuko-0.3.1/zuko/
+-rw-rw-r--   0 francois  (1001) francois  (1001)      177 2023-08-08 17:41:04.000000 zuko-0.3.1/zuko/__init__.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    20790 2023-08-02 20:00:36.000000 zuko-0.3.1/zuko/distributions.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-08-08 17:41:20.322286 zuko-0.3.1/zuko/flows/
+-rw-rw-r--   0 francois  (1001) francois  (1001)      273 2023-08-02 20:00:36.000000 zuko-0.3.1/zuko/flows/__init__.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     7476 2023-08-08 17:38:40.000000 zuko-0.3.1/zuko/flows/autoregressive.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     3953 2023-08-08 17:38:40.000000 zuko-0.3.1/zuko/flows/continuous.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4094 2023-08-08 17:38:40.000000 zuko-0.3.1/zuko/flows/core.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4958 2023-08-08 17:38:40.000000 zuko-0.3.1/zuko/flows/coupling.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4200 2023-08-08 17:38:40.000000 zuko-0.3.1/zuko/flows/gaussianization.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1986 2023-08-08 17:38:40.000000 zuko-0.3.1/zuko/flows/mixture.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     9941 2023-08-08 17:38:40.000000 zuko-0.3.1/zuko/flows/neural.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1359 2023-08-02 20:00:36.000000 zuko-0.3.1/zuko/flows/polynomial.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     3060 2023-08-02 20:00:36.000000 zuko-0.3.1/zuko/flows/spline.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     9073 2023-07-13 20:10:54.000000 zuko-0.3.1/zuko/nn.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    28089 2023-08-02 20:00:36.000000 zuko-0.3.1/zuko/transforms.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    13559 2023-08-01 12:27:42.000000 zuko-0.3.1/zuko/utils.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-08-08 17:41:20.322286 zuko-0.3.1/zuko.egg-info/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     5309 2023-08-08 17:41:20.000000 zuko-0.3.1/zuko.egg-info/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)      623 2023-08-08 17:41:20.000000 zuko-0.3.1/zuko.egg-info/SOURCES.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-08-08 17:41:20.000000 zuko-0.3.1/zuko.egg-info/dependency_links.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)       28 2023-08-08 17:41:20.000000 zuko-0.3.1/zuko.egg-info/requires.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        5 2023-08-08 17:41:20.000000 zuko-0.3.1/zuko.egg-info/top_level.txt
```

### Comparing `zuko-0.3.0/LICENSE` & `zuko-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zuko-0.3.0/PKG-INFO` & `zuko-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zuko
-Version: 0.3.0
+Version: 0.3.1
 Summary: Normalizing flows in PyTorch
 Author: François Rozet
 Author-email: francois.rozet@outlook.com
 Project-URL: Documentation, https://zuko.readthedocs.io
 Project-URL: Source, https://github.com/francois-rozet/zuko
 Project-URL: Tracker, https://github.com/francois-rozet/zuko/issues
 Keywords: torch,normalizing flows,probability,density,generative,deep learning
@@ -19,15 +19,15 @@
 
 ![Zuko's banner](https://raw.githubusercontent.com/francois-rozet/zuko/master/docs/images/banner.svg)
 
 # Zuko - Normalizing flows in PyTorch
 
 Zuko is a Python package that implements normalizing flows in [PyTorch](https://pytorch.org). It relies as much as possible on distributions and transformations already provided by PyTorch. Unfortunately, the `Distribution` and `Transform` classes of `torch` are not sub-classes of `torch.nn.Module`, which means you cannot send their internal tensors to GPU with `.to('cuda')` or retrieve their parameters with `.parameters()`. Worse, the concepts of conditional distribution and transformation, which are essential for probabilistic inference, are impossible to express.
 
-To solve these problems, `zuko` defines two abstract modules, `DistributionFactory` and `TransformFactory`, which represent parameterized recipes for building distributions and transformations, respectively. To condition a distribution or transformation simply means to consider the condition/context as part of the recipe, similar to [Pyro](http://pyro.ai)'s `ConditionalTransformModule`. A normalizing flow is a special `DistributionFactory` that contains a sequence of `TransformFactory` and a base `DistributionFactory`. This design enables flows to act like distributions while retaining features inherent to modules, such as trainable parameters. It also makes the implementations easier to understand and extend.
+To solve these problems, `zuko` defines two concepts: the `LazyDistribution` and `LazyTransform`, which are any modules whose forward pass returns a `Distribution` or `Transform`, respectively. Because the creation of the actual distribution/transformation is delayed, an eventual condition can be easily taken into account. Then, a normalizing flow is a special `LazyDistribution` that contains a sequence of `LazyTransform` and a base `LazyDistribution`. This design enables flows to act like distributions while retaining features inherent to modules, such as trainable parameters. It also makes the implementations easier to understand and extend.
 
 > In the [Avatar](https://wikipedia.org/wiki/Avatar:_The_Last_Airbender) cartoon, [Zuko](https://wikipedia.org/wiki/Zuko) is a powerful firebender 🔥
 
 ## Installation
 
 The `zuko` package is available on [PyPI](https://pypi.org/project/zuko), which means it is installable via `pip`.
```

### Comparing `zuko-0.3.0/README.md` & `zuko-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ![Zuko's banner](https://raw.githubusercontent.com/francois-rozet/zuko/master/docs/images/banner.svg)
 
 # Zuko - Normalizing flows in PyTorch
 
 Zuko is a Python package that implements normalizing flows in [PyTorch](https://pytorch.org). It relies as much as possible on distributions and transformations already provided by PyTorch. Unfortunately, the `Distribution` and `Transform` classes of `torch` are not sub-classes of `torch.nn.Module`, which means you cannot send their internal tensors to GPU with `.to('cuda')` or retrieve their parameters with `.parameters()`. Worse, the concepts of conditional distribution and transformation, which are essential for probabilistic inference, are impossible to express.
 
-To solve these problems, `zuko` defines two abstract modules, `DistributionFactory` and `TransformFactory`, which represent parameterized recipes for building distributions and transformations, respectively. To condition a distribution or transformation simply means to consider the condition/context as part of the recipe, similar to [Pyro](http://pyro.ai)'s `ConditionalTransformModule`. A normalizing flow is a special `DistributionFactory` that contains a sequence of `TransformFactory` and a base `DistributionFactory`. This design enables flows to act like distributions while retaining features inherent to modules, such as trainable parameters. It also makes the implementations easier to understand and extend.
+To solve these problems, `zuko` defines two concepts: the `LazyDistribution` and `LazyTransform`, which are any modules whose forward pass returns a `Distribution` or `Transform`, respectively. Because the creation of the actual distribution/transformation is delayed, an eventual condition can be easily taken into account. Then, a normalizing flow is a special `LazyDistribution` that contains a sequence of `LazyTransform` and a base `LazyDistribution`. This design enables flows to act like distributions while retaining features inherent to modules, such as trainable parameters. It also makes the implementations easier to understand and extend.
 
 > In the [Avatar](https://wikipedia.org/wiki/Avatar:_The_Last_Airbender) cartoon, [Zuko](https://wikipedia.org/wiki/Zuko) is a powerful firebender 🔥
 
 ## Installation
 
 The `zuko` package is available on [PyPI](https://pypi.org/project/zuko), which means it is installable via `pip`.
```

### Comparing `zuko-0.3.0/setup.cfg` & `zuko-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `zuko-0.3.0/tests/test_distributions.py` & `zuko-0.3.1/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `zuko-0.3.0/tests/test_flows.py` & `zuko-0.3.1/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `zuko-0.3.0/tests/test_nn.py` & `zuko-0.3.1/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `zuko-0.3.0/tests/test_transforms.py` & `zuko-0.3.1/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `zuko-0.3.0/tests/test_utils.py` & `zuko-0.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zuko-0.3.0/zuko/distributions.py` & `zuko-0.3.1/zuko/distributions.py`

 * *Files identical despite different names*

### Comparing `zuko-0.3.0/zuko/flows/autoregressive.py` & `zuko-0.3.1/zuko/flows/autoregressive.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from .core import *
 from ..distributions import DiagNormal
 from ..transforms import *
 from ..nn import MaskedMLP
 from ..utils import broadcast, unpack
 
 
-class MaskedAutoregressiveTransform(TransformFactory):
-    r"""Creates a masked autoregressive transformation factory.
+class MaskedAutoregressiveTransform(LazyTransform):
+    r"""Creates a lazy masked autoregressive transformation.
 
     See also:
         :class:`zuko.transforms.AutoregressiveTransform`
 
     References:
         | Masked Autoregressive Flow for Density Estimation (Papamakarios et al., 2017)
         | https://arxiv.org/abs/1705.07057
```

### Comparing `zuko-0.3.0/zuko/flows/continuous.py` & `zuko-0.3.1/zuko/flows/continuous.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from .core import *
 from ..distributions import DiagNormal
 from ..transforms import FreeFormJacobianTransform
 from ..nn import MLP
 from ..utils import broadcast
 
 
-class FFJTransform(TransformFactory):
-    r"""Creates a free-form Jacobian (FFJ) transformation factory.
+class FFJTransform(LazyTransform):
+    r"""Creates a lazy free-form Jacobian (FFJ) transformation.
 
     See also:
         :class:`zuko.transforms.FreeFormJacobianTransform`
 
     References:
         | FFJORD: Free-form Continuous Dynamics for Scalable Reversible Generative Models (Grathwohl et al., 2018)
         | https://arxiv.org/abs/1810.01367
```

### Comparing `zuko-0.3.0/zuko/flows/core.py` & `zuko-0.3.1/zuko/flows/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 r"""Core building blocks."""
 
 __all__ = [
-    'DistributionFactory',
-    'TransformFactory',
+    'LazyDistribution',
+    'LazyTransform',
     'Flow',
     'Unconditional',
 ]
 
 import abc
 import torch
 import torch.nn as nn
@@ -15,66 +15,69 @@
 from torch.distributions import Distribution, Transform
 from typing import *
 
 from ..distributions import NormalizingFlow
 from ..transforms import ComposedTransform
 
 
-class DistributionFactory(nn.Module, abc.ABC):
-    r"""Abstract distribution factory.
+class LazyDistribution(nn.Module, abc.ABC):
+    r"""Abstract lazy distribution.
 
-    A distribution factory is a module that builds and returns a distribution
+    A lazy distribution is a module that builds and returns a distribution
     :math:`p(X | c)` within its forward pass, given a context :math:`c`.
     """
 
     @abc.abstractmethod
-    def forward(self, c: Tensor = None) -> Distribution:
+    def forward(self, c: Any = None) -> Distribution:
         r"""
         Arguments:
             c: A context :math:`c`.
 
         Returns:
             A distribution :math:`p(X | c)`.
         """
 
         pass
 
 
-class TransformFactory(nn.Module, abc.ABC):
-    r"""Abstract transformation factory.
+class LazyTransform(nn.Module, abc.ABC):
+    r"""Abstract lazy transformation.
 
-    A transformation factory is a module that builds and returns a transformation
+    A lazy transformation is a module that builds and returns a transformation
     :math:`y = f(x | c)` within its forward pass, given a context :math:`c`.
     """
 
     @abc.abstractmethod
-    def forward(self, c: Tensor = None) -> Transform:
+    def forward(self, c: Any = None) -> Transform:
         r"""
         Arguments:
             c: A context :math:`c`.
 
         Returns:
             A transformation :math:`y = f(x | c)`.
         """
 
         pass
 
 
-class Flow(DistributionFactory):
-    r"""Creates a normalizing flow factory.
+class Flow(LazyDistribution):
+    r"""Creates a lazy normalizing flow.
+
+    See also:
+        :class:`zuko.distributions.NormalizingFlow`
 
     Arguments:
-        transforms: A list of transformation factories.
-        base: A distribution factory.
+        transforms: A sequence of lazy transformations.
+        base: A lazy distribution.
     """
 
     def __init__(
         self,
-        transforms: Sequence[TransformFactory],
-        base: DistributionFactory,
+        transforms: Sequence[LazyTransform],
+        base: LazyDistribution,
     ):
         super().__init__()
 
         self.transforms = nn.ModuleList(transforms)
         self.base = base
 
     def forward(self, c: Tensor = None) -> NormalizingFlow:
@@ -93,24 +96,24 @@
         else:
             base = self.base(c).expand(c.shape[:-1])
 
         return NormalizingFlow(transform, base)
 
 
 class Unconditional(nn.Module):
-    r"""Creates an unconditional factory from a recipe.
+    r"""Creates an unconditional lazy module from a constructor.
 
-    Typically, the recipe returns a distribution or transformation. The positional
-    arguments of the recipe are registered as buffers or parameters.
+    Typically, the constructor returns a distribution or transformation. The positional
+    arguments of the constructor are registered as buffers or parameters.
 
     Arguments:
-        recipe: An arbitrary function.
-        args: The positional tensor arguments passed to `recipe`.
+        meta: An arbitrary constructor function.
+        args: The positional tensor arguments passed to `meta`.
         buffer: Whether tensors are registered as buffers or parameters.
-        kwargs: The keyword arguments passed to `recipe`.
+        kwargs: The keyword arguments passed to `meta`.
 
     Examples:
         >>> mu, sigma = torch.zeros(3), torch.ones(3)
         >>> d = Unconditional(DiagNormal, mu, sigma, buffer=True)
         >>> d()
         DiagNormal(loc: torch.Size([3]), scale: torch.Size([3]))
         >>> d().sample()
@@ -122,22 +125,22 @@
         >>> x = torch.randn(3)
         >>> t()(x)
         tensor([0.5523, 0.7997, 0.9189])
     """
 
     def __init__(
         self,
-        recipe: Callable[..., Any],
+        meta: Callable[..., Any],
         *args: Tensor,
         buffer: bool = False,
         **kwargs,
     ):
         super().__init__()
 
-        self.recipe = recipe
+        self.meta = meta
 
         for i, arg in enumerate(args):
             if buffer:
                 self.register_buffer(f'_{i}', arg)
             else:
                 self.register_parameter(f'_{i}', nn.Parameter(arg))
 
@@ -148,15 +151,15 @@
 
     def forward(self, c: Tensor = None) -> Any:
         r"""
         Arguments:
             c: A context :math:`c`. This argument is always ignored.
 
         Returns:
-            :py:`recipe(*args, **kwargs)`
+            :py:`meta(*args, **kwargs)`
         """
 
-        return self.recipe(
+        return self.meta(
             *self._parameters.values(),
             *self._buffers.values(),
             **self.kwargs,
         )
```

### Comparing `zuko-0.3.0/zuko/flows/coupling.py` & `zuko-0.3.1/zuko/flows/coupling.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from .core import *
 from ..distributions import DiagNormal
 from ..transforms import *
 from ..nn import MLP
 from ..utils import broadcast, unpack
 
 
-class GeneralCouplingTransform(TransformFactory):
-    r"""Creates a general coupling transformation factory.
+class GeneralCouplingTransform(LazyTransform):
+    r"""Creates a lazy general coupling transformation.
 
     See also:
         :class:`zuko.transforms.CouplingTransform`
 
     References:
         | NICE: Non-linear Independent Components Estimation (Dinh et al., 2014)
         | https://arxiv.org/abs/1410.8516
```

### Comparing `zuko-0.3.0/zuko/flows/gaussianization.py` & `zuko-0.3.1/zuko/flows/gaussianization.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from .core import *
 from ..distributions import DiagNormal
 from ..transforms import *
 from ..nn import MLP
 from ..utils import unpack
 
 
-class ElementWiseTransform(TransformFactory):
-    r"""Creates an element-wise transformation.
+class ElementWiseTransform(LazyTransform):
+    r"""Creates a lazy element-wise transformation.
 
     Arguments:
         features: The number of features.
         context: The number of context features.
         univariate: The univariate transformation constructor.
         shapes: The shapes of the univariate transformation parameters.
         kwargs: Keyword arguments passed to :class:`zuko.nn.MLP`.
```

### Comparing `zuko-0.3.0/zuko/flows/mixture.py` & `zuko-0.3.1/zuko/flows/mixture.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from .core import *
 from ..distributions import Mixture
 from ..nn import MLP
 from ..utils import unpack
 
 
-class GMM(DistributionFactory):
+class GMM(LazyDistribution):
     r"""Creates a Gaussian mixture model (GMM).
 
     .. math:: p(X | c) = \sum_{i = 1}^K w_i(c) \, \mathcal{N}(X | \mu_i(c), \Sigma_i(c))
 
     Wikipedia:
         https://wikipedia.org/wiki/Mixture_model#Gaussian_mixture_model
```

### Comparing `zuko-0.3.0/zuko/flows/neural.py` & `zuko-0.3.1/zuko/flows/neural.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from ..distributions import DiagNormal
 from ..transforms import MonotonicTransform, UnconstrainedMonotonicTransform
 from ..nn import MLP, MonotonicMLP
 from ..utils import broadcast
 
 
 class NeuralAutoregressiveTransform(MaskedAutoregressiveTransform):
-    r"""Creates a neural autoregressive transformation factory.
+    r"""Creates a lazy neural autoregressive transformation.
 
     The monotonic neural network is parametrized by its internal positive weights,
     which are independent of the features and context. To modulate its behavior, it
     receives as input a signal that is autoregressively dependent on the features
     and context.
 
     See also:
@@ -158,15 +158,15 @@
             buffer=True,
         )
 
         super().__init__(transforms, base)
 
 
 class UnconstrainedNeuralAutoregressiveTransform(MaskedAutoregressiveTransform):
-    r"""Creates an unconstrained neural autoregressive transformation factory.
+    r"""Creates a lazy unconstrained neural autoregressive transformation.
 
     The integrand neural network is parametrized by its internal weights, which are
     independent of the features and context. To modulate its behavior, it receives as
     input a signal that is autoregressively dependent on the features and context. The
     integration constant has the same dependencies as the signal.
 
     See also:
```

### Comparing `zuko-0.3.0/zuko/flows/polynomial.py` & `zuko-0.3.1/zuko/flows/polynomial.py`

 * *Files identical despite different names*

### Comparing `zuko-0.3.0/zuko/flows/spline.py` & `zuko-0.3.1/zuko/flows/spline.py`

 * *Files identical despite different names*

### Comparing `zuko-0.3.0/zuko/nn.py` & `zuko-0.3.1/zuko/nn.py`

 * *Files identical despite different names*

### Comparing `zuko-0.3.0/zuko/transforms.py` & `zuko-0.3.1/zuko/transforms.py`

 * *Files identical despite different names*

### Comparing `zuko-0.3.0/zuko/utils.py` & `zuko-0.3.1/zuko/utils.py`

 * *Files identical despite different names*

### Comparing `zuko-0.3.0/zuko.egg-info/PKG-INFO` & `zuko-0.3.1/zuko.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zuko
-Version: 0.3.0
+Version: 0.3.1
 Summary: Normalizing flows in PyTorch
 Author: François Rozet
 Author-email: francois.rozet@outlook.com
 Project-URL: Documentation, https://zuko.readthedocs.io
 Project-URL: Source, https://github.com/francois-rozet/zuko
 Project-URL: Tracker, https://github.com/francois-rozet/zuko/issues
 Keywords: torch,normalizing flows,probability,density,generative,deep learning
@@ -19,15 +19,15 @@
 
 ![Zuko's banner](https://raw.githubusercontent.com/francois-rozet/zuko/master/docs/images/banner.svg)
 
 # Zuko - Normalizing flows in PyTorch
 
 Zuko is a Python package that implements normalizing flows in [PyTorch](https://pytorch.org). It relies as much as possible on distributions and transformations already provided by PyTorch. Unfortunately, the `Distribution` and `Transform` classes of `torch` are not sub-classes of `torch.nn.Module`, which means you cannot send their internal tensors to GPU with `.to('cuda')` or retrieve their parameters with `.parameters()`. Worse, the concepts of conditional distribution and transformation, which are essential for probabilistic inference, are impossible to express.
 
-To solve these problems, `zuko` defines two abstract modules, `DistributionFactory` and `TransformFactory`, which represent parameterized recipes for building distributions and transformations, respectively. To condition a distribution or transformation simply means to consider the condition/context as part of the recipe, similar to [Pyro](http://pyro.ai)'s `ConditionalTransformModule`. A normalizing flow is a special `DistributionFactory` that contains a sequence of `TransformFactory` and a base `DistributionFactory`. This design enables flows to act like distributions while retaining features inherent to modules, such as trainable parameters. It also makes the implementations easier to understand and extend.
+To solve these problems, `zuko` defines two concepts: the `LazyDistribution` and `LazyTransform`, which are any modules whose forward pass returns a `Distribution` or `Transform`, respectively. Because the creation of the actual distribution/transformation is delayed, an eventual condition can be easily taken into account. Then, a normalizing flow is a special `LazyDistribution` that contains a sequence of `LazyTransform` and a base `LazyDistribution`. This design enables flows to act like distributions while retaining features inherent to modules, such as trainable parameters. It also makes the implementations easier to understand and extend.
 
 > In the [Avatar](https://wikipedia.org/wiki/Avatar:_The_Last_Airbender) cartoon, [Zuko](https://wikipedia.org/wiki/Zuko) is a powerful firebender 🔥
 
 ## Installation
 
 The `zuko` package is available on [PyPI](https://pypi.org/project/zuko), which means it is installable via `pip`.
```

### Comparing `zuko-0.3.0/zuko.egg-info/SOURCES.txt` & `zuko-0.3.1/zuko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

