# Comparing `tmp/yet-another-retnet-0.1.0rc1.tar.gz` & `tmp/yet-another-retnet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yet-another-retnet-0.1.0rc1.tar", last modified: Thu Aug  3 17:23:14 2023, max compression
+gzip compressed data, was "yet-another-retnet-0.1.1.tar", last modified: Tue Aug  8 02:10:35 2023, max compression
```

## Comparing `yet-another-retnet-0.1.0rc1.tar` & `yet-another-retnet-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:23:14.090304 yet-another-retnet-0.1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:23:14.086304 yet-another-retnet-0.1.0rc1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:23:14.086304 yet-another-retnet-0.1.0rc1/.github/disabled-workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/.github/disabled-workflows/test-slow.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:23:14.086304 yet-another-retnet-0.1.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-08-03 17:23:14.090304 yet-another-retnet-0.1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:23:14.090304 yet-another-retnet-0.1.0rc1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)   235211 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/doc/benchmarks.png
--rw-r--r--   0 runner    (1001) docker     (123)    18616 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/doc/impossible-triangle.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    42227 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/doc/inference-memory.png
--rw-r--r--   0 runner    (1001) docker     (123)    39540 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/doc/inference-throughput.png
--rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/doc/retention-dual-forms.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    62327 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/doc/retnet-scaling.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:23:14.090304 yet-another-retnet-0.1.0rc1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/scripts/benchmark_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 17:23:14.090304 yet-another-retnet-0.1.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:23:14.090304 yet-another-retnet-0.1.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/tests/test_retention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/tests/test_retnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:23:14.090304 yet-another-retnet-0.1.0rc1/yet_another_retnet/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/yet_another_retnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16655 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/yet_another_retnet/retention.py
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/yet_another_retnet/retnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:23:14.090304 yet-another-retnet-0.1.0rc1/yet_another_retnet/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/yet_another_retnet/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/yet_another_retnet/utils/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-03 17:23:01.000000 yet-another-retnet-0.1.0rc1/yet_another_retnet/utils/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:23:14.090304 yet-another-retnet-0.1.0rc1/yet_another_retnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-08-03 17:23:14.000000 yet-another-retnet-0.1.0rc1/yet_another_retnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-03 17:23:14.000000 yet-another-retnet-0.1.0rc1/yet_another_retnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:23:14.000000 yet-another-retnet-0.1.0rc1/yet_another_retnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-03 17:23:14.000000 yet-another-retnet-0.1.0rc1/yet_another_retnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 17:23:14.000000 yet-another-retnet-0.1.0rc1/yet_another_retnet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:10:35.385808 yet-another-retnet-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:10:35.381808 yet-another-retnet-0.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:10:35.381808 yet-another-retnet-0.1.1/.github/disabled-workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/.github/disabled-workflows/test-slow.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:10:35.381808 yet-another-retnet-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-08-08 02:10:35.381808 yet-another-retnet-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:10:35.381808 yet-another-retnet-0.1.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)   235211 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/doc/benchmarks.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18616 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/doc/impossible-triangle.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    42227 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/doc/inference-memory.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39540 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/doc/inference-throughput.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/doc/retention-dual-forms.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    62327 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/doc/retnet-scaling.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:10:35.381808 yet-another-retnet-0.1.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/scripts/benchmark_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 02:10:35.385808 yet-another-retnet-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:10:35.381808 yet-another-retnet-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/tests/test_retention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/tests/test_retnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:10:35.381808 yet-another-retnet-0.1.1/yet_another_retnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/yet_another_retnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/yet_another_retnet/retention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/yet_another_retnet/retnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:10:35.381808 yet-another-retnet-0.1.1/yet_another_retnet/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/yet_another_retnet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/yet_another_retnet/utils/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-08 02:10:23.000000 yet-another-retnet-0.1.1/yet_another_retnet/utils/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:10:35.381808 yet-another-retnet-0.1.1/yet_another_retnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-08-08 02:10:35.000000 yet-another-retnet-0.1.1/yet_another_retnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-08 02:10:35.000000 yet-another-retnet-0.1.1/yet_another_retnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 02:10:35.000000 yet-another-retnet-0.1.1/yet_another_retnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-08 02:10:35.000000 yet-another-retnet-0.1.1/yet_another_retnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-08 02:10:35.000000 yet-another-retnet-0.1.1/yet_another_retnet.egg-info/top_level.txt
```

### Comparing `yet-another-retnet-0.1.0rc1/.coveragerc` & `yet-another-retnet-0.1.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/.github/disabled-workflows/test-slow.yaml` & `yet-another-retnet-0.1.1/.github/disabled-workflows/test-slow.yaml`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/.github/workflows/publish.yaml` & `yet-another-retnet-0.1.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/.github/workflows/test.yaml` & `yet-another-retnet-0.1.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/.gitignore` & `yet-another-retnet-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/LICENSE` & `yet-another-retnet-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/PKG-INFO` & `yet-another-retnet-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: yet-another-retnet
-Version: 0.1.0rc1
-Summary: yet-another-retnet
-Author-email: Frank Odom <fodom@plainsight.ai>
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # yet-another-retnet
 
 A simple but robust PyTorch implementation of RetNet from [Retentive Network: A Successor to Transformer for Large Language Models](https://arxiv.org/pdf/2307.08621.pdf).
 
 > Also see Microsoft's original implementation: [RetNet @ microsoft/torchscale](https://github.com/microsoft/torchscale/blob/main/torchscale/architecture/retnet.py)
 >
 > Ultimately, their implementation is the ground truth.  I have tried to make my implementation as readable and well-documented as possible, while still being consistent with the original.  My version also includes full type annotations, and a robust set of unit tests.
@@ -32,29 +20,40 @@
     - The retention layer explicitly includes a position embedding update, which is based on [xPos](https://arxiv.org/pdf/2212.10554.pdf).  It does not necessarily translate well to other domains (e.g. computer vision, heterogeneous graphs).  So, I have made it optional.
     - I'm not 100% sure why the authors did this.  It seems overly specific to the language modeling use case, and it's not clear to me that it was necessary.
 - [x] End-to-end `RetNet` module.  See: [retnet.py](yet_another_retnet/retnet.py)
     - [x] `RetNetDecoderLayer`
     - [x] `RetNetDecoder`
 - [x] Preconfigured 1.3B, 2.7B, and 6.7B models (untrained).  See: [retnet.py](yet_another_retnet/retnet.py)
 - [x] Reproduce inference memory and throughput benchmarks from the paper.  See: [Inference Benchmarks](#inference-benchmarks), [benchmark_inference.py](scripts/benchmark_inference.py)
+- [x] Release stable version on PyPI.
+    - [x] Prerelease
+    - [x] Stable
 - [ ] Equivalent **chunkwise** retention method.
-- [ ] Release stable version on PyPI.
 - [ ] Basic training example for language modeling.
 
 
 ## Install
 
+PyPI:
+```bash
+pip install yet-another-retnet
+```
+
+From source:
 ```bash
 pip install "yet-another-retnet @ git+ssh://git@github.com/fkodom/yet-another-retnet.git"
 ```
 
 For contributors:
 ```bash
-# Install all dev dependencies (tests etc.)
-pip install "yet-another-retnet[test] @ git+ssh://git@github.com/fkodom/yet-another-retnet.git"
+# Clone/fork the repository
+gh repo clone fkodom/yet-another-retnet
+cd yet-another-retnet
+# Install all dev dependencies (tests etc.) in editable mode
+pip install -e .[test]
 # Setup pre-commit hooks
 pre-commit install
 ```
 
 
 ## About
 
@@ -220,7 +219,20 @@
 From this repo:
 
 <p float="left">
     <img src="doc/inference-memory.png" alt="retention-dual-forms" width="300"/>
     <img src="doc/inference-throughput.png" alt="retention-benchmarks" width="300"/>
 </p>
 
+
+## Citations
+
+```bibtex
+@misc{sun2023retentive,
+      title={Retentive Network: A Successor to Transformer for Large Language Models}, 
+      author={Yutao Sun and Li Dong and Shaohan Huang and Shuming Ma and Yuqing Xia and Jilong Xue and Jianyong Wang and Furu Wei},
+      year={2023},
+      eprint={2307.08621},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
+```
```

### Comparing `yet-another-retnet-0.1.0rc1/README.md` & `yet-another-retnet-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: yet-another-retnet
+Version: 0.1.1
+Summary: yet-another-retnet
+Author-email: Frank Odom <fodom@plainsight.ai>
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # yet-another-retnet
 
 A simple but robust PyTorch implementation of RetNet from [Retentive Network: A Successor to Transformer for Large Language Models](https://arxiv.org/pdf/2307.08621.pdf).
 
 > Also see Microsoft's original implementation: [RetNet @ microsoft/torchscale](https://github.com/microsoft/torchscale/blob/main/torchscale/architecture/retnet.py)
 >
 > Ultimately, their implementation is the ground truth.  I have tried to make my implementation as readable and well-documented as possible, while still being consistent with the original.  My version also includes full type annotations, and a robust set of unit tests.
@@ -20,29 +32,40 @@
     - The retention layer explicitly includes a position embedding update, which is based on [xPos](https://arxiv.org/pdf/2212.10554.pdf).  It does not necessarily translate well to other domains (e.g. computer vision, heterogeneous graphs).  So, I have made it optional.
     - I'm not 100% sure why the authors did this.  It seems overly specific to the language modeling use case, and it's not clear to me that it was necessary.
 - [x] End-to-end `RetNet` module.  See: [retnet.py](yet_another_retnet/retnet.py)
     - [x] `RetNetDecoderLayer`
     - [x] `RetNetDecoder`
 - [x] Preconfigured 1.3B, 2.7B, and 6.7B models (untrained).  See: [retnet.py](yet_another_retnet/retnet.py)
 - [x] Reproduce inference memory and throughput benchmarks from the paper.  See: [Inference Benchmarks](#inference-benchmarks), [benchmark_inference.py](scripts/benchmark_inference.py)
+- [x] Release stable version on PyPI.
+    - [x] Prerelease
+    - [x] Stable
 - [ ] Equivalent **chunkwise** retention method.
-- [ ] Release stable version on PyPI.
 - [ ] Basic training example for language modeling.
 
 
 ## Install
 
+PyPI:
+```bash
+pip install yet-another-retnet
+```
+
+From source:
 ```bash
 pip install "yet-another-retnet @ git+ssh://git@github.com/fkodom/yet-another-retnet.git"
 ```
 
 For contributors:
 ```bash
-# Install all dev dependencies (tests etc.)
-pip install "yet-another-retnet[test] @ git+ssh://git@github.com/fkodom/yet-another-retnet.git"
+# Clone/fork the repository
+gh repo clone fkodom/yet-another-retnet
+cd yet-another-retnet
+# Install all dev dependencies (tests etc.) in editable mode
+pip install -e .[test]
 # Setup pre-commit hooks
 pre-commit install
 ```
 
 
 ## About
 
@@ -208,7 +231,20 @@
 From this repo:
 
 <p float="left">
     <img src="doc/inference-memory.png" alt="retention-dual-forms" width="300"/>
     <img src="doc/inference-throughput.png" alt="retention-benchmarks" width="300"/>
 </p>
 
+
+## Citations
+
+```bibtex
+@misc{sun2023retentive,
+      title={Retentive Network: A Successor to Transformer for Large Language Models}, 
+      author={Yutao Sun and Li Dong and Shaohan Huang and Shuming Ma and Yuqing Xia and Jilong Xue and Jianyong Wang and Furu Wei},
+      year={2023},
+      eprint={2307.08621},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
+```
```

### Comparing `yet-another-retnet-0.1.0rc1/doc/benchmarks.png` & `yet-another-retnet-0.1.1/doc/benchmarks.png`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/doc/impossible-triangle.jpeg` & `yet-another-retnet-0.1.1/doc/impossible-triangle.jpeg`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/doc/inference-memory.png` & `yet-another-retnet-0.1.1/doc/inference-memory.png`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/doc/inference-throughput.png` & `yet-another-retnet-0.1.1/doc/inference-throughput.png`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/doc/retention-dual-forms.jpeg` & `yet-another-retnet-0.1.1/doc/retention-dual-forms.jpeg`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/doc/retnet-scaling.jpeg` & `yet-another-retnet-0.1.1/doc/retnet-scaling.jpeg`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/pyproject.toml` & `yet-another-retnet-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/scripts/benchmark_inference.py` & `yet-another-retnet-0.1.1/scripts/benchmark_inference.py`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/tests/conftest.py` & `yet-another-retnet-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/tests/test_retention.py` & `yet-another-retnet-0.1.1/tests/test_retention.py`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/tests/test_retnet.py` & `yet-another-retnet-0.1.1/tests/test_retnet.py`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/yet_another_retnet/retention.py` & `yet-another-retnet-0.1.1/yet_another_retnet/retention.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import torch
 import torch.nn.functional as F
 from einops import einsum, rearrange, repeat
 from torch import Tensor, nn
 
 DEFAULT_DEVICE = torch.device("cpu")
-
 ActivationString = Literal["swish", "gelu", "relu"]
 
 
 def _get_activation_fn(activation: str) -> Callable[[Tensor], Tensor]:
     """Return an activation function given a string"""
     if activation == "swish":
         return F.relu
@@ -48,17 +47,17 @@
     query_length: int,
     key_length: int,
     decay_gammas: Tensor,
     device: Optional[Union[torch.device, str]] = None,
     dtype: Optional[torch.dtype] = None,
 ) -> Tensor:
     """The decay mask is one of the key components that makes *parallel* retention
-    equivalent to *recursive* retention.  The decay coefficients are pre-computed
+    equivalent to *recurrent* retention.  The decay coefficients are pre-computed
     and applied to the similarity matrix at once, rather than being applied to
-    each element in the recursive formulation.
+    each element in the recurrent formulation.
 
     See: https://arxiv.org/pdf/2307.08621v3.pdf, Equation 5
     """
     query_pos = torch.arange(query_length, device=device, dtype=dtype)
     key_pos = torch.arange(key_length, device=device, dtype=dtype)
 
     distance = torch.abs(query_pos.unsqueeze(-1) - key_pos.unsqueeze(0))
@@ -77,15 +76,15 @@
     head_dim: int,
     scale: float = 10000,
     device: Optional[Union[torch.device, str]] = None,
     dtype: Optional[torch.dtype] = None,
 ) -> Tensor:
     """Positional thetas are different for each value along head_dim, following the
     prescribed method in the paper.  These are used to update the positional
-    embeddings in both the parallel and recursive formulations of retention.
+    embeddings in both the parallel and recurrent formulations of retention.
     See: https://arxiv.org/pdf/2307.08621v3.pdf, Section 2.1 (Retention)
 
     NOTE: The actual values for thetas are not specified in the paper, so I
     copied these values from the official implementation.
     See: https://github.com/microsoft/torchscale/blob/7d231743f4f96c460b7cf0aa0cf242bb192b34f8/torchscale/architecture/retnet.py#L27C1-L28C59
     """
     x = torch.linspace(0, 1, steps=head_dim // 2, device=device, dtype=dtype)
@@ -189,15 +188,15 @@
 
     return retention, state
 
 
 class MultiScaleRetention(nn.Module):
     """Multi-scale retention (MSR) layer.  Intended to be (mostly) a drop-in replacement
     for nn.MultiheadAttention, but with the option to use either the parallel or
-    recursive formulation of retention. (Attention only has the parallel formulation.)
+    recurrent formulation of retention. (Attention only has the parallel formulation.)
 
     NOTE: As presented in the paper, Multi-Scale Retention includes an explicit
     position embedding, which is based on xPos.  IMO, this is unnecessary and overly
     specific to language modeling, since other domains (e.g. computer vision,
     heterogeneous graphs) will have different positional semantics.
 
     I have made the relational position embedding optional, so that this module
@@ -340,15 +339,15 @@
             cos = torch.cos(angles)
 
             q = _theta_shift(q, sin, cos)
             k = _complex_conjugate(_theta_shift(k, sin, cos))
 
         # Apply retention then group norm.
         retention, weights = retention_parallel(q, k, v, need_weights=need_weights)
-        # To apply group norm in an equivalent way to the recursive formulation,
+        # To apply group norm in an equivalent way to the recurrent formulation,
         # we fold the sequence dimension into the batch dimension.  Otherwise,
         # normalization would be applied over the entire input sequence.
         batch_size = retention.size(0)
         retention = rearrange(retention, "b h n d -> (b n) h d")
         retention = F.dropout(retention, p=self.dropout, training=self.training)
         retention = self.group_norm(retention)
         # Unfold 'n' from the batch dimension, and fold 'h' back into the embed dim.
```

### Comparing `yet-another-retnet-0.1.0rc1/yet_another_retnet/retnet.py` & `yet-another-retnet-0.1.1/yet_another_retnet/retnet.py`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/yet_another_retnet/utils/benchmark.py` & `yet-another-retnet-0.1.1/yet_another_retnet/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/yet_another_retnet/utils/profile.py` & `yet-another-retnet-0.1.1/yet_another_retnet/utils/profile.py`

 * *Files identical despite different names*

### Comparing `yet-another-retnet-0.1.0rc1/yet_another_retnet.egg-info/PKG-INFO` & `yet-another-retnet-0.1.1/yet_another_retnet.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yet-another-retnet
-Version: 0.1.0rc1
+Version: 0.1.1
 Summary: yet-another-retnet
 Author-email: Frank Odom <fodom@plainsight.ai>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -32,29 +32,40 @@
     - The retention layer explicitly includes a position embedding update, which is based on [xPos](https://arxiv.org/pdf/2212.10554.pdf).  It does not necessarily translate well to other domains (e.g. computer vision, heterogeneous graphs).  So, I have made it optional.
     - I'm not 100% sure why the authors did this.  It seems overly specific to the language modeling use case, and it's not clear to me that it was necessary.
 - [x] End-to-end `RetNet` module.  See: [retnet.py](yet_another_retnet/retnet.py)
     - [x] `RetNetDecoderLayer`
     - [x] `RetNetDecoder`
 - [x] Preconfigured 1.3B, 2.7B, and 6.7B models (untrained).  See: [retnet.py](yet_another_retnet/retnet.py)
 - [x] Reproduce inference memory and throughput benchmarks from the paper.  See: [Inference Benchmarks](#inference-benchmarks), [benchmark_inference.py](scripts/benchmark_inference.py)
+- [x] Release stable version on PyPI.
+    - [x] Prerelease
+    - [x] Stable
 - [ ] Equivalent **chunkwise** retention method.
-- [ ] Release stable version on PyPI.
 - [ ] Basic training example for language modeling.
 
 
 ## Install
 
+PyPI:
+```bash
+pip install yet-another-retnet
+```
+
+From source:
 ```bash
 pip install "yet-another-retnet @ git+ssh://git@github.com/fkodom/yet-another-retnet.git"
 ```
 
 For contributors:
 ```bash
-# Install all dev dependencies (tests etc.)
-pip install "yet-another-retnet[test] @ git+ssh://git@github.com/fkodom/yet-another-retnet.git"
+# Clone/fork the repository
+gh repo clone fkodom/yet-another-retnet
+cd yet-another-retnet
+# Install all dev dependencies (tests etc.) in editable mode
+pip install -e .[test]
 # Setup pre-commit hooks
 pre-commit install
 ```
 
 
 ## About
 
@@ -220,7 +231,20 @@
 From this repo:
 
 <p float="left">
     <img src="doc/inference-memory.png" alt="retention-dual-forms" width="300"/>
     <img src="doc/inference-throughput.png" alt="retention-benchmarks" width="300"/>
 </p>
 
+
+## Citations
+
+```bibtex
+@misc{sun2023retentive,
+      title={Retentive Network: A Successor to Transformer for Large Language Models}, 
+      author={Yutao Sun and Li Dong and Shaohan Huang and Shuming Ma and Yuqing Xia and Jilong Xue and Jianyong Wang and Furu Wei},
+      year={2023},
+      eprint={2307.08621},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
+```
```

### Comparing `yet-another-retnet-0.1.0rc1/yet_another_retnet.egg-info/SOURCES.txt` & `yet-another-retnet-0.1.1/yet_another_retnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

