# Comparing `tmp/empyrial-2.0.9.tar.gz` & `tmp/empyrial-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empyrial-2.0.9.tar", last modified: Wed Jul  5 03:04:05 2023, max compression
+gzip compressed data, was "empyrial-2.1.0.tar", last modified: Mon Aug  7 22:35:44 2023, max compression
```

## Comparing `empyrial-2.0.9.tar` & `empyrial-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:04:05.947246 empyrial-2.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 03:04:05.947246 empyrial-2.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-07-05 03:03:19.000000 empyrial-2.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-05 03:03:19.000000 empyrial-2.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-05 03:04:05.947246 empyrial-2.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:04:05.947246 empyrial-2.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:04:05.947246 empyrial-2.0.9/src/empyrial/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-05 03:03:19.000000 empyrial-2.0.9/src/empyrial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36808 2023-07-05 03:03:19.000000 empyrial-2.0.9/src/empyrial/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:04:05.947246 empyrial-2.0.9/src/empyrial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 03:04:05.000000 empyrial-2.0.9/src/empyrial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-05 03:04:05.000000 empyrial-2.0.9/src/empyrial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 03:04:05.000000 empyrial-2.0.9/src/empyrial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-05 03:04:05.000000 empyrial-2.0.9/src/empyrial.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 03:04:05.000000 empyrial-2.0.9/src/empyrial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 03:04:05.000000 empyrial-2.0.9/src/empyrial.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:35:44.546123 empyrial-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-07 22:35:44.546123 empyrial-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-08-07 22:35:08.000000 empyrial-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-07 22:35:08.000000 empyrial-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-07 22:35:44.546123 empyrial-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:35:44.542123 empyrial-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:35:44.546123 empyrial-2.1.0/src/empyrial/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 22:35:08.000000 empyrial-2.1.0/src/empyrial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38569 2023-08-07 22:35:08.000000 empyrial-2.1.0/src/empyrial/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:35:44.546123 empyrial-2.1.0/src/empyrial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-07 22:35:44.000000 empyrial-2.1.0/src/empyrial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-07 22:35:44.000000 empyrial-2.1.0/src/empyrial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 22:35:44.000000 empyrial-2.1.0/src/empyrial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-07 22:35:44.000000 empyrial-2.1.0/src/empyrial.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-07 22:35:44.000000 empyrial-2.1.0/src/empyrial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 22:35:44.000000 empyrial-2.1.0/src/empyrial.egg-info/top_level.txt
```

### Comparing `empyrial-2.0.9/README.md` & `empyrial-2.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <br><br><br><br>
 <div align="center">
 <img src="https://user-images.githubusercontent.com/61618641/120909011-98f8a180-c670-11eb-8844-2d423ba3fa9c.png"/>
 <br><br><br><br><br><br>
   
 ![](https://img.shields.io/badge/Downloads-101k-brightgreen)
 ![](https://img.shields.io/badge/license-MIT-orange)
-![](https://img.shields.io/badge/version-2.0.1-blueviolet)
+![](https://img.shields.io/badge/version-2.0.9-blueviolet)
 ![](https://img.shields.io/badge/language-python🐍-blue)
 ![](https://img.shields.io/badge/activity-9.7/10-ff69b4)
 ![](https://img.shields.io/badge/Open%20source-💜-white)	
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1NqTkkP2u1p1g8W8erU-Y-rSSVbPUDvq2?usp=sharing)
   
  </div>
```

### Comparing `empyrial-2.0.9/setup.cfg` & `empyrial-2.1.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = empyrial
-version = 2.0.9
+version = 2.1.0
 description = An Open Source Portfolio Management Framework for Everyone 投资组合管理
 url = https://github.com/ssantoshp/Empyrial
 long_description_content_type = text/markdown
 long_descript = # Empyrial
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: BSD License
```

### Comparing `empyrial-2.0.9/src/empyrial/main.py` & `empyrial-2.1.0/src/empyrial/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,14 +61,16 @@
         weights=None,
         rebalance=None,
         benchmark=None,
         end_date=TODAY,
         optimizer=None,
         max_vol=0.15,
         diversification=1,
+        expected_returns=None,
+        risk_model=None,
         # confidences=None,
         # view=None,
         min_weights=None,
         max_weights=None,
         risk_manager=None,
         data=None,
     ):
@@ -80,14 +82,20 @@
         self.portfolio = portfolio
         self.weights = weights
         self.benchmark = benchmark
         self.optimizer = optimizer
         self.rebalance = rebalance
         self.max_vol = max_vol
         self.diversification = diversification
+        self.expected_returns = expected_returns
+        if expected_returns is not None:
+            assert expected_returns in ["mean_historical_return", "ema_historical_return", "capm_return"], f"Expected return method: {expected_returns} not supported yet!"
+        self.risk_model = risk_model
+        if risk_model is not None:
+            assert risk_model in ["sample_cov", "semicovariance", "exp_cov", "ledoit_wolf", "ledoit_wolf_constant_variance", "ledoit_wolf_single_factor", "ledoit_wolf_constant_correlation", "oracle_approximating"], f"Risk model: {risk_model} not supported yet!"
         self.max_weights = max_weights
         self.min_weights = min_weights
         self.risk_manager = risk_manager
         self.data = data
 
         optimizers = {
             "EF": efficient_frontier,
@@ -111,34 +119,42 @@
                 self.portfolio,
                 self.rebalance,
                 self.weights,
                 self.max_vol,
                 self.diversification,
                 self.min_weights,
                 self.max_weights,
+                self.expected_returns,
+                self.risk_model
             )
 
 
 def get_returns(stocks, wts, start_date, end_date=TODAY):
     if len(stocks) > 1:
         assets = yf.download(stocks, start=start_date, end=end_date, progress=False)["Adj Close"]
         assets = assets.filter(stocks)
-        ret_data = assets.pct_change()[1:]
-        returns = (ret_data * wts).sum(axis=1)
+        initial_alloc = wts/assets.iloc[0]
+        if initial_alloc.isna().any():
+            raise ValueError("Some stock is not available at initial state!")
+        portfolio_value = (assets * initial_alloc).sum(axis=1)
+        returns = portfolio_value.pct_change()[1:]
         return returns
     else:
         df = yf.download(stocks, start=start_date, end=end_date, progress=False)["Adj Close"]
         df = pd.DataFrame(df)
-        returns = df.pct_change()
+        returns = df.pct_change()[1:]
         return returns
 
 
 def get_returns_from_data(data, wts):
-    ret_data = data.pct_change()[1:]
-    returns = (ret_data * wts).sum(axis=1)
+    initial_alloc = wts/data.iloc[0]
+    if initial_alloc.isna().any():
+        raise ValueError("Some stock is not available at initial state!")
+    portfolio_value = (data * initial_alloc).sum(axis=1)
+    returns = portfolio_value.pct_change()[1:]
     return returns
 
 
 def calculate_information_ratio(returns, benchmark_returns, days=252) -> float:
     return_difference = returns - benchmark_returns
     volatility = return_difference.std() * np.sqrt(days)
     information_ratio_result = return_difference.mean() / volatility
@@ -531,20 +547,20 @@
     )
     prices = ohlc["Adj Close"].dropna(how="all")
     df = prices.filter(my_portfolio.portfolio)
 
     # sometimes we will pick a date range where company isn't public we can't set price to 0 so it has to go to 1
     df = df.fillna(1)
 
-    mu = expected_returns.mean_historical_return(df)
-    S = risk_models.sample_cov(df)
+    mu = expected_returns.return_model(df, method=my_portfolio.expected_returns)
+    S = risk_models.risk_matrix(df, method=my_portfolio.risk_model)
 
     # optimize for max sharpe ratio
     ef = EfficientFrontier(mu, S)
-
+    ef.add_objective(objective_functions.L2_reg, gamma=my_portfolio.diversification)
     if my_portfolio.min_weights is not None:
         ef.add_constraint(lambda x: x >= my_portfolio.min_weights)
     if my_portfolio.max_weights is not None:
         ef.add_constraint(lambda x: x <= my_portfolio.max_weights)
     weights = ef.max_sharpe()
     cleaned_weights = ef.clean_weights()
     wts = cleaned_weights.items()
@@ -604,16 +620,16 @@
     )
     prices = ohlc["Adj Close"].dropna(how="all")
     prices = prices.filter(my_portfolio.portfolio)
 
     # sometimes we will pick a date range where company isn't public we can't set price to 0 so it has to go to 1
     prices = prices.fillna(1)
 
-    mu = expected_returns.capm_return(prices)
-    S = risk_models.CovarianceShrinkage(prices).ledoit_wolf()
+    mu = expected_returns.return_model(prices, method=my_portfolio.expected_returns)
+    S = risk_models.risk_matrix(prices, method=my_portfolio.risk_model)
 
     ef = EfficientFrontier(mu, S)
     ef.add_objective(objective_functions.L2_reg, gamma=my_portfolio.diversification)
     if my_portfolio.min_weights is not None:
         ef.add_constraint(lambda x: x >= my_portfolio.min_weights)
     if my_portfolio.max_weights is not None:
         ef.add_constraint(lambda x: x <= my_portfolio.max_weights)
@@ -639,16 +655,16 @@
         start=my_portfolio.start_date,
         end=my_portfolio.end_date,
         progress=False,
     )
     prices = ohlc["Adj Close"].dropna(how="all")
     prices = prices.filter(my_portfolio.portfolio)
 
-    mu = expected_returns.capm_return(prices)
-    S = risk_models.CovarianceShrinkage(prices).ledoit_wolf()
+    mu = expected_returns.return_model(prices, method=my_portfolio.expected_returns)
+    S = risk_models.risk_matrix(prices, method=my_portfolio.risk_model)
 
     ef = EfficientFrontier(mu, S)
     ef.add_objective(objective_functions.L2_reg, gamma=my_portfolio.diversification)
     if my_portfolio.min_weights is not None:
         ef.add_constraint(lambda x: x >= my_portfolio.min_weights)
     if my_portfolio.max_weights is not None:
         ef.add_constraint(lambda x: x <= my_portfolio.max_weights)
@@ -790,14 +806,16 @@
     portfolio_input,
     rebalance,
     allocation,
     vol_max,
     div,
     min,
     max,
+    expected_returns,
+    risk_model,
 ) -> pd.DataFrame:
     sdate = str(start_date)[:10]
     if rebalance[0] != sdate:
 
         # makes sure the start date matches the first element of the list of custom rebalance dates
         if type(rebalance) is list:
             raise KeyError("the rebalance dates and start date doesn't match")
@@ -832,27 +850,31 @@
                 portfolio=portfolio_input,
                 weights=allocation,
                 optimizer="{}".format(optimize),
                 max_vol=vol_max,
                 diversification=div,
                 min_weights=min,
                 max_weights=max,
+                expected_returns=expected_returns,
+                risk_model=risk_model,
             )
 
         except TypeError:
             portfolio = Engine(
                 start_date=dates[0],
                 end_date=dates[i + 1],
                 portfolio=portfolio_input,
                 weights=allocation,
                 optimizer=optimize,
                 max_vol=vol_max,
                 diversification=div,
                 min_weights=min,
                 max_weights=max,
+                expected_returns=expected_returns,
+                risk_model=risk_model,
             )
 
         output_df["{}".format(dates[i + 1])] = portfolio.weights
 
     # we have to run it one more time to get what the optimization is for up to today's date
     try:
         portfolio = Engine(
@@ -860,31 +882,37 @@
             portfolio=portfolio_input,
             weights=allocation,
             optimizer="{}".format(optimize),
             max_vol=vol_max,
             diversification=div,
             min_weights=min,
             max_weights=max,
+            expected_returns=expected_returns,
+            risk_model=risk_model,
         )
 
     except TypeError:
         portfolio = Engine(
             start_date=dates[0],
             portfolio=portfolio_input,
             weights=allocation,
             optimizer=optimize,
             max_vol=vol_max,
             diversification=div,
             min_weights=min,
             max_weights=max,
+            expected_returns=expected_returns,
+            risk_model=risk_model,
         )
 
     output_df["{}".format(TODAY)] = portfolio.weights
 
     make_rebalance.output = output_df
+    print("Rebalance schedule: ")
+    print(output_df)
     return output_df
 
 
 def get_report(my_portfolio, rf=0.0, sigma_value=1, confidence_value=0.95, filename : str ="report.pdf"):
     try:
         # we want to get the dataframe with the dates and weights
         rebalance_schedule = my_portfolio.rebalance
```

