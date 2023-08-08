# Comparing `tmp/slise-2.1.3.tar.gz` & `tmp/slise-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slise-2.1.3.tar", last modified: Mon Aug 29 12:42:02 2022, max compression
+gzip compressed data, was "slise-2.2.0.tar", last modified: Tue Aug  8 11:30:59 2023, max compression
```

## Comparing `slise-2.1.3.tar` & `slise-2.2.0.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 12:42:02.907203 slise-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-08-29 12:41:52.000000 slise-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5441 2022-08-29 12:42:02.907203 slise-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4682 2022-08-29 12:41:52.000000 slise-2.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-29 12:41:52.000000 slise-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      997 2022-08-29 12:42:02.907203 slise-2.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 12:42:02.907203 slise-2.1.3/slise/
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-08-29 12:41:52.000000 slise-2.1.3/slise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10496 2022-08-29 12:41:52.000000 slise-2.1.3/slise/data.py
--rw-r--r--   0 runner    (1001) docker     (121)    12598 2022-08-29 12:41:52.000000 slise-2.1.3/slise/initialisation.py
--rw-r--r--   0 runner    (1001) docker     (121)    19449 2022-08-29 12:41:52.000000 slise-2.1.3/slise/optimisation.py
--rw-r--r--   0 runner    (1001) docker     (121)    25001 2022-08-29 12:41:52.000000 slise-2.1.3/slise/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)    42978 2022-08-29 12:41:52.000000 slise-2.1.3/slise/slise.py
--rw-r--r--   0 runner    (1001) docker     (121)     3738 2022-08-29 12:41:52.000000 slise-2.1.3/slise/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 12:42:02.907203 slise-2.1.3/slise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5441 2022-08-29 12:42:02.000000 slise-2.1.3/slise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-08-29 12:42:02.000000 slise-2.1.3/slise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-29 12:42:02.000000 slise-2.1.3/slise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-29 12:42:02.000000 slise-2.1.3/slise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-08-29 12:42:02.000000 slise-2.1.3/slise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:30:59.217317 slise-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-08 11:30:49.000000 slise-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-08-08 11:30:59.217317 slise-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-08-08 11:30:49.000000 slise-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-08-08 11:30:49.000000 slise-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 11:30:59.217317 slise-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:30:59.217317 slise-2.2.0/slise/
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-08-08 11:30:49.000000 slise-2.2.0/slise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10496 2023-08-08 11:30:49.000000 slise-2.2.0/slise/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-08-08 11:30:49.000000 slise-2.2.0/slise/initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19449 2023-08-08 11:30:49.000000 slise-2.2.0/slise/optimisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-08-08 11:30:49.000000 slise-2.2.0/slise/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42974 2023-08-08 11:30:49.000000 slise-2.2.0/slise/slise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-08-08 11:30:49.000000 slise-2.2.0/slise/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:30:59.217317 slise-2.2.0/slise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-08-08 11:30:59.000000 slise-2.2.0/slise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-08 11:30:59.000000 slise-2.2.0/slise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 11:30:59.000000 slise-2.2.0/slise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-08 11:30:59.000000 slise-2.2.0/slise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 11:30:59.000000 slise-2.2.0/slise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:30:59.217317 slise-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-08-08 11:30:49.000000 slise-2.2.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-08-08 11:30:49.000000 slise-2.2.0/tests/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-08-08 11:30:49.000000 slise-2.2.0/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-08-08 11:30:49.000000 slise-2.2.0/tests/test_slise.py
```

### Comparing `slise-2.1.3/LICENSE` & `slise-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slise-2.1.3/PKG-INFO` & `slise-2.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,37 @@
-Metadata-Version: 2.1
-Name: slise
-Version: 2.1.3
-Summary: The SLISE algorithm for robust regression and explanations of black box models
-Home-page: https://github.com/edahelsinki/pyslise
-Author: Anton Björklund
-Author-email: anton.bjorklund@helsinki.fi
-License: MIT
-Keywords: Robust regression,Sparse Linear Regression,Explainable Artificial Intelligence,Local Explanations
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: tbb
-License-File: LICENSE
-
 ![PySLISE Banner Image](docs/pyslise_banner.webp)  
 [![PyPI](https://img.shields.io/pypi/v/slise)](https://pypi.org/project/slise/)
 [![Documentation](https://github.com/edahelsinki/pyslise/actions/workflows/python-docs.yml/badge.svg)](https://edahelsinki.github.io/pyslise/docs/slise/)
 [![Tests](https://github.com/edahelsinki/pyslise/actions/workflows/python-pytest.yml/badge.svg)](https://github.com/edahelsinki/pyslise/actions/workflows/python-pytest.yml)
 [![License: MIT](https://img.shields.io/github/license/edahelsinki/pyslise)](https://github.com/edahelsinki/pyslise/blob/master/LICENSE)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/edahelsinki/pyslise/HEAD?labpath=examples)
 
 # SLISE - Sparse Linear Subset Explanations
 
 Python implementation of the SLISE algorithm. The SLISE algorithm can be used for both robust regression and to explain outcomes from black box models.
-For more details see [the original paper](https://rdcu.be/bVbda) or [the robust regression paper](https://rdcu.be/cFRHD).
+For more details see the [conference paper](https://rdcu.be/bVbda), the [robust regression paper](https://rdcu.be/cFRHD), or the [local explanation paper](https://doi.org/10.3389/fcomp.2023.1143904).
 Alternatively for a more informal overview see [the presentation](https://github.com/edahelsinki/slise/raw/master/vignettes/presentation.pdf), or [the poster](https://github.com/edahelsinki/slise/raw/master/vignettes/poster.pdf).
 Finally, for learning to use the python package there are several [examples](https://github.com/edahelsinki/pyslise/tree/master/examples/) and [the documentation](https://edahelsinki.github.io/pyslise/docs/slise/).
 
 > *Björklund A., Henelius A., Oikarinen E., Kallonen K., Puolamäki K.* (2019)  
 > **Sparse Robust Regression for Explaining Classifiers.**  
 > Discovery Science (DS 2019).  
 > Lecture Notes in Computer Science, vol 11828, Springer.  
 > https://doi.org/10.1007/978-3-030-33778-0_27  
 
 > *Björklund A., Henelius A., Oikarinen E., Kallonen K., Puolamäki K.* (2022).  
 > **Robust regression via error tolerance.**  
 > Data Mining and Knowledge Discovery.  
 > https://doi.org/10.1007/s10618-022-00819-2  
 
+> *Björklund A., Henelius A., Oikarinen E., Kallonen K., Puolamäki K.* (2023)  
+> **Explaining any black box model using real data.**  
+> Frontiers in Computer Science 5:1143904.  
+> https://doi.org/10.3389/fcomp.2023.1143904  
+
 ## The idea
 
 In robust regression we fit regression models that can handle data that contains outliers (see the example below for why outliers are problematic for normal regression). SLISE accomplishes this by fitting a model such that the largest possible subset of the data items have an error less than a given value. All items with an error larger than that are considered potential outliers and do not affect the resulting model.
 
 SLISE can also be used to provide *local model-agnostic explanations* for outcomes from black box models. To do this we replace the ground truth response vector with the predictions from the complex model. Furthermore, we force the model to fit a selected item (making the explanation local). This gives us a local approximation of the complex model with a simpler linear model (this is similar to, e.g., [LIME](https://github.com/marcotcr/lime) and [SHAP](https://github.com/slundberg/shap)). In contrast to other methods SLISE creates explanations using real data (not some discretised and randomly sampled data) so we can be sure that all inputs are valid (i.e. in the correct data manifold, and follows the constraints used to generate the data, e.g., the laws of physics).
 
 ## Installation
```

### Comparing `slise-2.1.3/slise/__init__.py` & `slise-2.2.0/slise/__init__.py`

 * *Files identical despite different names*

### Comparing `slise-2.1.3/slise/data.py` & `slise-2.2.0/slise/data.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -79,47 +79,14 @@
         return X2
     else:
         X2 = np.zeros((X.shape[0], len(mask)), X.dtype)
         X2[:, mask] = X
         return X2
 
 
-def unscale_model(
-    model: np.ndarray,
-    x_center: np.ndarray,
-    x_scale: np.ndarray,
-    y_center: float = 0.0,
-    y_scale: float = 1.0,
-    columns: Optional[np.ndarray] = None,
-) -> np.ndarray:
-    """Scale a linear model such that it matches unnormalised data.
-
-    Args:
-        model (np.ndarray): The model for normalised data.
-        x_center (np.ndarray): The center used for normalising X.
-        x_scale (np.ndarray): The scale used for normalising X.
-        y_center (float, optional): The scale used for normalising y. Defaults to 0.0.
-        y_scale (float, optional): The center used for normalising y. Defaults to 1.0.
-        columns (Optional[np.ndarray], optional): Mask of removed columns (see remove_constant_columns). Defaults to None.
-
-    Returns:
-        np.ndarray: The unscaled model.
-    """
-    if len(model) == len(x_center):
-        model = np.concatenate((np.zeros(1, x_center.dtype), model))
-    else:
-        model = model.copy()
-    model[0] = (model[0] - np.sum(model[1:] * x_center / x_scale)) * y_scale + y_center
-    model[1:] = model[1:] / x_scale * y_scale
-    if columns is not None:
-        return add_constant_columns(model, columns, True)
-    else:
-        return model
-
-
 def normalise_robust(
     x: np.ndarray, epsilon: Optional[float] = None
 ) -> Tuple[np.ndarray, Union[float, np.ndarray], Union[float, np.ndarray]]:
     """A robust version of normalisation that uses median and mad (median absolute deviation).
         Any zeros in the scale are replaced by ones to avoid division by zero.
 
     Args:
@@ -181,14 +148,47 @@
                     x[:, constant_colums] - center[None, :]
                 ) / scale[None, :]
                 return y
             x = x[:, constant_colums]
         return (x - center[None, :]) / scale[None, :]
 
 
+def unscale_model(
+    model: np.ndarray,
+    x_center: np.ndarray,
+    x_scale: np.ndarray,
+    y_center: float = 0.0,
+    y_scale: float = 1.0,
+    columns: Optional[np.ndarray] = None,
+) -> np.ndarray:
+    """Scale a linear model such that it matches unnormalised data.
+
+    Args:
+        model (np.ndarray): The model for normalised data.
+        x_center (np.ndarray): The center used for normalising X.
+        x_scale (np.ndarray): The scale used for normalising X.
+        y_center (float, optional): The scale used for normalising y. Defaults to 0.0.
+        y_scale (float, optional): The center used for normalising y. Defaults to 1.0.
+        columns (Optional[np.ndarray], optional): Mask of removed columns (see remove_constant_columns). Defaults to None.
+
+    Returns:
+        np.ndarray: The unscaled model.
+    """
+    if len(model) == len(x_center):
+        model = np.concatenate((np.zeros(1, x_center.dtype), model))
+    else:
+        model = model.copy()
+    model[0] = (model[0] - np.sum(model[1:] * x_center / x_scale)) * y_scale + y_center
+    model[1:] = model[1:] / x_scale * y_scale
+    if columns is not None:
+        return add_constant_columns(model, columns, True)
+    else:
+        return model
+
+
 class DataScaling(NamedTuple):
     """
     Container class for scaling information
     """
 
     x_center: np.ndarray
     x_scale: np.ndarray
```

### Comparing `slise-2.1.3/slise/initialisation.py` & `slise-2.2.0/slise/initialisation.py`

 * *Files identical despite different names*

### Comparing `slise-2.1.3/slise/optimisation.py` & `slise-2.2.0/slise/optimisation.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -480,56 +480,14 @@
     epss = matching_epsilon(residuals, epsilon**2, beta, weight)
     beta = beta * epsilon**2
     print(
         f"beta: {beta:5.3f}    epsilon*: {epss:.3f}    Loss: {loss:6.2f}    B-Loss: {bloss:6.2f}"
     )
 
 
-def set_threads(num: int = -1) -> int:
-    """Set the number of numba threads.
-
-    Args:
-        num (int, optional): The number of threads. Defaults to -1.
-
-    Returns:
-        int: The old number of theads (or -1 if unchanged).
-    """
-    if num > 0:
-        old = get_num_threads()
-        if old != num:
-            set_num_threads(num)
-        return old
-    return -1
-
-
-@jit(nopython=True, fastmath=True, parallel=True, cache=True)
-def _dummy_numba(
-    x: np.ndarray,
-) -> np.ndarray:
-    """
-    A dummy function to check the numba compilation (see check_threading_layer).
-    """
-    return x * x
-
-
-def check_threading_layer():
-    """
-    Check which numba threading_layer is active, and warn if it is "workqueue".
-    """
-    _dummy_numba(np.ones(1))
-    try:
-        if threading_layer() == "workqueue":
-            warn(
-                'Using `numba.threading_layer()=="workqueue"` can be devastatingly slow! See https://numba.pydata.org/numba-doc/latest/user/threading-layer.html for alternatives.',
-                SliseWarning,
-            )
-    except ValueError as e:
-        warn(f"Numba: {e}", SliseWarning)
-
-
 @np.errstate(over="ignore")
 def graduated_optimisation(
     alpha: np.ndarray,
     X: np.ndarray,
     Y: np.ndarray,
     epsilon: float,
     beta: float = 0,
@@ -580,7 +538,49 @@
         alpha, X, Y, epsilon, beta, lambda1, lambda2, weight, max_iterations * 4
     )
     if debug:
         _debug_log(alpha, X, Y, epsilon, beta, lambda1, lambda2, weight)
         if w:
             print("Warnings from intermediate steps:", w)
     return alpha
+
+
+def set_threads(num: int = -1) -> int:
+    """Set the number of numba threads.
+
+    Args:
+        num (int, optional): The number of threads. Defaults to -1.
+
+    Returns:
+        int: The old number of theads (or -1 if unchanged).
+    """
+    if num > 0:
+        old = get_num_threads()
+        if old != num:
+            set_num_threads(num)
+        return old
+    return -1
+
+
+@jit(nopython=True, fastmath=True, parallel=True, cache=True)
+def _dummy_numba(
+    x: np.ndarray,
+) -> np.ndarray:
+    """
+    A dummy function to check the numba compilation (see check_threading_layer).
+    """
+    return x * x
+
+
+def check_threading_layer():
+    """
+    Check which numba threading_layer is active, and warn if it is "workqueue".
+    """
+    _dummy_numba(np.ones(1))
+    try:
+        if threading_layer() == "workqueue":
+            warn(
+                'Using `numba.threading_layer()=="workqueue"` can be devastatingly slow! See https://numba.pydata.org/numba-doc/latest/user/threading-layer.html for alternatives.',
+                SliseWarning,
+            )
+    except ValueError as e:
+        warn(f"Numba: {e}", SliseWarning)
```

### Comparing `slise-2.1.3/slise/plot.py` & `slise-2.2.0/slise/plot.py`

 * *Files 16% similar despite different names*

```diff
@@ -158,18 +158,18 @@
     epsilon: float,
     variables: Optional[List[str]] = None,
     title: str = "SLISE",
     decimals: int = 3,
     num_var: int = 10,
     unscaled: Optional[np.ndarray] = None,
     unscaled_y: Union[None, float] = None,
-    impact: Optional[np.ndarray] = None,
+    terms: Optional[np.ndarray] = None,
     scaled: Optional[np.ndarray] = None,
     alpha: Optional[np.ndarray] = None,
-    scaled_impact: Optional[np.ndarray] = None,
+    scaled_terms: Optional[np.ndarray] = None,
     classes: Optional[List[str]] = None,
     unscaled_preds: Optional[np.ndarray] = None,
     logit: bool = False,
 ):
     """Print the results from SLISE.
 
     Args:
@@ -180,39 +180,39 @@
         epsilon (float): (Unscaled) error tolerance.
         variables (Optional[List[str]], optional): Variable names. Defaults to None.
         title (str, optional): Title to print first. Defaults to "SLISE".
         decimals (int, optional): Number of decimals to print. Defaults to 3.
         num_var (int, optional): Exclude zero weights if there are too many variables. Defaults to 10.
         unscaled (Optional[np.ndarray], optional): Unscaled x (explained item). Defaults to None.
         unscaled_y (Union[None, float], optional): Unscaled y (explained outcome). Defaults to None.
-        impact (Optional[np.ndarray], optional): Unscaled impact (coefficients * x). Defaults to None.
+        terms (Optional[np.ndarray], optional): Unscaled terms (coefficients * x). Defaults to None.
         scaled (Optional[np.ndarray], optional): Scaled x (explained item). Defaults to None.
         alpha (Optional[np.ndarray], optional): Scaled model. Defaults to None.
-        scaled_impact (Optional[np.ndarray], optional): Scaled impact (alpha * scaled_x). Defaults to None.
+        scaled_terms (Optional[np.ndarray], optional): Scaled terms (alpha * scaled_x). Defaults to None.
         classes (Optional[List[str]], optional): Class names (if applicable). Defaults to None.
         unscaled_preds (Optional[np.ndarray], optional): Unscaled resonse (Y-vector). Defaults to None.
         logit (bool, optional): A logit transformation has been applied. Defaults to False.
     """
     rows = OrderedDict()
     rows["Variable Names:    "] = fill_column_names(
         variables, len(coefficients) - intercept, intercept
     )
     if unscaled is not None:
         rows["Explained Item:"] = [""] + ["%%.%df" % decimals % a for a in unscaled]
         rows["Model Weights:"] = ["%%.%df" % decimals % a for a in coefficients]
     else:
         rows["Coefficients:"] = ["%%.%df" % decimals % a for a in coefficients]
-    if impact is not None:
-        rows["Prediction Impact:"] = ["%%.%df" % decimals % a for a in impact]
+    if terms is not None:
+        rows["Prediction Term:"] = ["%%.%df" % decimals % a for a in terms]
     if scaled is not None:
         rows["Normalised Item:"] = [""] + ["%%.%df" % decimals % a for a in scaled]
     if alpha is not None:
         rows["Normalised Weights:"] = ["%%.%df" % decimals % a for a in alpha]
-    if scaled_impact is not None:
-        rows["Normalised Impact:"] = ["%%.%df" % decimals % a for a in scaled_impact]
+    if scaled_terms is not None:
+        rows["Normalised Term:"] = ["%%.%df" % decimals % a for a in scaled_terms]
     col_len = [
         max(8, *vs) + 1
         for vs in zip(*(tuple(len(v) for v in vs) for vs in rows.values()))
     ]
     if len(coefficients) > num_var:
         col_len = [l if c != 0 else 0 for l, c in zip(col_len, coefficients)]
     lab_len = max(len(l) for l in rows)
@@ -332,16 +332,16 @@
     X: np.ndarray,
     Y: np.ndarray,
     model: np.ndarray,
     subset: np.ndarray,
     alpha: Optional[np.ndarray] = None,
     x: Optional[np.ndarray] = None,
     y: Optional[float] = None,
-    impact: Optional[np.ndarray] = None,
-    norm_impact: Optional[np.ndarray] = None,
+    terms: Optional[np.ndarray] = None,
+    norm_terms: Optional[np.ndarray] = None,
     title: str = "SLISE Explanation",
     variables: Optional[List[str]] = None,
     decimals: int = 3,
     fig: Optional[Figure] = None,
 ):
     """Plot the SLISE result with density distributions for the dataset and barplot for the model.
 
@@ -349,16 +349,16 @@
         X (np.ndarray): Data matrix.
         Y (np.ndarray): Response vector.
         model (np.ndarray): Linear model.
         subset (np.ndarray): Selected subset.
         alpha (Optional[np.ndarray]): Scaled model. Defaults to None.
         x (Optional[np.ndarray], optional): The explained item (if it is an explanation). Defaults to None.
         y (Optional[float], optional): The explained outcome (if it is an explanation). Defaults to None.
-        impact (Optional[np.ndarray], optional): Impact vector (unscaled x*alpha), if available. Defaults to None.
-        norm_impact (Optional[np.ndarray], optional): Impact vector (scaled x*alpha), if available. Defaults to None.
+        terms (Optional[np.ndarray], optional): Term vector (unscaled x*alpha), if available. Defaults to None.
+        norm_terms (Optional[np.ndarray], optional): Term vector (scaled x*alpha), if available. Defaults to None.
         title (str, optional): Title of the plot. Defaults to "SLISE Explanation".
         variables (Optional[List[str]], optional): Names for the (columns/) variables. Defaults to None.
         decimals (int, optional): Number of decimals when writing numbers. Defaults to 3.
         fig (Optional[Figure], optional): Pyplot figure to plot on, if None then a new plot is created and shown. Defaults to None.
     """
     # Values and order
     variables = fill_column_names(variables, X.shape[1], True)
@@ -370,18 +370,18 @@
     if len(model) == X.shape[1]:
         model = np.concatenate((np.zeros(1, model.dtype), model))
         alpha = np.concatenate((np.zeros(1, model.dtype), alpha))
         variables[0] = ""
     order = get_explanation_order(np.abs(alpha), True)
     model = model[order]
     alpha = alpha[order]
-    if impact is not None:
-        impact = impact[order]
-    if norm_impact is not None:
-        norm_impact = norm_impact[order]
+    if terms is not None:
+        terms = terms[order]
+    if norm_terms is not None:
+        norm_terms = norm_terms[order]
     variables = [variables[i] for i in order]
     subsize = subset.mean()
 
     # Figures:
     if isinstance(fig, Figure):
         plot = False
         axs = fig.subplots(len(order), 2, squeeze=False)
@@ -446,20 +446,20 @@
     else:
         axbig.set_title("Explanation")
     ticks = np.arange(len(variables))
     axbig.set_yticks(ticks)
     axbig.set_yticklabels(variables)
     axbig.set_ylim(bottom=ticks[0] - 0.45, top=ticks[-1] + 0.45)
     axbig.invert_yaxis()
-    if impact is None and noalpha:
+    if terms is None and noalpha:
         column_color = [SLISE_ORANGE if v < 0 else SLISE_PURPLE for v in alpha]
         axbig.barh(ticks, alpha, color=column_color)
         for y, v in zip(ticks, model):
             text(0, y, v)
-    elif impact is None and not noalpha:
+    elif terms is None and not noalpha:
         axbig.barh(
             ticks - 0.2,
             model / np.max(np.abs(model)),
             height=0.35,
             color=SLISE_PURPLE,
             label="Coefficients",
         )
@@ -471,15 +471,15 @@
             label="Normalised",
         )
         for y, a, m in zip(ticks, alpha, model):
             text(0, y, m)
             text(0, y, a)
         axbig.set_xticks([])
         axbig.legend()
-    elif norm_impact is None:
+    elif norm_terms is None:
         axbig.barh(
             ticks[1:] - 0.2,
             model[1:] / np.max(np.abs(model)),
             height=0.35,
             color=SLISE_PURPLE,
             label="Linear Model",
         )
@@ -487,20 +487,20 @@
             ticks[0],
             model[0] / np.max(np.abs(model)),
             height=0.35,
             color=SLISE_PURPLE,
         )
         axbig.barh(
             ticks[1:] + 0.2,
-            impact[1:] / np.max(np.abs(impact[1:])),
+            terms[1:] / np.max(np.abs(terms[1:])),
             height=0.35,
             color=SLISE_ORANGE,
-            label="Prediction Impact",
+            label="Prediction Term",
         )
-        for y, a, m in zip(ticks, impact, model):
+        for y, a, m in zip(ticks, terms, model):
             if y == ticks[0]:
                 text(0, y, m)
                 continue
             text(0, y - 0.2, m)
             text(0, y + 0.2, a)
         axbig.set_xticks([])
         axbig.legend()
@@ -529,27 +529,27 @@
             ticks[0] + 0.11,
             alpha[0] / np.max(np.abs(alpha)),
             height=0.2,
             color=SLISE_DARKPURPLE,
         )
         axbig.barh(
             ticks[1:] + 0.11,
-            impact[1:] / np.max(np.abs(impact[1:])),
+            terms[1:] / np.max(np.abs(terms[1:])),
             height=0.2,
             color=SLISE_ORANGE,
-            label="Prediction Impact",
+            label="Prediction Term",
         )
         axbig.barh(
             ticks[1:] + 0.33,
-            norm_impact[1:] / np.max(np.abs(norm_impact[1:])),
+            norm_terms[1:] / np.max(np.abs(norm_terms[1:])),
             height=0.2,
             color=SLISE_DARKORANGE,
-            label="Normalised Impact",
+            label="Normalised Term",
         )
-        for y, i1, i2, m1, m2 in zip(ticks, impact, norm_impact, model, alpha):
+        for y, i1, i2, m1, m2 in zip(ticks, terms, norm_terms, model, alpha):
             if y == ticks[0]:
                 text(0, y - 0.11, m1)
                 text(0, y + 0.11, m2)
                 continue
             text(0, y - 0.33, m1)
             text(0, y - 0.11, m2)
             text(0, y + 0.11, i1)
```

### Comparing `slise-2.1.3/slise/slise.py` & `slise-2.2.0/slise/slise.py`

 * *Files 2% similar despite different names*

```diff
@@ -865,35 +865,37 @@
             X = self._X
             Y = self._Y
         if self._logit:
             Y = limited_logit(Y)
         res = mat_mul_inter(X, self.coefficients) - Y
         return res**2 < self.scaled_epsilon**2
 
-    def get_impact(
+    def get_terms(
         self, normalised: bool = False, x: Union[None, np.ndarray] = None
     ) -> np.ndarray:
-        """Get the "impact" of different variables on the outcome.
-            The impact is the (normalised) model times the (normalised) item.
+        """Get the "terms" of different variables on the outcome.
+            The terms are the (normalised) coefficients times the (normalised) values.
 
         Args:
-            normalised (bool, optional): Return the normalised impact (if normalisation is used). Defaults to False.
-            x (Union[None, np.ndarray], optional): The item to calculate the impact for (uses the explained item if None). Defaults to None.
+            normalised (bool, optional): Return the normalised terms (if normalisation is used). Defaults to False.
+            x (Union[None, np.ndarray], optional): The item to calculate the terms for (uses the explained item if None). Defaults to None.
 
         Returns:
-            np.ndarray: The impact vector.
+            np.ndarray: The terms vector.
         """
         if x is None:
             x = self._x
         if normalised and self._normalise:
             x = add_constant_columns(self._scale.scale_x(x), self._scale.columns, False)
             return add_intercept_column(x) * self.coefficients
         else:
             return add_intercept_column(x) * self.coefficients
 
+    get_impact = get_terms
+
     def print(
         self,
         variables: Union[List[str], None] = None,
         classes: Union[List[str], None] = None,
         num_var: int = 10,
         decimals: int = 3,
     ):
@@ -913,18 +915,18 @@
             self.scaled_epsilon,
             variables,
             "SLISE Explanation",
             decimals,
             num_var,
             unscaled=self._x,
             unscaled_y=self._y,
-            impact=self.get_impact(False),
+            terms=self.get_terms(False),
             scaled=None if self._scale is None else self._scale.scale_x(self._x, False),
             alpha=self.normalised(),
-            scaled_impact=None if self._scale is None else self.get_impact(True),
+            scaled_terms=None if self._scale is None else self.get_terms(True),
             classes=classes,
             unscaled_preds=self._Y,
             logit=self._logit,
         )
 
     def plot_2d(
         self,
@@ -1001,20 +1003,16 @@
         title: str = "SLISE Explanation",
         variables: list = None,
         decimals: int = 3,
         fig: Union[Figure, None] = None,
     ) -> SliseExplainer:
         """Plot the current explanation with density distributions for the dataset and a barplot for the model.
 
-        The barbplot contains both the approximating linear model (where the
-        weights can be loosely interpreted as the importance of the different
-        variables and their sign) and the "impact" which is the (scaled) model
-        time the (scaled) item values (which demonstrates how the explained
-        item interacts with the approximating linear model, since a negative
-        weight times a negative value actually supports a positive prediction).
+        The barplot contains both the approximating linear model (where the weights can be loosely interpreted as the importance of the different variables and their sign) and the "terms", which is the (scaled) model time the (scaled) item values.
+        The terms demonstrates how the explained item interacts with the approximating linear model, since a negative weight times a negative value actually supports a positive prediction.
 
         Args:
             title (str, optional): Title of the plot. Defaults to "SLISE Explanation".
             variables (list, optional): Names for the variables. Defaults to None.
             decimals (int, optional): Number of decimals to write. Defaults to 3.
             fig (Union[Figure, None], optional): Pyplot figure to plot on, if None then a new plot is created and shown. Defaults to None.
         """
@@ -1022,16 +1020,16 @@
             self._X,
             self._Y,
             self.coefficients,
             self.subset(),
             self.normalised(),
             self._x,
             self._y,
-            self.get_impact(False),
-            self.get_impact(True) if self._normalise else None,
+            self.get_terms(False),
+            self.get_terms(True) if self._normalise else None,
             title,
             variables,
             decimals,
             fig,
         )
 
     def plot_subset(
```

### Comparing `slise-2.1.3/slise/utils.py` & `slise-2.2.0/slise/utils.py`

 * *Files identical despite different names*

### Comparing `slise-2.1.3/slise.egg-info/PKG-INFO` & `slise-2.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,79 @@
 Metadata-Version: 2.1
 Name: slise
-Version: 2.1.3
+Version: 2.2.0
 Summary: The SLISE algorithm for robust regression and explanations of black box models
-Home-page: https://github.com/edahelsinki/pyslise
-Author: Anton Björklund
-Author-email: anton.bjorklund@helsinki.fi
-License: MIT
+Author-email: Anton Björklund <anton.bjorklund@helsinki.fi>
+License: MIT License
+        
+        Copyright (c) 2022 Anton Björklund
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://edahelsinki.fi/pyslise
+Project-URL: documentation, https://edahelsinki.fi/pyslise/docs/slise/
+Project-URL: repository, https://github.com/edahelsinki/pyslise.git
 Keywords: Robust regression,Sparse Linear Regression,Explainable Artificial Intelligence,Local Explanations
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 Provides-Extra: tbb
 License-File: LICENSE
 
 ![PySLISE Banner Image](docs/pyslise_banner.webp)  
 [![PyPI](https://img.shields.io/pypi/v/slise)](https://pypi.org/project/slise/)
 [![Documentation](https://github.com/edahelsinki/pyslise/actions/workflows/python-docs.yml/badge.svg)](https://edahelsinki.github.io/pyslise/docs/slise/)
 [![Tests](https://github.com/edahelsinki/pyslise/actions/workflows/python-pytest.yml/badge.svg)](https://github.com/edahelsinki/pyslise/actions/workflows/python-pytest.yml)
 [![License: MIT](https://img.shields.io/github/license/edahelsinki/pyslise)](https://github.com/edahelsinki/pyslise/blob/master/LICENSE)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/edahelsinki/pyslise/HEAD?labpath=examples)
 
 # SLISE - Sparse Linear Subset Explanations
 
 Python implementation of the SLISE algorithm. The SLISE algorithm can be used for both robust regression and to explain outcomes from black box models.
-For more details see [the original paper](https://rdcu.be/bVbda) or [the robust regression paper](https://rdcu.be/cFRHD).
+For more details see the [conference paper](https://rdcu.be/bVbda), the [robust regression paper](https://rdcu.be/cFRHD), or the [local explanation paper](https://doi.org/10.3389/fcomp.2023.1143904).
 Alternatively for a more informal overview see [the presentation](https://github.com/edahelsinki/slise/raw/master/vignettes/presentation.pdf), or [the poster](https://github.com/edahelsinki/slise/raw/master/vignettes/poster.pdf).
 Finally, for learning to use the python package there are several [examples](https://github.com/edahelsinki/pyslise/tree/master/examples/) and [the documentation](https://edahelsinki.github.io/pyslise/docs/slise/).
 
 > *Björklund A., Henelius A., Oikarinen E., Kallonen K., Puolamäki K.* (2019)  
 > **Sparse Robust Regression for Explaining Classifiers.**  
 > Discovery Science (DS 2019).  
 > Lecture Notes in Computer Science, vol 11828, Springer.  
 > https://doi.org/10.1007/978-3-030-33778-0_27  
 
 > *Björklund A., Henelius A., Oikarinen E., Kallonen K., Puolamäki K.* (2022).  
 > **Robust regression via error tolerance.**  
 > Data Mining and Knowledge Discovery.  
 > https://doi.org/10.1007/s10618-022-00819-2  
 
+> *Björklund A., Henelius A., Oikarinen E., Kallonen K., Puolamäki K.* (2023)  
+> **Explaining any black box model using real data.**  
+> Frontiers in Computer Science 5:1143904.  
+> https://doi.org/10.3389/fcomp.2023.1143904  
+
 ## The idea
 
 In robust regression we fit regression models that can handle data that contains outliers (see the example below for why outliers are problematic for normal regression). SLISE accomplishes this by fitting a model such that the largest possible subset of the data items have an error less than a given value. All items with an error larger than that are considered potential outliers and do not affect the resulting model.
 
 SLISE can also be used to provide *local model-agnostic explanations* for outcomes from black box models. To do this we replace the ground truth response vector with the predictions from the complex model. Furthermore, we force the model to fit a selected item (making the explanation local). This gives us a local approximation of the complex model with a simpler linear model (this is similar to, e.g., [LIME](https://github.com/marcotcr/lime) and [SHAP](https://github.com/slundberg/shap)). In contrast to other methods SLISE creates explanations using real data (not some discretised and randomly sampled data) so we can be sure that all inputs are valid (i.e. in the correct data manifold, and follows the constraints used to generate the data, e.g., the laws of physics).
 
 ## Installation
```

