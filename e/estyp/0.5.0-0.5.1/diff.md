# Comparing `tmp/estyp-0.5.0.tar.gz` & `tmp/estyp-0.5.1.tar.gz`

## Comparing `estyp-0.5.0.tar` & `estyp-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 estyp-0.5.0/estyp/__init__.py
--rw-r--r--   0        0        0    18392 2020-02-02 00:00:00.000000 estyp-0.5.0/estyp/cluster/__init__.py
--rw-r--r--   0        0        0     6157 2020-02-02 00:00:00.000000 estyp-0.5.0/estyp/linear_model/__init__.py
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 estyp-0.5.0/estyp/linear_model/stepwise/__init__.py
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 estyp-0.5.0/estyp/linear_model/stepwise/__base/__init__.py
--rw-r--r--   0        0        0    26835 2020-02-02 00:00:00.000000 estyp-0.5.0/estyp/testing/__init__.py
--rw-r--r--   0        0        0    31924 2020-02-02 00:00:00.000000 estyp-0.5.0/estyp/testing/__base/__init__.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 estyp-0.5.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.5.0/LICENSE
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 estyp-0.5.0/README.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 estyp-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 estyp-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 estyp-0.5.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 estyp-0.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 estyp-0.5.1/estyp/__init__.py
+-rw-r--r--   0        0        0    18824 2020-02-02 00:00:00.000000 estyp-0.5.1/estyp/cluster/__init__.py
+-rw-r--r--   0        0        0     7617 2020-02-02 00:00:00.000000 estyp-0.5.1/estyp/linear_model/__init__.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 estyp-0.5.1/estyp/linear_model/stepwise/__init__.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 estyp-0.5.1/estyp/linear_model/stepwise/__base/__init__.py
+-rw-r--r--   0        0        0    24812 2020-02-02 00:00:00.000000 estyp-0.5.1/estyp/testing/__init__.py
+-rw-r--r--   0        0        0    32299 2020-02-02 00:00:00.000000 estyp-0.5.1/estyp/testing/__base/__init__.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 estyp-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.5.1/LICENSE
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 estyp-0.5.1/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 estyp-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 estyp-0.5.1/PKG-INFO
```

### Comparing `estyp-0.5.0/estyp/linear_model/__init__.py` & `estyp-0.5.1/estyp/linear_model/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,98 +1,117 @@
-from typing import Literal
+from typing import Literal, Union
 
 import numpy as np
 from pandas import DataFrame, Series, concat
 from patsy import build_design_matrices, dmatrices
 from scipy.stats import norm
 from sklearn.linear_model import LogisticRegression as LogisticRegression_
 
 
 class LogisticRegression(LogisticRegression_):
     """
-# Logistic Regression
+Logistic Regression
+-------------------
 
-This class implements a logistic regression model. It inherits from the `sklearn.linear_model.LogisticRegression` class, but adds additional methods for calculating confidence intervals, p-values, and model summaries.
-
-## Parameters
-
-* `penalty`: The type of penalty to use. Can be one of `"none"` (default). `"l1"`, `"l2"`, or `"elasticnet"`.
-* `dual`: Whether to use the dual formulation of the problem.
-* `tol`: The tolerance for convergence.
-* `C`: The regularization strength.
-* `fit_intercept`: Whether to fit an intercept term.
-* `intercept_scaling`: The scaling factor for the intercept term.
-* `class_weight`: None (default), "balanced" or a dictionary that maps class labels to weights.
-* `random_state`: The random seed.
-* `solver`: The solver to use. Can be one of `"lbfgs"` (default), `"liblinear"`, `"newton-cg"`, `"newton-cholesky"`, `"sag"`, or `"saga"`.
-* `max_iter`: The maximum number of iterations.
-* `multi_class`: The type of multi-class classification to use. Can be one of `"auto"`, `"ovr"`, or `"multinomial"`.
-* `verbose`: The verbosity level.
-* `warm_start`: Whether to use the warm start.
-* `n_jobs`: The number of jobs to use for parallel processing.
-* `l1_ratio`: The l1_ratio parameter for elasticnet regularization.
-
-## Properties
-
-* `params`: Returns the estimated values for model parameters.
-* `aic`: Calculates the Akaike information criterion (AIC) for the model.
-* `bic`: Calculates the Bayesian information criterion (BIC) for the model.
-* `cov_matrix`: Returns the covariance matrix for model parámetres.
-
-## Methods
-
-* `fit()`: Fits the model to the data.
-* `predict()`: Predicts the class labels for new data.
-* `conf_int()`: Calculates the confidence intervals for the model coefficients.
-* `se()`: Calculates the standard errors for the model coefficients.
-* `z_values()`: Calculates the z-scores for the model coefficients.
-* `p_values()`: Calculates the p-values for the model coefficients.
-* `summary()`: Prints a summary of the model.
-
-
-## Examples
-
-```python
-import numpy as np
-import pandas as pd
-
-np.random.seed(123)
-data = pd.DataFrame({
-    "y": np.random.randint(2, size=100),
-    "x1": np.random.uniform(-1, 1, size=100),
-    "x2": np.random.uniform(-1, 1, size=100),
-})
+Description
+-----------
 
-formula = "y ~ x1 + x2"
+This class implements a logistic regression model. It inherits from the `sklearn.linear_model.LogisticRegression` class, but adds additional methods for calculating confidence intervals, p-values, and model summaries.
 
-spec = LogisticRegression.from_formula(formula, data)
-model = spec.fit()
+Parameters
+----------
 
-print(model.summary())
-```
+- `X`: A Pandas DataFrame or a NumPy array containing the model predictors.
+- `y`: A Pandas Series or a NumPy array containing the model response.
+- `penalty`: The type of penalty to use. Can be one of `"none"` (default). `"l1"`, `"l2"`, or `"elasticnet"`.
+- `dual`: Whether to use the dual formulation of the problem.
+- `tol`: The tolerance for convergence.
+- `C`: The regularization strength.
+- `fit_intercept`: Whether to fit an intercept term.
+- `intercept_scaling`: The scaling factor for the intercept term.
+- `class_weight`: None (default), "balanced" or a dictionary that maps class labels to weights.
+- `random_state`: The random seed.
+- `solver`: The solver to use. Can be one of `"lbfgs"` (default), `"liblinear"`, `"newton-cg"`, `"newton-cholesky"`, `"sag"`, or `"saga"`.
+- `max_iter`: The maximum number of iterations.
+- `multi_class`: The type of multi-class classification to use. Can be one of `"auto"`, `"ovr"`, or `"multinomial"`.
+- `verbose`: The verbosity level.
+- `warm_start`: Whether to use the warm start.
+- `n_jobs`: The number of jobs to use for parallel processing.
+- `l1_ratio`: The l1_ratio parameter for elasticnet regularization.
+
+Properties
+----------
+
+- `params`: Returns the estimated values for model parameters.
+- `aic`: Calculates the Akaike information criterion (AIC) for the model.
+- `bic`: Calculates the Bayesian information criterion (BIC) for the model.
+- `cov_matrix`: Returns the covariance matrix for model parámetres.
+
+Methods
+-------
+
+- `fit()`: Fits the model to the data.
+- `predict()`: Predicts the class labels for new data.
+- `conf_int()`: Calculates the confidence intervals for the model coefficients.
+- `se()`: Calculates the standard errors for the model coefficients.
+- `z_values()`: Calculates the z-scores for the model coefficients.
+- `p_values()`: Calculates the p-values for the model coefficients.
+- `summary()`: Prints a summary of the model.
+
+Examples
+--------
+
+>>> import numpy as np
+>>> import pandas as pd
+>>> np.random.seed(123)
+>>> data = pd.DataFrame({
+...     "y": np.random.randint(2, size=100),
+...     "x1": np.random.uniform(-1, 1, size=100),
+...     "x2": np.random.uniform(-1, 1, size=100),
+... })
+>>> formula = "y ~ x1 + x2"
+>>> spec = LogisticRegression.from_formula(formula, data)
+>>> model = spec.fit()
+>>> print(model.summary())
     """
     
-    def __init__(self, penalty: Literal['l1', 'l2', 'elasticnet'] = None, *, dual = False, tol = 0.0001, C = 1, fit_intercept = False, intercept_scaling = 1, class_weight = None, random_state = 2023, solver: Literal['lbfgs', 'liblinear', 'newton-cg', 'newton-cholesky', 'sag', 'saga'] = "lbfgs", max_iter = 100, multi_class: Literal['auto', 'ovr', 'multinomial'] = "auto", verbose = 0, warm_start: bool = False, n_jobs = -1, l1_ratio = None):
+    def __init__(self, X: Union[DataFrame, np.ndarray]=None, y: Union[Series, np.ndarray]=None, penalty: Literal['l1', 'l2', 'elasticnet'] = None, *, dual = False, tol = 0.0001, C = 1, fit_intercept = False, intercept_scaling = 1, class_weight = None, random_state = 2023, solver: Literal['lbfgs', 'liblinear', 'newton-cg', 'newton-cholesky', 'sag', 'saga'] = "lbfgs", max_iter = 100, multi_class: Literal['auto', 'ovr', 'multinomial'] = "auto", verbose = 0, warm_start: bool = False, n_jobs = -1, l1_ratio = None):
+        
         super().__init__(penalty=penalty, dual=dual, tol=tol, C=C, fit_intercept=fit_intercept, intercept_scaling=intercept_scaling, class_weight=class_weight, random_state=random_state, solver=solver, max_iter=max_iter, multi_class=multi_class, verbose=verbose, warm_start=warm_start, n_jobs=n_jobs, l1_ratio=l1_ratio)
+        
 
+        
+        if self.__dict__.get("X") is None and self.__dict__.get("y") is None:
+            if isinstance(X, np.ndarray):
+                X = DataFrame(X, columns=[f"var_{i+1}" for i in range(X.shape[1])])
+            if X is not None and y is not None:
+                data = concat([X, Series(y, name="y")], axis=1)
+                formula = f"y ~ {' + '.join(X.columns.tolist()) if X.columns.tolist() else 1}"
+                y, X = dmatrices(formula, data)
+                self.X = X
+                self.y = y.reshape(-1)
+                
     @classmethod
-    def from_formula(cls, formula, data):
+    def from_formula(cls, formula, data, **kwargs):
+        if "X" in kwargs.keys() or "y" in kwargs.keys():
+            raise ValueError("The 'X' and 'y' arguments cannot be used with the 'from_formula' method.")
         y, X = dmatrices(formula, data)
-        cls.y = y.reshape(-1)
-        cls.formula = formula
-        cls.X = X
-        return cls()
+        self_ = cls(**kwargs)
+        self_.y = y.reshape(-1)
+        self_.X = X
+        self_.formula = formula
+        return self_
 
     def __log_likelihood(self):
         z = np.dot(self.X, self.coef_.flatten())
         log_likelihood = np.sum(self.y * z - np.log(1 + np.exp(z)))
         return log_likelihood
 
 
-    def fit(self):
+    def fit(self, disp = None):
         super().fit(self.X, self.y)
         return self
     
     def conf_int(self, conf_level = 0.95):
         z_score = norm.ppf(1 - (1 - conf_level) / 2)
         standard_errors = np.sqrt(np.diag(self.cov_matrix))
         lower_limits = self.coef_[0] - z_score * standard_errors
@@ -144,10 +163,20 @@
         return aic.item()
     
     @property
     def bic(self):
         bic = -2 * self.__log_likelihood() + np.log(self.X.shape[0]) * (self.coef_.shape[0] - 1)
         return bic.item()
     
+    def deviance_residuals(self):
+        p = self.predict_proba(self.X)[:, 1]
+        residuals = -2 * (self.y * np.log(p) + (1 - self.y) * np.log(1 - p))
+        return residuals
+    
+    @property
+    def deviance(self):
+        residuals = self.deviance_residuals()
+        return np.sum(residuals).item()
+    
     
     def __repr__(self) -> str:
         return "LogisticRegression()"
```

### Comparing `estyp-0.5.0/estyp/linear_model/stepwise/__base/__init__.py` & `estyp-0.5.1/estyp/linear_model/stepwise/__base/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 from scipy.stats import f as fisher
 from estyp.testing.__base import __nested_models_test
 
 
-
-
-def __both_selection(formula, data, model, max_iter, **kwargs) -> str:
+def __both_selection(formula, data, model, max_iter, verbose, formula_kwargs, fit_kwargs) -> str:
     
-    print("Este proceso tarda un buen tiempo ¡Paciencia! Momento de cuestionarte si eres feliz.")
+    if verbose:
+        print("Este proceso tarda un buen tiempo ¡Paciencia! Momento de cuestionarte si eres feliz.")
     # Preparación
     fi = formula
-    e = model.from_formula(fi, data, **kwargs)
-    m = e.fit()
+    e = model.from_formula(fi, data, **formula_kwargs)
+    m = e.fit(**fit_kwargs)
     preds = e.formula.split("+")
     vr = preds[0].split("~")[0].strip()
     preds[0] = preds[0].split("~")[1]
     preds = [x.strip() for x in preds]
     
     # Algoritmo
     d = data.copy()
 
     aicf = m.aic
     aic0 = 0
 
     var_el = []
     var_ag = []
-    print(f"AIC Inicial: {aicf:0.2f}")
+    
+    if verbose:
+        print(f"AIC Inicial: {aicf:0.2f}")
 
     for i in range(max_iter):
         if i == 0:
             aics = []
             for p in preds:
                 # Crear formula
                 p0 = d.drop(columns=[p, vr]).columns.tolist()
                 f0 = f"{vr} ~ {' + '.join(p0) if p0 else 1}"
                 # Ajustar modelo y extraer AIC
-                m0 = model.from_formula(f0, d, **kwargs).fit()
+                m0 = model.from_formula(f0, d, **formula_kwargs).fit(**fit_kwargs)
                 aics.append(m0.aic)
             aic0 = min(aics)
             id_min_aic = aics.index(min(aics))
             if aic0 < aicf:
                 var_min = preds[id_min_aic]
                 data0 = d.drop(columns=var_min)
                 preds0 = data0.drop(columns=vr).columns.tolist()
                 ff = f"{vr} ~ {' + '.join(preds0) if preds0 else 1}"
                 var_el.append(var_min)
             else:
-                print("No hay mejoras en el AIC, por lo que no se eliminarán variables.")
+                if verbose:
+                    print("No hay mejoras en el AIC, por lo que no se eliminarán variables.")
                 return fi
         else:
             aicf = aic0
             # Quitar variable
             aics_a = []
             for p in preds0:
                 p0 = data0.drop(columns=[p, vr]).columns.tolist()
                 f0 = f"{vr} ~ {' + '.join(p0) if p0 else 1}"
-                m0 = model.from_formula(f0, d, **kwargs).fit()
+                m0 = model.from_formula(f0, d, **formula_kwargs).fit(**fit_kwargs)
                 aics_a.append(m0.aic)
             # Añadir variable
             aics_b = []
             for p in preds:
                 f0 = f"{ff} {('+ ' + p) if p not in preds0 else ''}"
-                m0 = model.from_formula(f0, d, **kwargs).fit() if p not in preds0 else None
+                m0 = model.from_formula(f0, d, **formula_kwargs).fit(**fit_kwargs) if p not in preds0 else None
                 aics_b.append(m0.aic if p not in preds0 else aics_a[preds0.index(p)])
             min_a, min_b = min(aics_a), min(aics_b)
             aic0 = min_a if min_a < min_b else min_b
             if aic0 < aicf:
                 if min_a < min_b:
                     var_min = preds0[aics_a.index(min_a)]
                     data0.drop(columns=var_min, inplace=True)
@@ -75,56 +77,61 @@
                     var_min = preds[aics_b.index(min_b)]
                     data0 = d[preds0 + [var_min, vr]]
                     preds0.append(var_min)
                     ff = f"{vr} ~ {' + '.join(preds0) if preds0 else 1}"
                     var_ag.append(var_min)
                 aicf = aic0
             else:
-                print("=========================")
-                print("|| Fin de la selección ||")
-                print("=========================")
-                print(f"AIC Obtenido: {aicf:0.2f}")
-                print("Variables eliminadas:", var_el if var_el else "Ninguna")
-                print("Variables agregadas:", var_ag if var_ag else "Ninguna")
-                print("Fórmula obtenida:", ff)
+                if verbose:
+                    print("=========================")
+                    print("|| Fin de la selección ||")
+                    print("=========================")
+                    print(f"AIC Obtenido: {aicf:0.2f}")
+                    print("Variables eliminadas:", var_el if var_el else "Ninguna")
+                    print("Variables agregadas:", var_ag if var_ag else "Ninguna")
+                    print("Fórmula obtenida:", ff)
                 return ff
-        print(f"Iteración {i + 1} Finalizada | AIC Actual: {aic0:0.2f}")
+        if verbose:
+            print(f"Iteración {i + 1} Finalizada | AIC Actual: {aic0:0.2f}")
         if not preds0:
             return f"{vr} + 1"
-    print("Máximas iteraciones alcanzadas")
+    if verbose:
+        print("Máximas iteraciones alcanzadas")
     return ff
 
 
-def __forward_selection(y, data, model, alpha, **kwargs):
+def __forward_selection(y, data, model, alpha, verbose, formula_kwargs, fit_kwargs):
     preds = data.columns.to_list()
     preds.remove(y)
 
     f_actual = f"{y} ~ 1"
-    m_actual = model.from_formula(f_actual, data, **kwargs).fit(disp=0)
+    m_actual = model.from_formula(f_actual, data, **formula_kwargs).fit(**fit_kwargs)
     termino = False
     
     while not termino:
         valores_p = []
         for p in preds:
             f_prueba = f"{f_actual} + {p}"
-            m_prueba = model.from_formula(f_prueba, data, **kwargs).fit(disp=0)
+            m_prueba = model.from_formula(f_prueba, data, **formula_kwargs).fit(**fit_kwargs)
             pv = __nested_models_test(m_actual, m_prueba).p_value
             valores_p.append(pv)
         min_vp = min(valores_p)
         if min_vp >= alpha:
             termino = True
             f_actual = f_actual.replace(" 1 +", "")
-            m_actual = model.from_formula(f_actual, data, **kwargs).fit(disp=0)
+            m_actual = model.from_formula(f_actual, data, **formula_kwargs).fit(**fit_kwargs)
         else:
             var_min = preds[valores_p.index(min_vp)]
             f_actual = f"{f_actual} + {var_min}"
-            m_actual = model.from_formula(f_actual, data, **kwargs).fit(disp=0)
+            m_actual = model.from_formula(f_actual, data, **formula_kwargs).fit(**fit_kwargs)
             preds.remove(var_min)
             termino = False if preds else True
             vp = f"{min_vp:0.4f}" if min_vp >= 0.0001 else "<0.0001"
-            print(f"Variable agregada: {var_min:30} | valor-p: {vp}")
-    print("=========================")
-    print("|| Fin de la selección ||")
-    print("=========================")
-    print("Fórmula obtenida:", f_actual)
+            if verbose:
+                print(f"Variable agregada: {var_min:30} | valor-p: {vp}")
+    if verbose:
+        print("=========================")
+        print("|| Fin de la selección ||")
+        print("=========================")
+        print("Fórmula obtenida:", f_actual)
     return f_actual
```

### Comparing `estyp-0.5.0/estyp/testing/__init__.py` & `estyp-0.5.1/estyp/testing/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,133 +18,121 @@
     __cor_test,
     __chisq_test,
 )
 
 
 class CheckModel:
     """
-    # Check Linear Regression Assumptions
+Check Linear Regression Assumptions
+-----------------------------------
 
-    The `CheckModel` class provides methods to test the assumptions of the linear regression model.
-    These assumptions are:
+The `CheckModel` class provides methods to test the assumptions of the linear regression model.
+These assumptions are:
 
-    - Normality of residuals
-    - Homoscedasticity (equal variance) of residuals
-    - Independence of residuals
-    - No Multicollinearity among predictors
-
-    Parameters
-    ----------
-    `fitted_model` : `RegressionResultsWrapper`
-        The fitted linear regression model which is an instance of RegressionResultsWrapper.
-
-    Example
-    -------
-    ```python
-    import statsmodels.api as sm
-    from sklearn.datasets import load_diabetes
-    diabetes = load_diabetes()
-    X = diabetes["data"]
-    y = diabetes["target"]
-    X = sm.add_constant(X)
-    model = sm.OLS(y, X)
-    fitted_model = model.fit()
-    cm = CheckModel(fitted_model)
-    cm.check_all()
-    ```
+- Normality of residuals
+- Homoscedasticity (equal variance) of residuals
+- Independence of residuals
+- No Multicollinearity among predictors
+
+Parameters
+----------
+`fitted_model` : `RegressionResultsWrapper`
+    The fitted linear regression model which is an instance of RegressionResultsWrapper.
+
+Example
+-------
+
+>>> import statsmodels.api as sm
+>>> from sklearn.datasets import load_diabetes
+>>> diabetes = load_diabetes()
+>>> X = diabetes["data"]
+>>> y = diabetes["target"]
+>>> X = sm.add_constant(X)
+>>> model = sm.OLS(y, X)
+>>> fitted_model = model.fit()
+>>> cm = CheckModel(fitted_model)
+>>> cm.check_all()
     """
 
     def __init__(self, fitted_model: RegressionResultsWrapper):
         if not isinstance(fitted_model, RegressionResultsWrapper):
             raise TypeError(
                 "The fitted model must be a RegressionResultsWrapper object"
             )
         self.model = fitted_model
 
     def check_normality(self, alpha=0.05, plot=True, return_pvals=False):
         """
-        Checks the normality assumption of the residuals using several statistical tests.
-
-        Parameters
-        ----------
-        `alpha` : float, optional
-            The significance level used by the statistical tests, by default 0.05.
-        `plot` : bool, optional
-            If `True`, a plot is shown for visual inspection of normality, by default `True`.
-        `return_pvals` : bool, optional
-            If `True`, the p-values of the statistical tests are returned, by default `False`.
+Checks the normality assumption of the residuals using several statistical tests.
 
-        Returns
-        -------
-        dict
-            A dictionary of p-values of the statistical tests if `return_pvals=True`.
+Parameters
+----------
+`alpha` : float, optional
+    The significance level used by the statistical tests, by default 0.05.
+`plot` : bool, optional
+    If `True`, a plot is shown for visual inspection of normality, by default `True`.
+`return_pvals` : bool, optional
+    If `True`, the p-values of the statistical tests are returned, by default `False`.
 
-        Example
-        -------
-        >>> cm.check_normality()
+Returns
+-------
+dict
+    A dictionary of p-values of the statistical tests if `return_pvals=True`.
         """
         normality = _CheckNormality(self.model)
         if plot:
             fig, ax = normality.plot()
             plt.show()
         pvals = normality.test(sign_level=alpha)
         if return_pvals:
             return pvals
 
     def check_homocedasticity(self, alpha=0.05, plot=True, return_pvals=False):
         """
-        Checks the homoscedasticity assumption (equal variance of residuals) using several statistical tests.
-
-        Parameters
-        ----------
-        `alpha` : float, optional
-            The significance level used by the statistical tests, by default 0.05.
-        `plot` : bool, optional
-            If `True`, a plot is shown for visual inspection of homoscedasticity, by default `True`.
-        `return_pvals` : bool, optional
-            If `True`, the p-values of the statistical tests are returned, by default `False`.
+Checks the homoscedasticity assumption (equal variance of residuals) using several statistical tests.
 
-        Returns
-        -------
-        dict
-            A dictionary of p-values of the statistical tests if `return_pvals=True`.
+Parameters
+----------
+`alpha` : float, optional
+    The significance level used by the statistical tests, by default 0.05.
+`plot` : bool, optional
+    If `True`, a plot is shown for visual inspection of homoscedasticity, by default `True`.
+`return_pvals` : bool, optional
+    If `True`, the p-values of the statistical tests are returned, by default `False`.
 
-        Example
-        -------
-        >>> cm.check_homocedasticity()
+Returns
+-------
+dict
+    A dictionary of p-values of the statistical tests if `return_pvals=True`.
         """
         homocedasticity = _CheckHomocedasticity(self.model)
         if plot:
             fig, ax = homocedasticity.plot()
             plt.show()
         pvals = homocedasticity.test(sign_level=alpha)
         if return_pvals:
             return pvals
 
     def check_independence(self, alpha=0.05, plot=True, return_vals=False):
         """
-        Checks the independence assumption of the residuals using several statistical tests.
+Checks the independence assumption of the residuals using several statistical tests.
 
-        Parameters
-        ----------
-        alpha : float, optional
-            The significance level used by the statistical tests, by default 0.05.
-        plot : bool, optional
-            If `True`, a plot is shown for visual inspection of independence, by default `True`.
-        return_pvals : bool, optional
-            If `True`, the p-values of the statistical tests are returned, by default `False`.
+Parameters
+----------
+alpha : float, optional
+    The significance level used by the statistical tests, by default 0.05.
+plot : bool, optional
+    If `True`, a plot is shown for visual inspection of independence, by default `True`.
+return_pvals : bool, optional
+    If `True`, the p-values of the statistical tests are returned, by default `False`.
 
-        Returns
-        -------
-        dict
-            A dictionary of values of the statistical tests if `return_vals=True`.
-
-        Example
-        -------
-        >>> cm.check_independence()
+Returns
+-------
+dict
+    A dictionary of values of the statistical tests if `return_vals=True`.
         """
         independence = _CheckIndependence(self.model)
         if plot:
             fig, ax = independence.plot()
             plt.show()
         vals = independence.test(sign_level=alpha)
         if return_vals:
@@ -161,48 +149,40 @@
         `return_cm` : bool, optional
             Returns the condition number of the model if True, by default False.
 
         Returns
         -------
         float
             The condition number of the model if `return_cm=True`.
-
-        Example
-        -------
-        >>> cm.check_multicollinearity()
         """
         multicollinearity = _CheckMulticollinearity(self.model)
         if plot:
             fig, ax = multicollinearity.plot()
             plt.show()
         pvals = multicollinearity.test()
         if return_cm:
             return pvals
 
     def check_all(self, alpha=0.05, plot=True, return_vals=False):
         """
-        Checks all the assumptions of the linear regression model.
-
-        Parameters
-        ----------
-        `alpha` : float, optional
-            The significance level used by the statistical tests, by default 0.05.
-        `plot` : bool, optional
-            If `True`, a plot is shown for visual inspection of each assumption, by default `True`.
-        `return_vals` : bool, optional
-            If `True`, the values of the statistical tests are returned, by default `False`.
+Checks all the assumptions of the linear regression model.
 
-        Returns
-        -------
-        dict
-            A dictionary of values of the statistical tests if `return_vals=True`.
+Parameters
+----------
+`alpha` : float, optional
+    The significance level used by the statistical tests, by default 0.05.
+`plot` : bool, optional
+    If `True`, a plot is shown for visual inspection of each assumption, by default `True`.
+`return_vals` : bool, optional
+    If `True`, the values of the statistical tests are returned, by default `False`.
 
-        Example
-        -------
-        >>> cm.check_all()
+Returns
+-------
+dict
+    A dictionary of values of the statistical tests if `return_vals=True`.
         """
         normality = _CheckNormality(self.model)
         homocedasticity = _CheckHomocedasticity(self.model)
         independence = _CheckIndependence(self.model)
         multicollinearity = _CheckMulticollinearity(self.model)
 
         normality_results = normality.test(sign_level=alpha)
@@ -236,414 +216,385 @@
     x: Union[List, np.ndarray, Series],
     y: Union[List, np.ndarray, Series],
     ratio: Union[float, int] = 1,
     alternative: Literal["two-sided", "less", "greater"] = "two-sided",
     conf_level=0.95,
 ) -> TestResults:
     """
-    # F Test to Compare Two Variances
-    ## Description
-    Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the software R.
-
-    ## Usage
-
-    ```python
-    var_test(x, y, ...)
-    var_test(x, y, ratio = 1,
-            alternative = [two-sided", "less", "greater"],
-            conf_level = 0.95)
-    ```
-
-    ## Arguments
-    * `x`, `y`: numeric list, `np.array` or `pd.Series` of data values.
-    * `ratio`: the hypothesized ratio of the population variances of x and y.
-    * `alternative`: a character string specifying the alternative hypothesis, must be one of "two.sided" (default), "greater" or "less". You can specify just the initial letter.
-    * `conf_level`: a number between 0 and 1 indicanting the confidence level of the interval.
-
-
-    ## Details
-    The null hypothesis is that the ratio of the variances of the populations from which x and y were drawn, is equal to ratio.
-
-    ## Value
-    An instance of the `TestResults` class containing the following attributes:
-
-    * `statistic`: the value of the F test statistic.
-    * `df`: the degrees of freedom for the F test statistic.
-    * `p_value`: the p-value for the test.
-    * `ci`: a confidence interval for the ratio of the population variances.
-    * `estimate`: the ratio of the sample variances of x and y.
-    * `alternative`: a string describing the alternative hypothesis.
-
-    ## Examples
-
-    ```python
-    import numpy as np
-    np.random.seed(2023)
-    x = np.random.normal(size=100)
-    y = np.random.normal(size=100)
-
-    print(var_test(x, y))
-    print(var_test(x, y, alternative="less"))
-    print(var_test(x, y, ratio = 0.9, alternative="greater"))
-    ```
+F Test to Compare Two Variances
+-------------------------------
+
+Description
+-----------
+Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the software R.
+
+
+Arguments
+---------
+- `x`, `y`: numeric list, `np.array` or `pd.Series` of data values.
+- `ratio`: the hypothesized ratio of the population variances of x and y.
+- `alternative`: a character string specifying the alternative hypothesis, must be one of "two-sided" (default), "greater" or "less". You can specify just the initial letter.
+- `conf_level`: a number between 0 and 1 indicanting the confidence level of the interval.
+
+Details
+-------
+The null hypothesis is that the ratio of the variances of the populations from which x and y were drawn, is equal to ratio.
+
+Value
+-----
+An instance of the `TestResults` class containing the following attributes:
+
+- `statistic`: the value of the F test statistic.
+- `df`: the degrees of freedom for the F test statistic.
+- `p_value`: the p-value for the test.
+- `ci`: a confidence interval for the ratio of the population variances.
+- `estimate`: the ratio of the sample variances of x and y.
+- `alternative`: a string describing the alternative hypothesis.
+
+Examples
+--------
+
+>>> import numpy as np
+>>> np.random.seed(2023)
+>>> x = np.random.normal(size=100)
+>>> y = np.random.normal(size=100)
+
+>>> print(var_test(x, y))
+>>> print(var_test(x, y, alternative="less"))
+>>> print(var_test(x, y, ratio=0.9, alternative="greater"))
     """
     return __var_test(x, y, ratio, alternative, conf_level)
 
 
 def t_test(
     x: Union[List, np.ndarray, Series],
     y: Union[List, np.ndarray, Series] = None,
     alternative: Literal["two-sided", "less", "greater"] = "two-sided",
     mu: Union[float, int] = 0,
     paired=False,
     var_equal=False,
     conf_level=0.95,
 ) -> TestResults:
     """
+Student's t-Test
+-----------------
 
-    # Student's t-Test
-    ## Description
-    Performs one and two sample t-tests on groups of data. This function is inspired by the `t.test()` function of the software R.
-
-    ## Usage
-    ```python
-    t_test(x, ...)
-    ```
-
-    ```python
-    t_test(x, y = None,
-        alternative = ["two-sided", "less", "greater"],
-        mu = 0, paired = False, var_equal = False,
-        conf_level = 0.95)
-    ```
-
-
-    ## Arguments
-    * `x`: a (non-empty) numeric container of data values.
-    * `y`: an (optional) numeric container of data values.
-    * `alternative`: a string specifying the alternative hypothesis, must be one of "two-sided" (default), "greater" or "less".
-    * `mu`: a number indicating the true value of the mean (or difference in means if you are performing a two sample test).
-    * `paired`: a logical indicating whether you want a paired t-test.
-    * `var_equal`: a logical variable indicating whether to treat the two variances as being equal. If `True` then the pooled variance is used to estimate the variance otherwise the Welch (or Satterthwaite) approximation to the degrees of freedom is used.
-    * `conf_level`: a number between 0 and 1 indicanting the confidence level of the interval.
-
-
-    ## Details
-    alternative = "greater" is the alternative that x has a larger mean than y. For the one-sample case: that the mean is positive.
-
-    If `paired` is `True` then both x and y must be specified and they must be the same length. Missing values are silently removed (in pairs if `paired` is `True`). If `var_equal` is `True` then the pooled estimate of the variance is used. By default, if `var_equal` is `False` then the variance is estimated separately for both groups and the Welch modification to the degrees of freedom is used.
-
-
-    ### Value
-    An instance of the `TestResults` class containing the following attributes:
-
-    * `statistic`: the value of the t-statistic.
-    * `df`: the degrees of freedom for the t-statistic.
-    * `p_value`: the p-value for the test.
-    * `ci`: a confidence interval for the mean appropriate to the specified alternative hypothesis.
-    * `estimate`: the estimated mean or list of estimated means depending on whether it was a one-sample test or a two-sample test.
-    * `alternative`: a character string describing the alternative hypothesis.
-    * `mu`: the mean of the null hypothesis.
-
-
-    ## Examples
-    ```python
-    import numpy as np
-    np.random.seed(2023)
-    x = np.random.normal(size=100)
-    y = np.random.normal(size=100)
-    mu = 0.1
-
-    print(t_test(x, mu=mu, alternative="less"))
-    print(t_test(x, y, mu=mu))
-    print(t_test(x, y, mu=mu, var_equal=True, alternative="greater"))
-    print(t_test(x, y, mu=mu, paired=True))
-    ```
+Description
+-----------
+Performs one and two sample t-tests on groups of data. This function is inspired by the `t.test()` function of the software R.
+
+
+Arguments
+---------
+- `x`: a (non-empty) numeric container of data values.
+- `y`: an (optional) numeric container of data values.
+- `alternative`: a string specifying the alternative hypothesis, must be one of "two-sided" (default), "greater" or "less".
+- `mu`: a number indicating the true value of the mean (or difference in means if you are performing a two sample test).
+- `paired`: a logical indicating whether you want a paired t-test.
+- `var_equal`: a logical variable indicating whether to treat the two variances as being equal. If `True` then the pooled variance is used to estimate the variance otherwise the Welch (or Satterthwaite) approximation to the degrees of freedom is used.
+- `conf_level`: a number between 0 and 1 indicanting the confidence level of the interval.
+
+Details
+-------
+alternative = "greater" is the alternative that x has a larger mean than y. For the one-sample case: that the mean is positive.
+
+If `paired` is `True` then both x and y must be specified and they must be the same length. Missing values are silently removed (in pairs if `paired` is `True`). If `var_equal` is `True` then the pooled estimate of the variance is used. By default, if `var_equal` is `False` then the variance is estimated separately for both groups and the Welch modification to the degrees of freedom is used.
+
+Value
+-----
+An instance of the `TestResults` class containing the following attributes:
+
+- `statistic`: the value of the t-statistic.
+- `df`: the degrees of freedom for the t-statistic.
+- `p_value`: the p-value for the test.
+- `ci`: a confidence interval for the mean appropriate to the specified alternative hypothesis.
+- `estimate`: the estimated mean or list of estimated means depending on whether it was a one-sample test or a two-sample test.
+- `alternative`: a character string describing the alternative hypothesis.
+- `mu`: the mean of the null hypothesis.
+
+Examples
+--------
+
+>>> import numpy as np
+>>> np.random.seed(2023)
+>>> x = np.random.normal(size=100)
+>>> y = np.random.normal(size=100)
+>>> mu = 0.1
+
+>>> print(t_test(x, mu=mu, alternative="less"))
+>>> print(t_test(x, y, mu=mu))
+>>> print(t_test(x, y, mu=mu, var_equal=True, alternative="greater"))
+>>> print(t_test(x, y, mu=mu, paired=True))
     """
     return __t_test(x, y, alternative, mu, paired, var_equal, conf_level)
 
 
 def nested_models_test(
     fitted_small_model: RegressionResultsWrapper,
     fitted_big_model: RegressionResultsWrapper,
 ) -> TestResults:
     """
-    # Nested Models F-Test Function
+Nested Models F-Test Function
+-----------------------------
+
+Description:
+-------------
+This function performs a nested models F-test using deviance from two fitted models from statsmodels library. The test compares two nested models: a larger or "big" model and a smaller or "small" model. The purpose of this test is to determine whether the larger model significantly improves the model fit compared to the smaller model by adding additional predictors.
 
-    ## Description
+Parameters:
+-----------
+`fitted_small_model` : `RegressionResultsWrapper`
+    The fitted model representing the smaller/nested model. It has to come from statsmodels.
+`fitted_big_model` : `RegressionResultsWrapper`
+    The fitted model representing the larger model, which includes all the predictors from the smaller model and potentially additional predictors. It has to come from statsmodels.
 
-    This function performs a nested models F-test using deviance from two fitted models from statsmodels library. The test compares two nested models: a larger or "big" model and a smaller or "small" model. The purpose of this test is to determine whether the larger model significantly improves the model fit compared to the smaller model by adding additional predictors.
+Returns:
+--------
+The function returns an object of class TestResults that contains the following information:
 
-    ## Parameters
-    * `fitted_small_model`: The fitted model representing the smaller/nested model. It have to come from statsmodels.
-    * `fitted_big_model`: : The fitted model representing the larger model, which includes all the predictors from the smaller model and potentially additional predictors. It have to come from statsmodels.
-
-    ## Returns
-
-    The function returns an object of class TestResults that contains the following information:
-
-    * `method`: A string indicating the name of the statistical test (Nested models F-test).
-    * `statistic`: The computed F-statistic value.
-    * `estimate`: The difference in deviances between the models.
-    * `df`: A dictionary with the degrees of freedom for the numerator and denominator of the F-statistic.
-    * p_value: The p-value associated with the F-statistic.
-
-    ## Examples
-    ### Example 1: With OLS
-    ```python
-    import pandas as pd
-    import statsmodels.api as sm
-    data = pd.DataFrame({
-        "x": [2.01, 2.99, 4.01, 5.01, 6.89],
-        "y": [2, 3, 4, 5, 6]
-    })
-
-    model_small = sm.OLS.from_formula("y ~ 1", data).fit()
-    model_big = sm.OLS.from_formula("y ~ x", data).fit()
-
-    print(nested_models_test(model_small, model_big))
-    ```
-    ### Example 2: With Logit
-    ```python
-    import pandas as pd
-    import statsmodels.api as sm
-    data = pd.DataFrame({
-        "x": [2.01, 2.99, 4.01, 3.01, 4.89],
-        "y": [0, 1, 1, 0, 1]
-    })
-
-    model_small = sm.Logit.from_formula("y ~ 1", data).fit()
-    model_big = sm.Logit.from_formula("y ~ x", data).fit()
-
-    print(nested_models_test(model_small, model_big))
-    ```
-    ### Example 3: With GLM
-    ```python
-    import pandas as pd
-    import statsmodels.api as sm
-    data = pd.DataFrame({
-        "x": [2.01, 2.99, 4.01, 5.01, 6.89],
-        "y": [2, 3, 4, 5, 6]
-    })
-    model_small = sm.GLM.from_formula("y ~ 1", data, family = sm.families.Gamma()).fit()
-    model_big = sm.GLM.from_formula("y ~ x", data, family = sm.families.Gamma()).fit()
+`method` : str
+    A string indicating the name of the statistical test (Nested models F-test).
+`statistic` : float
+    The computed F-statistic value.
+`estimate` : float
+    The difference in deviances between the models.
+`df` : dict
+    A dictionary with the degrees of freedom for the numerator and denominator of the F-statistic.
+`p_value` : float
+    The p-value associated with the F-statistic.
 
-    print(nested_models_test(model_small, model_big))
-    ```
+Examples:
+---------
+Example 1: With OLS
+
+>>> import pandas as pd
+>>> import statsmodels.api as sm
+>>> data = pd.DataFrame({
+...     "x": [2.01, 2.99, 4.01, 5.01, 6.89],
+...     "y": [2, 3, 4, 5, 6]
+... })
+>>> model_small = sm.OLS.from_formula("y ~ 1", data).fit()
+>>> model_big = sm.OLS.from_formula("y ~ x", data).fit()
+>>> print(nested_models_test(model_small, model_big))
+
+Example 2: With Logit
+
+>>> import pandas as pd
+>>> import statsmodels.api as sm
+>>> data = pd.DataFrame({
+...     "x": [2.01, 2.99, 4.01, 3.01, 4.89],
+...     "y": [0, 1, 1, 0, 1]
+... })
+>>> model_small = sm.Logit.from_formula("y ~ 1", data).fit()
+>>> model_big = sm.Logit.from_formula("y ~ x", data).fit()
+>>> print(nested_models_test(model_small, model_big))
+
+Example 3: With GLM
+
+>>> import pandas as pd
+>>> import statsmodels.api as sm
+>>> data = pd.DataFrame({
+...     "x": [2.01, 2.99, 4.01, 5.01, 6.89],
+...     "y": [2, 3, 4, 5, 6]
+... })
+>>> model_small = sm.GLM.from_formula("y ~ 1", data, family = sm.families.Gamma()).fit()
+>>> model_big = sm.GLM.from_formula("y ~ x", data, family = sm.families.Gamma()).fit()
+>>> print(nested_models_test(model_small, model_big))
     """
     return __nested_models_test(fitted_small_model, fitted_big_model)
 
 
 def prop_test(
     x: Union[List, np.ndarray, Series],
     n: Optional[Union[List, np.ndarray, Series]] = None,
     p: Optional[Union[float, List, np.ndarray]] = None,
     alternative: str = "two-sided",
     conf_level: float = 0.95,
     correct: bool = True,
 ) -> TestResults:
     """
-    # Test of Equal or Given Proportions.
+Test of Equal or Given Proportions.
+
+Parameters
+----------
+`x` : array_like
+    A vector of counts of successes, a one-dimensional table with two entries,
+    or a two-dimensional table (or matrix) with 2 columns, giving the counts of
+    successes and failures, respectively.
+`n` : array_like, optional
+    A vector of counts of trials; ignored if x is a matrix or a table.
+    If not provided, it is calculated as the sum of the elements in x.
+`p` : array_like, optional
+    A vector of probabilities of success. The length of p must be the same as
+    the number of groups specified by x, and its elements must be greater than
+    0 and less than 1.
+`alternative` : str, optional
+    A character string specifying the alternative hypothesis, must be one of
+    "two-sided" (default), "greater" or "less". You can specify just the
+    initial letter. Only used for testing the null that a single proportion
+    equals a given value, or that two proportions are equal; ignored otherwise.
+`conf_level` : float, optional
+    Confidence level of the returned confidence interval. Must be a single
+    number between 0 and 1. Only used when testing the null that a single
+    proportion equals a given value, or that two proportions are equal;
+    ignored otherwise.
+`correct` : bool, optional
+    A logical indicating whether Yates' continuity correction should be
+    applied where possible.
+
+Returns
+-------
+`TestResults`
+    A data class with the following attributes:
+
+    - `statistic` : float
+        The value of Pearson's chi-squared test statistic.
+    - `df` : int
+        The degrees of freedom of the approximate chi-squared distribution of
+        the test statistic.
+    - `p_value` : float
+        The p-value of the test.
+    - `estimate` : array_like
+        A vector with the sample proportions x/n.
+    - `null_value` : float or array_like
+        The value of p if specified by the null hypothesis.
+    - `conf_int` : array_like
+        A confidence interval for the true proportion if there is one group,
+        or for the difference in proportions if there are 2 groups and p is
+        not given, or None otherwise. In the cases where it is not None, the
+        returned confidence interval has an asymptotic confidence level as
+        specified by conf_level, and is appropriate to the specified
+        alternative hypothesis.
+    - `alternative` : str
+        A character string describing the alternative.
+    - `method` : str
+        A character string indicating the method used, and whether Yates'
+        continuity correction was applied.
+
+Examples
+--------
 
-    `prop_test()` can be used for testing the null that the proportions
-    (probabilities of success) in several groups are the same, or that they equal
-    certain given values.
-
-    Parameters
-    ----------
-    `x` : array_like
-        a vector of counts of successes, a one-dimensional table with two entries,
-        or a two-dimensional table (or matrix) with 2 columns, giving the counts of
-        successes and failures, respectively.
-    `n` : array_like, optional
-        a vector of counts of trials; ignored if x is a matrix or a table.
-        If not provided, it is calculated as the sum of the elements in x.
-    `p` : array_like, optional
-        a vector of probabilities of success. The length of p must be the same as
-        the number of groups specified by x, and its elements must be greater than
-        0 and less than 1.
-    alternative : str, optional
-        a character string specifying the alternative hypothesis, must be one of
-        "two.sided" (default), "greater" or "less". You can specify just the
-        initial letter. Only used for testing the null that a single proportion
-        equals a given value, or that two proportions are equal; ignored otherwise.
-    `conf_level` : float, optional
-        confidence level of the returned confidence interval. Must be a single
-        number between 0 and 1. Only used when testing the null that a single
-        proportion equals a given value, or that two proportions are equal;
-        ignored otherwise.
-    `correct` : bool, optional
-        a logical indicating whether Yates' continuity correction should be
-        applied where possible.
-
-    Returns
-    -------
-    `TestResult`
-        A data class with the following attributes:
-
-        `statistic` : float
-            the value of Pearson's chi-squared test statistic.
-        `df` : int
-            the degrees of freedom of the approximate chi-squared distribution of
-            the test statistic.
-        `p_value` : float
-            the p-value of the test.
-        `estimate` : array_like
-            a vector with the sample proportions x/n.
-        `null_value` : float or array_like
-            the value of p if specified by the null hypothesis.
-        `conf_int` : array_like
-            a confidence interval for the true proportion if there is one group,
-            or for the difference in proportions if there are 2 groups and p is
-            not given, or None otherwise. In the cases where it is not None, the
-            returned confidence interval has an asymptotic confidence level as
-            specified by conf_level, and is appropriate to the specified
-            alternative hypothesis.
-        `alternative` : str
-            a character string describing the alternative.
-        `method` : str
-            a character string indicating the method used, and whether Yates'
-            continuity correction was applied.
-
-    Example
-    --------
-    ```python
-    import numpy as np
-    from scipy import stats
-    x = np.array([83, 90, 129, 70])
-    n = np.array([86, 93, 136, 82])
-    result = prop_test(x, n)
-    print(result)
-    ```
+>>> import numpy as np
+>>> from scipy import stats
+>>> x = np.array([83, 90, 129, 70])
+>>> n = np.array([86, 93, 136, 82])
+>>> result = prop_test(x, n)
+>>> print(result)
     """
     return __prop_test(x, n, p, alternative, conf_level, correct)
 
 
 def cor_test(
     x: Union[List, np.ndarray, Series],
     y: Union[List, np.ndarray, Series],
     method: Literal["pearson", "kendall", "spearman"] = "pearson",
     alternative: Literal["two-sided", "less", "greater"] = "two-sided",
     conf_level: float = 0.95,
     continuity: bool = False,
 ) -> TestResults:
     """
-    # Test for Association/Correlation Between Paired Samples
+Test for Association/Correlation Between Paired Samples
+-------------------------------------------------------
 
-    Description
-    -----------
-    Test for association between paired samples, using one of Pearson's product moment correlation coefficient, Kendall's
-    tau or Spearman's rho.
-
-    Usage
-    -----
-    ```python
-    cor_test(x, y, ...)
-    cor_test(x, y, alternative="two-sided", method="pearson", conf_level=0.95, continuity=False)
-    ```
-
-    Arguments
-    ---------
-    `x`, `y` : array_like
-        Numeric one-dimensional `arrays`, `lists` or `pd.Series` of data values. `x` and `y` must have the same length.
-
-    `alternative` : str, optional
-        Indicates the alternative hypothesis and must be one of "two-sided", "greater" or "less".
-        "greater" corresponds to positive association, "less" to negative association.
-
-    `method` : str, optional
-        A string indicating which correlation coefficient is to be used for the test.
-        One of "pearson", "kendall", or "spearman".
-
-    `conf_level` : float, optional
-        Confidence level for the returned confidence interval. Currently only used for the
-        Pearson product moment correlation coefficient if there are at least 4 complete pairs of observations.
-
-    `continuity` : bool, optional
-        If `True`, a continuity correction is used for Kendall's tau.
-
-    Returns
-    -------
-    A `TestResults` instance containing the following atributes:
-        - `statistic`: the value of the test statistic.
-        - `df` (if applicable): the degrees of freedom of the test statistic.
-        - `p_value`: the p-value of the test.
-        - `estimate`: the estimated measure of association.
-        - `null_value`: the value of the association measure under the null hypothesis, always 0.
-        - `alternative`: a string describing the alternative hypothesis.
-        - `method`: a string indicating how the association was measured.
-        - `conf_int` (if applicable): a confidence interval for the measure of association.
-
-    Details
-    -------
-    The three methods each estimate the association between paired samples and compute a test of the value being zero.
-    They use different measures of association, all in the range [-1, 1] with 0 indicating no association.
-    These are sometimes referred to as tests of no correlation, but that term is often confined to the default method.
-
-    References
-    ----------
-    [1] D. J. Best & D. E. Roberts (1975). Algorithm AS 89: The Upper Tail Probabilities of Spearman's rho.
-        Applied Statistics, 24, 377--379. 10.2307/2347111.
-
-    [2] Myles Hollander & Douglas A. Wolfe (1973), Nonparametric Statistical Methods.
-        New York: John Wiley & Sons. Pages 185--194 (Kendall and Spearman tests).
-
-    Example
-    -------
-    Using the iris dataset to test the association between sepal length and petal length using Pearson's correlation:
-
-    ```python
-    from sklearn import datasets
-    iris = datasets.load_iris()
+Description
+-----------
+Test for association between paired samples, using one of Pearson's product moment correlation coefficient, Kendall's
+tau or Spearman's rho.
+
+Arguments
+---------
+`x`, `y` : array_like
+    Numeric one-dimensional `arrays`, `lists` or `pd.Series` of data values. `x` and `y` must have the same length.
+
+`alternative` : str, optional
+    Indicates the alternative hypothesis and must be one of "two-sided", "greater" or "less".
+    "greater" corresponds to positive association, "less" to negative association.
+
+`method` : str, optional
+    A string indicating which correlation coefficient is to be used for the test.
+    One of "pearson", "kendall", or "spearman".
+
+`conf_level` : float, optional
+    Confidence level for the returned confidence interval. Currently only used for the
+    Pearson product moment correlation coefficient if there are at least 4 complete pairs of observations.
+
+`continuity` : bool, optional
+    If `True`, a continuity correction is used for Kendall's tau.
 
-    sepal_length = iris.data[:, 0]
-    petal_length = iris.data[:, 2]
+Returns
+-------
+A `TestResults` instance containing the following atributes:
+    - `statistic`: the value of the test statistic.
+    - `df` (if applicable): the degrees of freedom of the test statistic.
+    - `p_value`: the p-value of the test.
+    - `estimate`: the estimated measure of association.
+    - `null_value`: the value of the association measure under the null hypothesis, always 0.
+    - `alternative`: a string describing the alternative hypothesis.
+    - `method`: a string indicating how the association was measured.
+    - `conf_int` (if applicable): a confidence interval for the measure of association.
+
+Details
+-------
+The three methods each estimate the association between paired samples and compute a test of the value being zero.
+They use different measures of association, all in the range [-1, 1] with 0 indicating no association.
+These are sometimes referred to as tests of no correlation, but that term is often confined to the default method.
+
+References
+----------
+[1] D. J. Best & D. E. Roberts (1975). Algorithm AS 89: The Upper Tail Probabilities of Spearman's rho.
+    Applied Statistics, 24, 377--379. 10.2307/2347111.
+
+[2] Myles Hollander & Douglas A. Wolfe (1973), Nonparametric Statistical Methods.
+    New York: John Wiley & Sons. Pages 185--194 (Kendall and Spearman tests).
+
+Example
+-------
+Using the iris dataset to test the association between sepal length and petal length using Pearson's correlation:
+
+>>> from sklearn import datasets
+>>> iris = datasets.load_iris()
+>>> sepal_length = iris.data[:, 0]
+>>> petal_length = iris.data[:, 2]
+>>> result = cor_test(sepal_length, petal_length, method="pearson")
+>>> print(result)
 
-    result = cor_test(sepal_length, petal_length, method="pearson")
-    print(result)
     """
     return __cor_test(x, y, method, alternative, conf_level, continuity)
 
 
 def chisq_test(
     x: Union[List, np.ndarray, Series],
     y: Union[List, np.ndarray, Series, None] = None,
     p: Union[List, np.ndarray, Series, None] = None,
     correct: bool = True,
     rescale_p: bool = False
 ):
     """
-# Pearson's Chi-squared Test for Count Data
+Pearson's Chi-squared Test for Count Data
+------------------------------------------
 
 
 Description
 -----------
 `chisq_test()` performs chi-squared contingency table tests and goodness-of-fit tests.
 
-Usage
-------
-```python
-chisq_test(x, ...)
-chisq_test(x, y=None, correct=True, p=None, rescale_p=False)
-```
-
 Arguments
 ---------
 `x`: arrat_like
     A numeric list or 2D list (matrix). x and y can also both be lists.
     
 `y`: array_like
     A numeric data ; ignored if x is a matrix. If x is a list, y should be a list of the same length. The default is None.
 
 `p`: array_like
     A list of probabilities of the same length as x. An error is raised if any entry of p is negative.
 
 `correct`: 
     A boolean indicating whether to apply continuity correction when computing the test statistic for 2x2 tables: 
-    one half is subtracted from all |O-E| differences; however, the correction will not be bigger than the differences themselves. The default is True.
+    one half is subtracted from all abs(O-E) differences; however, the correction will not be bigger than the differences themselves. The default is True.
 
 `rescale_p`: boolean
     A boolean; if True then p is rescaled (if necessary) to sum to 1. If rescale_p is False, and p does not sum to 1, an error is raised.
 
 Details
 -------
     If x is a matrix with one row or column, or if x is a list and y is not given, then a goodness-of-fit test is performed 
@@ -676,39 +627,43 @@
 
     `expected`:
         The expected counts under the null hypothesis.
 
 
 Examples
 --------
-```python
-## From Agresti(2007) p.39
-M = [[762, 327, 468], [484, 239, 477]]
-result1 = chisq_test(M)
-print(result1)
-
-## Effect of rescale_p
-x = [12, 5, 7, 7]
-p = [0.4, 0.4, 0.2, 0.2]
-result2 = chisq_test(x, p=p, rescale_p=True)
-print(result2)
-
-## Testing for population probabilities
-x = [20, 15, 25]
-result31 = chisq_test(x)
-print(result31)
-
-x = [89,37,30,28,2]
-p = [0.40,0.20,0.20,0.19,0.01]
-result32 = chisq_test(x, p=p)
-print(result32)
-
-
-# Goodness of fit
-x = [1, 2, 3, 4, 5, 6]
-y = [6, 1, 2, 3, 4, 5]
-result4 = chisq_test(x, y)
-print(result4)
-```
+
+From Agresti(2007) p.39
+
+>>> M = [[762, 327, 468], [484, 239, 477]]
+>>> result1 = chisq_test(M)
+>>> print(result1)
+
+Effect of rescale_p
+
+>>> x = [12, 5, 7, 7]
+>>> p = [0.4, 0.4, 0.2, 0.2]
+>>> result2 = chisq_test(x, p=p, rescale_p=True)
+>>> print(result2)
+
+Testing for population probabilities
+
+>>> x = [20, 15, 25]
+>>> result31 = chisq_test(x)
+>>> print(result31)
+
+A second example of testing for population probabilities
+
+>>> x = [89,37,30,28,2]
+>>> p = [0.40,0.20,0.20,0.19,0.01]
+>>> result32 = chisq_test(x, p=p)
+>>> print(result32)
+
+Goodness of fit
+
+>>> x = [1, 2, 3, 4, 5, 6]
+>>> y = [6, 1, 2, 3, 4, 5]
+>>> result4 = chisq_test(x, y)
+>>> print(result4)
     """
 
     return __chisq_test(x, y, p, correct, rescale_p)
```

### Comparing `estyp-0.5.0/estyp/testing/__base/__init__.py` & `estyp-0.5.1/estyp/testing/__base/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from statsmodels.genmod.families.family import Gaussian
 from statsmodels.stats.diagnostic import (acorr_breusch_godfrey,
                                           acorr_ljungbox, het_breuschpagan,
                                           het_goldfeldquandt, het_white)
 from statsmodels.stats.outliers_influence import variance_inflation_factor
 from statsmodels.stats.stattools import (durbin_watson, jarque_bera,
                                          omni_normtest)
+from estyp.linear_model import LogisticRegression
 
 
 class bcolors:
     HEADER = "\033[95m"
     OKGREEN = "\033[92m"
     WARNING = "\033[93m"
     FAIL = "\033[91m"
@@ -280,50 +281,50 @@
         # p-value
         p_value = self.p_value
         if p_value < 0.0001:
             p_value = "<0.0001"
         else:
             p_value = f"{p_value:0.4f}"
         # df
-        if self.__dict__.get("df"):
+        if self.__dict__.get("df") is not None:
             df = self.df
             if isinstance(df, (float, int)):
                 if df == float(int(df)):
                     df = int(df)
                 else:
                     df = f"{df:0.2f}"
             elif isinstance(df, dict):
                 df = {k: round(v, 2) for k, v in df.items()}
             elif isinstance(df, float):
                 df = f"{df:0.2f}"
         else:
             df = None
         # estimates
-        if self.__dict__.get("estimate"):
+        if self.__dict__.get("estimate") is not None:
             estimate = self.estimate
             if isinstance(estimate, (list, np.ndarray)):
                 estimate = [float(f"{e:0.6f}") for e in estimate]
             elif estimate == float(int(estimate)):
                 estimate = int(estimate)
             elif isinstance(estimate, float):
                 estimate = f"{estimate:0.6f}"
 
         string = f"""
     {bcolors.BOLD + bcolors.UNDERLINE + self.method + bcolors.ENDC}
     {self.__names['statistic']} = {self.statistic:0.4f} |{' df: ' + str(df) + ' |' if df is not None else ''} p-value = {p_value}
     alternative hypothesis: {self.__names["alternative"]}"""
-        if self.__dict__.get("conf_int"):
+        if self.__dict__.get("conf_int") is not None:
             if self.conf_int is not None:
                 cl = self.conf_level * 100
                 if cl == float(int(cl)):
                     cl = int(cl)
                 string += f"""
     {cl} percent confidence interval:
     {" "}{self.conf_int[0]:0.6f} {self.conf_int[1]:0.6f}"""
-        if self.__dict__.get("estimate"):
+        if self.__dict__.get("estimate") is not None:
             string += f"""
     sample estimates:
     {" " * 2}{self.__names["estimate"]}: {estimate}
     """
         return string
 
 
@@ -466,44 +467,58 @@
         "alternative": alternative,
     }
 
     return TestResults(res, names)
 
 
 def __deviance(fitted_model, response):
-    if isinstance(fitted_model.model, OLS):
-        return Gaussian().deviance(endog=response, mu=fitted_model.fittedvalues)
-    elif isinstance(fitted_model.model, GLM):
+    try:
+        fitted_model.model
+        ok = True
+    except:
+        ok = False
+    if ok:
+        if isinstance(fitted_model.model, OLS):
+            return Gaussian().deviance(endog=response, mu=fitted_model.fittedvalues)
+        elif isinstance(fitted_model.model, GLM):
+            return fitted_model.deviance
+        else:
+            return sum(fitted_model.resid_dev ** 2)
+    else:
         return fitted_model.deviance
-    return sum(fitted_model.resid_dev ** 2) 
 
 
 def __nested_models_test(fitted_small_model, fitted_big_model):
-    response = fitted_big_model.model.data.endog
-    n = fitted_big_model.fittedvalues.shape[0]
+    try:
+        response = fitted_big_model.model.data.endog
+    except:
+        response = fitted_big_model.y
+        
+    n = response.shape[0]
     p_big = fitted_big_model.params.shape[0] - 1
     p_small = fitted_small_model.params.shape[0] - 1
     d_big = __deviance(fitted_big_model, response)
     d_small = __deviance(fitted_small_model, response)
     df_num = p_big - p_small
     df_den = n - p_big - 1
     f_num = (d_small - d_big) / df_num
     f_den = d_big / df_den
     f_stat = f_num / f_den
     p_value = fisher(dfn=df_num, dfd=df_den).sf(f_stat)
+    diff_dev = float(d_small - d_big)
     names = {
         "statistic": "F",
         "estimate": "Difference in deviances between models",
         "alternative": "big model is true",
     }
 
     res = {
         "method": "Nested models F-test",
         "statistic": f_stat,
-        "estimate": d_small - d_big,
+        "estimate": diff_dev,
         "df": {"df_num": df_num, "df_den": df_den},
         "p_value": p_value,
     }
 
     return TestResults(res, names)
```

### Comparing `estyp-0.5.0/.gitignore` & `estyp-0.5.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 instance/
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
-docs/_build/
+#docs/_build/
 
 # PyBuilder
 .pybuilder/
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `estyp-0.5.0/LICENSE` & `estyp-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `estyp-0.5.0/README.md` & `estyp-0.5.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,32 @@
 # ESTYP: Extended Statistical Toolkit Yet Practical
 
-[![Downloads](https://static.pepy.tech/badge/estyp)](https://pepy.tech/project/estyp) [![PyPI version](https://badge.fury.io/py/estyp.svg)](https://badge.fury.io/py/estyp) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Contributions](https://img.shields.io/badge/Contributions-welcome-blue.svg)](https://github.com/estebanrucan/estyp/issues) [![Chilean](https://img.shields.io/badge/Made_in-%F0%9F%87%A8%F0%9F%87%B1_Chile-blue.svg)](https://es.wikipedia.org/wiki/Chile)
+[![Downloads](https://static.pepy.tech/badge/estyp)](https://pepy.tech/project/estyp) [![Documentation Status](https://readthedocs.org/projects/estyp/badge/?version=latest)](https://estyp.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/estyp.svg)](https://badge.fury.io/py/estyp) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Contributions](https://img.shields.io/badge/Contributions-welcome-blue.svg)](https://github.com/estebanrucan/estyp/issues) [![Chilean](https://img.shields.io/badge/Made_in-%F0%9F%87%A8%F0%9F%87%B1_Chile-blue.svg)](https://es.wikipedia.org/wiki/Chile)
 
 ## Description
 
-This library is a collection of statistical functions for Python.
+ESTYP (Extended Statistical Toolkit Yet Practical) is a Python library that serves as a multifaceted toolkit for statistical analysis. The `testing` module encompasses a wide range of statistical tests, including t-tests, chi-squared tests, and correlation tests, providing robust methods for data comparison and validation. In the `linear_model` module, users can find functionalities related to logistic regression, including variable selection techniques and additional methods for calculating confidence intervals and p-values. This module enhances the capabilities of traditional logistic regression analysis. The cluster module is designed to assist in clustering analysis, offering tools to identify the optimal number of `clusters` using methods like the elbow or silhouette techniques. Together, these modules form a comprehensive and practical statistical toolkit that caters to various analytical needs. 
 
 Actually, the name comes from the way my friends call me (Esti), plus "p" which is the initial of `python`.
 
-## Changelog 
+## Installation
+
+To install this library, you can use PyPI:
+
+```bash
+pip install estyp
+```
+
+## Documentation
+
+You can have a friendly introduction to this library in the [documentation](https://estyp.readthedocs.io/en/latest/).
 
-### V0.5.0
+## Changelog
 
-* Added `testing.chisq_test()` function to perform a chi-squared test.
-* Added `testing.cor_test()` function to perform a correlation test.
-* Added `cluster.NClusterSearch()` class to identify the optimal number of clusters for clustering algorithms with elbow or silhuette methods.
-* Added `kmodes >= 0.12.2` as a depedency of the library.
-* Added `__version__` atribute to the library.
-* Changed method displaying in `TestResults` class.
-* Minor changes in README.
-
-### V0.4.1
-
-* Bug fixes in `linear_model.LogisticRegression()` class.
-* Added downloads badge to README.
-* Changed `sklearn>=1.2.1` to `sklearn>=1.3.0` as a depedency of the library.
-
-### V0.4.0
-
-* Added `testing.prop_test()` function to perform a test of proportions.
-* Added `testing.CheckModel()` class to perform linear regression assumptions checking.
-* Added badges to README.
-* Minor changes in README.
-
-### V0.3.0
-
-* Changed `scipy>=1.11.1` to `scipy>=1.10.1` as a depedency of the library.
-* New modularization of the functions in the `linear_model` module.
-* Added `linear_model.stepwise.forward_selection()` function to perform forward variable selection based in p-values.
-* Added `testing.nested_models_test()` function to perform nested models testing.
-* Added option to specity aditional parameters of the model like `kwargs` in `linear_model.stepwise.forward_selection()` and `linear_model.stepwise.both_selection()` functions.  
-* Minor changes in README.
-
-### V0.2.5
-
-* Added `scipy>=1.11.1` as a depedency of the library.
-* New modularization of the functions in the `testing` module.
-* R like documentation in the `testing.var_test()` function.
-* Added `testing.t_test()` function to perform t-test like in software R.
+You can see the changelog [here](./CHANGELOG.md)
 
 ## Features
 
 ### `testing` module
 
 * `testing.CheckModel()`: This class provides methods to test the assumptions of the linear regression model., inspired by the `performance::check_model()` function of the R software.
 * `testing.t_test()`: Performs one and two sample t-tests on groups of data. This function is inspired by the `t.test()` function of the R software.
@@ -68,22 +43,14 @@
 * `linear_model.stepwise.forward_selection()`: This function performs forward variable selection based on p-values.
 
 ### `cluster` module
 
 * `cluster.NClusterSearch`: A helper class to identify the optimal number of clusters for clustering algorithms with elbow or silhuette methods.
 
 
-## Installation
-
-To install this library, you can use PyPI:
-
-```bash
-pip install estyp
-```
-
 ## License
 
 This library is under the MIT license.
 
 ## Contact
 
-If you have any questions about this library, you can contact me at [errucan@gmail.com](mailto:errucan@gmail.com).
+If you have any questions about this library, you can contact me at [LinkedIn](https://www.linkedin.com/in/estebanrucan/).
```

### Comparing `estyp-0.5.0/pyproject.toml` & `estyp-0.5.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "estyp"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
     { name="estebanrucan", email="errucan@gmail.com" },
 ]
 description = "Extended Statistical Toolkit Yet Practical"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9.12"
@@ -20,13 +20,14 @@
 dependencies = [
     "numpy >= 1.22.3",
     "scikit-learn >= 1.3.0",
     "matplotlib >= 3.4.3",
     "patsy >= 0.5.3",
     "statsmodels >= 0.13.5",
     "scipy >= 1.10.1",
-    "kmodes >= 0.12.2"
+    "kmodes >= 0.12.2",
+    "tqdm >= 4.65.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/estebanrucan/estyp"
 "Bug Tracker" = "https://github.com/estebanrucan/estyp/issues"
```

### Comparing `estyp-0.5.0/PKG-INFO` & `estyp-0.5.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estyp
-Version: 0.5.0
+Version: 0.5.1
 Summary: Extended Statistical Toolkit Yet Practical
 Project-URL: Homepage, https://github.com/estebanrucan/estyp
 Project-URL: Bug Tracker, https://github.com/estebanrucan/estyp/issues
 Author-email: estebanrucan <errucan@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Esteban Rucán Carrasco
@@ -34,66 +34,42 @@
 Requires-Dist: kmodes>=0.12.2
 Requires-Dist: matplotlib>=3.4.3
 Requires-Dist: numpy>=1.22.3
 Requires-Dist: patsy>=0.5.3
 Requires-Dist: scikit-learn>=1.3.0
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: statsmodels>=0.13.5
+Requires-Dist: tqdm>=4.65.0
 Description-Content-Type: text/markdown
 
 # ESTYP: Extended Statistical Toolkit Yet Practical
 
-[![Downloads](https://static.pepy.tech/badge/estyp)](https://pepy.tech/project/estyp) [![PyPI version](https://badge.fury.io/py/estyp.svg)](https://badge.fury.io/py/estyp) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Contributions](https://img.shields.io/badge/Contributions-welcome-blue.svg)](https://github.com/estebanrucan/estyp/issues) [![Chilean](https://img.shields.io/badge/Made_in-%F0%9F%87%A8%F0%9F%87%B1_Chile-blue.svg)](https://es.wikipedia.org/wiki/Chile)
+[![Downloads](https://static.pepy.tech/badge/estyp)](https://pepy.tech/project/estyp) [![Documentation Status](https://readthedocs.org/projects/estyp/badge/?version=latest)](https://estyp.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/estyp.svg)](https://badge.fury.io/py/estyp) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Contributions](https://img.shields.io/badge/Contributions-welcome-blue.svg)](https://github.com/estebanrucan/estyp/issues) [![Chilean](https://img.shields.io/badge/Made_in-%F0%9F%87%A8%F0%9F%87%B1_Chile-blue.svg)](https://es.wikipedia.org/wiki/Chile)
 
 ## Description
 
-This library is a collection of statistical functions for Python.
+ESTYP (Extended Statistical Toolkit Yet Practical) is a Python library that serves as a multifaceted toolkit for statistical analysis. The `testing` module encompasses a wide range of statistical tests, including t-tests, chi-squared tests, and correlation tests, providing robust methods for data comparison and validation. In the `linear_model` module, users can find functionalities related to logistic regression, including variable selection techniques and additional methods for calculating confidence intervals and p-values. This module enhances the capabilities of traditional logistic regression analysis. The cluster module is designed to assist in clustering analysis, offering tools to identify the optimal number of `clusters` using methods like the elbow or silhouette techniques. Together, these modules form a comprehensive and practical statistical toolkit that caters to various analytical needs. 
 
 Actually, the name comes from the way my friends call me (Esti), plus "p" which is the initial of `python`.
 
-## Changelog 
+## Installation
+
+To install this library, you can use PyPI:
+
+```bash
+pip install estyp
+```
+
+## Documentation
+
+You can have a friendly introduction to this library in the [documentation](https://estyp.readthedocs.io/en/latest/).
 
-### V0.5.0
+## Changelog
 
-* Added `testing.chisq_test()` function to perform a chi-squared test.
-* Added `testing.cor_test()` function to perform a correlation test.
-* Added `cluster.NClusterSearch()` class to identify the optimal number of clusters for clustering algorithms with elbow or silhuette methods.
-* Added `kmodes >= 0.12.2` as a depedency of the library.
-* Added `__version__` atribute to the library.
-* Changed method displaying in `TestResults` class.
-* Minor changes in README.
-
-### V0.4.1
-
-* Bug fixes in `linear_model.LogisticRegression()` class.
-* Added downloads badge to README.
-* Changed `sklearn>=1.2.1` to `sklearn>=1.3.0` as a depedency of the library.
-
-### V0.4.0
-
-* Added `testing.prop_test()` function to perform a test of proportions.
-* Added `testing.CheckModel()` class to perform linear regression assumptions checking.
-* Added badges to README.
-* Minor changes in README.
-
-### V0.3.0
-
-* Changed `scipy>=1.11.1` to `scipy>=1.10.1` as a depedency of the library.
-* New modularization of the functions in the `linear_model` module.
-* Added `linear_model.stepwise.forward_selection()` function to perform forward variable selection based in p-values.
-* Added `testing.nested_models_test()` function to perform nested models testing.
-* Added option to specity aditional parameters of the model like `kwargs` in `linear_model.stepwise.forward_selection()` and `linear_model.stepwise.both_selection()` functions.  
-* Minor changes in README.
-
-### V0.2.5
-
-* Added `scipy>=1.11.1` as a depedency of the library.
-* New modularization of the functions in the `testing` module.
-* R like documentation in the `testing.var_test()` function.
-* Added `testing.t_test()` function to perform t-test like in software R.
+You can see the changelog [here](./CHANGELOG.md)
 
 ## Features
 
 ### `testing` module
 
 * `testing.CheckModel()`: This class provides methods to test the assumptions of the linear regression model., inspired by the `performance::check_model()` function of the R software.
 * `testing.t_test()`: Performs one and two sample t-tests on groups of data. This function is inspired by the `t.test()` function of the R software.
@@ -110,22 +86,14 @@
 * `linear_model.stepwise.forward_selection()`: This function performs forward variable selection based on p-values.
 
 ### `cluster` module
 
 * `cluster.NClusterSearch`: A helper class to identify the optimal number of clusters for clustering algorithms with elbow or silhuette methods.
 
 
-## Installation
-
-To install this library, you can use PyPI:
-
-```bash
-pip install estyp
-```
-
 ## License
 
 This library is under the MIT license.
 
 ## Contact
 
-If you have any questions about this library, you can contact me at [errucan@gmail.com](mailto:errucan@gmail.com).
+If you have any questions about this library, you can contact me at [LinkedIn](https://www.linkedin.com/in/estebanrucan/).
```

