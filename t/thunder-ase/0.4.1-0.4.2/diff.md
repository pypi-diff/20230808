# Comparing `tmp/thunder-ase-0.4.1.tar.gz` & `tmp/thunder-ase-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunder-ase-0.4.1.tar", last modified: Fri Jul 14 05:48:11 2023, max compression
+gzip compressed data, was "thunder-ase-0.4.2.tar", last modified: Tue Aug  8 01:37:41 2023, max compression
```

## Comparing `thunder-ase-0.4.1.tar` & `thunder-ase-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:48:11.485443 thunder-ase-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-14 05:48:11.485443 thunder-ase-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 05:48:11.485443 thunder-ase-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:48:11.485443 thunder-ase-0.4.1/thunder_ase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/thunder_ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32532 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/thunder_ase/fireball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:48:11.485443 thunder-ase-0.4.1/thunder_ase/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/thunder_ase/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/thunder_ase/utils/basis_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/thunder_ase/utils/mwfn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/thunder_ase/utils/shell_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:48:11.485443 thunder-ase-0.4.1/thunder_ase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-14 05:48:11.000000 thunder-ase-0.4.1/thunder_ase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-14 05:48:11.000000 thunder-ase-0.4.1/thunder_ase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:48:11.000000 thunder-ase-0.4.1/thunder_ase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-14 05:48:11.000000 thunder-ase-0.4.1/thunder_ase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 05:48:11.000000 thunder-ase-0.4.1/thunder_ase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:37:41.968806 thunder-ase-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-08 01:37:41.968806 thunder-ase-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:37:41.968806 thunder-ase-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:37:41.968806 thunder-ase-0.4.2/thunder_ase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/thunder_ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32610 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/thunder_ase/fireball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:37:41.968806 thunder-ase-0.4.2/thunder_ase/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/thunder_ase/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/thunder_ase/utils/basis_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/thunder_ase/utils/mwfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/thunder_ase/utils/shell_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:37:41.968806 thunder-ase-0.4.2/thunder_ase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-08 01:37:41.000000 thunder-ase-0.4.2/thunder_ase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-08 01:37:41.000000 thunder-ase-0.4.2/thunder_ase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:37:41.000000 thunder-ase-0.4.2/thunder_ase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 01:37:41.000000 thunder-ase-0.4.2/thunder_ase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 01:37:41.000000 thunder-ase-0.4.2/thunder_ase.egg-info/top_level.txt
```

### Comparing `thunder-ase-0.4.1/PKG-INFO` & `thunder-ase-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thunder-ase
-Version: 0.4.1
+Version: 0.4.2
 Summary: ASE calculator interface for FIREBALL code
 Author-email: PJ Ren <openrpj@gmail.com>
 Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
 Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -64,14 +64,15 @@
 
 * `qstate` : The charge state of the system. Default is 0. Positive values mean add extra electrons, negatives mean remove electrons.
 * `efermi_t`: Smearing temperature at Fermi level. Default is 100.0, which is about 0.0086 eV. For metal system, larger value is recommended.
 * `max_scf_iterations_set`: Scf steps maximum. Default is 50.
 * `scf_tolerance_set`: Scf tolerance of charge. Default is 1.0E-6. Smaller value is recommended for higher precision, e.g. 1.0E-8.
 * `beta_set`: Broyden’s mix factor of charges. Default is 0.08.
 * `ecut_set`: To control mesh grid density. Default is 200.0.
+* `ipi`: open I-PI socket. Default is 0.
 * `iwriteout_charges`: Write out charges. Default is  0 (False).
 
 #### Basic Parameters of Thunder-ASE
 
 * `kpt_size`: Size of k point sampling. Default is None for molecules and [1, 1, 1] for crystals.
 * `kpt_offset`: Offset for k point sampling. Default is None for molecules and [0., 0., 0.] for crystals.
 * `kpt_interval`: Define kpoint sampling by the interval. Default is None.
```

### Comparing `thunder-ase-0.4.1/README.md` & `thunder-ase-0.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
 * `qstate` : The charge state of the system. Default is 0. Positive values mean add extra electrons, negatives mean remove electrons.
 * `efermi_t`: Smearing temperature at Fermi level. Default is 100.0, which is about 0.0086 eV. For metal system, larger value is recommended.
 * `max_scf_iterations_set`: Scf steps maximum. Default is 50.
 * `scf_tolerance_set`: Scf tolerance of charge. Default is 1.0E-6. Smaller value is recommended for higher precision, e.g. 1.0E-8.
 * `beta_set`: Broyden’s mix factor of charges. Default is 0.08.
 * `ecut_set`: To control mesh grid density. Default is 200.0.
+* `ipi`: open I-PI socket. Default is 0.
 * `iwriteout_charges`: Write out charges. Default is  0 (False).
 
 #### Basic Parameters of Thunder-ASE
 
 * `kpt_size`: Size of k point sampling. Default is None for molecules and [1, 1, 1] for crystals.
 * `kpt_offset`: Offset for k point sampling. Default is None for molecules and [0., 0., 0.] for crystals.
 * `kpt_interval`: Define kpoint sampling by the interval. Default is None.
```

### Comparing `thunder-ase-0.4.1/pyproject.toml` & `thunder-ase-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "thunder-ase"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="PJ Ren", email="openrpj@gmail.com" },
 ]
 description = "ASE calculator interface for FIREBALL code"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `thunder-ase-0.4.1/thunder_ase/fireball.py` & `thunder-ase-0.4.2/thunder_ase/fireball.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
     'iconstraint_ke': {'type': (int,), 'name': 'iconstraint_KE', 'default': 1},
     'ifix_neighbors': {'type': (int,), 'name': 'ifix_neighbors', 'default': 0},
     'ifix_charges': {'type': (int,), 'name': 'ifix_CHARGES', 'default': 1},
     'max_scf_iterations_set': {'type': (int,), 'name': 'max_scf_iterations_set', 'default': 50},
     'scf_tolerance_set': {'type': (int, float), 'name': 'scf_tolerance_set', 'default': 0.000001},
     'beta_set': {'type': (int, float), 'name': 'beta_set', 'default': 0.08},  # mix factor
     'ecut_set': {'type': (int, float), 'name': 'Ecut_set', 'default': 200.0},  # control mesh grid number
+    'ipi': {'type': (int,), 'name': 'ipi', 'default': 0},  # open I-PI socket
 }
 
 output_params = {
     'iwriteout_me_sandh': {'type': (int,), 'name': 'iwriteout_ME_SandH', 'default': 0},
     'iwriteout_density': {'type': (int,), 'name': 'iwriteout_density', 'default': 0},
     'iwriteout_cdcoeffs': {'type': (int,), 'name': 'iwriteout_cdcoeffs', 'default': 0},
     'iwriteout_charges': {'type': (int,), 'name': 'iwriteout_charges', 'default': 0},
```

### Comparing `thunder-ase-0.4.1/thunder_ase/utils/basis_set.py` & `thunder-ase-0.4.2/thunder_ase/utils/basis_set.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.4.1/thunder_ase/utils/mwfn.py` & `thunder-ase-0.4.2/thunder_ase/utils/mwfn.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.4.1/thunder_ase/utils/shell_dict.py` & `thunder-ase-0.4.2/thunder_ase/utils/shell_dict.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.4.1/thunder_ase.egg-info/PKG-INFO` & `thunder-ase-0.4.2/thunder_ase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thunder-ase
-Version: 0.4.1
+Version: 0.4.2
 Summary: ASE calculator interface for FIREBALL code
 Author-email: PJ Ren <openrpj@gmail.com>
 Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
 Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -64,14 +64,15 @@
 
 * `qstate` : The charge state of the system. Default is 0. Positive values mean add extra electrons, negatives mean remove electrons.
 * `efermi_t`: Smearing temperature at Fermi level. Default is 100.0, which is about 0.0086 eV. For metal system, larger value is recommended.
 * `max_scf_iterations_set`: Scf steps maximum. Default is 50.
 * `scf_tolerance_set`: Scf tolerance of charge. Default is 1.0E-6. Smaller value is recommended for higher precision, e.g. 1.0E-8.
 * `beta_set`: Broyden’s mix factor of charges. Default is 0.08.
 * `ecut_set`: To control mesh grid density. Default is 200.0.
+* `ipi`: open I-PI socket. Default is 0.
 * `iwriteout_charges`: Write out charges. Default is  0 (False).
 
 #### Basic Parameters of Thunder-ASE
 
 * `kpt_size`: Size of k point sampling. Default is None for molecules and [1, 1, 1] for crystals.
 * `kpt_offset`: Offset for k point sampling. Default is None for molecules and [0., 0., 0.] for crystals.
 * `kpt_interval`: Define kpoint sampling by the interval. Default is None.
```

