# Comparing `tmp/auto_rxn-2023.7.0.tar.gz` & `tmp/auto_rxn-2023.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_rxn-2023.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `auto_rxn-2023.7.0.tar` & `auto_rxn-2023.8.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0      764 2023-07-31 12:05:29.506278 auto_rxn-2023.7.0/.github/workflows/python-mypy.yml
--rw-r--r--   0        0        0     1033 2023-07-31 12:05:29.506278 auto_rxn-2023.7.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      790 2023-07-31 12:05:29.506278 auto_rxn-2023.7.0/.github/workflows/python-pytest.yml
--rw-r--r--   0        0        0      828 2023-07-31 12:05:29.506278 auto_rxn-2023.7.0/.github/workflows/run-entry-points.yml
--rw-r--r--   0        0        0      448 2023-07-31 12:05:29.506278 auto_rxn-2023.7.0/.gitignore
--rw-r--r--   0        0        0      359 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1245 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/LICENSE
--rw-r--r--   0        0        0     1247 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/README.md
--rw-r--r--   0        0        0       76 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/__init__.py
--rw-r--r--   0        0        0      220 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/__init__.py
--rw-r--r--   0        0        0     1098 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/__main__.py
--rw-r--r--   0        0        0      419 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/__version__.py
--rw-r--r--   0        0        0        0 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/_config.py
--rw-r--r--   0        0        0     2795 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/_device.py
--rw-r--r--   0        0        0     1098 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/_exceptions.py
--rw-r--r--   0        0        0     2156 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/_recipe.py
--rw-r--r--   0        0        0     3103 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/_run.py
--rw-r--r--   0        0        0     1248 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/_safety.py
--rw-r--r--   0        0        0      949 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/_testing.py
--rw-r--r--   0        0        0       77 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/devices/__init__.py
--rw-r--r--   0        0        0     2418 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/devices/_fake_furnace.py
--rw-r--r--   0        0        0     1285 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/devices/_fake_mfc.py
--rw-r--r--   0        0        0      160 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/devices/_reading.py
--rw-r--r--   0        0        0    19275 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/devices/_status.py
--rw-r--r--   0        0        0     1505 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/pyproject.toml
--rw-r--r--   0        0        0     1126 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/children/db.json
--rw-r--r--   0        0        0      159 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/children/recipe.csv
--rw-r--r--   0        0        0      796 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/children/test_children.py
--rw-r--r--   0        0        0     1127 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/fallback_position/db.json
--rw-r--r--   0        0        0      165 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/fallback_position/recipe.csv
--rw-r--r--   0        0        0      516 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/fallback_position/test_fallback.py
--rw-r--r--   0        0        0     1126 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/minimal_csv/db.json
--rw-r--r--   0        0        0      125 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/minimal_csv/recipe.csv
--rw-r--r--   0        0        0      308 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/minimal_csv/test_minimal_csv.py
--rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 auto_rxn-2023.7.0/PKG-INFO
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/__init__.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/.github/workflows/python-mypy.yml
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/.github/workflows/python-pytest.yml
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/.github/workflows/run-entry-points.yml
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/__init__.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/__main__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/__version__.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/_device.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/_exceptions.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/_limits.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/_recipe.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/_run.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/_safety.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/devices/__init__.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/devices/_fake_furnace.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/devices/_fake_mfc.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/devices/_reading.py
+-rw-r--r--   0        0        0    19275 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/devices/_status.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/testing/__init__.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/testing/_with_happi_db.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/auto_rxn/testing/_with_limit_set_to.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/tests/children/db.json
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/tests/children/recipe.csv
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/tests/children/test_children.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/tests/fallback_position/db.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/tests/fallback_position/recipe.csv
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/tests/fallback_position/test_fallback.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/tests/minimal_csv/db.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/tests/minimal_csv/recipe.csv
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/tests/minimal_csv/test_minimal_csv.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/LICENSE
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/README.md
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 auto_rxn-2023.8.0/PKG-INFO
```

### Comparing `auto_rxn-2023.7.0/.github/workflows/python-mypy.yml` & `auto_rxn-2023.8.0/.github/workflows/run-entry-points.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-name: mypy
+name: run entry points
 
 on:
   push:
   pull_request:
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: ["3.9", "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v2
-    - name: Setup Python 3.x
+    - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
+      with:
+        python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install setuptools==67.8.0
         python -m pip install --upgrade pip!=22.1.*
-        python -m pip install --upgrade mypy
-        python -m pip install --upgrade pandas-stubs
-        python -m pip install --upgrade types-appdirs
-        python -m pip install --upgrade wheel pytest numpy flit
+        python -m pip install --upgrade hatchling
+        python -m pip install --upgrade wheel pytest numpy
         python -m pip install --upgrade appdirs click happi pandas bluesky suitcase-csv matplotlib
         python -m pip install . --no-build-isolation
-    - name: Run mypy
+    - name: Test with pytest
       run: |
-        mypy auto_rxn
+        auto_rxn --version
+        auto_rxn --help
```

### Comparing `auto_rxn-2023.7.0/.github/workflows/python-publish.yml` & `auto_rxn-2023.8.0/.github/workflows/python-pytest.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-# This workflows will upload a Python Package using flit when a release is created
-# For more information see: https://help.github.com/en/actions/language-and-framework-guides/using-python-with-github-actions#publishing-to-package-registries
-
-name: Upload Python Package
+name: pytest
 
 on:
-  release:
-    types: [created]
+  push:
+  pull_request:
 
 jobs:
-  deploy:
+  build:
 
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: ["3.9", "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v2
-    - name: Set up Python
+    - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
-        python-version: '3.x'
+        python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install setuptools==67.8.0
         python -m pip install --upgrade pip!=22.1.*
-        python -m pip install --upgrade wheel pytest numpy flit
+        python -m pip install --upgrade hatchling
+        python -m pip install --upgrade wheel pytest numpy
         python -m pip install --upgrade appdirs click happi pandas bluesky suitcase-csv matplotlib
         python -m pip install . --no-build-isolation
-    - name: Build and publish
-      env:
-        FLIT_USERNAME: ${{ secrets.PYPI_USERNAME }}
-        FLIT_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
-      run: flit publish
+    - name: Pytest
+      run: |
+        cd tests
+        pytest
+
```

### Comparing `auto_rxn-2023.7.0/CHANGELOG.md` & `auto_rxn-2023.8.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/).
 
 ## [Unreleased]
 
+## [2023.8.0]
+
+### Fixed
+- complete refactor of limits behavior, doesn't force metadata into happi anymore
+
 ## [2023.7.0]
 
 ### Added
 - actually check safety limits within SafetyCallback
 - support for child devices
 - support for fallback position
 
@@ -34,13 +39,14 @@
 - minimum viable can actually run reactions via Bluesky
 
 ## [2023.4.0]
 
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/uw-madison-chem-shops/auto_rxn/-/compare/v2023.7.0...main
-[2023.7.0]: https://github.com/uw-madison-chem-shops/auto_rxn/-/compare/v2023.6.1...2023.7.0
-[2023.6.1]: https://github.com/uw-madison-chem-shops/auto_rxn/-/compare/v2023.6.0...2023.6.1
-[2023.6.0]: https://github.com/uw-madison-chem-shops/auto_rxn/-/compare/v2023.4.0...2023.6.0
+[Unreleased]: https://github.com/uw-madison-chem-shops/auto_rxn/-/compare/v2023.8.0...main
+[2023.8.0]: https://github.com/uw-madison-chem-shops/auto_rxn/-/compare/v2023.7.0...v2023.8.0
+[2023.7.0]: https://github.com/uw-madison-chem-shops/auto_rxn/-/compare/v2023.6.1...v2023.7.0
+[2023.6.1]: https://github.com/uw-madison-chem-shops/auto_rxn/-/compare/v2023.6.0...v2023.6.1
+[2023.6.0]: https://github.com/uw-madison-chem-shops/auto_rxn/-/compare/v2023.4.0...v2023.6.0
 [2023.4.0]: https://github.com/uw-madison-chem-shops/auto_rxn/-/tags/v2023.4.0
```

### Comparing `auto_rxn-2023.7.0/LICENSE` & `auto_rxn-2023.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_rxn-2023.7.0/README.md` & `auto_rxn-2023.8.0/README.md`

 * *Files identical despite different names*

### Comparing `auto_rxn-2023.7.0/auto_rxn/__main__.py` & `auto_rxn-2023.8.0/auto_rxn/__main__.py`

 * *Files identical despite different names*

### Comparing `auto_rxn-2023.7.0/auto_rxn/_exceptions.py` & `auto_rxn-2023.8.0/auto_rxn/_exceptions.py`

 * *Files identical despite different names*

### Comparing `auto_rxn-2023.7.0/auto_rxn/_recipe.py` & `auto_rxn-2023.8.0/auto_rxn/_recipe.py`

 * *Files identical despite different names*

### Comparing `auto_rxn-2023.7.0/auto_rxn/_run.py` & `auto_rxn-2023.8.0/auto_rxn/_run.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import bluesky
 from bluesky.callbacks.best_effort import BestEffortCallback
 from bluesky.utils import RequestStop
 from suitcase.csv import Serializer  # type: ignore
 import numpy as np
 
 from ._device import load_device
-from ._safety import SafetyCallback
+from ._limits import LimitsChecker, limits
 
 
 def run(recipe):
     RE = bluesky.RunEngine()
 
     devices = dict()
     for id in recipe.control_point_ids:
@@ -37,36 +37,37 @@
     datadir.mkdir(exist_ok=True, parents=True)
     RE.subscribe(Serializer(datadir, flush=True))
     recipe.save(datadir / "recipe.csv")
     from ._device import db_path
 
     shutil.copyfile(db_path, datadir / "db.json")
 
-    safety = SafetyCallback(devices)
+    safety = LimitsChecker(devices)
     safety_token = RE.subscribe(safety, "all")
 
     def plan():
         @bluesky.preprocessors.stage_decorator(all_devices)
         @bluesky.preprocessors.run_decorator()
         def inner_plan():
             for step, fallback_positions in zip(recipe.steps, recipe.fallback_positions):
                 # set fallback positions
                 for id, val in fallback_positions.setpoints.items():
-                    devices[id].set_fallback_position(val)
+                    limits.set_fallback(id, val)
 
                 # set positions
                 nestargs = [(devices[id], float(val)) for id, val in step.setpoints.items()]
                 yield from bluesky.plan_stubs.mv(*itertools.chain(*nestargs))
 
                 def fallback_to_safety(exception):
+                    print("FALLBack", exception)
                     RE.unsubscribe(safety_token)  # don't want to keep raising
                     nestargs = list()
-                    for device in devices.values():
-                        fallback = device.get_fallback_position()
-                        if fallback is not None:
+                    for name, device in devices.items():
+                        fallback = limits.get_fallback(name)
+                        if not np.isnan(fallback):
                             nestargs.append((device, fallback))
                     if nestargs:
                         yield from bluesky.plan_stubs.mv(*itertools.chain(*nestargs))
                     # keep recording data for 100 more seconds
                     yield from bluesky.plan_stubs.repeat(
                         functools.partial(bluesky.plan_stubs.one_shot, all_devices),
                         num=int(100),
```

### Comparing `auto_rxn-2023.7.0/auto_rxn/_safety.py` & `auto_rxn-2023.8.0/auto_rxn/_safety.py`

 * *Files identical despite different names*

### Comparing `auto_rxn-2023.7.0/auto_rxn/_testing.py` & `auto_rxn-2023.8.0/auto_rxn/testing/_with_happi_db.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 __all__ = ["with_happi_db"]
 
 
 import pathlib
 
-import appdirs
+import platformdirs
 import happi  # type: ignore
 
-from . import _device as auto_rxn_happi
+from .. import _device as auto_rxn_happi
 
 
 def with_happi_db(path):
     def decorator(function):
         def wrapper():
             # make happi client
             auto_rxn_happi.db_path = path
             auto_rxn_happi.happi_backend = happi.backends.backend(path)
             auto_rxn_happi.happi_client = happi.Client(database=auto_rxn_happi.happi_backend)
             auto_rxn_happi.device_singletons = dict()
 
             function()
 
             # make happi client
-            auto_rxn_happi.db_path = pathlib.Path(appdirs.user_data_dir("happi")) / "db.json"
-            db_path = pathlib.Path(appdirs.user_data_dir("happi")) / "db.json"
+            auto_rxn_happi.db_path = platformdirs.user_data_path("happi") / "db.json"
+            db_path = platformdirs.user_data_path("happi") / "db.json"
             auto_rxn_happi.happi_backend = happi.backends.backend(db_path)
             auto_rxn_happi.happi_client = happi.Client(database=auto_rxn_happi.happi_backend)
 
         return wrapper
 
     return decorator
```

### Comparing `auto_rxn-2023.7.0/auto_rxn/devices/_fake_furnace.py` & `auto_rxn-2023.8.0/auto_rxn/devices/_fake_furnace.py`

 * *Files identical despite different names*

### Comparing `auto_rxn-2023.7.0/auto_rxn/devices/_fake_mfc.py` & `auto_rxn-2023.8.0/auto_rxn/devices/_fake_mfc.py`

 * *Files identical despite different names*

### Comparing `auto_rxn-2023.7.0/auto_rxn/devices/_status.py` & `auto_rxn-2023.8.0/auto_rxn/devices/_status.py`

 * *Files identical despite different names*

### Comparing `auto_rxn-2023.7.0/pyproject.toml` & `auto_rxn-2023.8.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,57 @@
 [build-system]
-requires = ["flit_core >=2,<4"]
-build-backend = "flit_core.buildapi"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
-[tool.flit.metadata]
-module = "auto_rxn"
-dist-name = "auto_rxn"
+[project]
+name = "auto_rxn"
 author = "auto_rxn developers"
-home-page = "https://github.com/uw-madison-chem-shops/auto_rxn"
-description-file = "README.md"
 requires-python = ">=3.9"
-requires = ["appdirs",
-            "click",
-            "happi",
-            "pandas",
-            "bluesky",
-            "suitcase-csv",
-            ]
+readme = "README.md"
+dynamic = ["version"]
+license = "MIT"
+dependencies = ["platformdirs",
+                "click",
+                "happi",
+                "pandas",
+                "bluesky",
+                "suitcase-csv",
+	        "tomli",
+      	        "tomli-w",
+                 ]
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
-    "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
+    "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 
-[tool.flit.metadata.urls]
+[project.urls]
 Source = "https://github.com/uw-madison-chem-shops/auto_rxn"
 Issues = "https://github.com/uw-madison-chem-shops/auto_rxn/issues"
+"Home Page" = "https://github.com/uw-madison-chem-shops/auto_rxn"
 
 [tool.flit.metadata.requires-extra]
 dev = ["black", "pre-commit"]
 
-[tool.flit.scripts]
+[project.scripts]
 auto_rxn = "auto_rxn.__main__:main"
 
 [tool.flit.entrypoints."happi.containers"]
 fake_furnace = "auto_rxn.devices._fake_furnace"
 fake_mfc = "auto_rxn.devices._fake_mfc"
 
+[tool.hatch.version]
+path = "auto_rxn/__version__.py"
+
 [tool.black]
 line-length = 99
 target-version = ['py311']
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
```

### Comparing `auto_rxn-2023.7.0/tests/children/db.json` & `auto_rxn-2023.8.0/tests/minimal_csv/db.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807692307692308%*

 * *Differences: {"'myfurnace'": "{'last_edit': 'Thu Aug  3 17:13:15 2023'}",*

 * * "'mymfc'": "{'last_edit': 'Thu Aug  3 17:13:15 2023'}"}*

```diff
@@ -8,15 +8,15 @@
         "auto_rxn_upper_safety_limit": null,
         "creation": "Thu Jun  8 15:05:57 2023",
         "device_class": "auto_rxn.devices.FakeFurnace",
         "documentation": null,
         "kwargs": {
             "name": "{{name}}"
         },
-        "last_edit": "Mon Jul 31 06:02:12 2023",
+        "last_edit": "Thu Aug  3 17:13:15 2023",
         "name": "myfurnace",
         "type": "fake_furnace.devices._fake_furnace.FakeFurnaceItem"
     },
     "mymfc": {
         "_id": "mymfc",
         "active": true,
         "args": [],
@@ -25,12 +25,12 @@
         "auto_rxn_upper_safety_limit": null,
         "creation": "Fri Apr 14 16:44:36 2023",
         "device_class": "auto_rxn.devices.FakeMFC",
         "documentation": null,
         "kwargs": {
             "name": "{{name}}"
         },
-        "last_edit": "Mon Jul 31 06:02:13 2023",
+        "last_edit": "Thu Aug  3 17:13:15 2023",
         "name": "mymfc",
         "type": "fake_mfc.devices._fake_mfc.FakeMFCItem"
     }
 }
```

### Comparing `auto_rxn-2023.7.0/tests/fallback_position/db.json` & `auto_rxn-2023.8.0/tests/fallback_position/db.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807692307692308%*

 * *Differences: {"'myfurnace'": "{'last_edit': 'Thu Aug  3 17:23:39 2023'}",*

 * * "'mymfc'": "{'last_edit': 'Thu Aug  3 17:23:39 2023'}"}*

```diff
@@ -8,15 +8,15 @@
         "auto_rxn_upper_safety_limit": 200.0,
         "creation": "Thu Jun  8 15:05:57 2023",
         "device_class": "auto_rxn.devices.FakeFurnace",
         "documentation": null,
         "kwargs": {
             "name": "{{name}}"
         },
-        "last_edit": "Mon Jul 31 06:02:49 2023",
+        "last_edit": "Thu Aug  3 17:23:39 2023",
         "name": "myfurnace",
         "type": "fake_furnace.devices._fake_furnace.FakeFurnaceItem"
     },
     "mymfc": {
         "_id": "mymfc",
         "active": true,
         "args": [],
@@ -25,12 +25,12 @@
         "auto_rxn_upper_safety_limit": null,
         "creation": "Fri Apr 14 16:44:36 2023",
         "device_class": "auto_rxn.devices.FakeMFC",
         "documentation": null,
         "kwargs": {
             "name": "{{name}}"
         },
-        "last_edit": "Mon Jul 31 06:02:37 2023",
+        "last_edit": "Thu Aug  3 17:23:39 2023",
         "name": "mymfc",
         "type": "fake_mfc.devices._fake_mfc.FakeMFCItem"
     }
 }
```

### Comparing `auto_rxn-2023.7.0/tests/minimal_csv/db.json` & `auto_rxn-2023.8.0/tests/children/db.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807692307692308%*

 * *Differences: {"'myfurnace'": "{'last_edit': 'Thu Aug  3 17:23:14 2023'}",*

 * * "'mymfc'": "{'last_edit': 'Thu Aug  3 17:23:15 2023'}"}*

```diff
@@ -8,15 +8,15 @@
         "auto_rxn_upper_safety_limit": null,
         "creation": "Thu Jun  8 15:05:57 2023",
         "device_class": "auto_rxn.devices.FakeFurnace",
         "documentation": null,
         "kwargs": {
             "name": "{{name}}"
         },
-        "last_edit": "Mon Jul 31 06:04:30 2023",
+        "last_edit": "Thu Aug  3 17:23:14 2023",
         "name": "myfurnace",
         "type": "fake_furnace.devices._fake_furnace.FakeFurnaceItem"
     },
     "mymfc": {
         "_id": "mymfc",
         "active": true,
         "args": [],
@@ -25,12 +25,12 @@
         "auto_rxn_upper_safety_limit": null,
         "creation": "Fri Apr 14 16:44:36 2023",
         "device_class": "auto_rxn.devices.FakeMFC",
         "documentation": null,
         "kwargs": {
             "name": "{{name}}"
         },
-        "last_edit": "Mon Jul 31 06:04:30 2023",
+        "last_edit": "Thu Aug  3 17:23:15 2023",
         "name": "mymfc",
         "type": "fake_mfc.devices._fake_mfc.FakeMFCItem"
     }
 }
```

### Comparing `auto_rxn-2023.7.0/PKG-INFO` & `auto_rxn-2023.8.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: auto_rxn
-Version: 2023.7.0
-Summary: Python package for running chemical reactions as defined by recipe files.
-Home-page: https://github.com/uw-madison-chem-shops/auto_rxn
-Author: auto_rxn developers
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Classifier: Development Status :: 2 - Pre-Alpha
+Version: 2023.8.0
+Project-URL: Source, https://github.com/uw-madison-chem-shops/auto_rxn
+Project-URL: Issues, https://github.com/uw-madison-chem-shops/auto_rxn/issues
+Project-URL: Home Page, https://github.com/uw-madison-chem-shops/auto_rxn
+License-Expression: MIT
+License-File: LICENSE
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: appdirs
+Requires-Python: >=3.9
+Requires-Dist: bluesky
 Requires-Dist: click
 Requires-Dist: happi
 Requires-Dist: pandas
-Requires-Dist: bluesky
+Requires-Dist: platformdirs
 Requires-Dist: suitcase-csv
-Requires-Dist: black ; extra == "dev"
-Requires-Dist: pre-commit ; extra == "dev"
-Project-URL: Issues, https://github.com/uw-madison-chem-shops/auto_rxn/issues
-Project-URL: Source, https://github.com/uw-madison-chem-shops/auto_rxn
-Provides-Extra: dev
+Requires-Dist: tomli
+Requires-Dist: tomli-w
+Description-Content-Type: text/markdown
 
 # auto_rxn
 
 [![PyPI](https://img.shields.io/pypi/v/auto_rxn)](https://pypi.org/project/auto_rxn)
 [![Conda](https://img.shields.io/conda/vn/conda-forge/auto_rxn)](https://anaconda.org/conda-forge/auto_rxn)
 [![log](https://img.shields.io/badge/change-log-informational)](https://github.com/uw-madison-chem-shops/auto_rxn/-/blob/main/CHANGELOG.md)
 
@@ -61,8 +60,7 @@
 ## recipe files
 
 must have metadata:
 - `Control Point ID` (e.g. auto_rxn:FakeMFC)
 
 optional metadata
 - control point name
-
```

