# Comparing `tmp/nixtlats-0.1.3.tar.gz` & `tmp/nixtlats-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nixtlats-0.1.3.tar", last modified: Mon Aug  7 09:04:18 2023, max compression
+gzip compressed data, was "nixtlats-0.1.4.tar", last modified: Tue Aug  8 09:36:45 2023, max compression
```

## Comparing `nixtlats-0.1.3.tar` & `nixtlats-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:04:18.356775 nixtlats-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-07 09:03:58.000000 nixtlats-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-07 09:04:18.356775 nixtlats-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-08-07 09:03:58.000000 nixtlats-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:04:18.356775 nixtlats-0.1.3/nixtlats/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 09:03:58.000000 nixtlats-0.1.3/nixtlats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-08-07 09:03:58.000000 nixtlats-0.1.3/nixtlats/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-08-07 09:03:58.000000 nixtlats-0.1.3/nixtlats/timegpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:04:18.356775 nixtlats-0.1.3/nixtlats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-07 09:04:18.000000 nixtlats-0.1.3/nixtlats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-07 09:04:18.000000 nixtlats-0.1.3/nixtlats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:04:18.000000 nixtlats-0.1.3/nixtlats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 09:04:18.000000 nixtlats-0.1.3/nixtlats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 09:04:18.000000 nixtlats-0.1.3/nixtlats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 09:04:18.356775 nixtlats-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-07 09:03:58.000000 nixtlats-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:36:45.910358 nixtlats-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-08 09:36:34.000000 nixtlats-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-08 09:36:45.910358 nixtlats-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-08-08 09:36:34.000000 nixtlats-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:36:45.910358 nixtlats-0.1.4/nixtlats/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-08 09:36:34.000000 nixtlats-0.1.4/nixtlats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-08-08 09:36:34.000000 nixtlats-0.1.4/nixtlats/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14109 2023-08-08 09:36:34.000000 nixtlats-0.1.4/nixtlats/timegpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:36:45.910358 nixtlats-0.1.4/nixtlats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-08 09:36:45.000000 nixtlats-0.1.4/nixtlats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-08 09:36:45.000000 nixtlats-0.1.4/nixtlats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 09:36:45.000000 nixtlats-0.1.4/nixtlats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 09:36:45.000000 nixtlats-0.1.4/nixtlats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 09:36:45.000000 nixtlats-0.1.4/nixtlats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 09:36:45.910358 nixtlats-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-08 09:36:34.000000 nixtlats-0.1.4/setup.py
```

### Comparing `nixtlats-0.1.3/LICENSE` & `nixtlats-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nixtlats-0.1.3/PKG-INFO` & `nixtlats-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nixtlats
-Version: 0.1.3
+Version: 0.1.4
 Summary: Nixtla SDK
 Home-page: https://github.com/Nixtla/nixtla
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `nixtlats-0.1.3/README.md` & `nixtlats-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nixtlats-0.1.3/nixtlats/_modidx.py` & `nixtlats-0.1.4/nixtlats/_modidx.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,21 +3,31 @@
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/nixtlats/',
                 'doc_host': 'https://Nixtla.github.io',
                 'git_url': 'https://github.com/Nixtla/nixtla/',
                 'lib_path': 'nixtlats'},
   'syms': { 'nixtlats.timegpt': { 'nixtlats.timegpt.TimeGPT': ('timegpt.html#timegpt', 'nixtlats/timegpt.py'),
                                   'nixtlats.timegpt.TimeGPT.__init__': ('timegpt.html#timegpt.__init__', 'nixtlats/timegpt.py'),
+                                  'nixtlats.timegpt.TimeGPT._get_to_dict_args': ( 'timegpt.html#timegpt._get_to_dict_args',
+                                                                                  'nixtlats/timegpt.py'),
+                                  'nixtlats.timegpt.TimeGPT._hit_multi_series_endpoint': ( 'timegpt.html#timegpt._hit_multi_series_endpoint',
+                                                                                           'nixtlats/timegpt.py'),
+                                  'nixtlats.timegpt.TimeGPT._hit_multi_series_historic_endpoint': ( 'timegpt.html#timegpt._hit_multi_series_historic_endpoint',
+                                                                                                    'nixtlats/timegpt.py'),
                                   'nixtlats.timegpt.TimeGPT._infer_freq': ('timegpt.html#timegpt._infer_freq', 'nixtlats/timegpt.py'),
-                                  'nixtlats.timegpt.TimeGPT._input_size': ('timegpt.html#timegpt._input_size', 'nixtlats/timegpt.py'),
+                                  'nixtlats.timegpt.TimeGPT._model_params': ('timegpt.html#timegpt._model_params', 'nixtlats/timegpt.py'),
                                   'nixtlats.timegpt.TimeGPT._multi_series': ('timegpt.html#timegpt._multi_series', 'nixtlats/timegpt.py'),
                                   'nixtlats.timegpt.TimeGPT._parse_response': ( 'timegpt.html#timegpt._parse_response',
                                                                                 'nixtlats/timegpt.py'),
-                                  'nixtlats.timegpt.TimeGPT._preprocess_inputs': ( 'timegpt.html#timegpt._preprocess_inputs',
-                                                                                   'nixtlats/timegpt.py'),
+                                  'nixtlats.timegpt.TimeGPT._preprocess_dataframes': ( 'timegpt.html#timegpt._preprocess_dataframes',
+                                                                                       'nixtlats/timegpt.py'),
+                                  'nixtlats.timegpt.TimeGPT._resample_dataframe': ( 'timegpt.html#timegpt._resample_dataframe',
+                                                                                    'nixtlats/timegpt.py'),
+                                  'nixtlats.timegpt.TimeGPT._transform_dataframes': ( 'timegpt.html#timegpt._transform_dataframes',
+                                                                                      'nixtlats/timegpt.py'),
                                   'nixtlats.timegpt.TimeGPT._validate_inputs': ( 'timegpt.html#timegpt._validate_inputs',
                                                                                  'nixtlats/timegpt.py'),
                                   'nixtlats.timegpt.TimeGPT._validate_outputs': ( 'timegpt.html#timegpt._validate_outputs',
                                                                                   'nixtlats/timegpt.py'),
                                   'nixtlats.timegpt.TimeGPT.forecast': ('timegpt.html#timegpt.forecast', 'nixtlats/timegpt.py'),
                                   'nixtlats.timegpt.TimeGPT.request_headers': ( 'timegpt.html#timegpt.request_headers',
                                                                                 'nixtlats/timegpt.py'),
```

### Comparing `nixtlats-0.1.3/nixtlats/timegpt.py` & `nixtlats-0.1.4/nixtlats/timegpt.py`

 * *Files 15% similar despite different names*

```diff
@@ -60,32 +60,36 @@
         valid = True
         try:
             response = self._parse_response(response)
         except:
             valid = False
         return valid
 
-    def _input_size(self, freq: str):
+    def _model_params(self, freq: str):
         response_input_size = requests.post(
-            f"{self.api_url}/timegpt_input_size",
+            f"{self.api_url}/timegpt_model_params",
             json={"freq": freq},
             headers=self.request_headers,
         )
         response_input_size = self._parse_response(response_input_size)
-        return response_input_size["data"]
+        return response_input_size["data"]["detail"]
 
     def _validate_inputs(
         self,
         df: pd.DataFrame,
         X_df: pd.DataFrame,
         id_col: str,
         time_col: str,
         target_col: str,
     ):
-        renamer = {id_col: "unique_id", time_col: "ds", target_col: "y"}
+        renamer = {
+            id_col: "unique_id",
+            time_col: "ds",
+            target_col: "y",
+        }
         df = df.rename(columns=renamer)
         if df.dtypes.ds != "object":
             df["ds"] = df["ds"].astype(str)
         drop_uid = False
         if "unique_id" not in df.columns:
             # Insert unique_id column
             df = df.assign(unique_id="ts_0")
@@ -124,67 +128,112 @@
             raise Exception(
                 "Could not infer frequency of ds column. This could be due to "
                 "inconsistent intervals. Please check your data for missing, "
                 "duplicated or irregular timestamps"
             )
         return freq
 
-    def _preprocess_inputs(
+    def _resample_dataframe(
+        self,
+        df: pd.DataFrame,
+        freq: str,
+    ):
+        df = df.copy()
+        df["ds"] = pd.to_datetime(df["ds"])
+        resampled_df = df.set_index("ds").groupby("unique_id").resample(freq).bfill()
+        resampled_df = resampled_df.drop(columns="unique_id").reset_index()
+        resampled_df["ds"] = resampled_df["ds"].astype(str)
+        return resampled_df
+
+    def _preprocess_dataframes(
         self,
         df: pd.DataFrame,
         h: int,
+        X_df: Optional[pd.DataFrame],
         freq: str,
-        X_df: Optional[pd.DataFrame] = None,
     ):
-        input_size = self._input_size(freq)
+        """Returns Y_df and X_df dataframes in the structure expected by the endpoints."""
         y_cols = ["unique_id", "ds", "y"]
-        y = df[y_cols].groupby("unique_id").tail(input_size + h)
-        to_dict_args = {"orient": "split"}
-        if "index" in inspect.signature(pd.DataFrame.to_dict).parameters:
-            to_dict_args["index"] = False
-        if y["y"].isna().any():
+        Y_df = df[y_cols]
+        if Y_df["y"].isna().any():
             raise Exception("Your target variable contains NA, please check")
-        y = y.to_dict(**to_dict_args)
+        # Azul: efficient this code
+        # and think about returning dates that are not in the training set
+        Y_df = self._resample_dataframe(Y_df, freq)
         x_cols = []
-        if X_df is None:
-            x = None
-        else:
+        if X_df is not None:
             x_cols = X_df.drop(columns=["unique_id", "ds"]).columns.to_list()
             if not all(col in df.columns for col in x_cols):
                 raise Exception(
                     "You must include the exogenous variables in the `df` object, "
                     f'exogenous variables {",".join(x_cols)}'
                 )
-            x = (
-                df[["unique_id", "ds"] + x_cols]
-                .groupby("unique_id")
-                .tail(input_size + h)
-            )
-            x = pd.concat([x, X_df])
-            if x[x_cols].isna().any().any():
+            if len(X_df) != df["unique_id"].nunique() * h:
+                raise Exception(
+                    f"You have to pass the {h} future values of your "
+                    "exogenous variables for each time series"
+                )
+            X_df_history = df[["unique_id", "ds"] + x_cols]
+            X_df = pd.concat([X_df_history, X_df])
+            if X_df[x_cols].isna().any().any():
                 raise Exception(
                     "Some of your exogenous variables contain NA, please check"
                 )
-            x = x.sort_values(["unique_id", "ds"])
-            x = x.to_dict(**to_dict_args)
-        return y, x, x_cols
+            X_df = X_df.sort_values(["unique_id", "ds"]).reset_index(drop=True)
+            X_df = self._resample_dataframe(X_df, freq)
+        return Y_df, X_df, x_cols
 
-    def _multi_series(
+    def _get_to_dict_args(self):
+        to_dict_args = {"orient": "split"}
+        if "index" in inspect.signature(pd.DataFrame.to_dict).parameters:
+            to_dict_args["index"] = False
+        return to_dict_args
+
+    def _transform_dataframes(self, Y_df: pd.DataFrame, X_df: pd.DataFrame):
+        # contruction of y and x for the payload
+        to_dict_args = self._get_to_dict_args()
+        y = Y_df.to_dict(**to_dict_args)
+        x = X_df.to_dict(**to_dict_args) if X_df is not None else None
+        return y, x
+
+    def _hit_multi_series_endpoint(
         self,
-        df: pd.DataFrame,
+        Y_df: pd.DataFrame,
+        X_df: pd.DataFrame,
+        x_cols: List[str],
         h: int,
         freq: str,
-        X_df: Optional[pd.DataFrame] = None,
-        level: Optional[List[int]] = None,
-        finetune_steps: int = 0,
-        clean_ex_first: bool = True,
+        finetune_steps: int,
+        clean_ex_first: bool,
+        level: Optional[List[Union[int, float]]],
     ):
-        if freq is None:
-            freq = self._infer_freq(df)
-        y, x, x_cols = self._preprocess_inputs(df=df, h=h, freq=freq, X_df=X_df)
+        # restrict input only if we dont want
+        # to finetune the model
+        restrict_input = finetune_steps == 0
+        if restrict_input:
+            model_params = self._model_params(freq)
+            input_size, model_horizon = (
+                model_params["input_size"],
+                model_params["horizon"],
+            )
+            if level is not None:
+                # add sufficient info to compute
+                # conformal interval
+                input_size = 3 * input_size + max(model_horizon, h)
+        else:
+            input_size = model_horizon = None
+        # restricting the inputs if necessary
+        if restrict_input:
+            Y_df = Y_df.groupby("unique_id").tail(input_size)
+            if X_df is not None:
+                X_df = X_df.groupby("unique_id").tail(
+                    input_size + h
+                )  # history plus exogenous
+        y, x = self._transform_dataframes(Y_df, X_df)
+        # Contruct payload
         payload = dict(
             y=y,
             x=x,
             fh=h,
             freq=freq,
             level=level,
             finetune_steps=finetune_steps,
@@ -201,27 +250,88 @@
                 {
                     "features": x_cols,
                     "weights": response_timegpt["data"]["weights_x"],
                 }
             )
         return pd.DataFrame(**response_timegpt["data"]["forecast"])
 
+    def _hit_multi_series_historic_endpoint(
+        self,
+        Y_df: pd.DataFrame,
+        freq: str,
+        level: Optional[List[Union[int, float]]],
+    ):
+        y, x = self._transform_dataframes(Y_df, None)
+        # Contruct payload
+        payload = dict(
+            y=y,
+            freq=freq,
+            level=level,
+        )
+        response_timegpt = requests.post(
+            f"{self.api_url}/timegpt_multi_series_historic",
+            json=payload,
+            headers=self.request_headers,
+        )
+        response_timegpt = self._parse_response(response_timegpt)
+        return pd.DataFrame(**response_timegpt["data"]["forecast"])
+
+    def _multi_series(
+        self,
+        df: pd.DataFrame,
+        h: int,
+        freq: str,
+        X_df: Optional[pd.DataFrame],
+        level: Optional[List[Union[int, float]]],
+        finetune_steps: int,
+        clean_ex_first: bool,
+        add_history: bool,
+    ):
+        if freq is None:
+            freq = self._infer_freq(df)
+        Y_df, X_df, x_cols = self._preprocess_dataframes(
+            df=df,
+            h=h,
+            X_df=X_df,
+            freq=freq,
+        )
+        fcst_df = self._hit_multi_series_endpoint(
+            Y_df=Y_df,
+            X_df=X_df,
+            h=h,
+            freq=freq,
+            clean_ex_first=clean_ex_first,
+            finetune_steps=finetune_steps,
+            x_cols=x_cols,
+            level=level,
+        )
+        if add_history:
+            fitted_df = self._hit_multi_series_historic_endpoint(
+                Y_df=Y_df,
+                freq=freq,
+                level=level,
+            )
+            fitted_df = fitted_df.drop(columns="y")
+            fcst_df = pd.concat([fitted_df, fcst_df]).sort_values(["unique_id", "ds"])
+        return fcst_df
+
     def forecast(
         self,
         df: pd.DataFrame,
         h: int,
         freq: Optional[str] = None,
         id_col: str = "unique_id",
         time_col: str = "ds",
         target_col: str = "y",
         X_df: Optional[pd.DataFrame] = None,
         level: Optional[List[Union[int, float]]] = None,
         finetune_steps: int = 0,
         clean_ex_first: bool = True,
         validate_token: bool = False,
+        add_history: bool = False,
     ):
         """Forecast your time series using TimeGPT.
 
         Parameters
         ----------
         df : pandas.DataFrame
             The DataFrame on which the function will operate. Expected to contain at least the following columns:
@@ -252,17 +362,19 @@
             Confidence levels between 0 and 100 for prediction intervals.
         finetune_steps : int (default=0)
             Number of steps used to finetune TimeGPT in the
             new data.
         clean_ex_first : bool (default=True)
             Clean exogenous signal before making forecasts
             using TimeGPT.
-        validate_token: bool (default=False)
+        validate_token : bool (default=False)
             If True, validates token before
             sending requests.
+        add_history : bool (default=False)
+            Return fitted values of the model.
 
         Returns
         -------
         fcsts_df : pandas.DataFrame
             DataFrame with TimeGPT forecasts for point predictions and probabilistic
             predictions (if level is not None).
         """
@@ -282,14 +394,15 @@
             df=df,
             h=h,
             freq=freq,
             X_df=X_df,
             level=level,
             finetune_steps=finetune_steps,
             clean_ex_first=clean_ex_first,
+            add_history=add_history,
         )
         fcst_df = self._validate_outputs(
             fcst_df=fcst_df,
             id_col=id_col,
             time_col=time_col,
             target_col=target_col,
             drop_uid=drop_uid,
```

### Comparing `nixtlats-0.1.3/nixtlats.egg-info/PKG-INFO` & `nixtlats-0.1.4/nixtlats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nixtlats
-Version: 0.1.3
+Version: 0.1.4
 Summary: Nixtla SDK
 Home-page: https://github.com/Nixtla/nixtla
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `nixtlats-0.1.3/setup.py` & `nixtlats-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nixtlats",
-    version="0.1.3",
+    version="0.1.4",
     description="Nixtla SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nixtla/nixtla",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

