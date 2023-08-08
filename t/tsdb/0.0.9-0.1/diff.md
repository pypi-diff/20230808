# Comparing `tmp/tsdb-0.0.9.tar.gz` & `tmp/tsdb-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsdb-0.0.9.tar", last modified: Mon Jul 10 16:48:21 2023, max compression
+gzip compressed data, was "tsdb-0.1.tar", last modified: Tue Aug  8 13:39:56 2023, max compression
```

## Comparing `tsdb-0.0.9.tar` & `tsdb-0.1.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:48:21.903931 tsdb-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-10 16:48:07.000000 tsdb-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-10 16:48:21.903931 tsdb-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-10 16:48:07.000000 tsdb-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-10 16:48:21.903931 tsdb-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-10 16:48:07.000000 tsdb-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:48:21.899931 tsdb-0.0.9/tsdb/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:48:21.903931 tsdb-0.0.9/tsdb/data_loading_funcs/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/data_loading_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/data_loading_funcs/beijing_multisite_air_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/data_loading_funcs/electricity_load_diagrams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/data_loading_funcs/physionet_2012.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/data_loading_funcs/physionet_2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/data_loading_funcs/ucr_uea_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/data_loading_funcs/vessel_ais.py
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:48:21.903931 tsdb-0.0.9/tsdb/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-10 16:48:07.000000 tsdb-0.0.9/tsdb/tests/test_tsdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:48:21.899931 tsdb-0.0.9/tsdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-10 16:48:21.000000 tsdb-0.0.9/tsdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-10 16:48:21.000000 tsdb-0.0.9/tsdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:48:21.000000 tsdb-0.0.9/tsdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 16:48:21.000000 tsdb-0.0.9/tsdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 16:48:21.000000 tsdb-0.0.9/tsdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:39:56.188747 tsdb-0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-08-08 13:39:43.000000 tsdb-0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 13:39:43.000000 tsdb-0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-08-08 13:39:56.188747 tsdb-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-08-08 13:39:43.000000 tsdb-0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-08 13:39:56.188747 tsdb-0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-08-08 13:39:43.000000 tsdb-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:39:56.184747 tsdb-0.1/tsdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-08 13:39:43.000000 tsdb-0.1/tsdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-08-08 13:39:43.000000 tsdb-0.1/tsdb/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-08-08 13:39:43.000000 tsdb-0.1/tsdb/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:39:56.184747 tsdb-0.1/tsdb/loading_funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-08 13:39:43.000000 tsdb-0.1/tsdb/loading_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-08 13:39:43.000000 tsdb-0.1/tsdb/loading_funcs/beijing_multisite_air_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-08 13:39:43.000000 tsdb-0.1/tsdb/loading_funcs/electricity_load_diagrams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-08-08 13:39:43.000000 tsdb-0.1/tsdb/loading_funcs/physionet_2012.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-08-08 13:39:43.000000 tsdb-0.1/tsdb/loading_funcs/physionet_2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-08-08 13:39:43.000000 tsdb-0.1/tsdb/loading_funcs/ucr_uea_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-08-08 13:39:43.000000 tsdb-0.1/tsdb/loading_funcs/vessel_ais.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:39:56.188747 tsdb-0.1/tsdb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-08 13:39:43.000000 tsdb-0.1/tsdb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-08-08 13:39:43.000000 tsdb-0.1/tsdb/utils/downloading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-08 13:39:43.000000 tsdb-0.1/tsdb/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-08 13:39:43.000000 tsdb-0.1/tsdb/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:39:56.184747 tsdb-0.1/tsdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-08-08 13:39:56.000000 tsdb-0.1/tsdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-08 13:39:56.000000 tsdb-0.1/tsdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:39:56.000000 tsdb-0.1/tsdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-08 13:39:56.000000 tsdb-0.1/tsdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 13:39:56.000000 tsdb-0.1/tsdb.egg-info/top_level.txt
```

### Comparing `tsdb-0.0.9/LICENSE` & `tsdb-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsdb-0.0.9/PKG-INFO` & `tsdb-0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,81 +1,86 @@
 Metadata-Version: 2.1
 Name: tsdb
-Version: 0.0.9
+Version: 0.1
 Summary: TSDB (Time-Series DataBase): A Python Toolbox Helping Load Open-Source Time-Series Datasets
 Home-page: https://github.com/WenjieDu/TSDB
 Author: Wenjie Du
 Author-email: wenjay.du@gmail.com
 License: GPL-3.0
 Project-URL: Documentation, https://tsdb.readthedocs.io/
 Project-URL: Source, https://github.com/WenjieDu/TSDB/
 Project-URL: Tracker, https://github.com/WenjieDu/TSDB/issues/
 Project-URL: Download, https://github.com/WenjieDu/TSDB/archive/main.zip
-Keywords: time-series analysis,time series,time-series database,time-series datasets,datasets,database,dataset downloading,data mining
+Keywords: data mining,time series,time-series analysis,time-series database,time-series datasets,database,datasets,dataset downloading,imputation,classification,forecasting
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database
 Description-Content-Type: text/markdown
 Provides-Extra: basic
 License-File: LICENSE
 
-<a href='https://github.com/WenjieDu/TSDB'><img src="https://raw.githubusercontent.com/WenjieDu/TSDB/main/docs/_static/figs/TSDB_logo.svg?sanitize=true" align='right' width='235'/></a>
+<a href='https://github.com/WenjieDu/TSDB'><img src="https://raw.githubusercontent.com/PyPOTS/pypots.github.io/main/static/figs/pypots_logos/TSDB_logo_FFBG.svg?sanitize=truee" align='right' width='235'/></a>
 
 # <p align='center'>Welcome to TSDB</p>
 **<p align='center'>A Python Toolbox to Ease Loading Open-Source Time-Series Datasets</p>**
 
 <p align='center'>
     <!-- Python version -->
     <img src='https://img.shields.io/badge/python-v3-E97040?logo=python&logoColor=white'>
     <!-- PyPI version -->
-    <img alt="PyPI" src="https://img.shields.io/pypi/v/tsdb?color=green&label=PyPI&logo=pypi&logoColor=white">
+    <a href="https://pypi.python.org/pypi/tsdb">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/tsdb?color=green&label=PyPI&logo=pypi&logoColor=white">
+    </a>
     <!-- License -->
     <a href="https://github.com/WenjieDu/TSDB/blob/main/LICENSE">
         <img alt="GPL-v3 license" src="https://img.shields.io/badge/License-GPL--v3-E9BB41">
     </a>
     <!-- GitHub Testing -->
-    <a alt='GitHub Testing' href='https://github.com/WenjieDu/TSDB/actions/workflows/testing.yml'> 
+    <a alt='GitHub Testing' href='https://github.com/WenjieDu/TSDB/actions/workflows/testing_ci.yml'>
         <img src='https://img.shields.io/github/actions/workflow/status/wenjiedu/tsdb/testing_ci.yml?logo=github&color=C8D8E1&label=CI'>
     </a>
     <a href="https://codeclimate.com/github/WenjieDu/TSDB">
         <img alt="Code Climate maintainability" src="https://img.shields.io/codeclimate/maintainability-percentage/WenjieDu/TSDB?color=3C7699&label=Maintainability&logo=codeclimate">
     </a>
     <!-- Coveralls report -->
-    <a alt='Coveralls report' href='https://coveralls.io/github/WenjieDu/TSDB'> 
+    <a alt='Coveralls report' href='https://coveralls.io/github/WenjieDu/TSDB'>
         <img src='https://img.shields.io/coverallsCoverage/github/WenjieDu/TSDB?branch=main&logo=coveralls&color=75C1C4&label=Coverage'>
     </a>
     <a href="https://anaconda.org/conda-forge/tsdb">
         <img alt="Conda downloads" src="https://img.shields.io/conda/dn/conda-forge/tsdb?label=Conda%20Downloads&color=AED0ED&logo=anaconda&logoColor=white">
     </a>
     <!-- PyPI download number -->
     <a alt='PyPI download number' href='https://pypi.org/project/tsdb'>
         <img src='https://static.pepy.tech/personalized-badge/tsdb?period=total&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20Downloads'>
     </a>
 </p>
 
-> 📣 TSDB now supports a total of 1️⃣6️⃣5️⃣ time-series datasets ‼️
+> 📣 TSDB now supports a total of 1️⃣6️⃣8️⃣ time-series datasets ‼️
+
+<a href='https://github.com/WenjieDu/PyPOTS'><img src='https://raw.githubusercontent.com/PyPOTS/pypots.github.io/main/static/figs/pypots_logos/PyPOTS_logo_FFBG.svg?sanitize=true' width='160' align='left' /></a>
+TSDB is a part of [PyPOTS project](https://github.com/WenjieDu/PyPOTS) (a Python toolbox for data mining on Partially-Observed Time Series), and was separated from PyPOTS for decoupling datasets from learning algorithms.
 
 TSDB is created to help researchers and engineers get rid of data collecting and downloading, and focus back on data processing details. TSDB provides all-in-one-stop convenience for downloading and loading open-source time-series datasets (available datasets listed [below](https://github.com/WenjieDu/TSDB#-list-of-available-datasets)).
 
 ❗️Please note that due to people have very different requirements for data processing, data-loading functions in TSDB only contain the most general steps (e.g. removing invalid samples) and won't process the data (not even normalize it). So, no worries, TSDB won't affect your data preprocessing. If you only want the raw datasets, TSDB can help you download and save raw datasets as well (take a look at [Usage Examples](https://github.com/WenjieDu/TSDB#-usage-example) below).
 
 🤝 If you need TSDB to integrate an open-source dataset or want to add it into TSDB yourself, please feel free to request for it by creating an issue or make a PR to merge your code.
 
 🤗 **Please** star this repo to help others notice TSDB if you think it is a useful toolkit.
 **Please** properly [cite TSDB](https://github.com/WenjieDu/TSDB#-citing-tsdbpypots) in your publications
 if it helps with your research. This really means a lot to our open-source research. Thank you!
 
 
 ## ❖ Usage Examples
-TSDB now is available on <a alt='Anaconda' href='https://anaconda.org/conda-forge/tsdb'><img align='center' src='https://img.shields.io/badge/Anaconda--lightgreen?style=social&logo=anaconda'></a>❗️ 
+TSDB now is available on <a alt='Anaconda' href='https://anaconda.org/conda-forge/tsdb'><img align='center' src='https://img.shields.io/badge/Anaconda--lightgreen?style=social&logo=anaconda'></a>❗️
 
 Install it with `conda install tsdb`, you may need to specify the channel with option `-c conda-forge`
 
 or install from PyPI:
 > pip install tsdb
 
 or install from source code:
@@ -84,37 +89,34 @@
 ```python
 import tsdb
 
 tsdb.list_available_datasets()  # list all available datasets in TSDB
 data = tsdb.load_dataset('physionet_2012')  # select the dataset you need and load it, TSDB will download, extract, and process it automatically
 tsdb.download_and_extract('physionet_2012', './save_it_here')  # if you need the raw data, use download_and_extract()
 tsdb.list_cached_data()  # datasets you once loaded are cached, and you can check them with list_cached_data()
-tsdb.delete_cached_data()  # you can delete all cache with delete_cached_data() to free disk space
-tsdb.delete_cached_data(dataset_name='physionet_2012')  # or you can delete only one specific dataset and preserve others
+tsdb.delete_cached_data(dataset_name='physionet_2012')  # you can delete only one specific dataset and preserve others
+tsdb.delete_cached_data()  # or you can delete all cache with delete_cached_data() to free disk space
 ```
 
 That's all. Simple and efficient. Enjoy it! 😃
 
 
 ## ❖ List of Available Datasets
 
-| Name                                                                  | Main Tasks                              |
-|-----------------------------------------------------------------------|-----------------------------------------|
-| [PhysioNet Challenge 2012](datasets/PhysioNet-2012)                   | Classification, Forecasting, Imputation |
-| [PhysioNet Challenge 2019](datasets/PhysioNet-2019)                   | Classification, Imputation              |
-| [Beijing Multi-Site Air-Quality](datasets/BeijingMultiSiteAirQuality) | Forecasting, Imputation                 |
-| [Electricity Load Diagrams](datasets/ElectricityLoadDiagrams)         | Forecasting, Imputation                 |
-| [UCR & UEA Datasets](datasets/UCR_UEA_Datasets) (all 160 datasets)    | Classification                          |
-| [Vessel AIS](datasets/Vessel_AIS)                                     | Classification, Forecasting, Imputation |
+| Name                                                                             | Main Tasks                              |
+|----------------------------------------------------------------------------------|-----------------------------------------|
+| [PhysioNet Challenge 2012](dataset_profiles/physionet_2012)                      | Classification, Forecasting, Imputation |
+| [PhysioNet Challenge 2019](dataset_profiles/physionet_2019)                      | Classification, Imputation              |
+| [Beijing Multi-Site Air-Quality](dataset_profiles/beijing_multisite_air_quality) | Forecasting, Imputation                 |
+| [Electricity Load Diagrams](dataset_profiles/electricity_load_diagrams)          | Forecasting, Imputation                 |
+| [UCR & UEA Datasets](dataset_profiles/ucr_uea_datasets) (all 163 datasets)       | Classification                          |
+| [Vessel AIS](dataset_profiles/vessel_ais)                                        | Classification, Forecasting, Imputation |
 
 
 ## ❖ Citing TSDB/PyPOTS
-<a href='https://github.com/WenjieDu/PyPOTS'><img src='https://raw.githubusercontent.com/WenjieDu/PyPOTS/main/docs/_static/figs/PyPOTS_logo.svg?sanitize=true' width='160' align='left' /></a>
-TSDB is a part of [PyPOTS project](https://github.com/WenjieDu/PyPOTS) (a Python toolbox for data mining on Partially-Observed Time Series), and was separated from PyPOTS for decoupling datasets from learning algorithms.
-
 The paper introducing PyPOTS project is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
 and we are pursuing to publish it in prestigious academic venues, e.g. JMLR (track for
 [Machine Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use TSDB in your work,
 please cite PyPOTS project as below and 🌟star this repository to make others notice this library. 🤗 Thank you!
 
 ``` bibtex
 @article{du2023PyPOTS,
```

#### html2text {}

```diff
@@ -1,88 +1,91 @@
-Metadata-Version: 2.1 Name: tsdb Version: 0.0.9 Summary: TSDB (Time-Series
+Metadata-Version: 2.1 Name: tsdb Version: 0.1 Summary: TSDB (Time-Series
 DataBase): A Python Toolbox Helping Load Open-Source Time-Series Datasets Home-
 page: https://github.com/WenjieDu/TSDB Author: Wenjie Du Author-email:
 wenjay.du@gmail.com License: GPL-3.0 Project-URL: Documentation, https://
 tsdb.readthedocs.io/ Project-URL: Source, https://github.com/WenjieDu/TSDB/
 Project-URL: Tracker, https://github.com/WenjieDu/TSDB/issues/ Project-URL:
-Download, https://github.com/WenjieDu/TSDB/archive/main.zip Keywords: time-
-series analysis,time series,time-series database,time-series
-datasets,datasets,database,dataset downloading,data mining Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Education Classifier: Intended
-Audience :: Science/Research Classifier: License :: OSI Approved :: GNU General
-Public License v3 (GPLv3) Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Topic :: Database
-Description-Content-Type: text/markdown Provides-Extra: basic License-File:
-LICENSE [https://raw.githubusercontent.com/WenjieDu/TSDB/main/docs/_static/
-figs/TSDB_logo.svg?sanitize=true] #
+Download, https://github.com/WenjieDu/TSDB/archive/main.zip Keywords: data
+mining,time series,time-series analysis,time-series database,time-series
+datasets,database,datasets,dataset
+downloading,imputation,classification,forecasting Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: GNU General Public
+License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Topic :: Database Description-
+Content-Type: text/markdown Provides-Extra: basic License-File: LICENSE [https:
+//raw.githubusercontent.com/PyPOTS/pypots.github.io/main/static/figs/
+pypots_logos/TSDB_logo_FFBG.svg?sanitize=truee] #
                                 Welcome to TSDB
 **
        A Python Toolbox to Ease Loading Open-Source Time-Series Datasets
 **
  [https://img.shields.io/badge/python-v3-E97040?logo=python&logoColor=white]
   [PyPI]  [GPL-v3_license]  [https://img.shields.io/github/actions/workflow/
  status/wenjiedu/tsdb/testing_ci.yml?logo=github&color=C8D8E1&label=CI] [Code
   Climate_maintainability]  [https://img.shields.io/coverallsCoverage/github/
  WenjieDu/TSDB?branch=main&logo=coveralls&color=75C1C4&label=Coverage] [Conda
            downloads]  [https://static.pepy.tech/personalized-badge/
 tsdb?period=total&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20Downloads]
-> ð£ TSDB now supports a total of 1ï¸â£6ï¸â£5ï¸â£ time-series datasets
-â¼ï¸ TSDB is created to help researchers and engineers get rid of data
-collecting and downloading, and focus back on data processing details. TSDB
-provides all-in-one-stop convenience for downloading and loading open-source
-time-series datasets (available datasets listed [below](https://github.com/
-WenjieDu/TSDB#-list-of-available-datasets)). âï¸Please note that due to
-people have very different requirements for data processing, data-loading
-functions in TSDB only contain the most general steps (e.g. removing invalid
-samples) and won't process the data (not even normalize it). So, no worries,
-TSDB won't affect your data preprocessing. If you only want the raw datasets,
-TSDB can help you download and save raw datasets as well (take a look at [Usage
-Examples](https://github.com/WenjieDu/TSDB#-usage-example) below). ð¤ If you
-need TSDB to integrate an open-source dataset or want to add it into TSDB
-yourself, please feel free to request for it by creating an issue or make a PR
-to merge your code. ð¤ **Please** star this repo to help others notice TSDB
-if you think it is a useful toolkit. **Please** properly [cite TSDB](https://
-github.com/WenjieDu/TSDB#-citing-tsdbpypots) in your publications if it helps
-with your research. This really means a lot to our open-source research. Thank
-you! ## â Usage Examples TSDB now is available on [https://img.shields.io/
-badge/Anaconda--lightgreen?style=social&logo=anaconda]âï¸ Install it with
-`conda install tsdb`, you may need to specify the channel with option `-
-c conda-forge` or install from PyPI: > pip install tsdb or install from source
-code: > pip install `https://github.com/WenjieDu/TSDB/archive/main.zip`
-```python import tsdb tsdb.list_available_datasets() # list all available
-datasets in TSDB data = tsdb.load_dataset('physionet_2012') # select the
-dataset you need and load it, TSDB will download, extract, and process it
-automatically tsdb.download_and_extract('physionet_2012', './save_it_here') #
-if you need the raw data, use download_and_extract() tsdb.list_cached_data() #
-datasets you once loaded are cached, and you can check them with
-list_cached_data() tsdb.delete_cached_data() # you can delete all cache with
-delete_cached_data() to free disk space tsdb.delete_cached_data
-(dataset_name='physionet_2012') # or you can delete only one specific dataset
-and preserve others ``` That's all. Simple and efficient. Enjoy it! ð ## â
-List of Available Datasets | Name | Main Tasks | |-----------------------------
-------------------------------------------|------------------------------------
------| | [PhysioNet Challenge 2012](datasets/PhysioNet-2012) | Classification,
-Forecasting, Imputation | | [PhysioNet Challenge 2019](datasets/PhysioNet-2019)
-| Classification, Imputation | | [Beijing Multi-Site Air-Quality](datasets/
-BeijingMultiSiteAirQuality) | Forecasting, Imputation | | [Electricity Load
-Diagrams](datasets/ElectricityLoadDiagrams) | Forecasting, Imputation | | [UCR
-& UEA Datasets](datasets/UCR_UEA_Datasets) (all 160 datasets) | Classification
-| | [Vessel AIS](datasets/Vessel_AIS) | Classification, Forecasting, Imputation
-| ## â Citing TSDB/PyPOTS [https://raw.githubusercontent.com/WenjieDu/PyPOTS/
-main/docs/_static/figs/PyPOTS_logo.svg?sanitize=true] TSDB is a part of [PyPOTS
+> ð£ TSDB now supports a total of 1ï¸â£6ï¸â£8ï¸â£ time-series datasets
+â¼ï¸ [https://raw.githubusercontent.com/PyPOTS/pypots.github.io/main/static/
+figs/pypots_logos/PyPOTS_logo_FFBG.svg?sanitize=true] TSDB is a part of [PyPOTS
 project](https://github.com/WenjieDu/PyPOTS) (a Python toolbox for data mining
 on Partially-Observed Time Series), and was separated from PyPOTS for
-decoupling datasets from learning algorithms. The paper introducing PyPOTS
-project is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
-and we are pursuing to publish it in prestigious academic venues, e.g. JMLR
-(track for [Machine Learning Open Source Software](https://www.jmlr.org/mloss/
-)). If you use TSDB in your work, please cite PyPOTS project as below and
-ðstar this repository to make others notice this library. ð¤ Thank you!
-``` bibtex @article{du2023PyPOTS, title={{PyPOTS: A Python Toolbox for Data
-Mining on Partially-Observed Time Series}}, author={Wenjie Du}, year={2023},
-eprint={2305.18811}, archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://
-arxiv.org/abs/2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` or > Wenjie
-Du. (2023). > PyPOTS: A Python Toolbox for Data Mining on Partially-Observed
-Time Series. > arXiv, abs/2305.18811. https://doi.org/10.48550/arXiv.2305.18811
-ð  Visits [https://hits.seeyoufarm.com/api/count/incr/
+decoupling datasets from learning algorithms. TSDB is created to help
+researchers and engineers get rid of data collecting and downloading, and focus
+back on data processing details. TSDB provides all-in-one-stop convenience for
+downloading and loading open-source time-series datasets (available datasets
+listed [below](https://github.com/WenjieDu/TSDB#-list-of-available-datasets)).
+âï¸Please note that due to people have very different requirements for data
+processing, data-loading functions in TSDB only contain the most general steps
+(e.g. removing invalid samples) and won't process the data (not even normalize
+it). So, no worries, TSDB won't affect your data preprocessing. If you only
+want the raw datasets, TSDB can help you download and save raw datasets as well
+(take a look at [Usage Examples](https://github.com/WenjieDu/TSDB#-usage-
+example) below). ð¤ If you need TSDB to integrate an open-source dataset or
+want to add it into TSDB yourself, please feel free to request for it by
+creating an issue or make a PR to merge your code. ð¤ **Please** star this
+repo to help others notice TSDB if you think it is a useful toolkit. **Please**
+properly [cite TSDB](https://github.com/WenjieDu/TSDB#-citing-tsdbpypots) in
+your publications if it helps with your research. This really means a lot to
+our open-source research. Thank you! ## â Usage Examples TSDB now is
+available on [https://img.shields.io/badge/Anaconda--
+lightgreen?style=social&logo=anaconda]âï¸ Install it with `conda install
+tsdb`, you may need to specify the channel with option `-c conda-forge` or
+install from PyPI: > pip install tsdb or install from source code: > pip
+install `https://github.com/WenjieDu/TSDB/archive/main.zip` ```python import
+tsdb tsdb.list_available_datasets() # list all available datasets in TSDB data
+= tsdb.load_dataset('physionet_2012') # select the dataset you need and load
+it, TSDB will download, extract, and process it automatically
+tsdb.download_and_extract('physionet_2012', './save_it_here') # if you need the
+raw data, use download_and_extract() tsdb.list_cached_data() # datasets you
+once loaded are cached, and you can check them with list_cached_data()
+tsdb.delete_cached_data(dataset_name='physionet_2012') # you can delete only
+one specific dataset and preserve others tsdb.delete_cached_data() # or you can
+delete all cache with delete_cached_data() to free disk space ``` That's all.
+Simple and efficient. Enjoy it! ð ## â List of Available Datasets | Name |
+Main Tasks | |-----------------------------------------------------------------
+-----------------|-----------------------------------------| | [PhysioNet
+Challenge 2012](dataset_profiles/physionet_2012) | Classification, Forecasting,
+Imputation | | [PhysioNet Challenge 2019](dataset_profiles/physionet_2019) |
+Classification, Imputation | | [Beijing Multi-Site Air-Quality]
+(dataset_profiles/beijing_multisite_air_quality) | Forecasting, Imputation | |
+[Electricity Load Diagrams](dataset_profiles/electricity_load_diagrams) |
+Forecasting, Imputation | | [UCR & UEA Datasets](dataset_profiles/
+ucr_uea_datasets) (all 163 datasets) | Classification | | [Vessel AIS]
+(dataset_profiles/vessel_ais) | Classification, Forecasting, Imputation | ##
+â Citing TSDB/PyPOTS The paper introducing PyPOTS project is available on
+arXiv at [this URL](https://arxiv.org/abs/2305.18811), and we are pursuing to
+publish it in prestigious academic venues, e.g. JMLR (track for [Machine
+Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use TSDB
+in your work, please cite PyPOTS project as below and ðstar this repository
+to make others notice this library. ð¤ Thank you! ``` bibtex @article
+{du2023PyPOTS, title={{PyPOTS: A Python Toolbox for Data Mining on Partially-
+Observed Time Series}}, author={Wenjie Du}, year={2023}, eprint={2305.18811},
+archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://arxiv.org/abs/
+2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` or > Wenjie Du. (2023). >
+PyPOTS: A Python Toolbox for Data Mining on Partially-Observed Time Series. >
+arXiv, abs/2305.18811. https://doi.org/10.48550/arXiv.2305.18811  ð  Visits
+[https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FWenjieDu%2FTime_Series_Database&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+April+2022&edge_flat=false]
```

### Comparing `tsdb-0.0.9/README.md` & `tsdb-0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,61 @@
-<a href='https://github.com/WenjieDu/TSDB'><img src="https://raw.githubusercontent.com/WenjieDu/TSDB/main/docs/_static/figs/TSDB_logo.svg?sanitize=true" align='right' width='235'/></a>
+<a href='https://github.com/WenjieDu/TSDB'><img src="https://raw.githubusercontent.com/PyPOTS/pypots.github.io/main/static/figs/pypots_logos/TSDB_logo_FFBG.svg?sanitize=truee" align='right' width='235'/></a>
 
 # <p align='center'>Welcome to TSDB</p>
 **<p align='center'>A Python Toolbox to Ease Loading Open-Source Time-Series Datasets</p>**
 
 <p align='center'>
     <!-- Python version -->
     <img src='https://img.shields.io/badge/python-v3-E97040?logo=python&logoColor=white'>
     <!-- PyPI version -->
-    <img alt="PyPI" src="https://img.shields.io/pypi/v/tsdb?color=green&label=PyPI&logo=pypi&logoColor=white">
+    <a href="https://pypi.python.org/pypi/tsdb">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/tsdb?color=green&label=PyPI&logo=pypi&logoColor=white">
+    </a>
     <!-- License -->
     <a href="https://github.com/WenjieDu/TSDB/blob/main/LICENSE">
         <img alt="GPL-v3 license" src="https://img.shields.io/badge/License-GPL--v3-E9BB41">
     </a>
     <!-- GitHub Testing -->
-    <a alt='GitHub Testing' href='https://github.com/WenjieDu/TSDB/actions/workflows/testing.yml'> 
+    <a alt='GitHub Testing' href='https://github.com/WenjieDu/TSDB/actions/workflows/testing_ci.yml'>
         <img src='https://img.shields.io/github/actions/workflow/status/wenjiedu/tsdb/testing_ci.yml?logo=github&color=C8D8E1&label=CI'>
     </a>
     <a href="https://codeclimate.com/github/WenjieDu/TSDB">
         <img alt="Code Climate maintainability" src="https://img.shields.io/codeclimate/maintainability-percentage/WenjieDu/TSDB?color=3C7699&label=Maintainability&logo=codeclimate">
     </a>
     <!-- Coveralls report -->
-    <a alt='Coveralls report' href='https://coveralls.io/github/WenjieDu/TSDB'> 
+    <a alt='Coveralls report' href='https://coveralls.io/github/WenjieDu/TSDB'>
         <img src='https://img.shields.io/coverallsCoverage/github/WenjieDu/TSDB?branch=main&logo=coveralls&color=75C1C4&label=Coverage'>
     </a>
     <a href="https://anaconda.org/conda-forge/tsdb">
         <img alt="Conda downloads" src="https://img.shields.io/conda/dn/conda-forge/tsdb?label=Conda%20Downloads&color=AED0ED&logo=anaconda&logoColor=white">
     </a>
     <!-- PyPI download number -->
     <a alt='PyPI download number' href='https://pypi.org/project/tsdb'>
         <img src='https://static.pepy.tech/personalized-badge/tsdb?period=total&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20Downloads'>
     </a>
 </p>
 
-> 📣 TSDB now supports a total of 1️⃣6️⃣5️⃣ time-series datasets ‼️
+> 📣 TSDB now supports a total of 1️⃣6️⃣8️⃣ time-series datasets ‼️
+
+<a href='https://github.com/WenjieDu/PyPOTS'><img src='https://raw.githubusercontent.com/PyPOTS/pypots.github.io/main/static/figs/pypots_logos/PyPOTS_logo_FFBG.svg?sanitize=true' width='160' align='left' /></a>
+TSDB is a part of [PyPOTS project](https://github.com/WenjieDu/PyPOTS) (a Python toolbox for data mining on Partially-Observed Time Series), and was separated from PyPOTS for decoupling datasets from learning algorithms.
 
 TSDB is created to help researchers and engineers get rid of data collecting and downloading, and focus back on data processing details. TSDB provides all-in-one-stop convenience for downloading and loading open-source time-series datasets (available datasets listed [below](https://github.com/WenjieDu/TSDB#-list-of-available-datasets)).
 
 ❗️Please note that due to people have very different requirements for data processing, data-loading functions in TSDB only contain the most general steps (e.g. removing invalid samples) and won't process the data (not even normalize it). So, no worries, TSDB won't affect your data preprocessing. If you only want the raw datasets, TSDB can help you download and save raw datasets as well (take a look at [Usage Examples](https://github.com/WenjieDu/TSDB#-usage-example) below).
 
 🤝 If you need TSDB to integrate an open-source dataset or want to add it into TSDB yourself, please feel free to request for it by creating an issue or make a PR to merge your code.
 
 🤗 **Please** star this repo to help others notice TSDB if you think it is a useful toolkit.
 **Please** properly [cite TSDB](https://github.com/WenjieDu/TSDB#-citing-tsdbpypots) in your publications
 if it helps with your research. This really means a lot to our open-source research. Thank you!
 
 
 ## ❖ Usage Examples
-TSDB now is available on <a alt='Anaconda' href='https://anaconda.org/conda-forge/tsdb'><img align='center' src='https://img.shields.io/badge/Anaconda--lightgreen?style=social&logo=anaconda'></a>❗️ 
+TSDB now is available on <a alt='Anaconda' href='https://anaconda.org/conda-forge/tsdb'><img align='center' src='https://img.shields.io/badge/Anaconda--lightgreen?style=social&logo=anaconda'></a>❗️
 
 Install it with `conda install tsdb`, you may need to specify the channel with option `-c conda-forge`
 
 or install from PyPI:
 > pip install tsdb
 
 or install from source code:
@@ -59,37 +64,34 @@
 ```python
 import tsdb
 
 tsdb.list_available_datasets()  # list all available datasets in TSDB
 data = tsdb.load_dataset('physionet_2012')  # select the dataset you need and load it, TSDB will download, extract, and process it automatically
 tsdb.download_and_extract('physionet_2012', './save_it_here')  # if you need the raw data, use download_and_extract()
 tsdb.list_cached_data()  # datasets you once loaded are cached, and you can check them with list_cached_data()
-tsdb.delete_cached_data()  # you can delete all cache with delete_cached_data() to free disk space
-tsdb.delete_cached_data(dataset_name='physionet_2012')  # or you can delete only one specific dataset and preserve others
+tsdb.delete_cached_data(dataset_name='physionet_2012')  # you can delete only one specific dataset and preserve others
+tsdb.delete_cached_data()  # or you can delete all cache with delete_cached_data() to free disk space
 ```
 
 That's all. Simple and efficient. Enjoy it! 😃
 
 
 ## ❖ List of Available Datasets
 
-| Name                                                                  | Main Tasks                              |
-|-----------------------------------------------------------------------|-----------------------------------------|
-| [PhysioNet Challenge 2012](datasets/PhysioNet-2012)                   | Classification, Forecasting, Imputation |
-| [PhysioNet Challenge 2019](datasets/PhysioNet-2019)                   | Classification, Imputation              |
-| [Beijing Multi-Site Air-Quality](datasets/BeijingMultiSiteAirQuality) | Forecasting, Imputation                 |
-| [Electricity Load Diagrams](datasets/ElectricityLoadDiagrams)         | Forecasting, Imputation                 |
-| [UCR & UEA Datasets](datasets/UCR_UEA_Datasets) (all 160 datasets)    | Classification                          |
-| [Vessel AIS](datasets/Vessel_AIS)                                     | Classification, Forecasting, Imputation |
+| Name                                                                             | Main Tasks                              |
+|----------------------------------------------------------------------------------|-----------------------------------------|
+| [PhysioNet Challenge 2012](dataset_profiles/physionet_2012)                      | Classification, Forecasting, Imputation |
+| [PhysioNet Challenge 2019](dataset_profiles/physionet_2019)                      | Classification, Imputation              |
+| [Beijing Multi-Site Air-Quality](dataset_profiles/beijing_multisite_air_quality) | Forecasting, Imputation                 |
+| [Electricity Load Diagrams](dataset_profiles/electricity_load_diagrams)          | Forecasting, Imputation                 |
+| [UCR & UEA Datasets](dataset_profiles/ucr_uea_datasets) (all 163 datasets)       | Classification                          |
+| [Vessel AIS](dataset_profiles/vessel_ais)                                        | Classification, Forecasting, Imputation |
 
 
 ## ❖ Citing TSDB/PyPOTS
-<a href='https://github.com/WenjieDu/PyPOTS'><img src='https://raw.githubusercontent.com/WenjieDu/PyPOTS/main/docs/_static/figs/PyPOTS_logo.svg?sanitize=true' width='160' align='left' /></a>
-TSDB is a part of [PyPOTS project](https://github.com/WenjieDu/PyPOTS) (a Python toolbox for data mining on Partially-Observed Time Series), and was separated from PyPOTS for decoupling datasets from learning algorithms.
-
 The paper introducing PyPOTS project is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
 and we are pursuing to publish it in prestigious academic venues, e.g. JMLR (track for
 [Machine Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use TSDB in your work,
 please cite PyPOTS project as below and 🌟star this repository to make others notice this library. 🤗 Thank you!
 
 ``` bibtex
 @article{du2023PyPOTS,
```

#### html2text {}

```diff
@@ -1,73 +1,75 @@
-[https://raw.githubusercontent.com/WenjieDu/TSDB/main/docs/_static/figs/
-TSDB_logo.svg?sanitize=true] #
+[https://raw.githubusercontent.com/PyPOTS/pypots.github.io/main/static/figs/
+pypots_logos/TSDB_logo_FFBG.svg?sanitize=truee] #
                                 Welcome to TSDB
 **
        A Python Toolbox to Ease Loading Open-Source Time-Series Datasets
 **
  [https://img.shields.io/badge/python-v3-E97040?logo=python&logoColor=white]
   [PyPI]  [GPL-v3_license]  [https://img.shields.io/github/actions/workflow/
  status/wenjiedu/tsdb/testing_ci.yml?logo=github&color=C8D8E1&label=CI] [Code
   Climate_maintainability]  [https://img.shields.io/coverallsCoverage/github/
  WenjieDu/TSDB?branch=main&logo=coveralls&color=75C1C4&label=Coverage] [Conda
            downloads]  [https://static.pepy.tech/personalized-badge/
 tsdb?period=total&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20Downloads]
-> ð£ TSDB now supports a total of 1ï¸â£6ï¸â£5ï¸â£ time-series datasets
-â¼ï¸ TSDB is created to help researchers and engineers get rid of data
-collecting and downloading, and focus back on data processing details. TSDB
-provides all-in-one-stop convenience for downloading and loading open-source
-time-series datasets (available datasets listed [below](https://github.com/
-WenjieDu/TSDB#-list-of-available-datasets)). âï¸Please note that due to
-people have very different requirements for data processing, data-loading
-functions in TSDB only contain the most general steps (e.g. removing invalid
-samples) and won't process the data (not even normalize it). So, no worries,
-TSDB won't affect your data preprocessing. If you only want the raw datasets,
-TSDB can help you download and save raw datasets as well (take a look at [Usage
-Examples](https://github.com/WenjieDu/TSDB#-usage-example) below). ð¤ If you
-need TSDB to integrate an open-source dataset or want to add it into TSDB
-yourself, please feel free to request for it by creating an issue or make a PR
-to merge your code. ð¤ **Please** star this repo to help others notice TSDB
-if you think it is a useful toolkit. **Please** properly [cite TSDB](https://
-github.com/WenjieDu/TSDB#-citing-tsdbpypots) in your publications if it helps
-with your research. This really means a lot to our open-source research. Thank
-you! ## â Usage Examples TSDB now is available on [https://img.shields.io/
-badge/Anaconda--lightgreen?style=social&logo=anaconda]âï¸ Install it with
-`conda install tsdb`, you may need to specify the channel with option `-
-c conda-forge` or install from PyPI: > pip install tsdb or install from source
-code: > pip install `https://github.com/WenjieDu/TSDB/archive/main.zip`
-```python import tsdb tsdb.list_available_datasets() # list all available
-datasets in TSDB data = tsdb.load_dataset('physionet_2012') # select the
-dataset you need and load it, TSDB will download, extract, and process it
-automatically tsdb.download_and_extract('physionet_2012', './save_it_here') #
-if you need the raw data, use download_and_extract() tsdb.list_cached_data() #
-datasets you once loaded are cached, and you can check them with
-list_cached_data() tsdb.delete_cached_data() # you can delete all cache with
-delete_cached_data() to free disk space tsdb.delete_cached_data
-(dataset_name='physionet_2012') # or you can delete only one specific dataset
-and preserve others ``` That's all. Simple and efficient. Enjoy it! ð ## â
-List of Available Datasets | Name | Main Tasks | |-----------------------------
-------------------------------------------|------------------------------------
------| | [PhysioNet Challenge 2012](datasets/PhysioNet-2012) | Classification,
-Forecasting, Imputation | | [PhysioNet Challenge 2019](datasets/PhysioNet-2019)
-| Classification, Imputation | | [Beijing Multi-Site Air-Quality](datasets/
-BeijingMultiSiteAirQuality) | Forecasting, Imputation | | [Electricity Load
-Diagrams](datasets/ElectricityLoadDiagrams) | Forecasting, Imputation | | [UCR
-& UEA Datasets](datasets/UCR_UEA_Datasets) (all 160 datasets) | Classification
-| | [Vessel AIS](datasets/Vessel_AIS) | Classification, Forecasting, Imputation
-| ## â Citing TSDB/PyPOTS [https://raw.githubusercontent.com/WenjieDu/PyPOTS/
-main/docs/_static/figs/PyPOTS_logo.svg?sanitize=true] TSDB is a part of [PyPOTS
+> ð£ TSDB now supports a total of 1ï¸â£6ï¸â£8ï¸â£ time-series datasets
+â¼ï¸ [https://raw.githubusercontent.com/PyPOTS/pypots.github.io/main/static/
+figs/pypots_logos/PyPOTS_logo_FFBG.svg?sanitize=true] TSDB is a part of [PyPOTS
 project](https://github.com/WenjieDu/PyPOTS) (a Python toolbox for data mining
 on Partially-Observed Time Series), and was separated from PyPOTS for
-decoupling datasets from learning algorithms. The paper introducing PyPOTS
-project is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
-and we are pursuing to publish it in prestigious academic venues, e.g. JMLR
-(track for [Machine Learning Open Source Software](https://www.jmlr.org/mloss/
-)). If you use TSDB in your work, please cite PyPOTS project as below and
-ðstar this repository to make others notice this library. ð¤ Thank you!
-``` bibtex @article{du2023PyPOTS, title={{PyPOTS: A Python Toolbox for Data
-Mining on Partially-Observed Time Series}}, author={Wenjie Du}, year={2023},
-eprint={2305.18811}, archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://
-arxiv.org/abs/2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` or > Wenjie
-Du. (2023). > PyPOTS: A Python Toolbox for Data Mining on Partially-Observed
-Time Series. > arXiv, abs/2305.18811. https://doi.org/10.48550/arXiv.2305.18811
-ð  Visits [https://hits.seeyoufarm.com/api/count/incr/
+decoupling datasets from learning algorithms. TSDB is created to help
+researchers and engineers get rid of data collecting and downloading, and focus
+back on data processing details. TSDB provides all-in-one-stop convenience for
+downloading and loading open-source time-series datasets (available datasets
+listed [below](https://github.com/WenjieDu/TSDB#-list-of-available-datasets)).
+âï¸Please note that due to people have very different requirements for data
+processing, data-loading functions in TSDB only contain the most general steps
+(e.g. removing invalid samples) and won't process the data (not even normalize
+it). So, no worries, TSDB won't affect your data preprocessing. If you only
+want the raw datasets, TSDB can help you download and save raw datasets as well
+(take a look at [Usage Examples](https://github.com/WenjieDu/TSDB#-usage-
+example) below). ð¤ If you need TSDB to integrate an open-source dataset or
+want to add it into TSDB yourself, please feel free to request for it by
+creating an issue or make a PR to merge your code. ð¤ **Please** star this
+repo to help others notice TSDB if you think it is a useful toolkit. **Please**
+properly [cite TSDB](https://github.com/WenjieDu/TSDB#-citing-tsdbpypots) in
+your publications if it helps with your research. This really means a lot to
+our open-source research. Thank you! ## â Usage Examples TSDB now is
+available on [https://img.shields.io/badge/Anaconda--
+lightgreen?style=social&logo=anaconda]âï¸ Install it with `conda install
+tsdb`, you may need to specify the channel with option `-c conda-forge` or
+install from PyPI: > pip install tsdb or install from source code: > pip
+install `https://github.com/WenjieDu/TSDB/archive/main.zip` ```python import
+tsdb tsdb.list_available_datasets() # list all available datasets in TSDB data
+= tsdb.load_dataset('physionet_2012') # select the dataset you need and load
+it, TSDB will download, extract, and process it automatically
+tsdb.download_and_extract('physionet_2012', './save_it_here') # if you need the
+raw data, use download_and_extract() tsdb.list_cached_data() # datasets you
+once loaded are cached, and you can check them with list_cached_data()
+tsdb.delete_cached_data(dataset_name='physionet_2012') # you can delete only
+one specific dataset and preserve others tsdb.delete_cached_data() # or you can
+delete all cache with delete_cached_data() to free disk space ``` That's all.
+Simple and efficient. Enjoy it! ð ## â List of Available Datasets | Name |
+Main Tasks | |-----------------------------------------------------------------
+-----------------|-----------------------------------------| | [PhysioNet
+Challenge 2012](dataset_profiles/physionet_2012) | Classification, Forecasting,
+Imputation | | [PhysioNet Challenge 2019](dataset_profiles/physionet_2019) |
+Classification, Imputation | | [Beijing Multi-Site Air-Quality]
+(dataset_profiles/beijing_multisite_air_quality) | Forecasting, Imputation | |
+[Electricity Load Diagrams](dataset_profiles/electricity_load_diagrams) |
+Forecasting, Imputation | | [UCR & UEA Datasets](dataset_profiles/
+ucr_uea_datasets) (all 163 datasets) | Classification | | [Vessel AIS]
+(dataset_profiles/vessel_ais) | Classification, Forecasting, Imputation | ##
+â Citing TSDB/PyPOTS The paper introducing PyPOTS project is available on
+arXiv at [this URL](https://arxiv.org/abs/2305.18811), and we are pursuing to
+publish it in prestigious academic venues, e.g. JMLR (track for [Machine
+Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use TSDB
+in your work, please cite PyPOTS project as below and ðstar this repository
+to make others notice this library. ð¤ Thank you! ``` bibtex @article
+{du2023PyPOTS, title={{PyPOTS: A Python Toolbox for Data Mining on Partially-
+Observed Time Series}}, author={Wenjie Du}, year={2023}, eprint={2305.18811},
+archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://arxiv.org/abs/
+2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` or > Wenjie Du. (2023). >
+PyPOTS: A Python Toolbox for Data Mining on Partially-Observed Time Series. >
+arXiv, abs/2305.18811. https://doi.org/10.48550/arXiv.2305.18811  ð  Visits
+[https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FWenjieDu%2FTime_Series_Database&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+April+2022&edge_flat=false]
```

### Comparing `tsdb-0.0.9/setup.py` & `tsdb-0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,22 +18,25 @@
     project_urls={
         "Documentation": "https://tsdb.readthedocs.io/",
         "Source": "https://github.com/WenjieDu/TSDB/",
         "Tracker": "https://github.com/WenjieDu/TSDB/issues/",
         "Download": "https://github.com/WenjieDu/TSDB/archive/main.zip",
     },
     keywords=[
-        "time-series analysis",
+        "data mining",
         "time series",
+        "time-series analysis",
         "time-series database",
         "time-series datasets",
-        "datasets",
         "database",
+        "datasets",
         "dataset downloading",
-        "data mining",
+        "imputation",
+        "classification",
+        "forecasting",
     ],
     packages=find_packages(exclude=["tests"]),
     include_package_data=True,
     install_requires=[
         "numpy",
         "scikit-learn",
         "pandas",
```

### Comparing `tsdb-0.0.9/tsdb/__init__.py` & `tsdb-0.1/tsdb/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,21 @@
 # X.YaN # Alpha release
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
-__version__ = "0.0.9"
+__version__ = "0.1"
 
 
 try:
-    from tsdb.database import (
+    from tsdb.data_processing import (
         list_database,
         list_available_datasets,
-    )
-
-    from tsdb.data_processing import (
         window_truncate,
         download_and_extract,
         load_dataset,
         delete_cached_data,
         purge_given_path,
         list_cached_data,
         CACHED_DATASET_DIR,
```

### Comparing `tsdb-0.0.9/tsdb/data_loading_funcs/__init__.py` & `tsdb-0.1/tsdb/loading_funcs/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Functions to load specific datasets.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
-from tsdb.data_loading_funcs.beijing_multisite_air_quality import (
+from tsdb.loading_funcs.beijing_multisite_air_quality import (
     load_beijing_air_quality,
 )
-from tsdb.data_loading_funcs.electricity_load_diagrams import load_electricity
-from tsdb.data_loading_funcs.physionet_2012 import load_physionet2012
-from tsdb.data_loading_funcs.physionet_2019 import load_physionet2019
-from tsdb.data_loading_funcs.ucr_uea_datasets import load_ucr_uea_dataset
-from tsdb.data_loading_funcs.vessel_ais import load_ais
+from tsdb.loading_funcs.electricity_load_diagrams import load_electricity
+from tsdb.loading_funcs.physionet_2012 import load_physionet2012
+from tsdb.loading_funcs.physionet_2019 import load_physionet2019
+from tsdb.loading_funcs.ucr_uea_datasets import load_ucr_uea_dataset
+from tsdb.loading_funcs.vessel_ais import load_ais
 
 __all__ = [
     "load_beijing_air_quality",
     "load_electricity",
     "load_physionet2012",
     "load_physionet2019",
     "load_ucr_uea_dataset",
```

### Comparing `tsdb-0.0.9/tsdb/data_loading_funcs/beijing_multisite_air_quality.py` & `tsdb-0.1/tsdb/loading_funcs/beijing_multisite_air_quality.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Scripts related to dataset Beijing Multi-site Air Quality.
 
 For more information please refer to:
-https://github.com/WenjieDu/Time_Series_Database/tree/main/datasets/BeijingMultiSiteAirQuality
+https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/beijing_multisite_air_quality
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 import os
```

### Comparing `tsdb-0.0.9/tsdb/data_loading_funcs/electricity_load_diagrams.py` & `tsdb-0.1/tsdb/loading_funcs/electricity_load_diagrams.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Scripts related to dataset Electricity Load Diagrams.
 
 For more information please refer to:
-https://github.com/WenjieDu/Time_Series_Database/tree/main/datasets/ElectricityLoadDiagrams
+https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/electricity_load_diagrams
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 import os
```

### Comparing `tsdb-0.0.9/tsdb/data_loading_funcs/physionet_2012.py` & `tsdb-0.1/tsdb/loading_funcs/physionet_2012.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Scripts related to dataset PhysioNet Challenge 2012.
 
 For more information please refer to:
-https://github.com/WenjieDu/Time_Series_Database/tree/main/datasets/PhysioNet-2012
+https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/physionet_2012
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 import os
```

### Comparing `tsdb-0.0.9/tsdb/data_loading_funcs/physionet_2019.py` & `tsdb-0.1/tsdb/loading_funcs/physionet_2019.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
 Scripts related to dataset PhysioNet Challenge 2019.
 
+For more information please refer to:
+https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/physionet_2019
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 import os
```

### Comparing `tsdb-0.0.9/tsdb/data_loading_funcs/ucr_uea_datasets.py` & `tsdb-0.1/tsdb/loading_funcs/ucr_uea_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """
 Scripts related to UCR&UAE datasets http://timeseriesclassification.com/index.php
 
 Most of code comes from library tslearn https://github.com/tslearn-team/tslearn.
 
+For more information please refer to:
+https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/ucr_uea_datasets
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 import os
 import warnings
 
 import numpy
 from sklearn.utils.estimator_checks import _NotAnArray as NotAnArray
 
 try:
     from scipy.io import arff
+
     HAS_ARFF = True
 except Exception:
     HAS_ARFF = False
 
 
 def load_ucr_uea_dataset(local_path, dataset_name):
     try:
```

### Comparing `tsdb-0.0.9/tsdb/data_loading_funcs/vessel_ais.py` & `tsdb-0.1/tsdb/loading_funcs/vessel_ais.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Scripts related to dataset vessel_AIS.
 
 For more information please refer to:
-https://github.com/WenjieDu/Time_Series_Database/tree/main/datasets/Vessel_AIS
+https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/vessel_ais
 """
 
 # Created by Grgičević Luka <luka.grgicevic@ntnu.no>
 # Modified by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 import os
```

### Comparing `tsdb-0.0.9/tsdb/database.py` & `tsdb-0.1/tsdb/database.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,129 +1,182 @@
 """
 List available datasets and their official download links.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
+import os
+
+CACHED_DATASET_DIR = os.path.join(os.path.expanduser("~"), ".tsdb_cached_datasets")
+
 _DATABASE = {
-    # https://github.com/WenjieDu/Time_Series_Database/tree/main/datasets/PhysioNet-2012
+    # http://www.physionet.org/challenge/2012
+    # https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/physionet_2012
     "physionet_2012": [
         "https://www.physionet.org/files/challenge-2012/1.0.0/set-a.tar.gz",
         "https://www.physionet.org/files/challenge-2012/1.0.0/set-b.tar.gz",
         "https://www.physionet.org/files/challenge-2012/1.0.0/set-c.tar.gz",
         "https://www.physionet.org/files/challenge-2012/1.0.0/Outcomes-a.txt",
         "https://www.physionet.org/files/challenge-2012/1.0.0/Outcomes-b.txt",
         "https://www.physionet.org/files/challenge-2012/1.0.0/Outcomes-c.txt",
     ],
-    #
-    # https://github.com/WenjieDu/Time_Series_Database/tree/main/datasets/PhysioNet-2019
+    # http://www.physionet.org/challenge/2019
+    # https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/physionet_2019
     "physionet_2019": [
         "https://archive.physionet.org/users/shared/challenge-2019/training_setA.zip",
         "https://archive.physionet.org/users/shared/challenge-2019/training_setB.zip",
     ],
     #
-    # https://github.com/WenjieDu/Time_Series_Database/tree/main/datasets/ElectricityLoadDiagrams
+    # https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/electricity_load_diagrams
     "electricity_load_diagrams": "https://archive.ics.uci.edu/ml/machine-learning-databases/00321/LD2011_2014.txt.zip",
     #
-    # https://github.com/WenjieDu/Time_Series_Database/tree/main/datasets/BeijingMultiSiteAirQuality
+    # https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/beijing_multisite_air_quality
     "beijing_multisite_air_quality": "https://archive.ics.uci.edu/ml/machine-learning-databases/00501/"
-    "PRSA2017_Data_20130301-20170228.zip",
+                                     "PRSA2017_Data_20130301-20170228.zip",
     #
-    # https://github.com/WenjieDu/Time_Series_Database/tree/main/datasets/Vessel_AIS
-    "vessel_AIS": "https://zenodo.org/record/8064564/files/parquets.zip",
+    # https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/vessel_ais
+    "vessel_ais": "https://zenodo.org/record/8064564/files/parquets.zip",
 }
 
-_UCR_UEA_datasets = [
+# https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/ucr_uea_datasets
+# 128 UCR + 33 UEA + 2 old removed (NonInvasiveFatalECGThorax1 and 2) = 163
+_ucr_uea_datasets = [
+    "ACSF1",
     "Adiac",
+    "AllGestureWiimoteX",
+    "AllGestureWiimoteY",
+    "AllGestureWiimoteZ",
     "ArrowHead",
     "Beef",
     "BeetleFly",
     "BirdChicken",
+    "BME",
     "Car",
     "CBF",
+    "Chinatown",
     "ChlorineConcentration",
     "CinCECGTorso",
     "Coffee",
     "Computers",
     "CricketX",
     "CricketY",
     "CricketZ",
+    "Crop",
     "DiatomSizeReduction",
     "DistalPhalanxOutlineCorrect",
     "DistalPhalanxOutlineAgeGroup",
     "DistalPhalanxTW",
+    "DodgerLoopDay",
+    "DodgerLoopGame",
+    "DodgerLoopWeekend",
     "Earthquakes",
     "ECG200",
     "ECG5000",
     "ECGFiveDays",
     "ElectricDevices",
+    "EOGHorizontalSignal",
+    "EOGVerticalSignal",
+    "EthanolLevel",
     "FaceAll",
     "FaceFour",
     "FacesUCR",
     "FiftyWords",
     "Fish",
     "FordA",
     "FordB",
+    "FreezerRegularTrain",
+    "FreezerSmallTrain",
+    "Fungi",
+    "GestureMidAirD1",
+    "GestureMidAirD2",
+    "GestureMidAirD3",
+    "GesturePebbleZ1",
+    "GesturePebbleZ2",
     "GunPoint",
+    "GunPointAgeSpan",
+    "GunPointMaleVersusFemale",
+    "GunPointOldVersusYoung",
     "Ham",
     "HandOutlines",
     "Haptics",
     "Herring",
+    "HouseTwenty",
     "InlineSkate",
+    "InsectEPGRegularTrain",
+    "InsectEPGSmallTrain",
     "InsectWingbeatSound",
     "ItalyPowerDemand",
     "LargeKitchenAppliances",
     "Lightning2",
     "Lightning7",
     "Mallat",
     "Meat",
     "MedicalImages",
+    "MelbournePedestrian",
     "MiddlePhalanxOutlineCorrect",
     "MiddlePhalanxOutlineAgeGroup",
     "MiddlePhalanxTW",
+    "MixedShapesRegularTrain",
+    "MixedShapesSmallTrain",
     "MoteStrain",
-    "NonInvasiveFatalECGThorax1",
-    "NonInvasiveFatalECGThorax2",
+    "NonInvasiveFetalECGThorax1",
+    "NonInvasiveFetalECGThorax2",
     "OliveOil",
     "OSULeaf",
     "PhalangesOutlinesCorrect",
     "Phoneme",
+    "PickupGestureWiimoteZ",
+    "PigAirwayPressure",
+    "PigArtPressure",
+    "PigCVP",
+    "PLAID",
     "Plane",
+    "PowerCons",
     "ProximalPhalanxOutlineCorrect",
     "ProximalPhalanxOutlineAgeGroup",
     "ProximalPhalanxTW",
     "RefrigerationDevices",
+    "Rock",
     "ScreenType",
+    "SemgHandGenderCh2",
+    "SemgHandMovementCh2",
+    "SemgHandSubjectCh2",
+    "ShakeGestureWiimoteZ",
     "ShapeletSim",
     "ShapesAll",
     "SmallKitchenAppliances",
+    "SmoothSubspace",
     "SonyAIBORobotSurface1",
     "SonyAIBORobotSurface2",
     "StarLightCurves",
     "Strawberry",
     "SwedishLeaf",
     "Symbols",
     "SyntheticControl",
     "ToeSegmentation1",
     "ToeSegmentation2",
     "Trace",
     "TwoLeadECG",
     "TwoPatterns",
+    "UMD",
+    "UWaveGestureLibraryAll",
     "UWaveGestureLibraryX",
     "UWaveGestureLibraryY",
     "UWaveGestureLibraryZ",
-    "UWaveGestureLibraryAll",
     "Wafer",
     "Wine",
     "WordSynonyms",
     "Worms",
     "WormsTwoClass",
     "Yoga",
     "ArticularyWordRecognition",
+    "AsphaltObstaclesCoordinates",
+    "AsphaltPavementTypeCoordinates",
+    "AsphaltRegularityCoordinates",
     "AtrialFibrillation",
     "BasicMotions",
     "CharacterTrajectories",
     "Cricket",
     "DuckDuckGeese",
     "EigenWorms",
     "Epilepsy",
@@ -138,93 +191,26 @@
     "JapaneseVowels",
     "Libras",
     "LSST",
     "MotorImagery",
     "NATOPS",
     "PenDigits",
     "PEMS-SF",
-    "Phoneme",
+    "PhonemeSpectra",
     "RacketSports",
     "SelfRegulationSCP1",
     "SelfRegulationSCP2",
     "SpokenArabicDigits",
     "StandWalkJump",
     "UWaveGestureLibrary",
-    "ACSF1",
-    "AllGestureWiimoteX",
-    "AllGestureWiimoteY",
-    "AllGestureWiimoteZ",
-    "BME",
-    "Chinatown",
-    "Crop",
-    "DodgerLoopDay",
-    "DodgerLoopGame",
-    "DodgerLoopWeekend",
-    "EOGHorizontalSignal",
-    "EOGVerticalSignal",
-    "EthanolLevel",
-    "FreezerRegularTrain",
-    "FreezerSmallTrain",
-    "Fungi",
-    "GestureMidAirD1",
-    "GestureMidAirD2",
-    "GestureMidAirD3",
-    "GesturePebbleZ1",
-    "GesturePebbleZ2",
-    "GunPointAgeSpan",
-    "GunPointMaleVersusFemale",
-    "GunPointOldVersusYoung",
-    "HouseTwenty",
-    "InsectEPGRegularTrain",
-    "InsectEPGSmallTrain",
-    "MelbournePedestrian",
-    "MixedShapesRegularTrain",
-    "MixedShapesSmallTrain",
-    "NonInvasiveFetalECGThorax1",
-    "NonInvasiveFetalECGThorax2",
-    "PLAID",
-    "PickupGestureWiimoteZ",
-    "PigAirwayPressure",
-    "PigArtPressure",
-    "PigCVP",
-    "PowerCons",
-    "Rock",
-    "SemgHandGenderCh2",
-    "SemgHandMovementCh2",
-    "SemgHandSubjectCh2",
-    "ShakeGestureWiimoteZ",
-    "SmoothSubspace",
-    "UMD",
+    "NonInvasiveFatalECGThorax1",
+    "NonInvasiveFatalECGThorax2",
 ]
 
-UCR_UEA_datasets = {}
-for i in _UCR_UEA_datasets:
-    UCR_UEA_datasets[
-        "UCR_UEA_" + i
-    ] = f"https://www.timeseriesclassification.com/ClassificationDownloads/{i}.zip"
+UCR_UEA_DATASETS = {}
+for i in _ucr_uea_datasets:
+    UCR_UEA_DATASETS[
+        "ucr_uea_" + i
+        ] = f"https://www.timeseriesclassification.com/aeon-toolkit/{i}.zip"
 
-DATABASE = {**_DATABASE, **UCR_UEA_datasets}
+DATABASE = {**_DATABASE, **UCR_UEA_DATASETS}
 AVAILABLE_DATASETS = list(DATABASE.keys())
-
-
-def list_database():
-    """List the database.
-
-    Returns
-    -------
-    DATABASE : dict
-        A dict contains all datasets' names and download links.
-
-    """
-    return DATABASE
-
-
-def list_available_datasets():
-    """List all available datasets.
-
-    Returns
-    -------
-    AVAILABLE_DATASETS : list
-        A list contains all datasets' names.
-
-    """
-    return AVAILABLE_DATASETS
```

### Comparing `tsdb-0.0.9/tsdb.egg-info/PKG-INFO` & `tsdb-0.1/tsdb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,81 +1,86 @@
 Metadata-Version: 2.1
 Name: tsdb
-Version: 0.0.9
+Version: 0.1
 Summary: TSDB (Time-Series DataBase): A Python Toolbox Helping Load Open-Source Time-Series Datasets
 Home-page: https://github.com/WenjieDu/TSDB
 Author: Wenjie Du
 Author-email: wenjay.du@gmail.com
 License: GPL-3.0
 Project-URL: Documentation, https://tsdb.readthedocs.io/
 Project-URL: Source, https://github.com/WenjieDu/TSDB/
 Project-URL: Tracker, https://github.com/WenjieDu/TSDB/issues/
 Project-URL: Download, https://github.com/WenjieDu/TSDB/archive/main.zip
-Keywords: time-series analysis,time series,time-series database,time-series datasets,datasets,database,dataset downloading,data mining
+Keywords: data mining,time series,time-series analysis,time-series database,time-series datasets,database,datasets,dataset downloading,imputation,classification,forecasting
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database
 Description-Content-Type: text/markdown
 Provides-Extra: basic
 License-File: LICENSE
 
-<a href='https://github.com/WenjieDu/TSDB'><img src="https://raw.githubusercontent.com/WenjieDu/TSDB/main/docs/_static/figs/TSDB_logo.svg?sanitize=true" align='right' width='235'/></a>
+<a href='https://github.com/WenjieDu/TSDB'><img src="https://raw.githubusercontent.com/PyPOTS/pypots.github.io/main/static/figs/pypots_logos/TSDB_logo_FFBG.svg?sanitize=truee" align='right' width='235'/></a>
 
 # <p align='center'>Welcome to TSDB</p>
 **<p align='center'>A Python Toolbox to Ease Loading Open-Source Time-Series Datasets</p>**
 
 <p align='center'>
     <!-- Python version -->
     <img src='https://img.shields.io/badge/python-v3-E97040?logo=python&logoColor=white'>
     <!-- PyPI version -->
-    <img alt="PyPI" src="https://img.shields.io/pypi/v/tsdb?color=green&label=PyPI&logo=pypi&logoColor=white">
+    <a href="https://pypi.python.org/pypi/tsdb">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/tsdb?color=green&label=PyPI&logo=pypi&logoColor=white">
+    </a>
     <!-- License -->
     <a href="https://github.com/WenjieDu/TSDB/blob/main/LICENSE">
         <img alt="GPL-v3 license" src="https://img.shields.io/badge/License-GPL--v3-E9BB41">
     </a>
     <!-- GitHub Testing -->
-    <a alt='GitHub Testing' href='https://github.com/WenjieDu/TSDB/actions/workflows/testing.yml'> 
+    <a alt='GitHub Testing' href='https://github.com/WenjieDu/TSDB/actions/workflows/testing_ci.yml'>
         <img src='https://img.shields.io/github/actions/workflow/status/wenjiedu/tsdb/testing_ci.yml?logo=github&color=C8D8E1&label=CI'>
     </a>
     <a href="https://codeclimate.com/github/WenjieDu/TSDB">
         <img alt="Code Climate maintainability" src="https://img.shields.io/codeclimate/maintainability-percentage/WenjieDu/TSDB?color=3C7699&label=Maintainability&logo=codeclimate">
     </a>
     <!-- Coveralls report -->
-    <a alt='Coveralls report' href='https://coveralls.io/github/WenjieDu/TSDB'> 
+    <a alt='Coveralls report' href='https://coveralls.io/github/WenjieDu/TSDB'>
         <img src='https://img.shields.io/coverallsCoverage/github/WenjieDu/TSDB?branch=main&logo=coveralls&color=75C1C4&label=Coverage'>
     </a>
     <a href="https://anaconda.org/conda-forge/tsdb">
         <img alt="Conda downloads" src="https://img.shields.io/conda/dn/conda-forge/tsdb?label=Conda%20Downloads&color=AED0ED&logo=anaconda&logoColor=white">
     </a>
     <!-- PyPI download number -->
     <a alt='PyPI download number' href='https://pypi.org/project/tsdb'>
         <img src='https://static.pepy.tech/personalized-badge/tsdb?period=total&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20Downloads'>
     </a>
 </p>
 
-> 📣 TSDB now supports a total of 1️⃣6️⃣5️⃣ time-series datasets ‼️
+> 📣 TSDB now supports a total of 1️⃣6️⃣8️⃣ time-series datasets ‼️
+
+<a href='https://github.com/WenjieDu/PyPOTS'><img src='https://raw.githubusercontent.com/PyPOTS/pypots.github.io/main/static/figs/pypots_logos/PyPOTS_logo_FFBG.svg?sanitize=true' width='160' align='left' /></a>
+TSDB is a part of [PyPOTS project](https://github.com/WenjieDu/PyPOTS) (a Python toolbox for data mining on Partially-Observed Time Series), and was separated from PyPOTS for decoupling datasets from learning algorithms.
 
 TSDB is created to help researchers and engineers get rid of data collecting and downloading, and focus back on data processing details. TSDB provides all-in-one-stop convenience for downloading and loading open-source time-series datasets (available datasets listed [below](https://github.com/WenjieDu/TSDB#-list-of-available-datasets)).
 
 ❗️Please note that due to people have very different requirements for data processing, data-loading functions in TSDB only contain the most general steps (e.g. removing invalid samples) and won't process the data (not even normalize it). So, no worries, TSDB won't affect your data preprocessing. If you only want the raw datasets, TSDB can help you download and save raw datasets as well (take a look at [Usage Examples](https://github.com/WenjieDu/TSDB#-usage-example) below).
 
 🤝 If you need TSDB to integrate an open-source dataset or want to add it into TSDB yourself, please feel free to request for it by creating an issue or make a PR to merge your code.
 
 🤗 **Please** star this repo to help others notice TSDB if you think it is a useful toolkit.
 **Please** properly [cite TSDB](https://github.com/WenjieDu/TSDB#-citing-tsdbpypots) in your publications
 if it helps with your research. This really means a lot to our open-source research. Thank you!
 
 
 ## ❖ Usage Examples
-TSDB now is available on <a alt='Anaconda' href='https://anaconda.org/conda-forge/tsdb'><img align='center' src='https://img.shields.io/badge/Anaconda--lightgreen?style=social&logo=anaconda'></a>❗️ 
+TSDB now is available on <a alt='Anaconda' href='https://anaconda.org/conda-forge/tsdb'><img align='center' src='https://img.shields.io/badge/Anaconda--lightgreen?style=social&logo=anaconda'></a>❗️
 
 Install it with `conda install tsdb`, you may need to specify the channel with option `-c conda-forge`
 
 or install from PyPI:
 > pip install tsdb
 
 or install from source code:
@@ -84,37 +89,34 @@
 ```python
 import tsdb
 
 tsdb.list_available_datasets()  # list all available datasets in TSDB
 data = tsdb.load_dataset('physionet_2012')  # select the dataset you need and load it, TSDB will download, extract, and process it automatically
 tsdb.download_and_extract('physionet_2012', './save_it_here')  # if you need the raw data, use download_and_extract()
 tsdb.list_cached_data()  # datasets you once loaded are cached, and you can check them with list_cached_data()
-tsdb.delete_cached_data()  # you can delete all cache with delete_cached_data() to free disk space
-tsdb.delete_cached_data(dataset_name='physionet_2012')  # or you can delete only one specific dataset and preserve others
+tsdb.delete_cached_data(dataset_name='physionet_2012')  # you can delete only one specific dataset and preserve others
+tsdb.delete_cached_data()  # or you can delete all cache with delete_cached_data() to free disk space
 ```
 
 That's all. Simple and efficient. Enjoy it! 😃
 
 
 ## ❖ List of Available Datasets
 
-| Name                                                                  | Main Tasks                              |
-|-----------------------------------------------------------------------|-----------------------------------------|
-| [PhysioNet Challenge 2012](datasets/PhysioNet-2012)                   | Classification, Forecasting, Imputation |
-| [PhysioNet Challenge 2019](datasets/PhysioNet-2019)                   | Classification, Imputation              |
-| [Beijing Multi-Site Air-Quality](datasets/BeijingMultiSiteAirQuality) | Forecasting, Imputation                 |
-| [Electricity Load Diagrams](datasets/ElectricityLoadDiagrams)         | Forecasting, Imputation                 |
-| [UCR & UEA Datasets](datasets/UCR_UEA_Datasets) (all 160 datasets)    | Classification                          |
-| [Vessel AIS](datasets/Vessel_AIS)                                     | Classification, Forecasting, Imputation |
+| Name                                                                             | Main Tasks                              |
+|----------------------------------------------------------------------------------|-----------------------------------------|
+| [PhysioNet Challenge 2012](dataset_profiles/physionet_2012)                      | Classification, Forecasting, Imputation |
+| [PhysioNet Challenge 2019](dataset_profiles/physionet_2019)                      | Classification, Imputation              |
+| [Beijing Multi-Site Air-Quality](dataset_profiles/beijing_multisite_air_quality) | Forecasting, Imputation                 |
+| [Electricity Load Diagrams](dataset_profiles/electricity_load_diagrams)          | Forecasting, Imputation                 |
+| [UCR & UEA Datasets](dataset_profiles/ucr_uea_datasets) (all 163 datasets)       | Classification                          |
+| [Vessel AIS](dataset_profiles/vessel_ais)                                        | Classification, Forecasting, Imputation |
 
 
 ## ❖ Citing TSDB/PyPOTS
-<a href='https://github.com/WenjieDu/PyPOTS'><img src='https://raw.githubusercontent.com/WenjieDu/PyPOTS/main/docs/_static/figs/PyPOTS_logo.svg?sanitize=true' width='160' align='left' /></a>
-TSDB is a part of [PyPOTS project](https://github.com/WenjieDu/PyPOTS) (a Python toolbox for data mining on Partially-Observed Time Series), and was separated from PyPOTS for decoupling datasets from learning algorithms.
-
 The paper introducing PyPOTS project is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
 and we are pursuing to publish it in prestigious academic venues, e.g. JMLR (track for
 [Machine Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use TSDB in your work,
 please cite PyPOTS project as below and 🌟star this repository to make others notice this library. 🤗 Thank you!
 
 ``` bibtex
 @article{du2023PyPOTS,
```

#### html2text {}

```diff
@@ -1,88 +1,91 @@
-Metadata-Version: 2.1 Name: tsdb Version: 0.0.9 Summary: TSDB (Time-Series
+Metadata-Version: 2.1 Name: tsdb Version: 0.1 Summary: TSDB (Time-Series
 DataBase): A Python Toolbox Helping Load Open-Source Time-Series Datasets Home-
 page: https://github.com/WenjieDu/TSDB Author: Wenjie Du Author-email:
 wenjay.du@gmail.com License: GPL-3.0 Project-URL: Documentation, https://
 tsdb.readthedocs.io/ Project-URL: Source, https://github.com/WenjieDu/TSDB/
 Project-URL: Tracker, https://github.com/WenjieDu/TSDB/issues/ Project-URL:
-Download, https://github.com/WenjieDu/TSDB/archive/main.zip Keywords: time-
-series analysis,time series,time-series database,time-series
-datasets,datasets,database,dataset downloading,data mining Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Education Classifier: Intended
-Audience :: Science/Research Classifier: License :: OSI Approved :: GNU General
-Public License v3 (GPLv3) Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Topic :: Database
-Description-Content-Type: text/markdown Provides-Extra: basic License-File:
-LICENSE [https://raw.githubusercontent.com/WenjieDu/TSDB/main/docs/_static/
-figs/TSDB_logo.svg?sanitize=true] #
+Download, https://github.com/WenjieDu/TSDB/archive/main.zip Keywords: data
+mining,time series,time-series analysis,time-series database,time-series
+datasets,database,datasets,dataset
+downloading,imputation,classification,forecasting Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: GNU General Public
+License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Topic :: Database Description-
+Content-Type: text/markdown Provides-Extra: basic License-File: LICENSE [https:
+//raw.githubusercontent.com/PyPOTS/pypots.github.io/main/static/figs/
+pypots_logos/TSDB_logo_FFBG.svg?sanitize=truee] #
                                 Welcome to TSDB
 **
        A Python Toolbox to Ease Loading Open-Source Time-Series Datasets
 **
  [https://img.shields.io/badge/python-v3-E97040?logo=python&logoColor=white]
   [PyPI]  [GPL-v3_license]  [https://img.shields.io/github/actions/workflow/
  status/wenjiedu/tsdb/testing_ci.yml?logo=github&color=C8D8E1&label=CI] [Code
   Climate_maintainability]  [https://img.shields.io/coverallsCoverage/github/
  WenjieDu/TSDB?branch=main&logo=coveralls&color=75C1C4&label=Coverage] [Conda
            downloads]  [https://static.pepy.tech/personalized-badge/
 tsdb?period=total&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20Downloads]
-> ð£ TSDB now supports a total of 1ï¸â£6ï¸â£5ï¸â£ time-series datasets
-â¼ï¸ TSDB is created to help researchers and engineers get rid of data
-collecting and downloading, and focus back on data processing details. TSDB
-provides all-in-one-stop convenience for downloading and loading open-source
-time-series datasets (available datasets listed [below](https://github.com/
-WenjieDu/TSDB#-list-of-available-datasets)). âï¸Please note that due to
-people have very different requirements for data processing, data-loading
-functions in TSDB only contain the most general steps (e.g. removing invalid
-samples) and won't process the data (not even normalize it). So, no worries,
-TSDB won't affect your data preprocessing. If you only want the raw datasets,
-TSDB can help you download and save raw datasets as well (take a look at [Usage
-Examples](https://github.com/WenjieDu/TSDB#-usage-example) below). ð¤ If you
-need TSDB to integrate an open-source dataset or want to add it into TSDB
-yourself, please feel free to request for it by creating an issue or make a PR
-to merge your code. ð¤ **Please** star this repo to help others notice TSDB
-if you think it is a useful toolkit. **Please** properly [cite TSDB](https://
-github.com/WenjieDu/TSDB#-citing-tsdbpypots) in your publications if it helps
-with your research. This really means a lot to our open-source research. Thank
-you! ## â Usage Examples TSDB now is available on [https://img.shields.io/
-badge/Anaconda--lightgreen?style=social&logo=anaconda]âï¸ Install it with
-`conda install tsdb`, you may need to specify the channel with option `-
-c conda-forge` or install from PyPI: > pip install tsdb or install from source
-code: > pip install `https://github.com/WenjieDu/TSDB/archive/main.zip`
-```python import tsdb tsdb.list_available_datasets() # list all available
-datasets in TSDB data = tsdb.load_dataset('physionet_2012') # select the
-dataset you need and load it, TSDB will download, extract, and process it
-automatically tsdb.download_and_extract('physionet_2012', './save_it_here') #
-if you need the raw data, use download_and_extract() tsdb.list_cached_data() #
-datasets you once loaded are cached, and you can check them with
-list_cached_data() tsdb.delete_cached_data() # you can delete all cache with
-delete_cached_data() to free disk space tsdb.delete_cached_data
-(dataset_name='physionet_2012') # or you can delete only one specific dataset
-and preserve others ``` That's all. Simple and efficient. Enjoy it! ð ## â
-List of Available Datasets | Name | Main Tasks | |-----------------------------
-------------------------------------------|------------------------------------
------| | [PhysioNet Challenge 2012](datasets/PhysioNet-2012) | Classification,
-Forecasting, Imputation | | [PhysioNet Challenge 2019](datasets/PhysioNet-2019)
-| Classification, Imputation | | [Beijing Multi-Site Air-Quality](datasets/
-BeijingMultiSiteAirQuality) | Forecasting, Imputation | | [Electricity Load
-Diagrams](datasets/ElectricityLoadDiagrams) | Forecasting, Imputation | | [UCR
-& UEA Datasets](datasets/UCR_UEA_Datasets) (all 160 datasets) | Classification
-| | [Vessel AIS](datasets/Vessel_AIS) | Classification, Forecasting, Imputation
-| ## â Citing TSDB/PyPOTS [https://raw.githubusercontent.com/WenjieDu/PyPOTS/
-main/docs/_static/figs/PyPOTS_logo.svg?sanitize=true] TSDB is a part of [PyPOTS
+> ð£ TSDB now supports a total of 1ï¸â£6ï¸â£8ï¸â£ time-series datasets
+â¼ï¸ [https://raw.githubusercontent.com/PyPOTS/pypots.github.io/main/static/
+figs/pypots_logos/PyPOTS_logo_FFBG.svg?sanitize=true] TSDB is a part of [PyPOTS
 project](https://github.com/WenjieDu/PyPOTS) (a Python toolbox for data mining
 on Partially-Observed Time Series), and was separated from PyPOTS for
-decoupling datasets from learning algorithms. The paper introducing PyPOTS
-project is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
-and we are pursuing to publish it in prestigious academic venues, e.g. JMLR
-(track for [Machine Learning Open Source Software](https://www.jmlr.org/mloss/
-)). If you use TSDB in your work, please cite PyPOTS project as below and
-ðstar this repository to make others notice this library. ð¤ Thank you!
-``` bibtex @article{du2023PyPOTS, title={{PyPOTS: A Python Toolbox for Data
-Mining on Partially-Observed Time Series}}, author={Wenjie Du}, year={2023},
-eprint={2305.18811}, archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://
-arxiv.org/abs/2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` or > Wenjie
-Du. (2023). > PyPOTS: A Python Toolbox for Data Mining on Partially-Observed
-Time Series. > arXiv, abs/2305.18811. https://doi.org/10.48550/arXiv.2305.18811
-ð  Visits [https://hits.seeyoufarm.com/api/count/incr/
+decoupling datasets from learning algorithms. TSDB is created to help
+researchers and engineers get rid of data collecting and downloading, and focus
+back on data processing details. TSDB provides all-in-one-stop convenience for
+downloading and loading open-source time-series datasets (available datasets
+listed [below](https://github.com/WenjieDu/TSDB#-list-of-available-datasets)).
+âï¸Please note that due to people have very different requirements for data
+processing, data-loading functions in TSDB only contain the most general steps
+(e.g. removing invalid samples) and won't process the data (not even normalize
+it). So, no worries, TSDB won't affect your data preprocessing. If you only
+want the raw datasets, TSDB can help you download and save raw datasets as well
+(take a look at [Usage Examples](https://github.com/WenjieDu/TSDB#-usage-
+example) below). ð¤ If you need TSDB to integrate an open-source dataset or
+want to add it into TSDB yourself, please feel free to request for it by
+creating an issue or make a PR to merge your code. ð¤ **Please** star this
+repo to help others notice TSDB if you think it is a useful toolkit. **Please**
+properly [cite TSDB](https://github.com/WenjieDu/TSDB#-citing-tsdbpypots) in
+your publications if it helps with your research. This really means a lot to
+our open-source research. Thank you! ## â Usage Examples TSDB now is
+available on [https://img.shields.io/badge/Anaconda--
+lightgreen?style=social&logo=anaconda]âï¸ Install it with `conda install
+tsdb`, you may need to specify the channel with option `-c conda-forge` or
+install from PyPI: > pip install tsdb or install from source code: > pip
+install `https://github.com/WenjieDu/TSDB/archive/main.zip` ```python import
+tsdb tsdb.list_available_datasets() # list all available datasets in TSDB data
+= tsdb.load_dataset('physionet_2012') # select the dataset you need and load
+it, TSDB will download, extract, and process it automatically
+tsdb.download_and_extract('physionet_2012', './save_it_here') # if you need the
+raw data, use download_and_extract() tsdb.list_cached_data() # datasets you
+once loaded are cached, and you can check them with list_cached_data()
+tsdb.delete_cached_data(dataset_name='physionet_2012') # you can delete only
+one specific dataset and preserve others tsdb.delete_cached_data() # or you can
+delete all cache with delete_cached_data() to free disk space ``` That's all.
+Simple and efficient. Enjoy it! ð ## â List of Available Datasets | Name |
+Main Tasks | |-----------------------------------------------------------------
+-----------------|-----------------------------------------| | [PhysioNet
+Challenge 2012](dataset_profiles/physionet_2012) | Classification, Forecasting,
+Imputation | | [PhysioNet Challenge 2019](dataset_profiles/physionet_2019) |
+Classification, Imputation | | [Beijing Multi-Site Air-Quality]
+(dataset_profiles/beijing_multisite_air_quality) | Forecasting, Imputation | |
+[Electricity Load Diagrams](dataset_profiles/electricity_load_diagrams) |
+Forecasting, Imputation | | [UCR & UEA Datasets](dataset_profiles/
+ucr_uea_datasets) (all 163 datasets) | Classification | | [Vessel AIS]
+(dataset_profiles/vessel_ais) | Classification, Forecasting, Imputation | ##
+â Citing TSDB/PyPOTS The paper introducing PyPOTS project is available on
+arXiv at [this URL](https://arxiv.org/abs/2305.18811), and we are pursuing to
+publish it in prestigious academic venues, e.g. JMLR (track for [Machine
+Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use TSDB
+in your work, please cite PyPOTS project as below and ðstar this repository
+to make others notice this library. ð¤ Thank you! ``` bibtex @article
+{du2023PyPOTS, title={{PyPOTS: A Python Toolbox for Data Mining on Partially-
+Observed Time Series}}, author={Wenjie Du}, year={2023}, eprint={2305.18811},
+archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://arxiv.org/abs/
+2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` or > Wenjie Du. (2023). >
+PyPOTS: A Python Toolbox for Data Mining on Partially-Observed Time Series. >
+arXiv, abs/2305.18811. https://doi.org/10.48550/arXiv.2305.18811  ð  Visits
+[https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FWenjieDu%2FTime_Series_Database&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+April+2022&edge_flat=false]
```

