# Comparing `tmp/acb_mse-1.0.1.tar.gz` & `tmp/acb_mse-1.0.2.tar.gz`

## Comparing `acb_mse-1.0.1.tar` & `acb_mse-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    31896 2020-02-02 00:00:00.000000 acb_mse-1.0.1/Images/loss_curve_1.png
--rw-r--r--   0        0        0    43749 2020-02-02 00:00:00.000000 acb_mse-1.0.1/Images/loss_curve_2.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 acb_mse-1.0.1/src/acb_mse/__init__.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 acb_mse-1.0.1/src/acb_mse/acb_mse.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 acb_mse-1.0.1/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 acb_mse-1.0.1/LICENSE
--rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 acb_mse-1.0.1/README.md
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 acb_mse-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     7956 2020-02-02 00:00:00.000000 acb_mse-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    31896 2020-02-02 00:00:00.000000 acb_mse-1.0.2/Images/loss_curve_1.png
+-rw-r--r--   0        0        0    43749 2020-02-02 00:00:00.000000 acb_mse-1.0.2/Images/loss_curve_2.png
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 acb_mse-1.0.2/src/acb_mse/ACBLoss.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 acb_mse-1.0.2/src/acb_mse/__init__.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 acb_mse-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 acb_mse-1.0.2/LICENSE
+-rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 acb_mse-1.0.2/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 acb_mse-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7956 2020-02-02 00:00:00.000000 acb_mse-1.0.2/PKG-INFO
```

### Comparing `acb_mse-1.0.1/Images/loss_curve_1.png` & `acb_mse-1.0.2/Images/loss_curve_1.png`

 * *Files identical despite different names*

### Comparing `acb_mse-1.0.1/Images/loss_curve_2.png` & `acb_mse-1.0.2/Images/loss_curve_2.png`

 * *Files identical despite different names*

### Comparing `acb_mse-1.0.1/src/acb_mse/acb_mse.py` & `acb_mse-1.0.2/src/acb_mse/ACBLoss.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 
-class acb_mse(torch.nn.Module):
+class ACBLoss(torch.nn.Module):
     def __init__(self, zero_weighting=1, nonzero_weighting=1):
         """
         Initializes the ACB-MSE Loss Function class with weighting coefficients.
 
         Args:
         - zero_weighting: a scalar weighting coefficient for the MSE loss of zero pixels
         - nonzero_weighting: a scalar weighting coefficient for the MSE loss of non-zero pixels
@@ -44,23 +44,7 @@
         if torch.isnan(nonzero_loss):
             nonzero_loss = 0
 
         weighted_mse_loss = (self.zero_weighting * zero_loss) + (self.nonzero_weighting * nonzero_loss)
 
         return float(weighted_mse_loss)
 
-
-
-# Select weighting for each class if not wanting to use the defualt 1:1 weighting
-zero_weighting = 1.0
-nonzero_weighting = 1.2
-
-# Create an instance of the ACBMSE loss function with specified weighting coefficients
-loss_function = acb_mse(zero_weighting, nonzero_weighting)
-
-# Dummy target image and reconstructed image tensors (assuming B=10, C=3, H=256, W=256)
-target_image = torch.rand(10, 3, 256, 256)
-reconstructed_image = torch.rand(10, 3, 256, 256)
-
-# Calculate the ACBMSE loss
-loss = loss_function(reconstructed_image, target_image)
-print("ACB-MSE Loss:", loss)
```

### Comparing `acb_mse-1.0.1/LICENSE` & `acb_mse-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `acb_mse-1.0.1/README.md` & `acb_mse-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `acb_mse-1.0.1/pyproject.toml` & `acb_mse-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "acb_mse"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Adill Al-Ashgar", email="adillwmaa@gmail.com" },
 ]
 description = "Automatic-Class-Balanced MSE Loss for PyTorch (ACB-MSE) to combat class imbalanced datasets and stabilise fluctuating loss gradients."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+install_requires=[
+    'torch>=2.0',  
+]
+
 [project.urls]
 "Homepage" = "https://github.com/Adillwma/ACB-MSE"
 "Bug Tracker" = "https://github.com/Adillwma/ACB-MSE/issues"
```

### Comparing `acb_mse-1.0.1/PKG-INFO` & `acb_mse-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acb_mse
-Version: 1.0.1
+Version: 1.0.2
 Summary: Automatic-Class-Balanced MSE Loss for PyTorch (ACB-MSE) to combat class imbalanced datasets and stabilise fluctuating loss gradients.
 Project-URL: Homepage, https://github.com/Adillwma/ACB-MSE
 Project-URL: Bug Tracker, https://github.com/Adillwma/ACB-MSE/issues
 Author-email: Adill Al-Ashgar <adillwmaa@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

