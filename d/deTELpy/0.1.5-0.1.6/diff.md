# Comparing `tmp/deTELpy-0.1.5.tar.gz` & `tmp/deTELpy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deTELpy-0.1.5.tar", last modified: Mon Aug  7 14:44:11 2023, max compression
+gzip compressed data, was "dist/deTELpy-0.1.6.tar", last modified: Tue Aug  8 12:35:13 2023, max compression
```

## Comparing `deTELpy-0.1.5.tar` & `deTELpy-0.1.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-07 14:44:11.000000 deTELpy-0.1.5/
--rw-r--r--   0 moon       (502) staff       (20)        0 2023-08-04 09:12:13.000000 deTELpy-0.1.5/LICENSE
--rw-r--r--   0 moon       (502) staff       (20)    11684 2023-08-07 14:44:11.000000 deTELpy-0.1.5/PKG-INFO
--rw-r--r--   0 moon       (502) staff       (20)    11046 2023-08-07 14:11:48.000000 deTELpy-0.1.5/README.md
-drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-07 14:44:11.000000 deTELpy-0.1.5/deTEL/
--rw-r--r--   0 moon       (502) staff       (20)      223 2023-08-07 14:00:52.000000 deTELpy-0.1.5/deTEL/__init__.py
--rw-r--r--   0 moon       (502) staff       (20)      639 2023-08-07 13:59:54.000000 deTELpy-0.1.5/deTEL/__main__.py
-drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-07 14:44:11.000000 deTELpy-0.1.5/deTEL/eTEL/
--rw-r--r--   0 moon       (502) staff       (20)       19 2023-08-07 08:29:19.000000 deTELpy-0.1.5/deTEL/eTEL/__init__.py
--rw-r--r--   0 moon       (502) staff       (20)    17304 2023-08-04 08:39:43.000000 deTELpy-0.1.5/deTEL/eTEL/danger_mods.csv
--rw-r--r--   0 moon       (502) staff       (20)     4579 2023-08-04 08:39:43.000000 deTELpy-0.1.5/deTEL/eTEL/dataset_report.py
--rw-r--r--   0 moon       (502) staff       (20)    17922 2023-08-07 12:16:03.000000 deTELpy-0.1.5/deTEL/eTEL/eTEL.py
--rw-r--r--   0 moon       (502) staff       (20)     2380 2023-08-04 08:39:43.000000 deTELpy-0.1.5/deTEL/eTEL/extract_peptides.py
--rw-r--r--   0 moon       (502) staff       (20)    18799 2023-08-04 08:39:43.000000 deTELpy-0.1.5/deTEL/eTEL/global_report.py
--rw-r--r--   0 moon       (502) staff       (20)     3567 2023-08-04 08:39:43.000000 deTELpy-0.1.5/deTEL/eTEL/substitution_report.py
--rw-r--r--   0 moon       (502) staff       (20)    22110 2023-08-04 08:39:43.000000 deTELpy-0.1.5/deTEL/eTEL/toolbox.py
-drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-07 14:44:11.000000 deTELpy-0.1.5/deTEL/mTEL/
--rw-r--r--   0 moon       (502) staff       (20)       43 2023-08-07 08:29:19.000000 deTELpy-0.1.5/deTEL/mTEL/__init__.py
--rw-r--r--   0 moon       (502) staff       (20)     6522 2023-08-04 08:39:43.000000 deTELpy-0.1.5/deTEL/mTEL/data.py
--rw-r--r--   0 moon       (502) staff       (20)    10757 2023-08-07 12:16:03.000000 deTELpy-0.1.5/deTEL/mTEL/mTEL.py
--rw-r--r--   0 moon       (502) staff       (20)     8312 2023-08-04 12:27:10.000000 deTELpy-0.1.5/deTEL/mTEL/mcmc.py
--rw-r--r--   0 moon       (502) staff       (20)    20613 2023-08-04 12:13:33.000000 deTELpy-0.1.5/deTEL/mTEL/mtem.py
-drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-07 14:44:11.000000 deTELpy-0.1.5/deTEL/utility/
--rw-r--r--   0 moon       (502) staff       (20)     1100 2023-08-04 08:39:43.000000 deTELpy-0.1.5/deTEL/utility/downloadPRIDE.py
--rw-r--r--   0 moon       (502) staff       (20)     3279 2023-08-04 08:39:43.000000 deTELpy-0.1.5/deTEL/utility/prideCrawler.py
-drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-07 14:44:11.000000 deTELpy-0.1.5/deTELpy.egg-info/
--rw-r--r--   0 moon       (502) staff       (20)    11684 2023-08-07 14:44:11.000000 deTELpy-0.1.5/deTELpy.egg-info/PKG-INFO
--rw-r--r--   0 moon       (502) staff       (20)      895 2023-08-07 14:44:11.000000 deTELpy-0.1.5/deTELpy.egg-info/SOURCES.txt
--rw-r--r--   0 moon       (502) staff       (20)        1 2023-08-07 14:44:11.000000 deTELpy-0.1.5/deTELpy.egg-info/dependency_links.txt
--rw-r--r--   0 moon       (502) staff       (20)      171 2023-08-07 14:44:11.000000 deTELpy-0.1.5/deTELpy.egg-info/requires.txt
--rw-r--r--   0 moon       (502) staff       (20)        6 2023-08-07 14:44:11.000000 deTELpy-0.1.5/deTELpy.egg-info/top_level.txt
-drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-07 14:44:11.000000 deTELpy-0.1.5/eTEL/
-drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-07 14:44:11.000000 deTELpy-0.1.5/eTEL/workflow/
--rw-r--r--   0 moon       (502) staff       (20)     4579 2023-08-04 08:39:43.000000 deTELpy-0.1.5/eTEL/workflow/dataset_report.py
--rw-r--r--   0 moon       (502) staff       (20)    17922 2023-08-07 12:16:03.000000 deTELpy-0.1.5/eTEL/workflow/eTEL.py
--rw-r--r--   0 moon       (502) staff       (20)     2380 2023-08-04 08:39:43.000000 deTELpy-0.1.5/eTEL/workflow/extract_peptides.py
--rw-r--r--   0 moon       (502) staff       (20)    18799 2023-08-04 08:39:43.000000 deTELpy-0.1.5/eTEL/workflow/global_report.py
--rw-r--r--   0 moon       (502) staff       (20)     3567 2023-08-04 08:39:43.000000 deTELpy-0.1.5/eTEL/workflow/substitution_report.py
--rw-r--r--   0 moon       (502) staff       (20)    22110 2023-08-04 08:39:43.000000 deTELpy-0.1.5/eTEL/workflow/toolbox.py
-drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-07 14:44:11.000000 deTELpy-0.1.5/mTEL/
--rw-r--r--   0 moon       (502) staff       (20)     6522 2023-08-04 08:39:43.000000 deTELpy-0.1.5/mTEL/data.py
--rw-r--r--   0 moon       (502) staff       (20)    10757 2023-08-07 12:16:03.000000 deTELpy-0.1.5/mTEL/mTEL.py
--rw-r--r--   0 moon       (502) staff       (20)     8312 2023-08-04 12:27:10.000000 deTELpy-0.1.5/mTEL/mcmc.py
--rw-r--r--   0 moon       (502) staff       (20)    20613 2023-08-04 12:13:33.000000 deTELpy-0.1.5/mTEL/mtem.py
--rw-r--r--   0 moon       (502) staff       (20)       38 2023-08-07 14:44:11.000000 deTELpy-0.1.5/setup.cfg
--rw-r--r--   0 moon       (502) staff       (20)     1504 2023-08-07 14:43:59.000000 deTELpy-0.1.5/setup.py
-drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-07 14:44:11.000000 deTELpy-0.1.5/tests/
--rw-r--r--   0 moon       (502) staff       (20)      560 2023-08-07 09:25:07.000000 deTELpy-0.1.5/tests/test_run_deTEL.py
-drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-07 14:44:11.000000 deTELpy-0.1.5/utility/
--rw-r--r--   0 moon       (502) staff       (20)     1100 2023-08-04 08:39:43.000000 deTELpy-0.1.5/utility/downloadPRIDE.py
--rw-r--r--   0 moon       (502) staff       (20)     3279 2023-08-04 08:39:43.000000 deTELpy-0.1.5/utility/prideCrawler.py
+drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-08 12:35:13.000000 deTELpy-0.1.6/
+-rw-r--r--   0 moon       (502) staff       (20)     1536 2023-08-07 14:49:24.000000 deTELpy-0.1.6/LICENSE
+-rw-r--r--   0 moon       (502) staff       (20)    12043 2023-08-08 12:35:13.000000 deTELpy-0.1.6/PKG-INFO
+-rw-r--r--   0 moon       (502) staff       (20)    11414 2023-08-08 10:47:03.000000 deTELpy-0.1.6/README.md
+drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-08 12:35:13.000000 deTELpy-0.1.6/deTEL/
+-rw-r--r--   0 moon       (502) staff       (20)      223 2023-08-07 14:00:52.000000 deTELpy-0.1.6/deTEL/__init__.py
+-rw-r--r--   0 moon       (502) staff       (20)     6037 2023-08-08 12:33:57.000000 deTELpy-0.1.6/deTEL/__main__.py
+drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-08 12:35:13.000000 deTELpy-0.1.6/deTEL/eTEL/
+-rw-r--r--   0 moon       (502) staff       (20)       19 2023-08-07 08:29:19.000000 deTELpy-0.1.6/deTEL/eTEL/__init__.py
+-rw-r--r--   0 moon       (502) staff       (20)    17304 2023-08-04 08:39:43.000000 deTELpy-0.1.6/deTEL/eTEL/danger_mods.csv
+-rw-r--r--   0 moon       (502) staff       (20)     4579 2023-08-04 08:39:43.000000 deTELpy-0.1.6/deTEL/eTEL/dataset_report.py
+-rw-r--r--   0 moon       (502) staff       (20)    17922 2023-08-07 12:16:03.000000 deTELpy-0.1.6/deTEL/eTEL/eTEL.py
+-rw-r--r--   0 moon       (502) staff       (20)     2380 2023-08-04 08:39:43.000000 deTELpy-0.1.6/deTEL/eTEL/extract_peptides.py
+-rw-r--r--   0 moon       (502) staff       (20)    18799 2023-08-04 08:39:43.000000 deTELpy-0.1.6/deTEL/eTEL/global_report.py
+-rw-r--r--   0 moon       (502) staff       (20)     3567 2023-08-04 08:39:43.000000 deTELpy-0.1.6/deTEL/eTEL/substitution_report.py
+-rw-r--r--   0 moon       (502) staff       (20)    22110 2023-08-04 08:39:43.000000 deTELpy-0.1.6/deTEL/eTEL/toolbox.py
+drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-08 12:35:13.000000 deTELpy-0.1.6/deTEL/mTEL/
+-rw-r--r--   0 moon       (502) staff       (20)       43 2023-08-07 08:29:19.000000 deTELpy-0.1.6/deTEL/mTEL/__init__.py
+-rw-r--r--   0 moon       (502) staff       (20)     6522 2023-08-04 08:39:43.000000 deTELpy-0.1.6/deTEL/mTEL/data.py
+-rw-r--r--   0 moon       (502) staff       (20)    11959 2023-08-08 09:02:27.000000 deTELpy-0.1.6/deTEL/mTEL/mTEL.py
+-rw-r--r--   0 moon       (502) staff       (20)     8552 2023-08-08 12:29:25.000000 deTELpy-0.1.6/deTEL/mTEL/mcmc.py
+-rw-r--r--   0 moon       (502) staff       (20)    20613 2023-08-04 12:13:33.000000 deTELpy-0.1.6/deTEL/mTEL/mtem.py
+drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-08 12:35:13.000000 deTELpy-0.1.6/deTEL/utility/
+-rw-r--r--   0 moon       (502) staff       (20)     1100 2023-08-04 08:39:43.000000 deTELpy-0.1.6/deTEL/utility/downloadPRIDE.py
+-rw-r--r--   0 moon       (502) staff       (20)     3279 2023-08-04 08:39:43.000000 deTELpy-0.1.6/deTEL/utility/prideCrawler.py
+drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-08 12:35:13.000000 deTELpy-0.1.6/deTELpy.egg-info/
+-rw-r--r--   0 moon       (502) staff       (20)    12043 2023-08-08 12:35:13.000000 deTELpy-0.1.6/deTELpy.egg-info/PKG-INFO
+-rw-r--r--   0 moon       (502) staff       (20)      895 2023-08-08 12:35:13.000000 deTELpy-0.1.6/deTELpy.egg-info/SOURCES.txt
+-rw-r--r--   0 moon       (502) staff       (20)        1 2023-08-08 12:35:13.000000 deTELpy-0.1.6/deTELpy.egg-info/dependency_links.txt
+-rw-r--r--   0 moon       (502) staff       (20)      171 2023-08-08 12:35:13.000000 deTELpy-0.1.6/deTELpy.egg-info/requires.txt
+-rw-r--r--   0 moon       (502) staff       (20)        6 2023-08-08 12:35:13.000000 deTELpy-0.1.6/deTELpy.egg-info/top_level.txt
+drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-08 12:35:13.000000 deTELpy-0.1.6/eTEL/
+drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-08 12:35:13.000000 deTELpy-0.1.6/eTEL/workflow/
+-rw-r--r--   0 moon       (502) staff       (20)     4579 2023-08-04 08:39:43.000000 deTELpy-0.1.6/eTEL/workflow/dataset_report.py
+-rw-r--r--   0 moon       (502) staff       (20)    17922 2023-08-07 12:16:03.000000 deTELpy-0.1.6/eTEL/workflow/eTEL.py
+-rw-r--r--   0 moon       (502) staff       (20)     2380 2023-08-04 08:39:43.000000 deTELpy-0.1.6/eTEL/workflow/extract_peptides.py
+-rw-r--r--   0 moon       (502) staff       (20)    18799 2023-08-04 08:39:43.000000 deTELpy-0.1.6/eTEL/workflow/global_report.py
+-rw-r--r--   0 moon       (502) staff       (20)     3567 2023-08-04 08:39:43.000000 deTELpy-0.1.6/eTEL/workflow/substitution_report.py
+-rw-r--r--   0 moon       (502) staff       (20)    22110 2023-08-04 08:39:43.000000 deTELpy-0.1.6/eTEL/workflow/toolbox.py
+drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-08 12:35:13.000000 deTELpy-0.1.6/mTEL/
+-rw-r--r--   0 moon       (502) staff       (20)     6522 2023-08-04 08:39:43.000000 deTELpy-0.1.6/mTEL/data.py
+-rw-r--r--   0 moon       (502) staff       (20)    11959 2023-08-08 09:02:27.000000 deTELpy-0.1.6/mTEL/mTEL.py
+-rw-r--r--   0 moon       (502) staff       (20)     8552 2023-08-08 12:29:25.000000 deTELpy-0.1.6/mTEL/mcmc.py
+-rw-r--r--   0 moon       (502) staff       (20)    20613 2023-08-04 12:13:33.000000 deTELpy-0.1.6/mTEL/mtem.py
+-rw-r--r--   0 moon       (502) staff       (20)       38 2023-08-08 12:35:13.000000 deTELpy-0.1.6/setup.cfg
+-rw-r--r--   0 moon       (502) staff       (20)     1495 2023-08-08 12:34:31.000000 deTELpy-0.1.6/setup.py
+drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-08 12:35:13.000000 deTELpy-0.1.6/tests/
+-rw-r--r--   0 moon       (502) staff       (20)      560 2023-08-08 10:42:58.000000 deTELpy-0.1.6/tests/test_run_deTEL.py
+drwxr-xr-x   0 moon       (502) staff       (20)        0 2023-08-08 12:35:13.000000 deTELpy-0.1.6/utility/
+-rw-r--r--   0 moon       (502) staff       (20)     1100 2023-08-04 08:39:43.000000 deTELpy-0.1.6/utility/downloadPRIDE.py
+-rw-r--r--   0 moon       (502) staff       (20)     3279 2023-08-04 08:39:43.000000 deTELpy-0.1.6/utility/prideCrawler.py
```

### Comparing `deTELpy-0.1.5/PKG-INFO` & `deTELpy-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: deTELpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package of the deTEL translation error detection pipeline from mass-spectrometry data
 Home-page: https://git.mpi-cbg.de/atplab/detelpy
 Author: Cedric Landerer
 Author-email: landerer@mpi-cbg.de
-License: BSD 2-clause
+License: BSD
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
@@ -40,17 +40,21 @@
 eTEL detects translation errors in mass-spectrometry data and explores the empirical translation error landscape.
 mTEL is a model fitted to the translation errors detected by eTEL and describes the multinomial translation error landscape and extends the empirical translation error landscape.
 
 ## deTEL Python package
 ```bash
 pip install deTELpy
 
-python -m deTEL mTEL # To run mTEL
+python -m deTEL # To run eTEL/mTEL with GUI
 
-python -m deTEL eTEL # To run eTEL
+# To run eTEL with command line
+python -m deTEL eTEL -f tests/resources/s228c_orf_cds.fasta -psm tests/resources/psm.tsv -o tests/output -decoy rev_ -p substitutions -tol 0.005 -TEST -1
+
+# To run mTEL with command line
+python -m deTEL mTEL -f tests/resources/results_ionquant2 -r tests/resources/tRNA_count/yeast_tRNA_count.csv -o tests/output -s 250 -p 100 -c 4.2e-17 -t 10 -b 100 -nb -1 -a n
 ```
 
 # empirical Translation Error Landscape: eTEL 
 ![empirical Translation Error Landscape (eTEL)](img/eTEL.png)
 eTEL detects the empirical translation error landscape by first performing an open search using MSFragger [(see: Perform open search)](#perform-open-search-with-fragger_open_search).
 The second step is to extract translation errors using custom pythons scripts packaged [(see: detect_substitutions)](#detect_substitutions).
 The output of eTEL can directly be used to fit the mTEL model [(see: multinomial Translation Error Landscape: mTEL)](#multinomial-translation-error-landscape-mtel).
```

### Comparing `deTELpy-0.1.5/README.md` & `deTELpy-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,21 @@
 eTEL detects translation errors in mass-spectrometry data and explores the empirical translation error landscape.
 mTEL is a model fitted to the translation errors detected by eTEL and describes the multinomial translation error landscape and extends the empirical translation error landscape.
 
 ## deTEL Python package
 ```bash
 pip install deTELpy
 
-python -m deTEL mTEL # To run mTEL
+python -m deTEL # To run eTEL/mTEL with GUI
 
-python -m deTEL eTEL # To run eTEL
+# To run eTEL with command line
+python -m deTEL eTEL -f tests/resources/s228c_orf_cds.fasta -psm tests/resources/psm.tsv -o tests/output -decoy rev_ -p substitutions -tol 0.005 -TEST -1
+
+# To run mTEL with command line
+python -m deTEL mTEL -f tests/resources/results_ionquant2 -r tests/resources/tRNA_count/yeast_tRNA_count.csv -o tests/output -s 250 -p 100 -c 4.2e-17 -t 10 -b 100 -nb -1 -a n
 ```
 
 # empirical Translation Error Landscape: eTEL 
 ![empirical Translation Error Landscape (eTEL)](img/eTEL.png)
 eTEL detects the empirical translation error landscape by first performing an open search using MSFragger [(see: Perform open search)](#perform-open-search-with-fragger_open_search).
 The second step is to extract translation errors using custom pythons scripts packaged [(see: detect_substitutions)](#detect_substitutions).
 The output of eTEL can directly be used to fit the mTEL model [(see: multinomial Translation Error Landscape: mTEL)](#multinomial-translation-error-landscape-mtel).
```

### Comparing `deTELpy-0.1.5/deTEL/eTEL/danger_mods.csv` & `deTELpy-0.1.6/deTEL/eTEL/danger_mods.csv`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/deTEL/eTEL/dataset_report.py` & `deTELpy-0.1.6/deTEL/eTEL/dataset_report.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/deTEL/eTEL/eTEL.py` & `deTELpy-0.1.6/deTEL/eTEL/eTEL.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/deTEL/eTEL/extract_peptides.py` & `deTELpy-0.1.6/deTEL/eTEL/extract_peptides.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/deTEL/eTEL/global_report.py` & `deTELpy-0.1.6/deTEL/eTEL/global_report.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/deTEL/eTEL/substitution_report.py` & `deTELpy-0.1.6/deTEL/eTEL/substitution_report.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/deTEL/eTEL/toolbox.py` & `deTELpy-0.1.6/deTEL/eTEL/toolbox.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/deTEL/mTEL/data.py` & `deTELpy-0.1.6/deTEL/mTEL/data.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/deTEL/mTEL/mTEL.py` & `deTELpy-0.1.6/deTEL/mTEL/mTEL.py`

 * *Files 11% similar despite different names*

```diff
@@ -182,35 +182,70 @@
         # store fitted energies
         df = pd.DataFrame(index=model.CODONS, columns=model.CODONS)
         for codon in model.CODONS:
             df[codon] = model.calculate_detection_parameter(model.CODONS, codon, ppp_mean, wp)
         df.to_csv(os.path.join(args.output_folder, f"fitted_energies_{out_suffix}.csv"))
 
 
-@Gooey(program_name='mTEL', default_size=(610, 700))
+from wx.core import wx
+is_dark = wx.SystemSettings.GetAppearance().IsUsingDarkBackground()
+
+print(is_dark)
+
+bg_color = '#343434' if is_dark else '#eeeeee'
+wbg_color = '#262626' if is_dark else '#ffffff'
+fg_color = '#eeeeee' if is_dark else '#000000'
+
+item_default = {
+    'error_color': '#ea7878',
+    'label_color': fg_color,
+    'help_color': fg_color,
+    'full_width': False,
+    'validator': {
+        'type': 'local',
+        'test': 'lambda x: True',
+        'message': ''
+    },
+    'external_validator': {
+        'cmd': '',
+    }
+}
+
+@Gooey(program_name='mTEL',
+       default_size=(610, 700),
+       terminal_panel_color=bg_color,
+       terminal_font_color=fg_color,
+       body_bg_color=bg_color,
+       header_bg_color=wbg_color,
+       footer_bg_color=bg_color,
+       sidebar_bg_color=bg_color,)
 def main(args):
     parser = GooeyParser(
         description="mTEL uses observed translation errors \nto estimate a multinomial translation error landscape.")
+
+    for group in parser.parser._action_groups:
+        group.gooey_options = {'label_color': fg_color, 'description_color': fg_color}
+
     parser.add_argument("-f", dest="all_files", required=True, help="Folder with codon_count and error files",
-                        metavar="FILE", type=lambda x: is_valid_file(parser, x), widget="DirChooser")
+                        metavar="FILE", type=lambda x: is_valid_file(parser, x), widget="DirChooser", gooey_options=item_default)
     parser.add_argument("-r", dest="trna_count", required=True, help="tRNA count file", metavar="FILE",
-                        type=lambda x: is_valid_file(parser, x), widget="FileChooser")
+                        type=lambda x: is_valid_file(parser, x), widget="FileChooser", gooey_options=item_default)
     parser.add_argument("-o", dest="output_folder", required=True, help="Output folder", metavar="FILE",
-                        type=lambda x: prep_folder(x), widget="DirChooser")
-    parser.add_argument("-s", dest="samples", required=True, type=int, help="Number of samples")
-    parser.add_argument("-p", dest="post_samples", required=True, type=int, help="Posterior samples")
-    parser.add_argument("-c", dest="cell_vol", required=False, help="Cell Volume", type=float, default=4.2e-17)
-    parser.add_argument("-t", dest="thinning", required=False, help="Thinning", type=int, default=10)
-    parser.add_argument("-b", dest="burnin", required=False, help="Burn-in", type=int, default=100)
+                        type=lambda x: prep_folder(x), widget="DirChooser", gooey_options=item_default)
+    parser.add_argument("-s", dest="samples", required=True, type=int, help="Number of samples", gooey_options=item_default)
+    parser.add_argument("-p", dest="post_samples", required=True, type=int, help="Posterior samples", gooey_options=item_default)
+    parser.add_argument("-c", dest="cell_vol", required=False, help="Cell Volume", type=float, default=4.2e-17, gooey_options=item_default)
+    parser.add_argument("-t", dest="thinning", required=False, help="Thinning", type=int, default=10, gooey_options=item_default)
+    parser.add_argument("-b", dest="burnin", required=False, help="Burn-in", type=int, default=100, gooey_options=item_default)
     parser.add_argument("-nb", dest="num_bootsrap", required=False, help="Number of subsamples performed", type=int,
-                        default=-1)
+                        default=-1, gooey_options=item_default)
     parser.add_argument("-os", dest="out_suffix", required=False, help="suffix added to output files (default: date)",
-                        type=str, default="")
+                        type=str, default="", gooey_options=item_default)
     parser.add_argument("-a", dest="aggregate", required=False, type=str, default="n",
-                        help="aggregate all datasets by summation (y,n) Default: No (n)")
+                        help="aggregate all datasets by summation (y,n) Default: No (n)", gooey_options=item_default)
 
     args = parser.parse_args()
     run(args)
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `deTELpy-0.1.5/deTEL/mTEL/mcmc.py` & `deTELpy-0.1.6/deTEL/mTEL/mcmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,33 @@
+import io
+import time
 import sys
+from contextlib import redirect_stderr
 
 import matplotlib.pyplot as plt
 from tqdm import tqdm
 from dataclasses import dataclass, field
 
 import multiprocessing as mp
 import numpy as np
 
 from . import mtem
 from . import data
 
+
 # TODO change mtem to object that can be evaluated at a given parameter set in order to avoid passing model constants
 #  and data through the mcmc. This also allows to keep things cleaner in general
 
 @dataclass
 class MCMCstate:
     alpha: np.array = field(default_factory=np.array)  # position penalty
     beta: np.array = field(default_factory=np.array)  # nucleotide mismatching
     log_likelihood: float = 0.0
 
+
 @dataclass
 class MCMC:
     model: mtem.MTEM
 
     c_alpha: np.array = field(init=False)  # position penalty
     c_beta: np.array = field(init=False)  # nucleotide mismatching
 
@@ -123,23 +128,23 @@
             wobble_trace[i, :] = self.trace[i].beta
 
         return wobble_trace
 
     def position_penalty_posterior(self, samples):
         nsamples = len(self.trace)
         posterior = np.zeros(shape=(samples, self.trace[0].alpha.shape[0]))
-        for i, s in enumerate(range(nsamples-samples, nsamples)):
+        for i, s in enumerate(range(nsamples - samples, nsamples)):
             posterior[i, :] = self.trace[s].alpha
 
         return np.exp(posterior)
 
     def wobble_penalty_posterior(self, samples):
         nsamples = len(self.trace)
         posterior = np.zeros(shape=(samples, self.trace[0].beta.shape[0]))
-        for i, s in enumerate(range(nsamples-samples, nsamples)):
+        for i, s in enumerate(range(nsamples - samples, nsamples)):
             posterior[i, :] = self.trace[s].beta
 
         return posterior
 
     def likelihood_trace(self):
         t_len = len(self.trace)
         ll_trace = [0] * t_len
@@ -173,24 +178,28 @@
             reordered_data.append(d)
 
         return reordered_data
 
     def run(self, samples, thinning, burnin, ic_alpha, ic_beta, data):
         data = self.prepare_dataset(data)
 
-        iterations = (samples+burnin)*thinning
-        self.trace = samples*[MCMCstate]
+        iterations = (samples + burnin) * thinning
+        self.trace = samples * [MCMCstate]
 
         self.c_alpha = ic_alpha
         self.c_beta = ic_beta
         c_beta = self.model.format_wobble_penalties(self.c_beta)
         p = self.model.calculate_all_substitution_probabilities(np.exp(self.c_alpha), c_beta, combine_ile_leu=True)
         self.current_log_likelihood = self.log_likelihood(data, p)
         print('Initial log(likelihood): {}\n'.format(self.current_log_likelihood))
 
+        f = None
+        if not sys.stdin.isatty():
+            f = io.StringIO()
+
         for i in tqdm(range(0, iterations), file=sys.stdout):
             # Accept/Reject Position penalty
             self.p_alpha = self.propose(self.c_alpha, self.a_proposal_width)
             # forgetting this line caused a bug before. move it into the model itself?
             c_beta = self.model.format_wobble_penalties(self.c_beta)
             p = self.model.calculate_all_substitution_probabilities(np.exp(self.p_alpha), c_beta, combine_ile_leu=True)
             self.proposed_log_likelihood = self.log_likelihood(data, p)
@@ -204,15 +213,18 @@
             self.proposed_log_likelihood = self.log_likelihood(data, p)
             if self.accept_parameter_set(log_parameter=False):
                 self.update_beta()
 
             # ---- UPDATE TRACE ----
             if i / thinning >= burnin:
                 if i % thinning == 0:
-                    self.trace[int(i/thinning) - burnin] = MCMCstate(alpha=self.c_alpha, beta=self.c_beta,
-                                                                     log_likelihood=self.current_log_likelihood)
+                    self.trace[int(i / thinning) - burnin] = MCMCstate(alpha=self.c_alpha, beta=self.c_beta,
+                                                                       log_likelihood=self.current_log_likelihood)
 
             # ---- ADAPT PROPOSAL WIDTH ----
             if i != 0 and i % self.adaptive_width == 0:
                 self.update_proposal_width()
 
+            if f and i % 12 == 0:
+                print(end ='\n', flush=True)
+
         print('Final log(likelihood): {}\n'.format(self.current_log_likelihood))
```

### Comparing `deTELpy-0.1.5/deTEL/mTEL/mtem.py` & `deTELpy-0.1.6/deTEL/mTEL/mtem.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/deTEL/utility/downloadPRIDE.py` & `deTELpy-0.1.6/deTEL/utility/downloadPRIDE.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/deTEL/utility/prideCrawler.py` & `deTELpy-0.1.6/deTEL/utility/prideCrawler.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/deTELpy.egg-info/PKG-INFO` & `deTELpy-0.1.6/deTELpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: deTELpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package of the deTEL translation error detection pipeline from mass-spectrometry data
 Home-page: https://git.mpi-cbg.de/atplab/detelpy
 Author: Cedric Landerer
 Author-email: landerer@mpi-cbg.de
-License: BSD 2-clause
+License: BSD
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
@@ -40,17 +40,21 @@
 eTEL detects translation errors in mass-spectrometry data and explores the empirical translation error landscape.
 mTEL is a model fitted to the translation errors detected by eTEL and describes the multinomial translation error landscape and extends the empirical translation error landscape.
 
 ## deTEL Python package
 ```bash
 pip install deTELpy
 
-python -m deTEL mTEL # To run mTEL
+python -m deTEL # To run eTEL/mTEL with GUI
 
-python -m deTEL eTEL # To run eTEL
+# To run eTEL with command line
+python -m deTEL eTEL -f tests/resources/s228c_orf_cds.fasta -psm tests/resources/psm.tsv -o tests/output -decoy rev_ -p substitutions -tol 0.005 -TEST -1
+
+# To run mTEL with command line
+python -m deTEL mTEL -f tests/resources/results_ionquant2 -r tests/resources/tRNA_count/yeast_tRNA_count.csv -o tests/output -s 250 -p 100 -c 4.2e-17 -t 10 -b 100 -nb -1 -a n
 ```
 
 # empirical Translation Error Landscape: eTEL 
 ![empirical Translation Error Landscape (eTEL)](img/eTEL.png)
 eTEL detects the empirical translation error landscape by first performing an open search using MSFragger [(see: Perform open search)](#perform-open-search-with-fragger_open_search).
 The second step is to extract translation errors using custom pythons scripts packaged [(see: detect_substitutions)](#detect_substitutions).
 The output of eTEL can directly be used to fit the mTEL model [(see: multinomial Translation Error Landscape: mTEL)](#multinomial-translation-error-landscape-mtel).
```

### Comparing `deTELpy-0.1.5/deTELpy.egg-info/SOURCES.txt` & `deTELpy-0.1.6/deTELpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/eTEL/workflow/dataset_report.py` & `deTELpy-0.1.6/eTEL/workflow/dataset_report.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/eTEL/workflow/eTEL.py` & `deTELpy-0.1.6/eTEL/workflow/eTEL.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/eTEL/workflow/extract_peptides.py` & `deTELpy-0.1.6/eTEL/workflow/extract_peptides.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/eTEL/workflow/global_report.py` & `deTELpy-0.1.6/eTEL/workflow/global_report.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/eTEL/workflow/substitution_report.py` & `deTELpy-0.1.6/eTEL/workflow/substitution_report.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/eTEL/workflow/toolbox.py` & `deTELpy-0.1.6/eTEL/workflow/toolbox.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/mTEL/data.py` & `deTELpy-0.1.6/mTEL/data.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/mTEL/mTEL.py` & `deTELpy-0.1.6/mTEL/mTEL.py`

 * *Files 11% similar despite different names*

```diff
@@ -182,35 +182,70 @@
         # store fitted energies
         df = pd.DataFrame(index=model.CODONS, columns=model.CODONS)
         for codon in model.CODONS:
             df[codon] = model.calculate_detection_parameter(model.CODONS, codon, ppp_mean, wp)
         df.to_csv(os.path.join(args.output_folder, f"fitted_energies_{out_suffix}.csv"))
 
 
-@Gooey(program_name='mTEL', default_size=(610, 700))
+from wx.core import wx
+is_dark = wx.SystemSettings.GetAppearance().IsUsingDarkBackground()
+
+print(is_dark)
+
+bg_color = '#343434' if is_dark else '#eeeeee'
+wbg_color = '#262626' if is_dark else '#ffffff'
+fg_color = '#eeeeee' if is_dark else '#000000'
+
+item_default = {
+    'error_color': '#ea7878',
+    'label_color': fg_color,
+    'help_color': fg_color,
+    'full_width': False,
+    'validator': {
+        'type': 'local',
+        'test': 'lambda x: True',
+        'message': ''
+    },
+    'external_validator': {
+        'cmd': '',
+    }
+}
+
+@Gooey(program_name='mTEL',
+       default_size=(610, 700),
+       terminal_panel_color=bg_color,
+       terminal_font_color=fg_color,
+       body_bg_color=bg_color,
+       header_bg_color=wbg_color,
+       footer_bg_color=bg_color,
+       sidebar_bg_color=bg_color,)
 def main(args):
     parser = GooeyParser(
         description="mTEL uses observed translation errors \nto estimate a multinomial translation error landscape.")
+
+    for group in parser.parser._action_groups:
+        group.gooey_options = {'label_color': fg_color, 'description_color': fg_color}
+
     parser.add_argument("-f", dest="all_files", required=True, help="Folder with codon_count and error files",
-                        metavar="FILE", type=lambda x: is_valid_file(parser, x), widget="DirChooser")
+                        metavar="FILE", type=lambda x: is_valid_file(parser, x), widget="DirChooser", gooey_options=item_default)
     parser.add_argument("-r", dest="trna_count", required=True, help="tRNA count file", metavar="FILE",
-                        type=lambda x: is_valid_file(parser, x), widget="FileChooser")
+                        type=lambda x: is_valid_file(parser, x), widget="FileChooser", gooey_options=item_default)
     parser.add_argument("-o", dest="output_folder", required=True, help="Output folder", metavar="FILE",
-                        type=lambda x: prep_folder(x), widget="DirChooser")
-    parser.add_argument("-s", dest="samples", required=True, type=int, help="Number of samples")
-    parser.add_argument("-p", dest="post_samples", required=True, type=int, help="Posterior samples")
-    parser.add_argument("-c", dest="cell_vol", required=False, help="Cell Volume", type=float, default=4.2e-17)
-    parser.add_argument("-t", dest="thinning", required=False, help="Thinning", type=int, default=10)
-    parser.add_argument("-b", dest="burnin", required=False, help="Burn-in", type=int, default=100)
+                        type=lambda x: prep_folder(x), widget="DirChooser", gooey_options=item_default)
+    parser.add_argument("-s", dest="samples", required=True, type=int, help="Number of samples", gooey_options=item_default)
+    parser.add_argument("-p", dest="post_samples", required=True, type=int, help="Posterior samples", gooey_options=item_default)
+    parser.add_argument("-c", dest="cell_vol", required=False, help="Cell Volume", type=float, default=4.2e-17, gooey_options=item_default)
+    parser.add_argument("-t", dest="thinning", required=False, help="Thinning", type=int, default=10, gooey_options=item_default)
+    parser.add_argument("-b", dest="burnin", required=False, help="Burn-in", type=int, default=100, gooey_options=item_default)
     parser.add_argument("-nb", dest="num_bootsrap", required=False, help="Number of subsamples performed", type=int,
-                        default=-1)
+                        default=-1, gooey_options=item_default)
     parser.add_argument("-os", dest="out_suffix", required=False, help="suffix added to output files (default: date)",
-                        type=str, default="")
+                        type=str, default="", gooey_options=item_default)
     parser.add_argument("-a", dest="aggregate", required=False, type=str, default="n",
-                        help="aggregate all datasets by summation (y,n) Default: No (n)")
+                        help="aggregate all datasets by summation (y,n) Default: No (n)", gooey_options=item_default)
 
     args = parser.parse_args()
     run(args)
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `deTELpy-0.1.5/mTEL/mcmc.py` & `deTELpy-0.1.6/mTEL/mcmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,33 @@
+import io
+import time
 import sys
+from contextlib import redirect_stderr
 
 import matplotlib.pyplot as plt
 from tqdm import tqdm
 from dataclasses import dataclass, field
 
 import multiprocessing as mp
 import numpy as np
 
 from . import mtem
 from . import data
 
+
 # TODO change mtem to object that can be evaluated at a given parameter set in order to avoid passing model constants
 #  and data through the mcmc. This also allows to keep things cleaner in general
 
 @dataclass
 class MCMCstate:
     alpha: np.array = field(default_factory=np.array)  # position penalty
     beta: np.array = field(default_factory=np.array)  # nucleotide mismatching
     log_likelihood: float = 0.0
 
+
 @dataclass
 class MCMC:
     model: mtem.MTEM
 
     c_alpha: np.array = field(init=False)  # position penalty
     c_beta: np.array = field(init=False)  # nucleotide mismatching
 
@@ -123,23 +128,23 @@
             wobble_trace[i, :] = self.trace[i].beta
 
         return wobble_trace
 
     def position_penalty_posterior(self, samples):
         nsamples = len(self.trace)
         posterior = np.zeros(shape=(samples, self.trace[0].alpha.shape[0]))
-        for i, s in enumerate(range(nsamples-samples, nsamples)):
+        for i, s in enumerate(range(nsamples - samples, nsamples)):
             posterior[i, :] = self.trace[s].alpha
 
         return np.exp(posterior)
 
     def wobble_penalty_posterior(self, samples):
         nsamples = len(self.trace)
         posterior = np.zeros(shape=(samples, self.trace[0].beta.shape[0]))
-        for i, s in enumerate(range(nsamples-samples, nsamples)):
+        for i, s in enumerate(range(nsamples - samples, nsamples)):
             posterior[i, :] = self.trace[s].beta
 
         return posterior
 
     def likelihood_trace(self):
         t_len = len(self.trace)
         ll_trace = [0] * t_len
@@ -173,24 +178,28 @@
             reordered_data.append(d)
 
         return reordered_data
 
     def run(self, samples, thinning, burnin, ic_alpha, ic_beta, data):
         data = self.prepare_dataset(data)
 
-        iterations = (samples+burnin)*thinning
-        self.trace = samples*[MCMCstate]
+        iterations = (samples + burnin) * thinning
+        self.trace = samples * [MCMCstate]
 
         self.c_alpha = ic_alpha
         self.c_beta = ic_beta
         c_beta = self.model.format_wobble_penalties(self.c_beta)
         p = self.model.calculate_all_substitution_probabilities(np.exp(self.c_alpha), c_beta, combine_ile_leu=True)
         self.current_log_likelihood = self.log_likelihood(data, p)
         print('Initial log(likelihood): {}\n'.format(self.current_log_likelihood))
 
+        f = None
+        if not sys.stdin.isatty():
+            f = io.StringIO()
+
         for i in tqdm(range(0, iterations), file=sys.stdout):
             # Accept/Reject Position penalty
             self.p_alpha = self.propose(self.c_alpha, self.a_proposal_width)
             # forgetting this line caused a bug before. move it into the model itself?
             c_beta = self.model.format_wobble_penalties(self.c_beta)
             p = self.model.calculate_all_substitution_probabilities(np.exp(self.p_alpha), c_beta, combine_ile_leu=True)
             self.proposed_log_likelihood = self.log_likelihood(data, p)
@@ -204,15 +213,18 @@
             self.proposed_log_likelihood = self.log_likelihood(data, p)
             if self.accept_parameter_set(log_parameter=False):
                 self.update_beta()
 
             # ---- UPDATE TRACE ----
             if i / thinning >= burnin:
                 if i % thinning == 0:
-                    self.trace[int(i/thinning) - burnin] = MCMCstate(alpha=self.c_alpha, beta=self.c_beta,
-                                                                     log_likelihood=self.current_log_likelihood)
+                    self.trace[int(i / thinning) - burnin] = MCMCstate(alpha=self.c_alpha, beta=self.c_beta,
+                                                                       log_likelihood=self.current_log_likelihood)
 
             # ---- ADAPT PROPOSAL WIDTH ----
             if i != 0 and i % self.adaptive_width == 0:
                 self.update_proposal_width()
 
+            if f and i % 12 == 0:
+                print(end ='\n', flush=True)
+
         print('Final log(likelihood): {}\n'.format(self.current_log_likelihood))
```

### Comparing `deTELpy-0.1.5/mTEL/mtem.py` & `deTELpy-0.1.6/mTEL/mtem.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/setup.py` & `deTELpy-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
         readme_lines = f.readlines()
 
     return ''.join(readme_lines)
 README = README()  # NOQA
 
 setup(
     name='deTELpy',
-    version='0.1.5',
+    version='0.1.6',
     description='Python package of the deTEL translation error detection pipeline from mass-spectrometry data',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://git.mpi-cbg.de/atplab/detelpy',
     author='Cedric Landerer',
     author_email='landerer@mpi-cbg.de',
-    license='BSD 2-clause',
+    license='BSD',
     packages=['deTEL', 'deTEL.eTEL', 'deTEL.mTEL', 'deTEL.utility'],
     include_package_data=True,
     install_requires=['pandas==1.3.5',
                       'numpy',
                       'dataclasses>=0.6',
                       'pathlib>=1.0.1',
                       'biopython>=1.81',
```

### Comparing `deTELpy-0.1.5/tests/test_run_deTEL.py` & `deTELpy-0.1.6/tests/test_run_deTEL.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/utility/downloadPRIDE.py` & `deTELpy-0.1.6/utility/downloadPRIDE.py`

 * *Files identical despite different names*

### Comparing `deTELpy-0.1.5/utility/prideCrawler.py` & `deTELpy-0.1.6/utility/prideCrawler.py`

 * *Files identical despite different names*

