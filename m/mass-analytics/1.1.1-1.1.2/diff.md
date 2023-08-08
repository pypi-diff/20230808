# Comparing `tmp/mass_analytics-1.1.1.tar.gz` & `tmp/mass_analytics-1.1.2.tar.gz`

## Comparing `mass_analytics-1.1.1.tar` & `mass_analytics-1.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 mass_analytics-1.1.1/src/mass_analytics/__init__.py
--rw-r--r--   0        0        0    16135 2020-02-02 00:00:00.000000 mass_analytics-1.1.1/src/mass_analytics/data_frame_util.py
--rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 mass_analytics-1.1.1/src/mass_analytics/data_overview.py
--rw-r--r--   0        0        0     9881 2020-02-02 00:00:00.000000 mass_analytics-1.1.1/src/mass_analytics/date.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 mass_analytics-1.1.1/src/mass_analytics/plotting.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mass_analytics-1.1.1/src/mass_analytics/reader.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mass_analytics-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mass_analytics-1.1.1/README.md
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 mass_analytics-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 mass_analytics-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/src/mass_analytics/__init__.py
+-rw-r--r--   0        0        0    16924 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/src/mass_analytics/data_frame_util.py
+-rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/src/mass_analytics/data_overview.py
+-rw-r--r--   0        0        0     9879 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/src/mass_analytics/date.py
+-rw-r--r--   0        0        0    10808 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/src/mass_analytics/plotting.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/src/mass_analytics/reader.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/PKG-INFO
```

### Comparing `mass_analytics-1.1.1/src/mass_analytics/data_frame_util.py` & `mass_analytics-1.1.2/src/mass_analytics/data_frame_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pandas as pd
 import numpy as np
 import datetime
+import tqdm
 from pandas.api.types import is_string_dtype
 from .date import (get_date_columns,
                   is_date,
                   get_periodicity)
 
 
 def pivot_by_key(df, index_column_names, key_column_names, values_column_names, agg_funcs='sum'):
@@ -277,15 +278,15 @@
         new_df = pd.DataFrame(new_rows).groupby([Region, 'Date'])
     
     if additive:
         return new_df.sum().reset_index()
     else:
         return new_df.mean().reset_index()
 
-def get_nb_categories_overtime(df, date_col, categorical_col):
+def get_nb_categories_overtime(df, date_col, categorical_col, division_col=None):
     """
     Calculate the number of unique categories over time.
 
     This function calculates the number of unique categories in the specified categorical column
     for each time point in the specified date column. It is useful for visualizing how the number
     of categories changes over time.
 
@@ -322,44 +323,58 @@
 
     if date_col not in date_columns:
         raise ValueError(date_col+" is not a date column")
     
     # Check categorical_col
     cat_columns = []
     for col in df.columns:
-        if is_string_dtype(df[col]):
+        if is_string_dtype(df[col].dropna()):
             cat_columns.append(col)
     if categorical_col not in cat_columns:
         raise ValueError(categorical_col+" is not a categorical column")
     
+    # Check division_col
+    if division_col is not None:
+        if division_col not in cat_columns:
+            raise ValueError(division_col+" is not a categorical column")
+    
     if np.issubdtype(df[date_col].dtype, np.object_):
         df[date_col] = pd.to_datetime(df[date_col])
         dates = df[date_col]
     else:
         dates = df[date_col]
     
     periodicity = get_periodicity(df, date_col)[date_col] 
     min_date = min(dates)
     max_date = max(dates)
     
+
     new_dates = pd.date_range(start=min_date, end=max_date, freq=periodicity)
-    new_df = {date_col: new_dates,
-                "nb_"+categorical_col: []}
-    
-    all_cat = []
-    counter = 0
-    df.set_index(date_col, inplace=True)
-    for date in new_df[date_col]:
-        if date in df.index:
-            if df.loc[date][categorical_col] not in all_cat:
-                all_cat.append(df.loc[date][categorical_col])
-                counter += 1
+
+    if division_col is None:
+        new_df = {date_col: new_dates,
+                    "nb_"+categorical_col: []}
+        
+        all_cat = [np.nan]
+        counter = 0
+        df.set_index(date_col, inplace=True)
+        for date in tqdm.tqdm(new_df[date_col]):
+            if date in df.index:
+                group_cols = df.loc[date][categorical_col]
+                if group_cols is str:
+                    group_cols = [group_cols]
+                for val in set(group_cols):
+                    if val not in all_cat: 
+                        all_cat.append(val)
+                        counter += 1
                 new_df["nb_"+categorical_col].append(counter)
             else:
                 new_df["nb_"+categorical_col].append(counter)
-        else:
-            new_df["nb_"+categorical_col].append(counter)
-
-    return pd.DataFrame(new_df)
-    
-    
-
+        return pd.DataFrame(new_df)
+    else:
+        new_df = pd.DataFrame()
+        new_df[date_col] = new_dates
+        div_uq_vals =  df[division_col].dropna().unique()
+        for date in tqdm.tqdm(new_dates):
+            for d_u in div_uq_vals:
+                new_df.loc[new_df[date_col]==date, categorical_col+"_"+d_u] = df.loc[(df[date_col]<=date)&(df[division_col]==d_u), categorical_col].nunique()
+        return new_df
```

### Comparing `mass_analytics-1.1.1/src/mass_analytics/data_overview.py` & `mass_analytics-1.1.2/src/mass_analytics/data_overview.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.1/src/mass_analytics/date.py` & `mass_analytics-1.1.2/src/mass_analytics/date.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,16 +115,15 @@
 
     if len(date_columns) == 0:
         raise ValueError("No date columns found in the DataFrame.")
     if len(date_columns) == 1:
         return date_columns[0]
     else:
         return date_columns
-    
-    
+        
 def get_periodicity(df, *columns):
     """
     Description
         Determine the periodicity of the given DataFrame or specified columns.
 
         The function analyzes the DataFrame or specified columns and attempts to identify
         the data's periodicity, such as daily ('D'), weekly on Monday ('W-MON') or Saturday ('W-SAT'),
```

### Comparing `mass_analytics-1.1.1/src/mass_analytics/reader.py` & `mass_analytics-1.1.2/src/mass_analytics/reader.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.1/LICENSE.txt` & `mass_analytics-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.1/README.md` & `mass_analytics-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.1/pyproject.toml` & `mass_analytics-1.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,47 +2,46 @@
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6d61 7373 5f61 6e61 6c79 7469 6373   "mass_analytics
 00000070: 220d 0a76 6572 7369 6f6e 203d 2022 312e  "..version = "1.
-00000080: 312e 3122 0d0a 6175 7468 6f72 7320 3d20  1.1"..authors = 
+00000080: 312e 3222 0d0a 6175 7468 6f72 7320 3d20  1.2"..authors = 
 00000090: 5b0d 0a20 207b 206e 616d 653d 2253 656c  [..  { name="Sel
-000000a0: 696d 222c 2065 6d61 696c 3d22 7365 6c69  im", email="seli
-000000b0: 6d2e 616c 6f75 696e 6940 6d61 7373 2d61  m.alouini@mass-a
-000000c0: 6e61 6c79 7469 6373 2e63 6f6d 2220 7d2c  nalytics.com" },
-000000d0: 0d0a 5d0d 0a64 6573 6372 6970 7469 6f6e  ..]..description
-000000e0: 203d 2022 5374 7265 616d 6c69 6e65 2064   = "Streamline d
-000000f0: 6174 6120 7072 6570 726f 6365 7373 696e  ata preprocessin
-00000100: 6720 616e 6420 656e 6861 6e63 6520 616e  g and enhance an
-00000110: 616c 7973 6973 2077 6974 6820 6f75 7220  alysis with our 
-00000120: 506f 7765 7266 756c 2044 6174 6120 5072  Powerful Data Pr
-00000130: 6570 6172 6174 696f 6e20 5061 636b 6167  eparation Packag
-00000140: 652e 220d 0a72 6561 646d 6520 3d20 2252  e."..readme = "R
-00000150: 4541 444d 452e 6d64 220d 0a72 6571 7569  EADME.md"..requi
-00000160: 7265 732d 7079 7468 6f6e 203d 2022 3e3d  res-python = ">=
-00000170: 332e 3722 0d0a 636c 6173 7369 6669 6572  3.7"..classifier
-00000180: 7320 3d20 5b0d 0a20 2020 2022 5072 6f67  s = [..    "Prog
-00000190: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000001a0: 203a 3a20 5079 7468 6f6e 203a 3a20 3322   :: Python :: 3"
-000001b0: 2c0d 0a20 2020 2022 4c69 6365 6e73 6520  ,..    "License 
-000001c0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-000001d0: 3a3a 204d 4954 204c 6963 656e 7365 222c  :: MIT License",
-000001e0: 0d0a 2020 2020 224f 7065 7261 7469 6e67  ..    "Operating
-000001f0: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
-00000200: 6465 7065 6e64 656e 7422 2c0d 0a5d 0d0a  dependent",..]..
-00000210: 6465 7065 6e64 656e 6369 6573 203d 205b  dependencies = [
-00000220: 0d0a 2020 2020 2020 2020 226e 756d 7079  ..        "numpy
-00000230: 3d3d 312e 3235 2e31 222c 0d0a 2020 2020  ==1.25.1",..    
-00000240: 2020 2020 2270 616e 6461 733d 3d32 2e30      "pandas==2.0
-00000250: 2e33 222c 0d0a 2020 2020 2020 2020 2270  .3",..        "p
-00000260: 6c6f 746c 793d 3d35 2e31 352e 3022 2c0d  lotly==5.15.0",.
-00000270: 0a20 2020 2020 2020 2022 7374 7265 616d  .        "stream
-00000280: 6c69 743d 3d31 2e32 342e 3122 2c0d 0a20  lit==1.24.1",.. 
-00000290: 2020 2020 2020 2022 6f70 656e 7079 786c         "openpyxl
-000002a0: 222c 0d0a 2020 2020 2020 2020 2274 7164  ",..        "tqd
-000002b0: 6d22 2c0d 0a20 2020 2020 2020 2022 6675  m",..        "fu
-000002c0: 7a7a 7977 757a 7a79 222c 0d0a 2020 2020  zzywuzzy",..    
-000002d0: 2020 2020 2270 7974 686f 6e2d 4c65 7665      "python-Leve
-000002e0: 6e73 6874 6569 6e22 0d0a 2020 2020 5d0d  nshtein"..    ].
-000002f0: 0a                                       .
+000000a0: 696d 222c 2065 6d61 696c 3d22 616c 6f75  im", email="alou
+000000b0: 696e 6973 656c 696d 4067 6d61 696c 2e63  iniselim@gmail.c
+000000c0: 6f6d 2220 7d2c 0d0a 5d0d 0a64 6573 6372  om" },..]..descr
+000000d0: 6970 7469 6f6e 203d 2022 5374 7265 616d  iption = "Stream
+000000e0: 6c69 6e65 2064 6174 6120 7072 6570 726f  line data prepro
+000000f0: 6365 7373 696e 6720 616e 6420 656e 6861  cessing and enha
+00000100: 6e63 6520 616e 616c 7973 6973 2077 6974  nce analysis wit
+00000110: 6820 6f75 7220 506f 7765 7266 756c 2044  h our Powerful D
+00000120: 6174 6120 5072 6570 6172 6174 696f 6e20  ata Preparation 
+00000130: 5061 636b 6167 652e 220d 0a72 6561 646d  Package."..readm
+00000140: 6520 3d20 2252 4541 444d 452e 6d64 220d  e = "README.md".
+00000150: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
+00000160: 203d 2022 3e3d 332e 3722 0d0a 636c 6173   = ">=3.7"..clas
+00000170: 7369 6669 6572 7320 3d20 5b0d 0a20 2020  sifiers = [..   
+00000180: 2022 5072 6f67 7261 6d6d 696e 6720 4c61   "Programming La
+00000190: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001a0: 203a 3a20 3322 2c0d 0a20 2020 2022 4c69   :: 3",..    "Li
+000001b0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+000001c0: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+000001d0: 656e 7365 222c 0d0a 2020 2020 224f 7065  ense",..    "Ope
+000001e0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+000001f0: 204f 5320 496e 6465 7065 6e64 656e 7422   OS Independent"
+00000200: 2c0d 0a5d 0d0a 6465 7065 6e64 656e 6369  ,..]..dependenci
+00000210: 6573 203d 205b 0d0a 2020 2020 2020 2020  es = [..        
+00000220: 226e 756d 7079 3d3d 312e 3235 2e31 222c  "numpy==1.25.1",
+00000230: 0d0a 2020 2020 2020 2020 2270 616e 6461  ..        "panda
+00000240: 733d 3d32 2e30 2e33 222c 0d0a 2020 2020  s==2.0.3",..    
+00000250: 2020 2020 2270 6c6f 746c 793d 3d35 2e31      "plotly==5.1
+00000260: 352e 3022 2c0d 0a20 2020 2020 2020 2022  5.0",..        "
+00000270: 7374 7265 616d 6c69 743d 3d31 2e32 342e  streamlit==1.24.
+00000280: 3122 2c0d 0a20 2020 2020 2020 2022 6f70  1",..        "op
+00000290: 656e 7079 786c 222c 0d0a 2020 2020 2020  enpyxl",..      
+000002a0: 2020 2274 7164 6d22 2c0d 0a20 2020 2020    "tqdm",..     
+000002b0: 2020 2022 6675 7a7a 7977 757a 7a79 222c     "fuzzywuzzy",
+000002c0: 0d0a 2020 2020 2020 2020 2270 7974 686f  ..        "pytho
+000002d0: 6e2d 4c65 7665 6e73 6874 6569 6e22 0d0a  n-Levenshtein"..
+000002e0: 2020 2020 5d0d 0a                            ]..
```

### Comparing `mass_analytics-1.1.1/PKG-INFO` & `mass_analytics-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mass_analytics
-Version: 1.1.1
+Version: 1.1.2
 Summary: Streamline data preprocessing and enhance analysis with our Powerful Data Preparation Package.
-Author-email: Selim <selim.alouini@mass-analytics.com>
+Author-email: Selim <alouiniselim@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: fuzzywuzzy
 Requires-Dist: numpy==1.25.1
```

