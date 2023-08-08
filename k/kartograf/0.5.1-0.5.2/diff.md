# Comparing `tmp/kartograf-0.5.1.tar.gz` & `tmp/kartograf-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kartograf-0.5.1.tar", last modified: Wed Jun  7 21:06:30 2023, max compression
+gzip compressed data, was "kartograf-0.5.2.tar", last modified: Tue Aug  8 10:09:49 2023, max compression
```

## Comparing `kartograf-0.5.1.tar` & `kartograf-0.5.2.tar`

### file list

```diff
@@ -1,45 +1,42 @@
-drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.781697 kartograf-0.5.1/
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     1073 2023-02-02 13:06:04.000000 kartograf-0.5.1/LICENSE
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     3268 2023-06-07 21:06:30.780690 kartograf-0.5.1/PKG-INFO
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     2576 2023-06-05 14:08:55.000000 kartograf-0.5.1/README.md
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     1316 2023-06-05 14:08:55.000000 kartograf-0.5.1/pyproject.toml
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)       38 2023-06-07 21:06:30.782673 kartograf-0.5.1/setup.cfg
-drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.560423 kartograf-0.5.1/src/
-drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.619744 kartograf-0.5.1/src/kartograf/
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)      257 2023-06-07 19:45:21.000000 kartograf-0.5.1/src/kartograf/__init__.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     3650 2023-04-28 14:06:23.000000 kartograf-0.5.1/src/kartograf/_old_dev.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)       22 2023-06-07 21:06:30.000000 kartograf-0.5.1/src/kartograf/_version.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     2255 2023-04-28 14:59:10.000000 kartograf-0.5.1/src/kartograf/atom_align.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)    27089 2023-06-07 19:51:48.000000 kartograf-0.5.1/src/kartograf/atom_mapper.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)    17110 2023-06-07 20:38:42.000000 kartograf-0.5.1/src/kartograf/atom_mapping_scoring.py
-drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.673667 kartograf-0.5.1/src/kartograf/dev/
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-04-28 13:51:44.000000 kartograf-0.5.1/src/kartograf/dev/__init__.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)      667 2023-05-08 08:50:41.000000 kartograf-0.5.1/src/kartograf/dev/stylez.py
-drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.696674 kartograf-0.5.1/src/kartograf/dev/visualisation/
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-04-28 07:56:19.000000 kartograf-0.5.1/src/kartograf/dev/visualisation/__init__.py
-drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.719703 kartograf-0.5.1/src/kartograf/dev/visualisation/approachPics/
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-04-28 08:08:32.000000 kartograf-0.5.1/src/kartograf/dev/visualisation/approachPics/__init__.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     6339 2023-06-07 08:04:40.000000 kartograf-0.5.1/src/kartograf/dev/visualisation/approachPics/vis_approach.py
-drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.737695 kartograf-0.5.1/src/kartograf/dev/visualisation/benzenePics/
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-04-28 08:08:10.000000 kartograf-0.5.1/src/kartograf/dev/visualisation/benzenePics/__init__.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     9309 2023-05-03 08:01:11.000000 kartograf-0.5.1/src/kartograf/dev/visualisation/benzenePics/vis_metrics.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)      571 2023-04-28 08:01:29.000000 kartograf-0.5.1/src/kartograf/dev/visualisation/pymol_utils.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     1824 2023-06-07 08:25:12.000000 kartograf-0.5.1/src/kartograf/dev/visualisation/single.py
-drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.760656 kartograf-0.5.1/src/kartograf/filters/
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)      212 2023-06-07 19:45:21.000000 kartograf-0.5.1/src/kartograf/filters/__init__.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     1435 2023-06-07 19:45:21.000000 kartograf-0.5.1/src/kartograf/filters/element_change.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     2723 2023-06-07 19:45:21.000000 kartograf-0.5.1/src/kartograf/filters/ring_changes.py
-drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.776698 kartograf-0.5.1/src/kartograf/tests/
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-04-13 13:43:13.000000 kartograf-0.5.1/src/kartograf/tests/__init__.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     2574 2023-06-07 20:00:46.000000 kartograf-0.5.1/src/kartograf/tests/conf.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)      630 2023-04-28 15:03:26.000000 kartograf-0.5.1/src/kartograf/tests/test_atom_align.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     5193 2023-06-07 19:45:21.000000 kartograf-0.5.1/src/kartograf/tests/test_atom_mapper.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     3008 2023-06-07 19:45:21.000000 kartograf-0.5.1/src/kartograf/tests/test_atom_mapping_scorer.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     1232 2023-06-07 19:45:21.000000 kartograf-0.5.1/src/kartograf/tests/test_element_filters.py
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     2137 2023-06-07 19:45:21.000000 kartograf-0.5.1/src/kartograf/tests/test_ring_filters.py
-drwxr-sr-x   0 riesbenj (32407) BI-LINUX  (2600)        0 2023-06-07 21:06:30.667712 kartograf-0.5.1/src/kartograf.egg-info/
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     3268 2023-06-07 21:06:30.000000 kartograf-0.5.1/src/kartograf.egg-info/PKG-INFO
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)     1197 2023-06-07 21:06:30.000000 kartograf-0.5.1/src/kartograf.egg-info/SOURCES.txt
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)        1 2023-06-07 21:06:30.000000 kartograf-0.5.1/src/kartograf.egg-info/dependency_links.txt
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)       23 2023-06-07 21:06:30.000000 kartograf-0.5.1/src/kartograf.egg-info/requires.txt
--rw-r--r--   0 riesbenj (32407) BI-LINUX  (2600)       10 2023-06-07 21:06:30.000000 kartograf-0.5.1/src/kartograf.egg-info/top_level.txt
+drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-08-08 10:09:48.993731 kartograf-0.5.2/
+-rw-r--r--   0 bries     (1000) bries     (1000)     1073 2023-02-03 06:44:21.000000 kartograf-0.5.2/LICENSE
+-rw-r--r--   0 bries     (1000) bries     (1000)     3494 2023-08-08 10:09:48.993731 kartograf-0.5.2/PKG-INFO
+-rw-r--r--   0 bries     (1000) bries     (1000)     2886 2023-08-08 09:36:14.000000 kartograf-0.5.2/README.md
+-rw-r--r--   0 bries     (1000) bries     (1000)     1438 2023-08-08 09:36:14.000000 kartograf-0.5.2/pyproject.toml
+-rw-r--r--   0 bries     (1000) bries     (1000)       38 2023-08-08 10:09:48.993731 kartograf-0.5.2/setup.cfg
+drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-08-08 10:09:48.982898 kartograf-0.5.2/src/
+drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-08-08 10:09:48.982898 kartograf-0.5.2/src/kartograf/
+-rw-r--r--   0 bries     (1000) bries     (1000)      262 2023-06-26 20:50:03.000000 kartograf-0.5.2/src/kartograf/__init__.py
+-rw-r--r--   0 bries     (1000) bries     (1000)       22 2023-08-08 10:09:48.000000 kartograf-0.5.2/src/kartograf/_version.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     2348 2023-05-05 16:51:56.000000 kartograf-0.5.2/src/kartograf/atom_align.py
+-rw-r--r--   0 bries     (1000) bries     (1000)    28054 2023-08-08 09:36:14.000000 kartograf-0.5.2/src/kartograf/atom_mapper.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     1853 2023-08-08 09:36:14.000000 kartograf-0.5.2/src/kartograf/atom_mapping_scorer.py
+drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-08-08 10:09:48.982898 kartograf-0.5.2/src/kartograf/filters/
+-rw-r--r--   0 bries     (1000) bries     (1000)      221 2023-06-26 20:50:03.000000 kartograf-0.5.2/src/kartograf/filters/__init__.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     1475 2023-06-26 20:50:03.000000 kartograf-0.5.2/src/kartograf/filters/element_change.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     2803 2023-06-26 20:50:03.000000 kartograf-0.5.2/src/kartograf/filters/ring_changes.py
+drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-08-08 10:09:48.993731 kartograf-0.5.2/src/kartograf/mapping_metrics/
+-rw-r--r--   0 bries     (1000) bries     (1000)      368 2023-06-26 20:50:03.000000 kartograf-0.5.2/src/kartograf/mapping_metrics/__init__.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     1175 2023-06-26 20:50:03.000000 kartograf-0.5.2/src/kartograf/mapping_metrics/_abstract_scorer.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     2920 2023-06-26 20:50:03.000000 kartograf-0.5.2/src/kartograf/mapping_metrics/metric_mapping_rmsd.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     9377 2023-06-26 20:50:03.000000 kartograf-0.5.2/src/kartograf/mapping_metrics/metric_shape_difference.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     3626 2023-08-08 09:36:14.000000 kartograf-0.5.2/src/kartograf/mapping_metrics/metric_volume_ratio.py
+drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-08-08 10:09:48.993731 kartograf-0.5.2/src/kartograf/tests/
+-rw-r--r--   0 bries     (1000) bries     (1000)        0 2023-04-06 16:28:36.000000 kartograf-0.5.2/src/kartograf/tests/__init__.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     2574 2023-06-26 20:50:03.000000 kartograf-0.5.2/src/kartograf/tests/conf.py
+-rw-r--r--   0 bries     (1000) bries     (1000)      652 2023-05-05 16:51:56.000000 kartograf-0.5.2/src/kartograf/tests/test_atom_align.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     5357 2023-06-26 20:50:03.000000 kartograf-0.5.2/src/kartograf/tests/test_atom_mapper.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     3553 2023-08-08 09:36:14.000000 kartograf-0.5.2/src/kartograf/tests/test_atom_mapping_scorer.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     1272 2023-06-26 20:50:03.000000 kartograf-0.5.2/src/kartograf/tests/test_element_filters.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     2220 2023-06-26 20:50:03.000000 kartograf-0.5.2/src/kartograf/tests/test_ring_filters.py
+-rw-r--r--   0 bries     (1000) bries     (1000)      781 2023-08-08 09:36:14.000000 kartograf-0.5.2/src/kartograf/tests/test_utils_vis.py
+drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-08-08 10:09:48.993731 kartograf-0.5.2/src/kartograf/utils/
+-rw-r--r--   0 bries     (1000) bries     (1000)        0 2023-08-08 09:36:14.000000 kartograf-0.5.2/src/kartograf/utils/__init__.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     2004 2023-08-08 09:36:14.000000 kartograf-0.5.2/src/kartograf/utils/mapping_visualization_widget.py
+-rw-r--r--   0 bries     (1000) bries     (1000)     1259 2023-08-08 09:36:14.000000 kartograf-0.5.2/src/kartograf/utils/optional_imports.py
+drwxr-xr-x   0 bries     (1000) bries     (1000)        0 2023-08-08 10:09:48.982898 kartograf-0.5.2/src/kartograf.egg-info/
+-rw-r--r--   0 bries     (1000) bries     (1000)     3494 2023-08-08 10:09:48.000000 kartograf-0.5.2/src/kartograf.egg-info/PKG-INFO
+-rw-r--r--   0 bries     (1000) bries     (1000)     1163 2023-08-08 10:09:48.000000 kartograf-0.5.2/src/kartograf.egg-info/SOURCES.txt
+-rw-r--r--   0 bries     (1000) bries     (1000)        1 2023-08-08 10:09:48.000000 kartograf-0.5.2/src/kartograf.egg-info/dependency_links.txt
+-rw-r--r--   0 bries     (1000) bries     (1000)       34 2023-08-08 10:09:48.000000 kartograf-0.5.2/src/kartograf.egg-info/requires.txt
+-rw-r--r--   0 bries     (1000) bries     (1000)       10 2023-08-08 10:09:48.000000 kartograf-0.5.2/src/kartograf.egg-info/top_level.txt
```

### Comparing `kartograf-0.5.1/LICENSE` & `kartograf-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kartograf-0.5.1/PKG-INFO` & `kartograf-0.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kartograf
-Version: 0.5.1
+Version: 0.5.2
 Summary: Kartograf is a package for mapping geometrically atoms of two molecules. (like you need it with hybrid topology)
 Author-email: Benjamin Ries <benjamin-ries@outlook.com>, David Swenson <dwhswenson@gmail.com>, Irfan Alibay <irfan.alibay@gmail.com>, Mike Henry <mike.henry@choderalab.org>, Richard J Gowers <richardjgowers@gmail.com>
 Project-URL: Homepage, https://github.com/OpenFreeEnergy/kartograf
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -75,11 +75,23 @@
 
 ```shell
 conda install -c conda-forge kartograf
 ```
 
 Or use Kartograf from the OpenFE Environment (soon).
 
+For Developing Kartograf, you might want to use this approach:
+
+```shell
+git clone https://github.com/OpenFreeEnergy/kartograf.git
+
+cd kartograf
+conda env create -f environment.yml
+
+conda activate kartograf
+pip install .
+
+```
 ## References
```

### Comparing `kartograf-0.5.1/README.md` & `kartograf-0.5.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,72 +1,84 @@
-
-<p align="center">
-    <img src="docs/_static/img/Kartograf_logo_boxed_dark_transp.png" id="gh-dark-mode-only"  width=35%/>
-    <!-- <img src="img/Kartograf_logo_boxed_light_transp.png" id="gh-light-mode-only"  width=20%/> -->
-</p>
-
-Kartograf: A 3D Atom Graph Mapper
-==================================
-
-[//]: # (Badges)
-[![Logo](https://img.shields.io/badge/OSMF-OpenFreeEnergy-%23002f4a)](https://openfree.energy/)
-[![build](https://github.com/OpenFreeEnergy/kartograf/actions/workflows/ci.yaml/badge.svg)](https://github.com/OpenFreeEnergy/kartograf/actions/workflows/ci.yaml)
-[![coverage](https://codecov.io/gh/OpenFreeEnergy/kartograf/branch/main/graph/badge.svg)](https://codecov.io/gh/OpenFreeEnergy/kartograf)
-[![Documentation Status](https://readthedocs.org/projects/kartograf/badge/?version=latest)](https://kartograf.readthedocs.io/en/latest/?badge=latest)
-
-[![Pip Install](https://img.shields.io/badge/pip%20install-kartograf-d9c4b1)](https://pypi.org/project/kartograf/)
-[![Conda Install](https://img.shields.io/badge/Conda%20install---c%20conda--forge%20kartograf-009384)](https://anaconda.org/conda-forge/kartograf)
-
-
-Kartograf offers a geometric atom mapper approach, that allows to map a given set of ligand coordinates. (can be used for hybrid topology  RBFE calculations)
-This package can be used standalone, or from the OpenFE environment.
-
-**More will be here soon!**
-
-## Usage
-```python3
-from rdkit import Chem
-from kartograf.atom_align import align_mol_shape
-from kartograf import KartografAtomMapper, SmallMoleculeComponent
-
-#Preprocessing from Smiles - Here you can add your Input!
-# Generate Data: START
-smiles = ["c1ccccc1", "c1ccccc1(CO)"]
-rdmols = [Chem.MolFromSmiles(s) for s in smiles]
-rdmols = [Chem.AddHs(m, addCoords=True) for m in rdmols]
-[Chem.rdDistGeom.EmbedMolecule(m, useRandomCoords=False, randomSeed = 0) for m in rdmols]
-# Generate Data: END
-
-# Build Small Molecule Components
-molA, molB = [SmallMoleculeComponent.from_rdkit(m) for m in rdmols]
-
-# Align the mols first - this might not needed, depends on input.
-a_molB = align_mol_shape(molB, ref_mol=molA)
-
-
-# Build Kartograf Atom Mapper
-mapper = KartografAtomMapper(atom_map_hydrogens=True)
-
-# Get Mapping
-kartograf_mapping = next(mapper.suggest_mappings(molA, a_molB))
-
-kartograf_mapping
-```
-![](docs/_static/img/alignment_benz_ol.png)
-
-## Installation
-you can install Kartograf via the package manager of your choice:
-
-```shell
-pip install kartograf
-```
-
-```shell
-conda install -c conda-forge kartograf
-```
-
-Or use Kartograf from the OpenFE Environment (soon).
-
-## References
-
-
-
+
+<p align="center">
+    <img src="docs/_static/img/Kartograf_logo_boxed_dark_transp.png" id="gh-dark-mode-only"  width=35%/>
+    <!-- <img src="img/Kartograf_logo_boxed_light_transp.png" id="gh-light-mode-only"  width=20%/> -->
+</p>
+
+Kartograf: A 3D Atom Graph Mapper
+==================================
+
+[//]: # (Badges)
+[![Logo](https://img.shields.io/badge/OSMF-OpenFreeEnergy-%23002f4a)](https://openfree.energy/)
+[![build](https://github.com/OpenFreeEnergy/kartograf/actions/workflows/ci.yaml/badge.svg)](https://github.com/OpenFreeEnergy/kartograf/actions/workflows/ci.yaml)
+[![coverage](https://codecov.io/gh/OpenFreeEnergy/kartograf/branch/main/graph/badge.svg)](https://codecov.io/gh/OpenFreeEnergy/kartograf)
+[![Documentation Status](https://readthedocs.org/projects/kartograf/badge/?version=latest)](https://kartograf.readthedocs.io/en/latest/?badge=latest)
+
+[![Pip Install](https://img.shields.io/badge/pip%20install-kartograf-d9c4b1)](https://pypi.org/project/kartograf/)
+[![Conda Install](https://img.shields.io/badge/Conda%20install---c%20conda--forge%20kartograf-009384)](https://anaconda.org/conda-forge/kartograf)
+
+
+Kartograf offers a geometric atom mapper approach, that allows to map a given set of ligand coordinates. (can be used for hybrid topology  RBFE calculations)
+This package can be used standalone, or from the OpenFE environment.
+
+**More will be here soon!**
+
+## Usage
+```python3
+from rdkit import Chem
+from kartograf.atom_align import align_mol_shape
+from kartograf import KartografAtomMapper, SmallMoleculeComponent
+
+#Preprocessing from Smiles - Here you can add your Input!
+# Generate Data: START
+smiles = ["c1ccccc1", "c1ccccc1(CO)"]
+rdmols = [Chem.MolFromSmiles(s) for s in smiles]
+rdmols = [Chem.AddHs(m, addCoords=True) for m in rdmols]
+[Chem.rdDistGeom.EmbedMolecule(m, useRandomCoords=False, randomSeed = 0) for m in rdmols]
+# Generate Data: END
+
+# Build Small Molecule Components
+molA, molB = [SmallMoleculeComponent.from_rdkit(m) for m in rdmols]
+
+# Align the mols first - this might not needed, depends on input.
+a_molB = align_mol_shape(molB, ref_mol=molA)
+
+
+# Build Kartograf Atom Mapper
+mapper = KartografAtomMapper(atom_map_hydrogens=True)
+
+# Get Mapping
+kartograf_mapping = next(mapper.suggest_mappings(molA, a_molB))
+
+kartograf_mapping
+```
+![](docs/_static/img/alignment_benz_ol.png)
+
+## Installation
+you can install Kartograf via the package manager of your choice:
+
+```shell
+pip install kartograf
+```
+
+```shell
+conda install -c conda-forge kartograf
+```
+
+Or use Kartograf from the OpenFE Environment (soon).
+
+For Developing Kartograf, you might want to use this approach:
+
+```shell
+git clone https://github.com/OpenFreeEnergy/kartograf.git
+
+cd kartograf
+conda env create -f environment.yml
+
+conda activate kartograf
+pip install .
+
+```
+## References
+
+
+
```

### Comparing `kartograf-0.5.1/pyproject.toml` & `kartograf-0.5.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,54 @@
-[build-system]
-requires=[
-	"setuptools>=61.0",
-	"versioningit",
-]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "kartograf"
-dynamic = ["version"]
-authors=[
-    {name="Benjamin Ries", email="benjamin-ries@outlook.com"},
-    {name="David Swenson", email="dwhswenson@gmail.com"},
-    {name="Irfan Alibay", email="irfan.alibay@gmail.com"},
-    {name="Mike Henry", email="mike.henry@choderalab.org"},
-    {name="Richard J Gowers", email="richardjgowers@gmail.com"},
-]
-dependencies = [
-  'rdkit',
-  'scipy',
-  'numpy',
-  'gufe',
-]
-description="Kartograf is a package for mapping geometrically atoms of two molecules. (like you need it with hybrid topology)"
-readme="README.md"
-requires-python = ">=3.9"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/OpenFreeEnergy/kartograf"
-
-[tool.versioningit]
-default-version = "1+unknown"
-
-[tool.versioningit.format]
-distance = "{base_version}+{distance}.{vcs}{rev}"
-dirty = "{base_version}+{distance}.{vcs}{rev}.dirty"
-distance-dirty = "{base_version}+{distance}.{vcs}{rev}.dirty"
-
-[tool.versioningit.vcs]
-method = "git" 
-match = ["*"]
-default-tag = "0.0.0"
-
-[tool.versioningit.write]
-file = "src/kartograf/_version.py"
+[build-system]
+requires=[
+	"setuptools>=61.0",
+	"versioningit",
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "kartograf"
+dynamic = ["version"]
+authors=[
+    {name="Benjamin Ries", email="benjamin-ries@outlook.com"},
+    {name="David Swenson", email="dwhswenson@gmail.com"},
+    {name="Irfan Alibay", email="irfan.alibay@gmail.com"},
+    {name="Mike Henry", email="mike.henry@choderalab.org"},
+    {name="Richard J Gowers", email="richardjgowers@gmail.com"},
+]
+dependencies = [
+  'rdkit',
+  'scipy',
+  'numpy',
+  'gufe',
+  'ipywidgets',
+]
+description="Kartograf is a package for mapping geometrically atoms of two molecules. (like you need it with hybrid topology)"
+readme="README.md"
+requires-python = ">=3.9"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/OpenFreeEnergy/kartograf"
+
+[tool.poetry.extras]
+vis = ["openfe",   'py3Dmol']
+
+[tool.versioningit]
+default-version = "1+unknown"
+
+[tool.versioningit.format]
+distance = "{base_version}+{distance}.{vcs}{rev}"
+dirty = "{base_version}+{distance}.{vcs}{rev}.dirty"
+distance-dirty = "{base_version}+{distance}.{vcs}{rev}.dirty"
+
+[tool.versioningit.vcs]
+method = "git" 
+match = ["*"]
+default-tag = "0.0.0"
+
+[tool.versioningit.write]
+file = "src/kartograf/_version.py"
```

### Comparing `kartograf-0.5.1/src/kartograf/atom_align.py` & `kartograf-0.5.2/src/kartograf/atom_align.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-from copy import deepcopy
-
-from rdkit import Chem
-from rdkit.Chem import AllChem
-from rdkit.Chem import rdFMCS
-from rdkit.Chem import rdMolAlign
-
-from gufe import SmallMoleculeComponent
-
-import logging
-
-log = logging.getLogger(__name__)
-
-
-def align_mol_sceletons(
-    mol: SmallMoleculeComponent,
-    ref_mol: SmallMoleculeComponent,
-) -> SmallMoleculeComponent:
-    """
-        WORK IN PROGRESS!
-        This i a Wrapper for rdkit - MCS align
-        Aligns very simply molecule to the reference molecule, based on the shared MCS.
-
-    Parameters
-    ----------
-    mol : SmallMoleculeComponent
-        molecule to be aligned to molA (will be moved)
-    ref_mol : SmallMoleculeComponent
-        molecule with the reference_positions.
-
-    Returns
-    -------
-    SmallMoleculeComponent
-        return an aligned copy of molB
-    """
-    mol = deepcopy(mol)
-
-    mol1b = ref_mol._rdkit
-    mol2b = mol._rdkit
-
-    # MCS
-    p = rdFMCS.MCSParameters()
-    p.AtomTyper = rdFMCS.AtomCompare.CompareAny
-
-    res = rdFMCS.FindMCS([mol1b, mol2b], p)
-
-    # convert match to mapping
-    q = Chem.MolFromSmarts(res.smartsString)
-    logging.debug(q)
-
-    m1_idx = mol1b.GetSubstructMatch(q)
-    m2_idx = mol2b.GetSubstructMatch(q)
-    logging.debug(m1_idx, m2_idx)
-
-    idx_mappings = list(zip(m2_idx, m1_idx))
-
-    rms = AllChem.AlignMol(
-        prbMol=mol2b,
-        refMol=mol1b,
-        atomMap=idx_mappings,
-    )
-    logging.debug(rms)
-
-    mol._rdkit = mol2b
-    return mol
-
-def align_mol_shape(mol:SmallMoleculeComponent, ref_mol:SmallMoleculeComponent)->Chem.Mol:
-    """
-        WORK IN PROGRESS!
-        This i a Wrapper for rdkit / OPEN3DAlign
-        Aligns shape based two SmallMoleculeComponents.
-
-    Parameters
-    ----------
-    mol : SmallMoleculeComponent
-        molecule to be aligned to molA (will be moved)
-    ref_mol : SmallMoleculeComponent
-        molecule with the reference_positions.
-
-    Returns
-    -------
-    SmallMoleculeComponent
-        return an aligned copy of molB
-    """
-    mol = deepcopy(mol)
-
-    mol1b = ref_mol._rdkit
-    mol2b = mol._rdkit
-    pyO3A = rdMolAlign.GetO3A(prbMol=mol2b, refMol=mol1b,)
-    score = pyO3A.Align()
-    logging.debug("alignment score: "+str(score))
-
-    mol._rdkit = mol2b
+from copy import deepcopy
+
+from rdkit import Chem
+from rdkit.Chem import AllChem
+from rdkit.Chem import rdFMCS
+from rdkit.Chem import rdMolAlign
+
+from gufe import SmallMoleculeComponent
+
+import logging
+
+log = logging.getLogger(__name__)
+
+
+def align_mol_sceletons(
+    mol: SmallMoleculeComponent,
+    ref_mol: SmallMoleculeComponent,
+) -> SmallMoleculeComponent:
+    """
+        WORK IN PROGRESS!
+        This i a Wrapper for rdkit - MCS align
+        Aligns very simply molecule to the reference molecule, based on the shared MCS.
+
+    Parameters
+    ----------
+    mol : SmallMoleculeComponent
+        molecule to be aligned to molA (will be moved)
+    ref_mol : SmallMoleculeComponent
+        molecule with the reference_positions.
+
+    Returns
+    -------
+    SmallMoleculeComponent
+        return an aligned copy of molB
+    """
+    mol = deepcopy(mol)
+
+    mol1b = ref_mol._rdkit
+    mol2b = mol._rdkit
+
+    # MCS
+    p = rdFMCS.MCSParameters()
+    p.AtomTyper = rdFMCS.AtomCompare.CompareAny
+
+    res = rdFMCS.FindMCS([mol1b, mol2b], p)
+
+    # convert match to mapping
+    q = Chem.MolFromSmarts(res.smartsString)
+    logging.debug(q)
+
+    m1_idx = mol1b.GetSubstructMatch(q)
+    m2_idx = mol2b.GetSubstructMatch(q)
+    logging.debug(m1_idx, m2_idx)
+
+    idx_mappings = list(zip(m2_idx, m1_idx))
+
+    rms = AllChem.AlignMol(
+        prbMol=mol2b,
+        refMol=mol1b,
+        atomMap=idx_mappings,
+    )
+    logging.debug(rms)
+
+    mol._rdkit = mol2b
+    return mol
+
+def align_mol_shape(mol:SmallMoleculeComponent, ref_mol:SmallMoleculeComponent)->Chem.Mol:
+    """
+        WORK IN PROGRESS!
+        This i a Wrapper for rdkit / OPEN3DAlign
+        Aligns shape based two SmallMoleculeComponents.
+
+    Parameters
+    ----------
+    mol : SmallMoleculeComponent
+        molecule to be aligned to molA (will be moved)
+    ref_mol : SmallMoleculeComponent
+        molecule with the reference_positions.
+
+    Returns
+    -------
+    SmallMoleculeComponent
+        return an aligned copy of molB
+    """
+    mol = deepcopy(mol)
+
+    mol1b = ref_mol._rdkit
+    mol2b = mol._rdkit
+    pyO3A = rdMolAlign.GetO3A(prbMol=mol2b, refMol=mol1b,)
+    score = pyO3A.Align()
+    logging.debug("alignment score: "+str(score))
+
+    mol._rdkit = mol2b
     return mol
```

### Comparing `kartograf-0.5.1/src/kartograf/atom_mapper.py` & `kartograf-0.5.2/src/kartograf/atom_mapper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,786 +1,790 @@
-# This code is part of OpenFE and is licensed under the MIT license.
-# For details, see https://github.com/OpenFreeEnergy/kartograf
-
-import copy
-import inspect
-import numpy as np
-from enum import Enum
-
-from collections import OrderedDict
-from collections.abc import Iterator
-
-from rdkit import Chem
-
-from scipy.sparse import csr_matrix
-from scipy.optimize import linear_sum_assignment
-from scipy.sparse.csgraph import connected_components
-
-from typing import Callable, Dict, Iterable, List, Optional, Set, Tuple, Union
-
-from gufe import SmallMoleculeComponent
-from gufe import LigandAtomMapping
-from gufe import AtomMapping, AtomMapper
-
-import logging
-
-from .filters import (
-    filter_atoms_h_only_h_mapped,
-    filter_ringbreak_changes,
-    filter_ringsize_changes
-)
-
-log = logging.getLogger(__name__)
-
-
-# Enums:
-class mapping_algorithm(Enum):
-    """
-        This enum helps selecting the optimization algorithm for the distance graph based atom mapping.
-    """
-    linear_sum_assignment = "LSA"
-    minimal_spanning_tree = "MST"
-
-
-# Helper:
-vector_eucledean_dist = calculate_edge_weight = lambda x, y: np.sqrt(
-    np.sum(np.square(y - x), axis=1)
-)
-
-
-# Implementation of Mapper:
-class KartografAtomMapper(AtomMapper):
-    atom_max_distance: float
-    atom_ring_matches_ring: bool
-    atom_map_hydrogens: bool
-    mapping_algorithm: mapping_algorithm
-
-    _filter_funcs: list[
-        Callable[[Chem.Mol, Chem.Mol, dict[int, int]], dict[int, int]]
-    ]
-
-    def __init__(
-        self,
-        *,
-        atom_ring_matches_ring: bool = False,
-        atom_max_distance: float = 0.95,
-        atom_map_hydrogens: bool = True,
-        map_hydrogens_on_hydrogens_only: bool = False,
-        additional_mapping_filter_functions: Optional[
-            Iterable[
-                Callable[[Chem.Mol, Chem.Mol, dict[int, int]], dict[int, int]]
-            ]
-        ] = [filter_ringbreak_changes, filter_ringsize_changes],
-        _mapping_algorithm: Optional[
-            mapping_algorithm
-        ] = mapping_algorithm.linear_sum_assignment,
-    ):
-        """
-        This mapper is a homebrew, that utilises rdkit in order
-        to generate an atom-mapping based on the coordinates of two molecules.
-
-        Parameters
-        ----------
-        atom_ring_matches_ring : bool, optional
-            default False
-        atom_max_distance : float, optional
-            geometric criteria for two atoms, how far their distance
-            can be maximal (in Angstrom). Default 0.95
-        map_hydrogens_on_hydrogens_only : bool, optional
-            map hydrogens only on hydrogens. Default False
-        additional_mapping_filter_functions : Iterable[Callable[[Chem.Mol, Chem.Mol, Dict[int, int]], Dict[int, int]]], optional
-            with this optional parameter you can further filter the distance based mappings with your own custom filters, provided as iterables.
-            as default we suggest to avoid ring size/breaking changes.
-        _mapping_algorithm : str, optional
-            mapping_algorithm.linear_sum_assignment
-
-        """
-        self.atom_max_distance = atom_max_distance
-        self.atom_ring_matches_ring = atom_ring_matches_ring
-        self.atom_map_hydrogens = atom_map_hydrogens
-        self._map_hydrogens_on_hydrogens_only = False
-
-        self._filter_funcs = []
-        if map_hydrogens_on_hydrogens_only:
-            self._filter_funcs.append(filter_atoms_h_only_h_mapped)
-        if additional_mapping_filter_functions is not None:
-            self._filter_funcs.extend(additional_mapping_filter_functions)
-
-        if _mapping_algorithm == _mapping_algorithm.linear_sum_assignment:
-            self._map_hydrogens_on_hydrogens_only = True
-            self.mapping_algorithm = self._linearSumAlgorithm_map
-        elif _mapping_algorithm == _mapping_algorithm.minimal_spanning_tree:
-            self.mapping_algorithm = self._minimalSpanningTree_map
-        else:
-            raise ValueError(
-                "Mapping algorithm not implemented or unknown (options: MST or LSA). got key: "
-                + str(_mapping_algorithm)
-            )
-
-    """
-        Properties
-    """
-
-    @property
-    def map_hydrogens_on_hydrogens_only(self)->bool:
-        """this property is a shortcut for setting hydrogen shall be mapped only on hydrogen filter."""
-        return self._map_hydrogens_on_hydrogens_only
-    @map_hydrogens_on_hydrogens_only.setter
-    def map_hydrogens_on_hydrogens_only(self, s:bool):
-        self._map_hydrogens_on_hydrogens_only = s
-        if(s and filter_atoms_h_only_h_mapped not in self._filter_funcs):
-            self._filter_funcs.insert(0, filter_atoms_h_only_h_mapped)
-        elif(filter_atoms_h_only_h_mapped in self._filter_funcs):
-            self._filter_funcs.remove(filter_atoms_h_only_h_mapped)
-
-    """
-        Privat - Serialize
-    """
-
-    @classmethod
-    def _from_dict(cls, d: dict):
-        """Deserialize from dict representation"""
-        if(any([not k in cls._defaults() for k in d])):
-            raise ValueError("I don't know about all the keys here"+str(list(filter(lambda k: k in cls._defaults(), d.keys()))))
-        return cls(**d)
-
-    def _to_dict(self) -> dict:
-
-        d = {}
-        for key in self._defaults():
-            if(hasattr(self, key)):
-                d[key] = getattr(self, key)
-        return d
-
-    @classmethod
-    def _defaults(cls):
-        """This method should be overridden to provide the dict of defaults
-            appropriate for the `GufeTokenizable` subclass.
-        """
-        sig = inspect.signature(cls.__init__)
-
-        defaults = {
-            param.name: param.default for param in sig.parameters.values()
-            if param.default is not inspect.Parameter.empty
-        }
-
-        return defaults
-
-
-    """
-       Private - Set Operations
-    """
-
-    @classmethod
-    def _filter_mapping_for_max_overlapping_connected_atom_set(
-            cls, moleculeA: Chem.Mol, moleculeB: Chem.Mol, atom_mapping: Dict[int, int]
-    ) -> Dict[int, int]:
-        """
-            This algorithm finds the maximal overlapping connected  set of two molecules and a given mapping.
-            In order to accomplish this the following steps are executed:
-            1. find all connnected sets for molecule A and molecule B
-            2. get the maximal overlap between a set of molecule A and a set of molecule B
-            3. reduce the atom_mapping to the found maximal overlapping sets.
-
-        Parameters
-        ----------
-        moleculeA : Chem.Mol
-            molecule A which mapped atoms are represented by atom_mapping keys
-        moleculeB : Chem.Mol
-            molecule B which mapped atoms are represented by atom_mapping values
-        atom_mapping : Dict[int, int]
-            input atom_mapping, to be filtered.
-
-        Returns
-        -------
-        Dict[int, int]
-            a filtered mapping, containing the maximal overlapping filter.
-
-        """
-        # get connected sets from mappings
-        sets_a = cls._get_connected_atom_subsets(moleculeA, atom_mapping.keys())
-        sets_b = cls._get_connected_atom_subsets(moleculeB, atom_mapping.values())
-
-        log.debug(
-            "Found connected sets: "
-            + "\t".join(map(str, [sets_a, sets_b, atom_mapping]))
-        )
-
-        # get maximally overlapping largest sets
-        ((max_set_a_id, max_set_b_id), max_set) = cls._get_maximal_mapping_set_overlap(
-            sets_a, sets_b, atom_mapping
-        )
-
-        # filter mapping for atoms in maximally overlapping sets
-        atom_mapping = cls._filter_mapping_for_set_overlap(
-            sets_a[max_set_a_id], sets_b[max_set_b_id], atom_mapping
-        )
-
-        log.debug(
-            "Found connected set overlaps: "
-            + "\t".join(map(str, [max_set_a_id, max_set_b_id, max_set, atom_mapping]))
-        )
-
-        return atom_mapping
-
-    @staticmethod
-    def _get_connected_atom_subsets(
-        mol: Chem.Mol, to_be_searched: List[int]
-    ) -> List[Set[int]]:
-        """
-        Get the connected sets of all to_be_searched atom indices in mol. Connected means the atoms in a resulting connected set are connected by covalent bonds.
-
-        Parameters
-        ----------
-        mol : Chem.Mol
-            molecule graph containing the bond information
-        to_be_searched : List[int]
-            atom indices, that shall be grouped by connections.
-
-        Returns
-        -------
-        List[Set[int]]
-            return list of connected sets from the to_be_searched atom index list found in mol.
-        """
-        # Get bonded atoms sets
-        bonded_atom_sets = []
-        for aid in to_be_searched:
-            a = mol.GetAtomWithIdx(int(aid))
-            bond_atoms = [b.GetOtherAtomIdx(aid) for b in a.GetBonds()]
-            connected_atoms = set([aid] + bond_atoms)
-
-            # filter to not connect non mapped atoms
-            filtered_connected_atoms = set(
-                filter(lambda x: x in to_be_searched, connected_atoms)
-            )
-
-            # NO mapped atom connected?
-            if len(filtered_connected_atoms) == 1:
-                continue
-            else:
-                bonded_atom_sets.append(filtered_connected_atoms)
-        bonded_atom_sets = list(sorted(bonded_atom_sets))
-
-        log.debug("Bonded atom Sets: " + str(bonded_atom_sets))
-
-        # add new set or merge with existing set
-        atom_mappings = {i: a for i, a in enumerate(to_be_searched)}
-        r_atom_mappings = {a: i for i, a in enumerate(to_be_searched)}
-        max_n = len(to_be_searched)
-
-        connection_matrix = np.zeros(shape=(max_n, max_n))
-        for set_i in bonded_atom_sets:
-            for ai in set_i:
-                for aj in set_i:
-                    connection_matrix[r_atom_mappings[ai]][r_atom_mappings[aj]] = 1
-
-        log.debug("Adjacency Matrix: " + str(connection_matrix))
-
-        # get connected components
-        matrix = csr_matrix(connection_matrix)
-        n_components, labels = connected_components(csgraph=matrix, directed=False)
-
-        log.debug("Connected Components: " + str(n_components) + "\t" + str(labels))
-
-        # Translate back
-        merged_connnected_atom_sets = []
-        labels_sizes = [
-            label
-            for label, _ in sorted(
-                np.vstack(np.unique(labels, return_counts=True)).T,
-                key=lambda x: x[1],
-                reverse=True,
-            )
-        ]
-        for selected_label in labels_sizes:
-            connected_atoms_ids = list(
-                sorted(
-                    [
-                        atom_mappings[i]
-                        for i, label in enumerate(labels)
-                        if label == selected_label
-                    ]
-                )
-            )
-            merged_connnected_atom_sets.append(connected_atoms_ids)
-
-        log.debug("Merged Sets:" + str(merged_connnected_atom_sets))
-
-        return merged_connnected_atom_sets
-
-    @staticmethod
-    def _get_maximal_mapping_set_overlap(
-        sets_a: Iterable[Set], sets_b: Iterable[Set], mapping: Dict[int, int]
-    ) -> Tuple[Set, Set]:
-        """
-        get the largest set overlaps in the mapping of set_a and set_b.
-
-        Parameters
-        ----------
-        sets_a : Iterable[Set]
-            connected sets resulting from the mapping in state A
-        sets_b : Iterable[Set]
-            connected sets resulting from the mapping in state B
-        mapping : Dict[int, int]
-            proposed atom mapping from state A to state B
-
-        Returns
-        -------
-        Tuple[Set, Set]
-            returns the found maximal and maximal overlapping sets of a and the set of b
-        """
-        # Calculate overlaps
-
-        log.debug("Input: " + str(sets_a) + " " + str(sets_b) + " " + str(mapping))
-
-        max_set_combi = {}
-        for ida, set_a in enumerate(sets_a):
-            mapped_set_a = {mapping[a] for a in set_a}
-            for idb, set_b in enumerate(sets_b):
-                set_intersection_size = len(mapped_set_a.intersection(set_b))
-                if set_intersection_size:
-                    max_set_combi[(ida, idb)] = {
-                        "overlap_count": set_intersection_size,
-                        "set_a_size": len(set_a),
-                        "set_b_size": len(set_b),
-                    }
-
-        # sort overlap by size
-        overlap_sorted_sets = OrderedDict(
-            sorted(
-                max_set_combi.items(),
-                key=lambda x: x[1]["overlap_count"],
-                reverse=False,
-            )
-        )
-
-        log.debug("Set overlap properties" + str(overlap_sorted_sets))
-
-        max_overlap_set_a_id, max_overlap_set_b_id = overlap_sorted_sets.popitem()
-        return max_overlap_set_a_id, max_overlap_set_b_id
-
-    @staticmethod
-    def _filter_mapping_for_set_overlap(
-        set_a: Set[int], set_b: Set[int], mapping: Dict[int, int]
-    ) -> Dict[int, int]:
-        """
-        This filter reduces the mapping dict to only in the sets contained atom IDs
-
-        Parameters
-        ----------
-        set_a : Set[int]
-            this set contains the allowed keys
-        set_b : Set[int]
-            this set contains the allowed values
-        mapping : Dict[int, int]
-            this mapping is to be filtered by the set values.
-
-        Returns
-        -------
-        Dict[int, int]
-            filtered mapping
-
-        """
-        filtered_mapping = {}
-        for atom_a, atom_b in mapping.items():
-            if atom_a in set_a and atom_b in set_b:
-                filtered_mapping[atom_a] = atom_b
-        return filtered_mapping
-
-
-    """
-        Utils
-    """
-
-    @staticmethod
-    def _get_full_distance_matrix(
-        atomA_pos: np.array,
-        atomB_pos: np.array,
-        metric: Callable[
-            [Union[float, Iterable], Union[float, Iterable]], Union[float, Iterable]
-        ] = vector_eucledean_dist,
-    ) -> np.array:
-        """
-            calculates a full distance matrix between the two given input position matrixes.
-
-
-        Parameters
-        ----------
-        atomA_pos : np.array
-            position matrix A
-        atomB_pos : np.array
-            position matrix B
-        metric : Callable[[Union[float, Iterable], Union[float, Iterable]], Union[float, Iterable]], optional
-            the applied metric to calculate the distance matrix. default metric: eucledean distance.
-
-        Returns
-        -------
-        np.array
-            returns a distance matrix.
-
-        """
-        distance_matrix = []
-        for atomPosA in atomA_pos:
-            atomPos_distances = metric(atomPosA, atomB_pos)
-            distance_matrix.append(atomPos_distances)
-        distance_matrix = np.array(distance_matrix)
-        return distance_matrix
-
-    @staticmethod
-    def _mask_atoms(
-        mol, mol_pos, map_hydrogens: bool = False, masked_atoms=[]
-    ) -> Tuple[Dict, List]:
-        """
-        Mask atoms
-
-        Parameters
-        ----------
-        mol
-        mol_pos
-        map_hydrogens
-        masked_atoms
-
-        Returns
-        -------
-
-        """
-        pos = []
-        masked_atomMapping = {}
-        for atom in mol.GetAtoms():
-            atom_id = atom.GetIdx()
-            if (
-                map_hydrogens or atom.GetSymbol() != "H"
-            ) and atom_id not in masked_atoms:
-                masked_atomMapping[len(masked_atomMapping)] = atom_id
-                pos.append(mol_pos[atom_id])
-        pos = np.array(pos)
-
-        return masked_atomMapping, pos
-
-    def _minimalSpanningTree_map(
-        self, distance_matrix: np.array, max_dist: float
-    ) -> Dict[int, int]:
-        """
-        This function is a numpy graph based implementation to build up an Atom Mapping purely on 3D criteria.
-
-        Parameters
-        ----------
-        distance_matrix: np.array
-            distances of atoms to each other.
-        max_dist: float
-            maximal distance of a atoms in a mapping.
-
-        Returns
-        -------
-        Dict[int, int]
-            mapping of atoms.
-        """
-
-        # distance matrix:  - full graph
-        log.debug("Got Distance Matrix: \n" + str(distance_matrix))
-        edges = []
-        for i, distance_row in enumerate(distance_matrix):
-            for j, dist in enumerate(distance_row):
-                edges.append([float(dist), int(i), int(j)])
-
-        edges = np.array(edges)
-        log.debug("Edges: \n" + str(edges))
-
-        # priority queue based on edge weight
-        sorted_edges = edges[edges[:, 0].argsort()]
-        log.debug("Sorted Edges: \n" + str(sorted_edges))
-
-        # MST like algorithm
-        mapping = {}
-        for w, x, y in sorted_edges:
-            if w >= max_dist:  # filter for max dist
-                break
-            else:
-                if x not in mapping.keys() and y not in mapping.values():
-                    mapping[int(x)] = int(y)
-
-        return mapping
-
-    @staticmethod
-    def _linearSumAlgorithm_map(
-        distance_matrix: np.array, max_dist: float
-    ) -> Dict[int, int]:
-        """
-        This function is a LSA based implementation to build up an Atom Mapping purely on 3D criteria.
-
-        Parameters
-        ----------
-        distance_matrix: np.array
-            distances of atoms to each other.
-        max_dist: float
-            maximal distance of a atoms in a mapping.
-
-        Returns
-        -------
-        Dict[int, int]
-            mapping of atoms.
-        """
-        row_ind, col_ind = linear_sum_assignment(distance_matrix)
-        raw_mapping = list(zip(map(int, row_ind), map(int, col_ind)))
-        # filter for mask value
-        mapping = dict(filter(lambda x: distance_matrix[x] < max_dist, raw_mapping))
-
-        return mapping
-
-    def _additional_filter_rules(
-        self, molA: Chem.Mol, molB: Chem.Mol, mapping: dict[int, int]
-    ) -> Dict[int, int]:
-        """
-        apply additional filter rules to the given mapping.
-
-        Parameters
-        ----------
-        molA : Chem.Mol
-            mol, with atoms contained in mapping keys.
-        molB : Chem.Mol
-            mol, with atoms contained in mapping values.
-        mapping : Dict[int, int]
-            mapping to be filtered
-
-        Returns
-        -------
-        Dict[int, int]
-            filtered mapping
-        """
-        filtered_mapping = copy.deepcopy(mapping)
-        for filter_rule in self._filter_funcs:
-            filtered_mapping = filter_rule(molA, molB, filtered_mapping)
-        return filtered_mapping
-
-    def _calculate_mapping(
-        self,
-        molA: Chem.Mol,
-        molB: Chem.Mol,
-        max_d: float = 0.95,
-        masked_atoms_molA: Optional[list[int]] = None,
-        masked_atoms_molB: Optional[list[int]] = None,
-        pre_mapped_atoms: Optional[dict[int, int]] = None,
-        map_hydrogens: bool = True,
-    ) -> dict[int, int]:
-        """
-            find a mapping between two molecules based on 3D coordinates. This is a helper function for the suggest mapping functions.
-
-        Parameters
-        ----------
-        molA : Chem.Mol
-            rdkit Molecule A
-        molB : Chem.Mol
-            rdkit Molecule B
-        max_d : float, optional
-            maximal allowed distance for atoms to be mapped, by default 0.95
-        masked_atoms_molA : list, optional
-            remove categorical atoms by index of MolA from the mapping, by default []
-        masked_atoms_molB : list, optional
-            remove categorical atoms by index of MolB from the mapping, by default []
-        pre_mapped_atoms : dict, optional
-            pre_mapped atoms, that need to be part of the mapping, by default {}
-        map_hydrogens : bool, optional
-            if True map hydrogens as well, will hapen after heavy atom mapping, by default True
-
-        Returns
-        -------
-        AtomMapping
-            _description_
-        """
-        if masked_atoms_molA is None:
-            masked_atoms_molA = []
-        if masked_atoms_molB is None:
-            masked_atoms_molB = []
-        if pre_mapped_atoms is None:
-            pre_mapped_atoms = dict()
-
-        molA_pos = molA.GetConformer().GetPositions()
-        molB_pos = molB.GetConformer().GetPositions()
-        masked_atoms_molA = copy.deepcopy(masked_atoms_molA)
-        masked_atoms_molB = copy.deepcopy(masked_atoms_molB)
-        pre_mapped_atoms = copy.deepcopy(pre_mapped_atoms)
-
-        if len(pre_mapped_atoms) > 0:
-            masked_atoms_molA.extend(pre_mapped_atoms.keys())
-            masked_atoms_molB.extend(pre_mapped_atoms.values())
-
-        log.debug("Positions lengths: " + str(len(molA_pos)) + " " + str(len(molB_pos)))
-        log.debug("Positions: \n" + "\n\t".join(map(str, [molA_pos, molB_pos])))
-        log.debug("masked_atoms_molA: " + str(masked_atoms_molA))
-        log.debug("masked_atoms_molB: " + str(masked_atoms_molB))
-        log.debug("pre_mapped_atoms: " + str(pre_mapped_atoms))
-        log.debug("map_hydrogens: " + str(map_hydrogens))
-
-        log.info("Masking Atoms")
-
-        molA_masked_atomMapping, molA_pos = self._mask_atoms(
-            mol=molA,
-            mol_pos=molA_pos,
-            masked_atoms=masked_atoms_molA,
-            map_hydrogens=map_hydrogens,
-        )
-        molB_masked_atomMapping, molB_pos = self._mask_atoms(
-            mol=molB,
-            mol_pos=molB_pos,
-            masked_atoms=masked_atoms_molB,
-            map_hydrogens=map_hydrogens,
-        )
-
-        log.debug(
-            "Remove Masked Atoms: \n"
-            + "\n\t".join(map(str, [molA_masked_atomMapping, molB_masked_atomMapping]))
-            + "\n"
-            + "\n\t".join(map(str, [molA_pos, molB_pos]))
-        )
-        log.debug(
-            "filtered Masked Positions lengths: "
-            + "\t".join(map(str, [len(molA_pos), len(molB_pos)]))
-        )
-
-        if len(molA_pos) == 0 or len(molB_pos) == 0:  # TODO: check if this is correct
-            if(len(pre_mapped_atoms)==0): log.warning("no mappable Atoms were found!")
-            return pre_mapped_atoms
-
-        # Calculate mapping
-        log.info("Build Distance Matrix")
-        # distance matrix:  - full graph
-        distance_matrix = self._get_full_distance_matrix(molA_pos, molB_pos)
-        log.debug("Distance Matrix: \n" + str(distance_matrix))
-
-        # Mask distance matrix with max_d
-        # np.inf is considererd as not possible in lsa implementation - therefore use a high value
-        self.mask_dist_val = max_d * 10**6
-        masked_dmatrix = np.array(
-            np.ma.where(distance_matrix < max_d, distance_matrix, self.mask_dist_val)
-        )
-        log.debug(
-            "masked Distance Matrix: " + str(max_d) + "\n\t" + str(masked_dmatrix)
-        )
-
-        # solve atom mappings
-        log.info("Calculate Mapping")
-        mapping = self.mapping_algorithm(
-            distance_matrix=masked_dmatrix, max_dist=self.mask_dist_val
-        )
-        log.debug("Raw Mapping: " + str(mapping))
-
-        if len(mapping) == 0:  # TODO: check if this is correct
-            if(len(pre_mapped_atoms)==0): log.warning("no mapping could be found!")
-            return pre_mapped_atoms
-
-        # reverse any prior masking:
-        mapping = {
-            molA_masked_atomMapping[k]: molB_masked_atomMapping[v]
-            for k, v in mapping.items()
-        }
-
-        # filter mapping for rules:
-        if self._filter_funcs is not None:
-            mapping = self._additional_filter_rules(molA, molB, mapping)
-
-        if len(pre_mapped_atoms) > 0:
-            mapping.update(pre_mapped_atoms)
-        log.debug("reverse Masking Mapping: " + str(mapping))
-
-        # Reduce mapping to maximally overlapping two connected sets
-        log.info("Find Maximal overlapping connected sets of mapped atoms")
-        mapping = self._filter_mapping_for_max_overlapping_connected_atom_set(
-            moleculeA=molA, moleculeB=molB, atom_mapping=mapping
-        )
-        log.debug("Set overlap Mapping: " + str(mapping))
-
-        return mapping
-
-    """
-        Mapping functions
-    """
-
-    def suggest_mapping_from_rdmols(
-        self,
-        molA: Chem.Mol,
-        molB: Chem.Mol,
-        masked_atoms_molA: Optional[list] = None,
-        masked_atoms_molB: Optional[list] = None,
-        pre_mapped_atoms: Optional[dict] = None,
-    ) -> dict[int, int]:
-        """
-        The function effectivly maps the two molecules on to each other and
-        applies the given settings by the obj.
-
-        Parameters
-        ----------
-        molA, molB : rdkit.Chem.Mol
-            two rdkit molecules that should be mapped onto each other
-        masked_atoms_molA : list, optional
-            remove categorical atoms by index of MolA from the mapping, by default []
-        masked_atoms_molB : list, optional
-            remove categorical atoms by index of MolB from the mapping, by default []
-        pre_mapped_atoms : dict, optional
-            pre_mapped atoms, that need to be part of the mapping, by default {}
-        """
-        if masked_atoms_molA is None:
-            masked_atoms_molA = []
-        if masked_atoms_molB is None:
-            masked_atoms_molB = []
-        if pre_mapped_atoms is None:
-            pre_mapped_atoms = {}
-
-        molA = Chem.Mol(molA)
-        molB = Chem.Mol(molB)
-        masked_atoms_molA = copy.deepcopy(masked_atoms_molA)
-        masked_atoms_molB = copy.deepcopy(masked_atoms_molB)
-        pre_mapped_atoms = copy.deepcopy(pre_mapped_atoms)
-
-        log.info("#################################")
-        log.info("Map Heavy Atoms ")
-        log.info("#################################")
-
-        mapping = self._calculate_mapping(
-            molA,
-            molB,
-            max_d=self.atom_max_distance,
-            masked_atoms_molA=masked_atoms_molA,
-            masked_atoms_molB=masked_atoms_molB,
-            pre_mapped_atoms=pre_mapped_atoms,
-            map_hydrogens=False,
-        )
-
-        if self.atom_map_hydrogens:
-            log.info("#################################")
-            log.info("Map Hydrogen Atoms: ")
-            log.info("#################################")
-
-            pre_mapped_atoms.update(mapping)
-
-            mapping = self._calculate_mapping(
-                molA,
-                molB,
-                max_d=self.atom_max_distance,
-                masked_atoms_molA=masked_atoms_molA,
-                masked_atoms_molB=masked_atoms_molB,
-                pre_mapped_atoms=pre_mapped_atoms,
-                map_hydrogens=self.atom_map_hydrogens,
-            )
-
-        return mapping
-
-    def suggest_mappings(
-        self, A: SmallMoleculeComponent, B: SmallMoleculeComponent
-    ) -> Iterator[AtomMapping]:
-        """
-        return a generator for atom mappings.
-
-        Parameters
-        ----------
-        A : SmallMoleculeComponent
-            molecule A to be mapped.
-        B : SmallMoleculeComponent
-            molecule B to be mapped.
-
-        Returns
-        -------
-        Iterator[AtomMapping]
-            returns an interator of possible atom mappings.
-        """
-        yield LigandAtomMapping(
-            A, B, self.suggest_mapping_from_rdmols(molA=A.to_rdkit(), molB=B.to_rdkit())
-        )
+# This code is part of OpenFE and is licensed under the MIT license.
+# For details, see https://github.com/OpenFreeEnergy/kartograf
+
+import copy
+import inspect
+import numpy as np
+from enum import Enum
+
+from collections import OrderedDict
+from collections.abc import Iterator
+
+from rdkit import Chem
+
+from scipy.sparse import csr_matrix
+from scipy.optimize import linear_sum_assignment
+from scipy.sparse.csgraph import connected_components
+
+from typing import Callable, Dict, Iterable, List, Optional, Set, Tuple, Union
+
+from gufe import SmallMoleculeComponent
+from gufe import LigandAtomMapping
+from gufe import AtomMapping, AtomMapper
+
+import logging
+
+from .filters import (
+    filter_atoms_h_only_h_mapped,
+    filter_ringbreak_changes,
+    filter_ringsize_changes
+)
+
+log = logging.getLogger(__name__)
+
+
+# Enums:
+class mapping_algorithm(Enum):
+    """
+        This enum helps selecting the optimization algorithm for the distance graph based atom mapping.
+    """
+    linear_sum_assignment = "LSA"
+    minimal_spanning_tree = "MST"
+
+
+# Helper:
+vector_eucledean_dist = calculate_edge_weight = lambda x, y: np.sqrt(
+    np.sum(np.square(y - x), axis=1)
+)
+
+
+# Implementation of Mapper:
+class KartografAtomMapper(AtomMapper):
+    atom_max_distance: float
+    atom_ring_matches_ring: bool
+    atom_map_hydrogens: bool
+    mapping_algorithm: mapping_algorithm
+
+    _filter_funcs: list[
+        Callable[[Chem.Mol, Chem.Mol, dict[int, int]], dict[int, int]]
+    ]
+
+    def __init__(
+        self,
+        *,
+        atom_ring_matches_ring: bool = False,
+        atom_max_distance: float = 0.95,
+        atom_map_hydrogens: bool = True,
+        map_hydrogens_on_hydrogens_only: bool = False,
+        additional_mapping_filter_functions: Optional[
+            Iterable[
+                Callable[[Chem.Mol, Chem.Mol, dict[int, int]], dict[int, int]]
+            ]
+        ] = [filter_ringbreak_changes, filter_ringsize_changes],
+        _mapping_algorithm: Optional[
+            mapping_algorithm
+        ] = mapping_algorithm.linear_sum_assignment,
+    ):
+        """
+        This mapper is a homebrew, that utilises rdkit in order
+        to generate an atom-mapping based on the coordinates of two molecules.
+
+        Parameters
+        ----------
+        atom_ring_matches_ring : bool, optional
+            default False
+        atom_max_distance : float, optional
+            geometric criteria for two atoms, how far their distance
+            can be maximal (in Angstrom). Default 0.95
+        map_hydrogens_on_hydrogens_only : bool, optional
+            map hydrogens only on hydrogens. Default False
+        additional_mapping_filter_functions : Iterable[Callable[[Chem.Mol, Chem.Mol, Dict[int, int]], Dict[int, int]]], optional
+            with this optional parameter you can further filter the distance based mappings with your own custom filters, provided as iterables.
+            as default we suggest to avoid ring size/breaking changes.
+        _mapping_algorithm : str, optional
+            mapping_algorithm.linear_sum_assignment
+
+        """
+        self.atom_max_distance = atom_max_distance
+        self.atom_ring_matches_ring = atom_ring_matches_ring
+        self.atom_map_hydrogens = atom_map_hydrogens
+        self._map_hydrogens_on_hydrogens_only = False
+
+        self._filter_funcs = []
+        if map_hydrogens_on_hydrogens_only:
+            self._filter_funcs.append(filter_atoms_h_only_h_mapped)
+        if additional_mapping_filter_functions is not None:
+            self._filter_funcs.extend(additional_mapping_filter_functions)
+
+        if _mapping_algorithm == _mapping_algorithm.linear_sum_assignment:
+            self._map_hydrogens_on_hydrogens_only = True
+            self.mapping_algorithm = self._linearSumAlgorithm_map
+        elif _mapping_algorithm == _mapping_algorithm.minimal_spanning_tree:
+            self.mapping_algorithm = self._minimalSpanningTree_map
+        else:
+            raise ValueError(
+                "Mapping algorithm not implemented or unknown (options: MST or LSA). got key: "
+                + str(_mapping_algorithm)
+            )
+
+    """
+        Properties
+    """
+
+    @property
+    def map_hydrogens_on_hydrogens_only(self)->bool:
+        """this property is a shortcut for setting hydrogen shall be mapped only on hydrogen filter."""
+        return self._map_hydrogens_on_hydrogens_only
+    @map_hydrogens_on_hydrogens_only.setter
+    def map_hydrogens_on_hydrogens_only(self, s:bool):
+        self._map_hydrogens_on_hydrogens_only = s
+        if(s and filter_atoms_h_only_h_mapped not in self._filter_funcs):
+            self._filter_funcs.insert(0, filter_atoms_h_only_h_mapped)
+        elif(filter_atoms_h_only_h_mapped in self._filter_funcs):
+            self._filter_funcs.remove(filter_atoms_h_only_h_mapped)
+
+    """
+        Privat - Serialize
+    """
+
+    @classmethod
+    def _from_dict(cls, d: dict):
+        """Deserialize from dict representation"""
+        if(any([not k in cls._defaults() for k in d])):
+            raise ValueError("I don't know about all the keys here"+str(list(filter(lambda k: k in cls._defaults(), d.keys()))))
+        return cls(**d)
+
+    def _to_dict(self) -> dict:
+
+        d = {}
+        for key in self._defaults():
+            if(hasattr(self, key)):
+                d[key] = getattr(self, key)
+        return d
+
+    @classmethod
+    def _defaults(cls):
+        """This method should be overridden to provide the dict of defaults
+            appropriate for the `GufeTokenizable` subclass.
+        """
+        sig = inspect.signature(cls.__init__)
+
+        defaults = {
+            param.name: param.default for param in sig.parameters.values()
+            if param.default is not inspect.Parameter.empty
+        }
+
+        return defaults
+
+
+    """
+       Private - Set Operations
+    """
+
+    @classmethod
+    def _filter_mapping_for_max_overlapping_connected_atom_set(
+            cls, moleculeA: Chem.Mol, moleculeB: Chem.Mol, atom_mapping: Dict[int, int]
+    ) -> Dict[int, int]:
+        """
+            This algorithm finds the maximal overlapping connected  set of two molecules and a given mapping.
+            In order to accomplish this the following steps are executed:
+            1. find all connnected sets for molecule A and molecule B
+            2. get the maximal overlap between a set of molecule A and a set of molecule B
+            3. reduce the atom_mapping to the found maximal overlapping sets.
+
+        Parameters
+        ----------
+        moleculeA : Chem.Mol
+            molecule A which mapped atoms are represented by atom_mapping keys
+        moleculeB : Chem.Mol
+            molecule B which mapped atoms are represented by atom_mapping values
+        atom_mapping : Dict[int, int]
+            input atom_mapping, to be filtered.
+
+        Returns
+        -------
+        Dict[int, int]
+            a filtered mapping, containing the maximal overlapping filter.
+
+        """
+        # get connected sets from mappings
+        sets_a = cls._get_connected_atom_subsets(moleculeA, atom_mapping.keys())
+        sets_b = cls._get_connected_atom_subsets(moleculeB, atom_mapping.values())
+
+        log.debug(
+            "Found connected sets: "
+            + "\t".join(map(str, [sets_a, sets_b, atom_mapping]))
+        )
+
+        # get maximally overlapping largest sets
+        ((max_set_a_id, max_set_b_id), max_set) = cls._get_maximal_mapping_set_overlap(
+            sets_a, sets_b, atom_mapping
+        )
+
+        # filter mapping for atoms in maximally overlapping sets
+        atom_mapping = cls._filter_mapping_for_set_overlap(
+            sets_a[max_set_a_id], sets_b[max_set_b_id], atom_mapping
+        )
+
+        log.debug(
+            "Found connected set overlaps: "
+            + "\t".join(map(str, [max_set_a_id, max_set_b_id, max_set, atom_mapping]))
+        )
+
+        return atom_mapping
+
+    @staticmethod
+    def _get_connected_atom_subsets(
+        mol: Chem.Mol, to_be_searched: List[int]
+    ) -> List[Set[int]]:
+        """
+        Get the connected sets of all to_be_searched atom indices in mol. Connected means the atoms in a resulting connected set are connected by covalent bonds.
+
+        Parameters
+        ----------
+        mol : Chem.Mol
+            molecule graph containing the bond information
+        to_be_searched : List[int]
+            atom indices, that shall be grouped by connections.
+
+        Returns
+        -------
+        List[Set[int]]
+            return list of connected sets from the to_be_searched atom index list found in mol.
+        """
+        # Get bonded atoms sets
+        bonded_atom_sets = []
+        for aid in to_be_searched:
+            a = mol.GetAtomWithIdx(int(aid))
+            bond_atoms = [b.GetOtherAtomIdx(aid) for b in a.GetBonds()]
+            connected_atoms = set([aid] + bond_atoms)
+
+            # filter to not connect non mapped atoms
+            filtered_connected_atoms = set(
+                filter(lambda x: x in to_be_searched, connected_atoms)
+            )
+
+            # NO mapped atom connected?
+            if len(filtered_connected_atoms) == 1:
+                continue
+            else:
+                bonded_atom_sets.append(filtered_connected_atoms)
+        bonded_atom_sets = list(sorted(bonded_atom_sets))
+
+        log.debug("Bonded atom Sets: " + str(bonded_atom_sets))
+
+        # add new set or merge with existing set
+        atom_mappings = {i: a for i, a in enumerate(to_be_searched)}
+        r_atom_mappings = {a: i for i, a in enumerate(to_be_searched)}
+        max_n = len(to_be_searched)
+
+        connection_matrix = np.zeros(shape=(max_n, max_n))
+        for set_i in bonded_atom_sets:
+            for ai in set_i:
+                for aj in set_i:
+                    connection_matrix[r_atom_mappings[ai]][r_atom_mappings[aj]] = 1
+
+        log.debug("Adjacency Matrix: " + str(connection_matrix))
+
+        # get connected components
+        matrix = csr_matrix(connection_matrix)
+        n_components, labels = connected_components(csgraph=matrix, directed=False)
+
+        log.debug("Connected Components: " + str(n_components) + "\t" + str(labels))
+
+        # Translate back
+        merged_connnected_atom_sets = []
+        labels_sizes = [
+            label
+            for label, _ in sorted(
+                np.vstack(np.unique(labels, return_counts=True)).T,
+                key=lambda x: x[1],
+                reverse=True,
+            )
+        ]
+        for selected_label in labels_sizes:
+            connected_atoms_ids = list(
+                sorted(
+                    [
+                        atom_mappings[i]
+                        for i, label in enumerate(labels)
+                        if label == selected_label
+                    ]
+                )
+            )
+            merged_connnected_atom_sets.append(connected_atoms_ids)
+
+        log.debug("Merged Sets:" + str(merged_connnected_atom_sets))
+
+        return merged_connnected_atom_sets
+
+    @staticmethod
+    def _get_maximal_mapping_set_overlap(
+        sets_a: Iterable[Set], sets_b: Iterable[Set], mapping: Dict[int, int]
+    ) -> Tuple[Set, Set]:
+        """
+        get the largest set overlaps in the mapping of set_a and set_b.
+
+        Parameters
+        ----------
+        sets_a : Iterable[Set]
+            connected sets resulting from the mapping in state A
+        sets_b : Iterable[Set]
+            connected sets resulting from the mapping in state B
+        mapping : Dict[int, int]
+            proposed atom mapping from state A to state B
+
+        Returns
+        -------
+        Tuple[Set, Set]
+            returns the found maximal and maximal overlapping sets of a and the set of b
+        """
+        # Calculate overlaps
+
+        log.debug("Input: " + str(sets_a) + " " + str(sets_b) + " " + str(mapping))
+
+        max_set_combi = {}
+        for ida, set_a in enumerate(sets_a):
+            mapped_set_a = {mapping[a] for a in set_a}
+            for idb, set_b in enumerate(sets_b):
+                set_intersection_size = len(mapped_set_a.intersection(set_b))
+                if set_intersection_size:
+                    max_set_combi[(ida, idb)] = {
+                        "overlap_count": set_intersection_size,
+                        "set_a_size": len(set_a),
+                        "set_b_size": len(set_b),
+                    }
+
+        # sort overlap by size
+        overlap_sorted_sets = OrderedDict(
+            sorted(
+                max_set_combi.items(),
+                key=lambda x: x[1]["overlap_count"],
+                reverse=False,
+            )
+        )
+
+        log.debug("Set overlap properties" + str(overlap_sorted_sets))
+
+        max_overlap_set_a_id, max_overlap_set_b_id = overlap_sorted_sets.popitem()
+        return max_overlap_set_a_id, max_overlap_set_b_id
+
+    @staticmethod
+    def _filter_mapping_for_set_overlap(
+        set_a: Set[int], set_b: Set[int], mapping: Dict[int, int]
+    ) -> Dict[int, int]:
+        """
+        This filter reduces the mapping dict to only in the sets contained atom IDs
+
+        Parameters
+        ----------
+        set_a : Set[int]
+            this set contains the allowed keys
+        set_b : Set[int]
+            this set contains the allowed values
+        mapping : Dict[int, int]
+            this mapping is to be filtered by the set values.
+
+        Returns
+        -------
+        Dict[int, int]
+            filtered mapping
+
+        """
+        filtered_mapping = {}
+        for atom_a, atom_b in mapping.items():
+            if atom_a in set_a and atom_b in set_b:
+                filtered_mapping[atom_a] = atom_b
+        return filtered_mapping
+
+
+    """
+        Utils
+    """
+
+    @staticmethod
+    def _get_full_distance_matrix(
+        atomA_pos: np.array,
+        atomB_pos: np.array,
+        metric: Callable[
+            [Union[float, Iterable], Union[float, Iterable]], Union[float, Iterable]
+        ] = vector_eucledean_dist,
+    ) -> np.array:
+        """
+            calculates a full distance matrix between the two given input position matrixes.
+
+
+        Parameters
+        ----------
+        atomA_pos : np.array
+            position matrix A
+        atomB_pos : np.array
+            position matrix B
+        metric : Callable[[Union[float, Iterable], Union[float, Iterable]], Union[float, Iterable]], optional
+            the applied metric to calculate the distance matrix. default metric: eucledean distance.
+
+        Returns
+        -------
+        np.array
+            returns a distance matrix.
+
+        """
+        distance_matrix = []
+        for atomPosA in atomA_pos:
+            atomPos_distances = metric(atomPosA, atomB_pos)
+            distance_matrix.append(atomPos_distances)
+        distance_matrix = np.array(distance_matrix)
+        return distance_matrix
+
+    @staticmethod
+    def _mask_atoms(
+        mol, mol_pos, map_hydrogens: bool = False, masked_atoms=[]
+    ) -> Tuple[Dict, List]:
+        """
+        Mask atoms
+
+        Parameters
+        ----------
+        mol
+        mol_pos
+        map_hydrogens
+        masked_atoms
+
+        Returns
+        -------
+
+        """
+        pos = []
+        masked_atomMapping = {}
+        for atom in mol.GetAtoms():
+            atom_id = atom.GetIdx()
+            if (
+                map_hydrogens or atom.GetSymbol() != "H"
+            ) and atom_id not in masked_atoms:
+                masked_atomMapping[len(masked_atomMapping)] = atom_id
+                pos.append(mol_pos[atom_id])
+        pos = np.array(pos)
+
+        return masked_atomMapping, pos
+
+    def _minimalSpanningTree_map(
+        self, distance_matrix: np.array, max_dist: float
+    ) -> Dict[int, int]:
+        """
+        This function is a numpy graph based implementation to build up an Atom Mapping purely on 3D criteria.
+
+        Parameters
+        ----------
+        distance_matrix: np.array
+            distances of atoms to each other.
+        max_dist: float
+            maximal distance of a atoms in a mapping.
+
+        Returns
+        -------
+        Dict[int, int]
+            mapping of atoms.
+        """
+
+        # distance matrix:  - full graph
+        log.debug("Got Distance Matrix: \n" + str(distance_matrix))
+        edges = []
+        for i, distance_row in enumerate(distance_matrix):
+            for j, dist in enumerate(distance_row):
+                edges.append([float(dist), int(i), int(j)])
+
+        edges = np.array(edges)
+        log.debug("Edges: \n" + str(edges))
+
+        # priority queue based on edge weight
+        sorted_edges = edges[edges[:, 0].argsort()]
+        log.debug("Sorted Edges: \n" + str(sorted_edges))
+
+        # MST like algorithm
+        mapping = {}
+        for w, x, y in sorted_edges:
+            if w >= max_dist:  # filter for max dist
+                break
+            else:
+                if x not in mapping.keys() and y not in mapping.values():
+                    mapping[int(x)] = int(y)
+
+        return mapping
+
+    @staticmethod
+    def _linearSumAlgorithm_map(
+        distance_matrix: np.array, max_dist: float
+    ) -> Dict[int, int]:
+        """
+        This function is a LSA based implementation to build up an Atom Mapping purely on 3D criteria.
+
+        Parameters
+        ----------
+        distance_matrix: np.array
+            distances of atoms to each other.
+        max_dist: float
+            maximal distance of a atoms in a mapping.
+
+        Returns
+        -------
+        Dict[int, int]
+            mapping of atoms.
+        """
+        row_ind, col_ind = linear_sum_assignment(distance_matrix)
+        raw_mapping = list(zip(map(int, row_ind), map(int, col_ind)))
+        # filter for mask value
+        mapping = dict(filter(lambda x: distance_matrix[x] < max_dist, raw_mapping))
+
+        return mapping
+
+    def _additional_filter_rules(
+        self, molA: Chem.Mol, molB: Chem.Mol, mapping: dict[int, int]
+    ) -> Dict[int, int]:
+        """
+        apply additional filter rules to the given mapping.
+
+        Parameters
+        ----------
+        molA : Chem.Mol
+            mol, with atoms contained in mapping keys.
+        molB : Chem.Mol
+            mol, with atoms contained in mapping values.
+        mapping : Dict[int, int]
+            mapping to be filtered
+
+        Returns
+        -------
+        Dict[int, int]
+            filtered mapping
+        """
+        filtered_mapping = copy.deepcopy(mapping)
+        for filter_rule in self._filter_funcs:
+            filtered_mapping = filter_rule(molA, molB, filtered_mapping)
+        return filtered_mapping
+
+    def _calculate_mapping(
+        self,
+        molA: Chem.Mol,
+        molB: Chem.Mol,
+        max_d: float = 0.95,
+        masked_atoms_molA: Optional[list[int]] = None,
+        masked_atoms_molB: Optional[list[int]] = None,
+        pre_mapped_atoms: Optional[dict[int, int]] = None,
+        map_hydrogens: bool = True,
+    ) -> dict[int, int]:
+        """
+            find a mapping between two molecules based on 3D coordinates. This is a helper function for the suggest mapping functions.
+
+        Parameters
+        ----------
+        molA : Chem.Mol
+            rdkit Molecule A
+        molB : Chem.Mol
+            rdkit Molecule B
+        max_d : float, optional
+            maximal allowed distance for atoms to be mapped, by default 0.95
+        masked_atoms_molA : list, optional
+            remove categorical atoms by index of MolA from the mapping, by default []
+        masked_atoms_molB : list, optional
+            remove categorical atoms by index of MolB from the mapping, by default []
+        pre_mapped_atoms : dict, optional
+            pre_mapped atoms, that need to be part of the mapping, by default {}
+        map_hydrogens : bool, optional
+            if True map hydrogens as well, will hapen after heavy atom mapping, by default True
+
+        Returns
+        -------
+        AtomMapping
+            _description_
+        """
+        if masked_atoms_molA is None:
+            masked_atoms_molA = []
+        if masked_atoms_molB is None:
+            masked_atoms_molB = []
+        if pre_mapped_atoms is None:
+            pre_mapped_atoms = dict()
+
+        molA_pos = molA.GetConformer().GetPositions()
+        molB_pos = molB.GetConformer().GetPositions()
+        masked_atoms_molA = copy.deepcopy(masked_atoms_molA)
+        masked_atoms_molB = copy.deepcopy(masked_atoms_molB)
+        pre_mapped_atoms = copy.deepcopy(pre_mapped_atoms)
+
+        if len(pre_mapped_atoms) > 0:
+            masked_atoms_molA.extend(pre_mapped_atoms.keys())
+            masked_atoms_molB.extend(pre_mapped_atoms.values())
+
+        log.debug("Positions lengths: " + str(len(molA_pos)) + " " + str(len(molB_pos)))
+        log.debug("Positions: \n" + "\n\t".join(map(str, [molA_pos, molB_pos])))
+        log.debug("masked_atoms_molA: " + str(masked_atoms_molA))
+        log.debug("masked_atoms_molB: " + str(masked_atoms_molB))
+        log.debug("pre_mapped_atoms: " + str(pre_mapped_atoms))
+        log.debug("map_hydrogens: " + str(map_hydrogens))
+
+        log.info("Masking Atoms")
+
+        molA_masked_atomMapping, molA_pos = self._mask_atoms(
+            mol=molA,
+            mol_pos=molA_pos,
+            masked_atoms=masked_atoms_molA,
+            map_hydrogens=map_hydrogens,
+        )
+        molB_masked_atomMapping, molB_pos = self._mask_atoms(
+            mol=molB,
+            mol_pos=molB_pos,
+            masked_atoms=masked_atoms_molB,
+            map_hydrogens=map_hydrogens,
+        )
+
+        log.debug(
+            "Remove Masked Atoms: \n"
+            + "\n\t".join(map(str, [molA_masked_atomMapping, molB_masked_atomMapping]))
+            + "\n"
+            + "\n\t".join(map(str, [molA_pos, molB_pos]))
+        )
+        log.debug(
+            "filtered Masked Positions lengths: "
+            + "\t".join(map(str, [len(molA_pos), len(molB_pos)]))
+        )
+
+        if len(molA_pos) == 0 or len(molB_pos) == 0:  # TODO: check if this is correct
+            if(len(pre_mapped_atoms)==0): log.warning("no mappable Atoms were found!")
+            return pre_mapped_atoms
+
+        # Calculate mapping
+        log.info("Build Distance Matrix")
+        # distance matrix:  - full graph
+        distance_matrix = self._get_full_distance_matrix(molA_pos, molB_pos)
+        log.debug("Distance Matrix: \n" + str(distance_matrix))
+
+        # Mask distance matrix with max_d
+        # np.inf is considererd as not possible in lsa implementation - therefore use a high value
+        self.mask_dist_val = max_d * 10**6
+        masked_dmatrix = np.array(
+            np.ma.where(distance_matrix < max_d, distance_matrix, self.mask_dist_val)
+        )
+        log.debug(
+            "masked Distance Matrix: " + str(max_d) + "\n\t" + str(masked_dmatrix)
+        )
+
+        # solve atom mappings
+        log.info("Calculate Mapping")
+        mapping = self.mapping_algorithm(
+            distance_matrix=masked_dmatrix, max_dist=self.mask_dist_val
+        )
+        log.debug("Raw Mapping: " + str(mapping))
+
+        if len(mapping) == 0:  # TODO: check if this is correct
+            if(len(pre_mapped_atoms)==0): log.warning("no mapping could be found!")
+            return pre_mapped_atoms
+
+        # reverse any prior masking:
+        mapping = {
+            molA_masked_atomMapping[k]: molB_masked_atomMapping[v]
+            for k, v in mapping.items()
+        }
+
+        # filter mapping for rules:
+        if self._filter_funcs is not None:
+            mapping = self._additional_filter_rules(molA, molB, mapping)
+
+        if len(pre_mapped_atoms) > 0:
+            mapping.update(pre_mapped_atoms)
+        log.debug("reverse Masking Mapping: " + str(mapping))
+
+        if len(mapping) == 0:
+            if(len(pre_mapped_atoms)==0): log.warning("no mapping could be found, after applying filters!")
+            return pre_mapped_atoms
+
+        # Reduce mapping to maximally overlapping two connected sets
+        log.info("Find Maximal overlapping connected sets of mapped atoms")
+        mapping = self._filter_mapping_for_max_overlapping_connected_atom_set(
+            moleculeA=molA, moleculeB=molB, atom_mapping=mapping
+        )
+        log.debug("Set overlap Mapping: " + str(mapping))
+
+        return mapping
+
+    """
+        Mapping functions
+    """
+
+    def suggest_mapping_from_rdmols(
+        self,
+        molA: Chem.Mol,
+        molB: Chem.Mol,
+        masked_atoms_molA: Optional[list] = None,
+        masked_atoms_molB: Optional[list] = None,
+        pre_mapped_atoms: Optional[dict] = None,
+    ) -> dict[int, int]:
+        """
+        The function effectivly maps the two molecules on to each other and
+        applies the given settings by the obj.
+
+        Parameters
+        ----------
+        molA, molB : rdkit.Chem.Mol
+            two rdkit molecules that should be mapped onto each other
+        masked_atoms_molA : list, optional
+            remove categorical atoms by index of MolA from the mapping, by default []
+        masked_atoms_molB : list, optional
+            remove categorical atoms by index of MolB from the mapping, by default []
+        pre_mapped_atoms : dict, optional
+            pre_mapped atoms, that need to be part of the mapping, by default {}
+        """
+        if masked_atoms_molA is None:
+            masked_atoms_molA = []
+        if masked_atoms_molB is None:
+            masked_atoms_molB = []
+        if pre_mapped_atoms is None:
+            pre_mapped_atoms = {}
+
+        molA = Chem.Mol(molA)
+        molB = Chem.Mol(molB)
+        masked_atoms_molA = copy.deepcopy(masked_atoms_molA)
+        masked_atoms_molB = copy.deepcopy(masked_atoms_molB)
+        pre_mapped_atoms = copy.deepcopy(pre_mapped_atoms)
+
+        log.info("#################################")
+        log.info("Map Heavy Atoms ")
+        log.info("#################################")
+
+        mapping = self._calculate_mapping(
+            molA,
+            molB,
+            max_d=self.atom_max_distance,
+            masked_atoms_molA=masked_atoms_molA,
+            masked_atoms_molB=masked_atoms_molB,
+            pre_mapped_atoms=pre_mapped_atoms,
+            map_hydrogens=False,
+        )
+
+        if self.atom_map_hydrogens:
+            log.info("#################################")
+            log.info("Map Hydrogen Atoms: ")
+            log.info("#################################")
+
+            pre_mapped_atoms.update(mapping)
+
+            mapping = self._calculate_mapping(
+                molA,
+                molB,
+                max_d=self.atom_max_distance,
+                masked_atoms_molA=masked_atoms_molA,
+                masked_atoms_molB=masked_atoms_molB,
+                pre_mapped_atoms=pre_mapped_atoms,
+                map_hydrogens=self.atom_map_hydrogens,
+            )
+
+        return mapping
+
+    def suggest_mappings(
+        self, A: SmallMoleculeComponent, B: SmallMoleculeComponent
+    ) -> Iterator[AtomMapping]:
+        """
+        return a generator for atom mappings.
+
+        Parameters
+        ----------
+        A : SmallMoleculeComponent
+            molecule A to be mapped.
+        B : SmallMoleculeComponent
+            molecule B to be mapped.
+
+        Returns
+        -------
+        Iterator[AtomMapping]
+            returns an interator of possible atom mappings.
+        """
+        yield LigandAtomMapping(
+            A, B, self.suggest_mapping_from_rdmols(molA=A.to_rdkit(), molB=B.to_rdkit())
+        )
```

### Comparing `kartograf-0.5.1/src/kartograf/filters/ring_changes.py` & `kartograf-0.5.2/src/kartograf/filters/ring_changes.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import logging
-from rdkit import Chem
-
-logger = logging.getLogger(__name__)
-
-
-def filter_ringsize_changes(molA: Chem.Mol, molB: Chem.Mol,
-                            mapping: dict[int, int]) -> dict[int, int]:
-    """Prevents mutating the size of rings in the mapping"""
-    riA = molA.GetRingInfo()
-    riB = molB.GetRingInfo()
-
-    filtered_mapping = {}
-
-    for i, j in mapping.items():
-        at_i = molA.GetAtomWithIdx(i)
-        at_j = molB.GetAtomWithIdx(j)
-
-        if not (at_i.IsInRing() and at_j.IsInRing()):
-            # only applicable for atoms in rings
-            # other cases are handled with other filters
-            filtered_mapping[i] = j
-            continue
-
-        # AtomRingSizes gives as tuple of ring sizes that this atom is part of
-        rs_i = set(riA.AtomRingSizes(i))
-        rs_j = set(riB.AtomRingSizes(j))
-
-        # if there's any intersection in ring size, we're ok
-        if not (rs_i & rs_j):
-            # e.g. {5} and {6} we've mutated a ring, don't include
-            continue
-        filtered_mapping[i] = j
-
-    return filtered_mapping
-
-
-def filter_ringbreak_changes(molA: Chem.Mol, molB: Chem.Mol,
-                             mapping: dict[int, int]) -> dict[int, int]:
-    """Prevent any ring cleaving transformations in the mapping
-
-    This filter prevents any non-ring atom turning into a ring atom (or
-    vice versa)
-    """
-    filtered_mapping = {}
-
-    for i, j in mapping.items():
-        at_i = molA.GetAtomWithIdx(i)
-        at_j = molB.GetAtomWithIdx(j)
-        if at_i.IsInRing() ^ at_j.IsInRing():
-            continue
-        filtered_mapping[i] = j
-
-    return filtered_mapping
-
-
-def filter_whole_rings_only(molA: Chem.Mol, molB: Chem.Mol,
-                            mapping: dict[int, int]) -> dict[int, int]:
-    """Ensure that any mapped rings are wholly mapped"""
-    proposed_mapping = {**mapping}
-
-    for mol in [molA, molB]:  # loop over A->B and B->A directions
-        ri = mol.GetRingInfo().AtomRings()  # gives list of tuple of atom indices
-        ok: dict[int, bool] = {}  # if a ring atom, is this ok to keep?
-        for ring in ri:
-            # for each ring, atoms are ok if all the atoms of this ring are in
-            # the mapping
-            all_in_ring = all(atom in proposed_mapping for atom in ring)
-            for atom in ring:
-                ok[atom] = all_in_ring
-
-        filtered_mapping = {}
-        for i, j in proposed_mapping.items():
-            if ok.get(i, True):  # if not present, isn't in ring so keep
-                filtered_mapping[i] = j
-
-        # reverse the mapping to check B->A (then reverse again)
-        proposed_mapping = {v: k for k, v in filtered_mapping.items()}
-
-    return proposed_mapping
+import logging
+from rdkit import Chem
+
+logger = logging.getLogger(__name__)
+
+
+def filter_ringsize_changes(molA: Chem.Mol, molB: Chem.Mol,
+                            mapping: dict[int, int]) -> dict[int, int]:
+    """Prevents mutating the size of rings in the mapping"""
+    riA = molA.GetRingInfo()
+    riB = molB.GetRingInfo()
+
+    filtered_mapping = {}
+
+    for i, j in mapping.items():
+        at_i = molA.GetAtomWithIdx(i)
+        at_j = molB.GetAtomWithIdx(j)
+
+        if not (at_i.IsInRing() and at_j.IsInRing()):
+            # only applicable for atoms in rings
+            # other cases are handled with other filters
+            filtered_mapping[i] = j
+            continue
+
+        # AtomRingSizes gives as tuple of ring sizes that this atom is part of
+        rs_i = set(riA.AtomRingSizes(i))
+        rs_j = set(riB.AtomRingSizes(j))
+
+        # if there's any intersection in ring size, we're ok
+        if not (rs_i & rs_j):
+            # e.g. {5} and {6} we've mutated a ring, don't include
+            continue
+        filtered_mapping[i] = j
+
+    return filtered_mapping
+
+
+def filter_ringbreak_changes(molA: Chem.Mol, molB: Chem.Mol,
+                             mapping: dict[int, int]) -> dict[int, int]:
+    """Prevent any ring cleaving transformations in the mapping
+
+    This filter prevents any non-ring atom turning into a ring atom (or
+    vice versa)
+    """
+    filtered_mapping = {}
+
+    for i, j in mapping.items():
+        at_i = molA.GetAtomWithIdx(i)
+        at_j = molB.GetAtomWithIdx(j)
+        if at_i.IsInRing() ^ at_j.IsInRing():
+            continue
+        filtered_mapping[i] = j
+
+    return filtered_mapping
+
+
+def filter_whole_rings_only(molA: Chem.Mol, molB: Chem.Mol,
+                            mapping: dict[int, int]) -> dict[int, int]:
+    """Ensure that any mapped rings are wholly mapped"""
+    proposed_mapping = {**mapping}
+
+    for mol in [molA, molB]:  # loop over A->B and B->A directions
+        ri = mol.GetRingInfo().AtomRings()  # gives list of tuple of atom indices
+        ok: dict[int, bool] = {}  # if a ring atom, is this ok to keep?
+        for ring in ri:
+            # for each ring, atoms are ok if all the atoms of this ring are in
+            # the mapping
+            all_in_ring = all(atom in proposed_mapping for atom in ring)
+            for atom in ring:
+                ok[atom] = all_in_ring
+
+        filtered_mapping = {}
+        for i, j in proposed_mapping.items():
+            if ok.get(i, True):  # if not present, isn't in ring so keep
+                filtered_mapping[i] = j
+
+        # reverse the mapping to check B->A (then reverse again)
+        proposed_mapping = {v: k for k, v in filtered_mapping.items()}
+
+    return proposed_mapping
```

### Comparing `kartograf-0.5.1/src/kartograf/tests/conf.py` & `kartograf-0.5.2/src/kartograf/tests/conf.py`

 * *Files identical despite different names*

### Comparing `kartograf-0.5.1/src/kartograf/tests/test_atom_align.py` & `kartograf-0.5.2/src/kartograf/tests/test_atom_align.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# This code is part of OpenFE and is licensed under the MIT license.
-# For details, see https://github.com/OpenFreeEnergy/kartograf
-
-import pytest
-
-from kartograf.atom_align import align_mol_sceletons, align_mol_shape
-
-from .conf import stereco_chem_molecules
-
-
-def test_stereo_align_mcs(stereco_chem_molecules):
-    """
-    Currently a smoke test
-    """
-    molA, molB = stereco_chem_molecules
-    aligned_molA = align_mol_sceletons(molA, molB)
-
-def test_stereo_align_shape(stereco_chem_molecules):
-    """
-    Currently a smoke test
-    """
-    molA, molB = stereco_chem_molecules
+# This code is part of OpenFE and is licensed under the MIT license.
+# For details, see https://github.com/OpenFreeEnergy/kartograf
+
+import pytest
+
+from kartograf.atom_align import align_mol_sceletons, align_mol_shape
+
+from .conf import stereco_chem_molecules
+
+
+def test_stereo_align_mcs(stereco_chem_molecules):
+    """
+    Currently a smoke test
+    """
+    molA, molB = stereco_chem_molecules
+    aligned_molA = align_mol_sceletons(molA, molB)
+
+def test_stereo_align_shape(stereco_chem_molecules):
+    """
+    Currently a smoke test
+    """
+    molA, molB = stereco_chem_molecules
     aligned_molA = align_mol_shape(molA, molB)
```

### Comparing `kartograf-0.5.1/src/kartograf/tests/test_atom_mapper.py` & `kartograf-0.5.2/src/kartograf/tests/test_atom_mapper.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-# This code is part of OpenFE and is licensed under the MIT license.
-# For details, see https://github.com/OpenFreeEnergy/kartograf
-
-import pytest
-from kartograf import KartografAtomMapper
-from kartograf.atom_mapper import filter_atoms_h_only_h_mapped
-
-from .conf import (
-    naphtalene_benzene_molecules,
-    naphtalene_benzene_mapping,
-    stereco_chem_molecules,
-    stereo_chem_mapping,
-)
-from copy import deepcopy
-
-def check_mapping_vs_expected(mapping, expected_mapping):
-    assert len(expected_mapping) == len(mapping.componentA_to_componentB)
-
-    diff = []
-    for exp_k, exp_v in expected_mapping.items():
-        if exp_k not in mapping.componentA_to_componentB:
-            diff.append((exp_k, exp_v, None, "missing mapping for atom"))
-        elif exp_v != mapping.componentA_to_componentB[exp_k]:
-            diff.append(
-                (
-                    exp_k,
-                    exp_v,
-                    mapping.componentA_to_componentB[exp_k],
-                    "-",
-                    "differently mapped atoms",
-                )
-            )
-
-    if len(diff) > 0:
-        print("Differences: expected key, expected value, actual value")
-        print("\n".join(map(lambda x: "\t".join(map(str, x)), diff)))
-        raise ValueError("mapping did not match expected mapping!")
-
-
-def test_mapping_naphtalene_benzene(
-    naphtalene_benzene_molecules, naphtalene_benzene_mapping
-):
-    """
-    Test mapping of naphtalene to benzene.
-    """
-    expected_mapping = naphtalene_benzene_mapping.componentA_to_componentB
-    geom_mapper = KartografAtomMapper(
-        atom_max_distance=0.95,
-        atom_map_hydrogens=True,
-        map_hydrogens_on_hydrogens_only=False,
-    )
-
-    geom_mapping = next(
-        geom_mapper.suggest_mappings(
-            naphtalene_benzene_molecules[0],
-            naphtalene_benzene_molecules[1],
-        )
-    )
-
-    check_mapping_vs_expected(geom_mapping, expected_mapping)
-
-
-def test_mapping_naphtalene_benzene_noHs(naphtalene_benzene_molecules):
-    """
-    Test mapping of naphtalene to benzene without H-atoms.
-    """
-    expected_mapping = {10: 7, 11: 8, 12: 9, 13: 10, 0: 0, 1: 1, 2: 2, 3: 3, 4: 4, 5: 5}
-    geom_mapper = KartografAtomMapper(
-        atom_max_distance=0.95,
-        atom_map_hydrogens=True,
-        map_hydrogens_on_hydrogens_only=True,
-    )
-
-    geom_mapping = next(
-        geom_mapper.suggest_mappings(
-            naphtalene_benzene_molecules[0],
-            naphtalene_benzene_molecules[1],
-        )
-    )
-
-    check_mapping_vs_expected(geom_mapping, expected_mapping)
-
-
-def test_mapping_naphtalene_benzene_noHs_add_filter(naphtalene_benzene_molecules):
-    """
-    Test mapping of naphtalene to benzene without H-atoms added as additional filter.
-    """
-    expected_mapping = {10: 7, 11: 8, 12: 9, 13: 10, 0: 0, 1: 1, 2: 2, 3: 3, 4: 4, 5: 5}
-    geom_mapper = KartografAtomMapper(
-        atom_max_distance=0.95,
-        atom_map_hydrogens=True,
-        map_hydrogens_on_hydrogens_only=False,
-        additional_mapping_filter_functions=[filter_atoms_h_only_h_mapped],
-    )
-
-    geom_mapping = next(
-        geom_mapper.suggest_mappings(
-            naphtalene_benzene_molecules[0],
-            naphtalene_benzene_molecules[1],
-        )
-    )
-
-    check_mapping_vs_expected(geom_mapping, expected_mapping)
-
-
-def test_stereo_mapping(stereco_chem_molecules, stereo_chem_mapping):
-    """
-    Test weird Stereochemistry mapping.
-    """
-    expected_mapping = stereo_chem_mapping.componentA_to_componentB
-    geom_mapper = KartografAtomMapper(
-        atom_max_distance=0.95, atom_map_hydrogens=True
-    )  # mapping_algorithm.minimal_spanning_tree
-    geom_mapping = next(
-        geom_mapper.suggest_mappings(
-            stereco_chem_molecules[0],
-            stereco_chem_molecules[1],
-        )
-    )
-
-    check_mapping_vs_expected(geom_mapping, expected_mapping)
-
-
-def test_to_From_dict():
-    mapper = KartografAtomMapper()
-    d1 = mapper._to_dict()
-    mapper2 = KartografAtomMapper._from_dict(d1)
-    d2 = mapper2._to_dict()
-
-    for key, val1 in d1.items():
-        val2 = d2[key]
-
-        if(val1 != val2):
-            raise ValueError("they need to be identical.")
-
-    mapper2.atom_max_distance = 10
-    d3 = mapper2._to_dict()
-    print(d3)
-    for key, val1 in d1.items():
-        val2 = d3[key]
-
-        if(val1 != val2 and key != "atom_max_distance"):
-            raise ValueError("they need to be identical.")
-        if(key == "atom_max_distance" and val1 == val2 ):
-            raise ValueError("they must not be identical.")
-
-
-def test_filter_property():
-    mapper = KartografAtomMapper(map_hydrogens_on_hydrogens_only=False)
-    first_filters = deepcopy(mapper._filter_funcs)
-
-    mapper.map_hydrogens_on_hydrogens_only = True
-    second_filters = deepcopy(mapper._filter_funcs)
-
-    mapper.map_hydrogens_on_hydrogens_only = False
-    third_filters = deepcopy(mapper._filter_funcs)
-
-    assert len(first_filters) == len(third_filters)
-    assert len(first_filters) == len(second_filters)-1
-
-    assert filter_atoms_h_only_h_mapped in second_filters
-    assert filter_atoms_h_only_h_mapped not in first_filters
-    assert filter_atoms_h_only_h_mapped not in first_filters
-
+# This code is part of OpenFE and is licensed under the MIT license.
+# For details, see https://github.com/OpenFreeEnergy/kartograf
+
+import pytest
+from kartograf import KartografAtomMapper
+from kartograf.atom_mapper import filter_atoms_h_only_h_mapped
+
+from .conf import (
+    naphtalene_benzene_molecules,
+    naphtalene_benzene_mapping,
+    stereco_chem_molecules,
+    stereo_chem_mapping,
+)
+from copy import deepcopy
+
+def check_mapping_vs_expected(mapping, expected_mapping):
+    assert len(expected_mapping) == len(mapping.componentA_to_componentB)
+
+    diff = []
+    for exp_k, exp_v in expected_mapping.items():
+        if exp_k not in mapping.componentA_to_componentB:
+            diff.append((exp_k, exp_v, None, "missing mapping for atom"))
+        elif exp_v != mapping.componentA_to_componentB[exp_k]:
+            diff.append(
+                (
+                    exp_k,
+                    exp_v,
+                    mapping.componentA_to_componentB[exp_k],
+                    "-",
+                    "differently mapped atoms",
+                )
+            )
+
+    if len(diff) > 0:
+        print("Differences: expected key, expected value, actual value")
+        print("\n".join(map(lambda x: "\t".join(map(str, x)), diff)))
+        raise ValueError("mapping did not match expected mapping!")
+
+
+def test_mapping_naphtalene_benzene(
+    naphtalene_benzene_molecules, naphtalene_benzene_mapping
+):
+    """
+    Test mapping of naphtalene to benzene.
+    """
+    expected_mapping = naphtalene_benzene_mapping.componentA_to_componentB
+    geom_mapper = KartografAtomMapper(
+        atom_max_distance=0.95,
+        atom_map_hydrogens=True,
+        map_hydrogens_on_hydrogens_only=False,
+    )
+
+    geom_mapping = next(
+        geom_mapper.suggest_mappings(
+            naphtalene_benzene_molecules[0],
+            naphtalene_benzene_molecules[1],
+        )
+    )
+
+    check_mapping_vs_expected(geom_mapping, expected_mapping)
+
+
+def test_mapping_naphtalene_benzene_noHs(naphtalene_benzene_molecules):
+    """
+    Test mapping of naphtalene to benzene without H-atoms.
+    """
+    expected_mapping = {10: 7, 11: 8, 12: 9, 13: 10, 0: 0, 1: 1, 2: 2, 3: 3, 4: 4, 5: 5}
+    geom_mapper = KartografAtomMapper(
+        atom_max_distance=0.95,
+        atom_map_hydrogens=True,
+        map_hydrogens_on_hydrogens_only=True,
+    )
+
+    geom_mapping = next(
+        geom_mapper.suggest_mappings(
+            naphtalene_benzene_molecules[0],
+            naphtalene_benzene_molecules[1],
+        )
+    )
+
+    check_mapping_vs_expected(geom_mapping, expected_mapping)
+
+
+def test_mapping_naphtalene_benzene_noHs_add_filter(naphtalene_benzene_molecules):
+    """
+    Test mapping of naphtalene to benzene without H-atoms added as additional filter.
+    """
+    expected_mapping = {10: 7, 11: 8, 12: 9, 13: 10, 0: 0, 1: 1, 2: 2, 3: 3, 4: 4, 5: 5}
+    geom_mapper = KartografAtomMapper(
+        atom_max_distance=0.95,
+        atom_map_hydrogens=True,
+        map_hydrogens_on_hydrogens_only=False,
+        additional_mapping_filter_functions=[filter_atoms_h_only_h_mapped],
+    )
+
+    geom_mapping = next(
+        geom_mapper.suggest_mappings(
+            naphtalene_benzene_molecules[0],
+            naphtalene_benzene_molecules[1],
+        )
+    )
+
+    check_mapping_vs_expected(geom_mapping, expected_mapping)
+
+
+def test_stereo_mapping(stereco_chem_molecules, stereo_chem_mapping):
+    """
+    Test weird Stereochemistry mapping.
+    """
+    expected_mapping = stereo_chem_mapping.componentA_to_componentB
+    geom_mapper = KartografAtomMapper(
+        atom_max_distance=0.95, atom_map_hydrogens=True
+    )  # mapping_algorithm.minimal_spanning_tree
+    geom_mapping = next(
+        geom_mapper.suggest_mappings(
+            stereco_chem_molecules[0],
+            stereco_chem_molecules[1],
+        )
+    )
+
+    check_mapping_vs_expected(geom_mapping, expected_mapping)
+
+
+def test_to_From_dict():
+    mapper = KartografAtomMapper()
+    d1 = mapper._to_dict()
+    mapper2 = KartografAtomMapper._from_dict(d1)
+    d2 = mapper2._to_dict()
+
+    for key, val1 in d1.items():
+        val2 = d2[key]
+
+        if(val1 != val2):
+            raise ValueError("they need to be identical.")
+
+    mapper2.atom_max_distance = 10
+    d3 = mapper2._to_dict()
+    print(d3)
+    for key, val1 in d1.items():
+        val2 = d3[key]
+
+        if(val1 != val2 and key != "atom_max_distance"):
+            raise ValueError("they need to be identical.")
+        if(key == "atom_max_distance" and val1 == val2 ):
+            raise ValueError("they must not be identical.")
+
+
+def test_filter_property():
+    mapper = KartografAtomMapper(map_hydrogens_on_hydrogens_only=False)
+    first_filters = deepcopy(mapper._filter_funcs)
+
+    mapper.map_hydrogens_on_hydrogens_only = True
+    second_filters = deepcopy(mapper._filter_funcs)
+
+    mapper.map_hydrogens_on_hydrogens_only = False
+    third_filters = deepcopy(mapper._filter_funcs)
+
+    assert len(first_filters) == len(third_filters)
+    assert len(first_filters) == len(second_filters)-1
+
+    assert filter_atoms_h_only_h_mapped in second_filters
+    assert filter_atoms_h_only_h_mapped not in first_filters
+    assert filter_atoms_h_only_h_mapped not in first_filters
+
```

### Comparing `kartograf-0.5.1/src/kartograf/tests/test_atom_mapping_scorer.py` & `kartograf-0.5.2/src/kartograf/tests/test_atom_mapping_scorer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,99 +1,111 @@
-import pytest
-from kartograf.atom_mapping_scoring import (
-    MappingRMSDScorer,
-    _MappingShapeDistanceScorer,
-    MappingShapeMismatchScorer,
-    MappingShapeOverlapScorer,
-    MappingVolumeRatioScorer,
-    MappingRatioMappedAtomsScorer,
-    DefaultKartografScorer
-)
-
-from .conf import stereo_chem_mapping, benzene_benzene_mapping, benzene_benzene_empty_mapping
-
-
-def test_score_mappings_rmsd(stereo_chem_mapping):
-    """
-    Currently a smoke test
-    """
-    scorer = MappingRMSDScorer()
-    score = scorer.get_rmsd(stereo_chem_mapping)
-    print(score)
-
-
-def test_score_norm_mapping_rmsd(stereo_chem_mapping):
-    """
-    Currently a smoke test
-    """
-    scorer = MappingRMSDScorer()
-    score = scorer.get_rmsd_p(stereo_chem_mapping)
-    print(score)
-
-def test_score_mapping_volume_ratio(stereo_chem_mapping):
-    """
-    Currently a smoke test
-    """
-    scorer = MappingVolumeRatioScorer()
-    score = scorer(stereo_chem_mapping)
-    print(score)
-
-
-def test_score_shape_dist(stereo_chem_mapping):
-    """
-    Currently a smoke test
-    """
-    scorer = _MappingShapeDistanceScorer()
-    score = scorer(stereo_chem_mapping)
-    print(score)
-
-def test_score_shape_overlap(stereo_chem_mapping):
-    """
-    Currently a smoke test
-    """
-    scorer = MappingShapeOverlapScorer()
-    score = scorer(stereo_chem_mapping)
-    print(score)
-
-def test_score_shape_mismatch(stereo_chem_mapping):
-    """
-    Currently a smoke test
-    """
-    scorer = MappingShapeMismatchScorer()
-    score = scorer(stereo_chem_mapping)
-    print(score)
-
-
-@pytest.mark.parametrize("scorer_class", [ MappingRMSDScorer,
-    _MappingShapeDistanceScorer,
-    MappingShapeMismatchScorer,
-    MappingShapeOverlapScorer,
-    MappingVolumeRatioScorer,
-    MappingRatioMappedAtomsScorer,
-    DefaultKartografScorer])
-def test_scorer_identical_molecules(scorer_class, benzene_benzene_mapping):
-    """
-    Currently a smoke test
-    """
-    scorer = scorer_class()
-    score = scorer(benzene_benzene_mapping)
-
-    assert isinstance(score, float)
-    assert score == 0, "Score of identical Molecule should be 0"
-
-
-@pytest.mark.parametrize("scorer_class, exp", [(MappingRMSDScorer, 0),
-                                               (_MappingShapeDistanceScorer, 1),
-                                               (MappingShapeMismatchScorer,1),
-                                               (MappingShapeOverlapScorer, 1),
-                                               (MappingVolumeRatioScorer, 1),
-                                               (MappingRatioMappedAtomsScorer,1),
-                                               (DefaultKartografScorer,1)])
-def test_scorer_empty_mapping(scorer_class, exp:float, benzene_benzene_empty_mapping):
-    """
-    Currently a smoke test
-    """
-    scorer = scorer_class()
-    score = scorer(benzene_benzene_empty_mapping)
-
-    assert isinstance(score, float)
-    assert score == exp, "Score of non-Mapping should be "+str(exp)+" for "+str(scorer_class.__name__)+" but is: "+str(score)
+import pytest
+from kartograf.atom_mapping_scorer import DefaultKartografScorer
+from kartograf.mapping_metrics import (
+    MappingRMSDScorer,
+    MappingShapeMismatchScorer,
+    MappingShapeOverlapScorer,
+    MappingVolumeRatioScorer,
+    MappingRatioMappedAtomsScorer,
+
+)
+
+from kartograf.mapping_metrics.metric_shape_difference import _MappingShapeDistanceScorer
+from .conf import stereo_chem_mapping, benzene_benzene_mapping, benzene_benzene_empty_mapping
+
+
+def test_score_mappings_rmsd(stereo_chem_mapping):
+    """
+    Currently a smoke test
+    """
+    scorer = MappingRMSDScorer()
+    score = scorer.get_rmsd(stereo_chem_mapping)
+    print(score)
+
+
+def test_score_norm_mapping_rmsd(stereo_chem_mapping):
+    """
+    Currently a smoke test
+    """
+    scorer = MappingRMSDScorer()
+    score = scorer.get_rmsd_p(stereo_chem_mapping)
+    print(score)
+
+def test_score_mapping_volume_ratio(stereo_chem_mapping):
+    """
+    Currently a smoke test
+    """
+    scorer = MappingVolumeRatioScorer()
+    score = scorer(stereo_chem_mapping)
+    print(score)
+
+
+def test_score_shape_dist(stereo_chem_mapping):
+    """
+    Currently a smoke test
+    """
+    scorer = _MappingShapeDistanceScorer()
+    score = scorer(stereo_chem_mapping)
+    print(score)
+
+def test_score_shape_overlap(stereo_chem_mapping):
+    """
+    Currently a smoke test
+    """
+    scorer = MappingShapeOverlapScorer()
+    score = scorer(stereo_chem_mapping)
+    print(score)
+
+def test_score_shape_mismatch(stereo_chem_mapping):
+    """
+    Currently a smoke test
+    """
+    scorer = MappingShapeMismatchScorer()
+    score = scorer(stereo_chem_mapping)
+    print(score)
+
+
+@pytest.mark.parametrize("scorer_class", [ MappingRMSDScorer,
+    _MappingShapeDistanceScorer,
+    MappingShapeMismatchScorer,
+    MappingShapeOverlapScorer,
+    MappingVolumeRatioScorer,
+    MappingRatioMappedAtomsScorer,
+    DefaultKartografScorer])
+def test_scorer_identical_molecules(scorer_class, benzene_benzene_mapping):
+    """
+    Currently a smoke test
+    """
+    scorer = scorer_class()
+    score = scorer(benzene_benzene_mapping)
+
+    assert isinstance(score, float)
+    assert score == 0, "Score of identical Molecule should be 0"
+
+
+@pytest.mark.parametrize("scorer_class, exp", [(MappingRMSDScorer, 0),
+                                               (_MappingShapeDistanceScorer, 1),
+                                               (MappingShapeMismatchScorer,1),
+                                               (MappingShapeOverlapScorer, 1),
+                                               (MappingRatioMappedAtomsScorer,1)])
+def test_scorer_empty_mapping(scorer_class, exp:float, benzene_benzene_empty_mapping):
+    """
+    Currently a smoke test
+    """
+    scorer = scorer_class()
+    score = scorer(benzene_benzene_empty_mapping)
+
+    assert isinstance(score, float)
+    assert score == exp, "Score of non-Mapping should be "+str(exp)+" for "+str(scorer_class.__name__)+" but is: "+str(score)
+
+
+@pytest.mark.parametrize("scorer_class, exp", [(MappingVolumeRatioScorer, 1),
+                                               (DefaultKartografScorer,1)])
+def test_scorer_empty_mapping_err(scorer_class, exp:float, benzene_benzene_empty_mapping):
+    """
+    Currently a smoke test
+    """
+    with pytest.raises(ValueError) as exc:
+        scorer = scorer_class()
+        score = scorer(benzene_benzene_empty_mapping)
+
+    assert "Mapping is too small to calculate convex hull" in str(exc.value)
```

### Comparing `kartograf-0.5.1/src/kartograf/tests/test_element_filters.py` & `kartograf-0.5.2/src/kartograf/tests/test_element_filters.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import pytest
-from rdkit import Chem
-
-from kartograf import filters
-
-
-@pytest.mark.parametrize('reverse', [False, True])
-def test_atoms_H_only_H_mapped(reverse):
-    # ethane to propane, hydrogen from ethane mapped to carbon
-    m1 = Chem.AddHs(Chem.MolFromSmiles('CC'))
-    m2 = Chem.AddHs(Chem.MolFromSmiles('CCC'))
-    mapping = {0: 0, 1: 1,
-               2: 2,  # this is a H->C, should get removed
-               5: 3,  # this is a H->H, should remain
-               }
-    ref = {0: 0, 1: 1, 5: 3}
-    if reverse:
-        m1, m2 = m2, m1
-        mapping = {v: k for k, v in mapping.items()}
-        ref = {v: k for k, v in ref.items()}
-
-    newmapping = filters.filter_atoms_h_only_h_mapped(m1, m2, mapping)
-
-    assert newmapping == ref
-
-
-@pytest.mark.parametrize('reverse', [False, True])
-def test_element_change(reverse):
-    # benzene to pyridine, has heteroatom change
-    # will result in non-whole ring, but that isn't the job of this filter
-    m1 = Chem.MolFromSmiles('c1ccccn1')
-    m2 = Chem.MolFromSmiles('c1ccccc1')
-    if reverse:
-        m1, m2 = m2, m1
-
-    mapping = {i: i for i in range(6)}
-
-    newmapping = filters.filter_element_changes(m1, m2, mapping)
-
-    assert newmapping == {i: i for i in range(5)}
+import pytest
+from rdkit import Chem
+
+from kartograf import filters
+
+
+@pytest.mark.parametrize('reverse', [False, True])
+def test_atoms_H_only_H_mapped(reverse):
+    # ethane to propane, hydrogen from ethane mapped to carbon
+    m1 = Chem.AddHs(Chem.MolFromSmiles('CC'))
+    m2 = Chem.AddHs(Chem.MolFromSmiles('CCC'))
+    mapping = {0: 0, 1: 1,
+               2: 2,  # this is a H->C, should get removed
+               5: 3,  # this is a H->H, should remain
+               }
+    ref = {0: 0, 1: 1, 5: 3}
+    if reverse:
+        m1, m2 = m2, m1
+        mapping = {v: k for k, v in mapping.items()}
+        ref = {v: k for k, v in ref.items()}
+
+    newmapping = filters.filter_atoms_h_only_h_mapped(m1, m2, mapping)
+
+    assert newmapping == ref
+
+
+@pytest.mark.parametrize('reverse', [False, True])
+def test_element_change(reverse):
+    # benzene to pyridine, has heteroatom change
+    # will result in non-whole ring, but that isn't the job of this filter
+    m1 = Chem.MolFromSmiles('c1ccccn1')
+    m2 = Chem.MolFromSmiles('c1ccccc1')
+    if reverse:
+        m1, m2 = m2, m1
+
+    mapping = {i: i for i in range(6)}
+
+    newmapping = filters.filter_element_changes(m1, m2, mapping)
+
+    assert newmapping == {i: i for i in range(5)}
```

### Comparing `kartograf-0.5.1/src/kartograf.egg-info/PKG-INFO` & `kartograf-0.5.2/src/kartograf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kartograf
-Version: 0.5.1
+Version: 0.5.2
 Summary: Kartograf is a package for mapping geometrically atoms of two molecules. (like you need it with hybrid topology)
 Author-email: Benjamin Ries <benjamin-ries@outlook.com>, David Swenson <dwhswenson@gmail.com>, Irfan Alibay <irfan.alibay@gmail.com>, Mike Henry <mike.henry@choderalab.org>, Richard J Gowers <richardjgowers@gmail.com>
 Project-URL: Homepage, https://github.com/OpenFreeEnergy/kartograf
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -75,11 +75,23 @@
 
 ```shell
 conda install -c conda-forge kartograf
 ```
 
 Or use Kartograf from the OpenFE Environment (soon).
 
+For Developing Kartograf, you might want to use this approach:
+
+```shell
+git clone https://github.com/OpenFreeEnergy/kartograf.git
+
+cd kartograf
+conda env create -f environment.yml
+
+conda activate kartograf
+pip install .
+
+```
 ## References
```

