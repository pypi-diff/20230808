# Comparing `tmp/digiflow-3.0.1.tar.gz` & `tmp/digiflow-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digiflow-3.0.1.tar", last modified: Fri Jul 28 14:27:40 2023, max compression
+gzip compressed data, was "digiflow-3.1.0.tar", last modified: Tue Aug  8 12:25:44 2023, max compression
```

## Comparing `digiflow-3.0.1.tar` & `digiflow-3.1.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.358120 digiflow-3.0.1/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1106 2023-07-03 13:56:57.000000 digiflow-3.0.1/LICENCE
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      205 2023-07-04 08:42:32.000000 digiflow-3.0.1/MANIFEST.in
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1728 2023-07-28 14:27:40.358120 digiflow-3.0.1/PKG-INFO
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1260 2023-07-04 12:02:04.000000 digiflow-3.0.1/README.md
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      709 2023-07-28 14:27:28.000000 digiflow-3.0.1/pyproject.toml
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       38 2023-07-28 14:27:40.358120 digiflow-3.0.1/setup.cfg
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.342120 digiflow-3.0.1/src/
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.346120 digiflow-3.0.1/src/digiflow/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      509 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/__init__.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    12685 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/digflow_identifier.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    10920 2023-07-04 07:12:14.000000 digiflow-3.0.1/src/digiflow/digiflow_export.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    11390 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/digiflow_generate.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    39028 2023-07-28 14:25:35.000000 digiflow-3.0.1/src/digiflow/digiflow_io.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    31754 2023-07-03 13:49:57.000000 digiflow-3.0.1/src/digiflow/digiflow_metadata.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    12200 2023-07-04 08:47:08.000000 digiflow-3.0.1/src/digiflow/digiflow_validate.py
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.346120 digiflow-3.0.1/src/digiflow/resources/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     2676 2023-07-04 07:49:18.000000 digiflow-3.0.1/src/digiflow/resources/digilife.ini
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.346120 digiflow-3.0.1/src/digiflow/resources/sch/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   162203 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/sch/ddb_validierung_mets-mods-ap-digitalisierte-medien.sch
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   125014 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/sch/ddb_validierung_mets-mods-ap-digitalisierte-zeitungen.sch
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.346120 digiflow-3.0.1/src/digiflow/resources/xsd/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    55541 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/xsd/alto_4-2.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   135665 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/xsd/mets_1-12.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    98153 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/xsd/mix_2-0.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    52954 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/xsd/mods_3-7.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    88414 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/xsd/page_2019-07-15.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     3180 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/xsd/xlink.xsd
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5840 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/resources/xsd/xml.xsd
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.346120 digiflow-3.0.1/src/digiflow/schematron/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)  7072788 2023-07-03 13:38:30.000000 digiflow-3.0.1/src/digiflow/schematron/schxslt-cli.jar
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.346120 digiflow-3.0.1/src/digiflow.egg-info/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1728 2023-07-28 14:27:40.000000 digiflow-3.0.1/src/digiflow.egg-info/PKG-INFO
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1148 2023-07-28 14:27:40.000000 digiflow-3.0.1/src/digiflow.egg-info/SOURCES.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        1 2023-07-28 14:27:40.000000 digiflow-3.0.1/src/digiflow.egg-info/dependency_links.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       27 2023-07-28 14:27:40.000000 digiflow-3.0.1/src/digiflow.egg-info/requires.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        9 2023-07-28 14:27:40.000000 digiflow-3.0.1/src/digiflow.egg-info/top_level.txt
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-07-28 14:27:40.358120 digiflow-3.0.1/tests/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    12481 2023-07-04 07:12:14.000000 digiflow-3.0.1/tests/test_digiflow_generate.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    21727 2023-07-04 07:12:14.000000 digiflow-3.0.1/tests/test_digiflow_identifier.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    54615 2023-07-04 07:12:14.000000 digiflow-3.0.1/tests/test_digiflow_io.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    22460 2023-07-04 07:50:20.000000 digiflow-3.0.1/tests/test_digiflow_metadata.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    18594 2023-07-04 08:44:03.000000 digiflow-3.0.1/tests/test_digiflow_validate.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    15559 2023-07-04 07:12:14.000000 digiflow-3.0.1/tests/test_export_saf.py
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-08-08 12:25:44.333133 digiflow-3.1.0/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1106 2023-07-03 13:56:57.000000 digiflow-3.1.0/LICENCE
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      205 2023-07-04 08:42:32.000000 digiflow-3.1.0/MANIFEST.in
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1728 2023-08-08 12:25:44.333133 digiflow-3.1.0/PKG-INFO
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1260 2023-07-04 12:02:04.000000 digiflow-3.1.0/README.md
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      720 2023-08-07 05:42:32.000000 digiflow-3.1.0/pyproject.toml
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       38 2023-08-08 12:25:44.333133 digiflow-3.1.0/setup.cfg
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-08-08 12:25:44.297133 digiflow-3.1.0/src/
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-08-08 12:25:44.297133 digiflow-3.1.0/src/digiflow/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      509 2023-07-03 13:38:30.000000 digiflow-3.1.0/src/digiflow/__init__.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    12685 2023-07-03 13:38:30.000000 digiflow-3.1.0/src/digiflow/digflow_identifier.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    10920 2023-07-04 07:12:14.000000 digiflow-3.1.0/src/digiflow/digiflow_export.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    16820 2023-08-08 11:38:16.000000 digiflow-3.1.0/src/digiflow/digiflow_generate.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    39028 2023-07-28 14:25:35.000000 digiflow-3.1.0/src/digiflow/digiflow_io.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    31754 2023-07-03 13:49:57.000000 digiflow-3.1.0/src/digiflow/digiflow_metadata.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    12200 2023-07-04 08:47:08.000000 digiflow-3.1.0/src/digiflow/digiflow_validate.py
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-08-08 12:25:44.301133 digiflow-3.1.0/src/digiflow/resources/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     2676 2023-07-04 07:49:18.000000 digiflow-3.1.0/src/digiflow/resources/digilife.ini
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-08-08 12:25:44.301133 digiflow-3.1.0/src/digiflow/resources/sch/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   162203 2023-07-03 13:38:30.000000 digiflow-3.1.0/src/digiflow/resources/sch/ddb_validierung_mets-mods-ap-digitalisierte-medien.sch
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   125014 2023-07-03 13:38:30.000000 digiflow-3.1.0/src/digiflow/resources/sch/ddb_validierung_mets-mods-ap-digitalisierte-zeitungen.sch
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-08-08 12:25:44.309133 digiflow-3.1.0/src/digiflow/resources/xsd/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    55541 2023-07-03 13:38:30.000000 digiflow-3.1.0/src/digiflow/resources/xsd/alto_4-2.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)   135665 2023-07-03 13:38:30.000000 digiflow-3.1.0/src/digiflow/resources/xsd/mets_1-12.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    98153 2023-07-03 13:38:30.000000 digiflow-3.1.0/src/digiflow/resources/xsd/mix_2-0.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    52954 2023-07-03 13:38:30.000000 digiflow-3.1.0/src/digiflow/resources/xsd/mods_3-7.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    88414 2023-07-03 13:38:30.000000 digiflow-3.1.0/src/digiflow/resources/xsd/page_2019-07-15.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     3180 2023-07-03 13:38:30.000000 digiflow-3.1.0/src/digiflow/resources/xsd/xlink.xsd
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5840 2023-07-03 13:38:30.000000 digiflow-3.1.0/src/digiflow/resources/xsd/xml.xsd
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-08-08 12:25:44.309133 digiflow-3.1.0/src/digiflow/schematron/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)  7072788 2023-07-03 13:38:30.000000 digiflow-3.1.0/src/digiflow/schematron/schxslt-cli.jar
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-08-08 12:25:44.301133 digiflow-3.1.0/src/digiflow.egg-info/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1728 2023-08-08 12:25:44.000000 digiflow-3.1.0/src/digiflow.egg-info/PKG-INFO
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1148 2023-08-08 12:25:44.000000 digiflow-3.1.0/src/digiflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        1 2023-08-08 12:25:44.000000 digiflow-3.1.0/src/digiflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       34 2023-08-08 12:25:44.000000 digiflow-3.1.0/src/digiflow.egg-info/requires.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        9 2023-08-08 12:25:44.000000 digiflow-3.1.0/src/digiflow.egg-info/top_level.txt
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-08-08 12:25:44.329133 digiflow-3.1.0/tests/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    13100 2023-08-08 11:38:16.000000 digiflow-3.1.0/tests/test_digiflow_generate.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    21727 2023-07-04 07:12:14.000000 digiflow-3.1.0/tests/test_digiflow_identifier.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    54571 2023-08-07 08:09:47.000000 digiflow-3.1.0/tests/test_digiflow_io.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    22460 2023-07-04 07:50:20.000000 digiflow-3.1.0/tests/test_digiflow_metadata.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    18594 2023-07-04 08:44:03.000000 digiflow-3.1.0/tests/test_digiflow_validate.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    15559 2023-08-08 11:38:09.000000 digiflow-3.1.0/tests/test_export_saf.py
```

### Comparing `digiflow-3.0.1/LICENCE` & `digiflow-3.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/PKG-INFO` & `digiflow-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digiflow
-Version: 3.0.1
+Version: 3.1.0
 Summary: Father's Little Digitization Workflow Helper
 Author-email: Universitäts- und Landesbibliothek Sachsen-Anhalt <development@bibliothek.uni-halle.de>
 Project-URL: Homepage, https://github.com/ulb-sachsen-anhalt/digital-flow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `digiflow-3.0.1/README.md` & `digiflow-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/pyproject.toml` & `digiflow-3.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digiflow"
-version = "3.0.1"
+version = "3.1.0"
 description = "Father's Little Digitization Workflow Helper"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
 	{name = "Universitäts- und Landesbibliothek Sachsen-Anhalt", email = "development@bibliothek.uni-halle.de"}
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License"
 ]
 dependencies = [
 	"lxml",
 	"Pillow",
 	"numpy",
+	"docker",
 	"requests"
 ]
 
 [project.urls]
 Homepage = "https://github.com/ulb-sachsen-anhalt/digital-flow"
 
 [tool.setuptools]
```

### Comparing `digiflow-3.0.1/src/digiflow/digflow_identifier.py` & `digiflow-3.1.0/src/digiflow/digflow_identifier.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/src/digiflow/digiflow_export.py` & `digiflow-3.1.0/src/digiflow/digiflow_export.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/src/digiflow/digiflow_generate.py` & `digiflow-3.1.0/src/digiflow/digiflow_generate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,53 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
 
 import itertools
 import os
 import pathlib
 import platform
 import re
 import shutil
 import subprocess
 import time
+from abc import abstractmethod, ABC
+from dataclasses import dataclass
 
-import numpy as np
 from pathlib import Path
 
 from typing import (
-    List
+    List,
+    Tuple,
+    Union,
+    Final, Callable, Any, TypeVar, Generic,
 )
 
 from PIL import (
     Image
 )
 
+import numpy as np
+
+from docker import (
+    DockerClient,
+    from_env
+)
+from docker.models.containers import Container
+from docker.models.resource import Model
+from docker.types import Mount
 
 # default sub dir for structure creation
 DEFAULT_STRUCTURE_DIR = 'MAX'
 
 # derivates
+DEFAULT_DERIVANS_IMAGE = "ghcr.io/ulb-sachsen-anhalt/digital-derivans:latest"
 DEFAULT_DERIVANS_TIMEOUT = 10800
 DERIVANS_LABEL = 'derivans'
+DERIVANS_CNT_DATA_DIR: Final[str] = "/data_mets"
+DERIVANS_CNT_CONF_DIR: Final[str] = "/data_cfg"
 
 
 def id_generator(
         start=0, prefix=None, suffix=None, previous_value=None, padded=4):
     """
     Generate Numbers with schema [<prefix>]<4digits>[<suffix>]
     with default padded zeros to match 4-digit-numbers
@@ -145,17 +162,23 @@
     def _get_paths(self, start, number, padded=8, previous_value=None):
         self.name_generator = id_generator(
             start, previous_value=previous_value, padded=padded)
         names = list(itertools.islice(self.name_generator, number))
         return [os.path.join(self.path, n + self.blueprint.ext) for n in names]
 
 
-def generate_structure(start_dir,
-                       gens=[ResourceGenerator(DEFAULT_STRUCTURE_DIR)],
-                       number=10) -> List[str]:
+def generate_structure(
+        start_dir,
+        gens=None,
+        number=10
+) -> List[str]:
+
+    if gens is None:
+        gens = [ResourceGenerator(DEFAULT_STRUCTURE_DIR)]
+
     """
     Generate test data layouts using a list of Generators for
     * Kitodo2 metadata        (<id>/images/<title>_media/*.tif)
     * Kitodo2 export          (<title>/jpeg/*.jpg)
     * Archivierung            (<title>/content/ ,
                                <title>/metadata/images/<title>_media/*.tif)
     * Migration OAI Workspace (MAX/*.jpg)
@@ -177,140 +200,237 @@
                 generated.append(resource_path)
         else:
             generated.append(gen.get())
 
     return generated
 
 
-def run_profiled(func):
+_T = TypeVar('_T')
+_FuncWrapperResult = Tuple[float, str, _T]
+RunProfiledResult = Callable[[], _FuncWrapperResult[_T]]
+
+
+def run_profiled(func: Callable) -> RunProfiledResult:
     """
     Decorator to profile method execution time
     in seconds as float with 2 decimal digits
     """
 
-    def _get_func_name(func):
-        _label = str(func)
-        match = re.match(r'.*function ([\w\.]+) *', _label)
+    def _get_func_name(_func: Callable) -> str:
+        _label = str(_func)
+        match = re.match(r'.*function ([\w.]+) *', _label)
         if match:
             return match.group(1)
         else:
             # this recognizes even MagicMock-Objects
             match = re.match(r".*name='([a-z_]+)'.*", _label)
             if match:
                 return match.group(1)
         return 'func'
 
-    def func_wrapper(*args):
+    def func_wrapper(*args) -> _FuncWrapperResult[_T]:
         result = None
-        start = time.time()
+        start: float = time.perf_counter()
         if args:
             result = func(*args)
         else:
             result = func()
-        delta = time.time() - start
+        delta: float = time.perf_counter() - start
 
         # name of callee
-        label = _get_func_name(func)
-
-        return (round(delta, 2), label, result)
+        label: str = _get_func_name(func)
+        return round(delta, 2), label, result
 
     return func_wrapper
 
 
 @run_profiled
 def run_command(cmd, timeout) -> subprocess.CompletedProcess:
     """Forward command with given timeout
     """
     return subprocess.run(
-        cmd, shell=True, check=True,
+        cmd,
+        shell=True,
+        check=True,
         capture_output=True,
         encoding='UTF-8',
-        timeout=timeout)
+        timeout=timeout
+    )
+
 
+@dataclass(frozen=True)
+class DerivansResult:
+    command: str
+    duration: float
+    result: str | ContainerProcResult | None
+    label: str = None
 
-class DerivansManager:
-    """Manage Derivans (build, recreate, start, error)
-       needs: Java, Maven, GIT
+
+@dataclass(frozen=True)
+class ContainerProcResult:
+    exit_code: int
+    logs: str
+
+
+class BaseDerivansManager(ABC):
+    """Manage Derivans component calls
+    from within python modules
     """
 
-    def __init__(self,
-                 path_mets_file,
-                 path_binary,
-                 path_configuration=None,
-                 path_mvn_project=None):
-        if path_binary is None or\
-                not(Path(path_binary).is_dir() or Path(path_binary).is_file()):
-            raise RuntimeError(
-                "[DerivansManager] provide path_binary "
-                "pointing to file(jar) or a folder containing jar "
-                "not ({})".format(path_binary))
-        if path_mvn_project is not None\
-                and not Path(str(path_mvn_project)).is_dir():
-            raise RuntimeError(
-                "[DerivansManager] path_mvn_project ({}) "
-                "is invalid".format(path_mvn_project))
+    @staticmethod
+    def create(
+            path_mets_file: str,
+            container_image_name: str = None,
+            path_binary: str = None,
+            path_mvn_project: str = None,
+            path_configuration: str = None,
+    ) -> BaseDerivansManager:
+        """Create actual DerivansManager instance
+        depending on provided parameters"""
+
+        if container_image_name is not None:
+            return ContainerDerivansManager(
+                path_mets_file=path_mets_file,
+                container_image=container_image_name,
+                path_configuration=path_configuration,
+            )
+        return DerivansManager(
+            path_mets_file=path_mets_file,
+            path_binary=path_binary,
+            path_mvn_project=path_mvn_project,
+            path_configuration=path_configuration,
+        )
+
+    def __init__(
+            self,
+            path_mets_file,
+            path_configuration=None,
+    ):
         if path_configuration and not Path(str(path_configuration)).is_file():
-            raise RuntimeError(
-                "[DerivansManager] Configuration file not found: {}"
-                .format(path_configuration))
-
+            raise RuntimeError(f"[DerivansManager] config missing: {path_configuration}!")
         self.path_mets_file = path_mets_file
-        self.path_binary = path_binary
         self.path_configuration = path_configuration
-        self.path_mvn_project = path_mvn_project
-        self.path_exec = None
-        self._timeout = DEFAULT_DERIVANS_TIMEOUT
-        self._label = DERIVANS_LABEL
-        self.xargs = ''
+
+    @abstractmethod
+    def init(self) -> None:
+        """Setup application"""
+
+    @abstractmethod
+    def start(self) -> DerivansResult:
+        """Issue actual derivans instance
+        and communicate outcome"""
+
+
+class DerivansManager(BaseDerivansManager):
+    """Local Derivans instance.
+    Requires at least recent Java at
+    runtime, additionally Maven if
+    Derivans must be built at init stage"""
 
     @property
     def timeout(self):
+        """Timeout for derivans workflows"""
         return self._timeout
 
     @timeout.setter
     def timeout(self, timeout):
         self._timeout = timeout
 
     @property
     def label(self):
         return self._label
 
     @label.setter
     def label(self, label):
         self._label = label
 
-    def init(self):
-        """Setup Application"""
+    def __init__(
+            self,
+            path_mets_file: str,
+            path_binary: str,
+            path_mvn_project: str = None,
+            path_configuration: str = None,
+    ):
+        if path_binary is None or \
+                not (Path(path_binary).is_dir() or Path(path_binary).is_file()):
+            raise RuntimeError(f"[DerivansManager] invalid path_binary: {path_binary}!")
+        if path_mvn_project is not None \
+                and not Path(str(path_mvn_project)).is_dir():
+            raise RuntimeError(f"[DerivansManager] invalid path_mvn_project: {path_mvn_project}!")
+        super().__init__(
+            path_mets_file=path_mets_file,
+            path_configuration=path_configuration,
+        )
+        self.path_binary = path_binary
+        self.path_mvn_project = path_mvn_project
+        self._timeout = DEFAULT_DERIVANS_TIMEOUT
+        self._label = DERIVANS_LABEL
+        self.path_exec = None
+        self.xargs = ''
 
+    def init(self):
         _path_derivans = self.path_binary
 
         if Path(self.path_binary).is_dir():
             self.path_binary = self._identify_derivans_bin()
 
         if self.path_binary is None:
             self._recreate_app(_path_derivans)
 
         # fallback to default 'java' if no need to worry about
         if not self.path_exec:
             self.path_exec = 'java'
 
+    def start(self) -> DerivansResult:
+        """Create Derivates with provided configuration
+
+        * step into derivans root dir first
+        * respect actual operation system due executable path
+          wich might contain spaces on windows
+        * execute
+        * return to previous directory
+
+        """
+        derivans_root = os.path.dirname(self.path_binary)
+        prev_dir = os.path.abspath(os.curdir)
+        os.chdir(derivans_root)
+        path_exec = self.path_exec
+        if platform.system() not in ['Linux']:
+            path_exec = f'"{path_exec}"'
+        if self.xargs and not self.xargs.startswith(' '):
+            self.xargs = ' ' + self.xargs
+        cmd = f'{path_exec}{self.xargs} -jar {self.path_binary} {self.path_mets_file}'
+        if self.path_configuration:
+            cmd += f' -c {self.path_configuration}'
+        # disable pylint due it is not able to recognize
+        # output being created by decorator
+        time_duration, label, result = self._execute_derivans(cmd)  # pylint: disable=unpacking-non-sequence
+        os.chdir(prev_dir)
+        return DerivansResult(
+            command=cmd,
+            result=result,
+            duration=time_duration,
+            label=label,
+        )
+
     def _identify_derivans_bin(self, the_dir=None):
         if not the_dir:
             the_dir = self.path_binary
         all_files = [f for f in os.listdir(the_dir) if f.endswith('.jar')]
         derivantis = sorted([f for f in all_files if self._label in str(f)])
         if len(derivantis) > 0:
             return os.path.join(the_dir, derivantis[0])
+        return None
 
     def _recreate_app(self, target_dir):
         dir_derivans = self.path_mvn_project
         if not dir_derivans:
             raise RuntimeError("Derivans project dir unset!")
         if not os.path.isdir(dir_derivans):
-            raise RuntimeError("Invalid derivans project dir '{}'!".format(dir_derivans))
+            raise RuntimeError(f"Invalid derivans project dir: '{dir_derivans}'!")
 
         derivans_build_dir = os.path.join(dir_derivans, 'target')
         the_derivans = None
         if os.path.exists(derivans_build_dir):
             the_derivans = self._identify_derivans_bin(derivans_build_dir)
 
         # if derivans app not build yet, then ...
@@ -328,39 +448,81 @@
         # copy new built jar to target directory
         if not os.path.exists(target_dir):
             os.mkdir(target_dir)
         shutil.copy(the_derivans, target_dir)
         self.path_binary = os.path.join(
             target_dir, os.path.basename(the_derivans))
 
-    def start(self):
-        """Create Derivates with provided configuration
-
-        * step into derivans root dir first
-        * respect actual operation system due executable path
-          wich might contain spaces on windows
-        * execute
-        * return to previous directory
-        
-        """
+    def _execute_derivans(self, command) -> _FuncWrapperResult:
+        return run_command(command, self.timeout)
 
-        derivans_root = os.path.dirname(self.path_binary)
-        prev_dir = os.path.abspath(os.curdir)
-        os.chdir(derivans_root)
-        path_exec = self.path_exec
-        if platform.system() not in ['Linux']:
-            path_exec = '"{}"'.format(path_exec)
-        if self.xargs and not self.xargs.startswith(' '):
-            self.xargs = ' ' + self.xargs
-        cmd = '{}{} -jar {} {}'.format(path_exec,
-            self.xargs, self.path_binary, self.path_mets_file)
-        if self.path_configuration:
-            cmd += ' -c {}'.format(self.path_configuration)
-        # disable pylint due it is not able to recognize
-        # output being created by decorator
-        time_duration, label, result = self._execute_derivans(cmd)   # pylint: disable=unpacking-non-sequence
-        os.chdir(prev_dir)
-        return (cmd, label, time_duration, result)
 
+class ContainerDerivansManager(BaseDerivansManager):
+    """Containered Derivans instance.
+    Required local container runtime.
+    """
 
-    def _execute_derivans(self, command) -> subprocess.CompletedProcess:
-        return run_command(command, self.timeout)
+    def __init__(
+            self,
+            path_mets_file: str,
+            container_image: str = DEFAULT_DERIVANS_IMAGE,
+            path_configuration: str = None,
+    ):
+        super().__init__(
+            path_mets_file=path_mets_file,
+            path_configuration=path_configuration
+        )
+        self._container_image: str = container_image
+        self._client: DockerClient = from_env()
+
+    def init(self) -> None:
+        repo, tag = self._container_image.split(':')
+        self._client.images.pull(repo, tag)
+
+    def start(self) -> DerivansResult:
+        mounts: List[Mount] = []
+        command: List[str] = []
+        mets_path: Path = Path(self.path_mets_file).absolute()
+        if mets_path.is_dir():
+            command.append(DERIVANS_CNT_DATA_DIR)
+            mounts.append(Mount(source=str(mets_path), target=DERIVANS_CNT_DATA_DIR, type='bind'))
+        if mets_path.is_file():
+            mets_file_name: str = mets_path.name
+            mets_dir: str = str(mets_path.parent.absolute())
+            target_mets_file: str = str(Path(DERIVANS_CNT_DATA_DIR).joinpath(mets_file_name))
+            command.append(target_mets_file)
+            mounts.append(Mount(source=mets_dir, target=DERIVANS_CNT_DATA_DIR, type='bind'))
+        if self.path_configuration is not None:
+            config_path: Union[Path, None] = Path(self.path_configuration)
+            if config_path.exists() and config_path.is_file():
+                config_file_name: str = config_path.name
+                config_dir: str = str(config_path.parent.absolute())
+                target_config_file: str = str(Path(DERIVANS_CNT_CONF_DIR).joinpath(config_file_name))
+                mounts.append(Mount(source=config_dir, target=DERIVANS_CNT_CONF_DIR, type='bind'))
+                command.append('-c')
+                command.append(target_config_file)
+
+        start_time: float = time.perf_counter()
+        container: Container = self._client.containers.run(
+            image=self._container_image,
+            command=command,
+            user=os.getuid(),
+            mounts=mounts,
+            detach=True
+        )
+        exit_code: int = container.wait()['StatusCode']
+        logs: str = container.logs().decode('utf-8')
+        container.remove()
+
+        full_command_equivalent: List[str] = ['docker run -rm']
+        for mount in mounts:
+            full_command_equivalent.append(
+                f"--mount type={mount['Type']},source={mount['Source']},target={mount['Target']}"
+            )
+        full_command_equivalent.append(self._container_image)
+        full_command_equivalent.append(" ".join(command))
+        dur: float = time.perf_counter() - start_time
+        return DerivansResult(
+            command=" ".join(full_command_equivalent),
+            result=ContainerProcResult(exit_code=exit_code, logs=logs),
+            duration=dur,
+        )
```

### Comparing `digiflow-3.0.1/src/digiflow/digiflow_io.py` & `digiflow-3.1.0/src/digiflow/digiflow_io.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/src/digiflow/digiflow_metadata.py` & `digiflow-3.1.0/src/digiflow/digiflow_metadata.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/src/digiflow/digiflow_validate.py` & `digiflow-3.1.0/src/digiflow/digiflow_validate.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/src/digiflow/resources/digilife.ini` & `digiflow-3.1.0/src/digiflow/resources/digilife.ini`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/src/digiflow/resources/sch/ddb_validierung_mets-mods-ap-digitalisierte-medien.sch` & `digiflow-3.1.0/src/digiflow/resources/sch/ddb_validierung_mets-mods-ap-digitalisierte-medien.sch`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/src/digiflow/resources/sch/ddb_validierung_mets-mods-ap-digitalisierte-zeitungen.sch` & `digiflow-3.1.0/src/digiflow/resources/sch/ddb_validierung_mets-mods-ap-digitalisierte-zeitungen.sch`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/src/digiflow/resources/xsd/alto_4-2.xsd` & `digiflow-3.1.0/src/digiflow/resources/xsd/alto_4-2.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/src/digiflow/resources/xsd/mets_1-12.xsd` & `digiflow-3.1.0/src/digiflow/resources/xsd/mets_1-12.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/src/digiflow/resources/xsd/mix_2-0.xsd` & `digiflow-3.1.0/src/digiflow/resources/xsd/mix_2-0.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/src/digiflow/resources/xsd/mods_3-7.xsd` & `digiflow-3.1.0/src/digiflow/resources/xsd/mods_3-7.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/src/digiflow/resources/xsd/page_2019-07-15.xsd` & `digiflow-3.1.0/src/digiflow/resources/xsd/page_2019-07-15.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/src/digiflow/resources/xsd/xlink.xsd` & `digiflow-3.1.0/src/digiflow/resources/xsd/xlink.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/src/digiflow/resources/xsd/xml.xsd` & `digiflow-3.1.0/src/digiflow/resources/xsd/xml.xsd`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/src/digiflow/schematron/schxslt-cli.jar` & `digiflow-3.1.0/src/digiflow/schematron/schxslt-cli.jar`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/src/digiflow.egg-info/PKG-INFO` & `digiflow-3.1.0/src/digiflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digiflow
-Version: 3.0.1
+Version: 3.1.0
 Summary: Father's Little Digitization Workflow Helper
 Author-email: Universitäts- und Landesbibliothek Sachsen-Anhalt <development@bibliothek.uni-halle.de>
 Project-URL: Homepage, https://github.com/ulb-sachsen-anhalt/digital-flow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `digiflow-3.0.1/src/digiflow.egg-info/SOURCES.txt` & `digiflow-3.1.0/src/digiflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/tests/test_digiflow_generate.py` & `digiflow-3.1.0/tests/test_digiflow_generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # -*- coding: utf-8 -*-
 
 import os
 import subprocess
 import time
 
 from unittest import (
-    mock
+    mock,
 )
 
 import pytest
 
 from digiflow import (
     Blueprint,
     ResourceGenerator,
     DerivansManager,
     generate_structure,
     run_profiled,
-    id_generator
+    id_generator,
+    ContainerDerivansManager,
+    DEFAULT_DERIVANS_IMAGE,
 )
 
 
+DUMMY_METS = '<xml/>'
+
+
 def test_generate_migration_start_structure_layout(tmp_path):
     """Create default structure using DEFAULT_STRUCTURE_DIR"""
 
     # act
     created = generate_structure(tmp_path)
 
     # assert
@@ -67,15 +72,14 @@
     for res in created:
         assert os.path.isfile(os.path.join(tmp_path, res))
     assert os.path.isfile(
         os.path.join(str(tmp_path), '1003841856', 'zkw_open'))
 
 
 def test_generate_invalid_startdir():
-
     with pytest.raises(RuntimeError) as exc:
         generate_structure('foo/bar')
 
     assert 'Invalid start_dir \'foo/bar\' provided' in str(exc.value)
 
 
 def test_generator_with_prefix_and_suffix():
@@ -164,102 +168,122 @@
 def test_utils_profile_args_return():
     assert my_func_args(3, 5) == (0.25, 'my_func_args', 8)
 
 
 def test_utils_profile_class_context():
     my_stuff = MyClass()
     assert my_stuff.my_func_args(3, 5) == (0.25, 'MyClass.my_func_args', 17)
-    assert\
+    assert \
         MyClass.my_func_static(3, 5) == (0.25, 'MyClass.my_func_static', 15)
 
 
-def test_derivans_manager_with_path_bin_jar(tmp_path):
+@mock.patch('docker.models.images.ImageCollection.pull')
+def test_derivans_manager_with_container(mock_coll, tmp_path):
+    """Check init phase of containerized
+    Derivans execution context tries to
+    pull required default container image"""
+
+    # arrange
     test_project_root = tmp_path / 'migrationtest'
     test_project_root.mkdir()
-    test_project_bin = test_project_root / 'bin'
-    test_project_bin.mkdir()
-    jar_name = 'digital-derivans-1.2.3.jar'
-    jar_file = os.path.join(str(test_project_bin), jar_name)
-    with open(jar_file, 'wb') as fh:
-        fh.write(b'foofoo')
     mets_file = os.path.join(str(test_project_root), 'mets_mods.xml')
-    with open(mets_file, 'w') as fh:
-        fh.write('<xml/>')
-    dmanager = DerivansManager(
-        mets_file, path_binary=jar_file,
-        path_mvn_project=None)
+    with open(mets_file, 'w', encoding='utf-8') as fh_mets:
+        fh_mets.write(DUMMY_METS)
+    dmanager = ContainerDerivansManager(
+        mets_file,
+    )
+
+    # act
     dmanager.init()
 
+    # assert
+    assert mock_coll.call_count == 1
+    _call_args = mock_coll.call_args.args
+    assert len(_call_args) == 2
+    _image_label = DEFAULT_DERIVANS_IMAGE.split(':', maxsplit=1)[0]
+    assert _call_args[0] == f'{_image_label}'
+    assert _call_args[1] == 'latest'
+
 
 def test_derivans_manager_with_path_bin_dir(tmp_path):
     """
     Raise Exception because no valid Maven project
     Directory exists but required to build Derivans
     """
 
+    # arrange
     test_project_root = tmp_path / 'migrationtest'
     the_derivans = test_project_root / 'digital-derivans' / 'target'
     test_project_root.mkdir()
     os.makedirs(str(the_derivans), exist_ok=True)
     test_project_bin = test_project_root / 'bin'
     test_project_bin.mkdir()
     mets_file = os.path.join(str(test_project_root), 'mets_mods.xml')
-    with open(mets_file, 'w') as fh:
-        fh.write('<xml/>')
+    with open(mets_file, 'w', encoding='utf-8') as fh_mets:
+        fh_mets.write(DUMMY_METS)
 
     path_mvn_project = str(test_project_root / 'digital-derivans')
     dmanager = DerivansManager(
         mets_file, path_binary=str(test_project_bin),
         path_mvn_project=path_mvn_project)
-    cwd = os.getcwd()    
+    cwd = os.getcwd()
+
+    # act
     with pytest.raises(subprocess.CalledProcessError) as err:
         dmanager.init()
     os.chdir(cwd)  # subprocess is changing the cwd, so lets go back
+
+    # assert
     assert ("Command 'mvn clean package -DskipTests' "
             "returned non-zero exit status") in str(err.value)
 
 
 def test_derivans_manager_none_path_binary(tmp_path):
-    """Exception must be thrown if METS provided but invalid"""
+    """Exception must be thrown if invalid
+    None-path to local binary provided"""
 
+    # arrange
     test_project_root = tmp_path / 'migrationtest'
     test_project_root.mkdir()
     mets_file = os.path.join(str(test_project_root), 'mets_mods.xml')
-    with open(mets_file, 'w') as fh:
-        fh.write('<xml/>')
+    with open(mets_file, 'w', encoding='utf-8') as fh_mets:
+        fh_mets.write(DUMMY_METS)
+
+    # act
     with pytest.raises(RuntimeError) as exc:
         DerivansManager(mets_file, path_binary=None)
-    assert 'provide path_binary' in str(exc.value)
+
+    # assert
+    assert 'invalid path_binary' in str(exc.value)
 
 
 def _forward_derivans_call(*args):
     """take some rest and return alike
     the *real* call would do"""
 
     _delay = args[0]
     time.sleep(_delay)
     yield (_delay, 'execute', 'result')
 
 
 @mock.patch('digiflow.DerivansManager._execute_derivans')
 @mock.patch('digiflow.DerivansManager._identify_derivans_bin')
 def test_derivans_start_set_exec(mock_check, mock_call, tmp_path):
-
     # arrange
     test_project_root = tmp_path / 'migrationtest'
     the_derivans = test_project_root / 'digital-derivans' / 'target'
     test_project_root.mkdir()
     os.makedirs(str(the_derivans), exist_ok=True)
     test_project_bin = test_project_root / 'bin'
     test_project_bin.mkdir()
 
     # create some dummy file
     mets_file = os.path.join(str(test_project_root), 'mets_mods.xml')
-    with open(mets_file, 'w') as fh:
-        fh.write('<xml/>')
+    with open(mets_file, 'w', encoding='utf-8') as fh_mets:
+        fh_mets.write(DUMMY_METS)
     path_mvn_project = str(test_project_root / 'digital-derivans')
     dmanager = DerivansManager(
         mets_file, path_binary=str(test_project_bin),
         path_mvn_project=path_mvn_project)
     # here is the important detail
     dmanager.path_exec = '/usr/lib/jvm/java-11-openjdk-amd64/bin/java'
     mock_check.return_value = str(test_project_bin)
@@ -267,47 +291,46 @@
 
     # act
     dmanager.init()
     result = dmanager.start()
 
     # assert
     assert mock_call.call_count == 1
-    assert result[0].startswith('/usr/lib/jvm/java-11-openjdk-amd64/bin/java -jar')
+    assert result.command.startswith('/usr/lib/jvm/java-11-openjdk-amd64/bin/java -jar')
 
 
 @mock.patch('digiflow.DerivansManager._execute_derivans')
 @mock.patch('digiflow.DerivansManager._identify_derivans_bin')
 def test_derivans_start_default(mock_check, mock_call, tmp_path):
-
     # arrange
     test_project_root = tmp_path / 'migrationtest'
     the_derivans = test_project_root / 'digital-derivans' / 'target'
     test_project_root.mkdir()
     os.makedirs(str(the_derivans), exist_ok=True)
     test_project_bin = test_project_root / 'bin'
     test_project_bin.mkdir()
 
     # create some dummy file
     mets_file = os.path.join(str(test_project_root), 'mets_mods.xml')
-    with open(mets_file, 'w') as fh:
-        fh.write('<xml/>')
+    with open(mets_file, 'w', encoding='utf-8') as fh_mets:
+        fh_mets.write(DUMMY_METS)
     path_mvn_project = str(test_project_root / 'digital-derivans')
     dmanager = DerivansManager(
         mets_file, path_binary=str(test_project_bin),
         path_mvn_project=path_mvn_project)
     mock_check.return_value = str(test_project_bin)
     mock_call.side_effect = _forward_derivans_call(0.1)
 
     # act
     dmanager.init()
     result = dmanager.start()
 
     # assert
     assert mock_call.call_count == 1
-    assert result[0].startswith('java -jar')
+    assert result.command.startswith('java -jar')
 
 
 @mock.patch('digiflow.DerivansManager._execute_derivans')
 @mock.patch('digiflow.DerivansManager._identify_derivans_bin')
 def test_derivans_start_with_additional_config(mock_check, mock_call, tmp_path):
     """Prevent Regression and catch bug: 
         [undefined]TypeError: bad operand type for unary +: 'str'
@@ -319,32 +342,32 @@
     test_project_root.mkdir()
     os.makedirs(str(the_derivans), exist_ok=True)
     test_project_bin = test_project_root / 'bin'
     test_project_bin.mkdir()
 
     # create some dummy file
     mets_file = os.path.join(str(test_project_root), 'mets_mods.xml')
-    with open(mets_file, 'w') as fh:
-        fh.write('<xml/>')
+    with open(mets_file, 'w', encoding='utf-8') as fh_mets:
+        fh_mets.write(DUMMY_METS)
     path_mvn_project = str(test_project_root / 'digital-derivans')
     dmanager = DerivansManager(
         mets_file, path_binary=str(test_project_bin),
         path_mvn_project=path_mvn_project)
     mock_check.return_value = str(test_project_bin)
     dmanager.path_configuration = '/path/to/derivans.ini'
     mock_call.side_effect = _forward_derivans_call(0.1)
 
     # act
     dmanager.init()
     result = dmanager.start()
 
     # assert
     assert mock_call.call_count == 1
-    assert result[0].startswith('java -jar')
-    assert result[0].endswith('/path/to/derivans.ini')
+    assert result.command.startswith('java -jar')
+    assert result.command.endswith('/path/to/derivans.ini')
 
 
 @mock.patch('digiflow.DerivansManager._execute_derivans')
 @mock.patch('digiflow.DerivansManager._identify_derivans_bin')
 def test_derivans_start_with_java_xargs(mock_check, mock_call, tmp_path):
     """Prevent Regression and catch bug: 
         X11 connection rejected because of wrong authentication.
@@ -369,16 +392,16 @@
     test_project_root.mkdir()
     os.makedirs(str(the_derivans), exist_ok=True)
     test_project_bin = test_project_root / 'bin'
     test_project_bin.mkdir()
 
     # create some dummy file
     mets_file = os.path.join(str(test_project_root), 'mets_mods.xml')
-    with open(mets_file, 'w') as fh:
-        fh.write('<xml/>')
+    with open(mets_file, 'w', encoding='utf-8') as fh_mets:
+        fh_mets.write(DUMMY_METS)
     path_mvn_project = str(test_project_root / 'digital-derivans')
     dmanager = DerivansManager(
         mets_file, path_binary=str(test_project_bin),
         path_mvn_project=path_mvn_project)
     mock_check.return_value = str(test_project_bin)
     dmanager.path_configuration = '/path/to/derivans.ini'
     dmanager.xargs = '-Djava.awt.headless=true'
@@ -386,8 +409,8 @@
 
     # act
     dmanager.init()
     result = dmanager.start()
 
     # assert
     assert mock_call.call_count == 1
-    assert ' -Djava.awt.headless=true ' in result[0]
+    assert ' -Djava.awt.headless=true ' in result.command
```

### Comparing `digiflow-3.0.1/tests/test_digiflow_identifier.py` & `digiflow-3.1.0/tests/test_digiflow_identifier.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/tests/test_digiflow_io.py` & `digiflow-3.1.0/tests/test_digiflow_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -637,33 +637,32 @@
     oais.sweep()
 
     for item in Path(migration_sweeper_pdf_fixture).iterdir():
         if str(item.name) == 'DOWNLOAD':
             assert len(list(item.iterdir())) == 0
 
 
-def mock_get_smtp_server():
-    smtpmock = mock.Mock()
-    return smtpmock
-
-
-def test_send_mail(mocker):
+@mock.patch('digiflow.digiflow_io.get_smtp_server')
+def test_send_mail(mock_smtp):
     """test sending mail"""
 
-    mocker.patch(
-        'digiflow.digiflow_io.get_smtp_server', mock_get_smtp_server)
+    # arrange
     random_message = uuid.uuid4().hex
 
+    # act
     mess = send_mail(
         subject='test',
         message=random_message,
         sender='test@example.com',
         recipients='me@example.de')
+
+    # assert
     assert random_message in mess
     assert 'notification' in mess
+    assert mock_smtp.called
 
 
 def test_record_state_list_set_state_from(oai_record_list):
     """Behavior for changing state matching state and start time"""
 
     # arrange
     handler = OAIRecordHandler(
```

### Comparing `digiflow-3.0.1/tests/test_digiflow_metadata.py` & `digiflow-3.1.0/tests/test_digiflow_metadata.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/tests/test_digiflow_validate.py` & `digiflow-3.1.0/tests/test_digiflow_validate.py`

 * *Files identical despite different names*

### Comparing `digiflow-3.0.1/tests/test_export_saf.py` & `digiflow-3.1.0/tests/test_export_saf.py`

 * *Files identical despite different names*

