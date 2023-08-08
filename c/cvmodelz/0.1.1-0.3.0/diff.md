# Comparing `tmp/cvmodelz-0.1.1.tar.gz` & `tmp/cvmodelz-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cvmodelz-0.1.1.tar", last modified: Tue May 25 09:56:10 2021, max compression
+gzip compressed data, was "cvmodelz-0.3.0.tar", last modified: Tue Aug  8 07:42:06 2023, max compression
```

## Comparing `cvmodelz-0.1.1.tar` & `cvmodelz-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,54 @@
-drwxr-xr-x   0 dima      (1000) users      (100)        0 2021-05-25 09:56:10.983477 cvmodelz-0.1.1/
--rw-r--r--   0 dima      (1000) users      (100)      319 2021-05-25 09:56:10.983477 cvmodelz-0.1.1/PKG-INFO
--rw-r--r--   0 dima      (1000) users      (100)       95 2021-04-23 07:02:57.000000 cvmodelz-0.1.1/README.md
-drwxr-xr-x   0 dima      (1000) users      (100)        0 2021-05-25 09:56:10.979477 cvmodelz-0.1.1/cvmodelz/
--rw-r--r--   0 dima      (1000) users      (100)      229 2021-04-23 08:08:47.000000 cvmodelz-0.1.1/cvmodelz/__init__.py
--rw-r--r--   0 dima      (1000) users      (100)       20 2021-04-28 11:58:12.000000 cvmodelz-0.1.1/cvmodelz/_version.py
-drwxr-xr-x   0 dima      (1000) users      (100)        0 2021-05-25 09:56:10.983477 cvmodelz-0.1.1/cvmodelz/classifiers/
--rw-r--r--   0 dima      (1000) users      (100)      294 2021-04-28 09:06:18.000000 cvmodelz-0.1.1/cvmodelz/classifiers/__init__.py
--rw-r--r--   0 dima      (1000) users      (100)     3179 2021-04-29 10:30:28.000000 cvmodelz-0.1.1/cvmodelz/classifiers/base.py
--rw-r--r--   0 dima      (1000) users      (100)     2033 2021-04-29 13:19:52.000000 cvmodelz-0.1.1/cvmodelz/classifiers/separate_model_classifier.py
--rw-r--r--   0 dima      (1000) users      (100)      523 2021-04-23 12:33:58.000000 cvmodelz-0.1.1/cvmodelz/model_info.py
-drwxr-xr-x   0 dima      (1000) users      (100)        0 2021-05-25 09:56:10.983477 cvmodelz-0.1.1/cvmodelz/models/
--rw-r--r--   0 dima      (1000) users      (100)      566 2021-04-23 12:10:58.000000 cvmodelz-0.1.1/cvmodelz/models/__init__.py
--rw-r--r--   0 dima      (1000) users      (100)     3363 2021-04-29 13:34:28.000000 cvmodelz-0.1.1/cvmodelz/models/base.py
--rw-r--r--   0 dima      (1000) users      (100)     2398 2021-04-27 17:01:23.000000 cvmodelz-0.1.1/cvmodelz/models/factory.py
--rw-r--r--   0 dima      (1000) users      (100)      694 2021-04-28 11:54:13.000000 cvmodelz-0.1.1/cvmodelz/models/meta_info.py
-drwxr-xr-x   0 dima      (1000) users      (100)        0 2021-05-25 09:56:10.983477 cvmodelz-0.1.1/cvmodelz/models/pretrained/
--rw-r--r--   0 dima      (1000) users      (100)      580 2021-04-27 11:06:07.000000 cvmodelz-0.1.1/cvmodelz/models/pretrained/__init__.py
--rw-r--r--   0 dima      (1000) users      (100)     1400 2021-04-28 09:34:01.000000 cvmodelz-0.1.1/cvmodelz/models/pretrained/base.py
-drwxr-xr-x   0 dima      (1000) users      (100)        0 2021-05-25 09:56:10.983477 cvmodelz-0.1.1/cvmodelz/models/pretrained/inception/
--rw-r--r--   0 dima      (1000) users      (100)      106 2021-04-27 11:06:28.000000 cvmodelz-0.1.1/cvmodelz/models/pretrained/inception/__init__.py
--rw-r--r--   0 dima      (1000) users      (100)     6177 2021-04-28 09:34:13.000000 cvmodelz-0.1.1/cvmodelz/models/pretrained/inception/blocks.py
--rw-r--r--   0 dima      (1000) users      (100)     8223 2021-04-28 13:02:15.000000 cvmodelz-0.1.1/cvmodelz/models/pretrained/inception/inception_v3.py
--rw-r--r--   0 dima      (1000) users      (100)    21479 2021-04-28 16:03:48.000000 cvmodelz-0.1.1/cvmodelz/models/pretrained/inception/link_mappings.py
--rw-r--r--   0 dima      (1000) users      (100)     2328 2021-04-28 11:55:24.000000 cvmodelz-0.1.1/cvmodelz/models/pretrained/resnet.py
--rw-r--r--   0 dima      (1000) users      (100)      959 2021-04-28 13:20:52.000000 cvmodelz-0.1.1/cvmodelz/models/pretrained/vgg.py
--rw-r--r--   0 dima      (1000) users      (100)     2014 2021-04-28 09:35:02.000000 cvmodelz-0.1.1/cvmodelz/models/wrapper.py
-drwxr-xr-x   0 dima      (1000) users      (100)        0 2021-05-25 09:56:10.983477 cvmodelz-0.1.1/cvmodelz/utils/
--rw-r--r--   0 dima      (1000) users      (100)     2240 2021-04-23 13:00:40.000000 cvmodelz-0.1.1/cvmodelz/utils/__init__.py
-drwxr-xr-x   0 dima      (1000) users      (100)        0 2021-05-25 09:56:10.983477 cvmodelz-0.1.1/cvmodelz.egg-info/
--rw-r--r--   0 dima      (1000) users      (100)      319 2021-05-25 09:56:10.000000 cvmodelz-0.1.1/cvmodelz.egg-info/PKG-INFO
--rw-r--r--   0 dima      (1000) users      (100)      912 2021-05-25 09:56:10.000000 cvmodelz-0.1.1/cvmodelz.egg-info/SOURCES.txt
--rw-r--r--   0 dima      (1000) users      (100)        1 2021-05-25 09:56:10.000000 cvmodelz-0.1.1/cvmodelz.egg-info/dependency_links.txt
--rw-r--r--   0 dima      (1000) users      (100)        1 2021-04-23 15:30:23.000000 cvmodelz-0.1.1/cvmodelz.egg-info/not-zip-safe
--rw-r--r--   0 dima      (1000) users      (100)       87 2021-05-25 09:56:10.000000 cvmodelz-0.1.1/cvmodelz.egg-info/requires.txt
--rw-r--r--   0 dima      (1000) users      (100)        9 2021-05-25 09:56:10.000000 cvmodelz-0.1.1/cvmodelz.egg-info/top_level.txt
--rw-r--r--   0 dima      (1000) users      (100)       89 2021-05-25 09:36:27.000000 cvmodelz-0.1.1/requirements.txt
--rw-r--r--   0 dima      (1000) users      (100)       38 2021-05-25 09:56:10.983477 cvmodelz-0.1.1/setup.cfg
--rwxr-xr-x   0 dima      (1000) users      (100)     1046 2021-04-23 07:09:21.000000 cvmodelz-0.1.1/setup.py
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2023-08-08 07:42:06.014013 cvmodelz-0.3.0/
+-rw-r--r--   0 korsch   (10001) users    (10000)      308 2023-08-08 07:42:06.014013 cvmodelz-0.3.0/PKG-INFO
+-rw-r--r--   0 korsch   (10001) users    (10000)       95 2021-04-28 16:28:41.000000 cvmodelz-0.3.0/README.md
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2023-08-08 07:42:06.014013 cvmodelz-0.3.0/cvmodelz/
+-rw-r--r--   0 korsch   (10001) users    (10000)      229 2021-04-28 16:28:41.000000 cvmodelz-0.3.0/cvmodelz/__init__.py
+-rw-r--r--   0 korsch   (10001) users    (10000)       20 2023-03-23 08:29:22.000000 cvmodelz-0.3.0/cvmodelz/_version.py
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2023-08-08 07:42:06.014013 cvmodelz-0.3.0/cvmodelz/classifiers/
+-rw-r--r--   0 korsch   (10001) users    (10000)      294 2021-04-28 16:28:41.000000 cvmodelz-0.3.0/cvmodelz/classifiers/__init__.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     3298 2023-01-31 10:44:31.000000 cvmodelz-0.3.0/cvmodelz/classifiers/base.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     2163 2021-05-26 12:29:05.000000 cvmodelz-0.3.0/cvmodelz/classifiers/separate_model_classifier.py
+-rw-r--r--   0 korsch   (10001) users    (10000)      668 2021-11-09 12:56:23.000000 cvmodelz-0.3.0/cvmodelz/model_info.py
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2023-08-08 07:42:06.014013 cvmodelz-0.3.0/cvmodelz/models/
+-rw-r--r--   0 korsch   (10001) users    (10000)      696 2022-04-06 11:49:56.000000 cvmodelz-0.3.0/cvmodelz/models/__init__.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     3364 2023-03-23 08:30:29.000000 cvmodelz-0.3.0/cvmodelz/models/base.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     2767 2022-08-31 15:08:28.000000 cvmodelz-0.3.0/cvmodelz/models/factory.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     1013 2023-03-23 08:35:11.000000 cvmodelz-0.3.0/cvmodelz/models/meta_info.py
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2023-08-08 07:42:06.014013 cvmodelz-0.3.0/cvmodelz/models/pretrained/
+-rw-r--r--   0 korsch   (10001) users    (10000)      805 2022-04-06 11:49:45.000000 cvmodelz-0.3.0/cvmodelz/models/pretrained/__init__.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     1341 2023-03-23 08:30:48.000000 cvmodelz-0.3.0/cvmodelz/models/pretrained/base.py
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2023-08-08 07:42:06.014013 cvmodelz-0.3.0/cvmodelz/models/pretrained/inception/
+-rw-r--r--   0 korsch   (10001) users    (10000)      203 2022-04-06 10:13:11.000000 cvmodelz-0.3.0/cvmodelz/models/pretrained/inception/__init__.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     6177 2023-03-23 08:28:51.000000 cvmodelz-0.3.0/cvmodelz/models/pretrained/inception/blocks.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     8234 2023-03-23 08:32:30.000000 cvmodelz-0.3.0/cvmodelz/models/pretrained/inception/inception_v3.py
+-rw-r--r--   0 korsch   (10001) users    (10000)      800 2022-04-06 10:23:05.000000 cvmodelz-0.3.0/cvmodelz/models/pretrained/inception/inception_v3_hd.py
+-rw-r--r--   0 korsch   (10001) users    (10000)    21479 2021-04-28 16:28:41.000000 cvmodelz-0.3.0/cvmodelz/models/pretrained/inception/link_mappings.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     2869 2022-04-06 12:28:51.000000 cvmodelz-0.3.0/cvmodelz/models/pretrained/resnet.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     1124 2022-08-29 08:46:11.000000 cvmodelz-0.3.0/cvmodelz/models/pretrained/vgg.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     2443 2023-03-23 08:35:01.000000 cvmodelz-0.3.0/cvmodelz/models/wrapper.py
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2023-08-08 07:42:06.014013 cvmodelz-0.3.0/cvmodelz/utils/
+-rw-r--r--   0 korsch   (10001) users    (10000)     2499 2022-04-06 09:50:43.000000 cvmodelz-0.3.0/cvmodelz/utils/__init__.py
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2023-08-08 07:42:06.014013 cvmodelz-0.3.0/cvmodelz/utils/functions/
+-rw-r--r--   0 korsch   (10001) users    (10000)      286 2023-03-23 08:31:59.000000 cvmodelz-0.3.0/cvmodelz/utils/functions/__init__.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     1407 2023-03-23 08:21:26.000000 cvmodelz-0.3.0/cvmodelz/utils/functions/alpha_product.py
+-rw-r--r--   0 korsch   (10001) users    (10000)      755 2023-03-23 08:21:54.000000 cvmodelz-0.3.0/cvmodelz/utils/functions/signed_square_root.py
+-rw-r--r--   0 korsch   (10001) users    (10000)      910 2023-03-23 08:27:11.000000 cvmodelz-0.3.0/cvmodelz/utils/functions/tf_average.py
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2023-08-08 07:42:06.014013 cvmodelz-0.3.0/cvmodelz/utils/links/
+-rw-r--r--   0 korsch   (10001) users    (10000)      656 2023-03-23 08:28:08.000000 cvmodelz-0.3.0/cvmodelz/utils/links/__init__.py
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2023-08-08 07:42:06.014013 cvmodelz-0.3.0/cvmodelz/utils/links/pooling/
+-rw-r--r--   0 korsch   (10001) users    (10000)     1074 2023-03-23 08:33:05.000000 cvmodelz-0.3.0/cvmodelz/utils/links/pooling/__init__.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     1064 2023-03-23 08:18:57.000000 cvmodelz-0.3.0/cvmodelz/utils/links/pooling/alpha_pooling.py
+-rw-r--r--   0 korsch   (10001) users    (10000)     2235 2023-03-23 08:19:08.000000 cvmodelz-0.3.0/cvmodelz/utils/links/pooling/compact_bilinear.py
+-rw-r--r--   0 korsch   (10001) users    (10000)      378 2023-03-23 08:16:17.000000 cvmodelz-0.3.0/cvmodelz/utils/links/pooling/global_average.py
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2023-08-08 07:42:06.014013 cvmodelz-0.3.0/cvmodelz.egg-info/
+-rw-r--r--   0 korsch   (10001) users    (10000)      308 2023-08-08 07:42:05.000000 cvmodelz-0.3.0/cvmodelz.egg-info/PKG-INFO
+-rw-r--r--   0 korsch   (10001) users    (10000)     1369 2023-08-08 07:42:05.000000 cvmodelz-0.3.0/cvmodelz.egg-info/SOURCES.txt
+-rw-r--r--   0 korsch   (10001) users    (10000)        1 2023-08-08 07:42:05.000000 cvmodelz-0.3.0/cvmodelz.egg-info/dependency_links.txt
+-rw-r--r--   0 korsch   (10001) users    (10000)        1 2021-06-16 13:35:48.000000 cvmodelz-0.3.0/cvmodelz.egg-info/not-zip-safe
+-rw-r--r--   0 korsch   (10001) users    (10000)       87 2023-08-08 07:42:05.000000 cvmodelz-0.3.0/cvmodelz.egg-info/requires.txt
+-rw-r--r--   0 korsch   (10001) users    (10000)        9 2023-08-08 07:42:05.000000 cvmodelz-0.3.0/cvmodelz.egg-info/top_level.txt
+-rw-r--r--   0 korsch   (10001) users    (10000)       89 2021-11-10 06:33:31.000000 cvmodelz-0.3.0/requirements.txt
+-rw-r--r--   0 korsch   (10001) users    (10000)       38 2023-08-08 07:42:06.014013 cvmodelz-0.3.0/setup.cfg
+-rwxr-xr-x   0 korsch   (10001) users    (10000)     1046 2021-11-10 08:35:47.000000 cvmodelz-0.3.0/setup.py
+drwxr-xr-x   0 korsch   (10001) users    (10000)        0 2023-08-08 07:42:06.014013 cvmodelz-0.3.0/tests/
+-rw-r--r--   0 korsch   (10001) users    (10000)     2089 2021-04-28 16:28:41.000000 cvmodelz-0.3.0/tests/test_utils.py
```

### Comparing `cvmodelz-0.1.1/cvmodelz/classifiers/base.py` & `cvmodelz-0.3.0/cvmodelz/classifiers/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 		if only_head:
 			self.enable_only_head()
 
 	def setup(self, model: BaseModel) -> None:
 		self.model = model
 
 	def report(self, **values) -> None:
-		chainer.report(values, self)
+
+		chainer.report({key: chainer.as_array(val) for key, val in values.items()}, self)
 
 	def enable_only_head(self) -> None:
 		self.model.disable_update()
 		self.model.clf_layer.enable_update()
 
 	@property
 	def n_classes(self) -> int:
@@ -59,28 +60,31 @@
 			(2) Loading from a saved classifier.
 				- All weights are loaded as-it-is from
 				the given file.
 		"""
 
 		try:
 			# Case (2)
-			self.load_classifier(weights_file)
+			return self.load_classifier(weights_file)
 
 		except KeyError as e:
 			pass
 
 		# Case (1)
 		self.load_model(weights_file, n_classes=n_classes, finetune=finetune, **kwargs)
 
 		# else:
 		# 	# Case (0)
 		# 	pass
 
 	def load_classifier(self, weights_file: str):
 
+		if weights_file is None:
+			return
+
 		if isinstance(weights_file, io.BufferedIOBase):
 			assert not weights_file.closed, "The weights file was already closed!"
 			weights_file.seek(0)
 
 		npz.load_npz(weights_file, self, strict=True)
 
 	def get_model_loader(self, finetune: bool = False, model: BaseModel = None):
@@ -100,16 +104,16 @@
 	def feat_size(self) -> int:
 		return self.model.meta.feature_size
 
 	@property
 	def output_size(self) -> int:
 		return self.feat_size
 
-	def loss(self, pred: chainer.Variable, y: chainer.Variable) -> chainer.Variable:
-		return self.model.loss(pred, y, loss_func=self.loss_func)
+	def loss(self, pred: chainer.Variable, y: chainer.Variable, **kwargs) -> chainer.Variable:
+		return self.model.loss(pred, y, loss_func=self.loss_func, **kwargs)
 
 	def evaluations(self, pred: chainer.Variable, y: chainer.Variable) -> Dict[str, chainer.Variable]:
 		return dict(accuracy=self.model.accuracy(pred, y))
 
 	def forward(self, X: chainer.Variable, y: chainer.Variable) -> chainer.Variable:
 		pred = self.model(X, layer_name=self.layer_name)
```

### Comparing `cvmodelz-0.1.1/cvmodelz/classifiers/separate_model_classifier.py` & `cvmodelz-0.3.0/cvmodelz/classifiers/separate_model_classifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,22 +13,26 @@
 class SeparateModelClassifier(Classifier):
 	"""
 		Abstract Classifier, that holds two separate models.
 		The user has to define, how these models operate on the
 		input data. Hence, the forward method is abstract!
 	"""
 
+	def __init__(self, *args, copy_mode="copy", **kwargs):
+		self.copy_mode = copy_mode
+		super().__init__(*args, **kwargs)
+
 	@abc.abstractmethod
 	def forward(self, *args, **kwargs) -> chainer.Variable:
 		super().forward(*args, **kwargs)
 
 	def setup(self, model: BaseModel) -> None:
 		super().setup(model)
 
-		self.separate_model = self.model.copy(mode="copy")
+		self.separate_model = self.model.copy(mode=self.copy_mode)
 
 	def load_model(self, weights_file: str, n_classes: int, *, finetune: bool = False, **kwargs) -> None:
 		for model in [self.model, self.separate_model]:
 			model_loader = self.get_model_loader(finetune=finetune, model=model)
 			kwargs["strict"] = kwargs.get("strict", True)
 			model_loader(weights=weights_file, n_classes=n_classes, **kwargs)
```

### Comparing `cvmodelz-0.1.1/cvmodelz/models/__init__.py` & `cvmodelz-0.3.0/cvmodelz/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from cvmodelz.models.base import BaseModel
 from cvmodelz.models.factory import ModelFactory
 from cvmodelz.models.pretrained import InceptionV3
 from cvmodelz.models.pretrained import ResNet101
 from cvmodelz.models.pretrained import ResNet152
 from cvmodelz.models.pretrained import ResNet35
+from cvmodelz.models.pretrained import ResNet35HD
 from cvmodelz.models.pretrained import ResNet50
+from cvmodelz.models.pretrained import ResNet50HD
 from cvmodelz.models.pretrained import VGG16
 from cvmodelz.models.pretrained import VGG19
 
 __all__ = [
 	"BaseModel",
 	"ModelFactory",
 
 	"InceptionV3",
 
 	"ResNet50",
+	"ResNet50HD",
 	"ResNet35",
+	"ResNet35HD",
 	"ResNet101",
 	"ResNet152",
 
 	"VGG16",
 	"VGG19",
 ]
```

### Comparing `cvmodelz-0.1.1/cvmodelz/models/base.py` & `cvmodelz-0.3.0/cvmodelz/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import io
 import numpy as np
 
 from chainer import functions as F
 from chainer import links as L
 from chainer.initializers import HeNormal
 from chainer.serializers import npz
-from chainer_addons.links.pooling import PoolingType # TODO: replace this!
 from collections import OrderedDict
 from typing import Callable
 
 from cvmodelz import utils
 from cvmodelz.models.meta_info import ModelInfo
+from cvmodelz.utils.links.pooling import PoolingType
 
 class BaseModel(abc.ABC, chainer.Chain):
 
 	def __init__(self, pooling: Callable = PoolingType.G_AVG,
 		input_size=None, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 		self.init_model_info()
@@ -50,16 +50,16 @@
 	def clf_layer_name(self) -> str:
 		return self.meta.classifier_layers[-1]
 
 	@property
 	def clf_layer(self) -> chainer.Link:
 		return utils.get_attr_from_path(self.model_instance, self.clf_layer_name)
 
-	def loss(self, pred, gt, loss_func=F.softmax_cross_entropy):
-		return loss_func(pred, gt)
+	def loss(self, pred, gt, *, loss_func=F.softmax_cross_entropy, **kwargs):
+		return loss_func(pred, gt, **kwargs)
 
 	def accuracy(self, pred, gt):
 		return F.accuracy(pred, gt)
 
 	def reinitialize_clf(self, n_classes, feat_size=None, initializer=None):
 
 		if initializer is None or not callable(initializer):
```

### Comparing `cvmodelz-0.1.1/cvmodelz/models/factory.py` & `cvmodelz-0.3.0/cvmodelz/models/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import abc
 import pyaml
 
 
 from chainer import links as L
 from chainercv2.models import inceptionv3 as cv2inceptionv3
+from chainercv2.models import inceptionresnetv1 as cv2inceptionresnetv1
+from chainercv2.models import resnext as cv2resnext
 from chainercv2.models import resnet as cv2resnet
+from chainercv.links.model import ssd
+from chainercv.links.model import faster_rcnn
 from collections import OrderedDict
 
 from cvmodelz.models import pretrained
 from cvmodelz.models.wrapper import ModelWrapper
 
 class ModelFactory(abc.ABC):
 
@@ -18,34 +22,40 @@
 			L.ResNet101Layers,
 			L.ResNet152Layers,
 			# L.VGG16Layers,
 			# L.VGG19Layers,
 		),
 
 		chainercv=(
-			# todo: chainercv.links.models.ssd
+			ssd.SSD300,
+			faster_rcnn.FasterRCNNVGG16,
 		),
 
 		chainercv2=(
 			cv2resnet.resnet50,
-			# cv2resnet.resnet50b,
+			cv2resnet.resnet18,
 
 			cv2inceptionv3.inceptionv3,
+			cv2inceptionresnetv1.inceptionresnetv1,
+			cv2resnext.resnext50_32x4d,
 		),
 
 		cvmodelz=(
 			pretrained.VGG16,
 			pretrained.VGG19,
 
 			pretrained.ResNet35,
+			pretrained.ResNet35HD,
 			pretrained.ResNet50,
+			pretrained.ResNet50HD,
 			pretrained.ResNet101,
 			pretrained.ResNet152,
 
 			pretrained.InceptionV3,
+			pretrained.InceptionV3HD,
 		),
 	)
 
 	@abc.abstractmethod
 	def __init__(self):
 		raise NotImplementedError("instance creation is not supported!")
```

### Comparing `cvmodelz-0.1.1/cvmodelz/models/pretrained/__init__.py` & `cvmodelz-0.3.0/cvmodelz/models/pretrained/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from cvmodelz.models.pretrained.base import PretrainedModelMixin
 from cvmodelz.models.pretrained.inception import InceptionV3
+from cvmodelz.models.pretrained.inception import InceptionV3HD
 from cvmodelz.models.pretrained.resnet import ResNet101
 from cvmodelz.models.pretrained.resnet import ResNet152
 from cvmodelz.models.pretrained.resnet import ResNet35
+from cvmodelz.models.pretrained.resnet import ResNet35HD
 from cvmodelz.models.pretrained.resnet import ResNet50
+from cvmodelz.models.pretrained.resnet import ResNet50HD
 from cvmodelz.models.pretrained.vgg import VGG16
 from cvmodelz.models.pretrained.vgg import VGG19
 
 
 __all__ = [
 	"PretrainedModelMixin",
 
 	"VGG16",
 	"VGG19",
 
 	"ResNet35",
+	"ResNet35HD",
 	"ResNet50",
+	"ResNet50HD",
 	"ResNet101",
 	"ResNet152",
 
 	"InceptionV3",
+	"InceptionV3HD",
 ]
```

### Comparing `cvmodelz-0.1.1/cvmodelz/models/pretrained/base.py` & `cvmodelz-0.3.0/cvmodelz/models/pretrained/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import abc
 from chainer import links as L
 
 from cvmodelz.models.base import BaseModel
-from cvmodelz.models.meta_info import ModelInfo
 
 class PretrainedModelMixin(BaseModel):
 	"""
 		This mixin is designed to be a superclass besides one of
 		chainer's built in models (VGG, ResNet, GoogLeNet).
 
 		Example:
```

### Comparing `cvmodelz-0.1.1/cvmodelz/models/pretrained/inception/blocks.py` & `cvmodelz-0.3.0/cvmodelz/models/pretrained/inception/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import chainer
 import chainer.functions as F
 import chainer.links as L
 
-from chainer_addons.links import Conv2D_BN
-from chainer_addons.links.pooling import PoolingType
+from cvmodelz.utils.links import Conv2D_BN
+from cvmodelz.utils.links.pooling import PoolingType
 
 
 class InceptionHead(chainer.Chain):
 	def __init__(self):
 		super().__init__()
 		with self.init_scope():
 			# input 3 x 299 x 299
```

### Comparing `cvmodelz-0.1.1/cvmodelz/models/pretrained/inception/inception_v3.py` & `cvmodelz-0.3.0/cvmodelz/models/pretrained/inception/inception_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import chainer
 import chainer.functions as F
 import chainer.links as L
 import numpy as np
 
-from chainer_addons.links.pooling import PoolingType # TODO: replace this!
 from chainercv.transforms import resize
 from chainercv.transforms import scale
 from collections import OrderedDict
 from collections.abc import Iterable
 
 
 from cvmodelz.models.meta_info import ModelInfo
 from cvmodelz.models.pretrained.base import PretrainedModelMixin
 from cvmodelz.models.pretrained.inception import blocks
 from cvmodelz.models.pretrained.inception import link_mappings
+from cvmodelz.utils.links.pooling import PoolingType
 
 
 def _assign(name, param, data):
 	assert data.shape == param.shape, \
 		"\"{}\" does not match the shape: {} != {}!".format(
 			name, data.shape, param.shape)
 	if isinstance(param, chainer.variable.Parameter):
@@ -189,25 +189,25 @@
 		# input 2048 x 8 x 8
 		# global average pooling
 		# output 2048 x 1 x 1
 
 		# the final fc layer is initilized by PretrainedModelMixin
 		super().init_extra_layers(n_classes)
 
-	def loss(self, pred, gt, loss_func=F.softmax_cross_entropy, alpha=0.4):
+	def loss(self, pred, gt, *, loss_func=F.softmax_cross_entropy, alpha=0.4, **kwargs):
 		if isinstance(pred, tuple):
 			pred0, aux_pred = pred
 		else:
 			pred0, aux_pred = pred, None
 
-		loss = loss_func(pred0, gt)
+		loss = loss_func(pred0, gt, **kwargs)
 		if aux_pred is None:
 			return loss
 		else:
-			aux_loss = loss_func(aux_pred, gt)
+			aux_loss = loss_func(aux_pred, gt, **kwargs)
 			return (1-alpha) * loss + alpha * aux_loss
 
 	def accuracy(self, pred, gt):
 		if isinstance(pred, tuple):
 			pred0, aux_pred = pred
 		else:
 			pred0, aux_pred = pred, None
```

### Comparing `cvmodelz-0.1.1/cvmodelz/models/pretrained/inception/link_mappings.py` & `cvmodelz-0.3.0/cvmodelz/models/pretrained/inception/link_mappings.py`

 * *Files identical despite different names*

### Comparing `cvmodelz-0.1.1/cvmodelz/models/pretrained/resnet.py` & `cvmodelz-0.3.0/cvmodelz/models/pretrained/resnet.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,21 +22,40 @@
 			n_conv_maps=2048,
 
 			conv_map_layer="res5",
 			feature_layer="pool5",
 
 			classifier_layers=["fc6"],
 
-			prepare_func=prepare,
+			prepare_func=self.prepare,
 		)
 
+	def prepare(self, x, size=None, *, swap_channels=True, keep_ratio=True):
+		x = prepare(x, size)
+
+		# if not desired, we need to undo it
+		if not swap_channels:
+			x = x[:, :, ::-1]
+
+		return x
+
 	@property
 	def functions(self):
 		return super().functions
 
+class ResNetHDMixin:
+
+	def __init__(self, *args, **kwargs):
+		super().__init__(*args, **kwargs)
+		self.res4.a.conv1.stride = (1, 1)
+		self.res4.a.conv4.stride = (1, 1)
+
+		self.res5.a.conv1.stride = (1, 1)
+		self.res5.a.conv4.stride = (1, 1)
+
 """
 We need this to "extract" pretrained_model argument,
 otherwise it would be passed to the constructor of the
 chainer.Chain class, where it raises an error
 """
 class ResNet35Layers(chainer.Chain):
 
@@ -77,17 +96,22 @@
 		for key, funcs in self.functions.items():
 			for func in funcs:
 				x = func(x)
 			if key == layer_name:
 				return x
 
 
+class ResNet35HD(ResNetHDMixin, ResNet35):
+	pass
+
 class ResNet50(BaseResNet, L.ResNet50Layers):
 	n_layers = 50
 
+class ResNet50HD(ResNetHDMixin, ResNet50):
+	pass
 
 class ResNet101(BaseResNet, L.ResNet101Layers):
 	n_layers = 101
 
 
 class ResNet152(BaseResNet, L.ResNet152Layers):
 	n_layers = 152
```

### Comparing `cvmodelz-0.1.1/cvmodelz/models/wrapper.py` & `cvmodelz-0.3.0/cvmodelz/models/wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,81 @@
 import chainer
 
-from chainer import functions as F
 from collections import OrderedDict
 
 from cvmodelz.models.base import BaseModel
 from cvmodelz.models.meta_info import ModelInfo
 
 
-
 class ModelWrapper(BaseModel):
 	"""
 		This class is designed to wrap around chainercv2 models
 		and provide the loading API of the BaseModel class.
 		The wrapped model is stored under self.wrapped
 	"""
 
 	def __init__(self, model: chainer.Chain, *args, **kwargs):
-		super().__init__(*args, **kwargs)
-
 		name = model.__class__.__name__
 		self.__class__.__name__ = name
-		self.meta.name = name
+		self.model_name = name
+		super().__init__(*args, **kwargs)
+
 
 		if hasattr(model, "meta"):
 			self.meta = model.meta
 
 		with self.init_scope():
 			self.wrapped = model
 			delattr(self.wrapped.features, "final_pool")
 
-		self.meta.feature_size = self.clf_layer.W.shape[-1]
 
 	def init_model_info(self):
-		self.meta = ModelInfo(
-			classifier_layers=("output/fc",),
+		info = dict(
+			name=self.model_name,
+			feature_size=2048,
+			n_conv_maps=2048,
+			classifier_layers=["output/fc"],
 			conv_map_layer="features",
 			feature_layer="pool",
 		)
 
+		if self.model_name == "InceptionResNetV1":
+			info.update(dict(
+				input_size=299,
+				feature_size=1792,
+				n_conv_maps=1792,
+				classifier_layers=[
+					"output/fc1",
+					"output/fc2"
+				],
+			))
+
+		elif self.model_name == "InceptionV3":
+			info.update(dict(
+				input_size=299,
+			))
+
+		elif self.model_name in ["ResNet", "ResNeXt"]:
+			info.update(dict(
+				input_size=224,
+			))
+
+		self.meta = ModelInfo(**info)
+
 	@property
 	def model_instance(self) -> chainer.Chain:
 		return self.wrapped
 
 	@property
 	def functions(self) -> OrderedDict:
 
 		links = [
-			("features", [self.wrapped.features]),
-			("pool", [self.pool]),
-			("output/fc", [self.wrapped.output.fc]),
+			(self.meta.conv_map_layer, [self.wrapped.features]),
+			(self.meta.feature_layer, [self.pool]),
+			(self.clf_layer_name, [self.wrapped.output]),
 		]
 
 		return OrderedDict(links)
 
 	def load(self, *args, path="", **kwargs):
 		paths = [path, f"{path}wrapped/"]
 		for _path in paths:
```

### Comparing `cvmodelz-0.1.1/cvmodelz/utils/__init__.py` & `cvmodelz-0.3.0/cvmodelz/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import numpy as np
 import sys
 import logging
 
 from functools import partial
 from tabulate import tabulate
 
+from chainer.function_hooks import TimerHook
+from chainer.function_hooks import CupyMemoryProfileHook
+
+
 def get_attr_from_path(obj, path, *, sep="/"):
 	def getter(o, attr):
 		return
 	getter = lambda o, attr: (getattr(o, attr) if attr else o)
 	return reduce(getter, path.split(sep), obj)
 
 def _get_activation_shapes(model, input_size, input_var, batch_size=2, n_channels=3):
@@ -62,13 +66,21 @@
 
 	n_layers = len(list(model.links()))
 	rows.append(("# of layers", f"{n_layers:,d}"))
 
 	_print(f"Printing some information about \"{name}\" model")
 	_print(tabulate(rows, tablefmt="fancy_grid"))
 
-	shapes = _get_activation_shapes(model, input_size or default_size, input_var)
+	timer_hook = TimerHook()
+	memory_hook = CupyMemoryProfileHook()
+
+	with timer_hook, memory_hook:
+		shapes = _get_activation_shapes(model, input_size or default_size, input_var)
+
+	timer_hook.print_report()
+	memory_hook.print_report()
+
 	_print("In/Out activation shapes:")
 	_print(tabulate(shapes,
 		headers=["Link name", "Input", "Output"],
 		tablefmt="fancy_grid"))
```

### Comparing `cvmodelz-0.1.1/cvmodelz.egg-info/SOURCES.txt` & `cvmodelz-0.3.0/cvmodelz.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -21,9 +21,20 @@
 cvmodelz/models/pretrained/__init__.py
 cvmodelz/models/pretrained/base.py
 cvmodelz/models/pretrained/resnet.py
 cvmodelz/models/pretrained/vgg.py
 cvmodelz/models/pretrained/inception/__init__.py
 cvmodelz/models/pretrained/inception/blocks.py
 cvmodelz/models/pretrained/inception/inception_v3.py
+cvmodelz/models/pretrained/inception/inception_v3_hd.py
 cvmodelz/models/pretrained/inception/link_mappings.py
-cvmodelz/utils/__init__.py
+cvmodelz/utils/__init__.py
+cvmodelz/utils/functions/__init__.py
+cvmodelz/utils/functions/alpha_product.py
+cvmodelz/utils/functions/signed_square_root.py
+cvmodelz/utils/functions/tf_average.py
+cvmodelz/utils/links/__init__.py
+cvmodelz/utils/links/pooling/__init__.py
+cvmodelz/utils/links/pooling/alpha_pooling.py
+cvmodelz/utils/links/pooling/compact_bilinear.py
+cvmodelz/utils/links/pooling/global_average.py
+tests/test_utils.py
```

### Comparing `cvmodelz-0.1.1/setup.py` & `cvmodelz-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	line.strip()
 		for line in open(str(cwd / "requirements.txt")).readlines()
 ]
 
 setup(
 	name=pkg_name,
 	version=__version__,
-	python_requires=">3.6",
+	python_requires=">3.7",
 	description='Wrapper for various computer vision models (mostly provided by chainer, chainercv, and chainercv2)',
 	log_description=open(str(cwd / "README.md")).read(),
 	author='Dimitri Korsch',
 	author_email='korschdima@gmail.com',
 	license='MIT License',
 	packages=find_packages(exclude=("tests",)),
 	zip_safe=False,
```

