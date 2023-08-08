# Comparing `tmp/anatomy-0.1.5.tar.gz` & `tmp/anatomy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anatomy-0.1.5.tar", last modified: Thu Aug  3 16:20:38 2023, max compression
+gzip compressed data, was "anatomy-0.1.6.tar", last modified: Tue Aug  8 13:05:47 2023, max compression
```

## Comparing `anatomy-0.1.5.tar` & `anatomy-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 16:20:38.448448 anatomy-0.1.5/
--rw-rw-rw-   0        0        0     1090 2023-08-03 16:15:29.000000 anatomy-0.1.5/LICENSE
--rw-rw-rw-   0        0        0    19976 2023-08-03 16:20:38.443358 anatomy-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    19199 2023-08-03 16:13:40.000000 anatomy-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 16:20:38.442321 anatomy-0.1.5/anatomy/
--rw-rw-rw-   0        0        0      517 2023-08-03 16:15:42.000000 anatomy-0.1.5/anatomy/__init__.py
--rw-rw-rw-   0        0        0     4696 2022-09-27 13:04:11.000000 anatomy-0.1.5/anatomy/_algorithm.py
--rw-rw-rw-   0        0        0    11761 2022-10-05 11:58:24.000000 anatomy-0.1.5/anatomy/_base.py
--rw-rw-rw-   0        0        0     4419 2023-08-03 15:34:43.000000 anatomy-0.1.5/anatomy/_mas.py
--rw-rw-rw-   0        0        0     3041 2023-02-02 15:07:34.000000 anatomy-0.1.5/anatomy/_models.py
--rw-rw-rw-   0        0        0     2670 2022-10-19 10:06:08.000000 anatomy-0.1.5/anatomy/_subsets.py
-drwxrwxrwx   0        0        0        0 2023-08-03 16:20:38.443358 anatomy-0.1.5/anatomy.egg-info/
--rw-rw-rw-   0        0        0    19976 2023-08-03 16:20:38.000000 anatomy-0.1.5/anatomy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-08-03 16:20:38.000000 anatomy-0.1.5/anatomy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 16:20:38.000000 anatomy-0.1.5/anatomy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-08-03 16:20:38.000000 anatomy-0.1.5/anatomy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-03 16:20:38.000000 anatomy-0.1.5/anatomy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 16:20:38.448448 anatomy-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-08-03 10:00:07.000000 anatomy-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 13:05:47.598918 anatomy-0.1.6/
+-rw-rw-rw-   0        0        0     1090 2023-08-03 16:15:29.000000 anatomy-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0    19899 2023-08-08 13:05:47.598918 anatomy-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    19121 2023-08-08 12:49:04.000000 anatomy-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 13:05:47.589883 anatomy-0.1.6/anatomy/
+-rw-rw-rw-   0        0        0      517 2023-08-08 12:58:59.000000 anatomy-0.1.6/anatomy/__init__.py
+-rw-rw-rw-   0        0        0     4696 2022-09-27 13:04:11.000000 anatomy-0.1.6/anatomy/_algorithm.py
+-rw-rw-rw-   0        0        0    11761 2022-10-05 11:58:24.000000 anatomy-0.1.6/anatomy/_base.py
+-rw-rw-rw-   0        0        0    10477 2023-08-08 12:56:26.000000 anatomy-0.1.6/anatomy/_mas.py
+-rw-rw-rw-   0        0        0     3041 2023-02-02 15:07:34.000000 anatomy-0.1.6/anatomy/_models.py
+-rw-rw-rw-   0        0        0     2670 2022-10-19 10:06:08.000000 anatomy-0.1.6/anatomy/_subsets.py
+drwxrwxrwx   0        0        0        0 2023-08-08 13:05:47.597903 anatomy-0.1.6/anatomy.egg-info/
+-rw-rw-rw-   0        0        0    19899 2023-08-08 13:05:47.000000 anatomy-0.1.6/anatomy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-08-08 13:05:47.000000 anatomy-0.1.6/anatomy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 13:05:47.000000 anatomy-0.1.6/anatomy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-08-08 13:05:47.000000 anatomy-0.1.6/anatomy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-08 13:05:47.000000 anatomy-0.1.6/anatomy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 13:05:47.598918 anatomy-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-08-08 12:59:08.000000 anatomy-0.1.6/setup.py
```

### Comparing `anatomy-0.1.5/LICENSE` & `anatomy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `anatomy-0.1.5/PKG-INFO` & `anatomy-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anatomy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Shapley-based decomposition to anatomize the of out-of-sample accuracy of time-series forecasting models
 Home-page: https://github.com/sander-sn/anatomy
 Author: Sander Schwenk-Nebbe
 Author-email: sandersn@econ.au.dk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -312,38 +312,14 @@
 
     >>> df_oshapley.loc["ols+rf"].abs().mean(axis=0)
     base_contribution    0.078415
     x_0                  0.864057
     x_1                  0.786044
     x_2                  0.770115
 
-## Model Accordance Score:
-
-We can compute the MAS for our combination model (``ols+rf``) using $\text{oShapley-VI}$ and, for instance, the $\text{PBSV(RMSE)}_p$:
-
-    vi = df_oshapley.loc["ols+rf"].abs().mean(axis=0).drop("base_contribution")
-    pbsv = df_pbsv_rmse.loc["ols+rf"].iloc[0].drop("base_contribution")
-
-    h0 = MAS.H0(p=vi.shape[0])               # generate mas(p) under the null
-    loss_type = MAS.LossType.LOWER_IS_BETTER # rmse => lower is better
-
-    mas = MAS(vi, pbsv, loss_type, h0).compute()
-
-which yields the MAS:
-
-    >>> mas
-    {'mas': 1.0, 'mas_p_val': 0.0}
-
-### *Interpretation*
-
-In this example, the ranking of $\text{oShapley-VI}$ is identical to the signed-ranking of $\text{PBSV(RMSE)}_p$.
-Thus, MAS is 1 (perfect) and the null hypothesis of no relation between $\text{oShapley-VI}$ and $\text{PBSV(RMSE)}_p$ is rejected
-(``mas_p_val`` is the probability of observing a MAS lower or equal to ``mas`` under the null).
-
-
 ## The Efficiency property
 
 *During estimation, the `Anatomy` checks that the individual attributions of the predictors to the forecasts sum up exactly to the forecasts produced by the models. The estimation would be aborted if efficiency does not hold.*
 
 Due to the efficiency property of Shapley values, summing the individual contributions yields the decomposed value exactly. We can check that the results that `Anatomy` yields are consistet. We can recover the RMSE from the decomposed RMSE, but we can also recover the RMSE from the decomposed forecasts. Let's make sure that they match.
 
 We first anatomize the RMSE:
@@ -396,7 +372,31 @@
 which yields the same RMSE as the sum of the contributions of the RMSE decomposition:
 
     >>> rmse_b
     rf        1.131310
     ols       0.934551
     ols+rf    0.989733
 
+# Model Accordance Score:
+
+We can compute the MAS for our combination model (``ols+rf``) using $\text{oShapley-VI}$ and, for instance, the
+$\text{PBSV}$ for the root-mean-square error:
+
+    vi = df_oshapley.loc["ols+rf"].abs().mean(axis=0)
+    pbsv = df_pbsv_rmse.loc["ols+rf"].iloc[0]
+
+    # loss type is rmse, so lower is better:
+    loss_type = MAS.LossType.LOWER_IS_BETTER
+
+    mas = MAS(vi, pbsv, loss_type).compute()
+
+which yields the MAS:
+
+    >>> mas
+    {'mas': 1.0, 'mas_p_value': 0.020796}
+
+### *Interpretation*
+
+In this example, the ranking of $\text{oShapley-VI}$ is identical to the signed-ranking of $\text{PBSV}$.
+Thus, MAS is 1 (perfect) and the null hypothesis of no relation between $\text{oShapley-VI}_p$ and $\text{PBSV}_p$
+is rejected at the 5% level (``mas_p_value`` is the probability of observing a MAS at least as extreme as ``mas`` under
+the null).
```

### Comparing `anatomy-0.1.5/README.md` & `anatomy-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -300,38 +300,14 @@
 
     >>> df_oshapley.loc["ols+rf"].abs().mean(axis=0)
     base_contribution    0.078415
     x_0                  0.864057
     x_1                  0.786044
     x_2                  0.770115
 
-## Model Accordance Score:
-
-We can compute the MAS for our combination model (``ols+rf``) using $\text{oShapley-VI}$ and, for instance, the $\text{PBSV(RMSE)}_p$:
-
-    vi = df_oshapley.loc["ols+rf"].abs().mean(axis=0).drop("base_contribution")
-    pbsv = df_pbsv_rmse.loc["ols+rf"].iloc[0].drop("base_contribution")
-
-    h0 = MAS.H0(p=vi.shape[0])               # generate mas(p) under the null
-    loss_type = MAS.LossType.LOWER_IS_BETTER # rmse => lower is better
-
-    mas = MAS(vi, pbsv, loss_type, h0).compute()
-
-which yields the MAS:
-
-    >>> mas
-    {'mas': 1.0, 'mas_p_val': 0.0}
-
-### *Interpretation*
-
-In this example, the ranking of $\text{oShapley-VI}$ is identical to the signed-ranking of $\text{PBSV(RMSE)}_p$.
-Thus, MAS is 1 (perfect) and the null hypothesis of no relation between $\text{oShapley-VI}$ and $\text{PBSV(RMSE)}_p$ is rejected
-(``mas_p_val`` is the probability of observing a MAS lower or equal to ``mas`` under the null).
-
-
 ## The Efficiency property
 
 *During estimation, the `Anatomy` checks that the individual attributions of the predictors to the forecasts sum up exactly to the forecasts produced by the models. The estimation would be aborted if efficiency does not hold.*
 
 Due to the efficiency property of Shapley values, summing the individual contributions yields the decomposed value exactly. We can check that the results that `Anatomy` yields are consistet. We can recover the RMSE from the decomposed RMSE, but we can also recover the RMSE from the decomposed forecasts. Let's make sure that they match.
 
 We first anatomize the RMSE:
@@ -384,7 +360,31 @@
 which yields the same RMSE as the sum of the contributions of the RMSE decomposition:
 
     >>> rmse_b
     rf        1.131310
     ols       0.934551
     ols+rf    0.989733
 
+# Model Accordance Score:
+
+We can compute the MAS for our combination model (``ols+rf``) using $\text{oShapley-VI}$ and, for instance, the
+$\text{PBSV}$ for the root-mean-square error:
+
+    vi = df_oshapley.loc["ols+rf"].abs().mean(axis=0)
+    pbsv = df_pbsv_rmse.loc["ols+rf"].iloc[0]
+
+    # loss type is rmse, so lower is better:
+    loss_type = MAS.LossType.LOWER_IS_BETTER
+
+    mas = MAS(vi, pbsv, loss_type).compute()
+
+which yields the MAS:
+
+    >>> mas
+    {'mas': 1.0, 'mas_p_value': 0.020796}
+
+### *Interpretation*
+
+In this example, the ranking of $\text{oShapley-VI}$ is identical to the signed-ranking of $\text{PBSV}$.
+Thus, MAS is 1 (perfect) and the null hypothesis of no relation between $\text{oShapley-VI}_p$ and $\text{PBSV}_p$
+is rejected at the 5% level (``mas_p_value`` is the probability of observing a MAS at least as extreme as ``mas`` under
+the null).
```

### Comparing `anatomy-0.1.5/anatomy/__init__.py` & `anatomy-0.1.6/anatomy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 
 from ._mas import MAS
 from ._subsets import AnatomySubsets
 from ._models import AnatomyModel, AnatomyModelProvider, AnatomyModelCombination, AnatomyModelOutputTransformer
 from ._algorithm import AnatomyAlgorithm
 from ._base import Anatomy
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 __author__ = "Sander Schwenk-Nebbe"
 __copyright__ = "Copyright 2023, Sander Schwenk-Nebbe"
 __license__ = "MIT"
 __email__ = "sandersn@econ.au.dk"
```

### Comparing `anatomy-0.1.5/anatomy/_algorithm.py` & `anatomy-0.1.6/anatomy/_algorithm.py`

 * *Files identical despite different names*

### Comparing `anatomy-0.1.5/anatomy/_base.py` & `anatomy-0.1.6/anatomy/_base.py`

 * *Files identical despite different names*

### Comparing `anatomy-0.1.5/anatomy/_models.py` & `anatomy-0.1.6/anatomy/_models.py`

 * *Files identical despite different names*

### Comparing `anatomy-0.1.5/anatomy/_subsets.py` & `anatomy-0.1.6/anatomy/_subsets.py`

 * *Files identical despite different names*

### Comparing `anatomy-0.1.5/anatomy.egg-info/PKG-INFO` & `anatomy-0.1.6/anatomy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anatomy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Shapley-based decomposition to anatomize the of out-of-sample accuracy of time-series forecasting models
 Home-page: https://github.com/sander-sn/anatomy
 Author: Sander Schwenk-Nebbe
 Author-email: sandersn@econ.au.dk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -312,38 +312,14 @@
 
     >>> df_oshapley.loc["ols+rf"].abs().mean(axis=0)
     base_contribution    0.078415
     x_0                  0.864057
     x_1                  0.786044
     x_2                  0.770115
 
-## Model Accordance Score:
-
-We can compute the MAS for our combination model (``ols+rf``) using $\text{oShapley-VI}$ and, for instance, the $\text{PBSV(RMSE)}_p$:
-
-    vi = df_oshapley.loc["ols+rf"].abs().mean(axis=0).drop("base_contribution")
-    pbsv = df_pbsv_rmse.loc["ols+rf"].iloc[0].drop("base_contribution")
-
-    h0 = MAS.H0(p=vi.shape[0])               # generate mas(p) under the null
-    loss_type = MAS.LossType.LOWER_IS_BETTER # rmse => lower is better
-
-    mas = MAS(vi, pbsv, loss_type, h0).compute()
-
-which yields the MAS:
-
-    >>> mas
-    {'mas': 1.0, 'mas_p_val': 0.0}
-
-### *Interpretation*
-
-In this example, the ranking of $\text{oShapley-VI}$ is identical to the signed-ranking of $\text{PBSV(RMSE)}_p$.
-Thus, MAS is 1 (perfect) and the null hypothesis of no relation between $\text{oShapley-VI}$ and $\text{PBSV(RMSE)}_p$ is rejected
-(``mas_p_val`` is the probability of observing a MAS lower or equal to ``mas`` under the null).
-
-
 ## The Efficiency property
 
 *During estimation, the `Anatomy` checks that the individual attributions of the predictors to the forecasts sum up exactly to the forecasts produced by the models. The estimation would be aborted if efficiency does not hold.*
 
 Due to the efficiency property of Shapley values, summing the individual contributions yields the decomposed value exactly. We can check that the results that `Anatomy` yields are consistet. We can recover the RMSE from the decomposed RMSE, but we can also recover the RMSE from the decomposed forecasts. Let's make sure that they match.
 
 We first anatomize the RMSE:
@@ -396,7 +372,31 @@
 which yields the same RMSE as the sum of the contributions of the RMSE decomposition:
 
     >>> rmse_b
     rf        1.131310
     ols       0.934551
     ols+rf    0.989733
 
+# Model Accordance Score:
+
+We can compute the MAS for our combination model (``ols+rf``) using $\text{oShapley-VI}$ and, for instance, the
+$\text{PBSV}$ for the root-mean-square error:
+
+    vi = df_oshapley.loc["ols+rf"].abs().mean(axis=0)
+    pbsv = df_pbsv_rmse.loc["ols+rf"].iloc[0]
+
+    # loss type is rmse, so lower is better:
+    loss_type = MAS.LossType.LOWER_IS_BETTER
+
+    mas = MAS(vi, pbsv, loss_type).compute()
+
+which yields the MAS:
+
+    >>> mas
+    {'mas': 1.0, 'mas_p_value': 0.020796}
+
+### *Interpretation*
+
+In this example, the ranking of $\text{oShapley-VI}$ is identical to the signed-ranking of $\text{PBSV}$.
+Thus, MAS is 1 (perfect) and the null hypothesis of no relation between $\text{oShapley-VI}_p$ and $\text{PBSV}_p$
+is rejected at the 5% level (``mas_p_value`` is the probability of observing a MAS at least as extreme as ``mas`` under
+the null).
```

### Comparing `anatomy-0.1.5/setup.py` & `anatomy-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from pathlib import Path
 
 setup(
     name="anatomy",
-    version="0.1.5",
+    version="0.1.6",
     packages=["anatomy"],
     install_requires=[
         "joblib>=0.15.0",
         "numpy>=1.18.1",
         "pandas>=1.0.0"
     ],
     python_requires=">=3.9",
```

