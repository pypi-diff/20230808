# Comparing `tmp/prcv-1.0.1.tar.gz` & `tmp/prcv-1.0.2.tar.gz`

## Comparing `prcv-1.0.1.tar` & `prcv-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 prcv-1.0.1/demo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 prcv-1.0.1/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 prcv-1.0.1/src/prcv/__init__.py
--rw-r--r--   0        0        0    21223 2020-02-02 00:00:00.000000 prcv-1.0.1/src/prcv/methods.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 prcv-1.0.1/src/prcv/misc.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 prcv-1.0.1/src/prcv/scale.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 prcv-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 prcv-1.0.1/tests/common.py
--rw-r--r--   0        0        0     7654 2020-02-02 00:00:00.000000 prcv-1.0.1/tests/test_misc.py
--rw-r--r--   0        0        0     8508 2020-02-02 00:00:00.000000 prcv-1.0.1/tests/test_pcvpca.py
--rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 prcv-1.0.1/tests/test_pcvpcr.py
--rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 prcv-1.0.1/tests/test_pcvpls.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 prcv-1.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 prcv-1.0.1/LICENSE
--rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 prcv-1.0.1/README.md
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 prcv-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5466 2020-02-02 00:00:00.000000 prcv-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0  1013223 2020-02-02 00:00:00.000000 prcv-1.0.2/demo/corn.csv
+-rw-r--r--   0        0        0   376554 2020-02-02 00:00:00.000000 prcv-1.0.2/demo/demo.ipynb
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 prcv-1.0.2/demo/demo.py
+-rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 prcv-1.0.2/demo/misc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 prcv-1.0.2/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 prcv-1.0.2/src/prcv/__init__.py
+-rw-r--r--   0        0        0    21223 2020-02-02 00:00:00.000000 prcv-1.0.2/src/prcv/methods.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 prcv-1.0.2/src/prcv/misc.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 prcv-1.0.2/src/prcv/scale.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 prcv-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 prcv-1.0.2/tests/common.py
+-rw-r--r--   0        0        0     7654 2020-02-02 00:00:00.000000 prcv-1.0.2/tests/test_misc.py
+-rw-r--r--   0        0        0     8508 2020-02-02 00:00:00.000000 prcv-1.0.2/tests/test_pcvpca.py
+-rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 prcv-1.0.2/tests/test_pcvpcr.py
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 prcv-1.0.2/tests/test_pcvpls.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 prcv-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 prcv-1.0.2/LICENSE
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 prcv-1.0.2/README.md
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 prcv-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 prcv-1.0.2/PKG-INFO
```

### Comparing `prcv-1.0.1/src/prcv/methods.py` & `prcv-1.0.2/src/prcv/methods.py`

 * *Files identical despite different names*

### Comparing `prcv-1.0.1/src/prcv/misc.py` & `prcv-1.0.2/src/prcv/misc.py`

 * *Files identical despite different names*

### Comparing `prcv-1.0.1/tests/common.py` & `prcv-1.0.2/tests/common.py`

 * *Files identical despite different names*

### Comparing `prcv-1.0.1/tests/test_misc.py` & `prcv-1.0.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `prcv-1.0.1/tests/test_pcvpca.py` & `prcv-1.0.2/tests/test_pcvpca.py`

 * *Files identical despite different names*

### Comparing `prcv-1.0.1/tests/test_pcvpcr.py` & `prcv-1.0.2/tests/test_pcvpcr.py`

 * *Files identical despite different names*

### Comparing `prcv-1.0.1/tests/test_pcvpls.py` & `prcv-1.0.2/tests/test_pcvpls.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,19 +56,19 @@
     # make predictions for a = 1...ncomp components in a model
     for a in range(1, ncomp + 1):
         Pa = P[..., :a]
         Ca = C[..., :a]
 
         Tpva = Tpv[..., :a]
         Upva = Upv[..., :a]
-        Epva = Xpv - np.dot(Tpva, np.transpose(Pa))
+        Epva = Xpv - np.dot(Tpva, Pa.T)
 
         Qpv[..., a - 1] = (Epva * Epva).sum(axis = 1)
         Hpv[..., a - 1] = (Upva * Upva).sum(axis = 1)
-        Ypv[..., a - 1] = np.dot(Tpva, np.transpose(Ca)).flatten()
+        Ypv[..., a - 1] = np.dot(Tpva, Ca.T).flatten()
 
 
     Ypv = Ypv * sY + mY
     Epv = Ypv - Y
 
     return {'Yp': Ypv, 'T': Tpv, 'H': Hpv, 'Q': Qpv, 'RMSE': np.sqrt((Epv * Epv).mean(axis = 0))}
```

### Comparing `prcv-1.0.1/LICENSE` & `prcv-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prcv-1.0.1/README.md` & `prcv-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Procrustes cross-validation for Python
 
 Package `prcv` implements [Procrustes cross-validation](https://github.com/svkucheryavski/pcv) in Python language.
 
-Last version of the package (*1.0.0*) was released 8th of August, 2023 and contains small improvements, better test coverage, as well as a new experimental feature — CV scope. See details in the overall [project description](https://github.com/svkucheryavski/pcv).
+Last version of the package (*1.0.0*) was released 12th of August, 2023 and contains small improvements, better test coverage, as well as a new experimental feature — CV scope. See details in the overall [project description](https://github.com/svkucheryavski/pcv).
 
 ## Getting started
 
 You can install the package directly from PyPI by running `pip install prcv`. If you already have the package installed and want to upgrade it to the newest version use: `pip install prcv --upgrade`
 
 There are three main functions in the package:
 
@@ -14,15 +14,15 @@
 
 * `pcvpcr()` is implementation of PCV for PCR models.
 
 * `pcvpls()` is implementation of PCV for PLS models.
 
 All three functions return PV-set generated with given parameters. The PV-set has the same size as the calibration set. In case of regression (PCR or PLS) PV-set is generated only for predictors (X), the response values for PV-set are the same as for the calibration set.
 
-The last two functions return the PV-set and an additional outcome, `D`, which is a matrix (2D Numpy array) containing scaling factors ($c_k/c$), for each segment and each component. See all details in the [paper](https://doi.org/10.1016/j.aca.2023.341096).
+The last two functions return the PV-set and an additional outcome, `D`, which is a matrix (2D Numpy array) containing scaling factors ($c_k/c$), for each segment and each component. See all details in [the paper](https://doi.org/10.1016/j.aca.2023.341096).
 
 Below are examples of the function syntax with main parameters:
 
 ```python
 from prcv.methods import pcvpca, pcvpcr, pcvpls
 
 # set cross-validation settings — common for all methods above
@@ -53,12 +53,15 @@
 As it is written above there is also additional parameter, `cvscope`, which can have one of the two values, `'global'` or `'local'`. The default value is `'global'`, if you want to try the local scope, just add this parameter when you call one of the functions, like shown below (in this example some of the arguments are skipped for simplicity):
 
 ```r
 # PCV for PLS models with local CV scope
 Xpv, D = pcvpls(X, Y, ncomp = 20,  cv = {'type': 'ven', 'nseg': 4}, cvscope = 'local')
 ```
 
-File `demo.py`, which you can download from [GitHub repository](https://github.com/svkucheryavski/pcv/Python) contains a demo code based on *Corn* dataset from the [published paper](https://doi.org/10.1016/j.aca.2023.341096). See comments in the code for more details.
+Directory `demo`, which is available from [GitHub repository](https://github.com/svkucheryavski/pcv/Python), contains several files with dataset and demo code. Thus file `corn.csv` contains *Corn* dataset used in [the paper](https://doi.org/10.1016/j.aca.2023.341096) in Coma Separated Values format. File `demo.py` contains script with demo code and file `demo.ipynb` contains the same code but made as a Jupyter notebook. File `misc.py` contains several helper functions for the demo code, which are used in both the script and the notebook.
+
+Download all files and make sure all files are located in the same folder in order to run the code.
+
 
 The package code will be improved and extended gradually. If you found a bug please report using [issues](https://github.com/svkucheryavski/pcv/issues) or send an email.
```

### Comparing `prcv-1.0.1/pyproject.toml` & `prcv-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "numpy", "scipy"]
 build-backend = "hatchling.build"
 
 [project]
 name = "prcv"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Sergey Kucheryavskiy", email="svkucheryavski@gmail.com" },
 ]
 description = "Implementation of Procrustes cross-validation in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `prcv-1.0.1/PKG-INFO` & `prcv-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prcv
-Version: 1.0.1
+Version: 1.0.2
 Summary: Implementation of Procrustes cross-validation in Python
 Project-URL: Homepage, https://github.com/svkucheryavski/pcv
 Project-URL: Bug Tracker, https://github.com/svkucheryavski/pcv/issues
 Author-email: Sergey Kucheryavskiy <svkucheryavski@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Procrustes cross-validation for Python
 
 Package `prcv` implements [Procrustes cross-validation](https://github.com/svkucheryavski/pcv) in Python language.
 
-Last version of the package (*1.0.0*) was released 8th of August, 2023 and contains small improvements, better test coverage, as well as a new experimental feature — CV scope. See details in the overall [project description](https://github.com/svkucheryavski/pcv).
+Last version of the package (*1.0.0*) was released 12th of August, 2023 and contains small improvements, better test coverage, as well as a new experimental feature — CV scope. See details in the overall [project description](https://github.com/svkucheryavski/pcv).
 
 ## Getting started
 
 You can install the package directly from PyPI by running `pip install prcv`. If you already have the package installed and want to upgrade it to the newest version use: `pip install prcv --upgrade`
 
 There are three main functions in the package:
 
@@ -28,15 +28,15 @@
 
 * `pcvpcr()` is implementation of PCV for PCR models.
 
 * `pcvpls()` is implementation of PCV for PLS models.
 
 All three functions return PV-set generated with given parameters. The PV-set has the same size as the calibration set. In case of regression (PCR or PLS) PV-set is generated only for predictors (X), the response values for PV-set are the same as for the calibration set.
 
-The last two functions return the PV-set and an additional outcome, `D`, which is a matrix (2D Numpy array) containing scaling factors ($c_k/c$), for each segment and each component. See all details in the [paper](https://doi.org/10.1016/j.aca.2023.341096).
+The last two functions return the PV-set and an additional outcome, `D`, which is a matrix (2D Numpy array) containing scaling factors ($c_k/c$), for each segment and each component. See all details in [the paper](https://doi.org/10.1016/j.aca.2023.341096).
 
 Below are examples of the function syntax with main parameters:
 
 ```python
 from prcv.methods import pcvpca, pcvpcr, pcvpls
 
 # set cross-validation settings — common for all methods above
@@ -67,12 +67,15 @@
 As it is written above there is also additional parameter, `cvscope`, which can have one of the two values, `'global'` or `'local'`. The default value is `'global'`, if you want to try the local scope, just add this parameter when you call one of the functions, like shown below (in this example some of the arguments are skipped for simplicity):
 
 ```r
 # PCV for PLS models with local CV scope
 Xpv, D = pcvpls(X, Y, ncomp = 20,  cv = {'type': 'ven', 'nseg': 4}, cvscope = 'local')
 ```
 
-File `demo.py`, which you can download from [GitHub repository](https://github.com/svkucheryavski/pcv/Python) contains a demo code based on *Corn* dataset from the [published paper](https://doi.org/10.1016/j.aca.2023.341096). See comments in the code for more details.
+Directory `demo`, which is available from [GitHub repository](https://github.com/svkucheryavski/pcv/Python), contains several files with dataset and demo code. Thus file `corn.csv` contains *Corn* dataset used in [the paper](https://doi.org/10.1016/j.aca.2023.341096) in Coma Separated Values format. File `demo.py` contains script with demo code and file `demo.ipynb` contains the same code but made as a Jupyter notebook. File `misc.py` contains several helper functions for the demo code, which are used in both the script and the notebook.
+
+Download all files and make sure all files are located in the same folder in order to run the code.
+
 
 The package code will be improved and extended gradually. If you found a bug please report using [issues](https://github.com/svkucheryavski/pcv/issues) or send an email.
```

