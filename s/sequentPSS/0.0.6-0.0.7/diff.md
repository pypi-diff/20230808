# Comparing `tmp/sequentPSS-0.0.6.tar.gz` & `tmp/sequentPSS-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequentPSS-0.0.6.tar", last modified: Fri Aug  4 21:48:17 2023, max compression
+gzip compressed data, was "sequentPSS-0.0.7.tar", last modified: Mon Aug  7 22:58:42 2023, max compression
```

## Comparing `sequentPSS-0.0.6.tar` & `sequentPSS-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 21:48:17.707091 sequentPSS-0.0.6/
--rw-rw-rw-   0        0        0      159 2023-08-03 20:55:03.000000 sequentPSS-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      274 2023-08-04 21:48:17.706095 sequentPSS-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       93 2023-08-03 03:13:22.000000 sequentPSS-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 21:48:17.654234 sequentPSS-0.0.6/sequentPSS/
--rw-rw-rw-   0        0        0       27 2023-08-03 22:30:45.000000 sequentPSS-0.0.6/sequentPSS/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 21:48:17.700112 sequentPSS-0.0.6/sequentPSS/sampleData/
--rw-rw-rw-   0        0        0     1040 2023-08-02 16:41:16.000000 sequentPSS-0.0.6/sequentPSS/sampleData/O1.txt
--rw-rw-rw-   0        0        0     1040 2023-08-02 16:43:05.000000 sequentPSS-0.0.6/sequentPSS/sampleData/O2.txt
--rw-rw-rw-   0        0        0     1040 2023-08-02 16:39:01.000000 sequentPSS-0.0.6/sequentPSS/sampleData/O3.txt
--rw-rw-rw-   0        0        0   946401 2023-08-04 21:37:05.000000 sequentPSS-0.0.6/sequentPSS/sampleData/concatenated_df.csv
--rw-rw-rw-   0        0        0    10985 2023-08-04 21:45:53.000000 sequentPSS-0.0.6/sequentPSS/sequentPSS.py
-drwxrwxrwx   0        0        0        0 2023-08-04 21:48:17.688143 sequentPSS-0.0.6/sequentPSS.egg-info/
--rw-rw-rw-   0        0        0      274 2023-08-04 21:48:16.000000 sequentPSS-0.0.6/sequentPSS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-08-04 21:48:17.000000 sequentPSS-0.0.6/sequentPSS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 21:48:16.000000 sequentPSS-0.0.6/sequentPSS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-08-04 21:48:17.000000 sequentPSS-0.0.6/sequentPSS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-04 21:48:17.000000 sequentPSS-0.0.6/sequentPSS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 21:48:17.708091 sequentPSS-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1455 2023-08-04 21:47:43.000000 sequentPSS-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 22:58:42.948593 sequentPSS-0.0.7/
+-rw-rw-rw-   0        0        0      159 2023-08-03 20:55:03.000000 sequentPSS-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      274 2023-08-07 22:58:42.947596 sequentPSS-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       93 2023-08-03 03:13:22.000000 sequentPSS-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 22:58:42.858835 sequentPSS-0.0.7/sequentPSS/
+-rw-rw-rw-   0        0        0       27 2023-08-03 22:30:45.000000 sequentPSS-0.0.7/sequentPSS/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 22:58:42.940614 sequentPSS-0.0.7/sequentPSS/sampleData/
+-rw-rw-rw-   0        0        0     1040 2023-08-02 16:41:16.000000 sequentPSS-0.0.7/sequentPSS/sampleData/O1.txt
+-rw-rw-rw-   0        0        0     1040 2023-08-02 16:43:05.000000 sequentPSS-0.0.7/sequentPSS/sampleData/O2.txt
+-rw-rw-rw-   0        0        0     1040 2023-08-02 16:39:01.000000 sequentPSS-0.0.7/sequentPSS/sampleData/O3.txt
+-rw-rw-rw-   0        0        0   946401 2023-08-04 21:37:05.000000 sequentPSS-0.0.7/sequentPSS/sampleData/concatenated_df.csv
+-rw-rw-rw-   0        0        0    16587 2023-08-07 22:57:21.000000 sequentPSS-0.0.7/sequentPSS/sequentPSS.py
+drwxrwxrwx   0        0        0        0 2023-08-07 22:58:42.896732 sequentPSS-0.0.7/sequentPSS.egg-info/
+-rw-rw-rw-   0        0        0      274 2023-08-07 22:58:41.000000 sequentPSS-0.0.7/sequentPSS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-08-07 22:58:42.000000 sequentPSS-0.0.7/sequentPSS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 22:58:41.000000 sequentPSS-0.0.7/sequentPSS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-08-07 22:58:42.000000 sequentPSS-0.0.7/sequentPSS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-07 22:58:42.000000 sequentPSS-0.0.7/sequentPSS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 22:58:42.948593 sequentPSS-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1455 2023-08-07 22:58:33.000000 sequentPSS-0.0.7/setup.py
```

### Comparing `sequentPSS-0.0.6/sequentPSS/sampleData/O1.txt` & `sequentPSS-0.0.7/sequentPSS/sampleData/O1.txt`

 * *Files identical despite different names*

### Comparing `sequentPSS-0.0.6/sequentPSS/sampleData/O2.txt` & `sequentPSS-0.0.7/sequentPSS/sampleData/O2.txt`

 * *Files identical despite different names*

### Comparing `sequentPSS-0.0.6/sequentPSS/sampleData/O3.txt` & `sequentPSS-0.0.7/sequentPSS/sampleData/O3.txt`

 * *Files identical despite different names*

### Comparing `sequentPSS-0.0.6/sequentPSS/sampleData/concatenated_df.csv` & `sequentPSS-0.0.7/sequentPSS/sampleData/concatenated_df.csv`

 * *Files identical despite different names*

### Comparing `sequentPSS-0.0.6/sequentPSS/sequentPSS.py` & `sequentPSS-0.0.7/sequentPSS/sequentPSS.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-# In[51]:
+# In[1]:
 
 
 import numpy as np
 import pandas as pd
 import random2
 import os #os의 경우 기본적으로 주어지기 때문에 setup.py에 하지 않는다.
 
 
-# In[188]:
+# In[2]:
 
 
 from SALib.analyze import sobol
 from SALib.analyze import fast
 from SALib.analyze import rbd_fast
 from SALib.analyze import delta
 
 
 # ## data
 
-# In[225]:
+# In[3]:
 
 
 # change path to relative path - only for publishing
 current_directory = os.path.dirname(os.path.abspath(__file__))
 os.chdir(current_directory)
 
 path = "./sampleData/concatenated_df.csv"
@@ -36,15 +36,15 @@
 O2 = sorted(np.loadtxt(oPath + "O2.txt"))
 O3 = sorted(np.loadtxt(oPath + "O3.txt"))
 
 
 
 # ## simulation code
 
-# In[226]:
+# In[4]:
 
 
 def simple_Simulation(x1: 'int', x2: 'int', x3: 'int', n = 10):
     '''
     to make simple simulation
     
     Parameters
@@ -104,30 +104,29 @@
 
     
     return result_df
 
 
 # ## 1) preprocessing (1) - Determine a criterions for calibration
 
-# In[228]:
+# In[19]:
 
 
 # run multiple simulations
 
-def multiple_simple_simulation(x1_list, x2_list, x3_list, M = 150, u = 0.1, k = 3):
+def multiple_simple_simulation(x1_list, x2_list, x3_list, M = 150, k = 3):
     '''
     to make simple simulation results df by multiple parameters
     
     Parameters
     ----------
     x1: parameter 1. range: 1 to 5
     x2: parameter 2. range: 1 to 5
     x3: parameter 3. range: 1 to 5
     M: MonteCarlo index (default:100, too low:low accuracy, too high:computational intensity) 
-    u = leniency index (default:0.1, too low:overfit, too high:uncertainty)
     k = the number of parameters (3)
 
     Returns
     -------
     DataFrame
         A comma-separated values (csv) file is returned as two-dimensional
         data structure with labeled axes.
@@ -155,15 +154,15 @@
         prep1_dfs.append(tem_prep1_data)
 
     result_df = pd.concat(prep1_dfs, axis=0, ignore_index=True)
 
     return result_df
 
 
-# In[229]:
+# In[20]:
 
 
 # Preprocessing (1): determining a criterion for calibration
 
 #def prep1_criterion():
 
 def prep1_criterion(O_list, multi_simul_df, u, k):
@@ -246,15 +245,15 @@
     return rmse_sel_df, multi_simul_df_temp
     
     
 
 
 # ## 2) preprocessing (2) - Sorting Y and X
 
-# In[230]:
+# In[7]:
 
 
 def sorting_Y(multi_simul_df_rmse_sel):
     '''
     Count the cases where 'rmse' is smaller than 'rmse_sel'. If the counts are higher, that 'y' is calibrated first.
     
     Parameters
@@ -296,15 +295,15 @@
     sorted_y_seq_df = result_df.sort_values(by='count', ascending=False)
 
     print('The order of Ys:', sorted_y_seq_df['y'].to_list())
     
     return result_df
 
 
-# In[231]:
+# In[8]:
 
 
 def sorting_X(problem: dict, multi_simul_df_rmse_sel, GSA = 'RBD-FAST'):
     
     '''
     
     Sobol: Sobol’ Sensitivity Analysis
@@ -355,8 +354,162 @@
 
     print('The order of Xs:', sorted_x_seq_df['Xs'].to_list())
     
     
     return si_df
 
 
+# ## 3) Parameter space searching and calibration
+
+# In[47]:
+
+
+# run multiple simulations
+
+def fix_param_simple_simulation(x1_list, x2_list, x3_list, fix_x: str, M = 100):
+    '''
+    to make multiple simulation when fix parameter is needed
+    
+    Parameters
+    ----------
+    x1_list: list of x1 parameter space.
+    x2_list: list of x2 parameter space.
+    x3_list: list of x3 parameter space.
+    fix_x: string, target parameter that you want to fix
+    M: MonteCarlo index (default:100, too low:low accuracy, too high:computational intensity) 
+    
+
+    Returns
+    -------
+    DataFrame
+        A comma-separated values (csv) file is returned as two-dimensional
+        data structure with labeled axes.
+
+    Examples
+    --------
+    >>> multi_simul_df = multiple_simple_simulation(x1_list, x2_list, x3_list, M = 150, u = 0.1, k = 3)
+    '''    
+    
+    global simple_Simulation
+    
+    # list for saving all results dfs
+    prep1_dfs = []
+    
+    if fix_x == 'x1': target_list = x1_list.copy() # 만약 x1이 fix라면 target list는 x1
+    elif fix_x == 'x2': target_list = x2_list.copy()
+    elif fix_x == 'x3': target_list = x3_list.copy()
+    
+    for fix_param in (target_list):
+        for i in range(M): #M times
+            # set parameter space
+            if fix_x == 'x1': 
+                x_1 = fix_param # if, x1 is fixed, choose one of param in x1
+                x_2 = random2.choice(x2_list)
+                x_3 = random2.choice(x3_list)
+
+            elif fix_x == 'x2':
+                x_1 = random2.choice(x1_list)
+                x_2 = fix_param
+                x_3 = random2.choice(x3_list)
+
+            elif fix_x == 'x3':
+                x_1 = random2.choice(x1_list)
+                x_2 = random2.choice(x2_list)
+                x_3 = fix_param
+
+            # run model and save
+            tem_prep1_data = simple_Simulation(x1 = x_1, x2 = x_2, x3 = x_3, n = 1)
+
+            # append temporal result to list
+            prep1_dfs.append(tem_prep1_data)
+
+    result_df = pd.concat(prep1_dfs, axis=0, ignore_index=True)
+
+    return result_df
+
+
+# In[131]:
+
+
+# y_seq_df와 x_seq_df, multi_simul_df_rmse_sel를 이용해서 만들어야 함.
+# 시뮬결과에서 x로 시작하는 컬럼. 뽑아서 각 x마다 unique한 값들을 뽑아내서 sort함.
+# 이후 y_seq_df와 x_seq_df순서대로 calibration을 시작. y수만큼 진행됌.
+
+
+
+
+
+def seqCalibration(fix_x, fix_y, rmse_sel, simul_result_df, O_list, t, df_return = False): #x_index는 x 몇인지, y_index는 y 몇인지
+    
+    '''
+    to run sequential calibration by fixing one parameter and one dependent variable. by the creterion t (tolerance index), the permitable calibrated parameter space will vary.
+    If τ is too high, the parameter space will decrease significantly at once, resulting in stricter calibration.
+    
+    Parameters
+    ----------
+    fix_x: fixed x parameter in this round
+    fix_y: fixed y parameter in this round
+    rmse_sel: rmse_sel value of y from rmse_sel df
+    simul_result_df: simulation result df that includes each x, and corresponding y
+    O_list: A list that includes all observed data of Y
+    t: tolerance index
+    df_return: return the result df (True) or not (False)
+    
+    
+    Returns
+    -------
+    DataFrame
+        A comma-separated values (csv) file is returned as two-dimensional
+        data structure with labeled axes.
+
+    list 
+        A Python list is a data structure that holds multiple elements in a sequential order.
+    
+    Examples
+    --------
+    >>> x3_list, result_df = seqCalibration(fix_x = 'x3', fix_y = 'y1', rmse_sel = 401.295316, simul_result_df = fix_x3_simul_result_df,  O_list = O_list, t = 0.1, df_return = True)
+    >>> x3_list, = seqCalibration(fix_x = 'x3', fix_y = 'y1', rmse_sel = 401.295316, simul_result_df = fix_x3_simul_result_df,  O_list = O_list, t = 0.1)
+    
+    '''
+    
+    # fix_x3_simul_result_df 여기서 rmse를 구해서 옆에 붙이고,조합 당 몇개가 몇개중에 맞는지.
+    # --- func for RMSE calculation ---
+    def rmse(actual, predicted):
+        return np.sqrt(np.mean((np.array(actual) - np.array(predicted))**2))
+
+
+    # --- add combinations of y ---
+    df = simul_result_df.copy()
+    comb_columns = [col for col in df.columns if col.startswith('x')] # if the comlumn name starts with x
+    df['comb'] = df[comb_columns].apply(lambda row: list(row), axis=1)
+
+    
+    # --- compute rmse ---
+    df[fix_y + '_rmse'] = df[fix_y].apply(lambda x: rmse(x, O_list[int(fix_y[1:]) - 1])) # pull index of y and pull Observed data
+    df['n_R'] = 1   # ALl counts of RMSE result
+    df['n_C'] = 0   # ALl counts of RMSE result but lower than RMSE_sel
+    
+    # --- return result ---
+    df.loc[df[fix_y + '_rmse'] < rmse_sel, 'n_C'] = 1 # if y1_rmse is lower than rmse_sel -> put 1 in n_C
+    
+    # Output the 'fix_x' values as a list, where the 'n_C' /'n_R' based on unique values of 'fix_x' is equal to or greater than 10%.
+    result_summary = {}
+    unique_x_values = result_df[fix_x].unique()
+    new_x_list = []
+    
+    for x_value in unique_x_values:   # when n_C / n_R is greater than t : save it to the list
+        n_R_sum = result_df.loc[result_df[fix_x] == x_value, 'n_R'].sum()
+        n_C_sum = result_df.loc[result_df[fix_x] == x_value, 'n_C'].sum()
+        if n_C_sum / n_R_sum >= t:
+            result_summary[x_value] = round(n_C_sum / n_R_sum, 3)
+            new_x_list.append(x_value)
+    
+    print('reliability of \'' + fix_x + '\' for \'' + fix_y + '\' (1 - uncertainty degree): ', result_summary)
+    
+    new_x_list = sorted(new_x_list)
+    # --- return ---
+    if df_return == True:
+        return new_x_list, df
+    
+    else:
+        return new_x_list
```

### Comparing `sequentPSS-0.0.6/setup.py` & `sequentPSS-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'sequentPSS',
-    version = '0.0.6',
+    version = '0.0.7',
     description = "algorithm for sequential parameter searching with GSA",
     url = 'https://github.com/MG-Choi/sequentPSS',
     author = 'MoongiChoi',
     author_email = 'u1316663@utah.edu',
     packages = find_packages(),
     package_data = {'sequentPSS': ['sampleData/concatenated_df.csv', 'sampleData/O1.txt', 'sampleData/O2.txt', 'sampleData/O3.txt']},
     include_package_data = True,
```

