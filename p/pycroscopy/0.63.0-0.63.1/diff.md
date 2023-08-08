# Comparing `tmp/pycroscopy-0.63.0.tar.gz` & `tmp/pycroscopy-0.63.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycroscopy-0.63.0.tar", last modified: Mon Jul  3 19:51:33 2023, max compression
+gzip compressed data, was "pycroscopy-0.63.1.tar", last modified: Tue Aug  8 19:01:24 2023, max compression
```

## Comparing `pycroscopy-0.63.0.tar` & `pycroscopy-0.63.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.683387 pycroscopy-0.63.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-03 19:51:33.683387 pycroscopy-0.63.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.671388 pycroscopy-0.63.0/pycroscopy/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.671388 pycroscopy-0.63.0/pycroscopy/corr/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/corr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.675387 pycroscopy-0.63.0/pycroscopy/fft/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/fft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/fft/image_fft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.675387 pycroscopy-0.63.0/pycroscopy/image/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/image/image_atoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/image/image_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/image/image_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/image/image_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/image/image_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19356 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/image/image_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.675387 pycroscopy-0.63.0/pycroscopy/learn/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.679387 pycroscopy-0.63.0/pycroscopy/learn/dl/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/dl/datautils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/dl/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/dl/nnblocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/dl/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.679387 pycroscopy-0.63.0/pycroscopy/learn/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/ml/decompose.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/learn/ml/matrix_factor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.679387 pycroscopy-0.63.0/pycroscopy/signal/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/signal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.683387 pycroscopy-0.63.0/pycroscopy/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/stats/atom_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/stats/atom_stats_n.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/stats/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.683387 pycroscopy-0.63.0/pycroscopy/viz/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/pycroscopy/viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.671388 pycroscopy-0.63.0/pycroscopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-03 19:51:33.000000 pycroscopy-0.63.0/pycroscopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-03 19:51:33.000000 pycroscopy-0.63.0/pycroscopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:33.000000 pycroscopy-0.63.0/pycroscopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-03 19:51:33.000000 pycroscopy-0.63.0/pycroscopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 19:51:33.000000 pycroscopy-0.63.0/pycroscopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-03 19:51:33.683387 pycroscopy-0.63.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-03 19:47:32.000000 pycroscopy-0.63.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:01:24.377211 pycroscopy-0.63.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-08 18:57:59.000000 pycroscopy-0.63.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 18:57:59.000000 pycroscopy-0.63.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-08-08 19:01:24.377211 pycroscopy-0.63.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-08-08 18:57:59.000000 pycroscopy-0.63.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:01:24.369212 pycroscopy-0.63.1/pycroscopy/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:01:24.369212 pycroscopy-0.63.1/pycroscopy/corr/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/corr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:01:24.369212 pycroscopy-0.63.1/pycroscopy/fft/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/fft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/fft/image_fft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:01:24.373211 pycroscopy-0.63.1/pycroscopy/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/image/image_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/image/image_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/image/image_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/image/image_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/image/image_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19632 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/image/image_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:01:24.373211 pycroscopy-0.63.1/pycroscopy/learn/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/learn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:01:24.373211 pycroscopy-0.63.1/pycroscopy/learn/dl/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/learn/dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/learn/dl/datautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/learn/dl/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/learn/dl/nnblocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/learn/dl/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:01:24.373211 pycroscopy-0.63.1/pycroscopy/learn/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/learn/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/learn/ml/decompose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/learn/ml/matrix_factor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:01:24.377211 pycroscopy-0.63.1/pycroscopy/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/signal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:01:24.377211 pycroscopy-0.63.1/pycroscopy/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/stats/atom_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/stats/atom_stats_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/stats/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:01:24.377211 pycroscopy-0.63.1/pycroscopy/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/pycroscopy/viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:01:24.369212 pycroscopy-0.63.1/pycroscopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-08-08 19:01:24.000000 pycroscopy-0.63.1/pycroscopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-08 19:01:24.000000 pycroscopy-0.63.1/pycroscopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 19:01:24.000000 pycroscopy-0.63.1/pycroscopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-08 19:01:24.000000 pycroscopy-0.63.1/pycroscopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-08 19:01:24.000000 pycroscopy-0.63.1/pycroscopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-08 19:01:24.377211 pycroscopy-0.63.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-08-08 18:58:00.000000 pycroscopy-0.63.1/setup.py
```

### Comparing `pycroscopy-0.63.0/LICENSE.txt` & `pycroscopy-0.63.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/PKG-INFO` & `pycroscopy-0.63.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycroscopy
-Version: 0.63.0
+Version: 0.63.1
 Summary: Python library for scientific analysis of microscopy data
 Home-page: https://pycroscopy.github.io/pycroscopy/about.html
 Author: Pycroscopy contributors
 Author-email: pycroscopy@gmail.com
 License: MIT
 Keywords: EELS,STEM,TEM,XRD,AFM,SPM,STS,band excitation,BE,BEPS,Raman,NanoIR,electron microscopy, scanning probe, x-rays,atomic force microscopy,SIMS,energy,spectroscopy,imaging,microscopy,spectracharacterization,spectrogram,hyperspectral,multidimensional,data format,universal,clustering,decomposition,curve fitting,data analysis,PCA, SVD, NMF, DBSCAN, kMeans,machine learning,bayesian inference,fft filtering,signal processing,image cleaning,denoising,model,msa,quantification
 Platform: Linux
```

### Comparing `pycroscopy-0.63.0/README.rst` & `pycroscopy-0.63.1/README.rst`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy/__init__.py` & `pycroscopy-0.63.1/pycroscopy/__init__.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy/fft/image_fft.py` & `pycroscopy-0.63.1/pycroscopy/fft/image_fft.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy/image/__init__.py` & `pycroscopy-0.63.1/pycroscopy/image/__init__.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy/image/image_atoms.py` & `pycroscopy-0.63.1/pycroscopy/image/image_atoms.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy/image/image_clean.py` & `pycroscopy-0.63.1/pycroscopy/image/image_clean.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy/image/image_graph.py` & `pycroscopy-0.63.1/pycroscopy/image/image_graph.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy/image/image_registration.py` & `pycroscopy-0.63.1/pycroscopy/image/image_registration.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,26 +126,33 @@
         dem_reg[i, :, :] = sitk.GetArrayFromImage(out)
 
     print(':-)')
     print('You have successfully completed Diffeomorphic Demons Registration')
 
     demon_registered = sidpy.Dataset.from_array(dem_reg)
 
-    delattr(demon_registered, 'a')
-    delattr(demon_registered, 'b')
-    delattr(demon_registered, 'c')
+    # delattr(demon_registered, 'a')
+    # delattr(demon_registered, 'b')
+    # delattr(demon_registered, 'c')
+    demon_registered.del_dimension(0)
+    demon_registered.del_dimension(1)
+    demon_registered.del_dimension(2)
+    
     axis = dataset._axes[0]
-    axis.name = 'frame'
+    # axis.name = 'frame'
     demon_registered.set_dimension(0, axis)
+    demon_registered.rename_dimension(0, 'frame')
     axis = dataset._axes[1]
-    axis.name = 'x'
+    # axis.name = 'x'
     demon_registered.set_dimension(1, axis)
+    demon_registered.rename_dimension(0, 'x')
     axis = dataset._axes[2]
-    axis.name = 'y'
+    # axis.name = 'y'
     demon_registered.set_dimension(2, axis)
+    demon_registered.rename_dimension(2, 'y')
     demon_registered.title = 'Non-Rigid Registration'
     demon_registered.source = dataset.title
 
     demon_registered.metadata = {'analysis': 'non-rigid demon registration'}
     if 'input_crop' in dataset.metadata:
         demon_registered.metadata['input_crop'] = dataset.metadata['input_crop']
     if 'input_shape' in dataset.metadata:
@@ -226,24 +233,30 @@
     crop_reg, input_crop = crop_image_stack(rig_reg, drift)
 
     rigid_registered = dataset.like_data(crop_reg)
     rigid_registered.title = 'Rigid Registration'
     rigid_registered.source = dataset.title
     rigid_registered.metadata = {'analysis': 'rigid sub-pixel registration', 'drift': drift,
                                  'input_crop': input_crop, 'input_shape': dataset.shape[1:]}
-    if hasattr(rigid_registered, 'z'):
-        del rigid_registered.z
-    if hasattr(rigid_registered, 'x'):
-        del rigid_registered.x
-    if hasattr(rigid_registered, 'y'):
-        del rigid_registered.y
-    rigid_registered._axes = {}
+    #if hasattr(rigid_registered, 'a'):
+    #    del rigid_registered.a
+    #if hasattr(rigid_registered, 'b'):
+    #    del rigid_registered.b
+    #if hasattr(rigid_registered, 'c'):
+    #    del rigid_registered.c
+    #rigid_registered._axes = {}
+
+    rigid_registered.del_dimension(0)
+    rigid_registered.del_dimension(1)
+    rigid_registered.del_dimension(2)
+
     rigid_registered.set_dimension(0, dataset._axes[frame_dim[0]])
     rigid_registered.set_dimension(1, dataset._axes[spatial_dim[0]][input_crop[0]:input_crop[1]])
     rigid_registered.set_dimension(2, dataset._axes[spatial_dim[1]][input_crop[2]:input_crop[3]])
+
     return rigid_registered
 
 
 def rig_reg_drift(dset, rel_drift):
     """ Shifting images on top of each other
 
     Uses relative drift to shift images on top of each other,
```

### Comparing `pycroscopy-0.63.0/pycroscopy/image/image_utilities.py` & `pycroscopy-0.63.1/pycroscopy/image/image_utilities.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy/image/image_window.py` & `pycroscopy-0.63.1/pycroscopy/image/image_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Image windowing class
 
 import numpy as np
 import sidpy
 from sidpy.base.num_utils import build_ind_val_matrices
-from scipy.signal.windows import hamming, blackman
+from scipy.signal.windows import hamming, hann, blackman
 from skimage.transform import rescale
 import dask
 
 class ImageWindowing:
     """
     This class will generate windows from sidpy dataset objects. At present only 2D windowing is allowed.
     """
@@ -26,15 +26,15 @@
             - 'window_step_y' (integer) (required): step size of the window across the y-axis. Must divide into the image size in the y axis
             - 'mode' (string) (Optional, default is 'image'): One of 'image' or 'fft' which defines the processing to be performed for each window.
                 The choice of 'fft' will perform 2D fast Fourier transforms on each image whereas 'image' will not perform any operation on the window
             - 'fft_mode' (string) (Optional, default is 'abs'): If mode is 'fft', choose whether to look at amplitude or phase. Options are 'abs', 'phase' and 'complex'.
             - 'interpol_factor' (float) (Optional, default is 1.0): Interpolation factor for windows to increase or decrease size of the windows.
             - 'zoom_factor' (integer or list of ints) (Optional, default is 1): Zoom the window by this factor, typically done for 'fft' mode to observe higher frequencies clearly
                             If passing a list of ints, this will determine the degree of cropping per axis
-            - 'filter' (string) (Optional, default is None): Filtering to use for the image window. Options are 'blackman', 'hamming'.
+            - 'filter' (string) (Optional, default is None): Filtering to use for the image window. Options are 'blackman', 'hamming', 'hann'.
             The filter is applied to each window before 'mode'.
         - verbose : (Optional) Boolean
             Verbose flag. Default is False.
 
         Returns
         --------
         Instance of ImageWindowing object setup with parameters defined by the parms_dict above.
@@ -67,26 +67,30 @@
             self.zoom_factor = 1
             parms_dict['zoom_factor'] = 1
 
         # Based on the zoom and interpolation factors we need to figure out the final size of the window
         self.window_size_final_x, self.window_size_final_y = self._get_window_size()
         #Setup the filter for the window
         if 'filter' in parms_dict.keys():
-            if parms_dict['filter'] not in ['blackman', 'hamming']:
-                raise ValueError("Parameter 'filter' must be one of 'hamming', 'blackman'")
+            if parms_dict['filter'] not in ['blackman', 'hamming','hann']:
+                raise ValueError("Parameter 'filter' must be one of 'hamming', 'blackman', 'hann'")
             else:
                 self.filter = parms_dict['filter']
                 if self.filter == 'hamming':
                     filter_x = hamming(self.window_size_final_x)
                     filter_y = hamming(self.window_size_final_y)
                     self.filter_mat = np.sqrt(np.outer(filter_x, filter_y))
                 elif self.filter == 'blackman':
                     filter_x = blackman(self.window_size_final_x)
                     filter_y = blackman(self.window_size_final_y)
                     self.filter_mat = np.sqrt(np.outer(filter_x, filter_y))
+                elif self.filter == 'hanning':
+                    filter_x = hann(self.window_size_final_x)
+                    filter_y = hann(self.window_size_final_y)
+                    self.filter_mat = np.sqrt(np.outer(filter_x, filter_y))
         else:
             self.filter = 'None'
 
         if self.mode=='fft':
             #load FFT options
             if 'fft_mode' in parms_dict.keys():
                 if parms_dict['fft_mode'] not in ['abs', 'phase', 'complex']:
```

### Comparing `pycroscopy-0.63.0/pycroscopy/learn/__init__.py` & `pycroscopy-0.63.1/pycroscopy/learn/__init__.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy/learn/dl/datautils.py` & `pycroscopy-0.63.1/pycroscopy/learn/dl/datautils.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy/learn/dl/models.py` & `pycroscopy-0.63.1/pycroscopy/learn/dl/models.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy/learn/dl/nnblocks.py` & `pycroscopy-0.63.1/pycroscopy/learn/dl/nnblocks.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy/learn/dl/trainer.py` & `pycroscopy-0.63.1/pycroscopy/learn/dl/trainer.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy/learn/ml/decompose.py` & `pycroscopy-0.63.1/pycroscopy/learn/ml/decompose.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy/learn/ml/matrix_factor.py` & `pycroscopy-0.63.1/pycroscopy/learn/ml/matrix_factor.py`

 * *Files 6% similar despite different names*

```diff
@@ -166,14 +166,22 @@
             # Then we want to return components, abundances, and explained variances if available.
             # We should return a list of sidpy dataset objects
             self.abundances = abundances_dset.unfold()
             self.abundances.data_type = sidpy.DataType.IMAGE_STACK
 
             self.components = components_dset.unfold()
             self.components.data_type = sidpy.DataType.LINE_PLOT_FAMILY  # Check this again
+
+            #Let's save the processing steps done also
+            kw_args_list = [(key,val) for key, val in kwargs.items()]
+            mf_metadata = {'method':self.method, 'arguments':kw_args_list, 'n_components': self.ncomp, 'return_fit': self.return_fit}
+            
+            for data_set in [self.abundances,self.components, self.fit_dset]:
+                data_set.metadata['Matrix_Factorization'] = mf_metadata
+
             self.results_computed = True
             
 
             if self.return_fit:
                 return self.abundances, self.components, self.fit_dset
             else:
                 return self.abundances, self.components
```

### Comparing `pycroscopy-0.63.0/pycroscopy/stats/atom_stats.py` & `pycroscopy-0.63.1/pycroscopy/stats/atom_stats.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy/stats/atom_stats_n.py` & `pycroscopy-0.63.1/pycroscopy/stats/atom_stats_n.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy/stats/tree.py` & `pycroscopy-0.63.1/pycroscopy/stats/tree.py`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/pycroscopy.egg-info/PKG-INFO` & `pycroscopy-0.63.1/pycroscopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycroscopy
-Version: 0.63.0
+Version: 0.63.1
 Summary: Python library for scientific analysis of microscopy data
 Home-page: https://pycroscopy.github.io/pycroscopy/about.html
 Author: Pycroscopy contributors
 Author-email: pycroscopy@gmail.com
 License: MIT
 Keywords: EELS,STEM,TEM,XRD,AFM,SPM,STS,band excitation,BE,BEPS,Raman,NanoIR,electron microscopy, scanning probe, x-rays,atomic force microscopy,SIMS,energy,spectroscopy,imaging,microscopy,spectracharacterization,spectrogram,hyperspectral,multidimensional,data format,universal,clustering,decomposition,curve fitting,data analysis,PCA, SVD, NMF, DBSCAN, kMeans,machine learning,bayesian inference,fft filtering,signal processing,image cleaning,denoising,model,msa,quantification
 Platform: Linux
```

### Comparing `pycroscopy-0.63.0/pycroscopy.egg-info/SOURCES.txt` & `pycroscopy-0.63.1/pycroscopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycroscopy-0.63.0/setup.py` & `pycroscopy-0.63.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                 'matplotlib>=2.0.0',
                 'torch>=1.0.0',
                 'tensorly>=0.6.0',
                 'tqdm',
                 'ipywidgets>=5.2.2',
                 'ipython',
                 'simpleitk',
-                'sidpy>=0.0.6',
+                'sidpy>=0.12.1',
                 'pysptools',
                 'cvxopt>=1.2.7'
                 ]
 
 setup(
     name='pycroscopy',
     version=__version__,
```

