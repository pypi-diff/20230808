# Comparing `tmp/mass_analytics-1.1.4.tar.gz` & `tmp/mass_analytics-1.1.5.tar.gz`

## Comparing `mass_analytics-1.1.4.tar` & `mass_analytics-1.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/src/mass_analytics/__init__.py
--rw-r--r--   0        0        0    16924 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/src/mass_analytics/data_frame_util.py
--rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/src/mass_analytics/data_overview.py
--rw-r--r--   0        0        0     9789 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/src/mass_analytics/date.py
--rw-r--r--   0        0        0    13977 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/src/mass_analytics/plotting.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/src/mass_analytics/reader.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/LICENSE.txt
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 mass_analytics-1.1.5/src/mass_analytics/__init__.py
+-rw-r--r--   0        0        0    16924 2020-02-02 00:00:00.000000 mass_analytics-1.1.5/src/mass_analytics/data_frame_util.py
+-rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 mass_analytics-1.1.5/src/mass_analytics/data_overview.py
+-rw-r--r--   0        0        0     9789 2020-02-02 00:00:00.000000 mass_analytics-1.1.5/src/mass_analytics/date.py
+-rw-r--r--   0        0        0    13893 2020-02-02 00:00:00.000000 mass_analytics-1.1.5/src/mass_analytics/plotting.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mass_analytics-1.1.5/src/mass_analytics/reader.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mass_analytics-1.1.5/LICENSE.txt
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mass_analytics-1.1.5/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mass_analytics-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 mass_analytics-1.1.5/PKG-INFO
```

### Comparing `mass_analytics-1.1.4/src/mass_analytics/__init__.py` & `mass_analytics-1.1.5/src/mass_analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.4/src/mass_analytics/data_frame_util.py` & `mass_analytics-1.1.5/src/mass_analytics/data_frame_util.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.4/src/mass_analytics/data_overview.py` & `mass_analytics-1.1.5/src/mass_analytics/data_overview.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.4/src/mass_analytics/date.py` & `mass_analytics-1.1.5/src/mass_analytics/date.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.4/src/mass_analytics/plotting.py` & `mass_analytics-1.1.5/src/mass_analytics/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,19 +138,17 @@
         new_df = df.groupby(date_col).agg(aggregation).reset_index()
         for num in num_cols:
             fig = go.Figure(data=go.Scatter(x=list(new_df[date_col]), y=list(new_df[num]), mode='lines'))
             fig.update_layout(title_text=num + " overtime")
             fig.show()
     else:
         new_df = df.groupby([categorical_col, date_col]).agg(aggregation).reset_index(date_col)
-        print(new_df)
         for num in num_cols:
             fig = go.Figure()
             for cat in new_df.index.unique():
-                print(new_df.loc[cat][date_col], 'aaaaaaa')
                 fig.add_trace(go.Scatter(x=pd.Series(new_df.loc[cat][date_col]), y=pd.Series(new_df.loc[cat][num]), name=cat))
                 fig.update_layout(title_text=num + " overtime")
             fig.show()
 
 def plot_two_time_series(df, date_col, num_col_1, num_col_2, two_axis=False, agg=None):
     """
     Plots two time series on a single plot, allowing comparison of two numerical columns over time.
```

### Comparing `mass_analytics-1.1.4/src/mass_analytics/reader.py` & `mass_analytics-1.1.5/src/mass_analytics/reader.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.4/LICENSE.txt` & `mass_analytics-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.4/README.md` & `mass_analytics-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.4/pyproject.toml` & `mass_analytics-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6d61 7373 5f61 6e61 6c79 7469 6373   "mass_analytics
 00000070: 220d 0a76 6572 7369 6f6e 203d 2022 312e  "..version = "1.
-00000080: 312e 3422 0d0a 6175 7468 6f72 7320 3d20  1.4"..authors = 
+00000080: 312e 3522 0d0a 6175 7468 6f72 7320 3d20  1.5"..authors = 
 00000090: 5b0d 0a20 207b 206e 616d 653d 2253 656c  [..  { name="Sel
 000000a0: 696d 222c 2065 6d61 696c 3d22 616c 6f75  im", email="alou
 000000b0: 696e 6973 656c 696d 4067 6d61 696c 2e63  iniselim@gmail.c
 000000c0: 6f6d 2220 7d2c 0d0a 5d0d 0a64 6573 6372  om" },..]..descr
 000000d0: 6970 7469 6f6e 203d 2022 5374 7265 616d  iption = "Stream
 000000e0: 6c69 6e65 2064 6174 6120 7072 6570 726f  line data prepro
 000000f0: 6365 7373 696e 6720 616e 6420 656e 6861  cessing and enha
```

### Comparing `mass_analytics-1.1.4/PKG-INFO` & `mass_analytics-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mass_analytics
-Version: 1.1.4
+Version: 1.1.5
 Summary: Streamline data preprocessing and enhance analysis with our Powerful Data Preparation Package.
 Author-email: Selim <alouiniselim@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

