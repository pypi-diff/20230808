# Comparing `tmp/ultr_toolbox-0.1.0.tar.gz` & `tmp/ultr_toolbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultr_toolbox-0.1.0.tar", max compression
+gzip compressed data, was "ultr_toolbox-0.1.1.tar", max compression
```

## Comparing `ultr_toolbox-0.1.0.tar` & `ultr_toolbox-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1251 2023-08-07 14:39:14.110933 ultr_toolbox-0.1.0/README.md
--rw-r--r--   0        0        0      449 2023-08-08 07:01:46.498682 ultr_toolbox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-07 08:38:57.875358 ultr_toolbox-0.1.0/ultr_toolbox/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 08:47:06.422347 ultr_toolbox-0.1.0/ultr_toolbox/click_models/__init__.py
--rw-r--r--   0        0        0     1447 2023-08-07 14:05:50.952439 ultr_toolbox-0.1.0/ultr_toolbox/click_models/data.py
--rw-r--r--   0        0        0       36 2023-08-07 14:28:59.961103 ultr_toolbox-0.1.0/ultr_toolbox/click_models/em/__init__.py
--rw-r--r--   0        0        0     1336 2023-08-07 14:23:46.333602 ultr_toolbox-0.1.0/ultr_toolbox/click_models/em/trainer.py
--rw-r--r--   0        0        0     2007 2023-08-08 06:48:03.509826 ultr_toolbox-0.1.0/ultr_toolbox/click_models/metrics.py
--rw-r--r--   0        0        0      175 2023-08-07 14:29:51.451950 ultr_toolbox-0.1.0/ultr_toolbox/click_models/neural/__init__.py
--rw-r--r--   0        0        0      201 2023-08-08 06:08:37.053240 ultr_toolbox-0.1.0/ultr_toolbox/click_models/neural/base.py
--rw-r--r--   0        0        0      754 2023-08-08 06:08:37.051726 ultr_toolbox-0.1.0/ultr_toolbox/click_models/neural/cm.py
--rw-r--r--   0        0        0     1350 2023-08-08 06:08:37.055598 ultr_toolbox-0.1.0/ultr_toolbox/click_models/neural/dbn.py
--rw-r--r--   0        0        0      364 2023-08-07 09:06:21.959395 ultr_toolbox-0.1.0/ultr_toolbox/click_models/neural/loss.py
--rw-r--r--   0        0        0      633 2023-08-08 06:08:37.049680 ultr_toolbox-0.1.0/ultr_toolbox/click_models/neural/pbm.py
--rw-r--r--   0        0        0     4362 2023-08-08 06:41:18.691165 ultr_toolbox-0.1.0/ultr_toolbox/click_models/neural/trainer.py
--rw-r--r--   0        0        0     1734 2023-08-08 06:08:37.041783 ultr_toolbox-0.1.0/ultr_toolbox/click_models/neural/ubm.py
--rw-r--r--   0        0        0      214 2023-08-07 14:29:31.658095 ultr_toolbox-0.1.0/ultr_toolbox/click_models/stats/__init__.py
--rw-r--r--   0        0        0     3673 2023-08-07 14:14:44.894982 ultr_toolbox-0.1.0/ultr_toolbox/click_models/stats/models.py
--rw-r--r--   0        0        0     1034 2023-08-07 14:15:47.765261 ultr_toolbox-0.1.0/ultr_toolbox/click_models/stats/trainer.py
--rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 ultr_toolbox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1612 2023-08-08 07:07:20.396437 ultr_toolbox-0.1.1/README.md
+-rw-r--r--   0        0        0      448 2023-08-08 07:40:47.803448 ultr_toolbox-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-07 08:38:57.875358 ultr_toolbox-0.1.1/ultr_toolbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 08:47:06.422347 ultr_toolbox-0.1.1/ultr_toolbox/click_models/__init__.py
+-rw-r--r--   0        0        0     1447 2023-08-07 14:05:50.952439 ultr_toolbox-0.1.1/ultr_toolbox/click_models/data.py
+-rw-r--r--   0        0        0       36 2023-08-07 14:28:59.961103 ultr_toolbox-0.1.1/ultr_toolbox/click_models/em/__init__.py
+-rw-r--r--   0        0        0     1336 2023-08-07 14:23:46.333602 ultr_toolbox-0.1.1/ultr_toolbox/click_models/em/trainer.py
+-rw-r--r--   0        0        0     2007 2023-08-08 06:48:03.509826 ultr_toolbox-0.1.1/ultr_toolbox/click_models/metrics.py
+-rw-r--r--   0        0        0      175 2023-08-07 14:29:51.451950 ultr_toolbox-0.1.1/ultr_toolbox/click_models/neural/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-08 06:08:37.053240 ultr_toolbox-0.1.1/ultr_toolbox/click_models/neural/base.py
+-rw-r--r--   0        0        0      754 2023-08-08 06:08:37.051726 ultr_toolbox-0.1.1/ultr_toolbox/click_models/neural/cm.py
+-rw-r--r--   0        0        0     1350 2023-08-08 06:08:37.055598 ultr_toolbox-0.1.1/ultr_toolbox/click_models/neural/dbn.py
+-rw-r--r--   0        0        0      364 2023-08-07 09:06:21.959395 ultr_toolbox-0.1.1/ultr_toolbox/click_models/neural/loss.py
+-rw-r--r--   0        0        0      633 2023-08-08 06:08:37.049680 ultr_toolbox-0.1.1/ultr_toolbox/click_models/neural/pbm.py
+-rw-r--r--   0        0        0     4362 2023-08-08 06:41:18.691165 ultr_toolbox-0.1.1/ultr_toolbox/click_models/neural/trainer.py
+-rw-r--r--   0        0        0     1734 2023-08-08 06:08:37.041783 ultr_toolbox-0.1.1/ultr_toolbox/click_models/neural/ubm.py
+-rw-r--r--   0        0        0      214 2023-08-07 14:29:31.658095 ultr_toolbox-0.1.1/ultr_toolbox/click_models/stats/__init__.py
+-rw-r--r--   0        0        0     3673 2023-08-07 14:14:44.894982 ultr_toolbox-0.1.1/ultr_toolbox/click_models/stats/models.py
+-rw-r--r--   0        0        0     1034 2023-08-07 14:15:47.765261 ultr_toolbox-0.1.1/ultr_toolbox/click_models/stats/trainer.py
+-rw-r--r--   0        0        0     2338 1970-01-01 00:00:00.000000 ultr_toolbox-0.1.1/PKG-INFO
```

### Comparing `ultr_toolbox-0.1.0/ultr_toolbox/click_models/data.py` & `ultr_toolbox-0.1.1/ultr_toolbox/click_models/data.py`

 * *Files identical despite different names*

### Comparing `ultr_toolbox-0.1.0/ultr_toolbox/click_models/em/trainer.py` & `ultr_toolbox-0.1.1/ultr_toolbox/click_models/em/trainer.py`

 * *Files identical despite different names*

### Comparing `ultr_toolbox-0.1.0/ultr_toolbox/click_models/metrics.py` & `ultr_toolbox-0.1.1/ultr_toolbox/click_models/metrics.py`

 * *Files identical despite different names*

### Comparing `ultr_toolbox-0.1.0/ultr_toolbox/click_models/neural/cm.py` & `ultr_toolbox-0.1.1/ultr_toolbox/click_models/neural/cm.py`

 * *Files identical despite different names*

### Comparing `ultr_toolbox-0.1.0/ultr_toolbox/click_models/neural/dbn.py` & `ultr_toolbox-0.1.1/ultr_toolbox/click_models/neural/dbn.py`

 * *Files identical despite different names*

### Comparing `ultr_toolbox-0.1.0/ultr_toolbox/click_models/neural/pbm.py` & `ultr_toolbox-0.1.1/ultr_toolbox/click_models/neural/pbm.py`

 * *Files identical despite different names*

### Comparing `ultr_toolbox-0.1.0/ultr_toolbox/click_models/neural/trainer.py` & `ultr_toolbox-0.1.1/ultr_toolbox/click_models/neural/trainer.py`

 * *Files identical despite different names*

### Comparing `ultr_toolbox-0.1.0/ultr_toolbox/click_models/neural/ubm.py` & `ultr_toolbox-0.1.1/ultr_toolbox/click_models/neural/ubm.py`

 * *Files identical despite different names*

### Comparing `ultr_toolbox-0.1.0/ultr_toolbox/click_models/stats/models.py` & `ultr_toolbox-0.1.1/ultr_toolbox/click_models/stats/models.py`

 * *Files identical despite different names*

### Comparing `ultr_toolbox-0.1.0/ultr_toolbox/click_models/stats/trainer.py` & `ultr_toolbox-0.1.1/ultr_toolbox/click_models/stats/trainer.py`

 * *Files identical despite different names*

### Comparing `ultr_toolbox-0.1.0/PKG-INFO` & `ultr_toolbox-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,15 @@
-Metadata-Version: 2.1
-Name: ultr-toolbox
-Version: 0.1.0
-Summary: 
-Author: Philipp Hager
-Author-email: philipp.konstantin.hager@gmail.com
-Requires-Python: >=3.11,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flax (>=0.7.1,<0.8.0)
-Requires-Dist: jax (>=0.4.14,<0.5.0)
-Requires-Dist: optax (>=0.1.7,<0.2.0)
-Requires-Dist: pandas (>=2.0.3,<3.0.0)
-Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
-Requires-Dist: torch (>=2.0.1,<3.0.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Description-Content-Type: text/markdown
+## Install
+```bash
+pip install ultr-toolbox
+```
 
 ## Click Models
 
 ### Create Datasets
-
 ```Python
 from ultr_toolbox.click_models.data import ClickDataset
 
 train_dataset = ClickDataset(train_df)
 val_dataset = ClickDataset(val_df)
 test_dataset = ClickDataset(test_df)
 ```
@@ -36,14 +22,21 @@
 model = PositionBasedModel()
 trainer = NeuralTrainer(model)
 trainer.fit(train_dataset, val_dataset)
 metrics = trainer.test(test_dataset, metrics=[Perplexity()])
 ```
 
 ### Train PyClick models
+To optionally train click models from the [PyClick](https://github.com/markovi/PyClick) library,
+first install PyClick as a dependency:
+```bash
+pip install git+https://github.com/markovi/PyClick
+```
+
+Next, you can use the `PyClickTrainer` module to run the same pipeline as for the Jax-based neural click models:
 ```
 from pyclick.click_models import PBM
 
 from ultr_toolbox.click_models.metrics import Perplexity
 from ultr_toolbox.click_models.em import PyClickTrainer
 
 model = PBM()
@@ -58,8 +51,7 @@
 from ultr_toolbox.click_models.stats import StatsTrainer, RankDocumentBasedModel
 
 model = RankDocumentBasedModel()
 trainer = StatsTrainer(model)
 trainer.fit(train_dataset, val_dataset)
 metrics = trainer.test(test_dataset, metrics=[Perplexity()])
 ```
-
```

