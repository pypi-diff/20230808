# Comparing `tmp/asalix-0.1.0.tar.gz` & `tmp/asalix-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asalix-0.1.0.tar", last modified: Tue Aug  8 11:06:05 2023, max compression
+gzip compressed data, was "asalix-0.1.1.tar", last modified: Tue Aug  8 11:11:32 2023, max compression
```

## Comparing `asalix-0.1.0.tar` & `asalix-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 11:06:05.166557 asalix-0.1.0/
--rw-rw-rw-   0        0        0    35823 2023-07-25 08:45:32.000000 asalix-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      714 2023-08-08 11:06:05.166557 asalix-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6599 2023-08-08 11:04:04.000000 asalix-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-08 11:06:05.166557 asalix-0.1.0/asalix/
--rw-rw-rw-   0        0        0    14386 2023-08-08 10:53:37.000000 asalix-0.1.0/asalix/__init__.py
--rw-rw-rw-   0        0        0     4656 2023-07-26 06:32:54.000000 asalix-0.1.0/asalix/dataset_extractor.py
--rw-rw-rw-   0        0        0    12926 2023-07-27 13:17:19.000000 asalix-0.1.0/asalix/numerical_methods.py
--rw-rw-rw-   0        0        0    14070 2023-08-08 07:36:14.000000 asalix-0.1.0/asalix/plotter.py
-drwxrwxrwx   0        0        0        0 2023-08-08 11:06:05.166557 asalix-0.1.0/asalix.egg-info/
--rw-rw-rw-   0        0        0      714 2023-08-08 11:06:05.000000 asalix-0.1.0/asalix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-08-08 11:06:05.000000 asalix-0.1.0/asalix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 11:06:05.000000 asalix-0.1.0/asalix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      156 2023-08-08 11:06:05.000000 asalix-0.1.0/asalix.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-08 11:06:05.000000 asalix-0.1.0/asalix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-08 11:06:05.166557 asalix-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1184 2023-08-08 10:59:59.000000 asalix-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 11:11:32.006395 asalix-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-25 08:45:32.000000 asalix-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     7368 2023-08-08 11:11:32.006395 asalix-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6620 2023-08-08 11:06:48.000000 asalix-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 11:11:32.006395 asalix-0.1.1/asalix/
+-rw-rw-rw-   0        0        0    14386 2023-08-08 11:08:47.000000 asalix-0.1.1/asalix/__init__.py
+-rw-rw-rw-   0        0        0     4656 2023-07-26 06:32:54.000000 asalix-0.1.1/asalix/dataset_extractor.py
+-rw-rw-rw-   0        0        0    12926 2023-07-27 13:17:19.000000 asalix-0.1.1/asalix/numerical_methods.py
+-rw-rw-rw-   0        0        0    14070 2023-08-08 07:36:14.000000 asalix-0.1.1/asalix/plotter.py
+drwxrwxrwx   0        0        0        0 2023-08-08 11:11:32.006395 asalix-0.1.1/asalix.egg-info/
+-rw-rw-rw-   0        0        0     7368 2023-08-08 11:11:31.000000 asalix-0.1.1/asalix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-08-08 11:11:31.000000 asalix-0.1.1/asalix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 11:11:31.000000 asalix-0.1.1/asalix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      156 2023-08-08 11:11:31.000000 asalix-0.1.1/asalix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-08 11:11:31.000000 asalix-0.1.1/asalix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 11:11:32.006395 asalix-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1923 2023-08-08 11:11:03.000000 asalix-0.1.1/setup.py
```

### Comparing `asalix-0.1.0/LICENSE` & `asalix-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asalix-0.1.0/README.md` & `asalix-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 print("\n95% confidence internval")
 print("\u03C3 known:  ", ax.calculate_confidence_interval(dataset, 0.95, population=True))
 print("\u03C3 unknown:", ax.calculate_confidence_interval(dataset, 0.95, population=False))
 ```
 
 
 ## 3. For developers
-To upload a new version of **ASALIX** on [PyPi](https://pypi.org/):
+To upload a new version of **ASALIX** on [PyPi](https://pypi.org/project/asalix/0.1.0/):
 ```bash
 pip install --upgrade .
 python example.py
 python setup.py check
 python setup.py sdist
 twine upload dist/*
 ```
```

#### html2text {}

```diff
@@ -67,9 +67,9 @@
 and not normal data dataset = ax.extract_dataset(pd.DataFrame(
 {"normal_dataset": np.random.normal(100, 20, 20), "not_normal_dataset": list
 (range(1, 21))}), data_column_name="normal_dataset") # Print the confidence
 interval on screen print("\n95% confidence internval") print("\u03C3 known: ",
 ax.calculate_confidence_interval(dataset, 0.95, population=True)) print("\u03C3
 unknown:", ax.calculate_confidence_interval(dataset, 0.95, population=False))
 ``` ## 3. For developers To upload a new version of **ASALIX** on [PyPi](https:
-//pypi.org/): ```bash pip install --upgrade . python example.py python setup.py
-check python setup.py sdist twine upload dist/* ```
+//pypi.org/project/asalix/0.1.0/): ```bash pip install --upgrade . python
+example.py python setup.py check python setup.py sdist twine upload dist/* ```
```

### Comparing `asalix-0.1.0/asalix/__init__.py` & `asalix-0.1.1/asalix/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 asalix
 
 A comprehensive collection of mathematical tools and utilities designed to support Lean Six Sigma practitioners in their process improvement journey.
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __author__ = 'Stefano Rebughini'
 
 
 from asalix.dataset_extractor import DatasetExtractor
 from asalix.numerical_methods import NumericalMethods
 from asalix.plotter import Plotter
 from types import SimpleNamespace
```

### Comparing `asalix-0.1.0/asalix/dataset_extractor.py` & `asalix-0.1.1/asalix/dataset_extractor.py`

 * *Files identical despite different names*

### Comparing `asalix-0.1.0/asalix/numerical_methods.py` & `asalix-0.1.1/asalix/numerical_methods.py`

 * *Files identical despite different names*

### Comparing `asalix-0.1.0/asalix/plotter.py` & `asalix-0.1.1/asalix/plotter.py`

 * *Files identical despite different names*

