# Comparing `tmp/acb_mse-1.0.2.tar.gz` & `tmp/acb_mse-1.0.3.tar.gz`

## Comparing `acb_mse-1.0.2.tar` & `acb_mse-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    31896 2020-02-02 00:00:00.000000 acb_mse-1.0.2/Images/loss_curve_1.png
--rw-r--r--   0        0        0    43749 2020-02-02 00:00:00.000000 acb_mse-1.0.2/Images/loss_curve_2.png
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 acb_mse-1.0.2/src/acb_mse/ACBLoss.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 acb_mse-1.0.2/src/acb_mse/__init__.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 acb_mse-1.0.2/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 acb_mse-1.0.2/LICENSE
--rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 acb_mse-1.0.2/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 acb_mse-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     7956 2020-02-02 00:00:00.000000 acb_mse-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 acb_mse-1.0.3/__init__.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 acb_mse-1.0.3/acb_mse.py
+-rw-r--r--   0        0        0    31896 2020-02-02 00:00:00.000000 acb_mse-1.0.3/Images/loss_curve_1.png
+-rw-r--r--   0        0        0    43749 2020-02-02 00:00:00.000000 acb_mse-1.0.3/Images/loss_curve_2.png
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 acb_mse-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 acb_mse-1.0.3/LICENSE
+-rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 acb_mse-1.0.3/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 acb_mse-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7956 2020-02-02 00:00:00.000000 acb_mse-1.0.3/PKG-INFO
```

### Comparing `acb_mse-1.0.2/Images/loss_curve_1.png` & `acb_mse-1.0.3/Images/loss_curve_1.png`

 * *Files identical despite different names*

### Comparing `acb_mse-1.0.2/Images/loss_curve_2.png` & `acb_mse-1.0.3/Images/loss_curve_2.png`

 * *Files identical despite different names*

### Comparing `acb_mse-1.0.2/src/acb_mse/ACBLoss.py` & `acb_mse-1.0.3/acb_mse.py`

 * *Files identical despite different names*

### Comparing `acb_mse-1.0.2/LICENSE` & `acb_mse-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `acb_mse-1.0.2/README.md` & `acb_mse-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `acb_mse-1.0.2/pyproject.toml` & `acb_mse-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "acb_mse"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Adill Al-Ashgar", email="adillwmaa@gmail.com" },
 ]
 description = "Automatic-Class-Balanced MSE Loss for PyTorch (ACB-MSE) to combat class imbalanced datasets and stabilise fluctuating loss gradients."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `acb_mse-1.0.2/PKG-INFO` & `acb_mse-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acb_mse
-Version: 1.0.2
+Version: 1.0.3
 Summary: Automatic-Class-Balanced MSE Loss for PyTorch (ACB-MSE) to combat class imbalanced datasets and stabilise fluctuating loss gradients.
 Project-URL: Homepage, https://github.com/Adillwma/ACB-MSE
 Project-URL: Bug Tracker, https://github.com/Adillwma/ACB-MSE/issues
 Author-email: Adill Al-Ashgar <adillwmaa@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

