# Comparing `tmp/lightning-cv-0.0.1.tar.gz` & `tmp/lightning-cv-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-cv-0.0.1.tar", last modified: Wed Aug  2 20:39:54 2023, max compression
+gzip compressed data, was "lightning-cv-0.0.2.tar", last modified: Tue Aug  8 16:51:29 2023, max compression
```

## Comparing `lightning-cv-0.0.1.tar` & `lightning-cv-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxr-x   0 ccmartin6 (72295) ccmartin6 (72295)        0 2023-08-02 20:39:54.417776 lightning-cv-0.0.1/
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     1067 2023-07-28 15:21:44.000000 lightning-cv-0.0.1/LICENSE
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)    20682 2023-08-02 20:39:54.417776 lightning-cv-0.0.1/PKG-INFO
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)    18951 2023-08-01 19:15:13.000000 lightning-cv-0.0.1/README.md
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      733 2023-08-01 19:44:59.000000 lightning-cv-0.0.1/pyproject.toml
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)       38 2023-08-02 20:39:54.417776 lightning-cv-0.0.1/setup.cfg
-drwxrwxr-x   0 ccmartin6 (72295) ccmartin6 (72295)        0 2023-08-02 20:39:54.413776 lightning-cv-0.0.1/src/
-drwxrwxr-x   0 ccmartin6 (72295) ccmartin6 (72295)        0 2023-08-02 20:39:54.417776 lightning-cv-0.0.1/src/lightning_cv/
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      774 2023-08-02 19:52:10.000000 lightning-cv-0.0.1/src/lightning_cv/__init__.py
-drwxrwxr-x   0 ccmartin6 (72295) ccmartin6 (72295)        0 2023-08-02 20:39:54.417776 lightning-cv-0.0.1/src/lightning_cv/callbacks/
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      432 2023-08-02 19:50:50.000000 lightning-cv-0.0.1/src/lightning_cv/callbacks/__init__.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     1927 2023-08-02 19:49:14.000000 lightning-cv-0.0.1/src/lightning_cv/callbacks/callbacks.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     3154 2023-08-02 19:50:53.000000 lightning-cv-0.0.1/src/lightning_cv/callbacks/checkpoint.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      287 2023-08-02 19:50:47.000000 lightning-cv-0.0.1/src/lightning_cv/callbacks/logger.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      373 2023-08-02 19:50:38.000000 lightning-cv-0.0.1/src/lightning_cv/callbacks/lr_monitor.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      428 2023-08-02 19:50:08.000000 lightning-cv-0.0.1/src/lightning_cv/callbacks/mode.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     4384 2023-08-02 19:49:39.000000 lightning-cv-0.0.1/src/lightning_cv/callbacks/progress.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      704 2023-08-01 19:46:10.000000 lightning-cv-0.0.1/src/lightning_cv/callbacks/summary.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     2228 2023-08-02 19:46:28.000000 lightning-cv-0.0.1/src/lightning_cv/config.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     3498 2023-08-02 20:34:49.000000 lightning-cv-0.0.1/src/lightning_cv/data.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     1453 2023-08-02 19:44:06.000000 lightning-cv-0.0.1/src/lightning_cv/module.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     3775 2023-08-02 20:32:23.000000 lightning-cv-0.0.1/src/lightning_cv/split.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)    22694 2023-08-02 19:42:57.000000 lightning-cv-0.0.1/src/lightning_cv/trainer.py
-drwxrwxr-x   0 ccmartin6 (72295) ccmartin6 (72295)        0 2023-08-02 20:39:54.417776 lightning-cv-0.0.1/src/lightning_cv/tuning/
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      191 2023-08-02 16:45:09.000000 lightning-cv-0.0.1/src/lightning_cv/tuning/__init__.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     5747 2023-08-02 17:55:15.000000 lightning-cv-0.0.1/src/lightning_cv/tuning/callbacks.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     1488 2023-08-02 16:25:24.000000 lightning-cv-0.0.1/src/lightning_cv/tuning/config.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     2403 2023-08-02 16:54:20.000000 lightning-cv-0.0.1/src/lightning_cv/tuning/hyperparameters.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     6278 2023-08-02 19:45:44.000000 lightning-cv-0.0.1/src/lightning_cv/tuning/tuner.py
-drwxrwxr-x   0 ccmartin6 (72295) ccmartin6 (72295)        0 2023-08-02 20:39:54.417776 lightning-cv-0.0.1/src/lightning_cv/typehints/
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     1072 2023-08-02 19:41:34.000000 lightning-cv-0.0.1/src/lightning_cv/typehints/__init__.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      433 2023-08-02 19:39:44.000000 lightning-cv-0.0.1/src/lightning_cv/typehints/data.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     1085 2023-08-02 19:50:25.000000 lightning-cv-0.0.1/src/lightning_cv/typehints/module.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      677 2023-08-02 20:35:52.000000 lightning-cv-0.0.1/src/lightning_cv/typehints/split.py
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     3039 2023-08-02 19:46:25.000000 lightning-cv-0.0.1/src/lightning_cv/utils.py
-drwxrwxr-x   0 ccmartin6 (72295) ccmartin6 (72295)        0 2023-08-02 20:39:54.417776 lightning-cv-0.0.1/src/lightning_cv.egg-info/
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)    20682 2023-08-02 20:39:54.000000 lightning-cv-0.0.1/src/lightning_cv.egg-info/PKG-INFO
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     1059 2023-08-02 20:39:54.000000 lightning-cv-0.0.1/src/lightning_cv.egg-info/SOURCES.txt
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)        1 2023-08-02 20:39:54.000000 lightning-cv-0.0.1/src/lightning_cv.egg-info/dependency_links.txt
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)       31 2023-08-02 20:39:54.000000 lightning-cv-0.0.1/src/lightning_cv.egg-info/requires.txt
--rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)       13 2023-08-02 20:39:54.000000 lightning-cv-0.0.1/src/lightning_cv.egg-info/top_level.txt
+drwxrwxr-x   0 ccmartin6 (72295) ccmartin6 (72295)        0 2023-08-08 16:51:29.275748 lightning-cv-0.0.2/
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     1067 2023-07-28 15:21:44.000000 lightning-cv-0.0.2/LICENSE
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)    20688 2023-08-08 16:51:29.275748 lightning-cv-0.0.2/PKG-INFO
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)    18957 2023-08-08 16:44:24.000000 lightning-cv-0.0.2/README.md
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      847 2023-08-08 16:45:38.000000 lightning-cv-0.0.2/pyproject.toml
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)       38 2023-08-08 16:51:29.275748 lightning-cv-0.0.2/setup.cfg
+drwxrwxr-x   0 ccmartin6 (72295) ccmartin6 (72295)        0 2023-08-08 16:51:29.271747 lightning-cv-0.0.2/src/
+drwxrwxr-x   0 ccmartin6 (72295) ccmartin6 (72295)        0 2023-08-08 16:51:29.271747 lightning-cv-0.0.2/src/lightning_cv/
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      890 2023-08-08 16:49:16.000000 lightning-cv-0.0.2/src/lightning_cv/__init__.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      248 2023-08-08 16:48:33.000000 lightning-cv-0.0.2/src/lightning_cv/__metadata__.py
+drwxrwxr-x   0 ccmartin6 (72295) ccmartin6 (72295)        0 2023-08-08 16:51:29.275748 lightning-cv-0.0.2/src/lightning_cv/callbacks/
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      432 2023-08-02 19:50:50.000000 lightning-cv-0.0.2/src/lightning_cv/callbacks/__init__.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     1927 2023-08-02 19:49:14.000000 lightning-cv-0.0.2/src/lightning_cv/callbacks/callbacks.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     3154 2023-08-02 19:50:53.000000 lightning-cv-0.0.2/src/lightning_cv/callbacks/checkpoint.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      287 2023-08-02 19:50:47.000000 lightning-cv-0.0.2/src/lightning_cv/callbacks/logger.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      373 2023-08-02 19:50:38.000000 lightning-cv-0.0.2/src/lightning_cv/callbacks/lr_monitor.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      428 2023-08-02 19:50:08.000000 lightning-cv-0.0.2/src/lightning_cv/callbacks/mode.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     4384 2023-08-02 19:49:39.000000 lightning-cv-0.0.2/src/lightning_cv/callbacks/progress.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      704 2023-08-01 19:46:10.000000 lightning-cv-0.0.2/src/lightning_cv/callbacks/summary.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     2228 2023-08-02 19:46:28.000000 lightning-cv-0.0.2/src/lightning_cv/config.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     3498 2023-08-02 20:34:49.000000 lightning-cv-0.0.2/src/lightning_cv/data.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     1453 2023-08-02 19:44:06.000000 lightning-cv-0.0.2/src/lightning_cv/module.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     3775 2023-08-02 20:32:23.000000 lightning-cv-0.0.2/src/lightning_cv/split.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)    22700 2023-08-08 16:44:45.000000 lightning-cv-0.0.2/src/lightning_cv/trainer.py
+drwxrwxr-x   0 ccmartin6 (72295) ccmartin6 (72295)        0 2023-08-08 16:51:29.275748 lightning-cv-0.0.2/src/lightning_cv/tuning/
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      191 2023-08-02 16:45:09.000000 lightning-cv-0.0.2/src/lightning_cv/tuning/__init__.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     5747 2023-08-02 17:55:15.000000 lightning-cv-0.0.2/src/lightning_cv/tuning/callbacks.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     1588 2023-08-08 16:34:51.000000 lightning-cv-0.0.2/src/lightning_cv/tuning/config.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     2938 2023-08-08 16:38:12.000000 lightning-cv-0.0.2/src/lightning_cv/tuning/hyperparameters.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     6284 2023-08-08 16:43:12.000000 lightning-cv-0.0.2/src/lightning_cv/tuning/tuner.py
+drwxrwxr-x   0 ccmartin6 (72295) ccmartin6 (72295)        0 2023-08-08 16:51:29.275748 lightning-cv-0.0.2/src/lightning_cv/typehints/
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     1072 2023-08-02 19:41:34.000000 lightning-cv-0.0.2/src/lightning_cv/typehints/__init__.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      433 2023-08-02 19:39:44.000000 lightning-cv-0.0.2/src/lightning_cv/typehints/data.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     1085 2023-08-02 19:50:25.000000 lightning-cv-0.0.2/src/lightning_cv/typehints/module.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)      677 2023-08-02 20:35:52.000000 lightning-cv-0.0.2/src/lightning_cv/typehints/split.py
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     3039 2023-08-02 19:46:25.000000 lightning-cv-0.0.2/src/lightning_cv/utils.py
+drwxrwxr-x   0 ccmartin6 (72295) ccmartin6 (72295)        0 2023-08-08 16:51:29.271747 lightning-cv-0.0.2/src/lightning_cv.egg-info/
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)    20688 2023-08-08 16:51:29.000000 lightning-cv-0.0.2/src/lightning_cv.egg-info/PKG-INFO
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)     1092 2023-08-08 16:51:29.000000 lightning-cv-0.0.2/src/lightning_cv.egg-info/SOURCES.txt
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)        1 2023-08-08 16:51:29.000000 lightning-cv-0.0.2/src/lightning_cv.egg-info/dependency_links.txt
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)       34 2023-08-08 16:51:29.000000 lightning-cv-0.0.2/src/lightning_cv.egg-info/requires.txt
+-rw-rw-r--   0 ccmartin6 (72295) ccmartin6 (72295)       13 2023-08-08 16:51:29.000000 lightning-cv-0.0.2/src/lightning_cv.egg-info/top_level.txt
```

### Comparing `lightning-cv-0.0.1/LICENSE` & `lightning-cv-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-cv-0.0.1/PKG-INFO` & `lightning-cv-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-cv
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cross validation using Lightning Fabric
 Author-email: Cody Martin <codycmar10@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Cody Martin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -289,15 +289,15 @@
     def __init__(
         self, 
         model_type: type[CrossValModule], 
         config: CrossValidationTrainerConfig,
     ):  
         self.model_type
         self.config = config
-        self.fabric = L.Fabric(**self.config.dict(include=self.__fabric_keys__))
+        self.fabric = L.Fabric(**self.config.model_dump(include=self.__fabric_keys__))
 
         # other init logic
 
     def train_with_cross_validation(self, datamodule, model_config):
         # this method setups up k-fold models
         # then does the cross validation loop described in the 
         # `Overall workflow` section above
```

### Comparing `lightning-cv-0.0.1/README.md` & `lightning-cv-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,15 @@
     def __init__(
         self, 
         model_type: type[CrossValModule], 
         config: CrossValidationTrainerConfig,
     ):  
         self.model_type
         self.config = config
-        self.fabric = L.Fabric(**self.config.dict(include=self.__fabric_keys__))
+        self.fabric = L.Fabric(**self.config.model_dump(include=self.__fabric_keys__))
 
         # other init logic
 
     def train_with_cross_validation(self, datamodule, model_config):
         # this method setups up k-fold models
         # then does the cross validation loop described in the 
         # `Overall workflow` section above
```

### Comparing `lightning-cv-0.0.1/src/lightning_cv/__init__.py` & `lightning-cv-0.0.2/src/lightning_cv/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,21 @@
     module,
     split,
     trainer,
     tuning,
     typehints,
     utils,
 )
+from .__metadata__ import (
+    __author__,
+    __description__,
+    __license__,
+    __title__,
+    __version__,
+)
 from .config import CrossValidationTrainerConfig
 from .data import CrossValidationDataModule
 from .module import BaseModelConfig, CrossValModule, CrossValModuleMixin
 from .split import BaseCrossValidator, BaseGroupCrossValidator
 from .trainer import CrossValidationTrainer
 
 __all__ = [
```

### Comparing `lightning-cv-0.0.1/src/lightning_cv/callbacks/callbacks.py` & `lightning-cv-0.0.2/src/lightning_cv/callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-cv-0.0.1/src/lightning_cv/callbacks/checkpoint.py` & `lightning-cv-0.0.2/src/lightning_cv/callbacks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-cv-0.0.1/src/lightning_cv/callbacks/progress.py` & `lightning-cv-0.0.2/src/lightning_cv/callbacks/progress.py`

 * *Files identical despite different names*

### Comparing `lightning-cv-0.0.1/src/lightning_cv/callbacks/summary.py` & `lightning-cv-0.0.2/src/lightning_cv/callbacks/summary.py`

 * *Files identical despite different names*

### Comparing `lightning-cv-0.0.1/src/lightning_cv/config.py` & `lightning-cv-0.0.2/src/lightning_cv/config.py`

 * *Files identical despite different names*

### Comparing `lightning-cv-0.0.1/src/lightning_cv/data.py` & `lightning-cv-0.0.2/src/lightning_cv/data.py`

 * *Files identical despite different names*

### Comparing `lightning-cv-0.0.1/src/lightning_cv/module.py` & `lightning-cv-0.0.2/src/lightning_cv/module.py`

 * *Files identical despite different names*

### Comparing `lightning-cv-0.0.1/src/lightning_cv/split.py` & `lightning-cv-0.0.2/src/lightning_cv/split.py`

 * *Files identical despite different names*

### Comparing `lightning-cv-0.0.1/src/lightning_cv/trainer.py` & `lightning-cv-0.0.2/src/lightning_cv/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         self.should_stop = False
         self.current_train_metrics: MetricType = dict()
         self._current_val_metrics_per_fold: MetricType = dict()
 
         self._add_default_callbacks(self.config.callbacks)
 
-        fabric_kwargs = self.config.dict(include=self.__fabric_keys__)
+        fabric_kwargs = self.config.model_dump(include=self.__fabric_keys__)
         self.fabric = Fabric(**fabric_kwargs)
 
     @property
     def current_val_metrics(self) -> MetricType:
         if not hasattr(self, "_current_val_metrics"):
             raise RuntimeError(
                 "Current validation metrics aren't available until after the 1st epoch"
```

### Comparing `lightning-cv-0.0.1/src/lightning_cv/tuning/callbacks.py` & `lightning-cv-0.0.2/src/lightning_cv/tuning/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-cv-0.0.1/src/lightning_cv/tuning/config.py` & `lightning-cv-0.0.2/src/lightning_cv/tuning/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 SuggestValues = Literal["int", "float", "categorical"]
 
 
 class Tunable(BaseModel):
     name: str
     suggest: SuggestValues
+    parent: Optional[str] = Field(None, description="parent for nested hparams")
 
 
 class TunableInt(Tunable):
     suggest: Literal["int"]
     low: int
     high: int
     step: int = 1
@@ -43,15 +44,15 @@
     step: Optional[float] = None
     log: bool = False
 
 
 class TunableCategorical(Tunable, Generic[_T, _U]):
     suggest: Literal["categorical"]
     choices: Sequence[_T]
-    map: Optional[dict[_T, _U]]
+    map: Optional[dict[_T, _U]] = None
 
 
 TunableType = Annotated[
     TunableInt | TunableFloat | TunableCategorical[_T, _U],
     Field(discriminator="suggest"),
 ]
 TunableTypeTuple = (TunableInt, TunableFloat, TunableCategorical)
@@ -61,13 +62,13 @@
     hparams: list[TunableType]
 
 
 def load_config(file: str | Path) -> HparamConfig:
     with open(file, "rb") as fp:
         config = tomli.load(fp)
 
-    validated_config = HparamConfig.validate(config)
+    validated_config = HparamConfig.model_validate(config)
     return validated_config
 
 
 def DummyHparamConfig() -> HparamConfig:
-    return HparamConfig.construct()
+    return HparamConfig.model_construct()
```

### Comparing `lightning-cv-0.0.1/src/lightning_cv/tuning/hyperparameters.py` & `lightning-cv-0.0.2/src/lightning_cv/tuning/hyperparameters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import annotations
 
+from collections import defaultdict
 from pathlib import Path
-from typing import Mapping
+from typing import Mapping, Optional
 
 import optuna
 from lightning_utilities.core.apply_func import apply_to_collection
 
 from .config import (
     HparamConfig,
     TunableCategorical,
     TunableType,
     TunableTypeTuple,
     load_config,
 )
 
 TrialedValue = int | float | str
-IntFloatStrDict = dict[str, TrialedValue]
+IntFloatStrDict = dict[str, TrialedValue | dict[str, TrialedValue]]
 
 
 class HparamRegistry:
     __suggest_fields__ = {"low", "high", "step", "log", "choices", "name"}
 
     def __init__(self, config: HparamConfig):
         self._hparams: IntFloatStrDict = dict()
@@ -40,40 +41,52 @@
     @classmethod
     def from_file(cls, config_file: str | Path):
         config = load_config(config_file)
         return cls(config)
 
     def _register(
         self, x: TunableType, trial: optuna.Trial
-    ) -> tuple[str, TrialedValue]:
+    ) -> tuple[str, TrialedValue, Optional[str]]:
         method = f"suggest_{x.suggest}"
-        method_kwargs = x.dict(include=self.__suggest_fields__)
+        method_kwargs = x.model_dump(include=self.__suggest_fields__)
         trialed_value: TrialedValue = getattr(trial, method)(**method_kwargs)
 
         if isinstance(x, TunableCategorical) and x.map is not None:
             trialed_value = x.map[trialed_value]
 
-        return x.name, trialed_value
+        return x.name, trialed_value, x.parent
 
     def register_hparams(self, trial: optuna.Trial):
         hparams = apply_to_collection(
             data=self._hparam_config.hparams,
             dtype=TunableTypeTuple,
             function=self._register,
             trial=trial,
         )
 
+        nested_hparams = defaultdict(dict)
         # proxy hparams may map to an arbitrary number of other hparams that are dicts
         # ex: ProxyHparam has choices [a, b, c]
         # but each choice just maps -> a: {real_hparam1: x, real_hparam2: y}
         # thus, if anything mapped, unnest and remove proxy hparam
-        for key, value in hparams:
+
+        # further, need to convert to the correct nesting for the model config
+        for key, value, parent in hparams:
+            if parent is not None:
+                # create a new subdict with the parent as the key
+                current: dict = nested_hparams[parent]
+            else:
+                # otherwise add keys to root level
+                current = nested_hparams
+
             if isinstance(value, Mapping):
-                self._hparams.update(value)
+                current.update(value)
             else:
-                self._hparams[key] = value
+                current[key] = value
+
+        self._hparams = dict(nested_hparams)
 
 
 def suggest(trial: optuna.Trial, registry: HparamRegistry) -> IntFloatStrDict:
     registry.reset()
     registry.register_hparams(trial)
     return registry.hparams
```

### Comparing `lightning-cv-0.0.1/src/lightning_cv/tuning/tuner.py` & `lightning-cv-0.0.2/src/lightning_cv/tuning/tuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     def _init_model_config(
         self,
         model_config: ModelConfig,
         model_config_serializer: Optional[ModelConfigSerializeFn] = None,
     ) -> KwargType:
         if isinstance(model_config, BaseModelConfig):
             # pydantic model
-            return model_config.dict()
+            return model_config.model_dump()
         elif is_dataclass(model_config):
             return asdict(model_config)
 
         if model_config_serializer is None:
             raise ValueError(
                 "Model config is neither a `pydantic.BaseModel` nor a "
                 "`dataclasses.dataclass`. A serialization function to convert the "
```

### Comparing `lightning-cv-0.0.1/src/lightning_cv/typehints/__init__.py` & `lightning-cv-0.0.2/src/lightning_cv/typehints/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-cv-0.0.1/src/lightning_cv/typehints/module.py` & `lightning-cv-0.0.2/src/lightning_cv/typehints/module.py`

 * *Files identical despite different names*

### Comparing `lightning-cv-0.0.1/src/lightning_cv/typehints/split.py` & `lightning-cv-0.0.2/src/lightning_cv/typehints/split.py`

 * *Files identical despite different names*

### Comparing `lightning-cv-0.0.1/src/lightning_cv/utils.py` & `lightning-cv-0.0.2/src/lightning_cv/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-cv-0.0.1/src/lightning_cv.egg-info/PKG-INFO` & `lightning-cv-0.0.2/src/lightning_cv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-cv
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cross validation using Lightning Fabric
 Author-email: Cody Martin <codycmar10@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Cody Martin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -289,15 +289,15 @@
     def __init__(
         self, 
         model_type: type[CrossValModule], 
         config: CrossValidationTrainerConfig,
     ):  
         self.model_type
         self.config = config
-        self.fabric = L.Fabric(**self.config.dict(include=self.__fabric_keys__))
+        self.fabric = L.Fabric(**self.config.model_dump(include=self.__fabric_keys__))
 
         # other init logic
 
     def train_with_cross_validation(self, datamodule, model_config):
         # this method setups up k-fold models
         # then does the cross validation loop described in the 
         # `Overall workflow` section above
```

### Comparing `lightning-cv-0.0.1/src/lightning_cv.egg-info/SOURCES.txt` & `lightning-cv-0.0.2/src/lightning_cv.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 src/lightning_cv/__init__.py
+src/lightning_cv/__metadata__.py
 src/lightning_cv/config.py
 src/lightning_cv/data.py
 src/lightning_cv/module.py
 src/lightning_cv/split.py
 src/lightning_cv/trainer.py
 src/lightning_cv/utils.py
 src/lightning_cv.egg-info/PKG-INFO
```

