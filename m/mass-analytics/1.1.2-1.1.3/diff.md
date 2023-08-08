# Comparing `tmp/mass_analytics-1.1.2.tar.gz` & `tmp/mass_analytics-1.1.3.tar.gz`

## Comparing `mass_analytics-1.1.2.tar` & `mass_analytics-1.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/src/mass_analytics/__init__.py
--rw-r--r--   0        0        0    16924 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/src/mass_analytics/data_frame_util.py
--rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/src/mass_analytics/data_overview.py
--rw-r--r--   0        0        0     9879 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/src/mass_analytics/date.py
--rw-r--r--   0        0        0    10808 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/src/mass_analytics/plotting.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/src/mass_analytics/reader.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 mass_analytics-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/src/mass_analytics/__init__.py
+-rw-r--r--   0        0        0    16924 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/src/mass_analytics/data_frame_util.py
+-rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/src/mass_analytics/data_overview.py
+-rw-r--r--   0        0        0     9879 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/src/mass_analytics/date.py
+-rw-r--r--   0        0        0    10769 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/src/mass_analytics/plotting.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/src/mass_analytics/reader.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/PKG-INFO
```

### Comparing `mass_analytics-1.1.2/src/mass_analytics/__init__.py` & `mass_analytics-1.1.3/src/mass_analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.2/src/mass_analytics/data_frame_util.py` & `mass_analytics-1.1.3/src/mass_analytics/data_frame_util.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.2/src/mass_analytics/data_overview.py` & `mass_analytics-1.1.3/src/mass_analytics/data_overview.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.2/src/mass_analytics/date.py` & `mass_analytics-1.1.3/src/mass_analytics/date.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.2/src/mass_analytics/plotting.py` & `mass_analytics-1.1.3/src/mass_analytics/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import pandas as pd
 import numpy as np
 from pandas.api.types import is_numeric_dtype
 from pandas.api.types import is_string_dtype
 from .date import get_date_columns
 
 
-
 def plot_pie_chart(df, categorical_col, num_col, return_fig=False):
     """
     Plot a pie chart based on the provided DataFrame.
 
     Parameters:
         df (pandas.DataFrame): The DataFrame containing the data.
         categorical_col (str): The name of the column in the DataFrame that represents the categorical variable.
@@ -260,16 +259,16 @@
             fig.add_trace(go.Box(y=df[num_col]))
             fig.update_layout(xaxis_title=num_col)
             fig.show()
     else:
         unique_data = df[categorical_col].dropna().unique()
         for num_col in num_cols:
             count = 1
-            fig = make_subplots(rows=1, cols=len(unique_data))
+            fig = go.Figure()
             for u_d in unique_data:
                 fig.add_trace(go.Box(y=df[df[categorical_col]==u_d][num_col], name=u_d))
                 count += 1
-                fig.update_layout(title="Box Plots by "+categorical_col+" ("+num_col+")")
+            fig.update_layout(title="Box Plots by "+categorical_col+" ("+num_col+")")
             fig.show()
```

### Comparing `mass_analytics-1.1.2/src/mass_analytics/reader.py` & `mass_analytics-1.1.3/src/mass_analytics/reader.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.2/LICENSE.txt` & `mass_analytics-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.2/README.md` & `mass_analytics-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.2/pyproject.toml` & `mass_analytics-1.1.3/pyproject.toml`

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
-00000080: 312e 3222 0d0a 6175 7468 6f72 7320 3d20  1.2"..authors = 
+00000080: 312e 3322 0d0a 6175 7468 6f72 7320 3d20  1.3"..authors = 
 00000090: 5b0d 0a20 207b 206e 616d 653d 2253 656c  [..  { name="Sel
 000000a0: 696d 222c 2065 6d61 696c 3d22 616c 6f75  im", email="alou
 000000b0: 696e 6973 656c 696d 4067 6d61 696c 2e63  iniselim@gmail.c
 000000c0: 6f6d 2220 7d2c 0d0a 5d0d 0a64 6573 6372  om" },..]..descr
 000000d0: 6970 7469 6f6e 203d 2022 5374 7265 616d  iption = "Stream
 000000e0: 6c69 6e65 2064 6174 6120 7072 6570 726f  line data prepro
 000000f0: 6365 7373 696e 6720 616e 6420 656e 6861  cessing and enha
```

### Comparing `mass_analytics-1.1.2/PKG-INFO` & `mass_analytics-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mass_analytics
-Version: 1.1.2
+Version: 1.1.3
 Summary: Streamline data preprocessing and enhance analysis with our Powerful Data Preparation Package.
 Author-email: Selim <alouiniselim@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

