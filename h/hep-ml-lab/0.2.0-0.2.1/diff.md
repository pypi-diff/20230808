# Comparing `tmp/hep_ml_lab-0.2.0.tar.gz` & `tmp/hep_ml_lab-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hep_ml_lab-0.2.0.tar", max compression
+gzip compressed data, was "hep_ml_lab-0.2.1.tar", max compression
```

## Comparing `hep_ml_lab-0.2.0.tar` & `hep_ml_lab-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1064 2023-06-29 08:34:09.274711 hep_ml_lab-0.2.0/LICENSE
--rw-r--r--   0        0        0     1126 2023-07-23 09:05:49.138056 hep_ml_lab-0.2.0/README.md
--rw-r--r--   0        0        0       22 2023-07-23 12:01:53.779247 hep_ml_lab-0.2.0/hml/__init__.py
--rw-r--r--   0        0        0     2026 2023-07-23 09:05:49.138056 hep_ml_lab-0.2.0/hml/datasets.py
--rw-r--r--   0        0        0     9210 2023-07-01 13:43:36.139707 hep_ml_lab-0.2.0/hml/generators.py
--rw-r--r--   0        0        0      265 2023-07-23 09:05:49.138056 hep_ml_lab-0.2.0/hml/methods/__init__.py
--rw-r--r--   0        0        0      981 2023-07-23 09:02:58.598424 hep_ml_lab-0.2.0/hml/methods/base.py
--rw-r--r--   0        0        0    11423 2023-07-23 09:05:49.138056 hep_ml_lab-0.2.0/hml/methods/cuts.py
--rw-r--r--   0        0        0        0 2023-07-23 09:05:49.138056 hep_ml_lab-0.2.0/hml/methods/networks/__init__.py
--rw-r--r--   0        0        0     3056 2023-07-24 02:33:14.694378 hep_ml_lab-0.2.0/hml/methods/networks/base.py
--rw-r--r--   0        0        0      675 2023-07-23 09:05:49.138056 hep_ml_lab-0.2.0/hml/methods/networks/mlps.py
--rw-r--r--   0        0        0     6052 2023-07-23 09:05:49.142056 hep_ml_lab-0.2.0/hml/methods/trees.py
--rw-r--r--   0        0        0    10244 2023-07-24 02:31:38.230586 hep_ml_lab-0.2.0/hml/metrics.py
--rw-r--r--   0        0        0     6089 2023-07-01 13:43:36.139707 hep_ml_lab-0.2.0/hml/observables.py
--rw-r--r--   0        0        0     1023 2023-07-23 09:05:49.142056 hep_ml_lab-0.2.0/hml/preprocessing.py
--rw-r--r--   0        0        0     1147 2023-07-23 09:05:49.142056 hep_ml_lab-0.2.0/hml/representations.py
--rw-r--r--   0        0        0     2680 2023-06-29 08:34:09.306711 hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/B-L-4_UFO.log
--rw-r--r--   0        0        0      300 2023-06-29 08:34:09.306711 hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/CT_couplings.py
--rw-r--r--   0        0        0      883 2023-06-29 08:34:09.306711 hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/__init__.py
--rw-r--r--   0        0        0      443 2023-06-29 08:34:09.314711 hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/coupling_orders.py
--rw-r--r--   0        0        0    38010 2023-06-29 08:34:09.322712 hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/couplings.py
--rw-r--r--   0        0        0    81001 2023-06-29 08:34:09.330712 hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/decays.py
--rw-r--r--   0        0        0     1949 2023-06-29 08:34:09.330712 hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/function_library.py
--rw-r--r--   0        0        0     3335 2023-06-29 08:34:09.330712 hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/lorentz.py
--rw-r--r--   0        0        0    10985 2023-06-29 08:34:09.330712 hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/object_library.py
--rw-r--r--   0        0        0    27451 2023-06-29 08:34:09.330712 hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/parameters.py
--rw-r--r--   0        0        0    14000 2023-06-29 08:34:09.330712 hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/particles.py
--rw-r--r--   0        0        0     1351 2023-06-29 08:34:09.330712 hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/propagators.py
--rw-r--r--   0        0        0    61296 2023-06-29 08:34:09.338712 hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/vertices.py
--rw-r--r--   0        0        0     7957 2023-06-29 08:34:09.338712 hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/write_param_card.py
--rw-r--r--   0        0        0      121 2023-06-29 08:34:09.346712 hep_ml_lab-0.2.0/hml/theories/B-L_model/metadata.yml
--rw-r--r--   0        0        0        0 2023-06-29 08:34:09.346712 hep_ml_lab-0.2.0/hml/theories/__init__.py
--rw-r--r--   0        0        0      821 2023-07-23 12:01:53.783247 hep_ml_lab-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 hep_ml_lab-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-29 08:34:09.274711 hep_ml_lab-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1405 2023-08-06 14:51:09.481636 hep_ml_lab-0.2.1/README.md
+-rw-r--r--   0        0        0       22 2023-08-06 14:51:09.481636 hep_ml_lab-0.2.1/hml/__init__.py
+-rw-r--r--   0        0        0     2026 2023-07-23 09:05:49.138056 hep_ml_lab-0.2.1/hml/datasets.py
+-rw-r--r--   0        0        0    13800 2023-08-06 14:51:09.481636 hep_ml_lab-0.2.1/hml/generators.py
+-rw-r--r--   0        0        0      265 2023-07-23 09:05:49.138056 hep_ml_lab-0.2.1/hml/methods/__init__.py
+-rw-r--r--   0        0        0      981 2023-07-23 09:02:58.598424 hep_ml_lab-0.2.1/hml/methods/base.py
+-rw-r--r--   0        0        0    11423 2023-07-23 09:05:49.138056 hep_ml_lab-0.2.1/hml/methods/cuts.py
+-rw-r--r--   0        0        0        0 2023-07-23 09:05:49.138056 hep_ml_lab-0.2.1/hml/methods/networks/__init__.py
+-rw-r--r--   0        0        0     3056 2023-07-24 02:33:14.694378 hep_ml_lab-0.2.1/hml/methods/networks/base.py
+-rw-r--r--   0        0        0      675 2023-07-23 09:05:49.138056 hep_ml_lab-0.2.1/hml/methods/networks/mlps.py
+-rw-r--r--   0        0        0     6052 2023-07-23 09:05:49.142056 hep_ml_lab-0.2.1/hml/methods/trees.py
+-rw-r--r--   0        0        0    10244 2023-07-24 02:31:38.230586 hep_ml_lab-0.2.1/hml/metrics.py
+-rw-r--r--   0        0        0     6089 2023-07-01 13:43:36.139707 hep_ml_lab-0.2.1/hml/observables.py
+-rw-r--r--   0        0        0     1023 2023-07-23 09:05:49.142056 hep_ml_lab-0.2.1/hml/preprocessing.py
+-rw-r--r--   0        0        0     1147 2023-07-23 09:05:49.142056 hep_ml_lab-0.2.1/hml/representations.py
+-rw-r--r--   0        0        0     2680 2023-06-29 08:34:09.306711 hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/B-L-4_UFO.log
+-rw-r--r--   0        0        0      300 2023-06-29 08:34:09.306711 hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/CT_couplings.py
+-rw-r--r--   0        0        0      883 2023-06-29 08:34:09.306711 hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/__init__.py
+-rw-r--r--   0        0        0      443 2023-06-29 08:34:09.314711 hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/coupling_orders.py
+-rw-r--r--   0        0        0    38010 2023-06-29 08:34:09.322712 hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/couplings.py
+-rw-r--r--   0        0        0    81001 2023-06-29 08:34:09.330712 hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/decays.py
+-rw-r--r--   0        0        0     1949 2023-06-29 08:34:09.330712 hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/function_library.py
+-rw-r--r--   0        0        0     3335 2023-06-29 08:34:09.330712 hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/lorentz.py
+-rw-r--r--   0        0        0    10985 2023-06-29 08:34:09.330712 hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/object_library.py
+-rw-r--r--   0        0        0    27451 2023-06-29 08:34:09.330712 hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/parameters.py
+-rw-r--r--   0        0        0    14000 2023-06-29 08:34:09.330712 hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/particles.py
+-rw-r--r--   0        0        0     1351 2023-06-29 08:34:09.330712 hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/propagators.py
+-rw-r--r--   0        0        0    61296 2023-06-29 08:34:09.338712 hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/vertices.py
+-rw-r--r--   0        0        0     7957 2023-06-29 08:34:09.338712 hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/write_param_card.py
+-rw-r--r--   0        0        0      121 2023-06-29 08:34:09.346712 hep_ml_lab-0.2.1/hml/theories/B-L_model/metadata.yml
+-rw-r--r--   0        0        0        0 2023-06-29 08:34:09.346712 hep_ml_lab-0.2.1/hml/theories/__init__.py
+-rw-r--r--   0        0        0      835 2023-08-06 14:51:09.485636 hep_ml_lab-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2212 1970-01-01 00:00:00.000000 hep_ml_lab-0.2.1/PKG-INFO
```

### Comparing `hep_ml_lab-0.2.0/LICENSE` & `hep_ml_lab-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/datasets.py` & `hep_ml_lab-0.2.1/hml/datasets.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/methods/base.py` & `hep_ml_lab-0.2.1/hml/methods/base.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/methods/cuts.py` & `hep_ml_lab-0.2.1/hml/methods/cuts.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/methods/networks/base.py` & `hep_ml_lab-0.2.1/hml/methods/networks/base.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/methods/networks/mlps.py` & `hep_ml_lab-0.2.1/hml/methods/networks/mlps.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/methods/trees.py` & `hep_ml_lab-0.2.1/hml/methods/trees.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/metrics.py` & `hep_ml_lab-0.2.1/hml/metrics.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/observables.py` & `hep_ml_lab-0.2.1/hml/observables.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/preprocessing.py` & `hep_ml_lab-0.2.1/hml/preprocessing.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/representations.py` & `hep_ml_lab-0.2.1/hml/representations.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/B-L-4_UFO.log` & `hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/B-L-4_UFO.log`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/__init__.py` & `hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/__init__.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/couplings.py` & `hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/couplings.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/decays.py` & `hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/decays.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/function_library.py` & `hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/function_library.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/lorentz.py` & `hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/lorentz.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/object_library.py` & `hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/object_library.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/parameters.py` & `hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/parameters.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/particles.py` & `hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/particles.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/propagators.py` & `hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/propagators.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/vertices.py` & `hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/vertices.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/hml/theories/B-L_model/B-L-4_UFO/write_param_card.py` & `hep_ml_lab-0.2.1/hml/theories/B-L_model/B-L-4_UFO/write_param_card.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.2.0/pyproject.toml` & `hep_ml_lab-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [tool.poetry]
 name = "hep-ml-lab"
-version = "0.2.0"
+version = "0.2.1"
 description = "An end-to-end framework for applying machine learning to high-energy physics research."
 authors = ["Star9daisy", "star9daisy@outlook.com"]
 readme = "README.md"
 packages = [
     { include = "hml" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 pyyaml = "^6.0"
-numpy = "^1.24.3"
+numpy = "^1.22"
 scikit-learn = "^1.2.2"
 matplotlib = "^3.7.1"
 tensorflow = "^2.11.0"
 rich = "^13.4.2"
+pytest = "^7.3.2"
+h5py = "^3.6.0"
 
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "^1.4.3"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 mkdocs-material = "^9.1.15"
-pytest = "^7.3.2"
 black = "^23.3.0"
 python-dotenv = "^1.0.0"
 deptry = "^0.12.0"
 mkdocs-jupyter = "^0.24.1"
 mkdocs-exclude = "^1.0.2"
 pytest-cov = "^4.1.0"
```

### Comparing `hep_ml_lab-0.2.0/PKG-INFO` & `hep_ml_lab-0.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 Metadata-Version: 2.1
 Name: hep-ml-lab
-Version: 0.2.0
+Version: 0.2.1
 Summary: An end-to-end framework for applying machine learning to high-energy physics research.
 Author: Star9daisy
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: h5py (>=3.6.0,<4.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: numpy (>=1.22,<2.0)
+Requires-Dist: pytest (>=7.3.2,<8.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: tensorflow (>=2.11.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # HEP ML Lab (HML)
-[![codecov](https://codecov.io/gh/Star9daisy/hep-ml-lab/branch/main/graph/badge.svg?token=6VWJi5ct6c)](https://codecov.io/gh/Star9daisy/hml)
+![codecov](https://codecov.io/gh/Star9daisy/hep-ml-lab/branch/main/graph/badge.svg?token=6VWJi5ct6c)
 
 ❗ This framework is currently undergoing **rapid iteration**. Any comments and suggestions are welcome.
 
 ## Introduction
+HEP ML Lab (HML) is an end-to-end framework for applying machine learning (ML)
+to high energy physics (HEP) research. It provides a set of interfaces for data generation, model training and evaluation. It is designed to be modular and
+extensible so that you can easily customize it for your own research.
+
+## Installation
+```python
+pip install hep-ml-lab
+```
 
-HEP ML Lab (HML) is an end-to-end framework for applying machine learning (ML) to high energy physics (HEP)
-research. It provides a set of interfaces for data generation, model training and evaluation. It is designed to
-be modular and extensible so that you can easily customize it for your own research.
+## Usage
+Check out the [documents](https://star9daisy.github.io/hep-ml-lab/).
 
 ## Module overview
-
-Here is a brief overview of the modules in HML:
-
 - `hml.generators`: API of Madgraph5 for simulating colliding events;
 - `hml.theories`: Particle physics models;
 - `hml.observables`: General observables in jet physics;
 - `hml.representations`: Different data structure used to represent an event;
 - `hml.datasets`: Existing datasets and helper classes for creating new datasets;
 - `hml.methods`: Cuts, trees and networks for classification;
 - `hml.metrics`: Metrics used in classical signal vs background analysis;
 
+## Updates
+### v0.2.1
+- Add `summary` to `hml.generators.Madgraph5` to print a summary of all run.
+- Add `remove` to `hml.generators.Madgraph5` to remove a run.
+- Add `clean` to `hml.generators.Madgraph5` to remove the output directory.
```

