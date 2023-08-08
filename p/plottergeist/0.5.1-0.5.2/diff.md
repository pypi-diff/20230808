# Comparing `tmp/plottergeist-0.5.1.tar.gz` & `tmp/plottergeist-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plottergeist-0.5.1.tar", last modified: Tue Aug  8 16:07:31 2023, max compression
+gzip compressed data, was "dist/plottergeist-0.5.2.tar", last modified: Tue Aug  8 16:10:36 2023, max compression
```

## Comparing `plottergeist-0.5.1.tar` & `plottergeist-0.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 apereiro   (501) staff       (20)        0 2023-08-08 16:07:31.569992 plottergeist-0.5.1/
--rw-r--r--   0 apereiro   (501) staff       (20)     1066 2023-07-06 15:44:15.000000 plottergeist-0.5.1/LICENSE
--rw-r--r--   0 apereiro   (501) staff       (20)      713 2023-08-08 16:07:31.569853 plottergeist-0.5.1/PKG-INFO
--rw-r--r--   0 apereiro   (501) staff       (20)      329 2023-07-10 14:41:16.000000 plottergeist-0.5.1/README.md
-drwxr-xr-x   0 apereiro   (501) staff       (20)        0 2023-08-08 16:07:31.567447 plottergeist-0.5.1/plottergeist/
--rw-r--r--   0 apereiro   (501) staff       (20)      140 2023-07-10 14:49:21.000000 plottergeist-0.5.1/plottergeist/__init__.py
--rw-r--r--   0 apereiro   (501) staff       (20)    13337 2023-07-11 11:00:32.000000 plottergeist-0.5.1/plottergeist/fig_creator.py
--rw-r--r--   0 apereiro   (501) staff       (20)     2029 2023-07-09 10:54:33.000000 plottergeist-0.5.1/plottergeist/histogram.py
--rw-r--r--   0 apereiro   (501) staff       (20)     1898 2023-08-08 16:06:53.000000 plottergeist-0.5.1/plottergeist/residuals.py
--rw-r--r--   0 apereiro   (501) staff       (20)    36435 2023-07-11 10:33:05.000000 plottergeist-0.5.1/plottergeist/style.py
-drwxr-xr-x   0 apereiro   (501) staff       (20)        0 2023-08-08 16:07:31.568776 plottergeist-0.5.1/plottergeist.egg-info/
--rw-r--r--   0 apereiro   (501) staff       (20)      713 2023-08-08 16:07:31.000000 plottergeist-0.5.1/plottergeist.egg-info/PKG-INFO
--rw-r--r--   0 apereiro   (501) staff       (20)      397 2023-08-08 16:07:31.000000 plottergeist-0.5.1/plottergeist.egg-info/SOURCES.txt
--rw-r--r--   0 apereiro   (501) staff       (20)        1 2023-08-08 16:07:31.000000 plottergeist-0.5.1/plottergeist.egg-info/dependency_links.txt
--rw-r--r--   0 apereiro   (501) staff       (20)       23 2023-08-08 16:07:31.000000 plottergeist-0.5.1/plottergeist.egg-info/requires.txt
--rw-r--r--   0 apereiro   (501) staff       (20)       13 2023-08-08 16:07:31.000000 plottergeist-0.5.1/plottergeist.egg-info/top_level.txt
--rw-r--r--   0 apereiro   (501) staff       (20)       38 2023-08-08 16:07:31.570047 plottergeist-0.5.1/setup.cfg
--rw-r--r--   0 apereiro   (501) staff       (20)      921 2023-07-10 14:41:16.000000 plottergeist-0.5.1/setup.py
-drwxr-xr-x   0 apereiro   (501) staff       (20)        0 2023-08-08 16:07:31.569510 plottergeist-0.5.1/test/
--rw-r--r--   0 apereiro   (501) staff       (20)      450 2023-07-09 11:49:36.000000 plottergeist-0.5.1/test/test_histogram.py
--rw-r--r--   0 apereiro   (501) staff       (20)     4047 2023-07-11 15:07:52.000000 plottergeist-0.5.1/test/test_plot_1D.py
--rw-r--r--   0 apereiro   (501) staff       (20)     2660 2023-07-11 10:18:24.000000 plottergeist-0.5.1/test/test_plot_3D.py
+drwxr-xr-x   0 apereiro   (501) staff       (20)        0 2023-08-08 16:10:36.326253 plottergeist-0.5.2/
+-rw-r--r--   0 apereiro   (501) staff       (20)     1066 2023-07-06 15:44:15.000000 plottergeist-0.5.2/LICENSE
+-rw-r--r--   0 apereiro   (501) staff       (20)      713 2023-08-08 16:10:36.326127 plottergeist-0.5.2/PKG-INFO
+-rw-r--r--   0 apereiro   (501) staff       (20)      329 2023-07-10 14:41:16.000000 plottergeist-0.5.2/README.md
+drwxr-xr-x   0 apereiro   (501) staff       (20)        0 2023-08-08 16:10:36.323667 plottergeist-0.5.2/plottergeist/
+-rw-r--r--   0 apereiro   (501) staff       (20)      140 2023-07-10 14:49:21.000000 plottergeist-0.5.2/plottergeist/__init__.py
+-rw-r--r--   0 apereiro   (501) staff       (20)    13337 2023-07-11 11:00:32.000000 plottergeist-0.5.2/plottergeist/fig_creator.py
+-rw-r--r--   0 apereiro   (501) staff       (20)     2029 2023-07-09 10:54:33.000000 plottergeist-0.5.2/plottergeist/histogram.py
+-rw-r--r--   0 apereiro   (501) staff       (20)     1981 2023-08-08 16:10:10.000000 plottergeist-0.5.2/plottergeist/residuals.py
+-rw-r--r--   0 apereiro   (501) staff       (20)    36435 2023-07-11 10:33:05.000000 plottergeist-0.5.2/plottergeist/style.py
+drwxr-xr-x   0 apereiro   (501) staff       (20)        0 2023-08-08 16:10:36.325050 plottergeist-0.5.2/plottergeist.egg-info/
+-rw-r--r--   0 apereiro   (501) staff       (20)      713 2023-08-08 16:10:36.000000 plottergeist-0.5.2/plottergeist.egg-info/PKG-INFO
+-rw-r--r--   0 apereiro   (501) staff       (20)      397 2023-08-08 16:10:36.000000 plottergeist-0.5.2/plottergeist.egg-info/SOURCES.txt
+-rw-r--r--   0 apereiro   (501) staff       (20)        1 2023-08-08 16:10:36.000000 plottergeist-0.5.2/plottergeist.egg-info/dependency_links.txt
+-rw-r--r--   0 apereiro   (501) staff       (20)       23 2023-08-08 16:10:36.000000 plottergeist-0.5.2/plottergeist.egg-info/requires.txt
+-rw-r--r--   0 apereiro   (501) staff       (20)       13 2023-08-08 16:10:36.000000 plottergeist-0.5.2/plottergeist.egg-info/top_level.txt
+-rw-r--r--   0 apereiro   (501) staff       (20)       38 2023-08-08 16:10:36.326301 plottergeist-0.5.2/setup.cfg
+-rw-r--r--   0 apereiro   (501) staff       (20)      921 2023-07-10 14:41:16.000000 plottergeist-0.5.2/setup.py
+drwxr-xr-x   0 apereiro   (501) staff       (20)        0 2023-08-08 16:10:36.325795 plottergeist-0.5.2/test/
+-rw-r--r--   0 apereiro   (501) staff       (20)      450 2023-07-09 11:49:36.000000 plottergeist-0.5.2/test/test_histogram.py
+-rw-r--r--   0 apereiro   (501) staff       (20)     4047 2023-07-11 15:07:52.000000 plottergeist-0.5.2/test/test_plot_1D.py
+-rw-r--r--   0 apereiro   (501) staff       (20)     2660 2023-07-11 10:18:24.000000 plottergeist-0.5.2/test/test_plot_3D.py
```

### Comparing `plottergeist-0.5.1/LICENSE` & `plottergeist-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plottergeist-0.5.1/PKG-INFO` & `plottergeist-0.5.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plottergeist
-Version: 0.5.1
+Version: 0.5.2
 Summary: Statistics and scientific plotting
 Home-page: https://github.com/apereiroc/plottergeist
 Download-URL: https://github.com/apereiroc/plottergeist.git
 Author: Asier Pereiro Castro
 Author-email: asier.pereiro.castro@cern.ch
 License: MIT
 Requires-Python: >=3.7
```

### Comparing `plottergeist-0.5.1/plottergeist/fig_creator.py` & `plottergeist-0.5.2/plottergeist/fig_creator.py`

 * *Files identical despite different names*

### Comparing `plottergeist-0.5.1/plottergeist/histogram.py` & `plottergeist-0.5.2/plottergeist/histogram.py`

 * *Files identical despite different names*

### Comparing `plottergeist-0.5.1/plottergeist/residuals.py` & `plottergeist-0.5.2/plottergeist/residuals.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   density
   """
   _data = make_hist(data, weights=data_weights, density=density, bins=bins,
                     *args, **kwargs)
   _fit = make_hist(fit, weights=fit_weights, density=density, bins=_data.edges, *args,
                  **kwargs)
 
-  assert _fit.norm != 0.0
+  assert _fit.norm != 0.0, f"The integral of the histogram of the PDF is 0. Check the values: {_fit.counts}"
 
   _data_norm = 1.0
   # _fit_norm = 1.0
   _fit_norm = _data.norm/_fit.norm
 
   # if scale_fit:
   #   _fit_norm *= _data.norm / _fit.norm
```

### Comparing `plottergeist-0.5.1/plottergeist/style.py` & `plottergeist-0.5.2/plottergeist/style.py`

 * *Files identical despite different names*

### Comparing `plottergeist-0.5.1/plottergeist.egg-info/PKG-INFO` & `plottergeist-0.5.2/plottergeist.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plottergeist
-Version: 0.5.1
+Version: 0.5.2
 Summary: Statistics and scientific plotting
 Home-page: https://github.com/apereiroc/plottergeist
 Download-URL: https://github.com/apereiroc/plottergeist.git
 Author: Asier Pereiro Castro
 Author-email: asier.pereiro.castro@cern.ch
 License: MIT
 Requires-Python: >=3.7
```

### Comparing `plottergeist-0.5.1/setup.py` & `plottergeist-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `plottergeist-0.5.1/test/test_plot_1D.py` & `plottergeist-0.5.2/test/test_plot_1D.py`

 * *Files identical despite different names*

### Comparing `plottergeist-0.5.1/test/test_plot_3D.py` & `plottergeist-0.5.2/test/test_plot_3D.py`

 * *Files identical despite different names*

