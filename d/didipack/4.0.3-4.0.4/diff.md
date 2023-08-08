# Comparing `tmp/didipack-4.0.3.tar.gz` & `tmp/didipack-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "didipack-4.0.3.tar", last modified: Mon Aug  7 05:12:00 2023, max compression
+gzip compressed data, was "didipack-4.0.4.tar", last modified: Tue Aug  8 00:50:59 2023, max compression
```

## Comparing `didipack-4.0.3.tar` & `didipack-4.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 05:12:00.794567 didipack-4.0.3/
--rw-r--r--   0 adidishe   (503) staff       (20)     1061 2020-05-30 14:27:33.000000 didipack-4.0.3/LICENSE.txt
--rw-r--r--   0 adidishe   (503) staff       (20)      853 2023-08-07 05:12:00.794639 didipack-4.0.3/PKG-INFO
--rw-r--r--   0 adidishe   (503) staff       (20)     1055 2021-02-13 12:52:32.000000 didipack-4.0.3/README.md
-drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 05:12:00.790268 didipack-4.0.3/didipack/
--rw-r--r--   0 adidishe   (503) staff       (20)      226 2023-08-07 05:11:41.000000 didipack-4.0.3/didipack/__init__.py
-drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 05:12:00.792194 didipack-4.0.3/didipack/create_rf/
--rwxr--r--   0 adidishe   (503) staff       (20)    20378 2023-08-03 03:16:13.000000 didipack-4.0.3/didipack/create_rf/RandomFeaturesGenerator.py
--rw-r--r--   0 adidishe   (503) staff       (20)      174 2023-08-07 04:25:53.000000 didipack-4.0.3/didipack/create_rf/__init__.py
--rw-r--r--   0 adidishe   (503) staff       (20)      965 2023-08-07 05:11:41.000000 didipack-4.0.3/didipack/create_rf/aux.py
--rw-r--r--   0 adidishe   (503) staff       (20)     4937 2023-08-07 05:11:41.000000 didipack-4.0.3/didipack/create_rf/gen_rf_factors.py
--rw-r--r--   0 adidishe   (503) staff       (20)     3987 2023-08-07 05:11:41.000000 didipack-4.0.3/didipack/create_rf/pre_process_130.py
--rw-r--r--   0 adidishe   (503) staff       (20)     5707 2021-06-23 07:26:52.000000 didipack-4.0.3/didipack/latex_paper.py
--rw-r--r--   0 adidishe   (503) staff       (20)    18383 2021-02-12 21:49:54.000000 didipack-4.0.3/didipack/latex_ressource.py
--rw-r--r--   0 adidishe   (503) staff       (20)    10138 2023-08-07 04:10:35.000000 didipack-4.0.3/didipack/latex_table.py
--rw-r--r--   0 adidishe   (503) staff       (20)     5122 2023-08-07 04:46:58.000000 didipack-4.0.3/didipack/parameters.py
--rw-r--r--   0 adidishe   (503) staff       (20)      610 2021-02-13 11:17:35.000000 didipack-4.0.3/didipack/plot_function.py
-drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 05:12:00.793112 didipack-4.0.3/didipack/trainer/
--rw-r--r--   0 adidishe   (503) staff       (20)        2 2023-08-07 04:44:31.000000 didipack-4.0.3/didipack/trainer/__init__.py
--rw-r--r--   0 adidishe   (503) staff       (20)     5589 2023-08-07 05:11:41.000000 didipack-4.0.3/didipack/trainer/train_splitter.py
--rw-r--r--   0 adidishe   (503) staff       (20)     3622 2023-08-07 04:46:58.000000 didipack-4.0.3/didipack/trainer/trainer_abstract.py
--rw-r--r--   0 adidishe   (503) staff       (20)     1823 2023-08-07 05:11:41.000000 didipack-4.0.3/didipack/trainer/trainer_ridge.py
-drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 05:12:00.794319 didipack-4.0.3/didipack/utils/
--rw-r--r--   0 adidishe   (503) staff       (20)       12 2023-08-07 05:09:04.000000 didipack-4.0.3/didipack/utils/__init__.py
--rw-r--r--   0 adidishe   (503) staff       (20)     1585 2023-08-07 04:48:13.000000 didipack-4.0.3/didipack/utils/general.py
--rw-r--r--   0 adidishe   (503) staff       (20)     1230 2023-08-07 04:48:13.000000 didipack-4.0.3/didipack/utils/pandasplus.py
--rw-r--r--   0 adidishe   (503) staff       (20)      772 2023-07-21 00:00:42.000000 didipack-4.0.3/didipack/utils/plot.py
--rw-r--r--   0 adidishe   (503) staff       (20)     3703 2023-08-07 05:09:04.000000 didipack-4.0.3/didipack/utils/ridge.py
--rw-r--r--   0 adidishe   (503) staff       (20)      837 2023-01-31 16:53:40.000000 didipack-4.0.3/didipack/utils/smart_algebra.py
-drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 05:12:00.791124 didipack-4.0.3/didipack.egg-info/
--rw-r--r--   0 adidishe   (503) staff       (20)      853 2023-08-07 05:12:00.000000 didipack-4.0.3/didipack.egg-info/PKG-INFO
--rw-r--r--   0 adidishe   (503) staff       (20)      819 2023-08-07 05:12:00.000000 didipack-4.0.3/didipack.egg-info/SOURCES.txt
--rw-r--r--   0 adidishe   (503) staff       (20)        1 2023-08-07 05:12:00.000000 didipack-4.0.3/didipack.egg-info/dependency_links.txt
--rw-r--r--   0 adidishe   (503) staff       (20)       48 2023-08-07 05:12:00.000000 didipack-4.0.3/didipack.egg-info/requires.txt
--rw-r--r--   0 adidishe   (503) staff       (20)        9 2023-08-07 05:12:00.000000 didipack-4.0.3/didipack.egg-info/top_level.txt
--rw-r--r--   0 adidishe   (503) staff       (20)       79 2023-08-07 05:12:00.794872 didipack-4.0.3/setup.cfg
--rw-r--r--   0 adidishe   (503) staff       (20)     1325 2023-08-07 05:11:41.000000 didipack-4.0.3/setup.py
+drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-08 00:50:59.505247 didipack-4.0.4/
+-rw-r--r--   0 adidishe   (503) staff       (20)     1061 2020-05-30 14:27:33.000000 didipack-4.0.4/LICENSE.txt
+-rw-r--r--   0 adidishe   (503) staff       (20)      853 2023-08-08 00:50:59.505344 didipack-4.0.4/PKG-INFO
+-rw-r--r--   0 adidishe   (503) staff       (20)     1055 2021-02-13 12:52:32.000000 didipack-4.0.4/README.md
+drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-08 00:50:59.500595 didipack-4.0.4/didipack/
+-rw-r--r--   0 adidishe   (503) staff       (20)      294 2023-08-07 23:55:42.000000 didipack-4.0.4/didipack/__init__.py
+drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-08 00:50:59.502773 didipack-4.0.4/didipack/create_rf/
+-rwxr--r--   0 adidishe   (503) staff       (20)    20378 2023-08-03 03:16:13.000000 didipack-4.0.4/didipack/create_rf/RandomFeaturesGenerator.py
+-rw-r--r--   0 adidishe   (503) staff       (20)      174 2023-08-07 04:25:53.000000 didipack-4.0.4/didipack/create_rf/__init__.py
+-rw-r--r--   0 adidishe   (503) staff       (20)      965 2023-08-07 05:11:41.000000 didipack-4.0.4/didipack/create_rf/aux.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     4937 2023-08-07 05:11:41.000000 didipack-4.0.4/didipack/create_rf/gen_rf_factors.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     3987 2023-08-07 05:11:41.000000 didipack-4.0.4/didipack/create_rf/pre_process_130.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     5707 2021-06-23 07:26:52.000000 didipack-4.0.4/didipack/latex_paper.py
+-rw-r--r--   0 adidishe   (503) staff       (20)    18383 2021-02-12 21:49:54.000000 didipack-4.0.4/didipack/latex_ressource.py
+-rw-r--r--   0 adidishe   (503) staff       (20)    10138 2023-08-07 04:10:35.000000 didipack-4.0.4/didipack/latex_table.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     5122 2023-08-07 04:46:58.000000 didipack-4.0.4/didipack/parameters.py
+-rw-r--r--   0 adidishe   (503) staff       (20)      610 2021-02-13 11:17:35.000000 didipack-4.0.4/didipack/plot_function.py
+drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-08 00:50:59.503839 didipack-4.0.4/didipack/trainer/
+-rw-r--r--   0 adidishe   (503) staff       (20)        2 2023-08-07 04:44:31.000000 didipack-4.0.4/didipack/trainer/__init__.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     5589 2023-08-07 05:11:41.000000 didipack-4.0.4/didipack/trainer/train_splitter.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     3622 2023-08-07 04:46:58.000000 didipack-4.0.4/didipack/trainer/trainer_abstract.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     1823 2023-08-07 05:11:41.000000 didipack-4.0.4/didipack/trainer/trainer_ridge.py
+drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-08 00:50:59.504992 didipack-4.0.4/didipack/utils/
+-rw-r--r--   0 adidishe   (503) staff       (20)        0 2023-08-07 23:54:59.000000 didipack-4.0.4/didipack/utils/__init__.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     1812 2023-08-07 23:54:59.000000 didipack-4.0.4/didipack/utils/general.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     1230 2023-08-07 04:48:13.000000 didipack-4.0.4/didipack/utils/pandasplus.py
+-rw-r--r--   0 adidishe   (503) staff       (20)      886 2023-08-07 23:54:59.000000 didipack-4.0.4/didipack/utils/plot.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     3703 2023-08-07 05:09:04.000000 didipack-4.0.4/didipack/utils/ridge.py
+-rw-r--r--   0 adidishe   (503) staff       (20)      837 2023-01-31 16:53:40.000000 didipack-4.0.4/didipack/utils/smart_algebra.py
+drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-08 00:50:59.501374 didipack-4.0.4/didipack.egg-info/
+-rw-r--r--   0 adidishe   (503) staff       (20)      853 2023-08-08 00:50:59.000000 didipack-4.0.4/didipack.egg-info/PKG-INFO
+-rw-r--r--   0 adidishe   (503) staff       (20)      819 2023-08-08 00:50:59.000000 didipack-4.0.4/didipack.egg-info/SOURCES.txt
+-rw-r--r--   0 adidishe   (503) staff       (20)        1 2023-08-08 00:50:59.000000 didipack-4.0.4/didipack.egg-info/dependency_links.txt
+-rw-r--r--   0 adidishe   (503) staff       (20)       48 2023-08-08 00:50:59.000000 didipack-4.0.4/didipack.egg-info/requires.txt
+-rw-r--r--   0 adidishe   (503) staff       (20)        9 2023-08-08 00:50:59.000000 didipack-4.0.4/didipack.egg-info/top_level.txt
+-rw-r--r--   0 adidishe   (503) staff       (20)       79 2023-08-08 00:50:59.505648 didipack-4.0.4/setup.cfg
+-rw-r--r--   0 adidishe   (503) staff       (20)     1308 2023-08-08 00:50:45.000000 didipack-4.0.4/setup.py
```

### Comparing `didipack-4.0.3/LICENSE.txt` & `didipack-4.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/PKG-INFO` & `didipack-4.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: didipack
-Version: 4.0.3
+Version: 4.0.4
 Summary: Usefull time saver for data-science and finance with python
 Home-page: https://github.com/AntoineDidisheim
 Author: Antoine Didisheim
 Author-email: antoinedidisheim@gmail.com
 License: MIT
 Download-URL: https://github.com/AntoineDidisheim/didipack/archive/v0.1.1.tar.gz
 Keywords: LaTex,Finance
```

### Comparing `didipack-4.0.3/README.md` & `didipack-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/didipack/create_rf/RandomFeaturesGenerator.py` & `didipack-4.0.4/didipack/create_rf/RandomFeaturesGenerator.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/didipack/create_rf/aux.py` & `didipack-4.0.4/didipack/create_rf/aux.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/didipack/create_rf/gen_rf_factors.py` & `didipack-4.0.4/didipack/create_rf/gen_rf_factors.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/didipack/create_rf/pre_process_130.py` & `didipack-4.0.4/didipack/create_rf/pre_process_130.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/didipack/latex_paper.py` & `didipack-4.0.4/didipack/latex_paper.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/didipack/latex_ressource.py` & `didipack-4.0.4/didipack/latex_ressource.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/didipack/latex_table.py` & `didipack-4.0.4/didipack/latex_table.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/didipack/parameters.py` & `didipack-4.0.4/didipack/parameters.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/didipack/plot_function.py` & `didipack-4.0.4/didipack/plot_function.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/didipack/trainer/train_splitter.py` & `didipack-4.0.4/didipack/trainer/train_splitter.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/didipack/trainer/trainer_abstract.py` & `didipack-4.0.4/didipack/trainer/trainer_abstract.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/didipack/trainer/trainer_ridge.py` & `didipack-4.0.4/didipack/trainer/trainer_ridge.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/didipack/utils/general.py` & `didipack-4.0.4/didipack/utils/general.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 import numpy as np
 import pandas as pd
 import tqdm
 
-def split_array_fix_size(input_array, fix_size):
-    return [input_array[i:i + fix_size] for i in range(0, len(input_array), fix_size)]
+class General:
+    @staticmethod
+    def split_array_fix_size(input_array, fix_size):
+        return [input_array[i:i + fix_size] for i in range(0, len(input_array), fix_size)]
+
+    @staticmethod
+    def smart_chunks(lst, n):
+        """Choose chunking method based on deviation from the desired chunk size."""
+        chunk_count = len(lst) // n
+        remainder = len(lst) % n
+
+        # Calculate the size of the last chunk with the leftover method
+        leftover_last_chunk_size = remainder if remainder != 0 else n
+
+        # Calculate the size of the last chunk with the equally spread method
+        spread_last_chunk_size = n + 1 if remainder > chunk_count else n
+
+        # If the size of the last chunk with the leftover method is closer to n, use chunks_chunks_if_leftover_list
+        if abs(n - leftover_last_chunk_size) <= abs(n - spread_last_chunk_size):
+            return General.chunks_chunks_if_leftover_list(lst, n)
+
+        # Otherwise, use chunks_equally_spread
+        else:
+            return General.chunks_equally_spread(lst, n)
+
+    @staticmethod
+    def chunks_chunks_if_leftover_list(lst, n):
+        """Yield successive n-sized chunks from lst."""
+        for i in range(0, len(lst), n):
+            yield lst[i:i + n]
+
+    @staticmethod
+    def chunks_equally_spread(lst, n):
+        """Yield successive n-sized chunks from lst, spreading remainder equally."""
+        chunk_count = len(lst) // n
+        remainder = len(lst) % n
+        iterator = iter(lst)
+
+        full_chunks = []
+        for _ in range(chunk_count):
+            full_chunks.append([next(iterator) for _ in range(n)])
 
-def smart_chunks(lst, n):
-    """Choose chunking method based on deviation from the desired chunk size."""
-    chunk_count = len(lst) // n
-    remainder = len(lst) % n
-
-    # Calculate the size of the last chunk with the leftover method
-    leftover_last_chunk_size = remainder if remainder != 0 else n
-
-    # Calculate the size of the last chunk with the equally spread method
-    spread_last_chunk_size = n + 1 if remainder > chunk_count else n
-
-    # If the size of the last chunk with the leftover method is closer to n, use chunks_chunks_if_leftover_list
-    if abs(n - leftover_last_chunk_size) <= abs(n - spread_last_chunk_size):
-        return chunks_chunks_if_leftover_list(lst, n)
-
-    # Otherwise, use chunks_equally_spread
-    else:
-        return chunks_equally_spread(lst, n)
-
-def chunks_chunks_if_leftover_list(lst, n):
-    """Yield successive n-sized chunks from lst."""
-    for i in range(0, len(lst), n):
-        yield lst[i:i + n]
-
-def chunks_equally_spread(lst, n):
-    """Yield successive n-sized chunks from lst, spreading remainder equally."""
-    chunk_count = len(lst) // n
-    remainder = len(lst) % n
-    iterator = iter(lst)
-
-    full_chunks = []
-    for _ in range(chunk_count):
-        full_chunks.append([next(iterator) for _ in range(n)])
+        for i in range(remainder):
+            full_chunks[i % len(full_chunks)].append(next(iterator))
 
-    for i in range(remainder):
-        full_chunks[i % len(full_chunks)].append(next(iterator))
-
-    return full_chunks
+        return full_chunks
```

### Comparing `didipack-4.0.3/didipack/utils/pandasplus.py` & `didipack-4.0.4/didipack/utils/pandasplus.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/didipack/utils/plot.py` & `didipack-4.0.4/didipack/utils/plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import matplotlib.pyplot as plt
 
-def plot_dual_axis(df, col1, col2, label1=None, label2=None, xlabel = 'Date'):
-    fig, ax1 = plt.subplots()
+class PlotPlus:
+    @staticmethod
+    def plot_dual_axis(df, col1, col2, label1=None, label2=None, xlabel = 'Date'):
+        fig, ax1 = plt.subplots()
+
+        # Use column names as labels if no labels are provided
+        if label1 is None:
+            label1 = col1
+        if label2 is None:
+            label2 = col2
+
+        # Plotting col1 on the first y-axis
+        color = 'tab:blue'
+        ax1.set_xlabel(xlabel=xlabel)
+        ax1.set_ylabel(label1, color=color)
+        ax1.plot(df.index, df[col1], color=color)
+        ax1.tick_params(axis='y', labelcolor=color)
+
+        # Creating a second y-axis to plot col2
+        ax2 = ax1.twinx()
+
+        color = 'tab:red'
+        ax2.set_ylabel(label2, color=color)
+        ax2.plot(df.index, df[col2], color=color)
+        ax2.tick_params(axis='y', labelcolor=color)
 
-    # Use column names as labels if no labels are provided
-    if label1 is None:
-        label1 = col1
-    if label2 is None:
-        label2 = col2
-
-    # Plotting col1 on the first y-axis
-    color = 'tab:blue'
-    ax1.set_xlabel(xlabel=xlabel)
-    ax1.set_ylabel(label1, color=color)
-    ax1.plot(df.index, df[col1], color=color)
-    ax1.tick_params(axis='y', labelcolor=color)
-
-    # Creating a second y-axis to plot col2
-    ax2 = ax1.twinx()
-
-    color = 'tab:red'
-    ax2.set_ylabel(label2, color=color)
-    ax2.plot(df.index, df[col2], color=color)
-    ax2.tick_params(axis='y', labelcolor=color)
-
-    fig.tight_layout()
+        fig.tight_layout()
```

### Comparing `didipack-4.0.3/didipack/utils/ridge.py` & `didipack-4.0.4/didipack/utils/ridge.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/didipack/utils/smart_algebra.py` & `didipack-4.0.4/didipack/utils/smart_algebra.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/didipack.egg-info/PKG-INFO` & `didipack-4.0.4/didipack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: didipack
-Version: 4.0.3
+Version: 4.0.4
 Summary: Usefull time saver for data-science and finance with python
 Home-page: https://github.com/AntoineDidisheim
 Author: Antoine Didisheim
 Author-email: antoinedidisheim@gmail.com
 License: MIT
 Download-URL: https://github.com/AntoineDidisheim/didipack/archive/v0.1.1.tar.gz
 Keywords: LaTex,Finance
```

### Comparing `didipack-4.0.3/didipack.egg-info/SOURCES.txt` & `didipack-4.0.4/didipack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `didipack-4.0.3/setup.py` & `didipack-4.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='didipack',
     packages=setuptools.find_packages(),  # Automatically discover and include all packages in the package directory
-    version='4.0.3',
+    version='4.0.4',
     license='MIT',
     setup_requires=['wheel'],
     description='Usefull time saver for data-science and finance with python',
     author='Antoine Didisheim',
     author_email='antoinedidisheim@gmail.com',
     url='https://github.com/AntoineDidisheim',
     download_url='https://github.com/AntoineDidisheim/didipack/archive/v0.1.1.tar.gz',
@@ -33,11 +33,7 @@
     ],
     # If you have package data
     # package_data={
     #     'didipack': ['data/*.csv'],  # example, adjust as needed
     # },
 )
 
-
-'''
-T_train 
-'''
```

