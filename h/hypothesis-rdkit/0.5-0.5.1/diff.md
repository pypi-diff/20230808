# Comparing `tmp/hypothesis-rdkit-0.5.tar.gz` & `tmp/hypothesis-rdkit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis-rdkit-0.5.tar", last modified: Fri Jun  9 08:53:58 2023, max compression
+gzip compressed data, was "hypothesis-rdkit-0.5.1.tar", last modified: Tue Aug  8 13:01:19 2023, max compression
```

## Comparing `hypothesis-rdkit-0.5.tar` & `hypothesis-rdkit-0.5.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-06-09 08:53:58.112559 hypothesis-rdkit-0.5/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1081 2023-03-06 20:54:00.000000 hypothesis-rdkit-0.5/LICENSE
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       81 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/MANIFEST.in
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1785 2023-06-09 08:53:58.112559 hypothesis-rdkit-0.5/PKG-INFO
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1118 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/README.md
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-06-09 08:53:58.112559 hypothesis-rdkit-0.5/hypothesis_rdkit/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       24 2023-02-19 23:11:07.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     9399 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/fragment.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000) 22377762 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/fragments_100000.pkl
--rw-rw-r--   0 hirte     (1000) hirte     (1000)  2730143 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/fragments_100000.smi
--rw-rw-r--   0 hirte     (1000) hirte     (1000)  5932863 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/fragments_30000.pkl
--rw-rw-r--   0 hirte     (1000) hirte     (1000)   725332 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/fragments_30000.smi
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      199 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/hook.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     8201 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/strategy.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     3685 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/util.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-06-09 08:53:58.112559 hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1785 2023-06-09 08:53:58.000000 hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/PKG-INFO
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      632 2023-06-09 08:53:58.000000 hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/SOURCES.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)        1 2023-06-09 08:53:58.000000 hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/dependency_links.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       62 2023-06-09 08:53:58.000000 hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/entry_points.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       45 2023-06-09 08:53:58.000000 hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/requires.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       17 2023-06-09 08:53:58.000000 hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/top_level.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2023-06-09 08:53:58.112559 hypothesis-rdkit-0.5/setup.cfg
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1025 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/setup.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-06-09 08:53:58.112559 hypothesis-rdkit-0.5/tests/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      648 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.5/tests/test_mol_blocks.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      916 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/tests/test_mols.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      607 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.5/tests/test_smiles.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-08-08 13:01:19.432043 hypothesis-rdkit-0.5.1/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1081 2023-03-06 20:54:00.000000 hypothesis-rdkit-0.5.1/LICENSE
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       81 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5.1/MANIFEST.in
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1787 2023-08-08 13:01:19.432043 hypothesis-rdkit-0.5.1/PKG-INFO
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1118 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5.1/README.md
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-08-08 13:01:19.428043 hypothesis-rdkit-0.5.1/hypothesis_rdkit/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       24 2023-02-19 23:11:07.000000 hypothesis-rdkit-0.5.1/hypothesis_rdkit/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     9399 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5.1/hypothesis_rdkit/fragment.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000) 22377762 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5.1/hypothesis_rdkit/fragments_100000.pkl
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)  2730143 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5.1/hypothesis_rdkit/fragments_100000.smi
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)  5932863 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5.1/hypothesis_rdkit/fragments_30000.pkl
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)   725332 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5.1/hypothesis_rdkit/fragments_30000.smi
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      199 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.5.1/hypothesis_rdkit/hook.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     8201 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5.1/hypothesis_rdkit/strategy.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     3685 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5.1/hypothesis_rdkit/util.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-08-08 13:01:19.432043 hypothesis-rdkit-0.5.1/hypothesis_rdkit.egg-info/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1787 2023-08-08 13:01:19.000000 hypothesis-rdkit-0.5.1/hypothesis_rdkit.egg-info/PKG-INFO
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      632 2023-08-08 13:01:19.000000 hypothesis-rdkit-0.5.1/hypothesis_rdkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)        1 2023-08-08 13:01:19.000000 hypothesis-rdkit-0.5.1/hypothesis_rdkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       62 2023-08-08 13:01:19.000000 hypothesis-rdkit-0.5.1/hypothesis_rdkit.egg-info/entry_points.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       50 2023-08-08 13:01:19.000000 hypothesis-rdkit-0.5.1/hypothesis_rdkit.egg-info/requires.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       17 2023-08-08 13:01:19.000000 hypothesis-rdkit-0.5.1/hypothesis_rdkit.egg-info/top_level.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2023-08-08 13:01:19.432043 hypothesis-rdkit-0.5.1/setup.cfg
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1035 2023-08-08 12:58:05.000000 hypothesis-rdkit-0.5.1/setup.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-08-08 13:01:19.432043 hypothesis-rdkit-0.5.1/tests/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      648 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.5.1/tests/test_mol_blocks.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      916 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5.1/tests/test_mols.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      607 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.5.1/tests/test_smiles.py
```

### Comparing `hypothesis-rdkit-0.5/LICENSE` & `hypothesis-rdkit-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.5/PKG-INFO` & `hypothesis-rdkit-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-rdkit
-Version: 0.5
+Version: 0.5.1
 Home-page: https://github.com/shirte/hypothesis-rdkit
 Maintainer: Steffen Hirte
 Maintainer-email: shirte@users.noreply.github.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `hypothesis-rdkit-0.5/README.md` & `hypothesis-rdkit-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.5/hypothesis_rdkit/fragment.py` & `hypothesis-rdkit-0.5.1/hypothesis_rdkit/fragment.py`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.5/hypothesis_rdkit/fragments_100000.pkl` & `hypothesis-rdkit-0.5.1/hypothesis_rdkit/fragments_100000.pkl`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.5/hypothesis_rdkit/fragments_100000.smi` & `hypothesis-rdkit-0.5.1/hypothesis_rdkit/fragments_100000.smi`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.5/hypothesis_rdkit/fragments_30000.pkl` & `hypothesis-rdkit-0.5.1/hypothesis_rdkit/fragments_30000.pkl`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.5/hypothesis_rdkit/fragments_30000.smi` & `hypothesis-rdkit-0.5.1/hypothesis_rdkit/fragments_30000.smi`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.5/hypothesis_rdkit/strategy.py` & `hypothesis-rdkit-0.5.1/hypothesis_rdkit/strategy.py`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.5/hypothesis_rdkit/util.py` & `hypothesis-rdkit-0.5.1/hypothesis_rdkit/util.py`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/PKG-INFO` & `hypothesis-rdkit-0.5.1/hypothesis_rdkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-rdkit
-Version: 0.5
+Version: 0.5.1
 Home-page: https://github.com/shirte/hypothesis-rdkit
 Maintainer: Steffen Hirte
 Maintainer-email: shirte@users.noreply.github.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/SOURCES.txt` & `hypothesis-rdkit-0.5.1/hypothesis_rdkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.5/setup.py` & `hypothesis-rdkit-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import find_packages, setup
 
 setup(
     name="hypothesis-rdkit",
-    version="0.5",
+    version="0.5.1",
     maintainer="Steffen Hirte",
     maintainer_email="shirte@users.noreply.github.com",
     packages=find_packages(),
     url="https://github.com/shirte/hypothesis-rdkit",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     license_files=("LICENSE",),
-    install_requires=["hypothesis"],
+    install_requires=["hypothesis", "tqdm"],
     extras_require={"dev": ["black", "isort"], "test": ["pytest"]},
     entry_points={"hypothesis": {"_ = hypothesis_rdkit.hook:_hypothesis_setup_hook"}},
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `hypothesis-rdkit-0.5/tests/test_mol_blocks.py` & `hypothesis-rdkit-0.5.1/tests/test_mol_blocks.py`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.5/tests/test_mols.py` & `hypothesis-rdkit-0.5.1/tests/test_mols.py`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.5/tests/test_smiles.py` & `hypothesis-rdkit-0.5.1/tests/test_smiles.py`

 * *Files identical despite different names*

