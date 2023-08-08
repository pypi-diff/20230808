# Comparing `tmp/hdxms_datasets-0.1.2.tar.gz` & `tmp/hdxms_datasets-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdxms_datasets-0.1.2.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `hdxms_datasets-0.1.2.tar` & `hdxms_datasets-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,50 @@
--rw-r--r--   0        0        0     1073 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/LICENSE
--rw-r--r--   0        0        0      574 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/README.md
--rw-r--r--   0        0        0      388 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/hdxms_datasets/__init__.py
--rw-r--r--   0        0        0      281 2023-07-14 09:57:11.381758 hdxms_datasets-0.1.2/hdxms_datasets/__version__.py
--rw-r--r--   0        0        0     4029 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/hdxms_datasets/config.py
--rw-r--r--   0        0        0      171 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/hdxms_datasets/config.yaml
--rw-r--r--   0        0        0     7200 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/hdxms_datasets/datasets.py
--rw-r--r--   0        0        0     4652 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/hdxms_datasets/datavault.py
--rw-r--r--   0        0        0     4102 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/hdxms_datasets/process.py
--rw-r--r--   0        0        0     1215 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/hdxms_datasets/reader.py
--rw-r--r--   0        0        0     1594 2023-07-14 09:57:11.377758 hdxms_datasets-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 hdxms_datasets-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/.editorconfig
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/.gitattributes
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/MANIFEST.in
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/dependabot.yml
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/mkdocs.yml
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/.github/workflows/pin_requirements.yml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/.github/workflows/pypi_main.yml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/.github/workflows/pypi_test.yml
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/docs/index.md
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/docs/install.md
+-rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/docs/css/styles.css
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/docs/usage/configuration.md
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/docs/usage/loading.md
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/examples/load_datasets.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/examples/load_from_yaml.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/examples/load_local_datasets.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/examples/load_to_pyhdx.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/examples/update_config.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/hdxms_datasets/__init__.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/hdxms_datasets/__version__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/hdxms_datasets/_version.py
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/hdxms_datasets/config.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/hdxms_datasets/config.yaml
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/hdxms_datasets/datasets.py
+-rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/hdxms_datasets/datavault.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/hdxms_datasets/process.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/hdxms_datasets/reader.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/requirements/requirements-macOS-latest-3.10.txt
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/requirements/requirements-macOS-latest-3.9.txt
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/requirements/requirements-ubuntu-latest-3.10.txt
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/requirements/requirements-ubuntu-latest-3.9.txt
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/requirements/requirements-windows-latest-3.10.txt
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/requirements/requirements-windows-latest-3.9.txt
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/tests/test_hdxms_datasets.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/tests/datasets/index.txt
+-rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/tests/datasets/20221007_1530_SecA_Krishnamurthy/hdx_spec.yaml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/tests/datasets/20221007_1530_SecA_Krishnamurthy/metadata.yaml
+-rw-r--r--   0        0        0  1118033 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/tests/datasets/20221007_1530_SecA_Krishnamurthy/data/SecA.csv
+-rw-r--r--   0        0        0   168734 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/tests/test_data/monomer_experimental_peptides.csv
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/.gitignore
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/AUTHORS.rst
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/LICENSE
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/README.md
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 hdxms_datasets-0.1.3/PKG-INFO
```

### Comparing `hdxms_datasets-0.1.2/LICENSE` & `hdxms_datasets-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hdxms_datasets-0.1.2/README.md` & `hdxms_datasets-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hdxms_datasets-0.1.2/hdxms_datasets/config.py` & `hdxms_datasets-0.1.3/hdxms_datasets/config.py`

 * *Files identical despite different names*

### Comparing `hdxms_datasets-0.1.2/hdxms_datasets/datasets.py` & `hdxms_datasets-0.1.3/hdxms_datasets/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,17 @@
 
     metadata: Optional[dict] = field(default_factory=dict)
     """Optional metadata"""
 
     _cache: dict[tuple[str, str], pd.DataFrame] = field(init=False, default_factory=dict)
 
     @classmethod
-    def from_spec(cls, hdx_spec: dict, data_dir: Path, data_id = Optional[str], metadata: Optional[dict] = None):
+    def from_spec(
+        cls, hdx_spec: dict, data_dir: Path, data_id=Optional[str], metadata: Optional[dict] = None
+    ):
         metadata = metadata or {}
         data_id = data_id or uuid.uuid4().hex
         data_files = parse_data_files(hdx_spec["data_files"], data_dir)
 
         return cls(data_id, data_files, hdx_spec, metadata)
 
     @property
```

### Comparing `hdxms_datasets-0.1.2/hdxms_datasets/datavault.py` & `hdxms_datasets-0.1.3/hdxms_datasets/datavault.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,9 +142,9 @@
         hdx_spec = yaml.safe_load((self.cache_dir / data_id / "hdx_spec.yaml").read_text())
         dataset_metadata = yaml.safe_load((self.cache_dir / data_id / "metadata.yaml").read_text())
 
         return HDXDataSet.from_spec(
             hdx_spec=hdx_spec,
             data_dir=self.cache_dir / data_id,
             data_id=data_id,
-            metadata=dataset_metadata
+            metadata=dataset_metadata,
         )
```

### Comparing `hdxms_datasets-0.1.2/hdxms_datasets/process.py` & `hdxms_datasets-0.1.3/hdxms_datasets/process.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Literal, Optional, Union, TypeVar, TYPE_CHECKING
+from typing import Literal, Optional, Union, TYPE_CHECKING
 
-import numpy.typing as npt
 import pandas as pd
 
 from hdxms_datasets.config import cfg
 
 if TYPE_CHECKING:
     from hdxms_datasets import DataFile
 
 
 TIME_FACTORS = {"s": 1, "m": 60.0, "min": 60.0, "h": 3600, "d": 86400}
 TEMPERATURE_OFFSETS = {"c": 273.15, "celsius": 273.15, "k": 0.0, "kelvin": 0.0}
 
-A = TypeVar("A", npt.ArrayLike, pd.Series, pd.DataFrame)
-
 
 def convert_temperature(
     temperature_dict: dict, target_unit: str = "c"
 ) -> Union[float, list[float]]:
     """
     Convenience function to convert temperature values.
```

### Comparing `hdxms_datasets-0.1.2/hdxms_datasets/reader.py` & `hdxms_datasets-0.1.3/hdxms_datasets/reader.py`

 * *Files identical despite different names*

### Comparing `hdxms_datasets-0.1.2/pyproject.toml` & `hdxms_datasets-0.1.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,75 @@
+[build-system]
+requires = ["hatchling", "hatch-vcs"]
+build-backend = "hatchling.build"
+
 [project]
+name = "hdxms-datasets"
+description = "Download and parse curated HDX-MS datasets"
+authors = [
+  { name = "Jochem Smit", email = "jhsmit@gmail.com" },
+]
+readme = "README.md"
+license = "MIT"
+requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Intended Audience :: Science/Research",
 ]
 
+dependencies = [
+    "omegaconf",
+    "pandas",
+    "PyYAML",
+    "requests",
+    "packaging",
+]
+
+dynamic = ["version"]
+
+[project.optional-dependencies]
+docs = [
+    "mkdocs>=1.4.2",
+    "mkdocstrings[python]>=0.19.1",
+    "mkdocs-material>=8.5.11",
+    "pygments>=2.13.0",
+    "mkdocs-gen-files>=0.4.0",
+    "mkdocs-literate-nav>=0.5.0",
+    "mkdocs-jupyter>=0.22.0",
+    "jupyter>=1.0.0"
+]
+dev = [
+    "black[jupyter]>=22.12.0",
+]
+
+test = [
+    "pytest>=7.2.0",
+]
+
 [project.urls]
-repository = "https://github.com/Jhsmit/hdxms-datasets/"
-documentation = "https://jhsmit.github.io/hdxms-datasets/"
+Source = "https://github.com/Jhsmit/hdxms-datasets/"
+Documentation = "https://jhsmit.github.io/hdxms-datasets/"
+
+[tool.hatch.build]
+exclude = [
+    "_versioneer.py"
+]
+
+[tool.hatch.version]
+source = "vcs"
+
+[tool.hatch.build.hooks.vcs]
+version-file = "hdxms_datasets/_version.py"
 
 [tool.flake8]
 max-line-length = 100
 ignore = "D203"
 exclude = [".git", "__pycache__", "build", "dist", "docs"]
 max-complexity = 10
 
 [tool.black]
 line-length = 100
 
-[tool.poetry]
-name = "hdxms-datasets"
-version = "0.1.2" # placeholder
-description = "Download and parse curated HDX-MS datasets"
-authors = ["Jochem Smit <jhsmit@gmail.com>"]
-license = "MIT"
-readme = "README.md"
-packages = [{include = "hdxms_datasets"}]
-exclude = ["hdxms_datasets/_version.py"]
-
-
-[tool.poetry.dependencies]
-python = "^3.9"
-omegaconf = "^2.3.0"
-pandas = "^1.5.2"
-PyYAML = "^6.0"
-requests = "^2.28.1"
-packaging = "^22.0"
-
-
-[tool.poetry.group.dev.dependencies]
-black = "^22.12.0"
-pytest = "^7.2.0"
-mypy = "^0.991"
-pylint = "^2.15.9"
-poetry-dynamic-versioning = {extras = ["plugin"], version = "^0.21.2"}
-ipykernel = "^6.24.0"
-
-
-[tool.poetry.group.docs.dependencies]
-mkdocs = "^1.4.2"
-mkdocstrings = {extras = ["python"], version = "^0.19.1"}
-mkdocs-material = "^8.5.11"
-pygments = "^2.13.0"
-mkdocs-gen-files = "^0.4.0"
-mkdocs-literate-nav = "^0.5.0"
-
-[tool.poetry-dynamic-versioning]
-enable = false
-vcs = "git"
-style = "pep440"
-metadata = false
-
-[build-system]
-requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
-build-backend = "poetry_dynamic_versioning.backend"
-
+[tool.ruff]
+line-length = 100
```

