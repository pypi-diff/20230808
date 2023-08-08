# Comparing `tmp/BDMLtools-0.3.7.tar.gz` & `tmp/BDMLtools-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BDMLtools-0.3.7.tar", last modified: Wed May 24 02:40:59 2023, max compression
+gzip compressed data, was "BDMLtools-0.3.8.tar", last modified: Tue Aug  8 08:48:04 2023, max compression
```

## Comparing `BDMLtools-0.3.7.tar` & `BDMLtools-0.3.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.453074 BDMLtools-0.3.7/
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.431130 BDMLtools-0.3.7/BDMLtools/
--rwxr-xr-x   0 zengke     (501) staff       (20)     1544 2023-05-23 09:54:46.000000 BDMLtools-0.3.7/BDMLtools/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)     7931 2022-09-16 05:41:25.000000 BDMLtools-0.3.7/BDMLtools/base.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.434763 BDMLtools-0.3.7/BDMLtools/clearner/
--rw-r--r--   0 zengke     (501) staff       (20)      303 2022-05-30 05:46:05.000000 BDMLtools-0.3.7/BDMLtools/clearner/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)    21550 2023-05-10 02:08:49.000000 BDMLtools-0.3.7/BDMLtools/clearner/cleaner.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.435751 BDMLtools-0.3.7/BDMLtools/encoder/
--rw-r--r--   0 zengke     (501) staff       (20)      230 2022-09-09 08:32:26.000000 BDMLtools-0.3.7/BDMLtools/encoder/__init__.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    13123 2022-10-26 06:18:44.000000 BDMLtools-0.3.7/BDMLtools/encoder/woe.py
--rw-r--r--   0 zengke     (501) staff       (20)      617 2022-05-30 05:46:05.000000 BDMLtools-0.3.7/BDMLtools/exception.py
--rwxr-xr-x   0 zengke     (501) staff       (20)     5965 2022-07-22 07:30:31.000000 BDMLtools-0.3.7/BDMLtools/fun.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.437502 BDMLtools-0.3.7/BDMLtools/plotter/
--rw-r--r--   0 zengke     (501) staff       (20)      280 2022-07-08 09:08:07.000000 BDMLtools-0.3.7/BDMLtools/plotter/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)    32833 2022-08-30 04:00:04.000000 BDMLtools-0.3.7/BDMLtools/plotter/base.py
--rw-r--r--   0 zengke     (501) staff       (20)    16452 2023-04-03 07:45:25.000000 BDMLtools-0.3.7/BDMLtools/plotter/eval.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.439099 BDMLtools-0.3.7/BDMLtools/report/
--rw-r--r--   0 zengke     (501) staff       (20)      379 2022-05-30 05:46:05.000000 BDMLtools-0.3.7/BDMLtools/report/__init__.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    49254 2023-05-11 06:09:02.000000 BDMLtools-0.3.7/BDMLtools/report/report.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.444082 BDMLtools-0.3.7/BDMLtools/selector/
--rw-r--r--   0 zengke     (501) staff       (20)      902 2022-11-22 04:09:12.000000 BDMLtools-0.3.7/BDMLtools/selector/__init__.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    30341 2023-01-31 10:03:44.000000 BDMLtools-0.3.7/BDMLtools/selector/bin.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    61178 2023-03-29 06:28:50.000000 BDMLtools-0.3.7/BDMLtools/selector/bin_fun.py
--rw-r--r--   0 zengke     (501) staff       (20)    12019 2023-04-03 06:42:57.000000 BDMLtools-0.3.7/BDMLtools/selector/embeded.py
--rw-r--r--   0 zengke     (501) staff       (20)    16406 2023-04-19 06:45:01.000000 BDMLtools-0.3.7/BDMLtools/selector/fa.py
--rw-r--r--   0 zengke     (501) staff       (20)    25071 2023-03-30 01:22:06.000000 BDMLtools-0.3.7/BDMLtools/selector/lgbm.py
--rw-r--r--   0 zengke     (501) staff       (20)    27613 2022-10-08 09:45:23.000000 BDMLtools-0.3.7/BDMLtools/selector/logtit.py
--rw-r--r--   0 zengke     (501) staff       (20)    30242 2023-03-29 06:26:13.000000 BDMLtools-0.3.7/BDMLtools/selector/simple.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.447754 BDMLtools-0.3.7/BDMLtools/tuner/
--rw-r--r--   0 zengke     (501) staff       (20)      438 2023-05-23 09:53:29.000000 BDMLtools-0.3.7/BDMLtools/tuner/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)     6112 2023-05-23 07:03:18.000000 BDMLtools-0.3.7/BDMLtools/tuner/base.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    34492 2023-05-23 08:19:23.000000 BDMLtools-0.3.7/BDMLtools/tuner/bayesian.py
--rwxr-xr-x   0 zengke     (501) staff       (20)     5750 2023-04-19 06:49:36.000000 BDMLtools-0.3.7/BDMLtools/tuner/fun.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    45735 2023-05-23 09:50:24.000000 BDMLtools-0.3.7/BDMLtools/tuner/gridcv.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    24712 2023-04-19 03:29:39.000000 BDMLtools-0.3.7/BDMLtools/tuner/halvingcv.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.433335 BDMLtools-0.3.7/BDMLtools.egg-info/
--rw-r--r--   0 zengke     (501) staff       (20)     2136 2023-05-24 02:40:59.000000 BDMLtools-0.3.7/BDMLtools.egg-info/PKG-INFO
--rw-r--r--   0 zengke     (501) staff       (20)     1046 2023-05-24 02:40:59.000000 BDMLtools-0.3.7/BDMLtools.egg-info/SOURCES.txt
--rw-r--r--   0 zengke     (501) staff       (20)        1 2023-05-24 02:40:59.000000 BDMLtools-0.3.7/BDMLtools.egg-info/dependency_links.txt
--rw-r--r--   0 zengke     (501) staff       (20)      481 2023-05-24 02:40:59.000000 BDMLtools-0.3.7/BDMLtools.egg-info/requires.txt
--rw-r--r--   0 zengke     (501) staff       (20)       15 2023-05-24 02:40:59.000000 BDMLtools-0.3.7/BDMLtools.egg-info/top_level.txt
--rw-r--r--   0 zengke     (501) staff       (20)     1062 2022-09-07 02:01:45.000000 BDMLtools-0.3.7/LICENSE
--rw-r--r--   0 zengke     (501) staff       (20)     2136 2023-05-24 02:40:59.452629 BDMLtools-0.3.7/PKG-INFO
--rw-r--r--   0 zengke     (501) staff       (20)     1610 2023-05-24 01:49:35.000000 BDMLtools-0.3.7/README.md
--rw-r--r--   0 zengke     (501) staff       (20)       38 2023-05-24 02:40:59.453204 BDMLtools-0.3.7/setup.cfg
--rwxr-xr-x   0 zengke     (501) staff       (20)     3662 2023-05-11 10:01:26.000000 BDMLtools-0.3.7/setup.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.451935 BDMLtools-0.3.7/test/
--rwxr-xr-x   0 zengke     (501) staff       (20)        0 2022-07-12 06:58:12.000000 BDMLtools-0.3.7/test/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)     9104 2022-09-06 10:00:06.000000 BDMLtools-0.3.7/test/test_base.py
--rw-r--r--   0 zengke     (501) staff       (20)     4500 2022-09-06 10:08:22.000000 BDMLtools-0.3.7/test/test_clearner.py
--rw-r--r--   0 zengke     (501) staff       (20)     1966 2022-08-30 07:06:15.000000 BDMLtools-0.3.7/test/test_eval.py
--rw-r--r--   0 zengke     (501) staff       (20)     4873 2023-05-12 07:52:29.000000 BDMLtools-0.3.7/test/test_report.py
--rw-r--r--   0 zengke     (501) staff       (20)    18928 2023-05-12 07:52:56.000000 BDMLtools-0.3.7/test/test_selector.py
--rw-r--r--   0 zengke     (501) staff       (20)    26124 2023-05-24 01:22:44.000000 BDMLtools-0.3.7/test/test_tunner.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-08-08 08:48:04.701685 BDMLtools-0.3.8/
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-08-08 08:48:04.677418 BDMLtools-0.3.8/BDMLtools/
+-rwxr-xr-x   0 zengke     (501) staff       (20)     1544 2023-08-07 09:11:44.000000 BDMLtools-0.3.8/BDMLtools/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)     7931 2022-09-16 05:41:25.000000 BDMLtools-0.3.8/BDMLtools/base.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-08-08 08:48:04.681951 BDMLtools-0.3.8/BDMLtools/clearner/
+-rw-r--r--   0 zengke     (501) staff       (20)      303 2022-05-30 05:46:05.000000 BDMLtools-0.3.8/BDMLtools/clearner/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)    21550 2023-05-10 02:08:49.000000 BDMLtools-0.3.8/BDMLtools/clearner/cleaner.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-08-08 08:48:04.683617 BDMLtools-0.3.8/BDMLtools/encoder/
+-rw-r--r--   0 zengke     (501) staff       (20)      230 2022-09-09 08:32:26.000000 BDMLtools-0.3.8/BDMLtools/encoder/__init__.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    13123 2022-10-26 06:18:44.000000 BDMLtools-0.3.8/BDMLtools/encoder/woe.py
+-rw-r--r--   0 zengke     (501) staff       (20)      617 2022-05-30 05:46:05.000000 BDMLtools-0.3.8/BDMLtools/exception.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)     5965 2022-07-22 07:30:31.000000 BDMLtools-0.3.8/BDMLtools/fun.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-08-08 08:48:04.686015 BDMLtools-0.3.8/BDMLtools/plotter/
+-rw-r--r--   0 zengke     (501) staff       (20)      280 2022-07-08 09:08:07.000000 BDMLtools-0.3.8/BDMLtools/plotter/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)    32821 2023-08-07 08:04:33.000000 BDMLtools-0.3.8/BDMLtools/plotter/base.py
+-rw-r--r--   0 zengke     (501) staff       (20)    16452 2023-04-03 07:45:25.000000 BDMLtools-0.3.8/BDMLtools/plotter/eval.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-08-08 08:48:04.687427 BDMLtools-0.3.8/BDMLtools/report/
+-rw-r--r--   0 zengke     (501) staff       (20)      379 2022-05-30 05:46:05.000000 BDMLtools-0.3.8/BDMLtools/report/__init__.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    51744 2023-08-07 09:31:10.000000 BDMLtools-0.3.8/BDMLtools/report/report.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-08-08 08:48:04.693901 BDMLtools-0.3.8/BDMLtools/selector/
+-rw-r--r--   0 zengke     (501) staff       (20)      902 2022-11-22 04:09:12.000000 BDMLtools-0.3.8/BDMLtools/selector/__init__.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    30471 2023-08-07 10:18:02.000000 BDMLtools-0.3.8/BDMLtools/selector/bin.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    61452 2023-08-07 10:13:02.000000 BDMLtools-0.3.8/BDMLtools/selector/bin_fun.py
+-rw-r--r--   0 zengke     (501) staff       (20)    12019 2023-04-03 06:42:57.000000 BDMLtools-0.3.8/BDMLtools/selector/embeded.py
+-rw-r--r--   0 zengke     (501) staff       (20)    16406 2023-04-19 06:45:01.000000 BDMLtools-0.3.8/BDMLtools/selector/fa.py
+-rw-r--r--   0 zengke     (501) staff       (20)    24803 2023-08-08 06:39:48.000000 BDMLtools-0.3.8/BDMLtools/selector/lgbm.py
+-rw-r--r--   0 zengke     (501) staff       (20)    27612 2023-05-26 02:13:45.000000 BDMLtools-0.3.8/BDMLtools/selector/logtit.py
+-rw-r--r--   0 zengke     (501) staff       (20)    30309 2023-08-08 06:20:25.000000 BDMLtools-0.3.8/BDMLtools/selector/simple.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-08-08 08:48:04.697440 BDMLtools-0.3.8/BDMLtools/tuner/
+-rw-r--r--   0 zengke     (501) staff       (20)      438 2023-05-23 09:53:29.000000 BDMLtools-0.3.8/BDMLtools/tuner/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)     5738 2023-08-08 06:18:50.000000 BDMLtools-0.3.8/BDMLtools/tuner/base.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    34501 2023-07-24 09:29:22.000000 BDMLtools-0.3.8/BDMLtools/tuner/bayesian.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)     5750 2023-04-19 06:49:36.000000 BDMLtools-0.3.8/BDMLtools/tuner/fun.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    45727 2023-07-24 09:24:08.000000 BDMLtools-0.3.8/BDMLtools/tuner/gridcv.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    24712 2023-04-19 03:29:39.000000 BDMLtools-0.3.8/BDMLtools/tuner/halvingcv.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-08-08 08:48:04.680511 BDMLtools-0.3.8/BDMLtools.egg-info/
+-rw-r--r--   0 zengke     (501) staff       (20)     2235 2023-08-08 08:48:04.000000 BDMLtools-0.3.8/BDMLtools.egg-info/PKG-INFO
+-rw-r--r--   0 zengke     (501) staff       (20)     1046 2023-08-08 08:48:04.000000 BDMLtools-0.3.8/BDMLtools.egg-info/SOURCES.txt
+-rw-r--r--   0 zengke     (501) staff       (20)        1 2023-08-08 08:48:04.000000 BDMLtools-0.3.8/BDMLtools.egg-info/dependency_links.txt
+-rw-r--r--   0 zengke     (501) staff       (20)      432 2023-08-08 08:48:04.000000 BDMLtools-0.3.8/BDMLtools.egg-info/requires.txt
+-rw-r--r--   0 zengke     (501) staff       (20)       15 2023-08-08 08:48:04.000000 BDMLtools-0.3.8/BDMLtools.egg-info/top_level.txt
+-rw-r--r--   0 zengke     (501) staff       (20)     1062 2022-09-07 02:01:45.000000 BDMLtools-0.3.8/LICENSE
+-rw-r--r--   0 zengke     (501) staff       (20)     2235 2023-08-08 08:48:04.701247 BDMLtools-0.3.8/PKG-INFO
+-rw-r--r--   0 zengke     (501) staff       (20)     1709 2023-08-08 07:49:46.000000 BDMLtools-0.3.8/README.md
+-rw-r--r--   0 zengke     (501) staff       (20)       38 2023-08-08 08:48:04.701781 BDMLtools-0.3.8/setup.cfg
+-rwxr-xr-x   0 zengke     (501) staff       (20)     4049 2023-06-12 09:52:00.000000 BDMLtools-0.3.8/setup.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-08-08 08:48:04.700641 BDMLtools-0.3.8/test/
+-rwxr-xr-x   0 zengke     (501) staff       (20)        0 2022-07-12 06:58:12.000000 BDMLtools-0.3.8/test/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)     9104 2022-09-06 10:00:06.000000 BDMLtools-0.3.8/test/test_base.py
+-rw-r--r--   0 zengke     (501) staff       (20)     4500 2022-09-06 10:08:22.000000 BDMLtools-0.3.8/test/test_clearner.py
+-rw-r--r--   0 zengke     (501) staff       (20)     1966 2022-08-30 07:06:15.000000 BDMLtools-0.3.8/test/test_eval.py
+-rw-r--r--   0 zengke     (501) staff       (20)     4899 2023-08-07 08:07:53.000000 BDMLtools-0.3.8/test/test_report.py
+-rw-r--r--   0 zengke     (501) staff       (20)    18928 2023-05-12 07:52:56.000000 BDMLtools-0.3.8/test/test_selector.py
+-rw-r--r--   0 zengke     (501) staff       (20)    26124 2023-05-24 01:22:44.000000 BDMLtools-0.3.8/test/test_tunner.py
```

### Comparing `BDMLtools-0.3.7/BDMLtools/__init__.py` & `BDMLtools-0.3.8/BDMLtools/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from BDMLtools.plotter import BaseWoePlotter
 from BDMLtools.plotter import perfEval,perfEval2
 from BDMLtools.encoder import woeTransformer,binTransformer
 from BDMLtools.tuner import gridTuner,hgridTuner,FLgridTuner
 from BDMLtools.tuner import BayesianCVTuner,FLBSTuner,shapCheck
 
 
-__version__ = '0.3.7'
+__version__ = '0.3.8'
 
 __all__ = (    
     dtStandardization,
     outliersTransformer,
     dtypeAllocator,
     nanTransformer,
     FLBSTuner,
```

### Comparing `BDMLtools-0.3.7/BDMLtools/base.py` & `BDMLtools-0.3.8/BDMLtools/base.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/BDMLtools/clearner/cleaner.py` & `BDMLtools-0.3.8/BDMLtools/clearner/cleaner.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/BDMLtools/encoder/woe.py` & `BDMLtools-0.3.8/BDMLtools/encoder/woe.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/BDMLtools/exception.py` & `BDMLtools-0.3.8/BDMLtools/exception.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/BDMLtools/fun.py` & `BDMLtools-0.3.8/BDMLtools/fun.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/BDMLtools/plotter/base.py` & `BDMLtools-0.3.8/BDMLtools/plotter/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         #dt transform
         binx=self._get_bin(binx)
         
         binx_melt=pd.melt(binx,id_vars = ["bin","rowid"], value_vars =["pos", "neg"], 
                     value_name = "negpos").rename(columns={'variable':''})
         
         #title
-        title_string = binx['variable'][0]+'(iv:{},ks:{})'.format(round(binx['total_iv'][0],4),round(binx['ks_max'][0],4))
+        title_string = binx['variable'][0]+'(iv:{},ks:{})'.format(round(binx['total_iv'][0],4),round(binx['ks'][0],4))
     
         #adjust max val of y-left axis
         y_right_max = np.ceil(binx['badprob'].max()*10)
     
         if y_right_max % 2 == 1: 
     
             y_right_max=y_right_max+1
@@ -133,19 +133,19 @@
     
         if sort_column:
     
             binx_g_h['g']=binx_g_h['g'].astype('category').cat.reorder_categories(sort_column)
             binx_g_melt['g']=binx_g_melt['g'].astype('category').cat.reorder_categories(sort_column)
     
         #title
-        binx_g_ivks=binx_g_h[['total_iv','ks_max']].droplevel(1)
+        binx_g_ivks=binx_g_h[['total_iv','ks']].droplevel(1)
         binx_g_ivks=binx_g_ivks.loc[~binx_g_ivks.index.duplicated(),:]
         
         iv_d=binx_g_ivks['total_iv'].to_dict()
-        ks_d=binx_g_ivks['ks_max'].to_dict()
+        ks_d=binx_g_ivks['ks'].to_dict()
     
         keys=sort_column if sort_column else iv_d.keys()
         
         #title
         title_string=binx_g_h['variable'][0]+':'+(',').join(['{}(iv:{},ks:{})'.format(key,round(iv_d[key],4),round(ks_d[key],4)) for key in keys])
     
         #adjust max val of y-left axis
```

### Comparing `BDMLtools-0.3.7/BDMLtools/plotter/eval.py` & `BDMLtools-0.3.8/BDMLtools/plotter/eval.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/BDMLtools/report/report.py` & `BDMLtools-0.3.8/BDMLtools/report/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -276,42 +276,44 @@
             
         writer.close()     
         print('to_excel done') 
         
 
 class varReportSinge(Base,Specials,BaseWoePlotter):
     
-    def report(self, X, y,breaks,sample_weight=None,special_values=None,regularization=1e-10):
+    def report(self, X, y,breaks,sample_weight=None,special_values=None,regularization=1e-10,show_metrics=True):
         """ 
         分箱并产生特征分析报告、特征分析绘图报告  
         Params:
         ------
         X:pd.Series,单特征x
         y:pd.Series,目标特征
         breaks:list,分箱点
         regularization=1e-10:float,计算好坏分布时正则项强度,用于应对iv、woe计算时分母为0的情况，
                                    regularization越高则强度越高，不同的regularization将影响iv、ks、woe的结算结果，
                                    默认regularization=1e-10情况下，出现分母为0的变量的IV将被高估
         sample_weight:pd.Seires or None,样本权重
         special_values:特殊值指代值,若数据中某些值或某列某些值需特殊对待(这些值不是np.nan)时设定
             请特别注意若使用binSelector产生breaks_list,special_values必须与binSelector的special_values一致,否则报告的special行会产生错误结果
             + None,保证数据默认
-            + list=[value1,value2,...],数据中所有列的值在[value1,value2,...]中都会被替换，字符被替换为'missing',数值被替换为np.nan          
+            + list=[value1,value2,...],数据中所有列的值在[value1,value2,...]中都会被替换，字符被替换为'missing',数值被替换为np.nan 
+        show_metrics:bool,默认True，输出ks、lift、auc指标。此类指标更适合评分类变量。注意此指标会受到分箱切分点、正则参数的影响。
+            + 设定20-50等频分箱、regularization=0时相关指标会接近真实水平               
         Return:
         ------
         report_var,pd.DataFrame:单特征分析报告       
         """       
         
         self._check_x(X)
         self._check_yname(y)
         breaks=self._check_breaks(breaks)
                 
         X=self._sp_replace_single(X,self._check_spvalues(X.name,special_values),fill_num=np.finfo(np.float32).max,fill_str='special')
                
-        report_var=self.getReport_Single(X,y,breaks,sample_weight,special_values,regularization)
+        report_var=self.getReport_Single(X,y,breaks,sample_weight,special_values,regularization,show_metrics)
         
         return report_var 
     
     
     def woe_plot(self,X, y,breaks,sample_weight=None,special_values=None,figure_size=None,show_plot=True):        
         """ 
         分箱并产生特征分析报告、特征分析绘图报告  
@@ -340,15 +342,15 @@
         report_var=self.report(X,y,breaks,sample_weight,special_values)
         
         figure=self. _get_plot_single(report_var,figure_size,show_plot)
     
         return report_var,figure,breaks
    
         
-    def getReport_Single(self,X,y,breakslist_var,sample_weight,special_values,regularization):         
+    def getReport_Single(self,X,y,breakslist_var,sample_weight,special_values,regularization,show_metrics):         
 
          col=X.name
 
          #处理缺失值
          var_fillna=X
          
          #breaklist_var=list(breaks_list_dict[col])
@@ -409,17 +411,15 @@
              
              if 'missing' in var_bin.cat.categories:
                  
                  var_bin= var_bin.fillna('missing') 
             
              else:
                  
-                 var_bin= var_bin.cat.add_categories('missing').fillna('missing')
-                 
-                
+                 var_bin= var_bin.cat.add_categories('missing').fillna('missing')                                 
              
          else:
              
              raise ValueError('dtypes in X in (number,object),others not support')
          
          #若只计算全量数据则只输出全量的特征分析报告
              
@@ -432,44 +432,56 @@
          
          #print var_bin
          rename_aggfunc=dict(zip(['sample_weight',y.name],['count','bad']))
          result=pd.pivot_table(var_bin,index=col,values=[y.name,'sample_weight'],
                            margins=False,
                            aggfunc='sum').rename(columns=rename_aggfunc,level=0)#.droplevel(level=1,axis=1) 
 
-         var_tab=self._getVarReport_ks(result,col,regularization) 
+         var_tab=self._getVarReport_ks(result,col,show_metrics,regularization) 
          
          if is_string_dtype(var_fillna):
              
              var_tab.index=var_tab.index.astype('category') 
 
          return  var_tab.assign(
              
              breaks=var_tab.index.categories.map(lambda x:x if isinstance(x,str) else x.right))
             
-    def _getVarReport_ks(self,var_ptable,col,regularization=1e-10):
+    def _getVarReport_ks(self,var_ptable,col,show_metrics,regularization=1e-10):
         
         var_ptable['badprob']=var_ptable['bad'].div(var_ptable['count'])
         var_ptable['count_distr']=var_ptable['count'].div(var_ptable['count'].sum())
         var_ptable['good']=var_ptable['count'].sub(var_ptable['bad'])
         var_ptable['good_dis']=var_ptable['good'].add(regularization).div(var_ptable['good'].sum()+2*regularization)
         var_ptable['bad_dis']=var_ptable['bad'].add(regularization).div(var_ptable['bad'].sum()+2*regularization)
         var_ptable['bin_iv']=var_ptable['bad_dis'].sub(var_ptable['good_dis']).mul(
             (var_ptable["bad_dis"]).div((var_ptable["good_dis"])).apply(np.log)
         )
         var_ptable['total_iv']=var_ptable['bin_iv'].sum()
         var_ptable['woe']=(var_ptable["bad_dis"]).div((var_ptable["good_dis"])).apply(np.log)
-        var_ptable['ks']=var_ptable['good_dis'].cumsum().sub(var_ptable['bad_dis'].cumsum()).abs()
-        var_ptable['ks_max']=var_ptable['ks'].max()
+        var_ptable['ks_bin']=var_ptable['good_dis'].cumsum().sub(var_ptable['bad_dis'].cumsum()).abs()
+        var_ptable['ks']=var_ptable['ks_bin'].max()
         var_ptable['lift']=var_ptable['badprob'].div(var_ptable['bad'].sum()/var_ptable['count'].sum())
+        var_ptable['auc_bin']=var_ptable['good_dis'].cumsum().diff(1).fillna(var_ptable['good_dis'].cumsum()[0]).mul(
+            var_ptable['bad_dis'].cumsum().shift(1).fillna(0).add(var_ptable['bad_dis'].cumsum())
+        ).div(2)
+        var_ptable['auc']=var_ptable['auc_bin'].sum()        
+        
         var_ptable['variable']=col
         var_ptable.index.name='bin'
         #var_ptable=var_ptable.reset_index()
         #var_ptable['bin']=var_ptable['bin'].astype('str')
-        var_ptable=var_ptable[['variable', 'count', 'count_distr', 'good', 'bad', 'badprob','woe', 'bin_iv', 'total_iv','ks','ks_max','lift']].copy()
+        if show_metrics:
+            
+            var_ptable=var_ptable[['variable', 'count', 'count_distr', 'good', 'bad', 'badprob','woe','total_iv','ks','lift','auc']].copy()
+            
+        else:
+            
+            var_ptable=var_ptable[['variable', 'count', 'count_distr', 'good', 'bad', 'badprob','woe','total_iv']].copy()
+            
         
         if var_ptable.loc['special','count'] == 0:
             
             var_ptable.loc['special','woe'] = 0
             
         if var_ptable.loc['missing','count'] == 0:
             
@@ -491,14 +503,16 @@
             + None,保证数据默认
             + list=[value1,value2,...],数据中所有列的值在[value1,value2,...]中都会被替换，字符被替换为'missing',数值被替换为np.nan
             + dict={col_name1:[value1,value2,...],...},数据中指定列替换，被指定的列的值在[value1,value2,...]中都会被替换，字符被替换为'missing',数值被替换为np.nan  
         sample_weight:numpy.array or pd.Series or None,样本权重，若数据是经过抽样获取的，则可加入样本权重以计算加权的badrate,woe,iv,ks等指标
         regularization=1e-10:float,计算好坏分布时正则项强度,用于应对iv、woe计算时分母为0的情况，
                                    regularization越高则强度越高，不同的regularization将影响iv、ks、woe的结算结果，
                                    默认regularization=1e-10情况下，出现分母为0的变量的IV将被高估
+        show_metrics:bool,默认True，输出ks、lift、auc指标。此类指标更适合评价分数类变量。注意此指标会受到分箱切分点、正则参数的影响。
+            + 设定20-50等频分箱、regularization=0时相关指标会接近真实水平                          
         out_path:将报告输出到本地工作目录的str文件夹下，None代表不输出 
         tab_suffix:本地excel报告名后缀
         n_jobs:int,并行计算job数
         verbose:int,并行计算信息输出等级
     
     Attributes:
     -------
@@ -508,38 +522,39 @@
     -------
         fit:产生特征报告
         transform:返回原始数据
         woe_plot:返回各个特征的woe_plot        
         
     """
     
-    def __init__(self,breaks_list_dict,special_values=None,sample_weight=None,out_path=None,tab_suffix='',regularization=1e-10,n_jobs=-1,verbose=0):
+    def __init__(self,breaks_list_dict,special_values=None,sample_weight=None,out_path=None,tab_suffix='',regularization=1e-10,show_metrics=True,n_jobs=-1,verbose=0):
 
         self.breaks_list_dict = breaks_list_dict
         self.special_values = special_values
         self.sample_weight = sample_weight
         self.n_jobs = n_jobs
         self.verbose = verbose
         self.out_path = out_path
         self.tab_suffix = tab_suffix
         self.regularization=regularization
+        self.show_metrics=show_metrics
         
         self._is_fitted=False
         
     def fit(self, X, y):
 
         self._check_data(X,y)
         self._check_yname(y)
         self.breaks_list_dict=self._check_breaks(self.breaks_list_dict)
         
         n_jobs=effective_n_jobs(self.n_jobs)
         
         parallel=Parallel(n_jobs=n_jobs,verbose=self.verbose,batch_size=100)
         
-        out_list=parallel(delayed(self._get_report_single)(X,y,col,self.breaks_list_dict[col],self.sample_weight,self.special_values,self.regularization)
+        out_list=parallel(delayed(self._get_report_single)(X,y,col,self.breaks_list_dict[col],self.sample_weight,self.special_values,self.regularization,self.show_metrics)
                           for col in self.breaks_list_dict)
         
         self.var_report_dict={col:total for col,total in out_list}
         
         #输出报告    
         if self.out_path: 
             
@@ -573,17 +588,17 @@
         self._check_is_fitted()
         
         fig_out=self._woe_plot(self.var_report_dict,figure_size,n_jobs,verbose)
         
         return fig_out
         
         
-    def _get_report_single(self,X,y,col_name,breaks,sample_weight,special_values,regularization):
+    def _get_report_single(self,X,y,col_name,breaks,sample_weight,special_values,regularization,show_metrics):
            
-        vtabs=varReportSinge().report(X[col_name],y,breaks,sample_weight,special_values,regularization)
+        vtabs=varReportSinge().report(X[col_name],y,breaks,sample_weight,special_values,regularization,show_metrics)
         
         return col_name,vtabs
 
     
     def _writeExcel(self):
         
         if not glob(self.out_path):
@@ -634,39 +649,42 @@
     special_values:特殊值指代值
             + None,保持数据默认
             + list=[value1,value2,...],数据中所有列的值在[value1,value2,...]中都会被替换，字符被替换为'missing',数值被替换为np.nan
             + dict={col_name1:[value1,value2,...],...},数据中指定列替换，被指定的列的值在[value1,value2,...]中都会被替换，字符被替换为'missing',数值被替换为np.nan  
     regularization=1e-10:float,计算好坏分布时正则项强度,用于应对iv、woe计算时分母为0的情况，
                                regularization越高则强度越高，不同的regularization将影响iv、ks、woe的结算结果，
                                默认regularization=1e-10情况下，出现分母为0的变量的IV将被高估
+    show_metrics:bool,默认True，输出ks、lift、auc指标。此类指标更适合评价分数类变量。注意此指标会受到分箱切分点、正则参数的影响。
+            + 设定20-50等频分箱、regularization=0时相关指标会接近真实水平                               
     sample_weight:numpy.array or pd.Series(...,index=X.index) or None,样本权重，若数据是经过抽样获取的，则可加入样本权重以计算加权的badrate,woe,iv,ks等指标以还原抽样对分析影响
     n_jobs:int,并行计算job数
     verbose:int,并行计算信息输出等级
     out_path:将报告输出到本地工作目录的str文件夹下，None代表不输出 
     tab_suffix:本地excel报告名后缀
     
     Attributes:
     -------
         report_dict:dict,所有产生的报告
         
     """        
     
     def __init__(self,breaks_list_dict,columns,sort_columns=None,target='target',row_limit=0,output_psi=False,psi_base='all',
-                 special_values=None,sample_weight=None,regularization=1e-10,n_jobs=-1,verbose=0,out_path=None,tab_suffix='_group'):
+                 special_values=None,sample_weight=None,regularization=1e-10,show_metrics=True,n_jobs=-1,verbose=0,out_path=None,tab_suffix='_group'):
 
         self.breaks_list_dict=breaks_list_dict
         self.target=target
         self.columns=columns
         self.sort_columns=sort_columns      
         self.row_limit=row_limit
         self.output_psi=output_psi
         self.psi_base=psi_base
         self.special_values=special_values
         self.sample_weight=sample_weight
         self.regularization=regularization
+        self.show_metrics=show_metrics
         self.n_jobs=n_jobs
         self.verbose=verbose
         self.out_path=out_path
         self.tab_suffix=tab_suffix
         
         self._is_fitted=False
        
@@ -703,15 +721,16 @@
         n_jobs=effective_n_jobs(self.n_jobs)
         
         parallel=Parallel(n_jobs=n_jobs,verbose=self.verbose)
         
         out_list=parallel(delayed(self._group_parallel)(X_g_gen,g,self.target,self.columns,
                                                        self.breaks_list_dict,self.row_limit,
                                                        self.special_values,
-                                                       self.regularization) for g in X_g_gen.groups)
+                                                       self.regularization,
+                                                       self.show_metrics) for g in X_g_gen.groups)
         
         self.report_dict_raw={columns:vtabs for columns,vtabs in out_list}
         
         if all(np.array([len(self.report_dict_raw[key]) for key in self.report_dict_raw])==0):
             
             raise ValueError('row_limit too high to get group report,reset it and try again')
 
@@ -719,32 +738,32 @@
         
         report.index.rename([None, 'bin'],inplace=True)
 
         if self.sort_columns:       
             
             sort_columns_list=self._check_columns_sort(self.sort_columns, self.columns, X)                                    
     
-            report=self._vtab_column_sort(sort_columns_list,report)                
+            report=self._vtab_column_sort(sort_columns_list,report,self.show_metrics)                
                   
         self.report_dict=self._getReport(X,report,self.breaks_list_dict,self.special_values,self.n_jobs,self.verbose,
-                                        self.target,self.regularization,self.output_psi,self.psi_base)                    
+                                        self.target,self.regularization,self.show_metrics,self.output_psi,self.psi_base)                    
 
         if self.out_path:
                 
             self._writeExcel()  
             
         self._is_fitted=True                  
                                          
         return self
     
     def transform(self, X):     
      
         return X
 
-    def _group_parallel(self,X_g_gen,g,target,columns,breaks_list_dict,row_limit,special_values,regularization):
+    def _group_parallel(self,X_g_gen,g,target,columns,breaks_list_dict,row_limit,special_values,regularization,show_metrics):
     
         group_dt=X_g_gen.get_group(g)
         X_g=group_dt.drop([target]+columns,axis=1)
         y_g=group_dt[target]      
         w_g=group_dt['sample_weight']      
         
         if len(X_g)==0:
@@ -761,48 +780,54 @@
         
         else:
         
             res=varReport(breaks_list_dict=breaks_list_dict,
                           special_values=special_values,
                           sample_weight=w_g,
                           regularization=regularization,
+                          show_metrics=show_metrics,
                           n_jobs=1,                                  
                           verbose=0).fit(X_g,y_g)
         
             result=pd.concat(res.var_report_dict)
             
         return g,result
     
     
    
-    def _getReport(self,X,report,breaks_list_dict,special_values,n_jobs,verbose,target,regularization,
+    def _getReport(self,X,report,breaks_list_dict,special_values,n_jobs,verbose,target,regularization,show_metrics,
                   output_psi=True,psi_base='all'):
         
         report_out={}
             
         report_out['report_all']=report[[i for i in report.columns.tolist() if i[-1] not in \
                                       ['variable']]].reset_index().rename(columns={'level_0':'variable'})
                 
         report_out['report_brief']=report[[i for i in report.columns.tolist() if i[-1] in \
-                                      ['count','badprob','total_iv','ks_max','lift']]].reset_index().rename(columns={'level_0':'variable'})   
+                                      ['count','badprob','total_iv','ks','lift']]].reset_index().rename(columns={'level_0':'variable'})   
                             
         report_out['report_count']=report[[i for i in report.columns.tolist() if i[-1] in \
                                       ['count']]].reset_index().rename(columns={'level_0':'variable'})  
                 
         report_out['report_badprob']=report[[i for i in report.columns.tolist() if i[-1] in \
-                                        ['badprob']]].reset_index().rename(columns={'level_0':'variable'}) 
-            
-        report_out['report_lift']=report[[i for i in report.columns.tolist() if i[-1] in \
-                                            ['lift']]].reset_index().rename(columns={'level_0':'variable'})      
+                                        ['badprob']]].reset_index().rename(columns={'level_0':'variable'})                  
                 
         report_out['report_iv']=report[[i for i in report.columns.tolist() if i[-1] in \
                                    ['total_iv']]].droplevel(level=1).reset_index().drop_duplicates().rename(columns={'index':'variable'})  
+            
+        if show_metrics:
+            
+            report_out['report_lift']=report[[i for i in report.columns.tolist() if i[-1] in \
+                                                ['lift']]].reset_index().rename(columns={'level_0':'variable'})      
+                
+            report_out['report_ks']=report[[i for i in report.columns.tolist() if i[-1] in \
+                                   ['ks']]].droplevel(level=1).reset_index().drop_duplicates().rename(columns={'index':'variable'}) 
                 
-        report_out['report_ks']=report[[i for i in report.columns.tolist() if i[-1] in \
-                                   ['ks_max']]].droplevel(level=1).reset_index().drop_duplicates().rename(columns={'index':'variable'}) 
+            report_out['report_auc']=report[[i for i in report.columns.tolist() if i[-1] in \
+                                   ['auc']]].droplevel(level=1).reset_index().drop_duplicates().rename(columns={'index':'variable'}) 
         
         if output_psi:
             
             if psi_base=='all':
                 
                 all_var=varReport(breaks_list_dict=breaks_list_dict,
                                   special_values=special_values,
@@ -819,15 +844,15 @@
                                       
                 psi_tab=pd.concat([report_distr,psi_sum]).sort_index()     
                 
                 if self.sort_columns:       
                     
                     sort_columns_list=self._check_columns_sort(self.sort_columns, self.columns, X)                                    
             
-                    psi_tab=self._vtab_column_sort(sort_columns_list,psi_tab)                          
+                    psi_tab=self._vtab_column_sort(sort_columns_list,psi_tab,show_metrics)                          
                                       
                 report_out['report_psi']=psi_tab.reset_index().rename(columns={'level_0':'variable'})
             
             else:            
                 
                 X_q=X.query(psi_base)
                 
@@ -849,36 +874,37 @@
                                       
                 psi_tab=pd.concat([report_distr,psi_sum]).sort_index()     
                                 
                 if self.sort_columns:       
                                     
                     sort_columns_list=self._check_columns_sort(self.sort_columns, self.columns, X)                                    
                             
-                    psi_tab=self._vtab_column_sort(sort_columns_list,psi_tab)                            
+                    psi_tab=self._vtab_column_sort(sort_columns_list,psi_tab,show_metrics)                            
                                       
                 report_out['report_psi']=psi_tab.reset_index().rename(columns={'level_0':'variable'})                                        
                 
         return report_out        
             
     
     def _psi(self,base,col):
     
         base=base.replace(0,1e-10)
         col=col.replace(0,1e-10)   
         psi_out=base.sub(col).mul(base.div(col).map(np.log))
 
         return psi_out            
     
-    def _vtab_column_sort(self,sort_columns,report):
+    def _vtab_column_sort(self,sort_columns,report,show_metrics):
         
         sort_columns=sort_columns.copy()
         
         vt_cols=['variable', 'count', 'count_distr', 'good', 'bad', 'badprob', 'woe',
-                 'bin_iv', 'total_iv', 'ks', 'ks_max','lift', 'breaks']
-
+                      'total_iv', 'ks','lift','auc','breaks'] if show_metrics else ['variable', 'count', 'count_distr', 'good', 'bad', 
+                                                                                             'badprob', 'woe', 'total_iv','breaks']
+            
         sort_columns.append(vt_cols)
         
         cols_sorted=list(product(*sort_columns))
         
         cols_sorted_c=cols_sorted.copy()
         
         for col in cols_sorted_c:
@@ -941,16 +967,20 @@
                               engine='openpyxl')
 
         self.report_dict['report_all'].to_excel(writer,sheet_name='bin_all')
         self.report_dict['report_brief'].to_excel(writer,sheet_name='bin_brief')
         self.report_dict['report_count'].to_excel(writer,sheet_name='bin_count')     
         self.report_dict['report_badprob'].to_excel(writer,sheet_name='bin_badprob')     
         self.report_dict['report_iv'].to_excel(writer,sheet_name='bin_iv') 
-        self.report_dict['report_ks'].to_excel(writer,sheet_name='bin_ks') 
-        self.report_dict['report_lift'].to_excel(writer,sheet_name='bin_lift') 
+        
+        if self.show_metrics:
+        
+            self.report_dict['report_ks'].to_excel(writer,sheet_name='bin_ks') 
+            self.report_dict['report_lift'].to_excel(writer,sheet_name='bin_lift') 
+            self.report_dict['report_auc'].to_excel(writer,sheet_name='bin_auc') 
         
         if self.output_psi:
             
             self.report_dict['report_psi'].to_excel(writer,sheet_name='bin_psi')  
         
             
         writer.close()
```

### Comparing `BDMLtools-0.3.7/BDMLtools/selector/__init__.py` & `BDMLtools-0.3.8/BDMLtools/selector/__init__.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/BDMLtools/selector/bin.py` & `BDMLtools-0.3.8/BDMLtools/selector/bin.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,16 +205,16 @@
             
             raise ValueError("method in ('freq','pretty','freq-kmeans','chi2','tree')")                              
         
         
         #get iv and ks 
         optbindf_ks=pd.concat(bin_res.values())           
 
-        self.iv_info=optbindf_ks.groupby('variable')['bin_iv'].sum().rename('total_iv')
-        self.ks_info=optbindf_ks.groupby('variable')['ks'].max().rename('ks_max')
+        self.iv_info=optbindf_ks.groupby('variable')['total_iv'].max().rename('total_iv')
+        #self.ks_info=optbindf_ks.groupby('variable')['ks'].max().rename('ks')
         
         #fliter by iv
         self.keep_col=self.iv_info[self.iv_info>=self.iv_limit].index.tolist()  
         
         if not self.keep_col:
             
             warnings.warn('iv_limit too high to keep any variables,reset iv_limit')  
@@ -332,14 +332,16 @@
                                                                 X,y,
                                                                 sample_weight=self.sample_weight,
                                                                 special_values=self.special_values,
                                                                 figure_size=self.figure_size)
             
         else:
             
+            self.breaks_list_dict={i:self.breaks_list_dict[i] for i in self.breaks_list_dict if i not in self.column}
+            
             breaks_list_adj,vtabs_dict_adj=self._get_breaks_adj_g(self.breaks_list_dict,
                                                                 X,y,
                                                                 column=self.column,
                                                                 sort_column=self.sort_column,
                                                                 psi_base=self.psi_base,
                                                                 sample_weight=self.sample_weight,
                                                                 special_values=self.special_values,
```

### Comparing `BDMLtools-0.3.7/BDMLtools/selector/bin_fun.py` & `BDMLtools-0.3.8/BDMLtools/selector/bin_fun.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,26 @@
 from scipy.stats import chi2,chi2_contingency
 from warnings import warn
 from BDMLtools.fun import raw_to_bin_sc,Specials
 from BDMLtools.base import Base
 from BDMLtools.report.report import varReportSinge
 
 
+
+class varReportSinge_a(varReportSinge):
+    
+    """ 
+    过滤掉LGBM的warning信息
+    """    
+    
+    def report(self, *args, **kwargs):        
+               
+        return super().report(*args, show_metrics=False, **kwargs)
+
+
 def R_pretty(low, high, n):
     '''
     pretty breakpoints, the same as pretty function in R
     
     Params
     ------
     low: minimal value 
@@ -243,15 +255,15 @@
         return breaks
 
     breaks_list={name_value[0]:get_breaks(name_value[1],y) 
                  for name_value in X.items()}
     
     breaks_list=Base()._check_breaks(breaks_list)
     
-    bins={col:varReportSinge().report(X[col],y,breaks_list[col],ws,special_values) for col in X.columns}
+    bins={col:varReportSinge_a().report(X[col],y,breaks_list[col],ws,special_values) for col in X.columns}
    
     return breaks_list,bins
 
 
 class binKmeans(Base,Specials):
     
     """ 
@@ -367,15 +379,15 @@
              iter_times=len(breaks)
              iters=0
              breaks=breaks
              
              #no merge if n_clusters<=bin_limit(user-defined)
              if n_clusters<bin_limit:
                  
-                 vtab=varReportSinge().report(col,y,breaks=breaks,sample_weight=ws,special_values=special_values)
+                 vtab=varReportSinge_a().report(col,y,breaks=breaks,sample_weight=ws,special_values=special_values)
                  
                  return col.name,breaks,vtab
              
              else:
              
                  
                  while True:
@@ -417,15 +429,15 @@
                      if n_clusters<=1:
                          
                          n_clusters=1
          
          
                      n_clusters=var_bin['badprob'].unique().size-1                
                      
-                     res_km=KMeans(n_clusters=n_clusters,random_state=random_state).fit_predict(var_bin[['badprob']])
+                     res_km=KMeans(n_clusters=n_clusters,random_state=random_state,n_init=10).fit_predict(var_bin[['badprob']])
                      res_km_s=pd.Series(res_km,var_bin.index,name='cluster')
          
                      #update string breaks
                      breaks=var_bin.groupby(res_km_s)['bin'].apply(lambda x : '%,%'.join(x)).tolist() 
          
                      #combine_ratio calculation
                      var_bin_ratio=var_bin['badprob'].diff(1).abs().div(var_bin.badprob+1e-10)
@@ -443,30 +455,30 @@
                          
                          break  
                      #stop condition 2/2:iters gt max iters
                      if iters>=iter_times:
                          
                          break
                          
-                 vtab=varReportSinge().report(col,y,breaks=breaks,sample_weight=ws,special_values=special_values)
+                 vtab=varReportSinge_a().report(col,y,breaks=breaks,sample_weight=ws,special_values=special_values)
                  return col.name,breaks,vtab
      
          elif is_numeric_dtype(var_raw):
              
              #initialize params
              combine_ratio_count=True
              n_clusters=len(breaks)+1
              iter_times=col.unique().size
              iters=0
              breaks=breaks
              
              #no merge if n_clusters<=bin_limit(user-defined)
              if n_clusters<bin_limit:
                  
-                 vtab=varReportSinge().report(col,y,breaks=breaks,sample_weight=ws,special_values=special_values)
+                 vtab=varReportSinge_a().report(col,y,breaks=breaks,sample_weight=ws,special_values=special_values)
                  
                  return col.name,breaks,vtab
              
              else:
              
                  while True:
         
@@ -544,15 +556,15 @@
                      #stop condition 2/2:iters gt max iters
                      if iters>=iter_times:
                          
                          #print('iter_times')
                          
                          break
                      
-                 vtab=varReportSinge().report(col,y,breaks=breaks,sample_weight=ws,special_values=special_values)
+                 vtab=varReportSinge_a().report(col,y,breaks=breaks,sample_weight=ws,special_values=special_values)
                  
                  return col.name,breaks,vtab
              
          #列类型为其他特殊情况    
          else:
              
              raise ValueError("col's dtype in (number,object).")
@@ -680,36 +692,36 @@
                       
             
             #no cut applied when col's unique value pop too high               
             if col.value_counts(dropna=False).div(col.size).max()>0.95:
                 
                 breaks=[]       
                 
-                vtab=varReportSinge().report(col_raw,y,breaks,sample_weight=ws,special_values=special_values)
+                vtab=varReportSinge_a().report(col_raw,y,breaks,sample_weight=ws,special_values=special_values)
                 
             elif np.unique(col[~np.isnan(col)]).size==1:
                 
                 breaks=[]
                 
-                vtab=varReportSinge().report(col_raw,y,breaks,sample_weight=ws,special_values=special_values)
+                vtab=varReportSinge_a().report(col_raw,y,breaks,sample_weight=ws,special_values=special_values)
             
             #tree cut
             else:
                 
                 breaks=self._get_bestsplit(col.values,y.values,max_bin=max_bin,
                                      criteria=criteria,
                                      max_iters=100,
                                      tol=0.0001,
                                      ws=ws,
                                      distr_limit=distr_limit,
                                      is_str_dtype=False,
                                      coerce_monotonic=coerce_monotonic,
                                      bin_num_limit=bin_num_limit)
                 
-                vtab=varReportSinge().report(col_raw,y,breaks,sample_weight=ws,special_values=special_values)
+                vtab=varReportSinge_a().report(col_raw,y,breaks,sample_weight=ws,special_values=special_values)
         
         #string columns         
         elif is_string_dtype(col):
             
             
             if np.unique(col).size==1:
             
@@ -732,15 +744,15 @@
                                          distr_limit=distr_limit,
                                          is_str_dtype=True,
                                          bin_num_limit=bin_num_limit)
                 
                 #restore string breaks
                 breaks=['%,%'.join(i) for i in np.split(codes,np.int32(breaks_raw)) if i.tolist()]    
             
-            vtab=varReportSinge().report(col_raw,y,breaks,sample_weight=ws,special_values=special_values)
+            vtab=varReportSinge_a().report(col_raw,y,breaks,sample_weight=ws,special_values=special_values)
             
         else:
             
             raise ValueError("col's dtype in ('number','object')")
   
 
         return col.name,breaks,vtab
@@ -1072,15 +1084,15 @@
                 #chi2_merge
                 breaks=self._chi2_merge(col.values,y.values,ws=ws,max_bin=max_bin,
                               distr_limit=distr_limit,stop_limit=tol,
                               bin_num_limit=bin_num_limit,is_str_dtype=False,
                               coerce_monotonic=coerce_monotonic)
             
             #get vtab using chi2-breaks
-            vtab=varReportSinge().report(col_raw,y,breaks,sample_weight=ws,special_values=special_values)
+            vtab=varReportSinge_a().report(col_raw,y,breaks,sample_weight=ws,special_values=special_values)
             
         elif is_string_dtype(col):
             
             #print(col.name)
             
             #no merge applied when only one unique value existed in col
             if np.unique(col).size==1:
@@ -1100,15 +1112,15 @@
                                       bin_num_limit=bin_num_limit,
                                       is_str_dtype=True)
     
                 #restore string breaks
                 breaks=['%,%'.join(i) for i in np.split(codes,np.int32(breaks_raw)) if i.tolist()] 
             
             #get vtab using chi2-breaks
-            vtab=varReportSinge().report(col_raw,y,breaks,sample_weight=ws,special_values=special_values)
+            vtab=varReportSinge_a().report(col_raw,y,breaks,sample_weight=ws,special_values=special_values)
     
         else:
                 
             raise ValueError("col's dtype in ('number','object')")    
             
             
         return col.name,breaks,vtab     
@@ -1440,15 +1452,15 @@
                 #merge
                 breaks=self._pretty_merge(col.values,y.values,ws=ws,max_bin=max_bin,
                               distr_limit=distr_limit,
                               bin_num_limit=bin_num_limit,is_str_dtype=False,
                               coerce_monotonic=coerce_monotonic)
             
             #get vtab using chi2-breaks
-            vtab=varReportSinge().report(col_raw,y,breaks,sample_weight=ws,special_values=special_values)
+            vtab=varReportSinge_a().report(col_raw,y,breaks,sample_weight=ws,special_values=special_values)
             
         elif is_string_dtype(col):
             
             #no merge applied when only one unique value existed in col
             if np.unique(col).size==1:
                 
                 breaks=[]
@@ -1466,15 +1478,15 @@
                                       bin_num_limit=bin_num_limit,
                                       is_str_dtype=True)
     
                 #restore string breaks
                 breaks=['%,%'.join(i) for i in np.split(codes,np.int32(breaks_raw)) if i.tolist()] 
             
             #get vtab using chi2-breaks
-            vtab=varReportSinge().report(col_raw,y,breaks,sample_weight=ws,special_values=special_values)
+            vtab=varReportSinge_a().report(col_raw,y,breaks,sample_weight=ws,special_values=special_values)
     
         else:
                 
             raise ValueError("col's dtype in ('number','object')")    
             
             
         return col.name,breaks,vtab
```

### Comparing `BDMLtools-0.3.7/BDMLtools/selector/embeded.py` & `BDMLtools-0.3.8/BDMLtools/selector/embeded.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/BDMLtools/selector/fa.py` & `BDMLtools-0.3.8/BDMLtools/selector/fa.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/BDMLtools/selector/lgbm.py` & `BDMLtools-0.3.8/BDMLtools/selector/lgbm.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 from BDMLtools.base import Base
 from BDMLtools.tuner.base import BaseTunner
 from sklearn.model_selection import RepeatedStratifiedKFold
 from probatus.feature_elimination import EarlyStoppingShapRFECV,ShapRFECV
 from sklearn.model_selection import train_test_split
 from sklearn.inspection import permutation_importance
 from skopt import BayesSearchCV
-from BDMLtools.tuner.base import sLGBMClassifier
+from lightgbm import LGBMClassifier
 from BDMLtools.selector.bin_fun import R_pretty
-import warnings
 from mlxtend.feature_selection import SequentialFeatureSelector
 from sklearn.base import TransformerMixin
 import numpy as np
 
 
 class LgbmPISelector(TransformerMixin,Base,BaseTunner):
     
@@ -127,48 +126,48 @@
         
         if self.method=='raw':
                         
             if self.early_stopping_rounds:
                 
                 X_tr, X_val, y_tr, y_val = train_test_split(X,y,test_size=self.validation_fraction,random_state=self.random_state,stratify=y)
                 
-                estimator=sLGBMClassifier(random_state=self.random_state,
+                estimator=LGBMClassifier(random_state=self.random_state,verbose=-1,
                                           #n_jobs=effective_n_jobs(self.n_jobs),
                                           **self.clf_params).fit(
                     X_tr,y_tr,**self._get_fit_params(X_val,y_val,sample_weight,y.index,y_val.index)
                 )
                 
             else:
                 
-                estimator = sLGBMClassifier(random_state=self.random_state,
+                estimator = LGBMClassifier(random_state=self.random_state,verbose=-1,
                                             #n_jobs=effective_n_jobs(self.n_jobs),
                                             **self.clf_params).fit(
                     X,y,**{'sample_weight':sample_weight})  
                                                          
         else:
             
             para_space=self.clf_params if self.clf_params else self._lgbm_hpsearch_default()
             
             if self.early_stopping_rounds:
                 
                 X_tr, X_val, y_tr, y_val = train_test_split(X,y,test_size=self.validation_fraction,random_state=self.random_state,stratify=y)
 
                 self._BayesSearch_CV(para_space,X_tr,y_tr,None if sample_weight is None else sample_weight[y_tr.index])
     
-                estimator=sLGBMClassifier(random_state=self.random_state,
+                estimator=LGBMClassifier(random_state=self.random_state,verbose=-1,
                                           #n_jobs=effective_n_jobs(self.n_jobs),
                                           **self.bs_res.best_params_).fit(
                     X_tr,y_tr,**self._get_fit_params(X_val,y_val,sample_weight,y.index,y_val.index)
                 )  
             
             else:
                 
                 self._BayesSearch_CV(para_space,X,y,sample_weight)
                 
-                estimator = sLGBMClassifier(random_state=self.random_state,
+                estimator = LGBMClassifier(random_state=self.random_state,verbose=-1,
                                             #n_jobs=effective_n_jobs(self.n_jobs),
                                             **self.bs_res.best_params_).fit(
                     X,y,**{'sample_weight':sample_weight})  
                 
          
         self.pi = permutation_importance(estimator, X, y, n_repeats=self.pi_repeats,random_state=self.random_state,
                                          scoring=self.scoring,n_jobs=effective_n_jobs(self.n_jobs))
@@ -219,15 +218,15 @@
             scorer=self.scoring             
                     
         cv = RepeatedStratifiedKFold(n_splits=self.cv, n_repeats=self.repeats, random_state=self.random_state)
         
         n_jobs=effective_n_jobs(self.n_jobs)
                         
         bs=BayesSearchCV(
-            sLGBMClassifier(random_state=self.random_state),#,n_jobs=n_jobs
+            LGBMClassifier(random_state=self.random_state,verbose=-1),#,n_jobs=n_jobs
             para_space,cv=cv,
             n_iter=self.n_iter,n_points=self.init_points,
             n_jobs=n_jobs,#-1 if self.n_jobs==-1 else 1,
             verbose=self.verbose,refit=False,random_state=self.random_state,
             scoring=scorer,error_score=0)       
         
         self.bs_res=bs.fit(X,y,**{'sample_weight':sample_weight})
@@ -237,15 +236,14 @@
     @staticmethod
     def _lgbm_hpsearch_default():
 
         from skopt.utils import Categorical,Real,Integer
 
         para_space={
             'boosting_type':Categorical(['goss','gbdt']),
-            'verbose':Categorical([-1]), 
             'n_estimators': Integer(low=200, high=300, prior='uniform', transform='identity'),
             'learning_rate': Real(low=0.05, high=0.2, prior='uniform', transform='identity'),
             'max_depth': Integer(low=2, high=4, prior='uniform', transform='identity')            
         }
         
         return para_space
     
@@ -340,26 +338,16 @@
             
             keep_cols=self.clf.get_reduced_features_set(self.min_features_to_select)
             
         return X[keep_cols]
     
         
     def fit(self,X,y,cat_features=None,sample_weight=None,check_additivity=True):
-    
-        if not self.verbose:
-    
-            with warnings.catch_warnings():   
-
-                warnings.filterwarnings("ignore")
-
-                return self._fit(X,y,cat_features=None,sample_weight=None,check_additivity=check_additivity)
-            
-        else:
-            
-            return self._fit(X,y,cat_features=None,sample_weight=None,check_additivity=check_additivity)
+         
+        return self._fit(X,y,cat_features=None,sample_weight=None,check_additivity=check_additivity)
 
     
     
     def _fit(self,X,y,cat_features=None,sample_weight=None,check_additivity=True):
         
         """
         Parameters:
@@ -380,53 +368,54 @@
     
         cv = RepeatedStratifiedKFold(n_splits=self.cv, n_repeats=self.repeats, random_state=self.random_state)       
         
         n_jobs=effective_n_jobs(self.n_jobs)
 
         if self.method=='raw':
             
-            estimator=sLGBMClassifier(random_state=self.random_state,
+            estimator=LGBMClassifier(random_state=self.random_state,
+                                     verbose=-1,
                                       #n_jobs=effective_n_jobs(self.n_jobs),
                                       **self.clf_params)
             
         else:
             
             para_space=self.clf_params if self.clf_params else self._lgbm_hpsearch_default()
     
             
-            estimator=BayesSearchCV(sLGBMClassifier(random_state=self.random_state),para_space,
+            estimator=BayesSearchCV(LGBMClassifier(random_state=self.random_state,verbose=-1),para_space,
                                     n_iter=self.n_iter,n_points=self.n_points,
                                     random_state=self.random_state,
                                     n_jobs=n_jobs,#-1 if self.n_jobs==-1 else 1,
                                     verbose=self.verbose,cv=cv)
         
         if self.early_stopping_rounds:
         
         
             self.clf=EarlyStoppingShapRFECV(estimator,
                                         min_features_to_select=self.min_features_to_select,
                                         step=self.step,
                                         random_state=self.random_state,
                                         scoring=self.scoring,
                                         n_jobs=n_jobs,#-1 if self.n_jobs==-1 else 1,
-                                        verbose=-1,
+                                        verbose=self.verbose,
                                         early_stopping_rounds=self.early_stopping_rounds,
                                         cv=cv)
         
             self.clf.fit_compute(X,y,check_additivity=check_additivity,sample_weight=sample_weight)
             
         else:
 
             self.clf=ShapRFECV(estimator,
                                 min_features_to_select=self.min_features_to_select,
                                 step=self.step,
                                 random_state=self.random_state,
                                 scoring=self.scoring,
                                 n_jobs=n_jobs,#-1 if self.n_jobs==-1 else 1,
-                                verbose=-1,
+                                verbose=self.verbose,
                                 cv=cv)
         
             self.clf.fit_compute(X,y,check_additivity=check_additivity,sample_weight=sample_weight)
             
         
         self._is_fitted=True
     
@@ -434,15 +423,14 @@
     
     @staticmethod
     def _lgbm_hpsearch_default():
 
         from skopt.utils import Categorical,Real,Integer
 
         para_space={
-            'verbose':Categorical([-1]), 
             'boosting_type':Categorical(['goss','gbdt']),
             'n_estimators': Integer(low=30, high=300, prior='uniform', transform='identity'),
             'learning_rate': Real(low=0.05, high=0.2, prior='uniform', transform='identity'),
             'max_depth': Integer(low=1, high=4, prior='uniform', transform='identity')
         }
         
         return para_space
@@ -523,15 +511,15 @@
     Method:    
     --        
         fit(X,y,categorical_feature):拟合模型，categorical_feature为分类列列名list,默认None
         transform(X):对X进行特征筛选，返回筛选后的数据
         
     '''     
 
-    def __init__(self,forward=False,floating=False,k_features=5,clf_params={'verbose':-1},scoring='roc_auc',
+    def __init__(self,forward=False,floating=False,k_features=5,clf_params={},scoring='roc_auc',
                  cv=5,repeats=1,fixed_features=None,
                  random_state=123,n_jobs=-1,verbose=0):
         
         self.forward=forward
         self.floating=floating
         self.k_features=k_features
         self.clf_params=clf_params
@@ -578,15 +566,15 @@
         
         X=X.select_dtypes('number')
      
         cv = RepeatedStratifiedKFold(n_splits=self.cv, n_repeats=self.repeats, random_state=self.random_state)       
         
         n_jobs=effective_n_jobs(self.n_jobs)
         
-        lgbm=sLGBMClassifier(random_state=self.random_state,**self.clf_params)
+        lgbm=LGBMClassifier(random_state=self.random_state,verbose=-1,**self.clf_params)
         
         seq_clf = SequentialFeatureSelector(lgbm,                                            
                         k_features=self.k_features,
                         forward=self.forward,
                         floating=self.floating,
                         verbose=self.verbose,  
                         scoring=self.scoring,
```

### Comparing `BDMLtools-0.3.7/BDMLtools/selector/logtit.py` & `BDMLtools-0.3.8/BDMLtools/selector/logtit.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,15 +566,15 @@
         elif isinstance(self.logit_model,LogisticRegression):  
             
             logit_model_coef=dict(zip(self.logit_model.feature_names_in_.tolist(),self.logit_model.coef_.tolist()[0]))
             logit_model_intercept=self.logit_model.intercept_[0]
             self.columns=self.logit_model.feature_names_in_.tolist()
             
         else:
-            raise ValueError('type(logit_model) in (statsmodels..BinaryResultsWrapper;GLMResultsWrapper,sklearn.linear_model._logistic.LogisticRegression)')
+            raise ValueError('type(logit_model) in (statsmodels.BinaryResultsWrapper;GLMResultsWrapper,sklearn.linear_model._logistic.LogisticRegression)')
             
         self.scorecard=self._getPoints(self.varbin,logit_model_coef,logit_model_intercept,self.digit)
         
         self._is_fitted=True
         
         return self
```

### Comparing `BDMLtools-0.3.7/BDMLtools/selector/simple.py` & `BDMLtools-0.3.8/BDMLtools/selector/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from BDMLtools.fun import Specials
 from BDMLtools.selector.bin_fun import binFreq
 from sklearn.preprocessing import StandardScaler
 import numpy as np
 import pandas as pd
 import os
 from glob import glob
-from BDMLtools.tuner.base import sLGBMClassifier
+from lightgbm import LGBMClassifier
 from BDMLtools.base import Base
 #from lofo import LOFOImportance, Dataset
 from sklearn.feature_selection import SelectFpr,SelectFdr,SelectFwe
 #from BDMLtools.selector.lgbm import LgbmPISelector
 from joblib import effective_n_jobs
 
 
@@ -139,17 +139,18 @@
         
         
         max_depth=params['max_depth'] if 'max_depth' in params else 3
         learning_rate=params['learning_rate'] if 'learning_rate' in params else 0.01
         n_estimators=params['n_estimators'] if 'n_estimators' in params else 100
         n_jobs=params['n_jobs'] if 'n_jobs' in params else -1
 
-        lgb=sLGBMClassifier(
+        lgb=LGBMClassifier(
                 boosting_type='gbdt',
                 objective = 'binary',
+                verbose=-1,
                 learning_rate=learning_rate,
                 n_estimators=n_estimators,
                 max_depth=max_depth,
                 n_jobs=effective_n_jobs(n_jobs)
             ).fit(X_new,y,sample_weight=sample_weight)         
             
         return lgb
@@ -671,39 +672,41 @@
         
         if X_category.columns.size:
             
             X_category_encode=OrdinalEncoder().fit_transform(X_category).sub(1)
             
             X_new=pd.concat([X_numeric,X_category_encode],axis=1)
 
-            lgb=sLGBMClassifier(
+            lgb=LGBMClassifier(
                 boosting_type='gbdt',
                 objective = 'binary',
                 learning_rate=0.1,
                 n_estimators=tree_size,
                 random_state=123,
                 subsample=0.7,
                 colsample_bytree=1,
+                verbose=-1,
                 n_jobs=effective_n_jobs(self.n_jobs)
             ).fit(X_new,y,sample_weight=sample_weight,categorical_feature=X_category_encode.columns.tolist())         
 
             lgb_imps=lgb.booster_.feature_importance(importance_type='split')
         
             return X_new.columns[lgb_imps>tree_imps].tolist()+X_oth.columns.tolist()
         
         elif X_numeric.columns.size:
             
-            lgb=sLGBMClassifier(
+            lgb=LGBMClassifier(
                 boosting_type='gbdt',
                 objective = 'binary',
                 learning_rate=0.1,
                 n_estimators=tree_size,
                 random_state=123,
                 subsample=0.7,
                 colsample_bytree=1,
+                verbose=-1,
                 n_jobs=effective_n_jobs(self.n_jobs)
             ).fit(X_numeric,y,sample_weight=sample_weight)         
 
             lgb_imps=lgb.booster_.feature_importance(importance_type='split')
         
             return X_numeric.columns[lgb_imps>tree_imps].tolist()+X_oth.columns.tolist()
         
@@ -804,15 +807,15 @@
                 raise ValueError("tree_imps is in [0,inf]")     
             
     
         if self.iv_limit is not None:
             
             if not self.iv_limit>0:
                 
-                raise ValueError("auc_limit is in (0,inf]")           
+                raise ValueError("iv_limit is in (0,inf]")           
 
 
     def _writeExcel(self):
         
         if not glob(self.out_path):
             
             os.mkdir(self.out_path)
```

### Comparing `BDMLtools-0.3.7/BDMLtools/tuner/base.py` & `BDMLtools-0.3.8/BDMLtools/tuner/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from sklearn import metrics
 import numpy as np
 import pandas as pd
 from lightgbm import LGBMClassifier
-import warnings
 from scipy import special
 
 
 class BaseTunner:
     
     @property
     def _get_scorer(self):
@@ -92,30 +91,16 @@
         
         return np.round(score,0)
     
     
     def _cvresult_to_df(self,cv_results_):
     
         return pd.DataFrame(cv_results_)   
-
-
-class sLGBMClassifier(LGBMClassifier):
     
-    """ 
-    过滤掉LGBM的warning信息
-    """    
     
-    def fit(self, *args, **kwargs):        
-        
-        with warnings.catch_warnings():   
-            
-            warnings.filterwarnings("ignore", category=UserWarning)
-            
-            return super().fit(*args, verbose=False, **kwargs)
-        
         
 class FLLGBMSklearn(LGBMClassifier):
     """ 
     适合Focal Loss的lightgbm
     改造了predict_proba，注意前提为init_score被设定为定值
     """
```

### Comparing `BDMLtools-0.3.7/BDMLtools/tuner/bayesian.py` & `BDMLtools-0.3.8/BDMLtools/tuner/bayesian.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     
             para_space = {
                 'boosting_type':Categorical(['gbdt','goss']),
                 'n_estimators': Integer(30, 120),
                 'max_depth':Integer(2, 4),
                 'learning_rate': Real(0.05, 0.2,prior='uniform'),
             
-                'min_split_gain': Real(0, 10,prior='uniform'),
+                #'min_split_gain': Real(0, 10,prior='uniform'),
                 'min_child_samples':Integer(1, 100,prior='uniform'),
                 
                 'subsample':Real(0.5,1.0,prior='uniform'),
                 'colsample_bytree':Real(0.5,1.0,prior='uniform'),
                 'reg_lambda':Real(0,10,prior='uniform'),    
             } 
                         
@@ -467,15 +467,15 @@
         
             + 为解决样本不平衡问题而被提出的Focal Loss，通过引入类权重与对减少易分类样本的损失贡献同时增加难分类样本的损失贡献来减少样本不平衡问题
             + Focal Loss是一种变种的交叉熵损失函数,存在一阶、二阶导数，因此满足lgbm、xgb的要求
             + 对于样本不平衡问题,相较于传统样本处理方法(欠抽样、过抽样、smote、加权...)，Focal Loss提供了新的思路(由损失函数的构造方向解决样本不平衡问题)
             + Focal Loss中包含了类权重(alpha)，范围为(0,1),因此本模块不支持额外得再设定类权重、样本权重
             + Focal Loss中的gamma[0,+inf)值能减少易分类样本的损失贡献同时增加难分类样本的损失贡献。原始论文中gamma=2时效果最好            
                          
-        参考文献:
+        参考资料:
         [FocalLoss论文:Focal Loss for Dense Object Detection](https://arxiv.org/abs/1708.02002)
         [Lightgbm中Focal Loss损失函数的应用-scipy求导](https://github.com/jrzaurin/LightGBM-with-Focal-Loss)
         [Lightgbm中Focal Loss损失函数的应用-手工求导](https://maxhalford.github.io/blog/lightgbm-focal-loss/)
         [Lightgbm中自定义损失函数下预测边际值无法复现的问题](https://github.com/microsoft/LightGBM/issues/3312)
         
         Parameters:
         --
@@ -503,20 +503,20 @@
         
                 para_space = {
                     'boosting_type':Categorical(['gbdt','goss']),
                     'n_estimators': Integer(30, 120),
                     'max_depth':Integer(2, 4),
                     'learning_rate': Real(0.05, 0.2,prior='uniform'),
                 
-                    'min_split_gain': Real(0, 10,prior='uniform'),
+                    'min_split_gain': Real(0, 0.02,prior='uniform'),
                     'min_child_samples':Integer(1, 100,prior='uniform'),
                     
                     'subsample':Real(0.5,1.0,prior='uniform'),
                     'colsample_bytree':Real(0.5,1.0,prior='uniform'),
-                    'reg_lambda':Real(0,10,prior='uniform'),    
+                    'reg_lambda':Real(0,0.01,prior='uniform'),    
                 }                                  
               """   
               
         Attribute:    
         --
             params_best:最优参数组合,需先使用fit
             model_refit:最优参数下的lgbm模型,需先使用fit
@@ -831,20 +831,20 @@
 
                 'verbose':Categorical([-1]),
                 'boosting_type':Categorical(['gbdt','goss']),
                 'n_estimators': Integer(30, 120),
                 'max_depth':Integer(2, 4),
                 'learning_rate': Real(0.05, 0.2,prior='uniform'),
 
-                'min_split_gain': Real(0, 10,prior='uniform'),
+                'min_split_gain': Real(0, 0.02,prior='uniform'),
                 'min_child_samples':Integer(1, 100,prior='uniform'),
 
                 'subsample':Real(0.5,1.0,prior='uniform'),
                 'colsample_bytree':Real(0.5,1.0,prior='uniform'),
-                'reg_lambda':Real(0,10,prior='uniform'),    
+                'reg_lambda':Real(0,0.01,prior='uniform'),    
             } 
 
             # elif Estimator.__module__ == "catboost.core":
 
             #     para_space = {
 
             #         'n_estimators': Integer(30, 120),
```

### Comparing `BDMLtools-0.3.7/BDMLtools/tuner/fun.py` & `BDMLtools-0.3.8/BDMLtools/tuner/fun.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/BDMLtools/tuner/gridcv.py` & `BDMLtools-0.3.8/BDMLtools/tuner/gridcv.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,41 +600,40 @@
                  
                 para_space={
                      'boosting_type':['gbdt','goss'], 
                      'n_estimators':[100],
                      'learning_rate':[0.1], 
                     
                      'max_depth':[3],#[0,∞],
-                     'min_split_gain': [0],
+                     'min_split_gain': [0,0.02] #0-0.02,
                      'min_child_weight':[0],
                      
                      'scale_pos_weight':[1],
                      'subsample':[0.6,0.8],
                      'colsample_bytree' :[0.6,0.8],
-                     'reg_lambda':[0,10], 
+                     'reg_lambda':[0,0.01] #0-0.01, 
                      }
                 
              当Estimator=LGBMClassifier,method="random_grid": 
                  
                  from scipy.stats import randint as sp_randint
                  from scipy.stats import uniform as sp_uniform 
                  
                  para_space={
                      'boosting_type':['gbdt','goss'], #'goss','gbdt'
                      'n_estimators':sp_randint(low=100,high=110),
                      'learning_rate':sp_uniform(loc=0.1,scale=0), 
                     
                      'max_depth':sp_randint(low=2,high=4),#[0,∞],
-                     'min_split_gain': sp_uniform(loc=0,scale=0),
+                     'min_split_gain': sp_uniform(loc=0,scale=0),#0-0.02
                      'min_child_samples': sp_randint(low=100,high=300),#[0,∞],
                      
-                     'scale_pos_weight':[1],
                      'subsample':sp_uniform(loc=0.5,scale=0.5),
                      'colsample_bytree' :sp_uniform(loc=0.5,scale=0.5),
-                     'reg_lambda':sp_uniform(loc=0,scale=20),
+                     'reg_lambda':sp_uniform(loc=0,scale=20),#0-0.01
                      }
                 
         """   
     
     Attribute:    
     --
         cv_result:交叉验证结果,需先使用fit
```

### Comparing `BDMLtools-0.3.7/BDMLtools/tuner/halvingcv.py` & `BDMLtools-0.3.8/BDMLtools/tuner/halvingcv.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/BDMLtools.egg-info/PKG-INFO` & `BDMLtools-0.3.8/BDMLtools.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: BDMLtools
-Version: 0.3.7
+Version: 0.3.8
 Summary: Ml learning tools for busniess data mining
 Author: 曾珂
 Author-email: zengke403@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
 
-# BDMLtools-0.3.7
+# BDMLtools
 
 [![PyPI version](https://img.shields.io/pypi/pyversions/BDMLtools.svg)](https://pypi.python.org/pypi/BDMLtools)
 [![License](https://img.shields.io/github/license/zk403/mlearn)](https://github.com/zk403/mlearn/blob/main/LICENSE)
 [![Build Status](https://github.com/zk403/mlearn/actions/workflows/python-test.yml/badge.svg)](https://github.com/zk403/mlearn/actions/workflows/python-test.yml)
 [![codecov](https://codecov.io/gh/zk403/mlearn/main/graphs/badge.svg)](https://app.codecov.io/gh/zk403/mlearn)
 [![PyPI release](https://img.shields.io/pypi/v/BDMLtools.svg)](https://pypi.python.org/pypi/BDMLtools)
 
@@ -44,14 +44,17 @@
 
 ```
 pip uninstall BDMLtools
 ```
 
 更新
 ```
-v0.3.7
-1.新增支持二分类focal loss的损失函数FocalLoss
-2.新增支持二分类focal loss的lightgbm类FLLGBMSklearn
-3.新增支持二分类focal loss下lightgbm的贝叶斯搜索类FLBSTuner
-4.新增支持二分类focal loss下lightgbm的网格搜素、随机搜索类FLgridTuner
-5.更新单元测试脚本,更新部分代码说明
+v0.3.8
+1.报告模块中加入auc指标，加入参数show_metrics以控制auc、ks、lift的输出
+2.修复了binAdjuster中组变量加入breaks_list时导致终止的bug
+3.binSelector中将不再输出ks
+4.调整FLLGBMSklearn中与梯度、正则相关的树参数的默认范围，避免产生决策树无法生长的问题
+5.其他bug修复
+6.更新部分依赖库的版本
+7.更新单元测试脚本,更新部分代码说明
+8.更新example
 ```
```

### Comparing `BDMLtools-0.3.7/BDMLtools.egg-info/SOURCES.txt` & `BDMLtools-0.3.8/BDMLtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/LICENSE` & `BDMLtools-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/PKG-INFO` & `BDMLtools-0.3.8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: BDMLtools
-Version: 0.3.7
+Version: 0.3.8
 Summary: Ml learning tools for busniess data mining
 Author: 曾珂
 Author-email: zengke403@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
 
-# BDMLtools-0.3.7
+# BDMLtools
 
 [![PyPI version](https://img.shields.io/pypi/pyversions/BDMLtools.svg)](https://pypi.python.org/pypi/BDMLtools)
 [![License](https://img.shields.io/github/license/zk403/mlearn)](https://github.com/zk403/mlearn/blob/main/LICENSE)
 [![Build Status](https://github.com/zk403/mlearn/actions/workflows/python-test.yml/badge.svg)](https://github.com/zk403/mlearn/actions/workflows/python-test.yml)
 [![codecov](https://codecov.io/gh/zk403/mlearn/main/graphs/badge.svg)](https://app.codecov.io/gh/zk403/mlearn)
 [![PyPI release](https://img.shields.io/pypi/v/BDMLtools.svg)](https://pypi.python.org/pypi/BDMLtools)
 
@@ -44,14 +44,17 @@
 
 ```
 pip uninstall BDMLtools
 ```
 
 更新
 ```
-v0.3.7
-1.新增支持二分类focal loss的损失函数FocalLoss
-2.新增支持二分类focal loss的lightgbm类FLLGBMSklearn
-3.新增支持二分类focal loss下lightgbm的贝叶斯搜索类FLBSTuner
-4.新增支持二分类focal loss下lightgbm的网格搜素、随机搜索类FLgridTuner
-5.更新单元测试脚本,更新部分代码说明
+v0.3.8
+1.报告模块中加入auc指标，加入参数show_metrics以控制auc、ks、lift的输出
+2.修复了binAdjuster中组变量加入breaks_list时导致终止的bug
+3.binSelector中将不再输出ks
+4.调整FLLGBMSklearn中与梯度、正则相关的树参数的默认范围，避免产生决策树无法生长的问题
+5.其他bug修复
+6.更新部分依赖库的版本
+7.更新单元测试脚本,更新部分代码说明
+8.更新example
 ```
```

### Comparing `BDMLtools-0.3.7/README.md` & `BDMLtools-0.3.8/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# BDMLtools-0.3.7
+# BDMLtools
 
 [![PyPI version](https://img.shields.io/pypi/pyversions/BDMLtools.svg)](https://pypi.python.org/pypi/BDMLtools)
 [![License](https://img.shields.io/github/license/zk403/mlearn)](https://github.com/zk403/mlearn/blob/main/LICENSE)
 [![Build Status](https://github.com/zk403/mlearn/actions/workflows/python-test.yml/badge.svg)](https://github.com/zk403/mlearn/actions/workflows/python-test.yml)
 [![codecov](https://codecov.io/gh/zk403/mlearn/main/graphs/badge.svg)](https://app.codecov.io/gh/zk403/mlearn)
 [![PyPI release](https://img.shields.io/pypi/v/BDMLtools.svg)](https://pypi.python.org/pypi/BDMLtools)
 
@@ -28,14 +28,17 @@
 
 ```
 pip uninstall BDMLtools
 ```
 
 更新
 ```
-v0.3.7
-1.新增支持二分类focal loss的损失函数FocalLoss
-2.新增支持二分类focal loss的lightgbm类FLLGBMSklearn
-3.新增支持二分类focal loss下lightgbm的贝叶斯搜索类FLBSTuner
-4.新增支持二分类focal loss下lightgbm的网格搜素、随机搜索类FLgridTuner
-5.更新单元测试脚本,更新部分代码说明
+v0.3.8
+1.报告模块中加入auc指标，加入参数show_metrics以控制auc、ks、lift的输出
+2.修复了binAdjuster中组变量加入breaks_list时导致终止的bug
+3.binSelector中将不再输出ks
+4.调整FLLGBMSklearn中与梯度、正则相关的树参数的默认范围，避免产生决策树无法生长的问题
+5.其他bug修复
+6.更新部分依赖库的版本
+7.更新单元测试脚本,更新部分代码说明
+8.更新example
 ```
```

### Comparing `BDMLtools-0.3.7/setup.py` & `BDMLtools-0.3.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,39 +11,55 @@
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 # To use a consistent encoding
 from codecs import open
 from os import path
 import re
+import sys
+import platform
 
-base_pkgs=[       'numpy>=1.18,<=1.23.5',#https://github.com/numpy/numpy
+def system():
+    """
+    Returns the system os as a string. e.g.: "darwin"
+    """
+    return platform.system().lower()
+
+
+def python_ver():
+    """
+    Returns the python version as a string. e.g.: "3.8"
+    """
+    return str(sys.version_info.major) + "." + str(sys.version_info.minor)
+
+
+base_pkgs=[       #'numpy>=1.18,<=1.23.5',#https://github.com/numpy/numpy
                   #'matplotlib>=3.5.0,<=3.5.3',
                   #'lofo-importance>=0.3.1',#https://github.com/aerdem4/lofo-importance
                   'fastparquet>=0.7.1',#https://github.com/dask/fastparquet
                   'pandas>=1.3.5',#https://github.com/pandas-dev/pandas
                   #'statsmodels>=0.13.2',#https://github.com/statsmodels/statsmodels
                   'plotnine>=0.10.1',#https://github.com/has2k1/plotnine
                   'scikit-learn>=1.0.2',#https://github.com/scikit-learn/scikit-learn
                   'category_encoders>=2.3.0',#https://github.com/scikit-learn-contrib/category_encoders
                   'lightgbm>=3.3.0',#https://github.com/microsoft/LightGBM 
-                  'probatus>=1.8.9',#https://github.com/ing-bank/probatus
+                  'probatus>=2.0.0',#https://github.com/ing-bank/probatus
                   'mlxtend>=0.19.0',#https://github.com/rasbt/mlxtend
                   'scikit-optimize>=0.9.0',#https://github.com/scikit-optimize/scikit-optimize
                   'openpyxl'
                  ]
 
 dev_dep = [
     "pytest>=6.0.0",
     "pytest-cov>=2.10.0",
     "IPython",
     "mock",
     #'shap>=0.41.0',
-    'xgboost>=1.4.2',#https://github.com/dmlc/xgboost
-    'catboost>=1.0.4,<1.2',#https://github.com/catboost/catboost gituhb action failed in macox
+    'xgboost>=1.5.0',#https://github.com/dmlc/xgboost
+    "catboost>=1.1,<1.2" if python_ver() == "3.8" and system() == "darwin" else "catboost>=1.1" #https://github.com/catboost/catboost gituhb action failed in macox
 ]
 
 here = path.abspath(path.dirname(__file__))
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
```

### Comparing `BDMLtools-0.3.7/test/test_base.py` & `BDMLtools-0.3.8/test/test_base.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/test/test_clearner.py` & `BDMLtools-0.3.8/test/test_clearner.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/test/test_eval.py` & `BDMLtools-0.3.8/test/test_eval.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/test/test_report.py` & `BDMLtools-0.3.8/test/test_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,20 +99,20 @@
         res=varGroupsReport({'a':[1],'c':['1','2','3']},sample_weight=ws,columns=['g'],target='y',n_jobs=1).fit(X)
         res=varGroupsReport({'a':[1],'c':['1','2','3']},columns=['g'],row_limit=1,target='y',n_jobs=1).fit(X)
         res=varGroupsReport({'a':[1],'c':['1','2','3']},columns=['g'],sort_columns={'g':['g1','g2']},target='y',n_jobs=1).fit(X)   
         res=varGroupsReport({'a':[1],'c':['1','2','3']},out_path='tmp',columns=['g'],target='y',n_jobs=1).fit(X)
         
         assert hasattr(res,'report_dict')
         assert not len(set(res.report_dict.keys())-set(['report_all','report_brief','report_count',
-                                                        'report_badprob','report_iv','report_ks','report_lift']))
+                                                        'report_badprob','report_iv','report_ks','report_lift','report_auc']))
                  
         res=varGroupsReport({'a':[1],'c':['1','2','3']},columns=['g'],output_psi=True,target='y',n_jobs=1).fit(X)
         assert hasattr(res,'report_dict')
         assert not len(set(res.report_dict.keys())-set(['report_all','report_brief','report_count',
-                                                        'report_badprob','report_iv','report_ks','report_psi','report_lift']))
+                                                        'report_badprob','report_iv','report_ks','report_psi','report_lift','report_auc']))
         
         varGroupsPlot({'a':[1],'c':['1','2','3']},column='g',target='y',n_jobs=1).plot(X)
         varGroupsPlot({'a':[1],'c':['1','2','3']},column='g',sort_column=['g1','g2'],target='y',n_jobs=1).plot(X)
         
 
 def test_GainsTable():
```

### Comparing `BDMLtools-0.3.7/test/test_selector.py` & `BDMLtools-0.3.8/test/test_selector.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.7/test/test_tunner.py` & `BDMLtools-0.3.8/test/test_tunner.py`

 * *Files identical despite different names*

