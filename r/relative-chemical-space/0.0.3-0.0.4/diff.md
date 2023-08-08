# Comparing `tmp/relative_chemical_space-0.0.3.tar.gz` & `tmp/relative_chemical_space-0.0.4.tar.gz`

## Comparing `relative_chemical_space-0.0.3.tar` & `relative_chemical_space-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relative_chemical_space-0.0.3/src/relative_chemical_space/__init__.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 relative_chemical_space-0.0.3/src/relative_chemical_space/chemical_space.py
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 relative_chemical_space-0.0.3/src/relative_chemical_space/supporting_funtions.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 relative_chemical_space-0.0.3/LICENSE
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 relative_chemical_space-0.0.3/README.md
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 relative_chemical_space-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relative_chemical_space-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relative_chemical_space-0.0.4/src/relative_chemical_space/__init__.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 relative_chemical_space-0.0.4/src/relative_chemical_space/chemical_space.py
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 relative_chemical_space-0.0.4/src/relative_chemical_space/supporting_funtions.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 relative_chemical_space-0.0.4/LICENSE
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 relative_chemical_space-0.0.4/README.md
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 relative_chemical_space-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relative_chemical_space-0.0.4/PKG-INFO
```

### Comparing `relative_chemical_space-0.0.3/src/relative_chemical_space/chemical_space.py` & `relative_chemical_space-0.0.4/src/relative_chemical_space/chemical_space.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 def fragments_compound_space(compounds=None, fragments=None, metric='euclidean', distance_matrix=True, relative_space=False, pca_coordinates=False, input_distance_matrix=None):
     import numpy as np
-    from relative_chemical_space.supporting_funtions import *
+    from relative_chemical_space.supporting_funtions import distance_space
+    from relative_chemical_space.supporting_funtions import non_pca_relative_space
+    from relative_chemical_space.supporting_funtions import pca_relative_space
     
     # Distance-based space
         
     if distance_matrix == True and relative_space== False:
         return np.array(distance_space(compounds,fragments,metric))
     
     elif distance_matrix == True and relative_space== True:
```

### Comparing `relative_chemical_space-0.0.3/src/relative_chemical_space/supporting_funtions.py` & `relative_chemical_space-0.0.4/src/relative_chemical_space/supporting_funtions.py`

 * *Files identical despite different names*

### Comparing `relative_chemical_space-0.0.3/LICENSE` & `relative_chemical_space-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `relative_chemical_space-0.0.3/pyproject.toml` & `relative_chemical_space-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "relative_chemical_space"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Stiv Llenga", email="stiv.llenga@h-its.org" },
 ]
 description = "Functions for generating the MFSR and RCS representations."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `relative_chemical_space-0.0.3/PKG-INFO` & `relative_chemical_space-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relative_chemical_space
-Version: 0.0.3
+Version: 0.0.4
 Summary: Functions for generating the MFSR and RCS representations.
 Project-URL: Homepage, https://github.com/hits-ccc/MFSR_RCSa
 Author-email: Stiv Llenga <stiv.llenga@h-its.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

