# Comparing `tmp/mms_nirs-0.1.5.tar.gz` & `tmp/mms_nirs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mms_nirs-0.1.5.tar", max compression
+gzip compressed data, was "mms_nirs-0.2.0.tar", max compression
```

## Comparing `mms_nirs-0.1.5.tar` & `mms_nirs-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0      143 2023-05-03 11:01:49.168314 mms_nirs-0.1.5/README.md
--rw-r--r--   0        0        0      333 2023-07-31 12:30:11.002332 mms_nirs-0.1.5/mms_nirs/BRUNO/__init__.py
--rw-r--r--   0        0        0     3323 2023-07-31 12:30:11.002332 mms_nirs-0.1.5/mms_nirs/BRUNO/calc_values.py
--rw-r--r--   0        0        0     4835 2023-07-31 12:30:11.002332 mms_nirs-0.1.5/mms_nirs/BRUNO/derivative_fit.py
--rw-r--r--   0        0        0     5525 2023-07-31 12:30:11.002332 mms_nirs-0.1.5/mms_nirs/BRUNO/fminsearchbnd.py
--rw-r--r--   0        0        0     4335 2023-07-31 12:30:11.002332 mms_nirs-0.1.5/mms_nirs/BRUNO/model_types.py
--rw-r--r--   0        0        0      662 2023-05-09 17:15:42.681482 mms_nirs-0.1.5/mms_nirs/UCLN/DefaultValues.py
--rw-r--r--   0        0        0     3309 2023-07-31 09:39:28.273500 mms_nirs-0.1.5/mms_nirs/UCLN/UCLN.py
--rw-r--r--   0        0        0      152 2023-05-16 10:47:43.079500 mms_nirs-0.1.5/mms_nirs/UCLN/__init__.py
--rw-r--r--   0        0        0     3876 2023-05-09 17:15:42.681482 mms_nirs-0.1.5/mms_nirs/UCLN/defaults.csv
--rw-r--r--   0        0        0        0 2023-05-02 14:50:03.986089 mms_nirs-0.1.5/mms_nirs/__init__.py
--rw-r--r--   0        0        0      908 2023-07-31 12:34:33.022303 mms_nirs-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 mms_nirs-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-05-03 11:01:49.168314 mms_nirs-0.2.0/README.md
+-rw-r--r--   0        0        0      333 2023-07-31 12:30:11.002332 mms_nirs-0.2.0/mms_nirs/BRUNO/__init__.py
+-rw-r--r--   0        0        0     3757 2023-08-08 09:42:00.522844 mms_nirs-0.2.0/mms_nirs/BRUNO/calc_values.py
+-rw-r--r--   0        0        0     4835 2023-07-31 12:30:11.002332 mms_nirs-0.2.0/mms_nirs/BRUNO/derivative_fit.py
+-rw-r--r--   0        0        0     5525 2023-07-31 12:30:11.002332 mms_nirs-0.2.0/mms_nirs/BRUNO/fminsearchbnd.py
+-rw-r--r--   0        0        0     4335 2023-08-08 10:53:05.212146 mms_nirs-0.2.0/mms_nirs/BRUNO/model_types.py
+-rw-r--r--   0        0        0      662 2023-05-09 17:15:42.681482 mms_nirs-0.2.0/mms_nirs/UCLN/DefaultValues.py
+-rw-r--r--   0        0        0     3309 2023-07-31 09:39:28.273500 mms_nirs-0.2.0/mms_nirs/UCLN/UCLN.py
+-rw-r--r--   0        0        0      152 2023-05-16 10:47:43.079500 mms_nirs-0.2.0/mms_nirs/UCLN/__init__.py
+-rw-r--r--   0        0        0     3876 2023-05-09 17:15:42.681482 mms_nirs-0.2.0/mms_nirs/UCLN/defaults.csv
+-rw-r--r--   0        0        0        0 2023-05-02 14:50:03.986089 mms_nirs-0.2.0/mms_nirs/__init__.py
+-rw-r--r--   0        0        0      128 2023-08-08 13:47:20.854221 mms_nirs-0.2.0/mms_nirs/utils/__init__.py
+-rw-r--r--   0        0        0     1871 2023-08-08 13:47:20.854221 mms_nirs-0.2.0/mms_nirs/utils/attenuation.py
+-rw-r--r--   0        0        0      551 2023-08-08 13:47:20.854221 mms_nirs-0.2.0/mms_nirs/utils/dpf.py
+-rw-r--r--   0        0        0      908 2023-08-08 13:47:33.604219 mms_nirs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 mms_nirs-0.2.0/PKG-INFO
```

### Comparing `mms_nirs-0.1.5/mms_nirs/BRUNO/calc_values.py` & `mms_nirs-0.2.0/mms_nirs/BRUNO/calc_values.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,18 +7,25 @@
     QuantityType,
     derivative_fit,
     get_model,
 )
 from .fminsearchbnd import fminsearchbnd
 
 
-def smooth(a, span):
-    # a: NumPy 1-D array containing the data to be smoothed
-    # WSZ: smoothing window size needs, which must be odd number,
-    # as in the original MATLAB implementation
+def smooth(a: np.ndarray, span: int) -> np.ndarray:
+    """MATLAB Smooth function clone
+
+    Args:
+        a (np.ndarray): Numpy array of data to smooth
+        span (int): Size of smoothing window. Must be an odd number
+
+    Returns:
+        np.ndarray: Smoothed data
+    """
+
     out0 = np.convolve(a, np.ones(span, dtype=int), "valid") / span
     r = np.arange(1, span - 1, 2)
     start = np.cumsum(a[: span - 1])[::2] / r
     stop = (np.cumsum(a[:-span:-1])[::2] / r)[::-1]
     return np.concatenate((start, out0, stop))
 
 
@@ -87,30 +94,47 @@
     else:
         model_result = model_function(mua, mus, distance)
 
     model_1stdiff = np.diff(model_result, n=1)
 
     stO2 = coefficients[2] / (coefficients[1] + coefficients[2]) * 100
 
+    # Determine the score of the fit
+
     residual = (model_1stdiff - slope_1stdiff) ** 2
-    residual_norm = (
-        model_1stdiff / np.max(model_1stdiff)
-        - slope_1stdiff / np.max(model_1stdiff)
-    ) ** 2
     sum_residual = np.sum(residual)
 
+    # Indicies of values to determine range between
+    index_710 = np.where(wavelengths == 710)[0][0]
+    index_900 = np.where(wavelengths == 900)[0][0]
+
+    # Indices of HHb wavelengths
     index_HHb = np.arange(
         np.where(wavelengths == 750)[0][0],
         np.where(wavelengths == 770)[0][0] + 1,
     )
+
+    # Indices of H2O wavelengths
     index_water = np.arange(
         np.where(wavelengths == 825)[0][0],
         np.where(wavelengths == 840)[0][0] + 1,
     )
+
+    residual_norm = (
+        model_1stdiff / np.max(model_1stdiff)
+        - slope_1stdiff / np.max(model_1stdiff)
+    ) ** 2
+
     sum_hhb_residuals = np.sum(residual_norm[index_HHb])
     sum_water_residuals = np.sum(residual_norm[index_water])
+
     model_range = np.max(
-        model_1stdiff[6:197] / np.max(model_1stdiff[6:197])
-    ) - np.min(model_1stdiff[6:197] / np.max(model_1stdiff[6:197]))
+        model_1stdiff[index_710:index_900]
+        / np.max(model_1stdiff[index_710:index_900])
+    ) - np.min(
+        model_1stdiff[index_710:index_900]
+        / np.max(model_1stdiff[index_710:index_900])
+    )
+
     score = sum_hhb_residuals * sum_water_residuals / model_range
 
     return stO2, coefficients, residual, residual_norm, sum_residual, score
```

### Comparing `mms_nirs-0.1.5/mms_nirs/BRUNO/derivative_fit.py` & `mms_nirs-0.2.0/mms_nirs/BRUNO/derivative_fit.py`

 * *Files identical despite different names*

### Comparing `mms_nirs-0.1.5/mms_nirs/BRUNO/fminsearchbnd.py` & `mms_nirs-0.2.0/mms_nirs/BRUNO/fminsearchbnd.py`

 * *Files identical despite different names*

### Comparing `mms_nirs-0.1.5/mms_nirs/BRUNO/model_types.py` & `mms_nirs-0.2.0/mms_nirs/BRUNO/model_types.py`

 * *Files identical despite different names*

### Comparing `mms_nirs-0.1.5/mms_nirs/UCLN/DefaultValues.py` & `mms_nirs-0.2.0/mms_nirs/UCLN/DefaultValues.py`

 * *Files identical despite different names*

### Comparing `mms_nirs-0.1.5/mms_nirs/UCLN/UCLN.py` & `mms_nirs-0.2.0/mms_nirs/UCLN/UCLN.py`

 * *Files identical despite different names*

### Comparing `mms_nirs-0.1.5/mms_nirs/UCLN/defaults.csv` & `mms_nirs-0.2.0/mms_nirs/UCLN/defaults.csv`

 * *Files identical despite different names*

### Comparing `mms_nirs-0.1.5/pyproject.toml` & `mms_nirs-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mms-nirs"
-version = "0.1.5"
+version = "0.2.0"
 description = "Algorithms used in the multimodal spectroscopy group to process NIRS data"
 authors = ["Josh Buckland, <joshua.russell-buckland@ucl.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "mms_nirs" }]
 
 [tool.poetry.dependencies]
```

### Comparing `mms_nirs-0.1.5/PKG-INFO` & `mms_nirs-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mms-nirs
-Version: 0.1.5
+Version: 0.2.0
 Summary: Algorithms used in the multimodal spectroscopy group to process NIRS data
 License: MIT
 Author: Josh Buckland,
 Author-email: joshua.russell-buckland@ucl.ac.uk
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

