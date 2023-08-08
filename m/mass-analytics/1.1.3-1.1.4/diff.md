# Comparing `tmp/mass_analytics-1.1.3.tar.gz` & `tmp/mass_analytics-1.1.4.tar.gz`

## Comparing `mass_analytics-1.1.3.tar` & `mass_analytics-1.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/src/mass_analytics/__init__.py
--rw-r--r--   0        0        0    16924 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/src/mass_analytics/data_frame_util.py
--rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/src/mass_analytics/data_overview.py
--rw-r--r--   0        0        0     9879 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/src/mass_analytics/date.py
--rw-r--r--   0        0        0    10769 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/src/mass_analytics/plotting.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/src/mass_analytics/reader.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/LICENSE.txt
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 mass_analytics-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/src/mass_analytics/__init__.py
+-rw-r--r--   0        0        0    16924 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/src/mass_analytics/data_frame_util.py
+-rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/src/mass_analytics/data_overview.py
+-rw-r--r--   0        0        0     9789 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/src/mass_analytics/date.py
+-rw-r--r--   0        0        0    13977 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/src/mass_analytics/plotting.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/src/mass_analytics/reader.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 mass_analytics-1.1.4/PKG-INFO
```

### Comparing `mass_analytics-1.1.3/src/mass_analytics/__init__.py` & `mass_analytics-1.1.4/src/mass_analytics/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                             describe_categories,
                             value_matching)
 from .plotting import (plot_pie_chart,
                        plot_time_series,
                        plot_two_time_series,
                        plot_categorical_count_bar,
                        plot_correlation_heatmap,
-                       plot_box_subplots)
+                       plot_boxplots)
 
 
 __all__ = ["read_data", 
            "get_date_columns", 
            "get_periodicity",
            "pivot_by_key",
            "get_mapping_table",
@@ -35,10 +35,10 @@
            "split_value_by_day",
            "plot_pie_chart",
            "get_nb_categories_overtime",
            "plot_time_series",
            "plot_two_time_series",
            "plot_categorical_count_bar",
            "plot_correlation_heatmap",
-           "plot_box_subplots"
+           "plot_boxplots"
            ]
```

### Comparing `mass_analytics-1.1.3/src/mass_analytics/data_frame_util.py` & `mass_analytics-1.1.4/src/mass_analytics/data_frame_util.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.3/src/mass_analytics/data_overview.py` & `mass_analytics-1.1.4/src/mass_analytics/data_overview.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.3/src/mass_analytics/date.py` & `mass_analytics-1.1.4/src/mass_analytics/date.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,28 +82,26 @@
         ['Start_Date', 'End_Date']
     """
          
     # Result list
     date_columns = []
     
     NUMBER_OF_ROWS = df.shape[0]
-    if NUMBER_OF_ROWS > 1000:
-        NUMBER_ROW_TO_CHECK = 1000 # Check only 1000 rows
-    else:
-        NUMBER_ROW_TO_CHECK = NUMBER_OF_ROWS # Check all rows
+
+    NUMBER_ROW_TO_CHECK = min(1000,NUMBER_OF_ROWS)
                     
     for column in df.columns:
         if np.issubdtype(df[column].dtype, np.datetime64):
             date_columns.append(column)
             continue
         elif np.issubdtype(df[column].dtype, np.object_):
             counter = 0
             counter_nan = 0
-                
-            for index in range(0, NUMBER_OF_ROWS, int(NUMBER_OF_ROWS / NUMBER_ROW_TO_CHECK)):
+            index_range = np.random.choice(list(df.index),NUMBER_ROW_TO_CHECK,replace=False)
+            for index in index_range:
                 value = df[column][index]
                 if 'datetime.datetime' in str(type(df[column][index])):
                     counter += 1
                 elif type(value) is str:
                     if is_date(value):
                         counter += 1
                     elif value == 'nan':
```

### Comparing `mass_analytics-1.1.3/src/mass_analytics/plotting.py` & `mass_analytics-1.1.4/src/mass_analytics/plotting.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,26 +45,29 @@
     fig.update_layout(title_text="Distribution of "+ num_col + " by "+categorical_col)
 
     if return_fig:
         return fig
     else:
         fig.show()
     
-def plot_time_series(df, date_col=None, categorical_col=None, num_cols=None):
+def plot_time_series(df, date_col=None, categorical_col=None, num_cols=None, agg=None):
     """
     Plot time series data from a DataFrame.
 
     Parameters:
         df (pandas.DataFrame): The input DataFrame containing time series data.
         date_col (str, optional): The name of the column in the DataFrame representing dates or timestamps.
                                   If not provided, the function will try to automatically detect a suitable date column.
         categorical_col (str, optional): The name of the column in the DataFrame representing categories or groups.
                                          If provided, the function will generate separate plots for each category.
         num_cols (list of str, optional): A list of column names in the DataFrame containing numerical data to be plotted.
                                           If not provided, all numeric columns will be used.
+        agg (dict, optional): A dictionary specifying aggregation functions to apply to numerical columns.
+                             The keys are the numerical column names, and values are aggregation functions
+                             (e.g., {'Sales': 'sum', 'Profit': 'mean'}). Default is None, which performs sum.
 
     Raises:
         ValueError: If the provided `date_col` is not found in the DataFrame, or if there is more than one potential
                     date column when `date_col` is not specified, or if any of the columns in `num_cols` are not
                     numeric columns in the DataFrame.
 
     Returns:
@@ -84,92 +87,144 @@
     # Check date_col
     if date_col is None:
         date_col = get_date_columns(df)
         if type(date_col) is not str:
             raise ValueError("There is more than one date column.", date_col)
     else:
         cols = get_date_columns(df)
+        if type(cols) is str:
+            cols = [cols]
         if date_col not in cols:
             raise ValueError(date_col," is not a date column")
+        if np.issubdtype(df[date_col].dtype, np.object_):
+            df[date_col] = pd.to_datetime(df[date_col])
+        df.sort_values(by=date_col, inplace = True)
+        
+    # Check categorical_col
+    all_cat_cols = [col for col in df.columns if is_string_dtype(df[col])]
+    if categorical_col is not None:
+        if type(categorical_col) is not str:
+            raise ValueError('categorical_col must be a string !')
+        elif categorical_col not in all_cat_cols:
+            raise ValueError('Wrong categorical_col')
         
     # Check num_cols
     all_num_cols = []
     for col in df.columns:
         if is_numeric_dtype(df[col]):
             all_num_cols.append(col)
     
     if num_cols is None:
         num_cols = all_num_cols
+    elif type(num_cols) is not list:
+        raise ValueError('num_cols must be a list')
     elif set(num_cols).issubset(set(all_num_cols)) == False:
         raise ValueError(num_cols, " aren\'t all numerical columns")
     
+    aggregation = {}
+    for num in num_cols:
+        aggregation[num] = 'sum'
+    
+    if agg is not None:
+        if type(agg) is not dict:
+            raise ValueError('agg must be a dict !')
+        elif set(agg.keys()).issubset(set(aggregation.keys())) == False:
+            raise ValueError('Wrong keys for the agg variable')
+
+        for num in num_cols:
+            if num in agg.keys():
+                aggregation[num] = agg[num]
+    
     if categorical_col is None:
-        new_df = df.groupby(date_col).sum().reset_index()
+        new_df = df.groupby(date_col).agg(aggregation).reset_index()
         for num in num_cols:
             fig = go.Figure(data=go.Scatter(x=list(new_df[date_col]), y=list(new_df[num]), mode='lines'))
             fig.update_layout(title_text=num + " overtime")
             fig.show()
     else:
-        new_df = df.groupby([categorical_col, date_col]).sum().reset_index(date_col)
-        
+        new_df = df.groupby([categorical_col, date_col]).agg(aggregation).reset_index(date_col)
+        print(new_df)
         for num in num_cols:
             fig = go.Figure()
             for cat in new_df.index.unique():
-                fig.add_trace(go.Scatter(x=list(new_df.loc[cat][date_col]), y=list(new_df.loc[cat][num]), name=cat))
+                print(new_df.loc[cat][date_col], 'aaaaaaa')
+                fig.add_trace(go.Scatter(x=pd.Series(new_df.loc[cat][date_col]), y=pd.Series(new_df.loc[cat][num]), name=cat))
                 fig.update_layout(title_text=num + " overtime")
             fig.show()
 
-def plot_two_time_series(df, date_col, num_col_1, num_col_2, two_axis=False):
+def plot_two_time_series(df, date_col, num_col_1, num_col_2, two_axis=False, agg=None):
     """
     Plots two time series on a single plot, allowing comparison of two numerical columns over time.
 
     Parameters:
     df (pandas.DataFrame): The DataFrame containing the data to be plotted.
     date_col (str): The column name in the DataFrame representing the date or time values.
     num_col_1 (str): The column name in the DataFrame representing the first numerical series to be plotted.
     num_col_2 (str): The column name in the DataFrame representing the second numerical series to be plotted.
     two_axis (bool, optional): If True, the two series will be plotted with separate y-axes. If False (default),
                                both series will share the same y-axis.
+    agg (dict, optional): A dictionary specifying aggregation functions to apply to numerical columns.
+                             The keys are the numerical column names, and values are aggregation functions
+                             (e.g., {'Sales': 'sum', 'Profit': 'mean'}). Default is None, which performs sum.
 
     Returns:
     None
 
     Example:
     plot_two_time_series(df=my_data, date_col='Date', num_col_1='Sales', num_col_2='Profit', two_axis=True)
     """
 
+    # Check date column
+    cols = get_date_columns(df)
+    if type(cols) is str:
+        cols = [cols]
+    if date_col not in cols:
+        raise ValueError(date_col+" is not a date column")
     if np.issubdtype(df[date_col].dtype, np.object_):
         df[date_col] = pd.to_datetime(df[date_col])
     df.sort_values(by=date_col, inplace = True)
-
     
+    aggregation = {'a': 'sum', 'b': 'sum'}
+    if agg is not None:
+        if type(agg) is not dict:
+            raise ValueError('agg must be a dict !')
+        elif set(agg.keys()).issubset(set(aggregation.keys())) == False:
+            raise ValueError('Wrong keys for the agg variable')
+    
+        if num_col_1 in agg.keys():
+            aggregation[num_col_1] = agg[num_col_1]
+        if num_col_2 in agg.keys():
+            aggregation[num_col_2] = agg[num_col_2]
+
+    new_df = df.groupby(date_col).agg(aggregation).reset_index()
+
     if two_axis is False:
         fig = go.Figure()
-        fig.add_trace(go.Scatter(x=df[date_col], y=df[num_col_1],
+        fig.add_trace(go.Scatter(x=new_df[date_col], y=new_df[num_col_1],
                     mode='lines',
                     name=num_col_1))
-        fig.add_trace(go.Scatter(x=df[date_col], y=df[num_col_2],
+        fig.add_trace(go.Scatter(x=new_df[date_col], y=new_df[num_col_2],
                     mode='lines',
                     name=num_col_2))
     else:
         fig = make_subplots(specs=[[{"secondary_y": True}]])
         # Add traces
         fig.add_trace(
-            go.Scatter(x=df[date_col], y=df[num_col_1], name=num_col_1),
+            go.Scatter(x=new_df[date_col], y=new_df[num_col_1], name=num_col_1),
             secondary_y=False,
         )
 
         fig.add_trace(
-            go.Scatter(x=df[date_col], y=df[num_col_2], name=num_col_2),
+            go.Scatter(x=new_df[date_col], y=new_df[num_col_2], name=num_col_2),
             secondary_y=True,
         )
 
         # Add figure title
         fig.update_layout(
-            title_text="Double Y Axis by "+num_col_1+" and "+num_col_2
+            title_text=num_col_1+" vs "+num_col_2
         )
 
         # Set x-axis title
         fig.update_xaxes(title_text=date_col)
 
         # Set y-axes titles
         fig.update_yaxes(title_text=num_col_1, secondary_y=False)
@@ -192,26 +247,35 @@
 
     fig = go.Figure([go.Bar(x=cat_counts.index, y=cat_counts.values)])
     fig.update_layout(title=f"Count of Different Categories in '{cat_col}'",
                       xaxis_title=cat_col,
                       yaxis_title="Count")
     fig.show()
 
-def plot_correlation_heatmap(df):
+def plot_correlation_heatmap(df, num_cols=None):
     """
     Create a heatmap showing the correlation between different numerical features in a dataset.
 
     Parameters:
     df (pandas.DataFrame): The DataFrame containing the data.
-
+    num_cols (list of str, optional): A list of column names in the DataFrame containing numerical data to be plotted.
+                                          If not provided, all numeric columns will be used.
     Returns:
     None
     """
 
-    num_cols = [col for col in df.columns if is_numeric_dtype(df[col])]
+    all_num_cols = [col for col in df.columns if is_numeric_dtype(df[col])]
+    
+    if num_cols is None:
+        num_cols = all_num_cols
+    elif type(num_cols) is not list:
+        raise ValueError("num_cols must be a list")
+    elif set(num_cols).issubset(set(all_num_cols)) == False:
+        raise ValueError(str(num_cols)+" aren\'t all numerical columns")
+    
     # Calculate the correlation matrix
     correlation_matrix = df[num_cols].corr()
 
     # Create the heatmap using plotly.graph_objects
     fig = go.Figure(data=go.Heatmap(z=correlation_matrix.values,
                                      x=correlation_matrix.columns,
                                      y=correlation_matrix.index,
@@ -221,15 +285,15 @@
     fig.update_layout(title="Correlation Heatmap",
                       xaxis_title="Features",
                       yaxis_title="Features")
 
     # Show the plot
     fig.show()
 
-def plot_box_subplots(df, num_cols, categorical_col=None):
+def plot_boxplots(df, num_cols, categorical_col=None):
     """
     Create subplots with box plots for different numerical variables grouped by a categorical variable.
 
     Parameters:
     df (pandas.DataFrame): The DataFrame containing the data.
     cat_col (str): The name of the categorical column used for grouping.
 
@@ -267,8 +331,7 @@
             for u_d in unique_data:
                 fig.add_trace(go.Box(y=df[df[categorical_col]==u_d][num_col], name=u_d))
                 count += 1
             fig.update_layout(title="Box Plots by "+categorical_col+" ("+num_col+")")
             fig.show()
 
     
-
```

### Comparing `mass_analytics-1.1.3/src/mass_analytics/reader.py` & `mass_analytics-1.1.4/src/mass_analytics/reader.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.3/LICENSE.txt` & `mass_analytics-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.3/README.md` & `mass_analytics-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.1.3/pyproject.toml` & `mass_analytics-1.1.4/pyproject.toml`

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
-00000080: 312e 3322 0d0a 6175 7468 6f72 7320 3d20  1.3"..authors = 
+00000080: 312e 3422 0d0a 6175 7468 6f72 7320 3d20  1.4"..authors = 
 00000090: 5b0d 0a20 207b 206e 616d 653d 2253 656c  [..  { name="Sel
 000000a0: 696d 222c 2065 6d61 696c 3d22 616c 6f75  im", email="alou
 000000b0: 696e 6973 656c 696d 4067 6d61 696c 2e63  iniselim@gmail.c
 000000c0: 6f6d 2220 7d2c 0d0a 5d0d 0a64 6573 6372  om" },..]..descr
 000000d0: 6970 7469 6f6e 203d 2022 5374 7265 616d  iption = "Stream
 000000e0: 6c69 6e65 2064 6174 6120 7072 6570 726f  line data prepro
 000000f0: 6365 7373 696e 6720 616e 6420 656e 6861  cessing and enha
```

### Comparing `mass_analytics-1.1.3/PKG-INFO` & `mass_analytics-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mass_analytics
-Version: 1.1.3
+Version: 1.1.4
 Summary: Streamline data preprocessing and enhance analysis with our Powerful Data Preparation Package.
 Author-email: Selim <alouiniselim@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

