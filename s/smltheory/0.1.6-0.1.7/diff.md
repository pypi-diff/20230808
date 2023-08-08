# Comparing `tmp/smltheory-0.1.6.tar.gz` & `tmp/smltheory-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smltheory-0.1.6.tar", max compression
+gzip compressed data, was "smltheory-0.1.7.tar", max compression
```

## Comparing `smltheory-0.1.6.tar` & `smltheory-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0     1076 2023-08-01 20:38:18.331005 smltheory-0.1.6/LICENSE
--rw-r--r--   0        0        0     1041 2023-08-06 16:05:12.742227 smltheory-0.1.6/README.md
--rw-r--r--   0        0        0      593 2023-08-07 21:41:05.383645 smltheory-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      444 2023-08-06 01:37:23.815152 smltheory-0.1.6/src/smltheory/__init__.py
--rw-r--r--   0        0        0     6199 2023-08-06 01:58:07.279270 smltheory-0.1.6/src/smltheory/bayes_decision.py
--rw-r--r--   0        0        0        0 2023-08-05 02:48:00.360490 smltheory-0.1.6/src/smltheory/data/__init__.py
--rw-r--r--   0        0        0   589785 2023-08-05 03:48:26.746468 smltheory-0.1.6/src/smltheory/data/data_best_in_class.csv
--rw-r--r--   0        0        0  5998151 2023-07-27 15:14:55.256898 smltheory-0.1.6/src/smltheory/data/data_bv_tradeoff.csv
--rw-r--r--   0        0        0     8630 2023-08-05 03:18:12.360165 smltheory-0.1.6/src/smltheory/data/data_emp_loss.csv
--rw-r--r--   0        0        0    23457 2023-07-16 02:37:58.154443 smltheory-0.1.6/src/smltheory/data/data_est_error.csv
--rw-r--r--   0        0        0     8630 2023-08-05 03:18:38.737708 smltheory-0.1.6/src/smltheory/data/data_gen_error.csv
--rw-r--r--   0        0        0    23158 2023-08-05 22:49:49.318878 smltheory-0.1.6/src/smltheory/data/data_opt_error_fast.csv
--rw-r--r--   0        0        0     8557 2023-08-06 01:52:33.818341 smltheory-0.1.6/src/smltheory/datasets.py
--rw-r--r--   0        0        0     3971 2023-08-06 01:52:33.804070 smltheory-0.1.6/src/smltheory/est_error.py
--rw-r--r--   0        0        0    15895 2023-08-06 02:21:14.762431 smltheory-0.1.6/src/smltheory/generate_data.py
--rw-r--r--   0        0        0     9449 2023-08-04 14:15:40.598616 smltheory-0.1.6/src/smltheory/gradient_descent.py
--rw-r--r--   0        0        0     9377 2023-08-04 16:14:40.063052 smltheory-0.1.6/src/smltheory/least_squares.py
--rw-r--r--   0        0        0    11006 2023-08-06 02:27:17.083759 smltheory-0.1.6/src/smltheory/opt_error.py
--rw-r--r--   0        0        0     7613 2023-08-07 21:36:15.046665 smltheory-0.1.6/src/smltheory/overfitting.py
--rw-r--r--   0        0        0    15886 2023-08-04 17:06:08.189243 smltheory-0.1.6/src/smltheory/trun_mvnt.py
--rw-r--r--   0        0        0     1633 1970-01-01 00:00:00.000000 smltheory-0.1.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1076 2023-08-01 20:38:18.331005 smltheory-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1041 2023-08-06 16:05:12.742227 smltheory-0.1.7/README.md
+-rw-r--r--   0        0        0      593 2023-08-07 22:21:11.730777 smltheory-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      444 2023-08-06 01:37:23.815152 smltheory-0.1.7/src/smltheory/__init__.py
+-rw-r--r--   0        0        0     6199 2023-08-06 01:58:07.279270 smltheory-0.1.7/src/smltheory/bayes_decision.py
+-rw-r--r--   0        0        0        0 2023-08-05 02:48:00.360490 smltheory-0.1.7/src/smltheory/data/__init__.py
+-rw-r--r--   0        0        0   589785 2023-08-05 03:48:26.746468 smltheory-0.1.7/src/smltheory/data/data_best_in_class.csv
+-rw-r--r--   0        0        0  5998151 2023-07-27 15:14:55.256898 smltheory-0.1.7/src/smltheory/data/data_bv_tradeoff.csv
+-rw-r--r--   0        0        0     8630 2023-08-05 03:18:12.360165 smltheory-0.1.7/src/smltheory/data/data_emp_loss.csv
+-rw-r--r--   0        0        0    23457 2023-07-16 02:37:58.154443 smltheory-0.1.7/src/smltheory/data/data_est_error.csv
+-rw-r--r--   0        0        0     8630 2023-08-05 03:18:38.737708 smltheory-0.1.7/src/smltheory/data/data_gen_error.csv
+-rw-r--r--   0        0        0    23158 2023-08-05 22:49:49.318878 smltheory-0.1.7/src/smltheory/data/data_opt_error_fast.csv
+-rw-r--r--   0        0        0     8557 2023-08-06 01:52:33.818341 smltheory-0.1.7/src/smltheory/datasets.py
+-rw-r--r--   0        0        0     3971 2023-08-06 01:52:33.804070 smltheory-0.1.7/src/smltheory/est_error.py
+-rw-r--r--   0        0        0    15895 2023-08-06 02:21:14.762431 smltheory-0.1.7/src/smltheory/generate_data.py
+-rw-r--r--   0        0        0     9449 2023-08-04 14:15:40.598616 smltheory-0.1.7/src/smltheory/gradient_descent.py
+-rw-r--r--   0        0        0     9377 2023-08-04 16:14:40.063052 smltheory-0.1.7/src/smltheory/least_squares.py
+-rw-r--r--   0        0        0    11006 2023-08-06 02:27:17.083759 smltheory-0.1.7/src/smltheory/opt_error.py
+-rw-r--r--   0        0        0     7614 2023-08-07 22:20:14.994381 smltheory-0.1.7/src/smltheory/overfitting.py
+-rw-r--r--   0        0        0    15886 2023-08-04 17:06:08.189243 smltheory-0.1.7/src/smltheory/trun_mvnt.py
+-rw-r--r--   0        0        0     1633 1970-01-01 00:00:00.000000 smltheory-0.1.7/PKG-INFO
```

### Comparing `smltheory-0.1.6/LICENSE` & `smltheory-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.6/README.md` & `smltheory-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.6/pyproject.toml` & `smltheory-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smltheory"
-version = "0.1.6"
+version = "0.1.7"
 description = "Demonstrates propositions of supervised machine learning theories"
 authors = ["Sebastian Sciarra"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
```

### Comparing `smltheory-0.1.6/src/smltheory/bayes_decision.py` & `smltheory-0.1.7/src/smltheory/bayes_decision.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.6/src/smltheory/data/data_best_in_class.csv` & `smltheory-0.1.7/src/smltheory/data/data_best_in_class.csv`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.6/src/smltheory/data/data_bv_tradeoff.csv` & `smltheory-0.1.7/src/smltheory/data/data_bv_tradeoff.csv`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.6/src/smltheory/data/data_emp_loss.csv` & `smltheory-0.1.7/src/smltheory/data/data_emp_loss.csv`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.6/src/smltheory/data/data_est_error.csv` & `smltheory-0.1.7/src/smltheory/data/data_est_error.csv`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.6/src/smltheory/data/data_gen_error.csv` & `smltheory-0.1.7/src/smltheory/data/data_gen_error.csv`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.6/src/smltheory/data/data_opt_error_fast.csv` & `smltheory-0.1.7/src/smltheory/data/data_opt_error_fast.csv`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.6/src/smltheory/datasets.py` & `smltheory-0.1.7/src/smltheory/datasets.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.6/src/smltheory/est_error.py` & `smltheory-0.1.7/src/smltheory/est_error.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.6/src/smltheory/generate_data.py` & `smltheory-0.1.7/src/smltheory/generate_data.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.6/src/smltheory/gradient_descent.py` & `smltheory-0.1.7/src/smltheory/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.6/src/smltheory/least_squares.py` & `smltheory-0.1.7/src/smltheory/least_squares.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.6/src/smltheory/opt_error.py` & `smltheory-0.1.7/src/smltheory/opt_error.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.6/src/smltheory/overfitting.py` & `smltheory-0.1.7/src/smltheory/overfitting.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         String specifying polynomial model.
 
     Examples
     --------
     >>> gen_poly_reg_eq(poly_order=2)
     'wine_quality ~ np.power(weather, 1) + np.power(weather, 2) + np.power(winemaking_quality, 1) + np.power(winemaking_quality, 2)'
     """
+
     # compute polynomial terms for predictors
     weather_pred = ' + '.join(['np.power(weather, {})'.format(ord_value) for ord_value in range(1, poly_order + 1)])
     winemaking_quality_pred = ' + '.join(['np.power(winemaking_quality, {})'.format(ord_value)
                                           for ord_value in range(1, poly_order + 1)])
 
     # Compute all two-way interactions between weather and winemaking_quality
     if include_interactions and poly_order > 1:
@@ -97,14 +98,15 @@
     ... sample_size = sample_size_gen_error)
     #equation
     >>> equation = gen_poly_reg_eq(poly_order=2)
     >>> compute_emp_gen_error(equation=equation, data_emp_loss=data_emp_loss,
     ... data_gen_error=data_gen_error)
     {'emp_loss': 0.2420572087052563, 'gen_error': 0.25353431587715874}
     """
+    import numpy as np
     model = smf.ols(data=data_emp_loss, formula=equation).fit()
     y_test = model.predict(data_gen_error)
 
     emp_loss = mean_squared_error(y_true=data_emp_loss['wine_quality'], y_pred=model.fittedvalues)
     gen_error = mean_squared_error(y_true=data_gen_error['wine_quality'], y_pred=y_test)
 
     emp_loss_gen_error_dict = {'emp_loss': emp_loss, 'gen_error': gen_error}
@@ -163,15 +165,14 @@
     3           4  0.219007      0.339122
     4           5  0.202056      2.038340
     5           6  0.184981    537.737954
     6           7  0.177600   6801.505982
     7           8  0.176475  11862.620947
     8           9  0.176777  14885.917939
     """
-    import numpy as np
     # create all polynomial equations within the desired range
     gen_poly_reg_eq_partial = partial(gen_poly_reg_eq, include_interactions=include_interactions)
 
     poly_equations = list(map(gen_poly_reg_eq_partial, poly_order_range))
 
     # create partial version of function with data_emp_loss and data_gen_error fixed
     emp_gen_error_partial = partial(compute_emp_gen_error, data_emp_loss=data_emp_loss,
```

### Comparing `smltheory-0.1.6/src/smltheory/trun_mvnt.py` & `smltheory-0.1.7/src/smltheory/trun_mvnt.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.6/PKG-INFO` & `smltheory-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smltheory
-Version: 0.1.6
+Version: 0.1.7
 Summary: Demonstrates propositions of supervised machine learning theories
 License: MIT
 Author: Sebastian Sciarra
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

