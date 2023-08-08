# Comparing `tmp/cropclassification-0.1.0a2.tar.gz` & `tmp/cropclassification-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cropclassification-0.1.0a2.tar", last modified: Tue Jun  7 09:27:38 2022, max compression
+gzip compressed data, was "cropclassification-0.1.1.tar", last modified: Tue Aug  8 07:21:10 2023, max compression
```

## Comparing `cropclassification-0.1.0a2.tar` & `cropclassification-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,61 @@
-drwxrwxrwx   0        0        0        0 2022-06-07 09:27:38.030229 cropclassification-0.1.0a2/
--rw-rw-rw-   0        0        0      242 2022-06-01 07:19:26.000000 cropclassification-0.1.0a2/MANIFEST.in
--rw-rw-rw-   0        0        0     3250 2022-06-07 09:27:38.030229 cropclassification-0.1.0a2/PKG-INFO
--rw-rw-rw-   0        0        0     2789 2022-06-01 16:56:46.000000 cropclassification-0.1.0a2/README.md
-drwxrwxrwx   0        0        0        0 2022-06-07 09:27:37.826246 cropclassification-0.1.0a2/cropclassification/
--rw-rw-rw-   0        0        0        0 2020-07-02 13:54:25.000000 cropclassification-0.1.0a2/cropclassification/__init__.py
--rw-rw-rw-   0        0        0    16805 2022-06-01 16:19:07.000000 cropclassification-0.1.0a2/cropclassification/calc_marker.py
--rw-rw-rw-   0        0        0     9691 2022-06-01 16:18:59.000000 cropclassification-0.1.0a2/cropclassification/calc_timeseries.py
--rw-rw-rw-   0        0        0     3887 2022-06-01 13:24:59.000000 cropclassification-0.1.0a2/cropclassification/cropclassification.py
--rw-rw-rw-   0        0        0    11664 2022-05-31 07:16:57.000000 cropclassification-0.1.0a2/cropclassification/general.ini
-drwxrwxrwx   0        0        0        0 2022-06-07 09:27:37.897597 cropclassification-0.1.0a2/cropclassification/helpers/
--rw-rw-rw-   0        0        0        0 2020-07-02 13:54:25.000000 cropclassification-0.1.0a2/cropclassification/helpers/__init__.py
--rw-rw-rw-   0        0        0     4046 2022-05-31 07:16:51.000000 cropclassification-0.1.0a2/cropclassification/helpers/config_helper.py
--rw-rw-rw-   0        0        0     1505 2022-05-31 07:16:51.000000 cropclassification-0.1.0a2/cropclassification/helpers/dir_helper.py
--rw-rw-rw-   0        0        0     1601 2022-05-31 07:29:47.000000 cropclassification-0.1.0a2/cropclassification/helpers/log_helper.py
--rw-rw-rw-   0        0        0    16961 2022-05-31 07:16:51.000000 cropclassification-0.1.0a2/cropclassification/helpers/model_helper.py
--rw-rw-rw-   0        0        0     4371 2022-05-31 07:16:51.000000 cropclassification-0.1.0a2/cropclassification/helpers/pandas_helper.py
-drwxrwxrwx   0        0        0        0 2022-06-07 09:27:37.928854 cropclassification-0.1.0a2/cropclassification/postprocess/
--rw-rw-rw-   0        0        0        0 2020-07-02 13:54:25.000000 cropclassification-0.1.0a2/cropclassification/postprocess/__init__.py
--rw-rw-rw-   0        0        0    23982 2022-06-07 09:25:48.000000 cropclassification-0.1.0a2/cropclassification/postprocess/classification_postprocess.py
--rw-rw-rw-   0        0        0    66593 2022-05-31 07:16:51.000000 cropclassification-0.1.0a2/cropclassification/postprocess/classification_reporting.py
--rw-rw-rw-   0        0        0     7147 2020-04-01 13:39:27.000000 cropclassification-0.1.0a2/cropclassification/postprocess/html_rapport_script.js
--rw-rw-rw-   0        0        0     7970 2020-04-06 11:07:37.000000 cropclassification-0.1.0a2/cropclassification/postprocess/html_rapport_template.html
--rw-rw-rw-   0        0        0     1059 2022-05-31 07:16:51.000000 cropclassification-0.1.0a2/cropclassification/postprocess/html_rapport_test.py
-drwxrwxrwx   0        0        0        0 2022-06-07 09:27:37.963731 cropclassification-0.1.0a2/cropclassification/predict/
--rw-rw-rw-   0        0        0        0 2020-07-02 13:54:25.000000 cropclassification-0.1.0a2/cropclassification/predict/__init__.py
--rw-rw-rw-   0        0        0    11590 2022-05-31 07:16:51.000000 cropclassification-0.1.0a2/cropclassification/predict/classification.py
--rw-rw-rw-   0        0        0    14352 2022-05-31 07:16:51.000000 cropclassification-0.1.0a2/cropclassification/predict/classification_keras.py
--rw-rw-rw-   0        0        0     8269 2022-05-31 07:16:51.000000 cropclassification-0.1.0a2/cropclassification/predict/classification_sklearn.py
--rw-rw-rw-   0        0        0     3191 2022-05-31 07:16:51.000000 cropclassification-0.1.0a2/cropclassification/predict/multicrop.py
-drwxrwxrwx   0        0        0        0 2022-06-07 09:27:38.029229 cropclassification-0.1.0a2/cropclassification/preprocess/
--rw-rw-rw-   0        0        0        0 2020-07-02 13:54:25.000000 cropclassification-0.1.0a2/cropclassification/preprocess/__init__.py
--rw-rw-rw-   0        0        0    20973 2022-05-31 14:56:25.000000 cropclassification-0.1.0a2/cropclassification/preprocess/classification_preprocess.py
--rw-rw-rw-   0        0        0    44268 2022-06-01 13:30:22.000000 cropclassification-0.1.0a2/cropclassification/preprocess/classification_preprocess_BEFL.py
--rw-rw-rw-   0        0        0    12273 2022-05-31 07:16:51.000000 cropclassification-0.1.0a2/cropclassification/preprocess/timeseries.py
--rw-rw-rw-   0        0        0    74842 2022-05-31 10:24:37.000000 cropclassification-0.1.0a2/cropclassification/preprocess/timeseries_calc_dias_onda_per_image.py
--rw-rw-rw-   0        0        0    39291 2022-05-31 17:41:48.000000 cropclassification-0.1.0a2/cropclassification/preprocess/timeseries_calc_gee.py
--rw-rw-rw-   0        0        0    24680 2022-06-03 15:12:01.000000 cropclassification-0.1.0a2/cropclassification/preprocess/timeseries_util.py
--rw-rw-rw-   0        0        0        7 2022-06-07 09:27:05.000000 cropclassification-0.1.0a2/cropclassification/version.txt
-drwxrwxrwx   0        0        0        0 2022-06-07 09:27:37.861645 cropclassification-0.1.0a2/cropclassification.egg-info/
--rw-rw-rw-   0        0        0     3250 2022-06-07 09:27:37.000000 cropclassification-0.1.0a2/cropclassification.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1687 2022-06-07 09:27:37.000000 cropclassification-0.1.0a2/cropclassification.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-07 09:27:37.000000 cropclassification-0.1.0a2/cropclassification.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2022-06-07 09:27:37.000000 cropclassification-0.1.0a2/cropclassification.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       73 2022-06-07 09:27:37.000000 cropclassification-0.1.0a2/cropclassification.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2022-06-07 09:27:37.000000 cropclassification-0.1.0a2/cropclassification.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       76 2022-06-07 09:27:38.033233 cropclassification-0.1.0a2/setup.cfg
--rw-rw-rw-   0        0        0     1118 2022-06-01 11:50:26.000000 cropclassification-0.1.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:21:10.125729 cropclassification-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-08 07:20:53.000000 cropclassification-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-08-08 07:21:10.125729 cropclassification-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-08 07:20:53.000000 cropclassification-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:21:10.117729 cropclassification-0.1.1/cropclassification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16447 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/calc_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/calc_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/cropclassification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/general.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:21:10.121729 cropclassification-0.1.1/cropclassification/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/helpers/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/helpers/dir_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/helpers/log_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/helpers/model_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/helpers/pandas_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:21:10.121729 cropclassification-0.1.1/cropclassification/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23936 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/postprocess/classification_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66392 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/postprocess/classification_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/postprocess/html_rapport_script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/postprocess/html_rapport_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/postprocess/html_rapport_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:21:10.121729 cropclassification-0.1.1/cropclassification/predict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/predict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/predict/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/predict/classification_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/predict/classification_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/predict/multicrop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:21:10.121729 cropclassification-0.1.1/cropclassification/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43736 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/preprocess/_classification_preprocess_BEFL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/preprocess/_timeseries_calc_openeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27097 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/preprocess/_timeseries_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/preprocess/classification_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/preprocess/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:21:10.121729 cropclassification-0.1.1/cropclassification/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/util/geoops_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/util/io_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/util/openeo_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:21:10.125729 cropclassification-0.1.1/cropclassification/util/zonal_stats_bulk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/util/zonal_stats_bulk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/util/zonal_stats_bulk/_general_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29368 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/util/zonal_stats_bulk/_raster_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/util/zonal_stats_bulk/_vector_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/util/zonal_stats_bulk/_zonal_stats_bulk_pyqgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32636 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/util/zonal_stats_bulk/_zonal_stats_bulk_rs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 07:20:53.000000 cropclassification-0.1.1/cropclassification/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:21:10.117729 cropclassification-0.1.1/cropclassification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-08-08 07:21:10.000000 cropclassification-0.1.1/cropclassification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-08-08 07:21:10.000000 cropclassification-0.1.1/cropclassification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:21:10.000000 cropclassification-0.1.1/cropclassification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-08 07:21:10.000000 cropclassification-0.1.1/cropclassification.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-08 07:21:10.000000 cropclassification-0.1.1/cropclassification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-08 07:21:10.000000 cropclassification-0.1.1/cropclassification.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-08 07:21:10.125729 cropclassification-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-08 07:20:53.000000 cropclassification-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:21:10.125729 cropclassification-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-08 07:20:53.000000 cropclassification-0.1.1/tests/test_calc_timeseries.py
```

### Comparing `cropclassification-0.1.0a2/PKG-INFO` & `cropclassification-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,48 @@
-Metadata-Version: 2.1
-Name: cropclassification
-Version: 0.1.0a2
-Summary: Package to classify crops based on sentinel images.
-Home-page: https://github.com/theroggy/cropclassification
-Author: Pieter Roggemans
-Author-email: pieter.roggemans@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
-# Crop classification
-This is a collection of scripts that can help to classify crops using Sentinel data. 
-
-Probably this documentation won't suffice to get you started, but you are free to reach out for more info if you are really interested.
-
-In general, you should also be aware that the package isn't really meant to be an easy-to-use solution for crop classification. It is rather a quite specialised solution for our specific needs. Nonetheless we want to make the code public so if anyone is interested, they can have a look and possibly get some inspiration.
-
-## Installation manual
-1. Install conda
-
-As the scripts are written in Python, you need to use a package manager to be able to install the packages the scripts depend on. The rest of the installation manual assumes you use anaconda and python 3.6+. The installer for anaconda can be found here: https://www.anaconda.com/download/.
-
-2. Create new environment and install dependencies
-
-Once you have anaconda installed, you can open an anaconda terminal window and follow the following steps:
-
-      1. Create and activate a new conda environment
-      ```
-      conda create --name cropclassification
-      conda activate cropclassification
-      conda config --env --add channels conda-forge
-      conda config --env --set channel_priority strict
-      ```
-      2. Install the dependencies for the crop classification scripts:
-      ```
-      conda install python=3.9 geopandas geofileops "h5py<3" psutil rasterio "rasterstats<0.16.0" scikit-learn
-      ```
-      3. If it was the first time you installed anaconda/geopandas, you might have to restart your computer to proceed
-      4. Start the anaconda terminal window again and activate the environment
-      ```
-      conda activate cropclassification
-      ```
-      5. Now install cropclassification and dependencies that need pip with pip
-      ```
-      pip install cropclassification
-      ```
-4. Calculate time series 
-
-To calculate time series, you need to run `cropclassification -t <tasks_dir>`, with a 'calc_timeseries' type of task in the tasks dir 
-on a server that has access to sentinel CARD images.
-
-Mind: the sentinel CARD image structure as expected for timeseries calculation depends on the image type:
-  * for Sentinel 2 images this is the standard S2 L2A format as available on the open acces copernicus hub.
-  * for Sentinel 1 backscatter and sentinel 1 coherence data this is a non-standardized data structure as there isn't a standard format (yet) for level 2 processed sentinel 1 images (as far as I know). Check out the code to see the expected data structure ;-). 
-
-5. Start a crop classification
-
-Run `cropclassification -t <tasks_dir>`, with a 'calc_marker' type of task in the tasks dir.
-
-
+# Crop classification
+This is a collection of scripts that can help to classify crops using Sentinel data. 
+
+Probably this documentation won't suffice to get you started, but you are free to reach out for more info if you are really interested.
+
+In general, you should also be aware that the package isn't really meant to be an easy-to-use solution for crop classification. It is rather a quite specialised solution for our specific needs. Nonetheless we want to make the code public so if anyone is interested, they can have a look and possibly get some inspiration.
+
+## Installation manual
+1. Install conda
+
+As the scripts are written in Python, you need to use a package manager to be able to install the packages the scripts depend on. The rest of the installation manual assumes you use anaconda and python 3.6+. The installer for anaconda can be found here: https://www.anaconda.com/download/.
+
+2. Create new environment and install dependencies
+
+Once you have anaconda installed, you can open an anaconda terminal window and follow the following steps:
+
+      1. Create and activate a new conda environment
+      ```
+      conda create --name cropclassification
+      conda activate cropclassification
+      conda config --env --add channels conda-forge
+      conda config --env --set channel_priority strict
+      ```
+      2. Install the dependencies for the crop classification scripts:
+      ```
+      conda install python=3.9 geopandas geofileops "h5py<3" openeo psutil qgis rasterio rasterstats scikit-learn
+      ```
+      3. If it was the first time you installed anaconda/geopandas, you might have to restart your computer to proceed
+      4. Start the anaconda terminal window again and activate the environment
+      ```
+      conda activate cropclassification
+      ```
+      5. Now install cropclassification and dependencies that need pip with pip
+      ```
+      pip install cropclassification
+      ```
+4. Calculate time series 
+
+To calculate time series, you need to run `cropclassification -t <tasks_dir>`, with a 'calc_timeseries' type of task in the tasks dir 
+on a server that has access to sentinel CARD images.
+
+Mind: the sentinel CARD image structure as expected for timeseries calculation depends on the image type:
+  * for Sentinel 2 images this is the standard S2 L2A format as available on the open acces copernicus hub.
+  * for Sentinel 1 backscatter and sentinel 1 coherence data this is a non-standardized data structure as there isn't a standard format (yet) for level 2 processed sentinel 1 images (as far as I know). Check out the code to see the expected data structure ;-). 
+
+5. Start a crop classification
+
+Run `cropclassification -t <tasks_dir>`, with a 'calc_marker' type of task in the tasks dir.
```

### Comparing `cropclassification-0.1.0a2/cropclassification/calc_marker.py` & `cropclassification-0.1.1/cropclassification/calc_marker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,380 +1,378 @@
-# -*- coding: utf-8 -*-
-"""
-Main script to do a classification.
-"""
-
-import logging
-import os
-from pathlib import Path
-import shutil
-from typing import List
-
-# Import geofilops here already, if tensorflow is loaded first leads to dll load errors
-import geofileops as gfo
-
-from cropclassification.helpers import config_helper as conf
-from cropclassification.helpers import dir_helper
-from cropclassification.helpers import log_helper
-from cropclassification.helpers import model_helper as mh
-from cropclassification.preprocess import timeseries_util as ts_util
-from cropclassification.preprocess import timeseries as ts
-from cropclassification.preprocess import classification_preprocess as class_pre
-from cropclassification.predict import classification
-from cropclassification.postprocess import classification_postprocess as class_post
-from cropclassification.postprocess import classification_reporting as class_report
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-
-
-def calc_marker_task(config_paths: List[Path], default_basedir: Path):
-    """
-    Runs a marker using the setting in the config_paths.
-
-    Args:
-        config_paths (List[Path]): the config files to load
-        default_basedir (Path): the dir to resolve relative paths in the config
-            file to.
-
-    Raises:
-        Exception: [description]
-        Exception: [description]
-    """
-    # Read the configuration files
-    conf.read_config(config_paths, default_basedir=default_basedir)
-
-    # Create run dir to be used for the results
-    reuse_last_run_dir = conf.calc_marker_params.getboolean("reuse_last_run_dir")
-    reuse_last_run_dir_config = conf.calc_marker_params.getboolean(
-        "reuse_last_run_dir_config"
-    )
-    run_dir = dir_helper.create_run_dir(
-        conf.dirs.getpath("marker_dir"), reuse_last_run_dir
-    )
-    print(run_dir)
-    if not run_dir.exists():
-        os.makedirs(run_dir)
-
-    # Main initialisation of the logging
-    log_level = conf.general.get("log_level")
-    logger = log_helper.main_log_init(run_dir, __name__, log_level)      
-    logger.info(f"Run dir with reuse_last_run_dir: {reuse_last_run_dir}, {run_dir}")
-    logger.info(f"Config used: \n{conf.pformat_config()}")
-
-    # If running in conda, export the environment
-    conda_env = os.environ.get("CONDA_DEFAULT_ENV")
-    if conda_env is not None:
-        environment_yml_path = run_dir / f"{conda_env}.yml"
-        logger.info(f"Export conda environment used to {environment_yml_path}")
-        os.system(f"conda env export > {environment_yml_path}")
-
-    # If the config needs to be reused as well, load it, else write it
-    config_used_path = run_dir / "config_used.ini"
-    if (
-        reuse_last_run_dir
-        and reuse_last_run_dir_config
-        and run_dir.exists()
-        and config_used_path.exists()
-    ):
-        config_paths.append(config_used_path)
-        logger.info(f"Run dir config needs to be reused, so {config_paths}")
-        conf.read_config(config_paths=config_paths, default_basedir=default_basedir)
-        logger.info(
-            "Write new config_used.ini, because some parameters might have been added"
-        )
-        with open(config_used_path, "w") as config_used_file:
-            conf.config.write(config_used_file)
-    else:
-        # Copy the config files to a config dir for later notice
-        configfiles_used_dir = run_dir / "configfiles_used"
-        if configfiles_used_dir.exists():
-            shutil.rmtree(configfiles_used_dir)
-        configfiles_used_dir.mkdir()
-        for config_path in config_paths:
-            shutil.copy(config_path, configfiles_used_dir)
-
-        # Write the resolved complete config, so it can be reused
-        logger.info("Write config_used.ini, so it can be reused later on")
-        with open(config_used_path, "w") as config_used_file:
-            conf.config.write(config_used_file)
-
-    # Read the info about the run
-    input_parcel_filename = conf.calc_marker_params.getpath("input_parcel_filename")
-    input_parcel_filetype = conf.calc_marker_params["input_parcel_filetype"]
-    country_code = conf.calc_marker_params["country_code"]
-    classes_refe_filename = conf.calc_marker_params.getpath("classes_refe_filename")
-    input_groundtruth_filename = conf.calc_marker_params.getpath(
-        "input_groundtruth_filename"
-    )
-    input_model_to_use_relativepath = conf.calc_marker_params.getpath(
-        "input_model_to_use_relativepath"
-    )
-
-    # Prepare input paths
-    if input_model_to_use_relativepath is not None:
-        input_model_to_use_path = (
-            conf.dirs.getpath("model_dir") / input_model_to_use_relativepath
-        )
-        if not input_model_to_use_path.exists():
-            raise Exception(
-                "Input file input_model_to_use_path doesn't exist: "
-                f"{input_model_to_use_path}"
-            )
-    else:
-        input_model_to_use_path = None
-
-    input_dir = conf.dirs.getpath("input_dir")
-    input_parcel_path = input_dir / input_parcel_filename
-    if input_groundtruth_filename is not None:
-        input_groundtruth_path = input_dir / input_groundtruth_filename
-    else:
-        input_groundtruth_path = None
-
-    refe_dir = conf.dirs.getpath("refe_dir")
-    classes_refe_path = refe_dir / classes_refe_filename
-
-    # Check if the necessary input files exist...
-    for path in [classes_refe_path, input_parcel_path]:
-        if path is not None and not path.exists():
-            message = f"Input file doesn't exist, so STOP: {path}"
-            logger.critical(message)
-            raise Exception(message)
-
-    # Get some general config
-    data_ext = conf.general["data_ext"]
-    output_ext = conf.general["output_ext"]
-    geofile_ext = conf.general["geofile_ext"]
-
-    # -------------------------------------------------------------
-    # The real work
-    # -------------------------------------------------------------
-    # STEP 1: prepare parcel data for classification and image data extraction
-    # -------------------------------------------------------------
-
-    # Prepare the input data for optimal image data extraction:
-    #    1) apply a negative buffer on the parcel to evade mixels
-    #    2) remove features that became null because of buffer
-    input_preprocessed_dir = conf.dirs.getpath("input_preprocessed_dir")
-    buffer = conf.marker.getint("buffer")
-    input_parcel_nogeo_path = (
-        input_preprocessed_dir / f"{input_parcel_filename.stem}{data_ext}"
-    )
-    imagedata_input_parcel_filename = (
-        f"{input_parcel_filename.stem}_bufm{buffer}{geofile_ext}"
-    )
-    imagedata_input_parcel_path = (
-        input_preprocessed_dir / imagedata_input_parcel_filename
-    )
-    ts_util.prepare_input(
-        input_parcel_path=input_parcel_path,
-        output_imagedata_parcel_input_path=imagedata_input_parcel_path,
-        output_parcel_nogeo_path=input_parcel_nogeo_path,
-    )
-
-    # STEP 2: Get the timeseries data needed for the classification
-    # -------------------------------------------------------------
-    # Get the time series data (S1 and S2) to be used for the classification
-    # Result: data is put in files in timeseries_periodic_dir, in one file per
-    #         date/period
-    timeseries_periodic_dir = conf.dirs.getpath("timeseries_periodic_dir")
-    start_date_str = conf.marker["start_date_str"]
-    end_date_str = conf.marker["end_date_str"]
-    sensordata_to_use = conf.marker.getlist("sensordata_to_use")
-    parceldata_aggregations_to_use = conf.marker.getlist(
-        "parceldata_aggregations_to_use"
-    )
-    base_filename = f"{input_parcel_filename.stem}_bufm{buffer}_weekly"
-    ts.calc_timeseries_data(
-        input_parcel_path=imagedata_input_parcel_path,
-        input_country_code=country_code,
-        start_date_str=start_date_str,
-        end_date_str=end_date_str,
-        sensordata_to_get=sensordata_to_use,
-        base_filename=base_filename,
-        dest_data_dir=timeseries_periodic_dir,
-    )
-
-    # STEP 3: Preprocess all data needed for the classification
-    # -------------------------------------------------------------
-    # Prepare the basic input file with the classes that will be classified to.
-    # Remarks:
-    #    - this is typically specific for the input dataset and result wanted!!!
-    #    - the result is/should be a file with the following columns
-    #           - id (=id_column): unique ID for each parcel
-    #           - classname (=class_column): the class that must
-    #             be classified to.
-    #             Remarks: - if in classes_to_ignore_for_train, class not used for train
-    #                      - if in classes_to_ignore, the class will be ignored
-    #           - pixcount:
-    #             the number of S1/S2 pixels in the parcel.
-    #             Is -1 if the parcel doesn't have any S1/S2 data.
-    classtype_to_prepare = conf.preprocess["classtype_to_prepare"]
-    parcel_path = run_dir / f"{input_parcel_filename.stem}_parcel{data_ext}"
-    parcel_pixcount_path = (
-        timeseries_periodic_dir / f"{base_filename}_pixcount{data_ext}"
-    )
-    class_pre.prepare_input(
-        input_parcel_path=input_parcel_nogeo_path,
-        input_parcel_filetype=input_parcel_filetype,
-        input_parcel_pixcount_path=parcel_pixcount_path,
-        classtype_to_prepare=classtype_to_prepare,
-        classes_refe_path=classes_refe_path,
-        output_parcel_path=parcel_path,
-    )
-
-    # Collect all data needed to do the classification in one input file
-    parcel_classification_data_path = (
-        run_dir / f"{base_filename}_parcel_classdata{data_ext}"
-    )
-    ts.collect_and_prepare_timeseries_data(
-        input_parcel_path=input_parcel_nogeo_path,
-        timeseries_dir=timeseries_periodic_dir,
-        base_filename=base_filename,
-        output_path=parcel_classification_data_path,
-        start_date_str=start_date_str,
-        end_date_str=end_date_str,
-        sensordata_to_use=sensordata_to_use,
-        parceldata_aggregations_to_use=parceldata_aggregations_to_use,
-    )
-
-    # STEP 4: Train and test if necessary... and predict
-    # -------------------------------------------------------------
-    markertype = conf.marker.get("markertype")
-    parcel_predictions_proba_all_path = (
-        run_dir / f"{base_filename}_predict_proba_all{data_ext}"
-    )
-    classifier_ext = conf.classifier["classifier_ext"]
-    classifier_basepath = run_dir / f"{markertype}_01_mlp{classifier_ext}"
-
-    # Check if a model exists already
-    if input_model_to_use_path is None:
-        best_model = mh.get_best_model(run_dir, acc_metric_mode="min")
-        if best_model is not None:
-            input_model_to_use_path = best_model["path"]
-
-    # if there is no model to use specified, train one!
-    parcel_test_path = None
-    parcel_predictions_proba_test_path = None
-    if input_model_to_use_path is None:
-
-        # Create the training sample...
-        # Remark: this creates a list of representative test parcel + a list of
-        # (candidate) training parcel
-        balancing_strategy = conf.marker["balancing_strategy"]
-        parcel_train_path = run_dir / f"{base_filename}_parcel_train{data_ext}"
-        parcel_test_path = run_dir / f"{base_filename}_parcel_test{data_ext}"
-        class_pre.create_train_test_sample(
-            input_parcel_path=parcel_path,
-            output_parcel_train_path=parcel_train_path,
-            output_parcel_test_path=parcel_test_path,
-            balancing_strategy=balancing_strategy,
-        )
-
-        # Train the classifier and output predictions
-        parcel_predictions_proba_test_path = (
-            run_dir / f"{base_filename}_predict_proba_test{data_ext}"
-        )
-        classification.train_test_predict(
-            input_parcel_train_path=parcel_train_path,
-            input_parcel_test_path=parcel_test_path,
-            input_parcel_all_path=parcel_path,
-            input_parcel_classification_data_path=parcel_classification_data_path,
-            output_classifier_basepath=classifier_basepath,
-            output_predictions_test_path=parcel_predictions_proba_test_path,
-            output_predictions_all_path=parcel_predictions_proba_all_path,
-        )
-    else:
-        # there is a classifier specified, so just use it!
-        classification.predict(
-            input_parcel_path=parcel_path,
-            input_parcel_classification_data_path=parcel_classification_data_path,
-            input_classifier_basepath=classifier_basepath,
-            input_classifier_path=input_model_to_use_path,
-            output_predictions_path=parcel_predictions_proba_all_path,
-        )
-
-    # STEP 5: if necessary, do extra postprocessing
-    # -------------------------------------------------------------
-    """if postprocess_to_groups is not None:
-        # TODO
-    """
-
-    # STEP 6: do the default, mandatory postprocessing
-    # -------------------------------------------------------------
-    # If it was necessary to train, there will be a test prediction... so postprocess it
-    parcel_predictions_test_path = None
-    parcel_predictions_test_geopath = None
-    if (
-        input_model_to_use_path is None
-        and parcel_test_path is not None
-        and parcel_predictions_proba_test_path is not None
-    ):
-        parcel_predictions_test_path = (
-            run_dir / f"{base_filename}_predict_test{data_ext}"
-        )
-        parcel_predictions_test_geopath = (
-            run_dir / f"{base_filename}_predict_test{geofile_ext}"
-        )
-        class_post.calc_top3_and_consolidation(
-            input_parcel_path=parcel_test_path,
-            input_parcel_probabilities_path=parcel_predictions_proba_test_path,
-            input_parcel_geopath=input_parcel_path,
-            output_predictions_path=parcel_predictions_test_path,
-            output_predictions_geopath=parcel_predictions_test_geopath,
-        )
-
-    # Postprocess predictions
-    parcel_predictions_all_path = run_dir / f"{base_filename}_predict_all{data_ext}"
-    parcel_predictions_all_geopath = (
-        run_dir / f"{base_filename}_predict_all{geofile_ext}"
-    )
-    parcel_predictions_all_output_path = (
-        run_dir / f"{base_filename}_predict_all_output{output_ext}"
-    )
-    class_post.calc_top3_and_consolidation(
-        input_parcel_path=parcel_path,
-        input_parcel_probabilities_path=parcel_predictions_proba_all_path,
-        input_parcel_geopath=input_parcel_path,
-        output_predictions_path=parcel_predictions_all_path,
-        output_predictions_geopath=parcel_predictions_all_geopath,
-        output_predictions_output_path=parcel_predictions_all_output_path,
-    )
-
-    # STEP 7: Report on the accuracy, incl. ground truth
-    # -------------------------------------------------------------
-    # Preprocess the ground truth data if it is provided
-    groundtruth_path = None
-    if input_groundtruth_path is not None:
-        groundtruth_path = (
-            run_dir
-            / f"{input_groundtruth_path.stem}_classes{input_groundtruth_path.suffix}"
-        )
-        class_pre.prepare_input(
-            input_parcel_path=input_groundtruth_path,
-            input_parcel_filetype=input_parcel_filetype,
-            input_parcel_pixcount_path=parcel_pixcount_path,
-            classtype_to_prepare=conf.preprocess["classtype_to_prepare_groundtruth"],
-            classes_refe_path=classes_refe_path,
-            output_parcel_path=groundtruth_path,
-        )
-
-    # If we trained a model, there is a test prediction we want to report on
-    if input_model_to_use_path is None and parcel_predictions_test_geopath is not None:
-        # Print full reporting on the accuracy of the test dataset
-        report_txt = Path(f"{str(parcel_predictions_test_path)}_accuracy_report.txt")
-        class_report.write_full_report(
-            parcel_predictions_geopath=parcel_predictions_test_geopath,
-            output_report_txt=report_txt,
-            parcel_ground_truth_path=groundtruth_path,
-        )
-
-    # Print full reporting on the accuracy of the full dataset
-    report_txt = Path(f"{str(parcel_predictions_all_path)}_accuracy_report.txt")
-    class_report.write_full_report(
-        parcel_predictions_geopath=parcel_predictions_all_geopath,
-        output_report_txt=report_txt,
-        parcel_ground_truth_path=groundtruth_path,
-    )
-
-    logging.shutdown()
+# -*- coding: utf-8 -*-
+"""
+Main script to do a classification.
+"""
+
+import logging
+import os
+from pathlib import Path
+import shutil
+from typing import List
+
+# Import geofilops here already, if tensorflow is loaded first leads to dll load errors
+import geofileops as gfo  # noqa: F401
+
+from cropclassification.helpers import config_helper as conf
+from cropclassification.helpers import dir_helper
+from cropclassification.helpers import log_helper
+from cropclassification.helpers import model_helper as mh
+from cropclassification.preprocess import _timeseries_helper as ts_helper
+from cropclassification.preprocess import timeseries as ts
+from cropclassification.preprocess import classification_preprocess as class_pre
+from cropclassification.predict import classification
+from cropclassification.postprocess import classification_postprocess as class_post
+from cropclassification.postprocess import classification_reporting as class_report
+
+# -------------------------------------------------------------
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+
+
+def calc_marker_task(config_paths: List[Path], default_basedir: Path):
+    """
+    Runs a marker using the setting in the config_paths.
+
+    Args:
+        config_paths (List[Path]): the config files to load
+        default_basedir (Path): the dir to resolve relative paths in the config
+            file to.
+
+    Raises:
+        Exception: [description]
+        Exception: [description]
+    """
+    # Read the configuration files
+    conf.read_config(config_paths, default_basedir=default_basedir)
+
+    # Create run dir to be used for the results
+    reuse_last_run_dir = conf.calc_marker_params.getboolean("reuse_last_run_dir")
+    reuse_last_run_dir_config = conf.calc_marker_params.getboolean(
+        "reuse_last_run_dir_config"
+    )
+    run_dir = dir_helper.create_run_dir(
+        conf.dirs.getpath("marker_dir"), reuse_last_run_dir
+    )
+    print(run_dir)
+    if not run_dir.exists():
+        os.makedirs(run_dir)
+
+    # Main initialisation of the logging
+    log_level = conf.general.get("log_level")
+    logger = log_helper.main_log_init(run_dir, __name__, log_level)
+    logger.info(f"Run dir with reuse_last_run_dir: {reuse_last_run_dir}, {run_dir}")
+    logger.info(f"Config used: \n{conf.pformat_config()}")
+
+    # If running in conda, export the environment
+    conda_env = os.environ.get("CONDA_DEFAULT_ENV")
+    if conda_env is not None:
+        environment_yml_path = run_dir / f"{conda_env}.yml"
+        logger.info(f"Export conda environment used to {environment_yml_path}")
+        os.system(f"conda env export > {environment_yml_path}")
+
+    # If the config needs to be reused as well, load it, else write it
+    config_used_path = run_dir / "config_used.ini"
+    if (
+        reuse_last_run_dir
+        and reuse_last_run_dir_config
+        and run_dir.exists()
+        and config_used_path.exists()
+    ):
+        config_paths.append(config_used_path)
+        logger.info(f"Run dir config needs to be reused, so {config_paths}")
+        conf.read_config(config_paths=config_paths, default_basedir=default_basedir)
+        logger.info(
+            "Write new config_used.ini, because some parameters might have been added"
+        )
+        with open(config_used_path, "w") as config_used_file:
+            conf.config.write(config_used_file)
+    else:
+        # Copy the config files to a config dir for later notice
+        configfiles_used_dir = run_dir / "configfiles_used"
+        if configfiles_used_dir.exists():
+            shutil.rmtree(configfiles_used_dir)
+        configfiles_used_dir.mkdir()
+        for config_path in config_paths:
+            shutil.copy(config_path, configfiles_used_dir)
+
+        # Write the resolved complete config, so it can be reused
+        logger.info("Write config_used.ini, so it can be reused later on")
+        with open(config_used_path, "w") as config_used_file:
+            conf.config.write(config_used_file)
+
+    # Read the info about the run
+    input_parcel_filename = conf.calc_marker_params.getpath("input_parcel_filename")
+    input_parcel_filetype = conf.calc_marker_params["input_parcel_filetype"]
+    classes_refe_filename = conf.calc_marker_params.getpath("classes_refe_filename")
+    input_groundtruth_filename = conf.calc_marker_params.getpath(
+        "input_groundtruth_filename"
+    )
+    input_model_to_use_relativepath = conf.calc_marker_params.getpath(
+        "input_model_to_use_relativepath"
+    )
+
+    # Prepare input paths
+    if input_model_to_use_relativepath is not None:
+        input_model_to_use_path = (
+            conf.dirs.getpath("model_dir") / input_model_to_use_relativepath
+        )
+        if not input_model_to_use_path.exists():
+            raise Exception(
+                "Input file input_model_to_use_path doesn't exist: "
+                f"{input_model_to_use_path}"
+            )
+    else:
+        input_model_to_use_path = None
+
+    input_dir = conf.dirs.getpath("input_dir")
+    input_parcel_path = input_dir / input_parcel_filename
+    if input_groundtruth_filename is not None:
+        input_groundtruth_path = input_dir / input_groundtruth_filename
+    else:
+        input_groundtruth_path = None
+
+    refe_dir = conf.dirs.getpath("refe_dir")
+    classes_refe_path = refe_dir / classes_refe_filename
+
+    # Check if the necessary input files exist...
+    for path in [classes_refe_path, input_parcel_path]:
+        if path is not None and not path.exists():
+            message = f"Input file doesn't exist, so STOP: {path}"
+            logger.critical(message)
+            raise Exception(message)
+
+    # Get some general config
+    data_ext = conf.general["data_ext"]
+    output_ext = conf.general["output_ext"]
+    geofile_ext = conf.general["geofile_ext"]
+
+    # -------------------------------------------------------------
+    # The real work
+    # -------------------------------------------------------------
+    # STEP 1: prepare parcel data for classification and image data extraction
+    # -------------------------------------------------------------
+
+    # Prepare the input data for optimal image data extraction:
+    #    1) apply a negative buffer on the parcel to evade mixels
+    #    2) remove features that became null because of buffer
+    input_preprocessed_dir = conf.dirs.getpath("input_preprocessed_dir")
+    buffer = conf.marker.getint("buffer")
+    input_parcel_nogeo_path = (
+        input_preprocessed_dir / f"{input_parcel_filename.stem}{data_ext}"
+    )
+    imagedata_input_parcel_filename = (
+        f"{input_parcel_filename.stem}_bufm{buffer}{geofile_ext}"
+    )
+    imagedata_input_parcel_path = (
+        input_preprocessed_dir / imagedata_input_parcel_filename
+    )
+    ts_helper.prepare_input(
+        input_parcel_path=input_parcel_path,
+        output_imagedata_parcel_input_path=imagedata_input_parcel_path,
+        output_parcel_nogeo_path=input_parcel_nogeo_path,
+    )
+
+    # STEP 2: Get the timeseries data needed for the classification
+    # -------------------------------------------------------------
+    # Get the time series data (eg. S1, S2,...) to be used for the classification
+    # Result: data is put in files in timeseries_periodic_dir, in one file per
+    #         date/period
+    timeseries_periodic_dir = conf.dirs.getpath("timeseries_periodic_dir")
+    timeseries_periodic_dir = timeseries_periodic_dir / imagedata_input_parcel_path.stem
+    start_date_str = conf.marker["start_date_str"]
+    end_date_str = conf.marker["end_date_str"]
+    sensordata_to_use = conf.parse_sensordata_to_use(conf.marker["sensordata_to_use"])
+    parceldata_aggregations_to_use = conf.marker.getlist(
+        "parceldata_aggregations_to_use"
+    )
+    ts.calc_timeseries_data(
+        input_parcel_path=imagedata_input_parcel_path,
+        start_date_str=start_date_str,
+        end_date_str=end_date_str,
+        sensordata_to_get=sensordata_to_use,
+        dest_data_dir=timeseries_periodic_dir,
+    )
+
+    # STEP 3: Preprocess all data needed for the classification
+    # -------------------------------------------------------------
+    # Prepare the basic input file with the classes that will be classified to.
+    # Remarks:
+    #    - this is typically specific for the input dataset and result wanted!!!
+    #    - the result is/should be a file with the following columns
+    #           - id (=id_column): unique ID for each parcel
+    #           - classname (=class_column): the class that must
+    #             be classified to.
+    #             Remarks: - if in classes_to_ignore_for_train, class not used for train
+    #                      - if in classes_to_ignore, the class will be ignored
+    #           - pixcount:
+    #             the number of S1/S2 pixels in the parcel.
+    #             Is -1 if the parcel doesn't have any S1/S2 data.
+    classtype_to_prepare = conf.preprocess["classtype_to_prepare"]
+    parcel_path = run_dir / f"{input_parcel_filename.stem}_parcel{data_ext}"
+    base_filename = f"{input_parcel_filename.stem}_bufm{buffer}_weekly"
+    class_pre.prepare_input(
+        input_parcel_path=input_parcel_nogeo_path,
+        input_parcel_filetype=input_parcel_filetype,
+        timeseries_periodic_dir=timeseries_periodic_dir,
+        base_filename=base_filename,
+        data_ext=data_ext,
+        classtype_to_prepare=classtype_to_prepare,
+        classes_refe_path=classes_refe_path,
+        output_parcel_path=parcel_path,
+    )
+
+    # Collect all data needed to do the classification in one input file
+    parcel_classification_data_path = (
+        run_dir / f"{base_filename}_parcel_classdata{data_ext}"
+    )
+    ts.collect_and_prepare_timeseries_data(
+        input_parcel_path=input_parcel_nogeo_path,
+        timeseries_dir=timeseries_periodic_dir,
+        base_filename=base_filename,
+        output_path=parcel_classification_data_path,
+        start_date_str=start_date_str,
+        end_date_str=end_date_str,
+        sensordata_to_use=sensordata_to_use,
+        parceldata_aggregations_to_use=parceldata_aggregations_to_use,
+    )
+
+    # STEP 4: Train and test if necessary... and predict
+    # -------------------------------------------------------------
+    markertype = conf.marker.get("markertype")
+    parcel_predictions_proba_all_path = (
+        run_dir / f"{base_filename}_predict_proba_all{data_ext}"
+    )
+    classifier_ext = conf.classifier["classifier_ext"]
+    classifier_basepath = run_dir / f"{markertype}_01_mlp{classifier_ext}"
+
+    # Check if a model exists already
+    if input_model_to_use_path is None:
+        best_model = mh.get_best_model(run_dir, acc_metric_mode="min")
+        if best_model is not None:
+            input_model_to_use_path = best_model["path"]
+
+    # if there is no model to use specified, train one!
+    parcel_test_path = None
+    parcel_predictions_proba_test_path = None
+    if input_model_to_use_path is None:
+        # Create the training sample...
+        # Remark: this creates a list of representative test parcel + a list of
+        # (candidate) training parcel
+        balancing_strategy = conf.marker["balancing_strategy"]
+        parcel_train_path = run_dir / f"{base_filename}_parcel_train{data_ext}"
+        parcel_test_path = run_dir / f"{base_filename}_parcel_test{data_ext}"
+        class_pre.create_train_test_sample(
+            input_parcel_path=parcel_path,
+            output_parcel_train_path=parcel_train_path,
+            output_parcel_test_path=parcel_test_path,
+            balancing_strategy=balancing_strategy,
+        )
+
+        # Train the classifier and output predictions
+        parcel_predictions_proba_test_path = (
+            run_dir / f"{base_filename}_predict_proba_test{data_ext}"
+        )
+        classification.train_test_predict(
+            input_parcel_train_path=parcel_train_path,
+            input_parcel_test_path=parcel_test_path,
+            input_parcel_all_path=parcel_path,
+            input_parcel_classification_data_path=parcel_classification_data_path,
+            output_classifier_basepath=classifier_basepath,
+            output_predictions_test_path=parcel_predictions_proba_test_path,
+            output_predictions_all_path=parcel_predictions_proba_all_path,
+        )
+    else:
+        # there is a classifier specified, so just use it!
+        classification.predict(
+            input_parcel_path=parcel_path,
+            input_parcel_classification_data_path=parcel_classification_data_path,
+            input_classifier_basepath=classifier_basepath,
+            input_classifier_path=input_model_to_use_path,
+            output_predictions_path=parcel_predictions_proba_all_path,
+        )
+
+    # STEP 5: if necessary, do extra postprocessing
+    # -------------------------------------------------------------
+    """if postprocess_to_groups is not None:
+        # TODO
+    """
+
+    # STEP 6: do the default, mandatory postprocessing
+    # -------------------------------------------------------------
+    # If it was necessary to train, there will be a test prediction... so postprocess it
+    parcel_predictions_test_path = None
+    parcel_predictions_test_geopath = None
+    if (
+        input_model_to_use_path is None
+        and parcel_test_path is not None
+        and parcel_predictions_proba_test_path is not None
+    ):
+        parcel_predictions_test_path = (
+            run_dir / f"{base_filename}_predict_test{data_ext}"
+        )
+        parcel_predictions_test_geopath = (
+            run_dir / f"{base_filename}_predict_test{geofile_ext}"
+        )
+        class_post.calc_top3_and_consolidation(
+            input_parcel_path=parcel_test_path,
+            input_parcel_probabilities_path=parcel_predictions_proba_test_path,
+            input_parcel_geopath=input_parcel_path,
+            output_predictions_path=parcel_predictions_test_path,
+            output_predictions_geopath=parcel_predictions_test_geopath,
+        )
+
+    # Postprocess predictions
+    parcel_predictions_all_path = run_dir / f"{base_filename}_predict_all{data_ext}"
+    parcel_predictions_all_geopath = (
+        run_dir / f"{base_filename}_predict_all{geofile_ext}"
+    )
+    parcel_predictions_all_output_path = (
+        run_dir / f"{base_filename}_predict_all_output{output_ext}"
+    )
+    class_post.calc_top3_and_consolidation(
+        input_parcel_path=parcel_path,
+        input_parcel_probabilities_path=parcel_predictions_proba_all_path,
+        input_parcel_geopath=input_parcel_path,
+        output_predictions_path=parcel_predictions_all_path,
+        output_predictions_geopath=parcel_predictions_all_geopath,
+        output_predictions_output_path=parcel_predictions_all_output_path,
+    )
+
+    # STEP 7: Report on the accuracy, incl. ground truth
+    # -------------------------------------------------------------
+    # Preprocess the ground truth data if it is provided
+    groundtruth_path = None
+    if input_groundtruth_path is not None:
+        groundtruth_path = (
+            run_dir
+            / f"{input_groundtruth_path.stem}_classes{input_groundtruth_path.suffix}"
+        )
+        class_pre.prepare_input(
+            input_parcel_path=input_groundtruth_path,
+            input_parcel_filetype=input_parcel_filetype,
+            timeseries_periodic_dir=timeseries_periodic_dir,
+            base_filename=base_filename,
+            data_ext=data_ext,
+            classtype_to_prepare=conf.preprocess["classtype_to_prepare_groundtruth"],
+            classes_refe_path=classes_refe_path,
+            output_parcel_path=groundtruth_path,
+        )
+
+    # If we trained a model, there is a test prediction we want to report on
+    if input_model_to_use_path is None and parcel_predictions_test_geopath is not None:
+        # Print full reporting on the accuracy of the test dataset
+        report_txt = Path(f"{str(parcel_predictions_test_path)}_accuracy_report.txt")
+        class_report.write_full_report(
+            parcel_predictions_geopath=parcel_predictions_test_geopath,
+            output_report_txt=report_txt,
+            parcel_ground_truth_path=groundtruth_path,
+        )
+
+    # Print full reporting on the accuracy of the full dataset
+    report_txt = Path(f"{str(parcel_predictions_all_path)}_accuracy_report.txt")
+    class_report.write_full_report(
+        parcel_predictions_geopath=parcel_predictions_all_geopath,
+        output_report_txt=report_txt,
+        parcel_ground_truth_path=groundtruth_path,
+    )
+
+    logging.shutdown()
```

### Comparing `cropclassification-0.1.0a2/cropclassification/calc_timeseries.py` & `cropclassification-0.1.1/cropclassification/calc_timeseries.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,257 +1,308 @@
-# -*- coding: utf-8 -*-
-"""
-Calaculate the timeseries data per image on DIAS.
-"""
-
-import datetime
-import glob
-import os
-from pathlib import Path
-import shutil
-from typing import List
-
-# Import geofilops here already, if tensorflow is loaded first leads to dll load errors
-import geofileops as gfo
-
-from cropclassification.helpers import config_helper as conf
-from cropclassification.helpers import log_helper
-from cropclassification.preprocess import timeseries_calc_dias_onda_per_image as calc_ts
-from cropclassification.preprocess import timeseries_util as ts_util
-
-
-def calc_timeseries_task(config_paths: List[Path], default_basedir: Path):
-    """
-    Runs a calculation of timeseries with the settings in the config_paths.
-
-    Args:
-        config_paths (List[Path]): the config files to load
-        default_basedir (Path): the dir to resolve relative paths in the config
-            file to.
-
-    Raises:
-        Exception: [description]
-        Exception: [description]
-    """
-    # Read the configuration files
-    conf.read_config(config_paths, default_basedir=default_basedir)
-
-    test = conf.calc_timeseries_params.getboolean("test")
-
-    # As we want a weekly calculation, get nearest monday for start and stop day
-    start_date = ts_util.get_monday(
-        conf.marker["start_date_str"]
-    )  # output: vb 2018_2_1 - maandag van week 2 van 2018
-    end_date = ts_util.get_monday(conf.marker["end_date_str"])
-
-    calc_year_start = start_date.year
-    calc_year_stop = end_date.year
-    calc_month_start = start_date.month
-    calc_month_stop = end_date.month
-
-    # Init logging
-    base_log_dir = conf.dirs.getpath('log_dir')
-    log_level = conf.general.get("log_level")
-    if test:
-        base_log_dir = base_log_dir.parent / f"{base_log_dir.name}_test"
-    log_dir = base_log_dir / f"calc_dias_{datetime.datetime.now():%Y-%m-%d_%H-%M-%S}"
-
-    # Clean test log dir if it exist
-    if test and base_log_dir.exists():
-        shutil.rmtree(base_log_dir)
-
-    global logger
-    logger = log_helper.main_log_init(log_dir, __name__, log_level)
-    logger.info(f"Config used: \n{conf.pformat_config()}")
-
-    if test:
-        logger.info(
-            f"As we are testing, clean all test logging and use new log_dir: {log_dir}"
-        )
-
-    # Write the consolidated config as ini file again to the run dir
-    config_used_path = log_dir / "config_used.ini"
-    with open(config_used_path, "w") as config_used_file:
-        conf.config.write(config_used_file)
-
-    # TODO: this shouldn't be hardcoded!
-    input_parcel_filename = conf.calc_timeseries_params.getpath("input_parcel_filename")
-    input_features_filename = Path(
-        f"{input_parcel_filename.stem}_bufm5{input_parcel_filename.suffix}"
-    )
-    input_preprocessed_dir = conf.dirs.getpath("input_preprocessed_dir")
-    input_features_path = input_preprocessed_dir / input_features_filename
-
-    # Init output dir
-    timeseries_per_image_dir = conf.dirs.getpath("timeseries_per_image_dir")
-    if not test:
-        output_basedir = timeseries_per_image_dir
-    else:
-        output_basedir = Path(f"{str(timeseries_per_image_dir)}_test")
-        logger.info(f"As we are testing, use test output basedir: {output_basedir}")
-    output_dir = output_basedir / input_features_filename.stem
-    if test:
-        if output_dir.exists():
-            logger.info(f"As we are only testing, clean the output dir: {output_dir}")
-            # By adding a / at the end, only the contents are recursively deleted
-            shutil.rmtree(str(output_dir) + os.sep)
-
-    # Temp dir + clean contents from it.
-    temp_dir = conf.dirs.getpath("temp_dir") / "calc_dias"
-    logger.info(f"Clean the temp dir {temp_dir}")
-    if temp_dir.exists():
-        # By adding a / at the end, only the contents are recursively deleted
-        shutil.rmtree(str(temp_dir) + os.sep)
-
-    """
-    # TEST to extract exact footprint from S1 image...
-    path = "/mnt/NAS3/CARD/FLANDERS/S1A/L1TC/2017/01/01/S1A_IW_GRDH_1SDV_20170101T055005_20170101T055030_014634_017CB9_Orb_RBN_RTN_Cal_TC.CARD/S1A_IW_GRDH_1SDV_20170101T055005_20170101T055030_014634_017CB9_Orb_RBN_RTN_Cal_TC.data/Gamma0_VH.img"
-    image = rasterio.open(path)
-    geoms = list(rasterio.features.dataset_features(src=image, as_mask=True, precision=5))
-    footprint = gpd.GeoDataFrame.from_features(geoms)
-    logger.info(footprint)
-    footprint = footprint.simplify(0.00001)
-    logger.info(footprint)
-    logger.info("Ready")
-    # Start calculation
-    """
-
-    # Process S1 GRD images
-    input_image_paths = []
-    for year in range(calc_year_start, calc_year_stop + 1):
-        # TODO: works, but doesn't seem to be the most elegant code...
-        if year < calc_year_stop:
-            month_stop = 12
-        else:
-            month_stop = calc_month_stop
-        if year > calc_year_start:
-            month_start = 1
-        else:
-            month_start = calc_month_start
-        for month in range(calc_month_start, calc_month_stop + 1):
-            input_image_searchstr = (
-                f"/mnt/NAS*/CARD/FLANDERS/S1*/L1TC/{year}/{month:02d}/*/*.CARD"
-            )
-            input_image_paths.extend(glob.glob(input_image_searchstr))
-    logger.info(f"Found {len(input_image_paths)} S1 GRD images to process")
-
-    if test:
-        # Take only the x first images found while testing
-        input_image_paths = input_image_paths[:10]
-        logger.info(
-            f"As we are only testing, process only {len(input_image_paths)} test images"
-        )
-
-    input_image_paths = [
-        Path(input_image_path) for input_image_path in input_image_paths
-    ]
-
-    try:
-        calc_ts.calc_stats_per_image(
-            features_path=input_features_path,
-            id_column=conf.columns["id"],
-            image_paths=input_image_paths,
-            bands=["VV", "VH"],
-            output_dir=output_dir,
-            temp_dir=temp_dir,
-            log_dir=log_dir,
-            log_level=log_level,
-        )
-    except Exception as ex:
-        logger.exception(ex)
-
-    # Process S2 images
-    input_image_paths = []
-    for year in range(calc_year_start, calc_year_stop + 1):
-        # TODO: works, but doesn't seem to be the most elegant code...
-        if year < calc_year_stop:
-            month_stop = 12
-        else:
-            month_stop = calc_month_stop
-        if year > calc_year_start:
-            month_start = 1
-        else:
-            month_start = calc_month_start
-        for month in range(month_start, month_stop + 1):
-            input_image_searchstr = (
-                f"/mnt/NAS*/CARD/FLANDERS/S2*/L2A/{year}/{month:02d}/*/*.SAFE"
-            )
-            logger.info(f"Search for {input_image_searchstr}")
-            input_image_paths.extend(glob.glob(input_image_searchstr))
-    logger.info(f"Found {len(input_image_paths)} S2 images to process")
-
-    if test:
-        # Take only the x first images found while testing
-        input_image_paths = input_image_paths[:10]
-        logger.info(
-            f"As we are only testing, process only {len(input_image_paths)} test images"
-        )
-
-    # TODO: refactor underlying code so the SCL band is used regardless of it being
-    # passed here
-    max_cloudcover_pct = conf.timeseries.getfloat("max_cloudcover_pct")
-    input_image_paths = [
-        Path(input_image_path) for input_image_path in input_image_paths
-    ]
-
-    try:
-        calc_ts.calc_stats_per_image(
-            features_path=input_features_path,
-            id_column=conf.columns["id"],
-            image_paths=input_image_paths,
-            bands=conf.timeseries.getlist("s2bands"),
-            output_dir=output_dir,
-            temp_dir=temp_dir,
-            log_dir=log_dir,
-            log_level=log_level,
-            max_cloudcover_pct=max_cloudcover_pct,
-        )
-    except Exception as ex:
-        logger.exception(ex)
-
-    # Process S1 Coherence images
-    input_image_paths = []
-    for year in range(calc_year_start, calc_year_stop + 1):
-        # TODO: works, but doesn't seem to be the most elegant code...
-        if year < calc_year_stop:
-            month_stop = 12
-        else:
-            month_stop = calc_month_stop
-        if year > calc_year_start:
-            month_start = 1
-        else:
-            month_start = calc_month_start
-        for month in range(calc_month_start, calc_month_stop + 1):
-            input_image_searchstr = (
-                f"/mnt/NAS*/CARD/FLANDERS/S1*/L1CO/{year}/{month:02d}/*/*.CARD"
-            )
-            input_image_paths.extend(glob.glob(input_image_searchstr))
-    logger.info(f"Found {len(input_image_paths)} S1 Coherence images to process")
-
-    if test:
-        # Take only the x first images found while testing
-        input_image_paths = input_image_paths[:10]
-        logger.info(
-            f"As we are only testing, process only {len(input_image_paths)} test images"
-        )
-
-    input_image_paths = [
-        Path(input_image_path) for input_image_path in input_image_paths
-    ]
-
-    try:
-        calc_ts.calc_stats_per_image(
-            features_path=input_features_path,
-            id_column=conf.columns["id"],
-            image_paths=input_image_paths,
-            bands=["VV", "VH"],
-            output_dir=output_dir,
-            temp_dir=temp_dir,
-            log_dir=log_dir,
-            log_level=log_level,
-        )
-    except Exception as ex:
-        logger.exception(ex)
-
-
-if __name__ == "__main__":
-    raise Exception("Not implemented")
+# -*- coding: utf-8 -*-
+"""
+Calaculate the timeseries data per image on DIAS.
+"""
+
+import datetime
+import glob
+import os
+from pathlib import Path
+import shutil
+from typing import List
+import dateutil.parser
+
+# Import geofilops here already, if tensorflow is loaded first leads to dll load errors
+import geofileops as gfo  # noqa: F401
+
+from cropclassification.helpers import config_helper as conf
+from cropclassification.helpers import log_helper
+from cropclassification.util import zonal_stats_bulk
+from cropclassification.preprocess import _timeseries_helper as ts_helper
+
+
+def calc_timeseries_task(config_paths: List[Path], default_basedir: Path):
+    """
+    Runs a calculation of timeseries with the settings in the config_paths.
+
+    Args:
+        config_paths (List[Path]): the config files to load
+        default_basedir (Path): the dir to resolve relative paths in the config
+            file to.
+
+    Raises:
+        Exception: [description]
+        Exception: [description]
+    """
+    # Read the configuration files
+    conf.read_config(config_paths, default_basedir=default_basedir)
+
+    test = conf.calc_timeseries_params.getboolean("test")
+
+    # As we want a weekly calculation, get nearest monday for start and stop day
+    start_date = ts_helper.get_monday(
+        conf.marker["start_date_str"]
+    )  # output: vb 2018_2_1 - maandag van week 2 van 2018
+    end_date = ts_helper.get_monday(conf.marker["end_date_str"])
+
+    calc_year_start = start_date.year
+    calc_year_stop = end_date.year
+    calc_month_start = start_date.month
+    calc_month_stop = end_date.month
+
+    # Init logging
+    base_log_dir = conf.dirs.getpath("log_dir")
+    log_level = conf.general.get("log_level")
+    if test:
+        base_log_dir = base_log_dir.parent / f"{base_log_dir.name}_test"
+    log_dir = base_log_dir / f"calc_dias_{datetime.datetime.now():%Y-%m-%d_%H-%M-%S}"
+
+    # Clean test log dir if it exist
+    if test and base_log_dir.exists():
+        shutil.rmtree(base_log_dir)
+
+    global logger
+    logger = log_helper.main_log_init(log_dir, __name__, log_level)
+    logger.info(f"Config used: \n{conf.pformat_config()}")
+
+    if test:
+        logger.info(
+            f"As we are testing, clean all test logging and use new log_dir: {log_dir}"
+        )
+
+    # Write the consolidated config as ini file again to the run dir
+    config_used_path = log_dir / "config_used.ini"
+    with open(config_used_path, "w") as config_used_file:
+        conf.config.write(config_used_file)
+
+    # TODO: this shouldn't be hardcoded!
+    input_parcel_filename = conf.calc_timeseries_params.getpath("input_parcel_filename")
+    input_features_filename = Path(
+        f"{input_parcel_filename.stem}_bufm5{input_parcel_filename.suffix}"
+    )
+    input_preprocessed_dir = conf.dirs.getpath("input_preprocessed_dir")
+    input_features_path = input_preprocessed_dir / input_features_filename
+
+    # Init output dir
+    timeseries_per_image_dir = conf.dirs.getpath("timeseries_per_image_dir")
+    if not test:
+        output_basedir = timeseries_per_image_dir
+    else:
+        output_basedir = Path(f"{str(timeseries_per_image_dir)}_test")
+        logger.info(f"As we are testing, use test output basedir: {output_basedir}")
+    output_dir = output_basedir / input_features_filename.stem
+    if test:
+        if output_dir.exists():
+            logger.info(f"As we are only testing, clean the output dir: {output_dir}")
+            # By adding a / at the end, only the contents are recursively deleted
+            shutil.rmtree(str(output_dir) + os.sep)
+
+    # Temp dir + clean contents from it.
+    temp_dir = conf.dirs.getpath("temp_dir") / "calc_dias"
+    logger.info(f"Clean the temp dir {temp_dir}")
+    if temp_dir.exists():
+        # By adding a / at the end, only the contents are recursively deleted
+        shutil.rmtree(str(temp_dir) + os.sep)
+
+    # Process S1 GRD images
+    input_image_paths = []
+    for year in range(calc_year_start, calc_year_stop + 1):
+        # TODO: works, but doesn't seem to be the most elegant code...
+        if year < calc_year_stop:
+            month_stop = 12
+        else:
+            month_stop = calc_month_stop
+        if year > calc_year_start:
+            month_start = 1
+        else:
+            month_start = calc_month_start
+        for month in range(calc_month_start, calc_month_stop + 1):
+            input_image_searchstr = (
+                f"/mnt/NAS*/CARD/FLANDERS/S1*/L1TC/{year}/{month:02d}/*/*.CARD"
+            )
+            input_image_paths.extend(glob.glob(input_image_searchstr))
+    logger.info(f"Found {len(input_image_paths)} S1 GRD images in the time period")
+
+    # Verify which S1 images we actually want to process...
+    tmp_input_image_paths = []
+    esaSwitchedProcessingMethod = dateutil.parser.isoparse("2021-02-23").timestamp()
+    for input_image_path in input_image_paths:
+        input_image_path = Path(input_image_path)
+        # Get more detailed info about the image
+        try:
+            image_info = zonal_stats_bulk.get_image_info(input_image_path)
+        except Exception:
+            # If not possible to get info for image, log and skip it
+            logger.exception(f"SKIP image: error getting info for {input_image_path}")
+            continue
+
+        # Fast-24h <- 2021-02-23 -> NRT-3H
+        productTimelinessCategory = (
+            "Fast-24h"
+            if dateutil.parser.isoparse(
+                image_info.extra["acquisition_date"]
+            ).timestamp()
+            < esaSwitchedProcessingMethod
+            else "NRT-3h"
+        )
+
+        # If sentinel1 and wrong productTimelinessCategory, skip: we only
+        # want 1 type to evade images used twice
+        if (
+            image_info.imagetype.startswith("S1")
+            and image_info.extra["productTimelinessCategory"]
+            != productTimelinessCategory
+        ):
+            logger.info(
+                f"SKIP image, productTimelinessCategory should be "
+                f"'{productTimelinessCategory}', but is: "
+                f"{image_info.extra['productTimelinessCategory']} for "
+                f"{input_image_path}"
+            )
+            continue
+
+        tmp_input_image_paths.append(input_image_path)
+
+    input_image_paths = tmp_input_image_paths
+    logger.info(f"Found {len(input_image_paths)} S1 GRD images to process")
+
+    if test:
+        # Take only the x first images found while testing
+        input_image_paths = input_image_paths[:10]
+        logger.info(
+            f"As we are only testing, process only {len(input_image_paths)} test images"
+        )
+
+    try:
+        images_bands = [(path, ["VV", "VH"]) for path in input_image_paths]
+        zonal_stats_bulk.zonal_stats(
+            vector_path=input_features_path,
+            id_column=conf.columns["id"],
+            rasters_bands=images_bands,
+            output_dir=output_dir,
+            temp_dir=temp_dir,
+            log_dir=log_dir,
+            log_level=log_level,
+        )
+    except Exception as ex:
+        logger.exception(ex)
+
+    # Process S2 images
+    input_image_paths = []
+    for year in range(calc_year_start, calc_year_stop + 1):
+        # TODO: works, but doesn't seem to be the most elegant code...
+        if year < calc_year_stop:
+            month_stop = 12
+        else:
+            month_stop = calc_month_stop
+        if year > calc_year_start:
+            month_start = 1
+        else:
+            month_start = calc_month_start
+        for month in range(month_start, month_stop + 1):
+            input_image_searchstr = (
+                f"/mnt/NAS*/CARD/FLANDERS/S2*/L2A/{year}/{month:02d}/*/*.SAFE"
+            )
+            logger.info(f"Search for {input_image_searchstr}")
+            input_image_paths.extend(glob.glob(input_image_searchstr))
+    logger.info(f"Found {len(input_image_paths)} S2 images to process")
+
+    if test:
+        # Take only the x first images found while testing
+        input_image_paths = input_image_paths[:10]
+        logger.info(
+            f"As we are only testing, process only {len(input_image_paths)} test images"
+        )
+
+    # TODO: refactor underlying code so the SCL band is used regardless of it being
+    # passed here
+    max_cloudcover_pct = conf.timeseries.getfloat("max_cloudcover_pct")
+    # Verify which S1 images we actually want to process...
+    tmp_input_image_paths = []
+    for input_image_path in input_image_paths:
+        input_image_path = Path(input_image_path)
+
+        # Get more detailed info about the image
+        try:
+            image_info = zonal_stats_bulk.get_image_info(input_image_path)
+        except Exception:
+            # If not possible to get info for image, log and skip it
+            logger.exception(f"SKIP image: error getting info for {input_image_path}")
+            continue
+
+        # If sentinel2 and cloud coverage too high... skip
+        if (
+            max_cloudcover_pct >= 0
+            and image_info.imagetype.startswith("S2")
+            and image_info.extra["Cloud_Coverage_Assessment"] > max_cloudcover_pct
+        ):
+            logger.info(
+                "SKIP image, Cloud_Coverage_Assessment: "
+                f"{image_info.extra['Cloud_Coverage_Assessment']:0.2f} > "
+                f"{max_cloudcover_pct} for {input_image_path}"
+            )
+            continue
+
+        tmp_input_image_paths.append(input_image_path)
+
+    try:
+        bands = conf.timeseries.getlist("s2bands")
+        images_bands = [(path, bands) for path in input_image_paths]
+        zonal_stats_bulk.zonal_stats(
+            vector_path=input_features_path,
+            id_column=conf.columns["id"],
+            rasters_bands=images_bands,
+            output_dir=output_dir,
+            temp_dir=temp_dir,
+            log_dir=log_dir,
+            log_level=log_level,
+        )
+    except Exception as ex:
+        logger.exception(ex)
+
+    # Process S1 Coherence images
+    input_image_paths = []
+    for year in range(calc_year_start, calc_year_stop + 1):
+        # TODO: works, but doesn't seem to be the most elegant code...
+        if year < calc_year_stop:
+            month_stop = 12
+        else:
+            month_stop = calc_month_stop
+        if year > calc_year_start:
+            month_start = 1
+        else:
+            month_start = calc_month_start
+        for month in range(calc_month_start, calc_month_stop + 1):
+            input_image_searchstr = (
+                f"/mnt/NAS*/CARD/FLANDERS/S1*/L1CO/{year}/{month:02d}/*/*.CARD"
+            )
+            input_image_paths.extend(glob.glob(input_image_searchstr))
+    logger.info(f"Found {len(input_image_paths)} S1 Coherence images to process")
+
+    if test:
+        # Take only the x first images found while testing
+        input_image_paths = input_image_paths[:10]
+        logger.info(
+            f"As we are only testing, process only {len(input_image_paths)} test images"
+        )
+
+    input_image_paths = [
+        Path(input_image_path) for input_image_path in input_image_paths
+    ]
+
+    try:
+        images_bands = [(path, ["VV", "VH"]) for path in input_image_paths]
+        zonal_stats_bulk.zonal_stats(
+            vector_path=input_features_path,
+            id_column=conf.columns["id"],
+            rasters_bands=images_bands,
+            output_dir=output_dir,
+            temp_dir=temp_dir,
+            log_dir=log_dir,
+            log_level=log_level,
+        )
+    except Exception as ex:
+        logger.exception(ex)
+
+
+if __name__ == "__main__":
+    raise Exception("Not implemented")
```

### Comparing `cropclassification-0.1.0a2/cropclassification/general.ini` & `cropclassification-0.1.1/cropclassification/general.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,257 +1,245 @@
-# This is a config file with the shared/default settings for all markers. 
-
-# The job section contains information about the (cropclassification) task you want to run 
-[task]
-
-# The action you want to run:
-#    - calc_timeseries: calculate a Sentinel timeseries for a file with polygons
-#    - calc_maker: calculate a marker
-action = MUST_OVERRIDE
-
-# Extra config files to load, in addition to general defaults
-extra_config_files_to_load = MUST_OVERRIDE
-
-# The calc_marker_params section contains information to run a calc_marker task
-[calc_timeseries_params]
-
-# input files
-input_parcel_filename = MUST_OVERRIDE
-# if you wandt to do a test run, set to True
-test = False
-
-# The calc_marker_params section contains information to run a calc_marker task
-[calc_marker_params]
-
-# The type of the input file: typically country code
-country_code = BEFL
-# The filename of the vector (polygon) geofile
-input_parcel_filename = MUST_OVERRIDE
-# The type of the input file (= which preprocessing is needed/can be done)  
-input_parcel_filetype = ${country_code}
-# The lookup table (LUT) file where classes to classify to are specified
-classes_refe_filename = MUST_OVERRIDE
-# A groundtruth file for extra reporting, optional
-input_groundtruth_filename
-# The model to use if you want to reuse one instead of training one, optional
-input_model_to_use_relativepath
-# Do you want to reuse the last run dir for this marker run
-reuse_last_run_dir = False
-# Do you want to reuse the config used in the run dir you want to reuse
-reuse_last_run_dir_config = False
-
-# The general section contains some general confiuration ;-)
-[general]
-
-# File format (extension) to use for structured (table) data
-data_ext = .sqlite
-# File format (extension) to use for data that is output data (should be easy to use)
-output_ext = .tsv
-# File format for intermediary geo files (remark: gee needs .shp as input)
-geofile_ext = .gpkg
-
-# The log level to use
-log_level = INFO
-
-# Constants for types of aggregation to use
-# Mean value of the pixels values in a parcel.
-PARCELDATA_AGGRAGATION_MEAN = mean
-# Median value of the pixels values in a parcel.
-PARCELDATA_AGGRAGATION_MEDIAN = median
-# std dev of the values of the pixels in a parcel
-PARCELDATA_AGGRAGATION_STDDEV = std
-
-# Constants for types of sensor data
-SENSORDATA_S1 = S1
-# Sentinel 1 data
-# Sentinel 1 data, in dB
-SENSORDATA_S1DB = S1dB
-# Sentinel 1 data, divided in Ascending and Descending passes
-SENSORDATA_S1_ASCDESC = S1AscDesc
-# Sentinel 1 data, in dB, divided in Ascending and Descending passes
-SENSORDATA_S1DB_ASCDESC = S1dBAscDesc
-# Sentinel 2 data
-SENSORDATA_S2 = S2
-# Sentinel 2 data (B2,B3,B4,B8) IF available for 95% or area
-SENSORDATA_S2gt95 = S2gt95
-
-#SENSORDATA_S1_COHERENCE
-SENSORDATA_S1_COHERENCE = S1Coh
-
-[marker]
-# markertype, must be overriden in child ini files
-markertype = MUST_OVERRIDE
-
-# Year to use, should be overridden when running
-year = MUST_OVERRIDE
-
-# start date of timeseries data to use
-# remarks: nearest monday will be used + year will be replace in run-time
-start_date_str = ${year}-03-27 
-# end date of timeseries data to use
-# remarks: end date is NOT inclusive + year will be replace in run-time
-end_date_str = ${year}-08-10
-# negative buffer to apply to input parcels
-buffer = 5
-# minimum number of pixels that should be inside the buffered input parcels
-min_nb_pixels = -2 
-# minimum number of pixels that should be inside the buffered input parcels used when training
-min_nb_pixels_train = ${marker:min_nb_pixels}
-
-# classes that will be ignored for training + won't receive a prediction
-classes_to_ignore = ${classes_to_ignore_default}
-# define default ignores here, so it is easy to ADD extra for specific markers
-classes_to_ignore_default = IGNORE_DIFFICULT_PERMANENT_CLASS, IGNORE_UNIMPORTANT, IGNORE_NOT_ENOUGH_SAMPLES, IGNORE_EARLY_CROP, IGNORE_LATE_CROP, IGNORE_NEW_GRASSLAND
-
-# classes that should be ignored for training, but have to get a prediction
-classes_to_ignore_for_train = ${classes_to_ignore_for_train_default}
-# define default ignores here, so it is easy to ADD extra for specific markers
-classes_to_ignore_for_train_default = UNKNOWN
-
-# classes that should specified as unimportant in the reporting
-# Remark: this doesn't influence the training or predicting, these need to be set in 
-# the other paremeters!
-classes_to_ignore_unimportant = ${classes_to_ignore_unimportant_default}
-# define default ignores here, so it is easy to ADD extra for specific markers
-classes_to_ignore_unimportant_default = IGNORE_UNIMPORTANT
-
-# strategy to balance the training dataset for the marker. Possible values:
-#   * BALANCING_STRATEGY_NONE: don't apply any balancing: 20% of the input samples per class is used for training
-#   * BALANCING_STRATEGY_MEDIUM: 80% of input data is used for training, with maximum 10.000 samples per class and minimum 1.000 (samples will be duplicated if needed)
-#   * BALANCING_STRATEGY_MEDIUM2: 80% of input data is used for training, with maximum 10.000 samples per class depending on input count + minimum 1.000 (samples will be duplicated if needed)
-#   * BALANCING_STRATEGY_UPPER_LIMIT: 80% of input data is used for training, with a maximum of 10.000 samples per class
-#   * BALANCING_STRATEGY_PROPORTIONAL_GROUPS: 80% of input data is used for training, but for classes with > 10.000 samples +- only half of those are used  
-#   * BALANCING_STRATEGY_EQUAL: for each input class, the same amount of samples is used as training. For classes with few samples, (samples will be duplicated if needed)
-balancing_strategy = BALANCING_STRATEGY_MEDIUM2
-
-# The sensor data to be used for this marker
-sensordata_to_use = ${general:SENSORDATA_S1_ASCDESC}, ${general:SENSORDATA_S2gt95}
-# The aggregation type to use on parcel level
-parceldata_aggregations_to_use = ${general:PARCELDATA_AGGRAGATION_MEAN}
-
-# Postprocess...
-postprocess_to_groups = 
-
-[timeseries]
-# The way timeseries are calculated
-#     * gee: google earth engine
-#     * onda: ONDA DIAS
-timeseries_calc_type = onda
-
-# The maximum percentage cloudcover an (S2) image can have to be used
-max_cloudcover_pct = 15
-
-# The min percentage of parcels that need to have valid data for a time+sensor to use it 
-min_parcels_with_data_pct = 90
-
-# Bands to extract for S2 images 
-s2bands = B02-10m, B03-10m, B04-10m, B08-10m, B11-20m, B12-20m, SCL-20m
-
-[preprocess]
-# 
-dedicated_data_columns = ${columns:id}, ${columns:class}, ${columns:class}_orig, ${columns:class_declared}, ${columns:class_declared}_orig, ${columns:pixcount_s1s2}
-extra_export_columns = CODE_OBJ, LAYER_ID, PRC_ID, VERSIENR, GWSCOD_H
-
-# The way the classtype needs to be prepared
-classtype_to_prepare = ${marker:markertype}
-# The way the classtype for groundtruth needs to be prepared
-classtype_to_prepare_groundtruth = ${classtype_to_prepare}-GROUNDTRUTH
-
-[classifier]
-# The classifier type to use. Currently supported types:
-#     * keras_multilayer_perceptron (using keras)
-#     * multilayer_perceptron (using sklearn)
-#     * nearestneighbour
-#     * randomforest
-#     * svm
-classifier_type = keras_multilayer_perceptron
-# The extension of the file format to save the trained model to
-classifier_ext = .hdf5
-
-# For multilayer_perceptron, the hidden layer size(s) (as a komma seperated list)
-multilayer_perceptron_hidden_layer_sizes = 100, 100
-# For multilayer_perceptron, the percentage dropout to use between the hidden layers
-multilayer_perceptron_dropout_pct = 30
-# For multilayer_perceptron, the maximum number of iterations when training
-multilayer_perceptron_max_iter = 1000
-multilayer_perceptron_learning_rate_init = 0.001
-
-# For randomforest, the maximum number of trees to create
-randomforest_n_estimators = 200
-# For randomforest, the maximum depth of trees to create
-randomforest_max_depth = 35
-
-[postprocess]
-# Doubt: if highest probability < 2*second probability  
-doubt_proba1_st_2_x_proba2 = MUST_OVERRIDE
-# Doubt: if prediction == input class and highest probability < thresshold
-# Remark: should be floating point number from 0 till 1  
-doubt_pred_eq_input_proba1_st_thresshold = MUST_OVERRIDE
-# Doubt: if prediction != input class and highest probability < thresshold  
-# Remark: should be floating point number from 0 till 1
-doubt_pred_ne_input_proba1_st_thresshold = MUST_OVERRIDE
-
-[columns]
-# The columns to include in the final output file
-output_columns = LAYER_ID, PRC_ID, VERSIENR, markercode, run_id, ${prediction_full_alpha}, ${prediction_cons_status}, cons_date, pred1, pred1_prob, pred2, pred2_prob, pred3, pred3_prob, modify_date
-
-# Column name of the id column
-id = UID
-# Column name of the geom column
-geom = geometry
-
-# Column name of the crop on the parcel. For parcels that received an on the 
-# spot check (already), this column contains the corrected data.
-crop = GWSCOD_H
-# Column name of the crop on the parcel as declared by the farmer, even for
-# parcels that already received an on the spot check.
-crop_declared = GWSCOD_H_A
-# Column name of the classes to prepropress to in the refe file
-class_refe = classname_refe
-# Column name of the class, after preprocessing to optimize the classification
-# For parcels that received an on the spot check, the class contains the 
-# verified data so the training input is optimal
-class = classname
-# Column name of the class as declared by the farmer, even if the parcels that
-# (already) received an on the spot check
-class_declared = classname_declared
-# Column name of the class to use for balancing the training dataset
-class_balancing = ${class}
-# Column name of the class of the verified groundtruth
-class_groundtruth = classname_gt
-# Column name of the count of the number of pixels for sentinel1/2 images
-pixcount_s1s2 = pixcount
-# Column name of the consolidated prediction: can be doubt, not_enough_pixels,...
-prediction_cons = pred_consolidated
-# Column name of the status of the consolidated prediction: can be OK, NOK
-prediction_cons_status = pred_cons_status
-# Column name of the status of the prediction to use for the alpa error
-prediction_full_alpha = pred_full_alpha
-# Column name of the detailed conclusion based on standard prediction
-prediction_conclusion_detail = pred_conclusion_detail
-# Column name of the detailed conclusion based on prediction with doubt
-prediction_conclusion_detail_withdoubt = pred_conclusion_detail_withdoubt
-# Column name of the detailed conclusion based on consolidated prediction
-prediction_conclusion_detail_cons = pred_conclusion_detail_cons
-# Column name of the detailed conclusion based on full alpha prediction
-prediction_conclusion_detail_full_alpha = pred_conclusion_detail_full_alpha
-# Column name of the conclusion based on consolidated prediction
-prediction_conclusion_cons = pred_conclusion_cons
-
-[dirs]
-# Directories to use
-# data_dir can be specified as a relative path which will be resolved to
-# the parent dir of the tasks dir 
-data_dir = .
-temp_dir = ${dirs:data_dir}/tmp
-# marker_basedir can be specified as a relative path which will be resolved to
-# the parent dir of the tasks dir
-marker_basedir = .
-marker_dir = ${dirs:marker_basedir}/${marker:year}_${marker:markertype}
-timeseries_periodic_dir = ${dirs:data_dir}/_ts_periodic
-timeseries_per_image_dir = ${dirs:data_dir}/_ts_per_image
-input_dir = ${dirs:data_dir}/_inputdata
-input_preprocessed_dir = ${dirs:data_dir}/_inputdata_preprocessed
-model_dir = ${dirs:data_dir}/_models
-refe_dir = ${dirs:data_dir}/_refe
-log_dir = ${dirs:marker_basedir}/log
-gee = users/pieter_roggemans/
+# This is a config file with the shared/default settings for all markers. 
+
+# The job section contains information about the (cropclassification) task you want to run 
+[task]
+
+# The action you want to run:
+#    - calc_timeseries: calculate a Sentinel timeseries for a file with polygons
+#    - calc_maker: calculate a marker
+action = MUST_OVERRIDE
+
+# Extra config files to load, in addition to general defaults
+extra_config_files_to_load = MUST_OVERRIDE
+
+# The calc_marker_params section contains information to run a calc_marker task
+[calc_timeseries_params]
+
+# input files
+input_parcel_filename = MUST_OVERRIDE
+# if you wandt to do a test run, set to True
+test = False
+
+# The calc_marker_params section contains information to run a calc_marker task
+[calc_marker_params]
+
+# The type of the input file: typically country code
+country_code = BEFL
+# The filename of the vector (polygon) geofile
+input_parcel_filename = MUST_OVERRIDE
+# The type of the input file (= which preprocessing is needed/can be done)  
+input_parcel_filetype = ${country_code}
+# The lookup table (LUT) file where classes to classify to are specified
+classes_refe_filename = MUST_OVERRIDE
+# A groundtruth file for extra reporting, optional
+input_groundtruth_filename
+# The model to use if you want to reuse one instead of training one, optional
+input_model_to_use_relativepath
+# Do you want to reuse the last run dir for this marker run
+reuse_last_run_dir = False
+# Do you want to reuse the config used in the run dir you want to reuse
+reuse_last_run_dir_config = False
+
+# The general section contains some general confiuration ;-)
+[general]
+
+# File format (extension) to use for structured (table) data
+data_ext = .sqlite
+# File format (extension) to use for data that is output data (should be easy to use)
+output_ext = .tsv
+# File format for intermediary geo files (remark: gee needs .shp as input)
+geofile_ext = .gpkg
+
+# The log level to use
+log_level = INFO
+
+[marker]
+# markertype, must be overriden in child ini files
+markertype = MUST_OVERRIDE
+
+# Year to use, should be overridden when running
+year = MUST_OVERRIDE
+
+# start date of timeseries data to use
+# remarks: nearest monday will be used + year will be replace in run-time
+start_date_str = ${year}-03-27 
+# end date of timeseries data to use
+# remarks: end date is NOT inclusive + year will be replace in run-time
+end_date_str = ${year}-08-10
+# negative buffer to apply to input parcels
+buffer = 5
+# minimum number of pixels that should be inside the buffered input parcels
+min_nb_pixels = -2 
+# minimum number of pixels that should be inside the buffered input parcels used when training
+min_nb_pixels_train = ${marker:min_nb_pixels}
+
+# classes that will be ignored for training + won't receive a prediction
+classes_to_ignore = ${classes_to_ignore_default}
+# define default ignores here, so it is easy to ADD extra for specific markers
+classes_to_ignore_default = IGNORE_DIFFICULT_PERMANENT_CLASS, IGNORE_UNIMPORTANT, IGNORE_NOT_ENOUGH_SAMPLES, IGNORE_EARLY_CROP, IGNORE_LATE_CROP, IGNORE_NEW_GRASSLAND
+
+# classes that should be ignored for training, but have to get a prediction
+classes_to_ignore_for_train = ${classes_to_ignore_for_train_default}
+# define default ignores here, so it is easy to ADD extra for specific markers
+classes_to_ignore_for_train_default = UNKNOWN
+
+# classes that should specified as unimportant in the reporting
+# Remark: this doesn't influence the training or predicting, these need to be set in 
+# the other paremeters!
+classes_to_ignore_unimportant = ${classes_to_ignore_unimportant_default}
+# define default ignores here, so it is easy to ADD extra for specific markers
+classes_to_ignore_unimportant_default = IGNORE_UNIMPORTANT
+
+# strategy to balance the training dataset for the marker. Possible values:
+#   * BALANCING_STRATEGY_NONE: don't apply any balancing: 20% of the input samples per class is used for training
+#   * BALANCING_STRATEGY_MEDIUM: 80% of input data is used for training, with maximum 10.000 samples per class and minimum 1.000 (samples will be duplicated if needed)
+#   * BALANCING_STRATEGY_MEDIUM2: 80% of input data is used for training, with maximum 10.000 samples per class depending on input count + minimum 1.000 (samples will be duplicated if needed)
+#   * BALANCING_STRATEGY_UPPER_LIMIT: 80% of input data is used for training, with a maximum of 10.000 samples per class
+#   * BALANCING_STRATEGY_PROPORTIONAL_GROUPS: 80% of input data is used for training, but for classes with > 10.000 samples +- only half of those are used  
+#   * BALANCING_STRATEGY_EQUAL: for each input class, the same amount of samples is used as training. For classes with few samples, (samples will be duplicated if needed)
+balancing_strategy = BALANCING_STRATEGY_MEDIUM2
+
+# Sensordata to use for the markers. This is a list of ImageProfile names:
+#   - S1dB: Sentinel 1 data, in dB
+#   - S1ascDesc: Sentinel 1 data, divided in Ascending and Descending passes
+#   - S1dBAscDesc: Sentinel 1 data, in dB, divided in Ascending and Descending passes
+#   - S1Coh: Sentinel 1 coherence
+#   - S2gt95: Sentinel 2 data (B2,B3,B4,B8) IF available for 95% or area
+#
+#   - s2-landcover: Sentinel 2 landcover, based on SCL mask
+#   - s2-ndvi: Sentinel 2 ndvi
+#   - s2-agri: Sentinel 2 bands relevant for agriculture (B02, B03, B04, B08, B11, B12)
+#   - s1-grd-sigma0-asc: Sentinel 1 GRD, ascending orbit (VV, VH)
+#   - s1-grd-sigma0-desc: Sentinel 1 GRD, descending orbit (VV, VH)
+#   - s1-coh: Sentinel 1, 6 day or 12 day coherence, depending on availability (VV, VH)
+#
+# Optionally, it is possible to specify the bands of the ImageProfile to be used like this:
+#   eg. [..., {"s2-grd-sigma0-asc": ["VV", "VH"]}]
+sensordata_to_use = ["s2-agri", {"s1-grd-sigma0-asc": ["VV", "VH"]}, {"s1-grd-sigma0-desc": ["VV", "VH"]}]
+
+# The aggregation type to use on parcel level. Following options are avalable:
+#    - mean: the mean of the pixel values in a parcel
+#    - median: the median of the pixel values in a parcel
+#    - std: the standard deviation of the pixel values in a parcel
+parceldata_aggregations_to_use = median
+
+# Postprocess...
+postprocess_to_groups = 
+
+[timeseries]
+# The maximum percentage cloudcover an (S2) image can have to be used
+max_cloudcover_pct = 15
+
+# The min percentage of parcels that need to have valid data for a time+sensor to use it 
+min_parcels_with_data_pct = 90
+
+[preprocess]
+# 
+dedicated_data_columns = ${columns:id}, ${columns:class}, ${columns:class}_orig, ${columns:class_declared}, ${columns:class_declared}_orig, ${columns:pixcount_s1s2}
+extra_export_columns = CODE_OBJ, LAYER_ID, PRC_ID, VERSIENR, GWSCOD_H
+
+# The way the classtype needs to be prepared
+classtype_to_prepare = ${marker:markertype}
+# The way the classtype for groundtruth needs to be prepared
+classtype_to_prepare_groundtruth = ${classtype_to_prepare}-GROUNDTRUTH
+
+[classifier]
+# The classifier type to use. Currently supported types:
+#     * keras_multilayer_perceptron (using keras)
+#     * multilayer_perceptron (using sklearn)
+#     * nearestneighbour
+#     * randomforest
+#     * svm
+classifier_type = keras_multilayer_perceptron
+# The extension of the file format to save the trained model to
+classifier_ext = .hdf5
+
+# For multilayer_perceptron, the hidden layer size(s) (as a komma seperated list)
+multilayer_perceptron_hidden_layer_sizes = 100, 100
+# For multilayer_perceptron, the percentage dropout to use between the hidden layers
+multilayer_perceptron_dropout_pct = 30
+# For multilayer_perceptron, the maximum number of iterations when training
+multilayer_perceptron_max_iter = 1000
+multilayer_perceptron_learning_rate_init = 0.001
+
+# For randomforest, the maximum number of trees to create
+randomforest_n_estimators = 200
+# For randomforest, the maximum depth of trees to create
+randomforest_max_depth = 35
+
+[postprocess]
+# Doubt: if highest probability < 2*second probability  
+doubt_proba1_st_2_x_proba2 = MUST_OVERRIDE
+# Doubt: if prediction == input class and highest probability < thresshold
+# Remark: should be floating point number from 0 till 1  
+doubt_pred_eq_input_proba1_st_thresshold = MUST_OVERRIDE
+# Doubt: if prediction != input class and highest probability < thresshold  
+# Remark: should be floating point number from 0 till 1
+doubt_pred_ne_input_proba1_st_thresshold = MUST_OVERRIDE
+
+[columns]
+# The columns to include in the final output file
+output_columns = LAYER_ID, PRC_ID, VERSIENR, markercode, run_id, ${class}, ${prediction_full_alpha}, ${prediction_cons_status}, cons_date, pred1, pred1_prob, pred2, pred2_prob, pred3, pred3_prob, modify_date
+
+# Column name of the id column
+id = UID
+# Column name of the geom column
+geom = geometry
+
+# Column name of the crop on the parcel. For parcels that received an on the 
+# spot check (already), this column contains the corrected data.
+crop = GWSCOD_H
+# Column name of the crop on the parcel as declared by the farmer, even for
+# parcels that already received an on the spot check.
+crop_declared = GWSCOD_H_A
+# Column name of the classes to prepropress to in the refe file
+class_refe = classname_refe
+# Column name of the class, after preprocessing to optimize the classification
+# For parcels that received an on the spot check, the class contains the 
+# verified data so the training input is optimal
+class = classname
+# Column name of the class as declared by the farmer, even if the parcels that
+# (already) received an on the spot check
+class_declared = classname_declared
+# Column name of the class to use for balancing the training dataset
+class_balancing = ${class}
+# Column name of the class of the verified groundtruth
+class_groundtruth = classname_gt
+# Column name of the count of the number of pixels for sentinel1/2 images
+pixcount_s1s2 = pixcount
+# Column name of the consolidated prediction: can be doubt, not_enough_pixels,...
+prediction_cons = pred_consolidated
+# Column name of the status of the consolidated prediction: can be OK, NOK
+prediction_cons_status = pred_cons_status
+# Column name of the status of the prediction to use for the alpa error
+prediction_full_alpha = pred_full_alpha
+# Column name of the detailed conclusion based on standard prediction
+prediction_conclusion_detail = pred_conclusion_detail
+# Column name of the detailed conclusion based on prediction with doubt
+prediction_conclusion_detail_withdoubt = pred_conclusion_detail_withdoubt
+# Column name of the detailed conclusion based on consolidated prediction
+prediction_conclusion_detail_cons = pred_conclusion_detail_cons
+# Column name of the detailed conclusion based on full alpha prediction
+prediction_conclusion_detail_full_alpha = pred_conclusion_detail_full_alpha
+# Column name of the conclusion based on consolidated prediction
+prediction_conclusion_cons = pred_conclusion_cons
+
+[dirs]
+# Directories to use
+# data_dir can be specified as a relative path which will be resolved to
+# the parent dir of the tasks dir 
+data_dir = .
+# temp_dir can contain placeholder {tmp_dir}: resolves to the default system tempdir
+temp_dir = {tmp_dir}/cropclassification
+# marker_basedir can be specified as a relative path which will be resolved to
+# the parent dir of the tasks dir
+marker_basedir = .
+marker_dir = ${dirs:marker_basedir}/${marker:year}_${marker:markertype}
+images_periodic_dir = ${dirs:data_dir}/_images_periodic/${calc_marker_params:country_code}
+timeseries_periodic_dir = ${dirs:data_dir}/_ts_periodic
+timeseries_per_image_dir = ${dirs:data_dir}/_ts_per_image
+input_dir = ${dirs:data_dir}/_inputdata
+input_preprocessed_dir = ${dirs:data_dir}/_inputdata_preprocessed
+model_dir = ${dirs:data_dir}/_models
+refe_dir = ${dirs:data_dir}/_refe
+log_dir = ${dirs:marker_basedir}/log
+gee = users/pieter_roggemans/
```

### Comparing `cropclassification-0.1.0a2/cropclassification/helpers/dir_helper.py` & `cropclassification-0.1.1/cropclassification/helpers/dir_helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-"""
-Helper regarding directory operations.
-"""
-
-from datetime import datetime
-import os
-from pathlib import Path
-import re
-
-
-def create_run_dir(class_base_dir: Path, reuse_last_run_dir: bool) -> Path:
-    """
-    Create a new run dir, or get the last run dir.
-
-    Args
-        class_base_dir: the base dir to use to create the run dir in
-        reuse_last_run_dir: True to find the latest existing run dir and return that, False to create a new run dir
-    """
-
-    # Create class_base_dir if it doesn't exist
-    if not class_base_dir.exists():
-        os.makedirs(class_base_dir)
-
-    # Look for all existing run dirs
-    base_filename = f"Run_{datetime.now().strftime('%Y-%m-%d')}"
-    pattern = re.compile(base_filename + "_[0-9]{3}")
-    dir_list = [
-        x.path
-        for x in os.scandir(class_base_dir)
-        if x.is_dir() and re.search(pattern, x.path)
-    ]
-
-    # No dir yet with the patern -> return new one
-    if dir_list is None or not any(dir_list):
-        return class_base_dir / f"{base_filename}_{1:03d}"
-
-    # Get last run dir found... if we want to reuse it, return it
-    last_dir = sorted(dir_list, reverse=True)[0]
-    if reuse_last_run_dir:
-        return Path(last_dir)
-
-    # We don't want to reuse it, so create next one
-    _, last_dirname = os.path.split(last_dir)
-    last_iteration = int(last_dirname.replace(base_filename, "tmp").split("_")[1])
-    return class_base_dir / f"{base_filename}_{last_iteration + 1:03d}"
+"""
+Helper regarding directory operations.
+"""
+
+from datetime import datetime
+import os
+from pathlib import Path
+import re
+
+
+def create_run_dir(class_base_dir: Path, reuse_last_run_dir: bool) -> Path:
+    """
+    Create a new run dir, or get the last run dir.
+
+    Args
+        class_base_dir: the base dir to use to create the run dir in
+        reuse_last_run_dir: True to find the latest existing run dir and return that,
+            False to create a new run dir
+    """
+
+    # Create class_base_dir if it doesn't exist
+    if not class_base_dir.exists():
+        os.makedirs(class_base_dir)
+
+    # Look for all existing run dirs
+    base_filename = f"Run_{datetime.now().strftime('%Y-%m-%d')}"
+    pattern = re.compile(base_filename + "_[0-9]{3}")
+    dir_list = [
+        x.path
+        for x in os.scandir(class_base_dir)
+        if x.is_dir() and re.search(pattern, x.path)
+    ]
+
+    # No dir yet with the patern -> return new one
+    if dir_list is None or not any(dir_list):
+        return class_base_dir / f"{base_filename}_{1:03d}"
+
+    # Get last run dir found... if we want to reuse it, return it
+    last_dir = sorted(dir_list, reverse=True)[0]
+    if reuse_last_run_dir:
+        return Path(last_dir)
+
+    # We don't want to reuse it, so create next one
+    _, last_dirname = os.path.split(last_dir)
+    last_iteration = int(last_dirname.replace(base_filename, "tmp").split("_")[1])
+    return class_base_dir / f"{base_filename}_{last_iteration + 1:03d}"
```

### Comparing `cropclassification-0.1.0a2/cropclassification/helpers/log_helper.py` & `cropclassification-0.1.1/cropclassification/helpers/log_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-# -*- coding: utf-8 -*-
-"""
-Module to init logging.
-"""
-
-import datetime
-import logging
-import os
-from pathlib import Path
-
-
-def main_log_init(log_dir: Path, log_basefilename: str, log_level: str = "INFO"):
-
-    # Make sure the log dir exists
-    if not log_dir.exists():
-        os.makedirs(log_dir, exist_ok=True)
-
-    # Get root logger
-    logger = logging.getLogger("")
-
-    # Set the general maximum log level...
-    logger.setLevel(log_level)
-    for handler in logger.handlers:
-        handler.flush()
-        handler.close()
-
-    # Remove all handlers and add the ones I want again, so a new log file is created for each run
-    # Remark: the function removehandler doesn't seem to work?
-    logger.handlers = []
-
-    ch = logging.StreamHandler()
-    ch.setLevel(log_level)
-    # ch.setFormatter(logging.Formatter('%(levelname)s|%(name)s|%(message)s'))
-    # ch.setFormatter(logging.Formatter('%(asctime)s|%(levelname)s|%(name)s|%(message)s',
-    #                                  datefmt='%H:%M:%S,uuu'))
-    ch.setFormatter(
-        logging.Formatter(
-            fmt="%(asctime)s.%(msecs)03d|%(levelname)s|%(name)s|%(message)s",
-            datefmt="%H:%M:%S",
-        )
-    )
-    logger.addHandler(ch)
-
-    log_filepath = (
-        log_dir / f"{datetime.datetime.now():%Y-%m-%d_%H-%M-%S}_{log_basefilename}.log"
-    )
-    fh = logging.FileHandler(filename=str(log_filepath))
-    fh.setLevel(log_level)
-    fh.setFormatter(logging.Formatter("%(asctime)s|%(levelname)s|%(name)s|%(message)s"))
-    logger.addHandler(fh)
-
-    return logger
+# -*- coding: utf-8 -*-
+"""
+Module to init logging.
+"""
+
+import datetime
+import logging
+import os
+from pathlib import Path
+
+
+def main_log_init(log_dir: Path, log_basefilename: str, log_level: str = "INFO"):
+    # Make sure the log dir exists
+    if not log_dir.exists():
+        os.makedirs(log_dir, exist_ok=True)
+
+    # Get root logger
+    logger = logging.getLogger("")
+
+    # Set the general maximum log level...
+    logger.setLevel(log_level)
+    for handler in logger.handlers:
+        handler.flush()
+        handler.close()
+
+    # Remove all handlers and add the ones I want again, so a new log file is created
+    # for each run.
+    # Remark: the function removehandler doesn't seem to work?
+    logger.handlers = []
+
+    ch = logging.StreamHandler()
+    ch.setLevel(log_level)
+    # ch.setFormatter(logging.Formatter('%(levelname)s|%(name)s|%(message)s'))
+    # ch.setFormatter(logging.Formatter('%(asctime)s|%(levelname)s|%(name)s|%(message)s',
+    #                                  datefmt='%H:%M:%S,uuu'))
+    ch.setFormatter(
+        logging.Formatter(
+            fmt="%(asctime)s.%(msecs)03d|%(levelname)s|%(name)s|%(message)s",
+            datefmt="%H:%M:%S",
+        )
+    )
+    logger.addHandler(ch)
+
+    log_filepath = (
+        log_dir / f"{datetime.datetime.now():%Y-%m-%d_%H-%M-%S}_{log_basefilename}.log"
+    )
+    fh = logging.FileHandler(filename=str(log_filepath))
+    fh.setLevel(log_level)
+    fh.setFormatter(logging.Formatter("%(asctime)s|%(levelname)s|%(name)s|%(message)s"))
+    logger.addHandler(fh)
+
+    return logger
```

### Comparing `cropclassification-0.1.0a2/cropclassification/helpers/model_helper.py` & `cropclassification-0.1.1/cropclassification/helpers/model_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,467 +1,482 @@
-# -*- coding: utf-8 -*-
-"""
-Module with helper functions regarding (keras) models.
-"""
-
-import os
-import glob
-import logging
-from pathlib import Path
-from typing import Optional
-
-import pandas as pd
-from tensorflow import keras as kr
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-# logger.setLevel(logging.INFO)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def get_max_data_version(model_dir: Path) -> int:
-    """
-    Get the maximum data version a model exists for in the model_dir.
-
-    Args
-        model_dir: the dir to search models in
-    """
-    models_df = get_models(model_dir)
-    if models_df is not None and len(models_df.index) > 0:
-        train_data_version_max = models_df["train_data_version"].max()
-        return int(train_data_version_max)
-    else:
-        return -1
-
-
-def format_model_base_filename(
-    segment_subject: str, train_data_version: int, model_architecture: str
-) -> str:
-    """
-    Format the parameters into a model_base_filename.
-
-    Args
-        segment_subject: the segment subject
-        train_data_version: the version of the data used to train the model
-        model_architecture: the architecture of the model
-    """
-    retval = f"{segment_subject}_{train_data_version:02}_{model_architecture}"
-    return retval
-
-
-def format_model_filename(
-    segment_subject: str,
-    train_data_version: int,
-    model_architecture: str,
-    acc_train: float,
-    acc_val: float,
-    acc_combined: float,
-    epoch: int,
-) -> str:
-    """
-    Format the parameters into a model_filename.
-
-    Args
-        segment_subject: the segment subject
-        train_data_version: the version of the data used to train the model
-        model_architecture: the architecture of the model
-        acc_train: the accuracy reached for the training dataset
-        acc_val: the accuracy reached for the validation dataset
-        acc_combined: the average of the train and validation accuracy
-        epoch: the epoch during training that reached these model weights
-    """
-    base_filename = format_model_base_filename(
-        segment_subject=segment_subject,
-        train_data_version=train_data_version,
-        model_architecture=model_architecture,
-    )
-    filename = format_model_filename2(
-        model_base_filename=base_filename,
-        acc_train=acc_train,
-        acc_val=acc_val,
-        acc_combined=acc_combined,
-        epoch=epoch,
-    )
-    return filename
-
-
-def format_model_filename2(
-    model_base_filename: str,
-    acc_train: float,
-    acc_val: float,
-    acc_combined: float,
-    epoch: int,
-) -> str:
-    """
-    Format the parameters into a model_filename.
-
-    Args
-        model_base_filename: the base filename of the model
-        acc_train: the accuracy reached for the training dataset
-        acc_val: the accuracy reached for the validation dataset
-        acc_combined: the average of the train and validation accuracy
-        epoch: the epoch during training that reached these model weights
-    """
-    return f"{model_base_filename}_{acc_combined:.5f}_{acc_train:.5f}_{acc_val:.5f}_{epoch}.hdf5"
-
-
-def parse_model_filename(path: Path) -> dict:
-    """
-    Parse a model_filename to a dict containing the properties of the model:
-        * segment_subject: the segment subject
-        * train_data_version: the version of the data used to train the model
-        * model_architecture: the architecture of the model
-        * acc_train: the accuracy reached for the training dataset
-        * acc_val: the accuracy reached for the validation dataset
-        * acc_combined: the average of the train and validation accuracy
-        * epoch: the epoch during training that reached these model weights
-
-    Args
-        path: the path to the model file
-    """
-    # Prepare path to extract info
-    param_values = path.stem.split("_")
-
-    # Now extract fields...
-    segment_subject = param_values[0]
-    train_data_version = int(param_values[1])
-    model_architecture = param_values[2]
-    if len(param_values) > 3:
-        acc_combined = float(param_values[3])
-        acc_train = float(param_values[4])
-        acc_val = float(param_values[5])
-        epoch = int(param_values[6])
-    else:
-        acc_combined = 0.0
-        acc_train = 0.0
-        acc_val = 0.0
-        epoch = 0
-
-    return {
-        "path": path,
-        "filename": path.name,
-        "segment_subject": segment_subject,
-        "train_data_version": train_data_version,
-        "model_architecture": model_architecture,
-        "acc_combined": acc_combined,
-        "acc_train": acc_train,
-        "acc_val": acc_val,
-        "epoch": epoch,
-    }
-
-
-def get_models(
-    model_dir: Path, model_base_filename: Optional[str] = None
-) -> pd.DataFrame:
-    """
-    Return the list of models in the model_dir passed. It is returned as a
-    dataframe with the columns as returned in parse_model_filename()
-
-    Args
-        model_dir: dir containing the models
-        model_base_filename: optional, if passed, only the models with this
-            base filename will be returned
-    """
-
-    # glob search string
-    if model_base_filename is not None:
-        model_weight_paths = glob.glob(
-            f"{str(model_dir)}{os.sep}{model_base_filename}_*.hdf5"
-        )
-    else:
-        model_weight_paths = glob.glob(f"{str(model_dir)}{os.sep}*.hdf5")
-
-    # Loop through all models and extract necessary info...
-    model_info_list = []
-    for path in model_weight_paths:
-        model_info_list.append(parse_model_filename(Path(path)))
-
-    return pd.DataFrame.from_dict(model_info_list)
-
-
-def get_best_model(
-    model_dir: Path, acc_metric_mode: str, model_base_filename: Optional[str] = None
-) -> Optional[dict]:
-    """
-    Get the properties of the model with the highest combined accuracy for the highest
-    traindata version in the dir.
-
-    Args
-        model_dir: dir containing the models
-        acc_metric_mode:
-        model_base_filename: optional, if passed, only the models with this
-            base filename will be taken in account
-    """
-    # Check validaty of input
-    acc_metric_mode_values = ["min", "max"]
-    if acc_metric_mode not in acc_metric_mode_values:
-        raise Exception(
-            f"Invalid value for mode: {acc_metric_mode}, should be one of {acc_metric_mode_values}"
-        )
-
-    # Get list of existing models for this train dataset
-    model_info_df = get_models(
-        model_dir=model_dir, model_base_filename=model_base_filename
-    )
-
-    # If no model_base_filename provided, take highest data version
-    if model_base_filename is None:
-        max_data_version = get_max_data_version(model_dir)
-        if max_data_version == -1:
-            return None
-        model_info_df = model_info_df.loc[
-            model_info_df["train_data_version"] == max_data_version
-        ]
-
-    if len(model_info_df) > 0:
-        if acc_metric_mode == "max":
-            return model_info_df.loc[model_info_df["acc_combined"].values.argmax()]
-        else:
-            return model_info_df.loc[model_info_df["acc_combined"].values.argmin()]
-    else:
-        return None
-
-
-def save_and_clean_models(
-    model_save_dir: Path,
-    model_save_base_filename: str,
-    acc_metric_mode: str,
-    new_model=None,
-    new_model_acc_train: Optional[float] = None,
-    new_model_acc_val: Optional[float] = None,
-    new_model_epoch: Optional[int] = None,
-    save_weights_only: bool = False,
-    verbose: bool = True,
-    debug: bool = False,
-    only_report: bool = False,
-):
-    """
-    Save the new model if it is good enough... en cleanup existing models
-    if they are worse than the new or other existing models.
-
-    Args
-        model_save_dir: dir containing the models
-        model_save_base_filename: base filename that will be used
-        model_acc_metric_mode (str): use 'min' if the accuracy metrics should be
-                as low as possible, 'max' if a higher values is better.
-        new_model: optional, the keras model object that will be saved
-        new_model_acc_train: optional: the accuracy on the train dataset
-        new_model_acc_val: optional: the accuracy on the validation dataset
-        new_model_epoch: optional: the epoch in the training
-        verbose: report the best model after save and cleanup
-        debug: write debug logging
-        only_report: optional: only report which models would be cleaned up
-    """
-    # Check validaty of input
-    acc_metric_mode_values = ["min", "max"]
-    if acc_metric_mode not in acc_metric_mode_values:
-        raise Exception(
-            f"Invalid value for mode: {acc_metric_mode}, should be one of "
-            f"{acc_metric_mode_values}"
-        )
-
-    # Get a list of all existing models
-    model_info_df = get_models(
-        model_dir=model_save_dir, model_base_filename=model_save_base_filename
-    )
-
-    # If there is a new model passed as param, add it to the list
-    new_model_path = None
-    if (
-        new_model is not None
-        and new_model_acc_train is not None
-        and new_model_acc_val is not None
-        and new_model_epoch is not None
-    ):
-        # Calculate combined accuracy
-        new_model_acc_combined = (new_model_acc_train + new_model_acc_val) / 2
-
-        # Build save path
-        new_model_filename = format_model_filename2(
-            model_base_filename=model_save_base_filename,
-            acc_combined=new_model_acc_combined,
-            acc_train=new_model_acc_train,
-            acc_val=new_model_acc_val,
-            epoch=new_model_epoch,
-        )
-        new_model_path = model_save_dir / new_model_filename
-
-        # Append model to the retrieved models...
-        model_info_df = model_info_df.append(
-            {
-                "path": new_model_path,
-                "filename": new_model_filename,
-                "acc_combined": new_model_acc_combined,
-                "acc_train": new_model_acc_train,
-                "acc_val": new_model_acc_val,
-                "epoch": new_model_epoch,
-            },
-            ignore_index=True,
-        )
-
-    # For each model found, check if there is one with ALL parameters
-    # higher than itself. If one is found: delete model
-    # Remark: the list is sorted before iterating it, this way the logging
-    # is sorted from "worst to best"
-    if acc_metric_mode == "max":
-        model_info_sorted_df = model_info_df.sort_values(by="acc_combined")
-    else:
-        model_info_sorted_df = model_info_df.sort_values(
-            by="acc_combined", ascending=False
-        )
-    for _, model_info in model_info_sorted_df.iterrows():
-        if acc_metric_mode == "max":
-            better_ones_df = model_info_df[
-                (model_info_df["path"] != model_info["path"])
-                & (model_info_df["acc_combined"] >= model_info["acc_combined"])
-                & (model_info_df["acc_train"] >= model_info["acc_train"])
-                & (model_info_df["acc_val"] >= model_info["acc_val"])
-            ]
-        else:
-            better_ones_df = model_info_df[
-                (model_info_df["path"] != model_info["path"])
-                & (model_info_df["acc_combined"] <= model_info["acc_combined"])
-                & (model_info_df["acc_train"] <= model_info["acc_train"])
-                & (model_info_df["acc_val"] <= model_info["acc_val"])
-            ]
-
-        # If one or more better ones are found, no use in keeping it...
-        if len(better_ones_df) > 0:
-            if only_report:
-                logger.debug(f"DELETE {model_info['filename']}")
-            elif model_info["path"].exists():
-                logger.debug(f"DELETE {model_info['filename']}")
-                os.remove(model_info["path"])
-
-            if debug:
-                print(f"Better one(s) found for{model_info['filename']}:")
-                for _, better_one in better_ones_df.iterrows():
-                    print(f"  {better_one['filename']}")
-        else:
-            # No better one found, so keep it
-            logger.debug(f"KEEP {model_info['filename']}")
-
-            # If it is the new model that needs to be kept, save to disk
-            if (
-                new_model_path is not None
-                and new_model is not None
-                and only_report is not True
-                and model_info["path"] == new_model_path
-                and not new_model_path.exists()
-            ):
-                if save_weights_only:
-                    new_model.save_weights(new_model_path)
-                else:
-                    new_model.save(new_model_path)
-
-    if verbose is True or debug is True:
-        best_model = get_best_model(
-            model_save_dir, acc_metric_mode, model_save_base_filename
-        )
-        if best_model is not None:
-            print(
-                f"BEST MODEL: acc_combined: {best_model['acc_combined']}, acc_train: "
-                f"{best_model['acc_train']}, acc_val: {best_model['acc_val']}, epoch: "
-                f"{best_model['epoch']}"
-            )
-
-
-class ModelCheckpointExt(kr.callbacks.Callback):
-    def __init__(
-        self,
-        model_save_dir: Path,
-        model_save_base_filename: str,
-        acc_metric_mode: str,
-        acc_metric_train: str,
-        acc_metric_validation: str,
-        save_weights_only: bool = False,
-        verbose: bool = True,
-        only_report: bool = False,
-    ):
-        """[summary]
-
-        Args:
-            model_save_dir (Path): [description]
-            model_save_base_filename (str): [description]
-            acc_metric_mode (str): use 'min' if the accuracy metrics should be
-                    as low as possible, 'max' if a higher values is better.
-            acc_metric_train (str): [description]
-            acc_metric_validation (str): [description]
-            verbose (bool, optional): [description]. Defaults to True.
-            only_report (bool, optional): [description]. Defaults to False.
-        """
-
-        acc_metric_mode_values = ["min", "max"]
-        if acc_metric_mode not in acc_metric_mode_values:
-            raise Exception(
-                f"Invalid value for mode: {acc_metric_mode}, should be one of "
-                f"{acc_metric_mode_values}"
-            )
-
-        self.model_save_dir = model_save_dir
-        self.model_save_base_filename = model_save_base_filename
-        self.acc_metric_train = acc_metric_train
-        self.acc_metric_validation = acc_metric_validation
-        self.acc_metric_mode = acc_metric_mode
-        self.save_weights_only = save_weights_only
-        self.verbose = verbose
-        self.only_report = only_report
-
-    def on_epoch_end(self, epoch, logs={}):
-        logger.debug("Start in callback on_epoch_begin")
-
-        save_and_clean_models(
-            model_save_dir=self.model_save_dir,
-            model_save_base_filename=self.model_save_base_filename,
-            acc_metric_mode=self.acc_metric_mode,
-            new_model=self.model,
-            new_model_acc_train=logs.get(self.acc_metric_train),
-            new_model_acc_val=logs.get(self.acc_metric_validation),
-            new_model_epoch=epoch,
-            save_weights_only=self.save_weights_only,
-            verbose=self.verbose,
-            only_report=self.only_report,
-        )
-
-
-if __name__ == "__main__":
-
-    # raise Exception("Not implemented")
-
-    # General inits
-    segment_subject = "greenhouses"
-    base_dir = Path("X:/PerPersoon/PIEROG/Taken/2018/2018-08-12_AutoSegmentation")
-    traindata_version = 17
-    model_architecture = "inceptionresnetv2+linknet"
-
-    project_dir = base_dir / segment_subject
-
-    # Init logging
-    from . import log_helper
-
-    log_dir = project_dir / "log"
-    logger = log_helper.main_log_init(log_dir, __name__)
-
-    """
-    print(get_models(model_dir="",
-                     model_basename=""))
-    """
-    # Test the clean_models function (without new model)
-    # Build save dir and model base filename
-    model_save_dir = project_dir / "models"
-    model_save_base_filename = format_model_base_filename(
-        segment_subject, traindata_version, model_architecture
-    )
-
-    # Clean the models (only report)
-    save_and_clean_models(
-        model_save_dir=model_save_dir,
-        model_save_base_filename=model_save_base_filename,
-        acc_metric_mode="max",
-        only_report=True,
-    )
+# -*- coding: utf-8 -*-
+"""
+Module with helper functions regarding (keras) models.
+"""
+
+import os
+import glob
+import logging
+from pathlib import Path
+from typing import Optional
+
+import pandas as pd
+from tensorflow import keras as kr
+
+# -------------------------------------------------------------
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+# logger.setLevel(logging.INFO)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def get_max_data_version(model_dir: Path) -> int:
+    """
+    Get the maximum data version a model exists for in the model_dir.
+
+    Args
+        model_dir: the dir to search models in
+    """
+    models_df = get_models(model_dir)
+    if models_df is not None and len(models_df.index) > 0:
+        train_data_version_max = models_df["train_data_version"].max()
+        return int(train_data_version_max)
+    else:
+        return -1
+
+
+def format_model_base_filename(
+    segment_subject: str, train_data_version: int, model_architecture: str
+) -> str:
+    """
+    Format the parameters into a model_base_filename.
+
+    Args
+        segment_subject: the segment subject
+        train_data_version: the version of the data used to train the model
+        model_architecture: the architecture of the model
+    """
+    retval = f"{segment_subject}_{train_data_version:02}_{model_architecture}"
+    return retval
+
+
+def format_model_filename(
+    segment_subject: str,
+    train_data_version: int,
+    model_architecture: str,
+    acc_train: float,
+    acc_val: float,
+    acc_combined: float,
+    epoch: int,
+) -> str:
+    """
+    Format the parameters into a model_filename.
+
+    Args
+        segment_subject: the segment subject
+        train_data_version: the version of the data used to train the model
+        model_architecture: the architecture of the model
+        acc_train: the accuracy reached for the training dataset
+        acc_val: the accuracy reached for the validation dataset
+        acc_combined: the average of the train and validation accuracy
+        epoch: the epoch during training that reached these model weights
+    """
+    base_filename = format_model_base_filename(
+        segment_subject=segment_subject,
+        train_data_version=train_data_version,
+        model_architecture=model_architecture,
+    )
+    filename = format_model_filename2(
+        model_base_filename=base_filename,
+        acc_train=acc_train,
+        acc_val=acc_val,
+        acc_combined=acc_combined,
+        epoch=epoch,
+    )
+    return filename
+
+
+def format_model_filename2(
+    model_base_filename: str,
+    acc_train: float,
+    acc_val: float,
+    acc_combined: float,
+    epoch: int,
+) -> str:
+    """
+    Format the parameters into a model_filename.
+
+    Args
+        model_base_filename: the base filename of the model
+        acc_train: the accuracy reached for the training dataset
+        acc_val: the accuracy reached for the validation dataset
+        acc_combined: the average of the train and validation accuracy
+        epoch: the epoch during training that reached these model weights
+    """
+    res = (
+        f"{model_base_filename}_{acc_combined:.5f}_{acc_train:.5f}_{acc_val:.5f}_"
+        f"{epoch}.hdf5"
+    )
+    return res
+
+
+def parse_model_filename(path: Path) -> dict:
+    """
+    Parse a model_filename to a dict containing the properties of the model:
+        * segment_subject: the segment subject
+        * train_data_version: the version of the data used to train the model
+        * model_architecture: the architecture of the model
+        * acc_train: the accuracy reached for the training dataset
+        * acc_val: the accuracy reached for the validation dataset
+        * acc_combined: the average of the train and validation accuracy
+        * epoch: the epoch during training that reached these model weights
+
+    Args
+        path: the path to the model file
+    """
+    # Prepare path to extract info
+    param_values = path.stem.split("_")
+
+    # Now extract fields...
+    segment_subject = param_values[0]
+    train_data_version = int(param_values[1])
+    model_architecture = param_values[2]
+    if len(param_values) > 3:
+        acc_combined = float(param_values[3])
+        acc_train = float(param_values[4])
+        acc_val = float(param_values[5])
+        epoch = int(param_values[6])
+    else:
+        acc_combined = 0.0
+        acc_train = 0.0
+        acc_val = 0.0
+        epoch = 0
+
+    return {
+        "path": path,
+        "filename": path.name,
+        "segment_subject": segment_subject,
+        "train_data_version": train_data_version,
+        "model_architecture": model_architecture,
+        "acc_combined": acc_combined,
+        "acc_train": acc_train,
+        "acc_val": acc_val,
+        "epoch": epoch,
+    }
+
+
+def get_models(
+    model_dir: Path, model_base_filename: Optional[str] = None
+) -> pd.DataFrame:
+    """
+    Return the list of models in the model_dir passed. It is returned as a
+    dataframe with the columns as returned in parse_model_filename()
+
+    Args
+        model_dir: dir containing the models
+        model_base_filename: optional, if passed, only the models with this
+            base filename will be returned
+    """
+
+    # glob search string
+    if model_base_filename is not None:
+        model_weight_paths = glob.glob(
+            f"{str(model_dir)}{os.sep}{model_base_filename}_*.hdf5"
+        )
+    else:
+        model_weight_paths = glob.glob(f"{str(model_dir)}{os.sep}*.hdf5")
+
+    # Loop through all models and extract necessary info...
+    model_info_list = []
+    for path in model_weight_paths:
+        model_info_list.append(parse_model_filename(Path(path)))
+
+    return pd.DataFrame.from_dict(model_info_list)  # type: ignore
+
+
+def get_best_model(
+    model_dir: Path, acc_metric_mode: str, model_base_filename: Optional[str] = None
+) -> Optional[dict]:
+    """
+    Get the properties of the model with the highest combined accuracy for the highest
+    traindata version in the dir.
+
+    Args
+        model_dir: dir containing the models
+        acc_metric_mode:
+        model_base_filename: optional, if passed, only the models with this
+            base filename will be taken in account
+    """
+    # Check validaty of input
+    acc_metric_mode_values = ["min", "max"]
+    if acc_metric_mode not in acc_metric_mode_values:
+        raise Exception(
+            f"Invalid value for mode: {acc_metric_mode}, should be one of "
+            f"{acc_metric_mode_values}"
+        )
+
+    # Get list of existing models for this train dataset
+    model_info_df = get_models(
+        model_dir=model_dir, model_base_filename=model_base_filename
+    )
+
+    # If no model_base_filename provided, take highest data version
+    if model_base_filename is None:
+        max_data_version = get_max_data_version(model_dir)
+        if max_data_version == -1:
+            return None
+        model_info_df = model_info_df.loc[
+            model_info_df["train_data_version"] == max_data_version
+        ]
+
+    if len(model_info_df) > 0:
+        if acc_metric_mode == "max":
+            return model_info_df.loc[
+                model_info_df["acc_combined"].values.argmax()  # type: ignore
+            ]
+        else:
+            return model_info_df.loc[
+                model_info_df["acc_combined"].values.argmin()  # type: ignore
+            ]
+    else:
+        return None
+
+
+def save_and_clean_models(
+    model_save_dir: Path,
+    model_save_base_filename: str,
+    acc_metric_mode: str,
+    new_model=None,
+    new_model_acc_train: Optional[float] = None,
+    new_model_acc_val: Optional[float] = None,
+    new_model_epoch: Optional[int] = None,
+    save_weights_only: bool = False,
+    verbose: bool = True,
+    debug: bool = False,
+    only_report: bool = False,
+):
+    """
+    Save the new model if it is good enough... en cleanup existing models
+    if they are worse than the new or other existing models.
+
+    Args
+        model_save_dir: dir containing the models
+        model_save_base_filename: base filename that will be used
+        model_acc_metric_mode (str): use 'min' if the accuracy metrics should be
+                as low as possible, 'max' if a higher values is better.
+        new_model: optional, the keras model object that will be saved
+        new_model_acc_train: optional: the accuracy on the train dataset
+        new_model_acc_val: optional: the accuracy on the validation dataset
+        new_model_epoch: optional: the epoch in the training
+        verbose: report the best model after save and cleanup
+        debug: write debug logging
+        only_report: optional: only report which models would be cleaned up
+    """
+    # Check validaty of input
+    acc_metric_mode_values = ["min", "max"]
+    if acc_metric_mode not in acc_metric_mode_values:
+        raise Exception(
+            f"Invalid value for mode: {acc_metric_mode}, should be one of "
+            f"{acc_metric_mode_values}"
+        )
+
+    # Get a list of all existing models
+    model_info_df = get_models(
+        model_dir=model_save_dir, model_base_filename=model_save_base_filename
+    )
+
+    # If there is a new model passed as param, add it to the list
+    new_model_path = None
+    if (
+        new_model is not None
+        and new_model_acc_train is not None
+        and new_model_acc_val is not None
+        and new_model_epoch is not None
+    ):
+        # Calculate combined accuracy
+        new_model_acc_combined = (new_model_acc_train + new_model_acc_val) / 2
+
+        # Build save path
+        new_model_filename = format_model_filename2(
+            model_base_filename=model_save_base_filename,
+            acc_combined=new_model_acc_combined,
+            acc_train=new_model_acc_train,
+            acc_val=new_model_acc_val,
+            epoch=new_model_epoch,
+        )
+        new_model_path = model_save_dir / new_model_filename
+
+        # Append model to the retrieved models...
+        model_info_df = pd.concat(
+            [
+                model_info_df,
+                pd.DataFrame(
+                    [
+                        {
+                            "path": new_model_path,
+                            "filename": new_model_filename,
+                            "acc_combined": new_model_acc_combined,
+                            "acc_train": new_model_acc_train,
+                            "acc_val": new_model_acc_val,
+                            "epoch": new_model_epoch,
+                        }
+                    ]
+                ),
+            ],
+            ignore_index=True,
+        )
+
+    # For each model found, check if there is one with ALL parameters
+    # higher than itself. If one is found: delete model
+    # Remark: the list is sorted before iterating it, this way the logging
+    # is sorted from "worst to best"
+    if acc_metric_mode == "max":
+        model_info_sorted_df = model_info_df.sort_values(by="acc_combined")
+    else:
+        model_info_sorted_df = model_info_df.sort_values(
+            by="acc_combined", ascending=False
+        )
+    for _, model_info in model_info_sorted_df.iterrows():
+        if acc_metric_mode == "max":
+            better_ones_df = model_info_df[
+                (model_info_df["path"] != model_info["path"])
+                & (model_info_df["acc_combined"] >= model_info["acc_combined"])
+                & (model_info_df["acc_train"] >= model_info["acc_train"])
+                & (model_info_df["acc_val"] >= model_info["acc_val"])
+            ]
+        else:
+            better_ones_df = model_info_df[
+                (model_info_df["path"] != model_info["path"])
+                & (model_info_df["acc_combined"] <= model_info["acc_combined"])
+                & (model_info_df["acc_train"] <= model_info["acc_train"])
+                & (model_info_df["acc_val"] <= model_info["acc_val"])
+            ]
+
+        # If one or more better ones are found, no use in keeping it...
+        if len(better_ones_df) > 0:
+            if only_report:
+                logger.debug(f"DELETE {model_info['filename']}")
+            elif model_info["path"].exists():
+                logger.debug(f"DELETE {model_info['filename']}")
+                os.remove(model_info["path"])
+
+            if debug:
+                print(f"Better one(s) found for{model_info['filename']}:")
+                for _, better_one in better_ones_df.iterrows():
+                    print(f"  {better_one['filename']}")
+        else:
+            # No better one found, so keep it
+            logger.debug(f"KEEP {model_info['filename']}")
+
+            # If it is the new model that needs to be kept, save to disk
+            if (
+                new_model_path is not None
+                and new_model is not None
+                and only_report is not True
+                and model_info["path"] == new_model_path
+                and not new_model_path.exists()
+            ):
+                if save_weights_only:
+                    new_model.save_weights(new_model_path)
+                else:
+                    new_model.save(new_model_path)
+
+    if verbose is True or debug is True:
+        best_model = get_best_model(
+            model_save_dir, acc_metric_mode, model_save_base_filename
+        )
+        if best_model is not None:
+            print(
+                f"BEST MODEL: acc_combined: {best_model['acc_combined']}, acc_train: "
+                f"{best_model['acc_train']}, acc_val: {best_model['acc_val']}, epoch: "
+                f"{best_model['epoch']}"
+            )
+
+
+class ModelCheckpointExt(kr.callbacks.Callback):
+    def __init__(
+        self,
+        model_save_dir: Path,
+        model_save_base_filename: str,
+        acc_metric_mode: str,
+        acc_metric_train: str,
+        acc_metric_validation: str,
+        save_weights_only: bool = False,
+        verbose: bool = True,
+        only_report: bool = False,
+    ):
+        """[summary]
+
+        Args:
+            model_save_dir (Path): [description]
+            model_save_base_filename (str): [description]
+            acc_metric_mode (str): use 'min' if the accuracy metrics should be
+                    as low as possible, 'max' if a higher values is better.
+            acc_metric_train (str): [description]
+            acc_metric_validation (str): [description]
+            verbose (bool, optional): [description]. Defaults to True.
+            only_report (bool, optional): [description]. Defaults to False.
+        """
+
+        acc_metric_mode_values = ["min", "max"]
+        if acc_metric_mode not in acc_metric_mode_values:
+            raise Exception(
+                f"Invalid value for mode: {acc_metric_mode}, should be one of "
+                f"{acc_metric_mode_values}"
+            )
+
+        self.model_save_dir = model_save_dir
+        self.model_save_base_filename = model_save_base_filename
+        self.acc_metric_train = acc_metric_train
+        self.acc_metric_validation = acc_metric_validation
+        self.acc_metric_mode = acc_metric_mode
+        self.save_weights_only = save_weights_only
+        self.verbose = verbose
+        self.only_report = only_report
+
+    def on_epoch_end(self, epoch, logs={}):
+        logger.debug("Start in callback on_epoch_begin")
+
+        save_and_clean_models(
+            model_save_dir=self.model_save_dir,
+            model_save_base_filename=self.model_save_base_filename,
+            acc_metric_mode=self.acc_metric_mode,
+            new_model=self.model,
+            new_model_acc_train=logs.get(self.acc_metric_train),
+            new_model_acc_val=logs.get(self.acc_metric_validation),
+            new_model_epoch=epoch,
+            save_weights_only=self.save_weights_only,
+            verbose=self.verbose,
+            only_report=self.only_report,
+        )
+
+
+if __name__ == "__main__":
+    # raise Exception("Not implemented")
+
+    # General inits
+    segment_subject = "greenhouses"
+    base_dir = Path("X:/PerPersoon/PIEROG/Taken/2018/2018-08-12_AutoSegmentation")
+    traindata_version = 17
+    model_architecture = "inceptionresnetv2+linknet"
+
+    project_dir = base_dir / segment_subject
+
+    # Init logging
+    from . import log_helper
+
+    log_dir = project_dir / "log"
+    logger = log_helper.main_log_init(log_dir, __name__)
+
+    """
+    print(get_models(model_dir="",
+                     model_basename=""))
+    """
+    # Test the clean_models function (without new model)
+    # Build save dir and model base filename
+    model_save_dir = project_dir / "models"
+    model_save_base_filename = format_model_base_filename(
+        segment_subject, traindata_version, model_architecture
+    )
+
+    # Clean the models (only report)
+    save_and_clean_models(
+        model_save_dir=model_save_dir,
+        model_save_base_filename=model_save_base_filename,
+        acc_metric_mode="max",
+        only_report=True,
+    )
```

### Comparing `cropclassification-0.1.0a2/cropclassification/helpers/pandas_helper.py` & `cropclassification-0.1.1/cropclassification/helpers/pandas_helper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,126 +1,131 @@
-# -*- coding: utf-8 -*-
-"""
-Module with helper functions to expand on some features of pandas.
-"""
-
-from pathlib import Path
-import os
-from typing import List, Optional
-
-import pandas as pd
-import sqlite3
-
-
-def read_file(
-    path: Path, table_name: str = "info", columns: Optional[List[str]] = None
-) -> pd.DataFrame:
-    """
-    Reads a file to a pandas dataframe. The fileformat is detected based on the
-    path extension.
-
-    # TODO: think about if possible/how to support  adding optional parameter and pass
-    # them to next function, example encoding, float_format,...
-    """
-    if columns is not None and type(columns) is not list:
-        raise Exception(f"Parameter columns should be list, but is {type(columns)}")
-
-    ext_lower = path.suffix.lower()
-    if ext_lower == ".csv":
-        try:
-            data_read_df = pd.read_csv(str(path), usecols=columns, low_memory=False)
-        except UnicodeDecodeError:
-            # If a unicode decode error is thrown, try again using ANSI encoding
-            data_read_df = pd.read_csv(
-                str(path), usecols=columns, low_memory=False, encoding="ANSI"
-            )
-        return data_read_df
-    elif ext_lower == ".tsv":
-        try:
-            data_read_df = pd.read_csv(
-                str(path), usecols=columns, sep="\t", low_memory=False
-            )
-        except UnicodeDecodeError:
-            # If a unicode decode error is thrown, try again using ANSI encoding
-            data_read_df = pd.read_csv(
-                str(path),
-                usecols=columns,
-                sep="\t",
-                low_memory=False,
-                encoding="ANSI",
-            )
-        return data_read_df
-    elif ext_lower == ".parquet":
-        return pd.read_parquet(str(path), columns=columns)
-    elif ext_lower in (".sqlite", ".gpkg"):
-        sql_db = None
-        try:
-            sql_db = sqlite3.connect(str(path))
-            if columns is None:
-                cols_to_select = "*"
-            else:
-                cols_to_select = ", ".join(columns)
-            data_read_df = pd.read_sql_query(
-                f'select {cols_to_select} from "{table_name}"', sql_db
-            )
-        except Exception as ex:
-            raise Exception(f"Error reading data from {str(path)}") from ex
-        finally:
-            if sql_db is not None:
-                sql_db.close()
-        return data_read_df
-    else:
-        raise Exception(f"Not implemented for extension {ext_lower}")
-
-
-def to_file(
-    df: pd.DataFrame,
-    path: Path,
-    table_name: str = "info",
-    index: bool = True,
-    append: bool = False,
-):
-    """
-    Reads a pandas dataframe to file. The file format is detected based on the path
-    extension.
-
-    # TODO: think about if possible/how to support  adding optional parameter and pass
-    # them to next function, example encoding, float_format,...
-    """
-    ext_lower = path.suffix.lower()
-    if ext_lower == ".csv":
-        if append:
-            raise Exception("Append is not supported for csv files")
-        df.to_csv(str(path), float_format="%.10f", encoding="utf-8", index=index)
-    elif ext_lower == ".tsv":
-        if append:
-            raise Exception("Append is not supported for tsv files")
-        df.to_csv(
-            str(path), sep="\t", float_format="%.10f", encoding="utf-8", index=index
-        )
-    elif ext_lower == ".parquet":
-        if append:
-            raise Exception("Append is not supported for parquet files")
-        df.to_parquet(str(path), index=index)
-    elif ext_lower == ".sqlite":
-        if_exists = "fail"
-        if append:
-            if_exists = "append"
-        elif os.path.exists(path):
-            os.remove(path)
-        sql_db = None
-        try:
-            sql_db = sqlite3.connect(str(path))
-            df.to_sql(
-                name=table_name,
-                con=sql_db,
-                if_exists=if_exists,
-                index=index,
-                chunksize=50000,
-            )
-        except Exception as ex:
-            raise Exception(f"Error in to_file to file {str(path)}") from ex
-        finally:
-            if sql_db is not None:
-                sql_db.close()
-    else:
-        raise Exception(f"Not implemented for extension {ext_lower}")
+# -*- coding: utf-8 -*-
+"""
+Module with helper functions to expand on some features of pandas.
+"""
+
+from pathlib import Path
+import os
+from typing import List, Optional, Union
+
+import pandas as pd
+import sqlite3
+
+
+def read_file(
+    path: Path, table_name: str = "info", columns: Optional[List[str]] = None
+) -> pd.DataFrame:
+    """
+    Reads a file to a pandas dataframe. The fileformat is detected based on the
+    path extension.
+
+    # TODO: think about if possible/how to support  adding optional parameter and pass
+    # them to next function, example encoding, float_format,...
+    """
+    if columns is not None and type(columns) is not list:
+        raise Exception(f"Parameter columns should be list, but is {type(columns)}")
+
+    ext_lower = path.suffix.lower()
+    if ext_lower == ".csv":
+        try:
+            data_read_df = pd.read_csv(
+                str(path), usecols=columns, low_memory=False  # type: ignore
+            )
+        except UnicodeDecodeError:
+            # If a unicode decode error is thrown, try again using ANSI encoding
+            data_read_df = pd.read_csv(
+                str(path),
+                usecols=columns,  # type: ignore
+                low_memory=False,
+                encoding="ANSI",
+            )
+        return data_read_df
+    elif ext_lower == ".tsv":
+        try:
+            data_read_df = pd.read_csv(
+                str(path), usecols=columns, sep="\t", low_memory=False  # type: ignore
+            )
+        except UnicodeDecodeError:
+            # If a unicode decode error is thrown, try again using ANSI encoding
+            data_read_df = pd.read_csv(
+                str(path),
+                usecols=columns,  # type: ignore
+                sep="\t",
+                low_memory=False,
+                encoding="ANSI",
+            )
+        return data_read_df
+    elif ext_lower == ".parquet":
+        return pd.read_parquet(str(path), columns=columns)
+    elif ext_lower in (".sqlite", ".gpkg"):
+        sql_db = None
+        try:
+            sql_db = sqlite3.connect(str(path))
+            if columns is None:
+                cols_to_select = "*"
+            else:
+                cols_to_select = ", ".join(columns)
+            data_read_df = pd.read_sql_query(
+                f'select {cols_to_select} from "{table_name}"', sql_db
+            )
+        except Exception as ex:
+            raise Exception(f"Error reading data from {str(path)}") from ex
+        finally:
+            if sql_db is not None:
+                sql_db.close()
+        return data_read_df
+    else:
+        raise Exception(f"Not implemented for extension {ext_lower}")
+
+
+def to_file(
+    df: Union[pd.DataFrame, pd.Series],
+    path: Path,
+    table_name: str = "info",
+    index: bool = True,
+    append: bool = False,
+):
+    """
+    Reads a pandas dataframe to file. The file format is detected based on the path
+    extension.
+
+    # TODO: think about if possible/how to support  adding optional parameter and pass
+    # them to next function, example encoding, float_format,...
+    """
+    ext_lower = path.suffix.lower()
+    if ext_lower == ".csv":
+        if append:
+            raise Exception("Append is not supported for csv files")
+        df.to_csv(str(path), float_format="%.10f", encoding="utf-8", index=index)
+    elif ext_lower == ".tsv":
+        if append:
+            raise Exception("Append is not supported for tsv files")
+        df.to_csv(
+            str(path), sep="\t", float_format="%.10f", encoding="utf-8", index=index
+        )
+    elif ext_lower == ".parquet":
+        if append:
+            raise Exception("Append is not supported for parquet files")
+        df.to_parquet(str(path), index=index)
+    elif ext_lower == ".sqlite":
+        if_exists = "fail"
+        if append:
+            if_exists = "append"
+        elif os.path.exists(path):
+            os.remove(path)
+        sql_db = None
+        try:
+            sql_db = sqlite3.connect(str(path))
+            df.to_sql(
+                name=table_name,
+                con=sql_db,
+                if_exists=if_exists,
+                index=index,
+                chunksize=50000,
+            )
+        except Exception as ex:
+            raise Exception(f"Error in to_file to file {str(path)}") from ex
+        finally:
+            if sql_db is not None:
+                sql_db.close()
+    else:
+        raise Exception(f"Not implemented for extension {ext_lower}")
```

### Comparing `cropclassification-0.1.0a2/cropclassification/postprocess/classification_postprocess.py` & `cropclassification-0.1.1/cropclassification/postprocess/classification_postprocess.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,547 +1,558 @@
-# -*- coding: utf-8 -*-
-"""
-Module with postprocessing functions on classification results.
-"""
-
-import datetime
-import logging
-from pathlib import Path
-from typing import Optional
-
-import numpy as np
-import pandas as pd
-import geofileops as gfo
-import geopandas as gpd
-
-import cropclassification.helpers.config_helper as conf
-import cropclassification.helpers.pandas_helper as pdh
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-# logger.setLevel(logging.DEBUG)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def calc_top3_and_consolidation(
-    input_parcel_path: Path,
-    input_parcel_probabilities_path: Path,
-    input_parcel_geopath: Path,
-    output_predictions_path: Path,
-    output_predictions_geopath: Path,
-    output_predictions_output_path: Optional[Path] = None,
-    force: bool = False,
-):
-    """
-    Calculate the top3 prediction and a consolidation prediction.
-
-    Remark: in this logic the declared crop/class (class_declared) is used, as we want
-    to compare with the declaration of the farmer, rather than taking into account
-    corrections already.
-
-    Args:
-        input_parcel_path (Path): [description]
-        input_parcel_probabilities_path (Path): [description]
-        output_predictions_path (Path): [description]
-        output_predictions_geopath (Path): [description]
-        output_predictions_output_path (Path, optional): [description].
-            Defaults to None.
-        force (bool, optional): [description]. Defaults to False.
-    """
-
-    # If force is false and output exists, already, return
-    if force is False and output_predictions_path.exists():
-        logger.warning(
-            "calc_top3_and_consolidation: output file exist and force is False, so "
-            f"stop: {output_predictions_path}"
-        )
-        return
-
-    # Read input files
-    logger.info("Read input file")
-    proba_df = pdh.read_file(input_parcel_probabilities_path)
-
-    top3_df = calc_top3(proba_df)
-
-    # Read input files
-    logger.info("Read input file")
-    input_parcel_df = pdh.read_file(input_parcel_path)
-
-    # All input parcels must stay in the output, so left join input with pred
-    top3_df.set_index(conf.columns["id"], inplace=True)
-    if input_parcel_df.index.name != conf.columns["id"]:
-        input_parcel_df.set_index(conf.columns["id"], inplace=True)
-    cols_to_join = top3_df.columns.difference(input_parcel_df.columns)
-    pred_df = input_parcel_df.join(top3_df[cols_to_join], how="left")
-
-    # The parcels added by the join don't have a prediction yet, so apply it
-    # For the ignore classes, set the prediction to the ignore type
-    classes_to_ignore = conf.marker.getlist("classes_to_ignore")
-    pred_df.loc[
-        pred_df[conf.columns["class_declared"]].isin(classes_to_ignore), "pred1"
-    ] = pred_df[conf.columns["class_declared"]]
-    # For all other parcels without prediction there must have been no data
-    # available for a classification, so set prediction to NODATA
-    pred_df["pred1"].fillna("NODATA", inplace=True)
-
-    # Add doubt columns
-    add_doubt_column(
-        pred_df=pred_df,
-        new_pred_column=conf.columns["prediction_cons"],
-        apply_doubt_pct_proba=True,
-        apply_doubt_min_nb_pixels=True,
-        apply_doubt_marker_specific=False,
-    )
-    add_doubt_column(
-        pred_df=pred_df,
-        new_pred_column=conf.columns["prediction_full_alpha"],
-        apply_doubt_pct_proba=True,
-        apply_doubt_min_nb_pixels=True,
-        apply_doubt_marker_specific=True,
-    )
-
-    # Calculate the status of the consolidated prediction (OK=usable, NOK=not)
-    pred_df.loc[
-        pred_df[conf.columns["prediction_full_alpha"]].isin(proba_df.columns),
-        conf.columns["prediction_cons_status"],
-    ] = "OK"
-    pred_df[conf.columns["prediction_cons_status"]].fillna("NOK", inplace=True)
-
-    logger.info("Write full prediction data to file")
-    pdh.to_file(pred_df, output_predictions_path)
-
-    # Output to geo file
-    input_parcel_gdf = gfo.read_file(input_parcel_geopath)
-    pred_gdf = gpd.GeoDataFrame(input_parcel_gdf.merge(pred_df, how="inner"))
-    gfo.to_file(pred_gdf, output_predictions_geopath)
-
-    # Create final output file with the most important info
-    if output_predictions_output_path is not None:
-
-        # First add some aditional columns specific for the export
-        pred_df["markercode"] = conf.marker["markertype"]
-        pred_df["run_id"] = conf.general["run_id"]
-        today = datetime.date.today()
-        pred_df["cons_date"] = today
-        pred_df["modify_date"] = today
-        logger.info("Write final output prediction data to file")
-        pred_df.reset_index(inplace=True)
-        pred_df = pred_df[conf.columns.getlist("output_columns")]
-        pdh.to_file(pred_df, output_predictions_output_path, index=False)
-
-        # Write oracle sqlldr file
-        table_name = None
-        table_columns = None
-        if conf.marker["markertype"] in ["LANDCOVER", "LANDCOVER-EARLY"]:
-            table_name = "mon_marker_landcover"
-            table_columns = (
-                "layer_id, prc_id, versienummer, markercode, run_id, cons_landcover, "
-                + "cons_status, cons_date date 'yyyy-mm-dd', landcover1, probability1, "
-                + "landcover2, probability2, landcover3, probability3, "
-                + "modify_date date 'yyyy-mm-dd'"
-            )
-        elif conf.marker["markertype"] in ["CROPGROUP", "CROPGROUP-EARLY"]:
-            table_name = "mon_marker_cropgroup"
-            table_columns = (
-                "layer_id, prc_id, versienummer, markercode, run_id, cons_cropgroup, "
-                + "cons_status, cons_date date 'yyyy-mm-dd', cropgroup1, probability1, "
-                + "cropgroup2, probability2, cropgroup3, probability3, "
-                + "modify_date date 'yyyy-mm-dd'"
-            )
-        else:
-            table_name = None
-            logger.warning(
-                f"Table unknown for marker type {conf.marker['markertype']}, so cannot write .ctl file"
-            )
-
-        if table_name is not None and table_columns is not None:
-            with open(str(output_predictions_output_path) + ".ctl", "w") as ctlfile:
-                # SKIP=1 to skip the columns names line, the other ones to evade
-                # more commits than needed
-                ctlfile.write(
-                    "OPTIONS (SKIP=1, ROWS=10000, BINDSIZE=40000000, READSIZE=40000000)\n"
-                )
-                ctlfile.write("LOAD DATA\n")
-                ctlfile.write(
-                    f"INFILE '{output_predictions_output_path.name}'  \"str '\\n'\"\n"
-                )
-                ctlfile.write(f"INSERT INTO TABLE {table_name} APPEND\n")
-                # A tab as seperator is apparently X'9'
-                ctlfile.write("FIELDS TERMINATED BY X'9'\n")
-                ctlfile.write(f"({table_columns})\n")
-
-
-def calc_top3(proba_df: pd.DataFrame) -> pd.DataFrame:
-
-    # Calculate the top 3 predictions
-    logger.info("Calculate top3")
-    proba_tmp_df = proba_df.copy()
-    for column in proba_tmp_df.columns:
-        if column in conf.preprocess.getlist("dedicated_data_columns"):
-            proba_tmp_df.drop(column, axis=1, inplace=True)
-
-    # Get the top 3 predictions for each row
-    # First get the indeces of the top 3 predictions for each row
-    # Remark: argsort sorts ascending, so we need to take:
-    #     - "[:,": for all rows
-    #     - ":-4": the last 3 elements of the values
-    #     - ":-1]": and than reverse the order with a negative step
-    top3_pred_classes_idx = np.argsort(proba_tmp_df.values, axis=1)[:, :-4:-1]
-    # Convert the indeces to classes
-    top3_pred_classes = np.take(proba_tmp_df.columns, top3_pred_classes_idx)
-    # Get the values of the top 3 predictions
-    top3_pred_values = np.sort(proba_tmp_df.values, axis=1)[:, :-4:-1]
-    # Concatenate both
-    top3_pred = np.concatenate([top3_pred_classes, top3_pred_values], axis=1)
-    # Concatenate the ids, the classes and the top3 predictions
-    id_class_top3 = np.concatenate(
-        [
-            proba_df[[conf.columns["id"], conf.columns["class_declared"]]].values,
-            top3_pred,
-        ],
-        axis=1,
-    )
-
-    # Convert to dataframe
-    top3_df = pd.DataFrame(
-        id_class_top3,
-        columns=[
-            conf.columns["id"],
-            conf.columns["class_declared"],
-            "pred1",
-            "pred2",
-            "pred3",
-            "pred1_prob",
-            "pred2_prob",
-            "pred3_prob",
-        ],
-    )
-
-    return top3_df
-
-
-def add_doubt_column(
-    pred_df: pd.DataFrame,
-    new_pred_column: str,
-    apply_doubt_pct_proba: bool,
-    apply_doubt_min_nb_pixels: bool,
-    apply_doubt_marker_specific: bool,
-):
-
-    # Calculate predictions with doubt column
-    classes_to_ignore = conf.marker.getlist("classes_to_ignore")
-
-    # Init with the standard prediction
-    pred_df[new_pred_column] = "UNDEFINED"
-
-    # If NODATA OR ignore class, retained those from pred1
-    pred_df.loc[
-        (pred_df[new_pred_column] == "UNDEFINED")
-        & (
-            (pred_df["pred1"] == "NODATA")
-            | (pred_df[conf.columns["class_declared"]].isin(classes_to_ignore))
-        ),
-        new_pred_column,
-    ] = pred_df["pred1"]
-
-    # Doubt based on percentage probability
-    if apply_doubt_pct_proba:
-        # Apply doubt for parcels with a low percentage of probability -> = doubt!
-        doubt_proba1_st_2_x_proba2 = conf.postprocess.getboolean(
-            "doubt_proba1_st_2_x_proba2"
-        )
-        if doubt_proba1_st_2_x_proba2 is True:
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (
-                    pred_df["pred1_prob"].map(float)
-                    < 2.0 * pred_df["pred2_prob"].map(float)
-                ),
-                new_pred_column,
-            ] = "DOUBT:PROBA1<2*PROBA2"
-
-        # Apply doubt for parcels with prediction != unverified input
-        doubt_pred_ne_input_proba1_st_pct = conf.postprocess.getfloat(
-            "doubt_pred_ne_input_proba1_st_pct"
-        )
-        if doubt_pred_ne_input_proba1_st_pct > 0:
-            if doubt_pred_ne_input_proba1_st_pct > 100:
-                raise Exception(
-                    f"doubt_pred_ne_input_proba1_st_pct should be float from 0 till 100, not {doubt_pred_ne_input_proba1_st_pct}"
-                )
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (pred_df["pred1"] != pred_df[conf.columns["class_declared"]])
-                & (
-                    pred_df["pred1_prob"].map(float)
-                    < (doubt_pred_ne_input_proba1_st_pct / 100)
-                ),
-                new_pred_column,
-            ] = "DOUBT:PRED<>INPUT-PROBA1<X"
-
-        # Apply doubt for parcels with prediction == unverified input
-        doubt_pred_eq_input_proba1_st_pct = conf.postprocess.getfloat(
-            "doubt_pred_eq_input_proba1_st_pct"
-        )
-        if doubt_pred_eq_input_proba1_st_pct > 0:
-            if doubt_pred_eq_input_proba1_st_pct > 100:
-                raise Exception(
-                    f"doubt_pred_ne_input_proba1_st_pct should be float from 0 till 100, not {doubt_pred_eq_input_proba1_st_pct}"
-                )
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (pred_df["pred1"] == pred_df[conf.columns["class_declared"]])
-                & (
-                    pred_df["pred1_prob"].map(float)
-                    < (doubt_pred_eq_input_proba1_st_pct / 100)
-                ),
-                new_pred_column,
-            ] = "DOUBT:PRED=INPUT-PROBA1<X"
-
-    # Marker specific doubt
-    if apply_doubt_marker_specific is True:
-        # Apply some extra, marker-specific doubt algorythms
-        if conf.marker["markertype"] in ("LANDCOVER", "LANDCOVER-EARLY"):
-            logger.info("Apply some marker-specific doubt algorythms")
-
-            # Remarks:
-            #   - To be sure apply RISKY_DOUBT first, so if there would be
-            #     overlapping criteria, RISKY_DOUBT "wins".
-            #   - Don't overwrite existing DOUBT on parcels, because the
-            #     general doubt reasons should win compared to the marker
-            #     specific doubt/risky_doubt reasons.
-            #   - RISKY DOUBT is used when ground truth resulted in partly alpha
-            #     errors, partly correct, classifications.
-
-            # If parcel was declared as grassland, and is classified as arable, set to
-            # risky doubt.
-            # Remark: those gave 50% false positives for LANDCOVER marker
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (pred_df[conf.columns["class_declared"]] == "MON_LC_GRASSES")
-                & (pred_df["pred1"] == "MON_LC_ARABLE"),
-                new_pred_column,
-            ] = "RISKY_DOUBT:GRASS-SEEN-AS-ARABLE"
-
-            # If parcel was declared as fallow, and is classified as something else,
-            # set to doubt.
-            # Remark: those gave 50% false positives for marker LANDCOVER
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (pred_df[conf.columns["class_declared"]] == "MON_LC_FALLOW")
-                & (pred_df["pred1"] != "MON_LC_FALLOW"),
-                new_pred_column,
-            ] = "RISKY_DOUBT:FALLOW-UNCONFIRMED"
-
-            # If parcel was declared as "9603: Boomkweek-sierplanten", but is not
-            # classified as such: doubt
-            # Remark: they gave 50% false positives for marker LANDCOVER
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (pred_df[conf.columns["crop_declared"]].isin(["9603"]))
-                & (pred_df["pred1"] == "MON_LC_GRASSES"),
-                new_pred_column,
-            ] = "RISKY_DOUBT:BOOMSIER-SEEN-AS-GRASSES"
-
-            # If parcel was declared as grain, but is not classified as MON_LC_ARABLE:
-            # doubt
-            # Remark: - those gave > 50% false positives for marker LANDCOVER-EARLY
-            #         - gave > 33 % false positives for marker LANDCOVER
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (
-                    pred_df[conf.columns["crop_declared"]].isin(
-                        ["39", "311", "321", "322", "331", "342", "639", "646"]
-                    )
-                )
-                & (pred_df["pred1"] != "MON_LC_ARABLE"),
-                new_pred_column,
-            ] = "RISKY_DOUBT:GRAIN-UNCONFIRMED"
-
-            # If parcel was declared as one of the following fabaceae, but is not
-            # classified as such: doubt
-            # Remark: - those gave > 50% false positives for marker LANDCOVER-EARLY
-            #         - gave 33-100% false positives for marker LANDCOVER
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (
-                    pred_df[conf.columns["crop_declared"]].isin(
-                        [
-                            "43",
-                            "51",
-                            "52",
-                            "721",
-                            "722",
-                            "731",
-                            "732",
-                            "831",
-                            "931",
-                            "8410",
-                        ]
-                    )
-                )
-                & (pred_df["pred1"] != "MON_LC_FABACEAE"),
-                new_pred_column,
-            ] = "RISKY_DOUBT:FABACEAE-UNCONFIRMED"
-
-            # Declared class was not correct, but groundtruth class is permanent
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (pred_df[conf.columns["class_declared"]] != pred_df["pred1"])
-                & (pred_df["pred1"].isin(["MON_LC_BOS", "MON_LC_HEIDE"])),
-                new_pred_column,
-            ] = "RISKY_DOUBT:DECL<>PRED-PRED=" + pred_df["pred1"].map(str)
-
-            # If parcel was declared as some arable crops (9534 = knolvenkel), and is
-            # classified as fabaceae, set to doubt
-            # Remark: those gave 100% false positives for marker LANDCOVER
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (pred_df[conf.columns["crop_declared"]].isin(["9534"]))
-                & (pred_df["pred1"] == "MON_LC_FABACEAE"),
-                new_pred_column,
-            ] = "DOUBT:ARABLE-SEEN-AS-FABACEAE"
-
-            # If parcel was declared as 'other herbs' or 'flowers', but is not
-            # confirmed as MON_LC_ARABLE classified as such: doubt
-            # Remark: - those gave > 50% false positives for marker LANDCOVER-EARLY
-            #         - gave 33-50% false positives for marker LANDCOVER
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (pred_df[conf.columns["crop_declared"]].isin(["956", "957", "9831"]))
-                & (pred_df["pred1"] != "MON_LC_ARABLE"),
-                new_pred_column,
-            ] = "RISKY_DOUBT:HERBS-UNCONFIRMED"
-
-            # If parcel was declared as 'aardbeien', but is not confirmed as 
-            # MON_LC_ARABLE classified as such: doubt
-            # Remark: - those gave > 50% false positives for marker LANDCOVER-EARLY
-            #         - gave 33-50% false positives for marker LANDCOVER
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (pred_df[conf.columns["crop_declared"]].isin(["9516"]))
-                & (pred_df["pred1"] != "MON_LC_ARABLE"),
-                new_pred_column,
-            ] = "RISKY_DOUBT:AARDBEIEN-UNCONFIRMED"
-
-            # Declared class was not correct, but groundtruth class is permanent
-            # TODO: probably dirty this is hardcoded here!
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (pred_df[conf.columns["class_declared"]] != pred_df["pred1"])
-                & (
-                    pred_df["pred1"].isin(
-                        ["MON_LC_BOS", "MON_LC_HEIDE", "MON_LC_OVERK_LOO"]
-                    )
-                ),
-                new_pred_column,
-            ] = "RISKY_DOUBT:DECL<>PRED-PRED=" + pred_df["pred1"].map(str)
-
-            # If parcel was declared as 9410 and classified as ARABLE, set to doubt
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (pred_df[conf.columns["crop_declared"]].isin(["9410"]))
-                & (pred_df["pred1"] == "MON_LC_ARABLE"),
-                new_pred_column,
-            ] = "RISKY_DOUBT:STAMSLABONEN-SEEN-AS-ARABLE"
-
-            # If parcel was declared as 9602 and classified as FRUIT, set to doubt
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (pred_df[conf.columns["crop_declared"]].isin(["9602"]))
-                & (pred_df["pred1"] == "MON_LC_FRUIT"),
-                new_pred_column,
-            ] = "RISKY_DOUBT:BOOM/FRUITKWEEK-UNCONFIRMED"
-
-            # Parcel was declared as one of the following + classified as GRASSES
-            # 
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (
-                    pred_df[conf.columns["crop_declared"]].isin(
-                        [
-                            "36",
-                            "895",
-                            "9582",
-#                            "744",
-#                            "9202",
-#                            "9714",
-#                            "832",
-#                            "9602",
-#                            "9730",
-                        ]
-                    )
-                )
-                & (pred_df["pred1"] == "MON_LC_GRASSES"),
-                new_pred_column,
-            ] = "RISKY_DOUBT:SEEN-AS-GRASSES"
-
-            # Parcel was declared as one of the following and classified as ARABLE
-            # Ground truth in some cases confirmed the classification, in others
-            # resulted in alpha errors -> RISKY_DOUBT
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (
-                    pred_df[conf.columns["crop_declared"]].isin(
-                        ["601", "644", "932", "9412", "9584", "8411"]
-                    )
-                )
-                & (pred_df["pred1"] == "MON_LC_ARABLE"),
-                new_pred_column,
-            ] = "RISKY_DOUBT:SEEN-AS-ARABLE"
-
-            # If parcel was declared as one of the following and classified as FABACEAE, set to RISKY_DOUBT
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (pred_df[conf.columns["crop_declared"]].isin(["9546"]))
-                & (pred_df["pred1"] == "MON_LC_FABACEAE"),
-                new_pred_column,
-            ] = "RISKY_DOUBT:SAVOOIKOOL-SEEN-AS-FABACEAE"
-
-        elif conf.marker["markertype"] in ("CROPGROUP", "CROPGROUP-EARLY"):
-            logger.info("Apply some marker-specific doubt algorythms")
-
-            # Red parcels declared as MON_TRITICALE always seem to be predicted wrong, so place them in doubt
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (pred_df[conf.columns["class_declared"]] != pred_df["pred1"])
-                & (pred_df[conf.columns["class_declared"]] == "MON_TRITICALE"),
-                new_pred_column,
-            ] = "RISKY_DOUBT:TRITICALE-UNCONFIRMED"
-
-            # Red parcels with MON_HEIDE seem to have a difficult time seeing the difference between MON_HEIDE and MON_GRASSEN
-            pred_df.loc[
-                (pred_df[new_pred_column] == "UNDEFINED")
-                & (pred_df[conf.columns["class_declared"]] != pred_df["pred1"])
-                & (pred_df["pred1"] == "MON_HEIDE"),
-                new_pred_column,
-            ] = "RISKY_DOUBT:HEIDE-UNCONFIRMED"
-
-            """
-            # Note: this will INCREASE the alpha errors, because we remove a large portion of red parcels to doubt (~886 parcels => 16 alpha errors)
-            pred_df.loc[((pred_df[new_pred_column] == 'UNDEFINED') | (~pred_df[new_pred_column].str.startswith('DOUBT')))
-                            & (pred_df[conf.columns['class_declared']] != pred_df['pred1'])
-                            & (pred_df[conf.columns['class_declared']] == 'MON_GRASSEN'),
-                        new_pred_column] = 'RISKY_DOUBT:GRASSEN-UNCONFIRMED'
-            """
-
-    # Accuracy with few pixels might be lower, so set those to doubt
-    if apply_doubt_min_nb_pixels is True:
-        pred_df.loc[
-            (
-                pred_df[conf.columns["pixcount_s1s2"]]
-                < conf.marker.getfloat("min_nb_pixels")
-            )
-            & (~pred_df[new_pred_column].str.startswith("DOUBT")),
-            new_pred_column,
-        ] = "DOUBT:NOT_ENOUGH_PIXELS"
-
-    # Finally, predictions that have no value yet, get the original prediction
-    pred_df.loc[pred_df[new_pred_column] == "UNDEFINED", new_pred_column] = pred_df[
-        "pred1"
-    ]
+# -*- coding: utf-8 -*-
+"""
+Module with postprocessing functions on classification results.
+"""
+
+import datetime
+import logging
+from pathlib import Path
+from typing import Optional
+
+import numpy as np
+import pandas as pd
+import geofileops as gfo
+import geopandas as gpd
+
+import cropclassification.helpers.config_helper as conf
+import cropclassification.helpers.pandas_helper as pdh
+
+# -------------------------------------------------------------
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+# logger.setLevel(logging.DEBUG)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def calc_top3_and_consolidation(
+    input_parcel_path: Path,
+    input_parcel_probabilities_path: Path,
+    input_parcel_geopath: Path,
+    output_predictions_path: Path,
+    output_predictions_geopath: Path,
+    output_predictions_output_path: Optional[Path] = None,
+    force: bool = False,
+):
+    """
+    Calculate the top3 prediction and a consolidation prediction.
+
+    Remark: in this logic the declared crop/class (class_declared) is used, as we want
+    to compare with the declaration of the farmer, rather than taking into account
+    corrections already.
+
+    Args:
+        input_parcel_path (Path): [description]
+        input_parcel_probabilities_path (Path): [description]
+        output_predictions_path (Path): [description]
+        output_predictions_geopath (Path): [description]
+        output_predictions_output_path (Path, optional): [description].
+            Defaults to None.
+        force (bool, optional): [description]. Defaults to False.
+    """
+
+    # If force is false and output exists, already, return
+    if force is False and output_predictions_path.exists():
+        logger.warning(
+            "calc_top3_and_consolidation: output file exist and force is False, so "
+            f"stop: {output_predictions_path}"
+        )
+        return
+
+    # Read input files
+    logger.info("Read input file")
+    proba_df = pdh.read_file(input_parcel_probabilities_path)
+
+    top3_df = calc_top3(proba_df)
+
+    # Read input files
+    logger.info("Read input file")
+    input_parcel_df = pdh.read_file(input_parcel_path)
+
+    # All input parcels must stay in the output, so left join input with pred
+    top3_df.set_index(conf.columns["id"], inplace=True)
+    if input_parcel_df.index.name != conf.columns["id"]:
+        input_parcel_df.set_index(conf.columns["id"], inplace=True)
+    cols_to_join = top3_df.columns.difference(input_parcel_df.columns)
+    pred_df = input_parcel_df.join(top3_df[cols_to_join], how="left")
+
+    # The parcels added by the join don't have a prediction yet, so apply it
+    # For the ignore classes, set the prediction to the ignore type
+    classes_to_ignore = conf.marker.getlist("classes_to_ignore")
+    pred_df.loc[
+        pred_df[conf.columns["class_declared"]].isin(classes_to_ignore), "pred1"
+    ] = pred_df[conf.columns["class_declared"]]
+    # For all other parcels without prediction there must have been no data
+    # available for a classification, so set prediction to NODATA
+    pred_df["pred1"].fillna("NODATA", inplace=True)
+
+    # Add doubt columns
+    add_doubt_column(
+        pred_df=pred_df,
+        new_pred_column=conf.columns["prediction_cons"],
+        apply_doubt_pct_proba=True,
+        apply_doubt_min_nb_pixels=True,
+        apply_doubt_marker_specific=False,
+    )
+    add_doubt_column(
+        pred_df=pred_df,
+        new_pred_column=conf.columns["prediction_full_alpha"],
+        apply_doubt_pct_proba=True,
+        apply_doubt_min_nb_pixels=True,
+        apply_doubt_marker_specific=True,
+    )
+
+    # Calculate the status of the consolidated prediction (OK=usable, NOK=not)
+    pred_df.loc[
+        pred_df[conf.columns["prediction_full_alpha"]].isin(proba_df.columns),
+        conf.columns["prediction_cons_status"],
+    ] = "OK"
+    pred_df[conf.columns["prediction_cons_status"]].fillna("NOK", inplace=True)
+
+    logger.info("Write full prediction data to file")
+    pdh.to_file(pred_df, output_predictions_path)
+
+    # Output to geo file
+    input_parcel_gdf = gfo.read_file(input_parcel_geopath)
+    pred_gdf = gpd.GeoDataFrame(input_parcel_gdf.merge(pred_df, how="inner"))
+    pred_gdf.to_file(output_predictions_geopath, engine="pyogrio")
+
+    # Create final output file with the most important info
+    if output_predictions_output_path is not None:
+        # First add some aditional columns specific for the export
+        pred_df["markercode"] = conf.marker["markertype"]
+        pred_df["run_id"] = conf.general["run_id"]
+        today = datetime.date.today()
+        pred_df["cons_date"] = today
+        pred_df["modify_date"] = today
+        logger.info("Write final output prediction data to file")
+        pred_df.reset_index(inplace=True)
+        pred_df = pred_df[conf.columns.getlist("output_columns")]
+        pdh.to_file(
+            pred_df, output_predictions_output_path, index=False  # type: ignore
+        )
+
+        # Write oracle sqlldr file
+        table_name = None
+        table_columns = None
+        if conf.marker["markertype"] in ["LANDCOVER", "LANDCOVER-EARLY"]:
+            table_name = "mon_marker_landcover"
+            table_columns = (
+                "layer_id, prc_id, versienummer, markercode, run_id, cons_input, "
+                "cons_landcover, cons_status, cons_date date 'yyyy-mm-dd', landcover1, "
+                "probability1, landcover2, probability2, landcover3, probability3, "
+                "modify_date date 'yyyy-mm-dd'"
+            )
+        elif conf.marker["markertype"] in ["CROPGROUP", "CROPGROUP-EARLY"]:
+            table_name = "mon_marker_cropgroup"
+            table_columns = (
+                "layer_id, prc_id, versienummer, markercode, run_id, cons_input, "
+                "cons_cropgroup, cons_status, cons_date date 'yyyy-mm-dd', cropgroup1, "
+                "probability1, cropgroup2, probability2, cropgroup3, probability3, "
+                "modify_date date 'yyyy-mm-dd'"
+            )
+        else:
+            table_name = None
+            logger.warning(
+                f"Table unknown for marker type {conf.marker['markertype']}, so cannot "
+                "write .ctl file"
+            )
+
+        if table_name is not None and table_columns is not None:
+            with open(str(output_predictions_output_path) + ".ctl", "w") as ctlfile:
+                # SKIP=1 to skip the columns names line, the other ones to evade
+                # more commits than needed
+                ctlfile.write(
+                    "OPTIONS (SKIP=1, ROWS=10000, BINDSIZE=40000000, "
+                    "READSIZE=40000000)\n"
+                )
+                ctlfile.write("LOAD DATA\n")
+                ctlfile.write(
+                    f"INFILE '{output_predictions_output_path.name}'  \"str '\\n'\"\n"
+                )
+                ctlfile.write(f"INSERT INTO TABLE {table_name} APPEND\n")
+                # A tab as seperator is apparently X'9'
+                ctlfile.write("FIELDS TERMINATED BY X'9'\n")
+                ctlfile.write(f"({table_columns})\n")
+
+
+def calc_top3(proba_df: pd.DataFrame) -> pd.DataFrame:
+    # Calculate the top 3 predictions
+    logger.info("Calculate top3")
+    proba_tmp_df = proba_df.copy()
+    for column in proba_tmp_df.columns:
+        if column in conf.preprocess.getlist("dedicated_data_columns"):
+            proba_tmp_df.drop(column, axis=1, inplace=True)
+
+    # Get the top 3 predictions for each row
+    # First get the indices of the top 3 predictions for each row
+    # Remark: argsort sorts ascending, so we need to take:
+    #     - "[:,": for all rows
+    #     - ":-4": the last 3 elements of the values
+    #     - ":-1]": and than reverse the order with a negative step
+    top3_pred_classes_idx = np.argsort(proba_tmp_df.values, axis=1)[:, :-4:-1]
+    # Convert the indices to classes
+    top3_pred_classes = np.take(proba_tmp_df.columns, top3_pred_classes_idx)
+    # Get the values of the top 3 predictions
+    top3_pred_values = np.sort(proba_tmp_df.values, axis=1)[:, :-4:-1]
+    # Concatenate both
+    top3_pred = np.concatenate([top3_pred_classes, top3_pred_values], axis=1)
+    # Concatenate the ids, the classes and the top3 predictions
+    id_class_top3 = np.concatenate(
+        [
+            proba_df[[conf.columns["id"], conf.columns["class_declared"]]].values,
+            top3_pred,
+        ],
+        axis=1,
+    )
+
+    # Convert to dataframe
+    # Also apply infer_objects: otherwise the float columns are of object dtype.
+    top3_df = pd.DataFrame(
+        id_class_top3,
+        columns=[
+            conf.columns["id"],
+            conf.columns["class_declared"],
+            "pred1",
+            "pred2",
+            "pred3",
+            "pred1_prob",
+            "pred2_prob",
+            "pred3_prob",
+        ],
+    ).infer_objects()
+
+    return top3_df
+
+
+def add_doubt_column(
+    pred_df: pd.DataFrame,
+    new_pred_column: str,
+    apply_doubt_pct_proba: bool,
+    apply_doubt_min_nb_pixels: bool,
+    apply_doubt_marker_specific: bool,
+):
+    # Calculate predictions with doubt column
+    classes_to_ignore = conf.marker.getlist("classes_to_ignore")
+
+    # Init with the standard prediction
+    pred_df[new_pred_column] = "UNDEFINED"
+
+    # If NODATA OR ignore class, retained those from pred1
+    pred_df.loc[
+        (pred_df[new_pred_column] == "UNDEFINED")
+        & (
+            (pred_df["pred1"] == "NODATA")
+            | (pred_df[conf.columns["class_declared"]].isin(classes_to_ignore))
+        ),
+        new_pred_column,
+    ] = pred_df["pred1"]
+
+    # Doubt based on percentage probability
+    if apply_doubt_pct_proba:
+        # Apply doubt for parcels with a low percentage of probability -> = doubt!
+        doubt_proba1_st_2_x_proba2 = conf.postprocess.getboolean(
+            "doubt_proba1_st_2_x_proba2"
+        )
+        if doubt_proba1_st_2_x_proba2 is True:
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (
+                    pred_df["pred1_prob"].map(float)
+                    < 2.0 * pred_df["pred2_prob"].map(float)
+                ),
+                new_pred_column,
+            ] = "DOUBT:PROBA1<2*PROBA2"
+
+        # Apply doubt for parcels with prediction != unverified input
+        doubt_pred_ne_input_proba1_st_pct = conf.postprocess.getfloat(
+            "doubt_pred_ne_input_proba1_st_pct"
+        )
+        if doubt_pred_ne_input_proba1_st_pct > 0:
+            if doubt_pred_ne_input_proba1_st_pct > 100:
+                raise Exception(
+                    "doubt_pred_ne_input_proba1_st_pct should be float from 0 till 100,"
+                    f" not {doubt_pred_ne_input_proba1_st_pct}"
+                )
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (pred_df["pred1"] != pred_df[conf.columns["class_declared"]])
+                & (
+                    pred_df["pred1_prob"].map(float)
+                    < (doubt_pred_ne_input_proba1_st_pct / 100)
+                ),
+                new_pred_column,
+            ] = "DOUBT:PRED<>INPUT-PROBA1<X"
+
+        # Apply doubt for parcels with prediction == unverified input
+        doubt_pred_eq_input_proba1_st_pct = conf.postprocess.getfloat(
+            "doubt_pred_eq_input_proba1_st_pct"
+        )
+        if doubt_pred_eq_input_proba1_st_pct > 0:
+            if doubt_pred_eq_input_proba1_st_pct > 100:
+                raise Exception(
+                    "doubt_pred_ne_input_proba1_st_pct should be float from 0 till 100,"
+                    f" not {doubt_pred_eq_input_proba1_st_pct}"
+                )
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (pred_df["pred1"] == pred_df[conf.columns["class_declared"]])
+                & (
+                    pred_df["pred1_prob"].map(float)
+                    < (doubt_pred_eq_input_proba1_st_pct / 100)
+                ),
+                new_pred_column,
+            ] = "DOUBT:PRED=INPUT-PROBA1<X"
+
+    # Marker specific doubt
+    if apply_doubt_marker_specific is True:
+        # Apply some extra, marker-specific doubt algorythms
+        if conf.marker["markertype"] in ("LANDCOVER", "LANDCOVER-EARLY"):
+            logger.info("Apply some marker-specific doubt algorythms")
+
+            # Remarks:
+            #   - To be sure apply RISKY_DOUBT first, so if there would be
+            #     overlapping criteria, RISKY_DOUBT "wins".
+            #   - Don't overwrite existing DOUBT on parcels, because the
+            #     general doubt reasons should win compared to the marker
+            #     specific doubt/risky_doubt reasons.
+            #   - RISKY DOUBT is used when ground truth resulted in partly alpha
+            #     errors, partly correct, classifications.
+
+            # If parcel was declared as grassland, and is classified as arable, set to
+            # risky doubt.
+            # Remark: those gave 50% false positives for LANDCOVER marker
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (pred_df[conf.columns["class_declared"]] == "MON_LC_GRASSES")
+                & (pred_df["pred1"] == "MON_LC_ARABLE"),
+                new_pred_column,
+            ] = "RISKY_DOUBT:GRASS-SEEN-AS-ARABLE"
+
+            # If parcel was declared as fallow, and is classified as something else,
+            # set to doubt.
+            # Remark: those gave 50% false positives for marker LANDCOVER
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (pred_df[conf.columns["class_declared"]] == "MON_LC_FALLOW")
+                & (pred_df["pred1"] != "MON_LC_FALLOW"),
+                new_pred_column,
+            ] = "RISKY_DOUBT:FALLOW-UNCONFIRMED"
+
+            # If parcel was declared as "9603: Boomkweek-sierplanten", but is not
+            # classified as such: doubt
+            # Remark: they gave 50% false positives for marker LANDCOVER
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (pred_df[conf.columns["crop_declared"]].isin(["9603"]))
+                & (pred_df["pred1"] == "MON_LC_GRASSES"),
+                new_pred_column,
+            ] = "RISKY_DOUBT:BOOMSIER-SEEN-AS-GRASSES"
+
+            # If parcel was declared as grain, but is not classified as MON_LC_ARABLE:
+            # doubt
+            # Remark: - those gave > 50% false positives for marker LANDCOVER-EARLY
+            #         - gave > 33 % false positives for marker LANDCOVER
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (
+                    pred_df[conf.columns["crop_declared"]].isin(
+                        ["39", "311", "321", "322", "331", "342", "639", "646"]
+                    )
+                )
+                & (pred_df["pred1"] != "MON_LC_ARABLE"),
+                new_pred_column,
+            ] = "RISKY_DOUBT:GRAIN-UNCONFIRMED"
+
+            # If parcel was declared as one of the following fabaceae, but is not
+            # classified as such: doubt
+            # Remark: - those gave > 50% false positives for marker LANDCOVER-EARLY
+            #         - gave 33-100% false positives for marker LANDCOVER
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (
+                    pred_df[conf.columns["crop_declared"]].isin(
+                        [
+                            "43",
+                            "51",
+                            "52",
+                            "721",
+                            "722",
+                            "731",
+                            "732",
+                            "831",
+                            "931",
+                            "8410",
+                        ]
+                    )
+                )
+                & (pred_df["pred1"] != "MON_LC_FABACEAE"),
+                new_pred_column,
+            ] = "RISKY_DOUBT:FABACEAE-UNCONFIRMED"
+
+            # Declared class was not correct, but groundtruth class is permanent
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (pred_df[conf.columns["class_declared"]] != pred_df["pred1"])
+                & (pred_df["pred1"].isin(["MON_LC_BOS", "MON_LC_HEIDE"])),
+                new_pred_column,
+            ] = "RISKY_DOUBT:DECL<>PRED-PRED=" + pred_df["pred1"].map(str)
+
+            # If parcel was declared as some arable crops (9534 = knolvenkel), and is
+            # classified as fabaceae, set to doubt
+            # Remark: those gave 100% false positives for marker LANDCOVER
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (pred_df[conf.columns["crop_declared"]].isin(["9534"]))
+                & (pred_df["pred1"] == "MON_LC_FABACEAE"),
+                new_pred_column,
+            ] = "DOUBT:ARABLE-SEEN-AS-FABACEAE"
+
+            # If parcel was declared as 'other herbs' or 'flowers', but is not
+            # confirmed as MON_LC_ARABLE classified as such: doubt
+            # Remark: - those gave > 50% false positives for marker LANDCOVER-EARLY
+            #         - gave 33-50% false positives for marker LANDCOVER
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (pred_df[conf.columns["crop_declared"]].isin(["956", "957", "9831"]))
+                & (pred_df["pred1"] != "MON_LC_ARABLE"),
+                new_pred_column,
+            ] = "RISKY_DOUBT:HERBS-UNCONFIRMED"
+
+            # If parcel was declared as 'aardbeien', but is not confirmed as
+            # MON_LC_ARABLE classified as such: doubt
+            # Remark: - those gave > 50% false positives for marker LANDCOVER-EARLY
+            #         - gave 33-50% false positives for marker LANDCOVER
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (pred_df[conf.columns["crop_declared"]].isin(["9516"]))
+                & (pred_df["pred1"] != "MON_LC_ARABLE"),
+                new_pred_column,
+            ] = "RISKY_DOUBT:AARDBEIEN-UNCONFIRMED"
+
+            # Declared class was not correct, but groundtruth class is permanent
+            # TODO: probably dirty this is hardcoded here!
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (pred_df[conf.columns["class_declared"]] != pred_df["pred1"])
+                & (
+                    pred_df["pred1"].isin(
+                        ["MON_LC_BOS", "MON_LC_HEIDE", "MON_LC_OVERK_LOO"]
+                    )
+                ),
+                new_pred_column,
+            ] = "RISKY_DOUBT:DECL<>PRED-PRED=" + pred_df["pred1"].map(str)
+
+            # If parcel was declared as 9410 and classified as ARABLE, set to doubt
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (pred_df[conf.columns["crop_declared"]].isin(["9410"]))
+                & (pred_df["pred1"] == "MON_LC_ARABLE"),
+                new_pred_column,
+            ] = "RISKY_DOUBT:STAMSLABONEN-SEEN-AS-ARABLE"
+
+            # If parcel was declared as 9602 and classified as FRUIT, set to doubt
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (pred_df[conf.columns["crop_declared"]].isin(["9602"]))
+                & (pred_df["pred1"] == "MON_LC_FRUIT"),
+                new_pred_column,
+            ] = "RISKY_DOUBT:BOOM/FRUITKWEEK-UNCONFIRMED"
+
+            # Parcel was declared as one of the following + classified as GRASSES
+            #
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (
+                    pred_df[conf.columns["crop_declared"]].isin(
+                        [
+                            "36",
+                            "895",
+                            "9582",
+                            #                            "744",
+                            #                            "9202",
+                            #                            "9714",
+                            #                            "832",
+                            #                            "9602",
+                            #                            "9730",
+                        ]
+                    )
+                )
+                & (pred_df["pred1"] == "MON_LC_GRASSES"),
+                new_pred_column,
+            ] = "RISKY_DOUBT:SEEN-AS-GRASSES"
+
+            # Parcel was declared as one of the following and classified as ARABLE
+            # Ground truth in some cases confirmed the classification, in others
+            # resulted in alpha errors -> RISKY_DOUBT
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (
+                    pred_df[conf.columns["crop_declared"]].isin(
+                        ["601", "644", "932", "9412", "9584", "8411"]
+                    )
+                )
+                & (pred_df["pred1"] == "MON_LC_ARABLE"),
+                new_pred_column,
+            ] = "RISKY_DOUBT:SEEN-AS-ARABLE"
+
+            # If parcel was declared as one of the following and classified as
+            # FABACEAE, set to RISKY_DOUBT
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (pred_df[conf.columns["crop_declared"]].isin(["9546"]))
+                & (pred_df["pred1"] == "MON_LC_FABACEAE"),
+                new_pred_column,
+            ] = "RISKY_DOUBT:SAVOOIKOOL-SEEN-AS-FABACEAE"
+
+        elif conf.marker["markertype"] in ("CROPGROUP", "CROPGROUP-EARLY"):
+            logger.info("Apply some marker-specific doubt algorythms")
+
+            # Red parcels declared as MON_TRITICALE always seem to be predicted wrong,
+            # so place them in doubt
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (pred_df[conf.columns["class_declared"]] != pred_df["pred1"])
+                & (pred_df[conf.columns["class_declared"]] == "MON_TRITICALE"),
+                new_pred_column,
+            ] = "RISKY_DOUBT:TRITICALE-UNCONFIRMED"
+
+            # Red parcels with MON_HEIDE seem to have a difficult time seeing the
+            # difference between MON_HEIDE and MON_GRASSEN
+            pred_df.loc[
+                (pred_df[new_pred_column] == "UNDEFINED")
+                & (pred_df[conf.columns["class_declared"]] != pred_df["pred1"])
+                & (pred_df["pred1"] == "MON_HEIDE"),
+                new_pred_column,
+            ] = "RISKY_DOUBT:HEIDE-UNCONFIRMED"
+
+            """
+            # Note: this will INCREASE the alpha errors, because we remove a large
+            # portion of red parcels to doubt (~886 parcels => 16 alpha errors)
+            pred_df.loc[
+                ((pred_df[new_pred_column] == 'UNDEFINED') |
+                        (~pred_df[new_pred_column].str.startswith('DOUBT')))
+                    & (pred_df[conf.columns['class_declared']] != pred_df['pred1'])
+                    & (pred_df[conf.columns['class_declared']] == 'MON_GRASSEN'),
+                    new_pred_column
+            ] = 'RISKY_DOUBT:GRASSEN-UNCONFIRMED'
+            """
+
+    # Accuracy with few pixels might be lower, so set those to doubt
+    if apply_doubt_min_nb_pixels is True:
+        pred_df.loc[
+            (
+                pred_df[conf.columns["pixcount_s1s2"]]
+                < conf.marker.getfloat("min_nb_pixels")
+            )
+            & (~pred_df[new_pred_column].str.startswith("DOUBT")),
+            new_pred_column,
+        ] = "DOUBT:NOT_ENOUGH_PIXELS"
+
+    # Finally, predictions that have no value yet, get the original prediction
+    pred_df.loc[pred_df[new_pred_column] == "UNDEFINED", new_pred_column] = pred_df[
+        "pred1"
+    ]
```

### Comparing `cropclassification-0.1.0a2/cropclassification/postprocess/html_rapport_script.js` & `cropclassification-0.1.1/cropclassification/postprocess/html_rapport_script.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,183 +1,183 @@
-var IS_LOCAL_DEV = true;
-
-$(document).ready(function() {
-
-    $("table")
-        .removeAttr("border")
-        .addClass("table table-striped table-hover table-sm");
-
-    $("button.toggle-button")
-        .on("click", function(e) {
-            $(e.target).siblings().closest(".toggle-visible").toggle();
-        });
-
-    chart_general_accuracies(document.getElementById("chart_general_accuracies"), general_acuracies_data.count);
-    chart_confusion_matrices(document.getElementById("chart_confusion_matrices"), confusion_matrices_data);
-    chart_confusion_matrices(document.getElementById("chart_confusion_matrices_consolidated"), confusion_matrices_consolidated_data);
-
-    function chart_general_accuracies(elem, data) {
-        var chartLegend = [];
-        var chartData = [];
-
-        Object.keys(data).forEach(function(key, index) {
-            chartLegend.push(key);
-            chartData.push({
-                name: key,
-                value: data[key]
-            });
-        });
-
-        var chart = echarts.init(elem);
-        var chartOptions = {
-            tooltip: {
-                formatter: "{a} <br/>{b}: {c} ({d}%)"
-            },
-            legend: {
-                orient: 'vertical',
-                x: 'left',
-                data: chartLegend
-            },
-            toolbox: {
-                show: true,
-                feature: {
-                    dataView: {
-                        show: true,
-                        readOnly: false
-                    },
-                    restore: {
-                        show: true
-                    },
-                    saveAsImage: {
-                        show: true
-                    }
-                }
-            },
-            calculable: true,
-            series: {
-                name: 'accuracies',
-                type: 'pie',
-                radius: ['50%', '70%'],
-                avoidLabelOverlap: false,
-                label: {
-                    normal: {
-                        show: false,
-                        position: 'center'
-                    },
-                    emphasis: {
-                        show: true,
-                        textStyle: {
-                            fontSize: '30',
-                            fontWeight: 'bold'
-                        }
-                    }
-                },
-                labelLine: {
-                    normal: {
-                        show: false
-                    }
-                },
-                data: chartData
-            }
-        };
-
-        if (chartOptions && typeof chartOptions === "object") {
-            chart.setOption(chartOptions, true);
-        }
-    }
-
-    function chart_confusion_matrices(elem, data) {
-
-        // data verwerken
-        var rows = Object.keys(data).filter(x => !x.startsWith("nb_") && !x.startsWith("pct_"));
-        var series = [];
-        var categories = [];
-
-        rows.forEach(function(rowKey, rowIndex) {
-            categories.push(rowKey);
-
-            rows.forEach(function(columnKey, columnIndex) {
-                // per rij loopen en de kolom waarde (=predicted value) ophalen
-                series.push([rowIndex, columnIndex, data[rowKey][columnKey] || "-"]);
-            });
-        });
-
-        var chart = echarts.init(elem);
-        var chartOptions = {
-            tooltip: {
-                position: 'top',
-                formatter: function(params) {
-                    var categoryX = categories[params.value[0]];
-                    var categoryY = categories[params.value[1]];
-
-                    var nb_input_x = data.nb_input[categoryX];
-                    var nb_predicted_x = data.nb_predicted[categoryX];
-                    var nb_predicted_x_correct = data.nb_predicted_correct[categoryX];
-                    var nb_predicted_x_wrong = data.nb_predicted_wrong[categoryX];
-                    var pct_predicted_x_correct = data.pct_predicted_correct[categoryX];
-                    var pct_predicted_x_wrong = data.pct_predicted_wrong[categoryX];
-
-                    var nb_input_y = data.nb_input[categoryY];
-                    var nb_predicted_y = data.nb_predicted[categoryY];
-                    var nb_predicted_y_correct = data.nb_predicted_correct[categoryY];
-                    var nb_predicted_y_wrong = data.nb_predicted_wrong[categoryY];
-                    var pct_predicted_y_correct = data.pct_predicted_correct[categoryY];
-                    var pct_predicted_y_wrong = data.pct_predicted_wrong[categoryY];
-
-                    return params.value[2] + "/" + nb_input_x + "<br/>" +
-                        categoryX + " (input: " + nb_input_x + ", predicted: " + nb_predicted_x + ")<br/>" +
-                        "&nbsp;&nbsp;&nbsp;<span class='oi oi-thumb-up text-success'></span>" + (pct_predicted_x_correct || 0).toFixed(2) + "%" +
-                        "(" + nb_predicted_x_correct + "/" + nb_input_x + "), <span class='oi oi-thumb-down text-danger'></span>" + (pct_predicted_x_wrong || 0).toFixed(2) + "% (" + nb_predicted_x_wrong + "/" + nb_input_x + ")<br/>" +
-                        categoryY + " (input: " + nb_input_y + ", predicted: " + nb_predicted_y + ")<br/>" +
-                        "&nbsp;&nbsp;&nbsp;<span class='oi oi-thumb-up text-success'></span>" + (pct_predicted_y_correct || 0).toFixed(2) + "%" +
-                        "(" + nb_predicted_y_correct + "/" + nb_input_y + "), <span class='oi oi-thumb-down text-danger'></span>" + (pct_predicted_y_wrong || 0).toFixed(2) + "% (" + nb_predicted_y_wrong + "/" + nb_input_y + ")<br/>";
-                }
-            },
-            legend: {
-                data: categories
-            },
-            grid: {
-                left: 2,
-                bottom: 10,
-                right: 10,
-                containLabel: true
-            },
-            xAxis: {
-                type: 'category',
-                data: categories,
-                boundaryGap: false
-            },
-            yAxis: {
-                type: 'category',
-                data: categories
-            },
-            series: {
-                name: "confusion matrices",
-                type: "scatter",
-                data: series,
-                large: true,
-                itemStyle: {
-                    color: function(params) {
-                        return params.value[0] === params.value[1] ?
-                            "green" :
-                            "red";
-                    }
-                },
-                symbolSize: function(val) {
-                    if (val[2] === "-") return 0;
-
-                    var denomitor = data.nb_predicted[categories[val[0]]];
-                    if (categories[val[0]] === "DOUBT") {
-                        // NOTE: If we're comparing with DOUBT, then use the predicted value of the comparing crop. This provides more information.
-                        denomitor = data.nb_predicted[categories[val[1]]];
-                    }
-
-                    return (val[2] / denomitor) * 100;
-                }
-            }
-        };
-
-        if (chartOptions && typeof chartOptions === "object") {
-            chart.setOption(chartOptions, true);
-        }
-    }
+var IS_LOCAL_DEV = true;
+
+$(document).ready(function() {
+
+    $("table")
+        .removeAttr("border")
+        .addClass("table table-striped table-hover table-sm");
+
+    $("button.toggle-button")
+        .on("click", function(e) {
+            $(e.target).siblings().closest(".toggle-visible").toggle();
+        });
+
+    chart_general_accuracies(document.getElementById("chart_general_accuracies"), general_acuracies_data.count);
+    chart_confusion_matrices(document.getElementById("chart_confusion_matrices"), confusion_matrices_data);
+    chart_confusion_matrices(document.getElementById("chart_confusion_matrices_consolidated"), confusion_matrices_consolidated_data);
+
+    function chart_general_accuracies(elem, data) {
+        var chartLegend = [];
+        var chartData = [];
+
+        Object.keys(data).forEach(function(key, index) {
+            chartLegend.push(key);
+            chartData.push({
+                name: key,
+                value: data[key]
+            });
+        });
+
+        var chart = echarts.init(elem);
+        var chartOptions = {
+            tooltip: {
+                formatter: "{a} <br/>{b}: {c} ({d}%)"
+            },
+            legend: {
+                orient: 'vertical',
+                x: 'left',
+                data: chartLegend
+            },
+            toolbox: {
+                show: true,
+                feature: {
+                    dataView: {
+                        show: true,
+                        readOnly: false
+                    },
+                    restore: {
+                        show: true
+                    },
+                    saveAsImage: {
+                        show: true
+                    }
+                }
+            },
+            calculable: true,
+            series: {
+                name: 'accuracies',
+                type: 'pie',
+                radius: ['50%', '70%'],
+                avoidLabelOverlap: false,
+                label: {
+                    normal: {
+                        show: false,
+                        position: 'center'
+                    },
+                    emphasis: {
+                        show: true,
+                        textStyle: {
+                            fontSize: '30',
+                            fontWeight: 'bold'
+                        }
+                    }
+                },
+                labelLine: {
+                    normal: {
+                        show: false
+                    }
+                },
+                data: chartData
+            }
+        };
+
+        if (chartOptions && typeof chartOptions === "object") {
+            chart.setOption(chartOptions, true);
+        }
+    }
+
+    function chart_confusion_matrices(elem, data) {
+
+        // data verwerken
+        var rows = Object.keys(data).filter(x => !x.startsWith("nb_") && !x.startsWith("pct_"));
+        var series = [];
+        var categories = [];
+
+        rows.forEach(function(rowKey, rowIndex) {
+            categories.push(rowKey);
+
+            rows.forEach(function(columnKey, columnIndex) {
+                // per rij loopen en de kolom waarde (=predicted value) ophalen
+                series.push([rowIndex, columnIndex, data[rowKey][columnKey] || "-"]);
+            });
+        });
+
+        var chart = echarts.init(elem);
+        var chartOptions = {
+            tooltip: {
+                position: 'top',
+                formatter: function(params) {
+                    var categoryX = categories[params.value[0]];
+                    var categoryY = categories[params.value[1]];
+
+                    var nb_input_x = data.nb_input[categoryX];
+                    var nb_predicted_x = data.nb_predicted[categoryX];
+                    var nb_predicted_x_correct = data.nb_predicted_correct[categoryX];
+                    var nb_predicted_x_wrong = data.nb_predicted_wrong[categoryX];
+                    var pct_predicted_x_correct = data.pct_predicted_correct[categoryX];
+                    var pct_predicted_x_wrong = data.pct_predicted_wrong[categoryX];
+
+                    var nb_input_y = data.nb_input[categoryY];
+                    var nb_predicted_y = data.nb_predicted[categoryY];
+                    var nb_predicted_y_correct = data.nb_predicted_correct[categoryY];
+                    var nb_predicted_y_wrong = data.nb_predicted_wrong[categoryY];
+                    var pct_predicted_y_correct = data.pct_predicted_correct[categoryY];
+                    var pct_predicted_y_wrong = data.pct_predicted_wrong[categoryY];
+
+                    return params.value[2] + "/" + nb_input_x + "<br/>" +
+                        categoryX + " (input: " + nb_input_x + ", predicted: " + nb_predicted_x + ")<br/>" +
+                        "&nbsp;&nbsp;&nbsp;<span class='oi oi-thumb-up text-success'></span>" + (pct_predicted_x_correct || 0).toFixed(2) + "%" +
+                        "(" + nb_predicted_x_correct + "/" + nb_input_x + "), <span class='oi oi-thumb-down text-danger'></span>" + (pct_predicted_x_wrong || 0).toFixed(2) + "% (" + nb_predicted_x_wrong + "/" + nb_input_x + ")<br/>" +
+                        categoryY + " (input: " + nb_input_y + ", predicted: " + nb_predicted_y + ")<br/>" +
+                        "&nbsp;&nbsp;&nbsp;<span class='oi oi-thumb-up text-success'></span>" + (pct_predicted_y_correct || 0).toFixed(2) + "%" +
+                        "(" + nb_predicted_y_correct + "/" + nb_input_y + "), <span class='oi oi-thumb-down text-danger'></span>" + (pct_predicted_y_wrong || 0).toFixed(2) + "% (" + nb_predicted_y_wrong + "/" + nb_input_y + ")<br/>";
+                }
+            },
+            legend: {
+                data: categories
+            },
+            grid: {
+                left: 2,
+                bottom: 10,
+                right: 10,
+                containLabel: true
+            },
+            xAxis: {
+                type: 'category',
+                data: categories,
+                boundaryGap: false
+            },
+            yAxis: {
+                type: 'category',
+                data: categories
+            },
+            series: {
+                name: "confusion matrices",
+                type: "scatter",
+                data: series,
+                large: true,
+                itemStyle: {
+                    color: function(params) {
+                        return params.value[0] === params.value[1] ?
+                            "green" :
+                            "red";
+                    }
+                },
+                symbolSize: function(val) {
+                    if (val[2] === "-") return 0;
+
+                    var denomitor = data.nb_predicted[categories[val[0]]];
+                    if (categories[val[0]] === "DOUBT") {
+                        // NOTE: If we're comparing with DOUBT, then use the predicted value of the comparing crop. This provides more information.
+                        denomitor = data.nb_predicted[categories[val[1]]];
+                    }
+
+                    return (val[2] / denomitor) * 100;
+                }
+            }
+        };
+
+        if (chartOptions && typeof chartOptions === "object") {
+            chart.setOption(chartOptions, true);
+        }
+    }
 });
```

### Comparing `cropclassification-0.1.0a2/cropclassification/postprocess/html_rapport_test.py` & `cropclassification-0.1.1/cropclassification/postprocess/html_rapport_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-import os
-from pathlib import Path
-import sys
-
-[sys.path.append(i) for i in [".", ".."]]
-import cropclassification.postprocess.classification_reporting as class_report
-
-base_dir = Path("x:/Monitoring/Markers/PlayGround/JoeBro")
-input_dir = base_dir / "InputData"
-class_base_dir = base_dir / "HTML"
-input_groundtruth_path = input_dir / "Prc_BEFL_2018_groundTruth.csv"
-parcel_pixcount_path = input_dir / "BEFL2018_bufm10_weekly_pixcount.csv"
-
-parcel_predictions_all_path = (
-    class_base_dir / "BEFL2018_bufm10_weekly_predict_all.csv"
-)
-groundtruth_path = class_base_dir / "Prc_BEFL_2018_groundTruth_classes.csv"
-report_txt = class_base_dir / "testje_accuracy_report.txt"
-report_html = Path(str(report_txt).replace(".txt", ".html"))
-
-if report_txt.exists():
-    os.remove(report_txt)
-if report_html.exists():
-    os.remove(report_html)
-
-class_report.write_full_report(
-    parcel_predictions_geopath=parcel_predictions_all_path,
-    output_report_txt=report_txt,
-    parcel_ground_truth_path=groundtruth_path,
-    force=True,
-)
+import os
+from pathlib import Path
+
+import cropclassification.postprocess.classification_reporting as class_report
+
+base_dir = Path("x:/Monitoring/Markers/PlayGround/JoeBro")
+input_dir = base_dir / "InputData"
+class_base_dir = base_dir / "HTML"
+input_groundtruth_path = input_dir / "Prc_BEFL_2018_groundTruth.csv"
+parcel_pixcount_path = input_dir / "BEFL2018_bufm10_weekly_pixcount.csv"
+
+parcel_predictions_all_path = class_base_dir / "BEFL2018_bufm10_weekly_predict_all.csv"
+groundtruth_path = class_base_dir / "Prc_BEFL_2018_groundTruth_classes.csv"
+report_txt = class_base_dir / "testje_accuracy_report.txt"
+report_html = Path(str(report_txt).replace(".txt", ".html"))
+
+if report_txt.exists():
+    os.remove(report_txt)
+if report_html.exists():
+    os.remove(report_html)
+
+class_report.write_full_report(
+    parcel_predictions_geopath=parcel_predictions_all_path,
+    output_report_txt=report_txt,
+    parcel_ground_truth_path=groundtruth_path,
+    force=True,
+)
```

### Comparing `cropclassification-0.1.0a2/cropclassification/predict/classification.py` & `cropclassification-0.1.1/cropclassification/predict/classification.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,293 +1,297 @@
-# -*- coding: utf-8 -*-
-"""
-Module that implements the classification logic.
-"""
-
-import ast
-import glob
-import logging
-import os
-from pathlib import Path
-from typing import Optional
-
-import pandas as pd
-
-import cropclassification.helpers.config_helper as conf
-import cropclassification.helpers.pandas_helper as pdh
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-# logger.setLevel(logging.DEBUG)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def train_test_predict(
-    input_parcel_train_path: Path,
-    input_parcel_test_path: Path,
-    input_parcel_all_path: Path,
-    input_parcel_classification_data_path: Path,
-    output_classifier_basepath: Path,
-    output_predictions_test_path: Path,
-    output_predictions_all_path: Path,
-    force: bool = False,
-):
-    """Train a classifier, test it and do full predictions.
-
-    Args
-        input_parcel_classes_train_path: the list of parcels with classes to train the
-            classifier, without data!
-        input_parcel_classes_test_path: the list of parcels with classes to test the
-            classifier, without data!
-        input_parcel_classes_all_path: the list of parcels with classes that need to be
-            classified, without data!
-        input_parcel_classification_data_path: the data to be used for the
-            classification for all parcels.
-        output_classifier_basepath: the file path where to save the classifier.
-        output_predictions_test_path: the file path where to save the test predictions.
-        output_predictions_all_path: the file path where to save the predictions for
-            all parcels.
-        force: if True, overwrite all existing output files, if False, don't overwrite
-            them.
-    """
-
-    logger.info("train_test_predict: Start")
-
-    if (
-        force is False
-        # and os.path.exists(output_classifier_basepath)
-        and output_predictions_test_path.exists()
-        and output_predictions_all_path.exists()
-    ):
-        logger.warning(
-            "predict: output files exist and force is False, so stop: "
-            f"{output_classifier_basepath}, {output_predictions_test_path}, "
-            f"{output_predictions_all_path}"
-        )
-        return
-
-    # Read the classification data from the csv so we can pass it on to the other
-    # functions to improve performance...
-    logger.info(
-        f"Read classification data file: {input_parcel_classification_data_path}"
-    )
-    input_parcel_classification_data_df = pdh.read_file(
-        input_parcel_classification_data_path
-    )
-    if input_parcel_classification_data_df.index.name != conf.columns["id"]:
-        input_parcel_classification_data_df.set_index(conf.columns["id"], inplace=True)
-    logger.debug("Read classification data file ready")
-
-    # Train the classification
-    output_classifier_path = train(
-        input_parcel_train_path=input_parcel_train_path,
-        input_parcel_test_path=input_parcel_test_path,
-        input_parcel_classification_data_path=input_parcel_classification_data_path,
-        output_classifier_basepath=output_classifier_basepath,
-        force=force,
-        input_parcel_classification_data_df=input_parcel_classification_data_df,
-    )
-
-    # Predict the test parcels
-    predict(
-        input_parcel_path=input_parcel_test_path,
-        input_parcel_classification_data_path=input_parcel_classification_data_path,
-        input_classifier_basepath=output_classifier_basepath,
-        input_classifier_path=output_classifier_path,
-        output_predictions_path=output_predictions_test_path,
-        force=force,
-        input_parcel_classification_data_df=input_parcel_classification_data_df,
-    )
-
-    # Predict all parcels
-    predict(
-        input_parcel_path=input_parcel_all_path,
-        input_parcel_classification_data_path=input_parcel_classification_data_path,
-        input_classifier_basepath=output_classifier_basepath,
-        input_classifier_path=output_classifier_path,
-        output_predictions_path=output_predictions_all_path,
-        force=force,
-        input_parcel_classification_data_df=input_parcel_classification_data_df,
-    )
-
-
-def train(
-    input_parcel_train_path: Path,
-    input_parcel_test_path: Path,
-    input_parcel_classification_data_path: Path,
-    output_classifier_basepath: Path,
-    force: bool = False,
-    input_parcel_classification_data_df: Optional[pd.DataFrame] = None,
-) -> Path:
-    """Train a classifier and test it by predicting the test cases."""
-
-    logger.info("train_and_test: Start")
-    if force is False and output_classifier_basepath.exists():
-        logger.warning(
-            "predict: classifier already exist and force == False, so don't retrain: "
-            f"{output_classifier_basepath}"
-        )
-        return output_classifier_basepath
-
-    # If the classification data isn't passed as dataframe, read it from file
-    if input_parcel_classification_data_df is None:
-        logger.info(
-            f"Read classification data file: {input_parcel_classification_data_path}"
-        )
-        input_parcel_classification_data_df = pdh.read_file(
-            input_parcel_classification_data_path
-        )
-        if input_parcel_classification_data_df.index.name != conf.columns["id"]:
-            input_parcel_classification_data_df.set_index(
-                conf.columns["id"], inplace=True
-            )
-        logger.debug("Read classification data file ready")
-
-    # Read the train parcels
-    logger.info(f"Read train file: {input_parcel_train_path}")
-    train_df = pdh.read_file(
-        input_parcel_train_path, columns=[conf.columns["id"], conf.columns["class"]]
-    )
-    if train_df.index.name != conf.columns["id"]:
-        train_df.set_index(conf.columns["id"], inplace=True)
-    logger.debug("Read train file ready")
-
-    # Join the columns of input_parcel_classification_data_df that aren't yet in
-    # train_df
-    logger.info("Join train sample with the classification data")
-    train_df = train_df.join(input_parcel_classification_data_df, how="inner")
-
-    # Read the test/validation data
-    logger.info(f"Read test file: {input_parcel_test_path}")
-    test_df = pdh.read_file(
-        input_parcel_test_path, columns=[conf.columns["id"], conf.columns["class"]]
-    )
-    if test_df.index.name != conf.columns["id"]:
-        test_df.set_index(conf.columns["id"], inplace=True)
-    logger.debug("Read test file ready")
-
-    # Join the columns of input_parcel_classification_data_df that aren't yet in test_df
-    logger.info("Join test sample with the classification data")
-    test_df = test_df.join(input_parcel_classification_data_df, how="inner")
-
-    # Train
-    if conf.classifier["classifier_type"].lower() == "keras_multilayer_perceptron":
-        import cropclassification.predict.classification_keras as class_core_keras
-
-        return class_core_keras.train(
-            train_df=train_df,
-            test_df=test_df,
-            output_classifier_basepath=output_classifier_basepath,
-        )
-    else:
-        import cropclassification.predict.classification_sklearn as class_core_sklearn
-
-        return class_core_sklearn.train(
-            train_df=train_df,
-            output_classifier_basepath=output_classifier_basepath,
-        )
-
-
-def predict(
-    input_parcel_path: Path,
-    input_parcel_classification_data_path: Path,
-    input_classifier_basepath: Path,
-    input_classifier_path: Path,
-    output_predictions_path: Path,
-    force: bool = False,
-    input_parcel_classification_data_df: Optional[pd.DataFrame] = None,
-):
-    """Predict the classes for the input data."""
-
-    # If force is False, and the output file exist already, return
-    if force is False and output_predictions_path.exists():
-        logger.warning(
-            "predict: predictions output file already exists and force is false, so "
-            f"stop: {output_predictions_path}"
-        )
-        return
-
-    # Read the input parcels
-    logger.info(f"Read input file: {input_parcel_path}")
-    input_parcel_df = pdh.read_file(
-        input_parcel_path,
-        columns=[
-            conf.columns["id"],
-            conf.columns["class"],
-            conf.columns["class_declared"],
-        ],
-    )
-    if input_parcel_df.index.name != conf.columns["id"]:
-        input_parcel_df.set_index(conf.columns["id"], inplace=True)
-    logger.debug("Read train file ready")
-
-    # For parcels of a class that should be ignored, don't predict
-    input_parcel_df = input_parcel_df.loc[
-        ~input_parcel_df[conf.columns["class_declared"]].isin(
-            conf.marker.getlist("classes_to_ignore")
-        )
-    ]
-
-    # get the expected columns from the classifier
-    datacolumns_path = glob.glob(
-        os.path.join(os.path.dirname(input_classifier_path), "*datacolumns.txt")
-    )[0]
-    with open(datacolumns_path, "r") as f:
-        input_classifier_datacolumns = ast.literal_eval(f.readline())
-
-    # If the classification data isn't passed as dataframe, read it from the csv
-    if input_parcel_classification_data_df is None:
-        logger.info(
-            f"Read classification data file: {input_parcel_classification_data_path}"
-        )
-        input_parcel_classification_data_df = pdh.read_file(
-            input_parcel_classification_data_path
-        )
-        if input_parcel_classification_data_df.index.name != conf.columns["id"]:
-            input_parcel_classification_data_df.set_index(
-                conf.columns["id"], inplace=True
-            )
-        logger.debug("Read classification data file ready")
-
-    # only take the required columns as expected by the classifier
-    input_parcel_classification_data_df = input_parcel_classification_data_df[
-        input_classifier_datacolumns
-    ]
-
-    # Join the data to send to prediction logic
-    logger.info("Join input parcels with the classification data")
-    input_parcel_for_predict_df = input_parcel_df.join(
-        input_parcel_classification_data_df, how="inner"
-    )
-
-    # Predict!
-    logger.info(f"Predict using this model: {input_classifier_path}")
-    if conf.classifier["classifier_type"].lower() == "keras_multilayer_perceptron":
-        import cropclassification.predict.classification_keras as class_core_keras
-
-        class_core_keras.predict_proba(
-            parcel_df=input_parcel_for_predict_df,
-            classifier_basepath=input_classifier_basepath,
-            classifier_path=input_classifier_path,
-            output_parcel_predictions_path=output_predictions_path,
-        )
-    else:
-        import cropclassification.predict.classification_sklearn as class_core_sklearn
-
-        class_core_sklearn.predict_proba(
-            parcel_df=input_parcel_for_predict_df,
-            classifier_basepath=input_classifier_basepath,
-            classifier_path=input_classifier_path,
-            output_parcel_predictions_path=output_predictions_path,
-        )
-
-
-# If the script is run directly...
-if __name__ == "__main__":
-    logger.critical("Not implemented exception!")
-    raise Exception("Not implemented")
+# -*- coding: utf-8 -*-
+"""
+Module that implements the classification logic.
+"""
+
+import ast
+import glob
+import logging
+import os
+from pathlib import Path
+from typing import Optional
+
+import pandas as pd
+
+import cropclassification.helpers.config_helper as conf
+import cropclassification.helpers.pandas_helper as pdh
+
+# -------------------------------------------------------------
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+# logger.setLevel(logging.DEBUG)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def train_test_predict(
+    input_parcel_train_path: Path,
+    input_parcel_test_path: Path,
+    input_parcel_all_path: Path,
+    input_parcel_classification_data_path: Path,
+    output_classifier_basepath: Path,
+    output_predictions_test_path: Path,
+    output_predictions_all_path: Path,
+    force: bool = False,
+):
+    """Train a classifier, test it and do full predictions.
+
+    Args
+        input_parcel_classes_train_path: the list of parcels with classes to train the
+            classifier, without data!
+        input_parcel_classes_test_path: the list of parcels with classes to test the
+            classifier, without data!
+        input_parcel_classes_all_path: the list of parcels with classes that need to be
+            classified, without data!
+        input_parcel_classification_data_path: the data to be used for the
+            classification for all parcels.
+        output_classifier_basepath: the file path where to save the classifier.
+        output_predictions_test_path: the file path where to save the test predictions.
+        output_predictions_all_path: the file path where to save the predictions for
+            all parcels.
+        force: if True, overwrite all existing output files, if False, don't overwrite
+            them.
+    """
+
+    logger.info("train_test_predict: Start")
+
+    if (
+        force is False
+        # and os.path.exists(output_classifier_basepath)
+        and output_predictions_test_path.exists()
+        and output_predictions_all_path.exists()
+    ):
+        logger.warning(
+            "predict: output files exist and force is False, so stop: "
+            f"{output_classifier_basepath}, {output_predictions_test_path}, "
+            f"{output_predictions_all_path}"
+        )
+        return
+
+    # Read the classification data from the csv so we can pass it on to the other
+    # functions to improve performance...
+    logger.info(
+        f"Read classification data file: {input_parcel_classification_data_path}"
+    )
+    input_parcel_classification_data_df = pdh.read_file(
+        input_parcel_classification_data_path
+    )
+    if input_parcel_classification_data_df.index.name != conf.columns["id"]:
+        input_parcel_classification_data_df.set_index(conf.columns["id"], inplace=True)
+    logger.debug("Read classification data file ready")
+    if len(input_parcel_classification_data_df.columns) == 0:
+        raise ValueError(
+            f"no classification data found in {input_parcel_classification_data_path}"
+        )
+
+    # Train the classification
+    output_classifier_path = train(
+        input_parcel_train_path=input_parcel_train_path,
+        input_parcel_test_path=input_parcel_test_path,
+        input_parcel_classification_data_path=input_parcel_classification_data_path,
+        output_classifier_basepath=output_classifier_basepath,
+        force=force,
+        input_parcel_classification_data_df=input_parcel_classification_data_df,
+    )
+
+    # Predict the test parcels
+    predict(
+        input_parcel_path=input_parcel_test_path,
+        input_parcel_classification_data_path=input_parcel_classification_data_path,
+        input_classifier_basepath=output_classifier_basepath,
+        input_classifier_path=output_classifier_path,
+        output_predictions_path=output_predictions_test_path,
+        force=force,
+        input_parcel_classification_data_df=input_parcel_classification_data_df,
+    )
+
+    # Predict all parcels
+    predict(
+        input_parcel_path=input_parcel_all_path,
+        input_parcel_classification_data_path=input_parcel_classification_data_path,
+        input_classifier_basepath=output_classifier_basepath,
+        input_classifier_path=output_classifier_path,
+        output_predictions_path=output_predictions_all_path,
+        force=force,
+        input_parcel_classification_data_df=input_parcel_classification_data_df,
+    )
+
+
+def train(
+    input_parcel_train_path: Path,
+    input_parcel_test_path: Path,
+    input_parcel_classification_data_path: Path,
+    output_classifier_basepath: Path,
+    force: bool = False,
+    input_parcel_classification_data_df: Optional[pd.DataFrame] = None,
+) -> Path:
+    """Train a classifier and test it by predicting the test cases."""
+
+    logger.info("train_and_test: Start")
+    if force is False and output_classifier_basepath.exists():
+        logger.warning(
+            "predict: classifier already exist and force == False, so don't retrain: "
+            f"{output_classifier_basepath}"
+        )
+        return output_classifier_basepath
+
+    # If the classification data isn't passed as dataframe, read it from file
+    if input_parcel_classification_data_df is None:
+        logger.info(
+            f"Read classification data file: {input_parcel_classification_data_path}"
+        )
+        input_parcel_classification_data_df = pdh.read_file(
+            input_parcel_classification_data_path
+        )
+        if input_parcel_classification_data_df.index.name != conf.columns["id"]:
+            input_parcel_classification_data_df.set_index(
+                conf.columns["id"], inplace=True
+            )
+        logger.debug("Read classification data file ready")
+
+    # Read the train parcels
+    logger.info(f"Read train file: {input_parcel_train_path}")
+    train_df = pdh.read_file(
+        input_parcel_train_path, columns=[conf.columns["id"], conf.columns["class"]]
+    )
+    if train_df.index.name != conf.columns["id"]:
+        train_df.set_index(conf.columns["id"], inplace=True)
+    logger.debug("Read train file ready")
+
+    # Join the columns of input_parcel_classification_data_df that aren't yet in
+    # train_df
+    logger.info("Join train sample with the classification data")
+    train_df = train_df.join(input_parcel_classification_data_df, how="inner")
+
+    # Read the test/validation data
+    logger.info(f"Read test file: {input_parcel_test_path}")
+    test_df = pdh.read_file(
+        input_parcel_test_path, columns=[conf.columns["id"], conf.columns["class"]]
+    )
+    if test_df.index.name != conf.columns["id"]:
+        test_df.set_index(conf.columns["id"], inplace=True)
+    logger.debug("Read test file ready")
+
+    # Join the columns of input_parcel_classification_data_df that aren't yet in test_df
+    logger.info("Join test sample with the classification data")
+    test_df = test_df.join(input_parcel_classification_data_df, how="inner")
+
+    # Train
+    if conf.classifier["classifier_type"].lower() == "keras_multilayer_perceptron":
+        import cropclassification.predict.classification_keras as class_core_keras
+
+        return class_core_keras.train(
+            train_df=train_df,
+            test_df=test_df,
+            output_classifier_basepath=output_classifier_basepath,
+        )
+    else:
+        import cropclassification.predict.classification_sklearn as class_core_sklearn
+
+        return class_core_sklearn.train(
+            train_df=train_df,
+            output_classifier_basepath=output_classifier_basepath,
+        )
+
+
+def predict(
+    input_parcel_path: Path,
+    input_parcel_classification_data_path: Path,
+    input_classifier_basepath: Path,
+    input_classifier_path: Path,
+    output_predictions_path: Path,
+    force: bool = False,
+    input_parcel_classification_data_df: Optional[pd.DataFrame] = None,
+):
+    """Predict the classes for the input data."""
+
+    # If force is False, and the output file exist already, return
+    if force is False and output_predictions_path.exists():
+        logger.warning(
+            "predict: predictions output file already exists and force is false, so "
+            f"stop: {output_predictions_path}"
+        )
+        return
+
+    # Read the input parcels
+    logger.info(f"Read input file: {input_parcel_path}")
+    input_parcel_df = pdh.read_file(
+        input_parcel_path,
+        columns=[
+            conf.columns["id"],
+            conf.columns["class"],
+            conf.columns["class_declared"],
+        ],
+    )
+    if input_parcel_df.index.name != conf.columns["id"]:
+        input_parcel_df.set_index(conf.columns["id"], inplace=True)
+    logger.debug("Read train file ready")
+
+    # For parcels of a class that should be ignored, don't predict
+    input_parcel_df = input_parcel_df.loc[
+        ~input_parcel_df[conf.columns["class_declared"]].isin(
+            conf.marker.getlist("classes_to_ignore")
+        )
+    ]
+
+    # get the expected columns from the classifier
+    datacolumns_path = glob.glob(
+        os.path.join(os.path.dirname(input_classifier_path), "*datacolumns.txt")
+    )[0]
+    with open(datacolumns_path, "r") as f:
+        input_classifier_datacolumns = ast.literal_eval(f.readline())
+
+    # If the classification data isn't passed as dataframe, read it from the csv
+    if input_parcel_classification_data_df is None:
+        logger.info(
+            f"Read classification data file: {input_parcel_classification_data_path}"
+        )
+        input_parcel_classification_data_df = pdh.read_file(
+            input_parcel_classification_data_path
+        )
+        if input_parcel_classification_data_df.index.name != conf.columns["id"]:
+            input_parcel_classification_data_df.set_index(
+                conf.columns["id"], inplace=True
+            )
+        logger.debug("Read classification data file ready")
+
+    # only take the required columns as expected by the classifier
+    input_parcel_classification_data_df = input_parcel_classification_data_df[
+        input_classifier_datacolumns
+    ]  # type: ignore
+
+    # Join the data to send to prediction logic
+    logger.info("Join input parcels with the classification data")
+    input_parcel_for_predict_df = input_parcel_df.join(
+        input_parcel_classification_data_df, how="inner"  # type: ignore
+    )
+
+    # Predict!
+    logger.info(f"Predict using this model: {input_classifier_path}")
+    if conf.classifier["classifier_type"].lower() == "keras_multilayer_perceptron":
+        import cropclassification.predict.classification_keras as class_core_keras
+
+        class_core_keras.predict_proba(
+            parcel_df=input_parcel_for_predict_df,
+            classifier_basepath=input_classifier_basepath,
+            classifier_path=input_classifier_path,
+            output_parcel_predictions_path=output_predictions_path,
+        )
+    else:
+        import cropclassification.predict.classification_sklearn as class_core_sklearn
+
+        class_core_sklearn.predict_proba(
+            parcel_df=input_parcel_for_predict_df,
+            classifier_basepath=input_classifier_basepath,
+            classifier_path=input_classifier_path,
+            output_parcel_predictions_path=output_predictions_path,
+        )
+
+
+# If the script is run directly...
+if __name__ == "__main__":
+    logger.critical("Not implemented exception!")
+    raise Exception("Not implemented")
```

### Comparing `cropclassification-0.1.0a2/cropclassification/predict/classification_sklearn.py` & `cropclassification-0.1.1/cropclassification/predict/classification_sklearn.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,204 +1,205 @@
-# -*- coding: utf-8 -*-
-"""
-Module that implements the classification logic.
-"""
-
-import ast
-import glob
-import logging
-import os
-from pathlib import Path
-
-import numpy as np
-import pandas as pd
-from sklearn.neural_network import MLPClassifier
-from sklearn.ensemble import RandomForestClassifier
-from sklearn.neighbors import KNeighborsClassifier
-from sklearn.externals import joblib
-from sklearn.svm import SVC
-
-import cropclassification.helpers.config_helper as conf
-import cropclassification.helpers.pandas_helper as pdh
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def train(train_df: pd.DataFrame, output_classifier_basepath: Path) -> Path:
-    """
-    Train a classifier and output the trained classifier to the output file.
-
-    Args
-        train_df: pandas DataFrame containing the train data. Columns:
-            * global_settings.id_column: the id of the parcel
-            * global_settings.class_column: the class of the parcel
-            * ... all columns that will be used as classification data
-        output_classifier_basepath: the path where the classifier can be written
-    """
-    output_classifier_path_noext, _ = os.path.splitext(output_classifier_basepath)
-    output_classifier_path = output_classifier_basepath
-    output_classifier_datacolumns_path = Path(
-        f"{output_classifier_path_noext}_datacolumns.txt"
-    )
-
-    # Split the input dataframe in one with the train classes and one with the train
-    # data
-    train_classes_df = train_df[conf.columns["class"]]
-    cols_to_keep = train_df.columns.difference(
-        [conf.columns["id"], conf.columns["class"]]
-    )
-    train_data_df = train_df[cols_to_keep]
-
-    logger.info(
-        "Train file processed and rows with missing data removed, data shape: "
-        f"{train_data_df.shape}, labels shape: {train_classes_df.shape}"
-    )
-    with pd.option_context("display.max_rows", None, "display.max_columns", None):
-        logger.info(f"Resulting Columns for training data: {train_data_df.columns}")
-    with open(output_classifier_datacolumns_path, "w") as file:
-        file.write(str(list(train_data_df.columns)))
-
-    # Using almost all defaults for the classifier seems to work best...
-    logger.info("Start training")
-    classifier_type_lower = conf.classifier["classifier_type"].lower()
-    if classifier_type_lower == "randomforest":
-        n_estimators = conf.classifier.getint("randomforest_n_estimators")
-        max_depth = conf.classifier.getint("randomforest_max_depth")
-        classifier = RandomForestClassifier(
-            n_estimators=n_estimators, max_depth=max_depth
-        )
-    elif classifier_type_lower == "nearestneighbor":
-        classifier = KNeighborsClassifier(weights="distance", n_jobs=-1)
-    elif classifier_type_lower == "multilayer_perceptron":
-        hidden_layer_sizes = tuple(
-            conf.classifier.getlistint("multilayer_perceptron_hidden_layer_sizes")
-        )
-        max_iter = conf.classifier.getint("multilayer_perceptron_max_iter")
-        learning_rate_init = conf.classifier.getfloat(
-            "multilayer_perceptron_learning_rate_init"
-        )
-        classifier = MLPClassifier(
-            max_iter=max_iter,
-            hidden_layer_sizes=hidden_layer_sizes,
-            learning_rate_init=learning_rate_init,
-        )
-    elif classifier_type_lower == "svm":
-        # cache_size=1000 (MB) should speed up training
-        # probability=True is necessary to be able to use predict_proba
-        classifier = SVC(C=64.0, gamma=0.125, probability=True, cache_size=1000)
-    else:
-        message = (
-            "Unsupported classifier in conf.classifier['classifier_type']: "
-            f"{conf.classifier['classifier_type']}"
-        )
-        logger.critical(message)
-        raise Exception(message)
-
-    logger.info(f"Start fitting classifier:\n{classifier}")
-    classifier.fit(train_data_df, train_classes_df)
-
-    # Write the learned model to a file...
-    logger.info(f"Write the learned model file to {output_classifier_path}")
-    joblib.dump(classifier, output_classifier_path)
-
-    return output_classifier_path
-
-
-def predict_proba(
-    parcel_df: pd.DataFrame,
-    classifier_basepath: Path,
-    classifier_path: Path,
-    output_parcel_predictions_path: Path,
-) -> pd.DataFrame:
-    """
-    Predict the probabilities for all input data using the classifier provided and
-    write it to the output file.
-
-    Args
-        parcel_df: pandas DataFrame containing the data to classify. Columns:
-            * global_settings.id_column: the id of the parcel.
-            * global_settings.class_column: the class of the parcel. Isn't really used.
-            * ... all columns that will be used as classification data.
-        classifier_path: the path where the classifier can be written.
-        output_parcel_predictions_path: file to write the predictions to.
-    """
-
-    # Some basic checks that input is ok
-    column_class = conf.columns["class"]
-    column_class_declared = conf.columns["class_declared"]
-    parcel_df.reset_index(inplace=True)
-    if (
-        conf.columns["id"] not in parcel_df.columns
-        or column_class not in parcel_df.columns
-    ):
-        message = (
-            f"Columns {conf.columns['id']} and {column_class} are mandatory for input "
-            "parameter parcel_df!"
-        )
-        logger.critical(message)
-        raise Exception(message)
-
-    # Now do final preparation for the classification
-    parcel_classes_df = parcel_df[conf.columns["class"]]
-    cols_to_keep = parcel_df.columns.difference(
-        [conf.columns["id"], column_class, column_class_declared]
-    )
-    parcel_data_df = parcel_df[cols_to_keep]
-
-    logger.info(
-        "Train file processed and rows with missing data removed, data shape: "
-        f"{parcel_data_df.shape}, labels shape: {parcel_classes_df.shape}"
-    )
-    with pd.option_context("display.max_rows", None, "display.max_columns", None):
-        logger.info(f"Resulting Columns for training data: {parcel_data_df.columns}")
-
-    # Check of the input data columns match the columns needed for the classifier
-    classifier_datacolumns_path = glob.glob(
-        os.path.join(os.path.dirname(classifier_path), "*_datacolumns.txt")
-    )[0]
-    with open(classifier_datacolumns_path, "r") as file:
-        classifier_datacolumns = ast.literal_eval(file.readline())
-    if classifier_datacolumns != list(parcel_data_df.columns):
-        raise Exception(
-            "Input datacolumns for predict don't match needed columns for classifier: "
-            f"\ninput: {parcel_data_df.columns}, \nneeded: {classifier_datacolumns}"
-        )
-
-    # Load the classifier
-    classifier = joblib.load(classifier_path)
-    logger.info(f"Classifier has the following columns: {classifier.classes_}")
-
-    logger.info(f"Predict classes with probabilities: {len(parcel_df.index)} rows")
-    class_proba = classifier.predict_proba(parcel_data_df)
-    logger.info(f"Predict classes with probabilities ready")
-
-    # Convert probabilities to dataframe, combine with input data and write to file
-    id_class_proba = np.concatenate(
-        [
-            parcel_df[[conf.columns["id"], column_class, column_class_declared]].values,
-            class_proba,
-        ],
-        axis=1,
-    )
-    cols = [conf.columns["id"], column_class, column_class_declared]
-    cols.extend(classifier.classes_)
-    proba_df = pd.DataFrame(id_class_proba, columns=cols)
-
-    # If output path provided, write results
-    if output_parcel_predictions_path:
-        pdh.to_file(proba_df, output_parcel_predictions_path)
-
-    return proba_df
-
-
-# If the script is run directly...
-if __name__ == "__main__":
-    logger.critical("Not implemented exception!")
-    raise Exception("Not implemented")
+# -*- coding: utf-8 -*-
+"""
+Module that implements the classification logic.
+"""
+
+import ast
+import glob
+import logging
+import os
+from pathlib import Path
+
+import numpy as np
+import pandas as pd
+from sklearn.neural_network import MLPClassifier
+from sklearn.ensemble import RandomForestClassifier
+from sklearn.neighbors import KNeighborsClassifier
+import joblib
+from sklearn.svm import SVC
+
+import cropclassification.helpers.config_helper as conf
+import cropclassification.helpers.pandas_helper as pdh
+
+# -------------------------------------------------------------
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def train(train_df: pd.DataFrame, output_classifier_basepath: Path) -> Path:
+    """
+    Train a classifier and output the trained classifier to the output file.
+
+    Args
+        train_df: pandas DataFrame containing the train data. Columns:
+            * global_settings.id_column: the id of the parcel
+            * global_settings.class_column: the class of the parcel
+            * ... all columns that will be used as classification data
+        output_classifier_basepath: the path where the classifier can be written
+    """
+    output_classifier_path_noext, _ = os.path.splitext(output_classifier_basepath)
+    output_classifier_path = output_classifier_basepath
+    output_classifier_datacolumns_path = Path(
+        f"{output_classifier_path_noext}_datacolumns.txt"
+    )
+
+    # Split the input dataframe in one with the train classes and one with the train
+    # data
+    train_classes_df = train_df[conf.columns["class"]]
+    cols_to_keep = train_df.columns.difference(
+        [conf.columns["id"], conf.columns["class"]]  # type: ignore
+    )
+    train_data_df = train_df[cols_to_keep]
+
+    logger.info(
+        "Train file processed and rows with missing data removed, data shape: "
+        f"{train_data_df.shape}, labels shape: {train_classes_df.shape}"
+    )
+    with pd.option_context(
+        "display.max_rows", None, "display.max_columns", None
+    ):  # type: ignore
+        logger.info(f"Resulting Columns for training data: {train_data_df.columns}")
+    with open(output_classifier_datacolumns_path, "w") as file:
+        file.write(str(list(train_data_df.columns)))
+
+    # Using almost all defaults for the classifier seems to work best...
+    logger.info("Start training")
+    classifier_type_lower = conf.classifier["classifier_type"].lower()
+    if classifier_type_lower == "randomforest":
+        n_estimators = conf.classifier.getint("randomforest_n_estimators")
+        max_depth = conf.classifier.getint("randomforest_max_depth")
+        classifier = RandomForestClassifier(
+            n_estimators=n_estimators, max_depth=max_depth
+        )
+    elif classifier_type_lower == "nearestneighbor":
+        classifier = KNeighborsClassifier(weights="distance", n_jobs=-1)
+    elif classifier_type_lower == "multilayer_perceptron":
+        hidden_layer_sizes = tuple(
+            conf.classifier.getlistint("multilayer_perceptron_hidden_layer_sizes")
+        )
+        max_iter = conf.classifier.getint("multilayer_perceptron_max_iter")
+        learning_rate_init = conf.classifier.getfloat(
+            "multilayer_perceptron_learning_rate_init"
+        )
+        classifier = MLPClassifier(
+            max_iter=max_iter,
+            hidden_layer_sizes=hidden_layer_sizes,
+            learning_rate_init=learning_rate_init,
+        )
+    elif classifier_type_lower == "svm":
+        # cache_size=1000 (MB) should speed up training
+        # probability=True is necessary to be able to use predict_proba
+        classifier = SVC(
+            C=64.0, gamma=0.125, probability=True, cache_size=1000  # type: ignore
+        )
+    else:
+        message = (
+            "Unsupported classifier in conf.classifier['classifier_type']: "
+            f"{conf.classifier['classifier_type']}"
+        )
+        logger.critical(message)
+        raise Exception(message)
+
+    logger.info(f"Start fitting classifier:\n{classifier}")
+    classifier.fit(train_data_df, train_classes_df)
+
+    # Write the learned model to a file...
+    logger.info(f"Write the learned model file to {output_classifier_path}")
+    joblib.dump(classifier, output_classifier_path)
+
+    return output_classifier_path
+
+
+def predict_proba(
+    parcel_df: pd.DataFrame,
+    classifier_basepath: Path,
+    classifier_path: Path,
+    output_parcel_predictions_path: Path,
+) -> pd.DataFrame:
+    """
+    Predict the probabilities for all input data using the classifier provided and
+    write it to the output file.
+
+    Args
+        parcel_df: pandas DataFrame containing the data to classify. Columns:
+            * global_settings.id_column: the id of the parcel.
+            * global_settings.class_column: the class of the parcel. Isn't really used.
+            * ... all columns that will be used as classification data.
+        classifier_path: the path where the classifier can be written.
+        output_parcel_predictions_path: file to write the predictions to.
+    """
+
+    # Some basic checks that input is ok
+    column_class = conf.columns["class"]
+    column_class_declared = conf.columns["class_declared"]
+    parcel_df.reset_index(inplace=True)
+    if (
+        conf.columns["id"] not in parcel_df.columns
+        or column_class not in parcel_df.columns
+    ):
+        message = (
+            f"Columns {conf.columns['id']} and {column_class} are mandatory for input "
+            "parameter parcel_df!"
+        )
+        logger.critical(message)
+        raise Exception(message)
+
+    # Now do final preparation for the classification
+    parcel_classes_df = parcel_df[conf.columns["class"]]
+    cols_to_keep = parcel_df.columns.difference(
+        [conf.columns["id"], column_class, column_class_declared]  # type: ignore
+    )
+    parcel_data_df = parcel_df[cols_to_keep]
+
+    logger.info(
+        "Train file processed and rows with missing data removed, data shape: "
+        f"{parcel_data_df.shape}, labels shape: {parcel_classes_df.shape}"
+    )
+    with pd.option_context(
+        "display.max_rows", None, "display.max_columns", None
+    ):  # type: ignore
+        logger.info(f"Resulting Columns for training data: {parcel_data_df.columns}")
+
+    # Check of the input data columns match the columns needed for the classifier
+    classifier_datacolumns_path = glob.glob(
+        os.path.join(os.path.dirname(classifier_path), "*_datacolumns.txt")
+    )[0]
+    with open(classifier_datacolumns_path, "r") as file:
+        classifier_datacolumns = ast.literal_eval(file.readline())
+    if classifier_datacolumns != list(parcel_data_df.columns):
+        raise Exception(
+            "Input datacolumns for predict don't match needed columns for classifier: "
+            f"\ninput: {parcel_data_df.columns}, \nneeded: {classifier_datacolumns}"
+        )
+
+    # Load the classifier
+    classifier = joblib.load(classifier_path)
+    logger.info(f"Classifier has the following columns: {classifier.classes_}")
+
+    logger.info(f"Predict classes with probabilities: {len(parcel_df.index)} rows")
+    class_proba = classifier.predict_proba(parcel_data_df)
+    logger.info("Predict classes with probabilities ready")
+
+    # Convert probabilities to dataframe, combine with input data and write to file
+    id_class_proba = np.concatenate(
+        [
+            parcel_df[[conf.columns["id"], column_class, column_class_declared]].values,
+            class_proba,
+        ],
+        axis=1,
+    )
+    cols = [conf.columns["id"], column_class, column_class_declared]
+    cols.extend(classifier.classes_)
+    proba_df = pd.DataFrame(id_class_proba, columns=cols)
+    proba_df = proba_df.set_index(keys=conf.columns["id"])
+
+    # If output path provided, write results
+    if output_parcel_predictions_path:
+        pdh.to_file(proba_df, output_parcel_predictions_path)
+
+    return proba_df
```

### Comparing `cropclassification-0.1.0a2/cropclassification/predict/multicrop.py` & `cropclassification-0.1.1/cropclassification/predict/multicrop.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,89 @@
-# -*- coding: utf-8 -*-
-"""
-Multicrop marker.
-"""
-
-import logging
-from pathlib import Path
-
-import pandas as pd
-
-import cropclassification.helpers.config_helper as conf
-import cropclassification.helpers.pandas_helper as pdh
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def detect_multicrop(input_parcel_path: Path, input_parcel_timeseries_data_path: Path):
-
-    """
-    logger.info(f"Read input file: {input_parcel_path}")
-    df_input_parcel = pd.read_csv(input_parcel_path, low_memory=False)
-    logger.debug('Read train file ready')
-    """
-
-    # If the classification data isn't passed as dataframe, read it from the csv
-    logger.info(f"Read classification data file: {input_parcel_timeseries_data_path}")
-    df_timeseries_data = pd.read_csv(
-        input_parcel_timeseries_data_path, low_memory=False
-    )
-    df_timeseries_data.set_index(conf.columns["id"], inplace=True)
-    logger.debug("Read classification data file ready")
-
-    # Add column with the max of all columns (= all stdDev's)
-    df_timeseries_data["max_stddev"] = df_timeseries_data.max(axis=1)
-
-    """
-    # Prepare the data to send to prediction logic...
-    logger.info("Join train sample with the classification data")
-    df_input_parcel_for_detect = (df_input_parcel#[[gs.id_column, gs.class_column]]
-                                   .join(df_timeseries_data
-                                         , how='inner', on=gs.id_column))
-
-    # Only keep the parcels with relevant crops/production types
-    productiontype_column = 'GESP_PM'
-    if productiontype_column in df_input_parcel_for_detect.columns:
-        # Serres, tijdelijke overkappingen en loodsen
-        df_input_parcel_for_detect.loc[~df_input_parcel_for_detect[productiontype_column].isin(['SER', 'SGM'])]
-        df_input_parcel_for_detect.loc[~df_input_parcel_for_detect[productiontype_column].isin(['PLA', 'PLO', 'NPO'])]
-        df_input_parcel_for_detect.loc[df_input_parcel_for_detect[productiontype_column] != 'LOO']     # Een loods is hetzelfde als een stal...
-        df_input_parcel_for_detect.loc[df_input_parcel_for_detect[productiontype_column] != 'CON']    # Containers, niet op volle grond...
-
-    crop_columnname = 'GWSCOD_H'
-    df_input_parcel_for_detect.loc[~df_input_parcel_for_detect[crop_columnname].isin(['1', '2', '3'])]
-
-    # Keep the parcels with the 1000 largest stdDev
-    df_largest = df_input_parcel_for_detect.nlargest(1000, columns='max_stddev', keep='first')
-    """
-
-    # df_result = df_timeseries_data['max_stddev'].to_frame()
-    df_result = df_timeseries_data
-    logger.info(df_result)
-
-    # Write to file
-    output_path = Path(str(input_parcel_timeseries_data_path) + "_largestStdDev.csv")
-    logger.info(f"Write output file: {output_path}")
-    pdh.to_file(df_result, output_path)
+# -*- coding: utf-8 -*-
+"""
+Multicrop marker.
+"""
+
+import logging
+from pathlib import Path
+
+import pandas as pd
+
+import cropclassification.helpers.config_helper as conf
+import cropclassification.helpers.pandas_helper as pdh
+
+# -------------------------------------------------------------
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def detect_multicrop(input_parcel_path: Path, input_parcel_timeseries_data_path: Path):
+    """
+    logger.info(f"Read input file: {input_parcel_path}")
+    df_input_parcel = pd.read_csv(input_parcel_path, low_memory=False)
+    logger.debug('Read train file ready')
+    """
+
+    # If the classification data isn't passed as dataframe, read it from the csv
+    logger.info(f"Read classification data file: {input_parcel_timeseries_data_path}")
+    df_timeseries_data = pd.read_csv(
+        input_parcel_timeseries_data_path, low_memory=False
+    )
+    df_timeseries_data.set_index(conf.columns["id"], inplace=True)
+    logger.debug("Read classification data file ready")
+
+    # Add column with the max of all columns (= all stdDev's)
+    df_timeseries_data["max_stddev"] = df_timeseries_data.max(axis=1)
+
+    """
+    # Prepare the data to send to prediction logic...
+    logger.info("Join train sample with the classification data")
+    df_input_parcel_for_detect = (
+        df_input_parcel.join(  # [[gs.id_column, gs.class_column]]
+            df_timeseries_data, how="inner", on=gs.id_column
+        )
+    )
+
+    # Only keep the parcels with relevant crops/production types
+    productiontype_column = "GESP_PM"
+    if productiontype_column in df_input_parcel_for_detect.columns:
+        # Serres, tijdelijke overkappingen en loodsen
+        df_input_parcel_for_detect.loc[
+            ~df_input_parcel_for_detect[productiontype_column].isin(["SER", "SGM"])
+        ]
+        df_input_parcel_for_detect.loc[
+            ~df_input_parcel_for_detect[productiontype_column].isin(
+                ["PLA", "PLO", "NPO"]
+            )
+        ]
+        df_input_parcel_for_detect.loc[
+            df_input_parcel_for_detect[productiontype_column] != "LOO"
+        ]  # Een loods is hetzelfde als een stal...
+        df_input_parcel_for_detect.loc[
+            df_input_parcel_for_detect[productiontype_column] != "CON"
+        ]  # Containers, niet op volle grond...
+
+    crop_columnname = "GWSCOD_H"
+    df_input_parcel_for_detect.loc[
+        ~df_input_parcel_for_detect[crop_columnname].isin(["1", "2", "3"])
+    ]
+
+    # Keep the parcels with the 1000 largest stdDev
+    df_largest = df_input_parcel_for_detect.nlargest(
+        1000, columns="max_stddev", keep="first"
+    )
+    """
+
+    # df_result = df_timeseries_data['max_stddev'].to_frame()
+    df_result = df_timeseries_data
+    logger.info(df_result)
+
+    # Write to file
+    output_path = Path(str(input_parcel_timeseries_data_path) + "_largestStdDev.csv")
+    logger.info(f"Write output file: {output_path}")
+    pdh.to_file(df_result, output_path)
```

### Comparing `cropclassification-0.1.0a2/cropclassification/preprocess/classification_preprocess.py` & `cropclassification-0.1.1/cropclassification/preprocess/classification_preprocess.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,492 +1,549 @@
-# -*- coding: utf-8 -*-
-"""
-Module with helper functions to preprocess the data to use for the classification.
-"""
-
-import logging
-import os
-from pathlib import Path
-import shutil
-
-import pandas as pd
-
-import cropclassification.preprocess.classification_preprocess_BEFL as befl
-import cropclassification.helpers.config_helper as conf
-import cropclassification.helpers.pandas_helper as pdh
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-
-# Get a logger...
-logger = logging.getLogger(__name__)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def prepare_input(
-    input_parcel_path: Path,
-    input_parcel_filetype: str,
-    input_parcel_pixcount_path: Path,
-    classtype_to_prepare: str,
-    classes_refe_path: Path,
-    output_parcel_path: Path,
-    force: bool = False,
-):
-    """
-    Prepare a raw input file by eg. adding the classification classes to use for the
-    classification,...
-    """
-
-    # If force == False Check and the output file exists already, stop.
-    if force is False and os.path.exists(output_parcel_path) is True:
-        logger.warning(
-            f"prepare_input: output file exists + force is False: {output_parcel_path}"
-        )
-        return
-
-    # If it exists, copy the refe file to the run dir, so we always keep knowing which
-    # refe was used
-    if classes_refe_path is not None:
-        shutil.copy(classes_refe_path, output_parcel_path.parent)
-
-    if input_parcel_filetype == "BEFL":
-        # classes_refe_path must exist for BEFL!
-        if not classes_refe_path.exists():
-            raise Exception(f"Input classes file doesn't exist: {classes_refe_path}")
-
-        df_parceldata = befl.prepare_input(
-            input_parcel_path=input_parcel_path,
-            classtype_to_prepare=classtype_to_prepare,
-            classes_refe_path=classes_refe_path,
-            output_dir=output_parcel_path.parent,
-        )
-    else:
-        message = f"Unknown value for input_parcel_filetype: {input_parcel_filetype}"
-        logger.critical(message)
-        raise Exception(message)
-
-    # Load pixcount data and join it
-    logger.info(f"Read pixcount file {input_parcel_pixcount_path}")
-    df_pixcount = pdh.read_file(input_parcel_pixcount_path)
-    logger.debug(f"Read pixcount file ready, shape: {df_pixcount.shape}")
-    if df_pixcount.index.name != conf.columns["id"]:
-        df_pixcount.set_index(conf.columns["id"], inplace=True)
-
-    df_parceldata.set_index(conf.columns["id"], inplace=True)
-    df_parceldata = df_parceldata.join(
-        df_pixcount[conf.columns["pixcount_s1s2"]], how="left"
-    )
-    df_parceldata[conf.columns["pixcount_s1s2"]].fillna(value=0, inplace=True)
-
-    # Export result to file
-    output_ext = os.path.splitext(output_parcel_path)[1]
-    for column in df_parceldata.columns:
-        # if the output asked is a csv... we don't need the geometry...
-        if column == conf.columns["geom"] and output_ext == ".csv":
-            df_parceldata.drop(column, axis=1, inplace=True)
-
-    logger.info(f"Write output to {output_parcel_path}")
-    # If extension is not .shp, write using pandas (=a lot faster!)
-    if output_ext.lower() != ".shp":
-        pdh.to_file(df_parceldata, output_parcel_path)
-    else:
-        df_parceldata.to_file(output_parcel_path, index=False)
-
-
-def create_train_test_sample(
-    input_parcel_path: Path,
-    output_parcel_train_path: Path,
-    output_parcel_test_path: Path,
-    balancing_strategy: str,
-    force: bool = False,
-):
-    """Create a seperate train and test sample from the general input file."""
-
-    # If force == False Check and the output files exist already, stop.
-    if (
-        force is False
-        and output_parcel_train_path.exists() is True
-        and output_parcel_test_path.exists() is True
-    ):
-        logger.warning(
-            "create_train_test_sample: output files already exist and force is False: "
-            f"{output_parcel_train_path}, {output_parcel_test_path}"
-        )
-        return
-
-    # Load input data...
-    logger.info(
-        f"Start create_train_test_sample with balancing_strategy {balancing_strategy}"
-    )
-    logger.info(f"Read input file {input_parcel_path}")
-    df_in = pdh.read_file(input_parcel_path)
-    logger.debug(f"Read input file ready, shape: {df_in.shape}")
-
-    # Init some many-used variables from config
-    class_balancing_column = conf.columns["class_balancing"]
-    class_column = conf.columns["class"]
-
-    with pd.option_context(
-        "display.max_rows", None, "display.max_columns", None
-    ):  # type: ignore
-        count_per_class = df_in.groupby(class_balancing_column, as_index=False).size()
-        logger.info(
-            f"Number of elements per classname in input dataset:\n{count_per_class}"
-        )
-
-    # The test dataset should be as representative as possible for the entire dataset,
-    # so create this first as a 20% sample of each class without any additional checks.
-    # Remark: group_keys=False evades that apply creates an extra index-level of the
-    #     groups above the data and evades having to do
-    #     .reset_index(level=class_balancing_column_NAME, drop=True)
-    #     to get rid of the group level
-    test_df = df_in.groupby(class_balancing_column, group_keys=False).apply(
-        pd.DataFrame.sample, frac=0.20
-    )
-    logger.debug(
-        f"df_test after sampling 20% of data per class, shape: {test_df.shape}"
-    )
-
-    # The candidate parcel for training are all non-test parcel
-    train_base_df = df_in[~df_in.index.isin(test_df.index)]
-    logger.debug(f"df_train_base after isin\n{train_base_df}")
-
-    # Remove parcel with too few pixels from the train sample
-    min_pixcount = conf.marker.getfloat("min_nb_pixels_train")
-    train_base_df = train_base_df[
-        train_base_df[conf.columns["pixcount_s1s2"]] >= min_pixcount
-    ]
-    logger.debug(
-        "Number of parcels in df_train_base after filter on pixcount >= "
-        f"{min_pixcount}: {len(train_base_df)}"
-    )
-
-    # Some classes shouldn't be used for training... so remove them!
-    logger.info(
-        "Remove 'classes_to_ignore_for_train' from train sample (= where "
-        f"{class_column} is in: {conf.marker.getlist('classes_to_ignore_for_train')}"
-    )
-    train_base_df = train_base_df[
-        ~train_base_df[class_column].isin(
-            conf.marker.getlist("classes_to_ignore_for_train")
-        )
-    ]
-
-    # All classes_to_ignore aren't meant for training either...
-    logger.info(
-        f"Remove 'classes_to_ignore' from train sample (= where {class_column} is in: "
-        f"{conf.marker.getlist('classes_to_ignore')}"
-    )
-    train_base_df = train_base_df[
-        ~train_base_df[class_column].isin(conf.marker.getlist("classes_to_ignore"))
-    ]
-
-    # Print the train base result before applying any balancing
-    with pd.option_context(
-        "display.max_rows", None, "display.max_columns", None
-    ):  # type: ignore
-        count_per_class = train_base_df.groupby(
-            class_balancing_column, as_index=False
-        ).size()
-        logger.info(
-            "Number of elements per classname for train dataset, before balancing:\n"
-            f"{count_per_class}"
-        )
-
-    # Depending on the balancing_strategy, use different way to get a training sample
-    if balancing_strategy == "BALANCING_STRATEGY_NONE":
-        # Just use 25% of all non-test data as train data -> 25% of 80% of data -> 20%
-        # of all data will be training date
-        # Remark: - this is very unbalanced, eg. classes with 10.000 times the input
-        #           size than other classes
-        #         - this results in a relatively high accuracy in overall numbers, but
-        #           the small classes are not detected at all
-        train_df = train_base_df.groupby(
-            class_balancing_column, group_keys=False
-        ).apply(pd.DataFrame.sample, frac=0.25)
-
-    elif balancing_strategy == "BALANCING_STRATEGY_MEDIUM":
-        # Balance the train data, but still use some larger samples for the classes
-        # that have a lot of members in the input dataset
-        # Remark: with the upper limit of 10.000 this gives still OK results overall,
-        #     and also the smaller classes give some results with upper limit of 4000
-        #     results significantly less good.
-
-        # For the larger classes, favor them by leaving the samples larger but cap at
-        # upper_limit
-        upper_limit = 10000
-        lower_limit = 1000
-        logger.info(
-            f"Cap over {upper_limit}, keep the full number of training sample till "
-            f"{lower_limit}, samples smaller than that are oversampled"
-        )
-        train_df = (
-            train_base_df.groupby(class_balancing_column)
-            .filter(lambda x: len(x) >= upper_limit)
-            .groupby(class_balancing_column, group_keys=False)
-            .apply(pd.DataFrame.sample, upper_limit)
-        )
-        # Middle classes use the number as they are
-        train_df = train_df.append(
-            train_base_df.groupby(class_balancing_column)
-            .filter(lambda x: len(x) < upper_limit)
-            .groupby(class_balancing_column)
-            .filter(lambda x: len(x) >= lower_limit)
-        )
-        # For smaller classes, oversample...
-        train_df = train_df.append(
-            train_base_df.groupby(class_balancing_column)
-            .filter(lambda x: len(x) < lower_limit)
-            .groupby(class_balancing_column, group_keys=False)
-            .apply(pd.DataFrame.sample, lower_limit, replace=True)
-        )
-
-    elif balancing_strategy == "BALANCING_STRATEGY_MEDIUM2":
-        # Balance the train data, but still use some larger samples for the classes
-        # that have a lot of members in the input dataset
-        # Remark: with the upper limit of 10.000 this gives still OK results overall,
-        #     and also the smaller classes give some results with upper limit of 4000
-        #     results significantly less good.
-
-        # For the larger classes, leave the samples larger but cap
-        cap_count_limit1 = 100000
-        cap_train_limit1 = 30000
-        logger.info(
-            f"Cap balancing classes over {cap_count_limit1} to {cap_train_limit1}"
-        )
-        train_df = (
-            train_base_df.groupby(class_balancing_column)
-            .filter(lambda x: len(x) >= cap_count_limit1)
-            .groupby(class_balancing_column, group_keys=False)
-            .apply(pd.DataFrame.sample, cap_train_limit1)
-        )
-        cap_count_limit2 = 50000
-        cap_train_limit2 = 20000
-        logger.info(
-            f"Cap balancing classes between {cap_count_limit2} and {cap_count_limit1} "
-            f"to {cap_train_limit2}"
-        )
-        train_cap2_df = (
-            train_base_df.groupby(class_balancing_column)
-            .filter(lambda x: len(x) < cap_count_limit1)
-            .groupby(class_balancing_column)
-            .filter(lambda x: len(x) >= cap_count_limit2)
-            .groupby(class_balancing_column, group_keys=False)
-        )
-        if len(train_cap2_df) > 0:
-            train_df = train_df.append(
-                train_cap2_df.apply(pd.DataFrame.sample, cap_train_limit2)
-            )
-        cap_count_limit3 = 20000
-        cap_train_limit3 = 10000
-        logger.info(
-            f"Cap balancing classes between {cap_count_limit3} and {cap_count_limit2} "
-            f"to {cap_train_limit3}"
-        )
-        train_df = train_df.append(
-            train_base_df.groupby(class_balancing_column)
-            .filter(lambda x: len(x) < cap_count_limit2)
-            .groupby(class_balancing_column)
-            .filter(lambda x: len(x) >= cap_count_limit3)
-            .groupby(class_balancing_column, group_keys=False)
-            .apply(pd.DataFrame.sample, cap_train_limit3)
-        )
-        cap_count_limit4 = 10000
-        cap_train_limit4 = 10000
-        logger.info(
-            f"Cap balancing classes between {cap_count_limit4} and {cap_count_limit3} "
-            f"to {cap_train_limit4}"
-        )
-        train_df = train_df.append(
-            train_base_df.groupby(class_balancing_column)
-            .filter(lambda x: len(x) < cap_count_limit3)
-            .groupby(class_balancing_column)
-            .filter(lambda x: len(x) >= cap_count_limit4)
-            .groupby(class_balancing_column, group_keys=False)
-            .apply(pd.DataFrame.sample, cap_train_limit4)
-        )
-        oversample_count = 1000
-        # Middle classes use the number as they are
-        logger.info(
-            f"For classes between {cap_count_limit4} and {oversample_count}, just use "
-            "all samples"
-        )
-        train_df = train_df.append(
-            train_base_df.groupby(class_balancing_column)
-            .filter(lambda x: len(x) < cap_count_limit4)
-            .groupby(class_balancing_column)
-            .filter(lambda x: len(x) >= oversample_count)
-        )
-        # For smaller classes, oversample...
-        logger.info(
-            f"For classes smaller than {oversample_count}, oversample to "
-            f"{oversample_count}"
-        )
-        train_df = train_df.append(
-            train_base_df.groupby(class_balancing_column)
-            .filter(lambda x: len(x) < oversample_count)
-            .groupby(class_balancing_column, group_keys=False)
-            .apply(pd.DataFrame.sample, oversample_count, replace=True)
-        )
-
-    elif balancing_strategy == "BALANCING_STRATEGY_PROPORTIONAL_GROUPS":
-        # Balance the train data, but still use some larger samples for the classes
-        # that have a lot of members in the input dataset
-        # Remark: with the upper limit of 10.000 this gives still OK results overall,
-        #     and also the smaller classes give some results with upper limit of 4000
-        #     results significantly less good.
-
-        # For the larger classes, leave the samples larger but cap
-        upper_count_limit1 = 100000
-        upper_train_limit1 = 30000
-        logger.info(
-            f"Cap balancing classes over {upper_count_limit1} to {upper_train_limit1}"
-        )
-        train_df = (
-            train_base_df.groupby(class_balancing_column)
-            .filter(lambda x: len(x) >= upper_count_limit1)
-            .groupby(class_balancing_column, group_keys=False)
-            .apply(pd.DataFrame.sample, upper_train_limit1)
-        )
-        upper_count_limit2 = 50000
-        upper_train_limit2 = 20000
-        logger.info(
-            f"Cap balancing classes between {upper_count_limit2} and "
-            f"{upper_count_limit1} to {upper_train_limit2}"
-        )
-        train_limit2_df = (
-            train_base_df.groupby(class_balancing_column)
-            .filter(lambda x: len(x) < upper_count_limit1)
-            .groupby(class_balancing_column)
-            .filter(lambda x: len(x) >= upper_count_limit2)
-            .groupby(class_balancing_column, group_keys=False)
-        )
-        if len(train_limit2_df) > 0:
-            train_df = train_df.append(
-                train_limit2_df.apply(pd.DataFrame.sample, upper_train_limit2)
-        )
-        upper_count_limit3 = 20000
-        upper_train_limit3 = 10000
-        logger.info(
-            f"Cap balancing classes between {upper_count_limit3} and "
-            f"{upper_count_limit2} to {upper_train_limit3}"
-        )
-        train_limit3_df = (
-            train_base_df.groupby(class_balancing_column)
-            .filter(lambda x: len(x) < upper_count_limit2)
-            .groupby(class_balancing_column)
-            .filter(lambda x: len(x) >= upper_count_limit3)
-            .groupby(class_balancing_column, group_keys=False)
-        )
-        if len(train_limit3_df) > 0:
-            train_df = train_df.append(
-                train_limit3_df.apply(pd.DataFrame.sample, upper_train_limit3)
-            )
-        upper_count_limit4 = 10000
-        upper_train_limit4 = 5000
-        logger.info(
-            f"Cap balancing classes between {upper_count_limit4} and "
-            f"{upper_count_limit3} to {upper_train_limit4}"
-        )
-        train_limit4_df = (
-            train_base_df.groupby(class_balancing_column)
-            .filter(lambda x: len(x) < upper_count_limit3)
-            .groupby(class_balancing_column)
-            .filter(lambda x: len(x) >= upper_count_limit4)
-            .groupby(class_balancing_column, group_keys=False)
-        )
-        if len(train_limit4_df) > 0:
-            train_df = train_df.append(
-                train_limit4_df.apply(pd.DataFrame.sample, upper_train_limit4)
-            )
-        # For smaller balancing classes, just use all samples
-        train_df = train_df.append(
-            train_base_df.groupby(class_balancing_column).filter(
-                lambda x: len(x) < upper_count_limit4
-            )
-        )
-
-    elif balancing_strategy == "BALANCING_STRATEGY_UPPER_LIMIT":
-        # Balance the train data, but still use some larger samples for the classes
-        # that have a lot of members in the input dataset
-        # Remark: with the upper limit of 10.000 this gives still OK results overall,
-        #     and also the smaller classes give some results with upper limit of 4000
-        #     results significantly less good.
-
-        # For the larger classes, favor them by leaving the samples larger but cap at
-        # upper_limit
-        upper_limit = 10000
-        logger.info(f"Cap over {upper_limit}...")
-        train_df = (
-            train_base_df.groupby(class_balancing_column)
-            .filter(lambda x: len(x) >= upper_limit)
-            .groupby(class_balancing_column, group_keys=False)
-            .apply(pd.DataFrame.sample, upper_limit)
-        )
-        # For smaller classes, just use all samples
-        train_df = train_df.append(
-            train_base_df.groupby(class_balancing_column).filter(
-                lambda x: len(x) < upper_limit
-            )
-        )
-
-    elif balancing_strategy == "BALANCING_STRATEGY_EQUAL":
-        # In theory the most logical way to balance: make sure all classes have the
-        # same amount of training data by undersampling the largest classes and
-        # oversampling the small classes.
-        train_df = train_base_df.groupby(
-            class_balancing_column, group_keys=False
-        ).apply(pd.DataFrame.sample, 2000, replace=True)
-
-    else:
-        raise Exception(f"Unknown balancing strategy, STOP!: {balancing_strategy}")
-
-    # Log the resulting numbers per class in the train sample
-    with pd.option_context(
-        "display.max_rows", None, "display.max_columns", None
-    ):  # type: ignore
-        count_per_class = train_df.groupby(
-            class_balancing_column, as_index=False
-        ).size()
-        logger.info(
-            "Number of elements per class_balancing_column in train dataset:\n"
-            f"{count_per_class}"
-        )
-        if class_balancing_column != class_column:
-            count_per_class = train_df.groupby(class_column, as_index=False).size()
-            logger.info(
-                "Number of elements per class_column in train dataset:\n"
-                f"{count_per_class}"
-            )
-
-    # Log the resulting numbers per class in the test sample
-    with pd.option_context(
-        "display.max_rows", None, "display.max_columns", None
-    ):  # type: ignore
-        count_per_class = test_df.groupby(class_balancing_column, as_index=False).size()
-        logger.info(
-            "Number of elements per class_balancing_column in test dataset:\n"
-            f"{count_per_class}"
-        )
-        if class_balancing_column != class_column:
-            count_per_class = test_df.groupby(class_column, as_index=False).size()
-            logger.info(
-                "Number of elements per class_column in test dataset:\n"
-                f"{count_per_class}"
-            )
-
-    # Write to output files
-    logger.info("Write the output files")
-    train_df.set_index(conf.columns["id"], inplace=True)
-    test_df.set_index(conf.columns["id"], inplace=True)
-    pdh.to_file(train_df, output_parcel_train_path)  # The ID column is the index...
-    pdh.to_file(test_df, output_parcel_test_path)  # The ID column is the index...
-
-
-# If the script is run directly...
-if __name__ == "__main__":
-    logger.critical("Not implemented exception!")
-    raise Exception("Not implemented")
+# -*- coding: utf-8 -*-
+"""
+Module with helper functions to preprocess the data to use for the classification.
+"""
+
+import logging
+import os
+from pathlib import Path
+import shutil
+
+import pandas as pd
+
+import cropclassification.preprocess._classification_preprocess_BEFL as befl
+import cropclassification.helpers.config_helper as conf
+import cropclassification.helpers.pandas_helper as pdh
+
+# -------------------------------------------------------------
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+
+# Get a logger...
+logger = logging.getLogger(__name__)
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def prepare_input(
+    input_parcel_path: Path,
+    input_parcel_filetype: str,
+    timeseries_periodic_dir: Path,
+    base_filename: str,
+    data_ext: str,
+    classtype_to_prepare: str,
+    classes_refe_path: Path,
+    output_parcel_path: Path,
+    force: bool = False,
+):
+    """
+    Prepare a raw input file by eg. adding the classification classes to use for the
+    classification,...
+    """
+
+    # If force == False Check and the output file exists already, stop.
+    if not force and output_parcel_path.exists():
+        logger.warning(
+            f"prepare_input: output file exists + force is False: {output_parcel_path}"
+        )
+        return
+
+    # If it exists, copy the refe file to the run dir, so we always keep knowing which
+    # refe was used
+    if classes_refe_path is not None:
+        shutil.copy(classes_refe_path, output_parcel_path.parent)
+
+    if input_parcel_filetype == "BEFL":
+        # classes_refe_path must exist for BEFL!
+        if not classes_refe_path.exists():
+            raise Exception(f"Input classes file doesn't exist: {classes_refe_path}")
+
+        df_parceldata = befl.prepare_input(
+            input_parcel_path=input_parcel_path,
+            classtype_to_prepare=classtype_to_prepare,
+            classes_refe_path=classes_refe_path,
+            output_dir=output_parcel_path.parent,
+        )
+    else:
+        message = f"Unknown value for input_parcel_filetype: {input_parcel_filetype}"
+        logger.critical(message)
+        raise Exception(message)
+
+    # Load pixcount data and join it
+    parcel_pixcount_path = (
+        timeseries_periodic_dir / f"{base_filename}_pixcount{data_ext}"
+    )
+    if parcel_pixcount_path.exists():
+        logger.info(f"Read pixcount file {parcel_pixcount_path}")
+        df_pixcount = pdh.read_file(parcel_pixcount_path)
+        logger.debug(f"Read pixcount file ready, shape: {df_pixcount.shape}")
+    else:
+        parcel_pixcount_path = next(timeseries_periodic_dir.glob("*s2*.sqlite"))
+        df_pixcount = pdh.read_file(parcel_pixcount_path)
+        df_pixcount = df_pixcount[[conf.columns["id"], "count"]].rename(
+            columns={"count": conf.columns["pixcount_s1s2"]}
+        )
+
+    if df_pixcount.index.name != conf.columns["id"]:
+        df_pixcount.set_index(conf.columns["id"], inplace=True)
+
+    df_parceldata.set_index(conf.columns["id"], inplace=True)
+    df_parceldata = df_parceldata.join(
+        df_pixcount[conf.columns["pixcount_s1s2"]], how="left"
+    )
+    df_parceldata[conf.columns["pixcount_s1s2"]].fillna(value=0, inplace=True)
+
+    # Export result to file
+    output_ext = os.path.splitext(output_parcel_path)[1]
+    for column in df_parceldata.columns:
+        # if the output asked is a csv... we don't need the geometry...
+        if column == conf.columns["geom"] and output_ext == ".csv":
+            df_parceldata.drop(column, axis=1, inplace=True)
+
+    logger.info(f"Write output to {output_parcel_path}")
+    # If extension is not .shp, write using pandas (=a lot faster!)
+    if output_ext.lower() != ".shp":
+        pdh.to_file(df_parceldata, output_parcel_path)
+    else:
+        df_parceldata.to_file(output_parcel_path, index=False)
+
+
+def create_train_test_sample(
+    input_parcel_path: Path,
+    output_parcel_train_path: Path,
+    output_parcel_test_path: Path,
+    balancing_strategy: str,
+    force: bool = False,
+):
+    """Create a seperate train and test sample from the general input file."""
+
+    # If force == False Check and the output files exist already, stop.
+    if (
+        force is False
+        and output_parcel_train_path.exists() is True
+        and output_parcel_test_path.exists() is True
+    ):
+        logger.warning(
+            "create_train_test_sample: output files already exist and force is False: "
+            f"{output_parcel_train_path}, {output_parcel_test_path}"
+        )
+        return
+
+    # Load input data...
+    logger.info(
+        f"Start create_train_test_sample with balancing_strategy {balancing_strategy}"
+    )
+    logger.info(f"Read input file {input_parcel_path}")
+    df_in = pdh.read_file(input_parcel_path)
+    logger.debug(f"Read input file ready, shape: {df_in.shape}")
+
+    # Init some many-used variables from config
+    class_balancing_column = conf.columns["class_balancing"]
+    class_column = conf.columns["class"]
+
+    with pd.option_context(
+        "display.max_rows", None, "display.max_columns", None
+    ):  # type: ignore
+        count_per_class = df_in.groupby(class_balancing_column, as_index=False).size()
+        logger.info(
+            f"Number of elements per classname in input dataset:\n{count_per_class}"
+        )
+
+    # The test dataset should be as representative as possible for the entire dataset,
+    # so create this first as a 20% sample of each class without any additional checks.
+    # Remark: group_keys=False evades that apply creates an extra index-level of the
+    #     groups above the data and evades having to do
+    #     .reset_index(level=class_balancing_column_NAME, drop=True)
+    #     to get rid of the group level
+    test_df = df_in.groupby(class_balancing_column, group_keys=False).apply(
+        pd.DataFrame.sample, frac=0.20
+    )
+    logger.debug(
+        f"df_test after sampling 20% of data per class, shape: {test_df.shape}"
+    )
+
+    # The candidate parcel for training are all non-test parcel
+    train_base_df = df_in[~df_in.index.isin(test_df.index)]
+    logger.debug(f"df_train_base after isin\n{train_base_df}")
+
+    # Remove parcel with too few pixels from the train sample
+    min_pixcount = conf.marker.getfloat("min_nb_pixels_train")
+    train_base_df = train_base_df[
+        train_base_df[conf.columns["pixcount_s1s2"]] >= min_pixcount
+    ]
+    logger.debug(
+        "Number of parcels in df_train_base after filter on pixcount >= "
+        f"{min_pixcount}: {len(train_base_df)}"
+    )
+
+    # Some classes shouldn't be used for training... so remove them!
+    logger.info(
+        "Remove 'classes_to_ignore_for_train' from train sample (= where "
+        f"{class_column} is in: {conf.marker.getlist('classes_to_ignore_for_train')}"
+    )
+    train_base_df = train_base_df[
+        ~train_base_df[class_column].isin(
+            conf.marker.getlist("classes_to_ignore_for_train")
+        )
+    ]
+
+    # All classes_to_ignore aren't meant for training either...
+    logger.info(
+        f"Remove 'classes_to_ignore' from train sample (= where {class_column} is in: "
+        f"{conf.marker.getlist('classes_to_ignore')}"
+    )
+    train_base_df = train_base_df[
+        ~train_base_df[class_column].isin(conf.marker.getlist("classes_to_ignore"))
+    ]
+
+    # Print the train base result before applying any balancing
+    with pd.option_context(
+        "display.max_rows", None, "display.max_columns", None
+    ):  # type: ignore
+        count_per_class = train_base_df.groupby(
+            class_balancing_column, as_index=False
+        ).size()
+        logger.info(
+            "Number of elements per classname for train dataset, before balancing:\n"
+            f"{count_per_class}"
+        )
+
+    # Depending on the balancing_strategy, use different way to get a training sample
+    train_df = pd.DataFrame().reindex_like(train_base_df)
+    if balancing_strategy == "BALANCING_STRATEGY_NONE":
+        # Just use 25% of all non-test data as train data -> 25% of 80% of data -> 20%
+        # of all data will be training date
+        # Remark: - this is very unbalanced, eg. classes with 10.000 times the input
+        #           size than other classes
+        #         - this results in a relatively high accuracy in overall numbers, but
+        #           the small classes are not detected at all
+        train_df = train_base_df.groupby(
+            class_balancing_column, group_keys=False
+        ).apply(pd.DataFrame.sample, frac=0.25)
+
+    elif balancing_strategy == "BALANCING_STRATEGY_MEDIUM":
+        # Balance the train data, but still use some larger samples for the classes
+        # that have a lot of members in the input dataset
+        # Remark: with the upper limit of 10.000 this gives still OK results overall,
+        #     and also the smaller classes give some results with upper limit of 4000
+        #     results significantly less good.
+
+        # For the larger classes, favor them by leaving the samples larger but cap at
+        # upper_limit
+        upper_limit = 10000
+        lower_limit = 1000
+        logger.info(
+            f"Cap over {upper_limit}, keep the full number of training sample till "
+            f"{lower_limit}, samples smaller than that are oversampled"
+        )
+        train_df = (
+            train_base_df.groupby(class_balancing_column)
+            .filter(lambda x: len(x) >= upper_limit)
+            .groupby(class_balancing_column, group_keys=False)
+            .apply(pd.DataFrame.sample, upper_limit)
+        )
+        # Middle classes use the number as they are
+        train_df = pd.concat(
+            [
+                train_df,
+                train_base_df.groupby(class_balancing_column)
+                .filter(lambda x: len(x) < upper_limit)
+                .groupby(class_balancing_column)
+                .filter(lambda x: len(x) >= lower_limit),
+            ]
+        )
+        # For smaller classes, oversample...
+        train_df = pd.concat(
+            [
+                train_df,
+                train_base_df.groupby(class_balancing_column)
+                .filter(lambda x: len(x) < lower_limit)
+                .groupby(class_balancing_column, group_keys=False)
+                .apply(pd.DataFrame.sample, lower_limit, replace=True),
+            ]
+        )
+
+    elif balancing_strategy == "BALANCING_STRATEGY_MEDIUM2":
+        # Balance the train data, but still use some larger samples for the classes
+        # that have a lot of members in the input dataset
+        # Remark: with the upper limit of 10.000 this gives still OK results overall,
+        #     and also the smaller classes give some results with upper limit of 4000
+        #     results significantly less good.
+
+        # For the larger classes, leave the samples larger but cap
+        # Cap 1
+        cap_count_limit1 = 100000
+        cap_train_limit1 = 30000
+        logger.info(
+            f"Cap balancing classes over {cap_count_limit1} to {cap_train_limit1}"
+        )
+        train_capped_df = (
+            train_base_df.groupby(class_balancing_column)
+            .filter(lambda x: len(x) >= cap_count_limit1)
+            .groupby(class_balancing_column, group_keys=False)
+        )
+        if len(train_capped_df) > 0:
+            train_df = pd.concat(
+                [train_df, train_capped_df.apply(pd.DataFrame.sample, cap_train_limit1)]
+            )
+
+        # Cap 2
+        cap_count_limit2 = 50000
+        cap_train_limit2 = 20000
+        logger.info(
+            f"Cap balancing classes between {cap_count_limit2} and {cap_count_limit1} "
+            f"to {cap_train_limit2}"
+        )
+        train_capped_df = (
+            train_base_df.groupby(class_balancing_column)
+            .filter(lambda x: len(x) < cap_count_limit1)
+            .groupby(class_balancing_column)
+            .filter(lambda x: len(x) >= cap_count_limit2)
+            .groupby(class_balancing_column, group_keys=False)
+        )
+        if len(train_capped_df) > 0:
+            train_df = pd.concat(
+                [train_df, train_capped_df.apply(pd.DataFrame.sample, cap_train_limit2)]
+            )
+
+        # Cap 3
+        cap_count_limit3 = 20000
+        cap_train_limit3 = 10000
+        logger.info(
+            f"Cap balancing classes between {cap_count_limit3} and {cap_count_limit2} "
+            f"to {cap_train_limit3}"
+        )
+        train_capped_df = (
+            train_base_df.groupby(class_balancing_column)
+            .filter(lambda x: len(x) < cap_count_limit2)
+            .groupby(class_balancing_column)
+            .filter(lambda x: len(x) >= cap_count_limit3)
+            .groupby(class_balancing_column, group_keys=False)
+        )
+        if len(train_capped_df) > 0:
+            train_df = pd.concat(
+                [train_df, train_capped_df.apply(pd.DataFrame.sample, cap_train_limit3)]
+            )
+
+        # Cap 4
+        cap_count_limit4 = 10000
+        cap_train_limit4 = 10000
+        logger.info(
+            f"Cap balancing classes between {cap_count_limit4} and {cap_count_limit3} "
+            f"to {cap_train_limit4}"
+        )
+        train_capped_df = (
+            train_base_df.groupby(class_balancing_column)
+            .filter(lambda x: len(x) < cap_count_limit3)
+            .groupby(class_balancing_column)
+            .filter(lambda x: len(x) >= cap_count_limit4)
+            .groupby(class_balancing_column, group_keys=False)
+        )
+        if len(train_capped_df) > 0:
+            train_df = pd.concat(
+                [train_df, train_capped_df.apply(pd.DataFrame.sample, cap_train_limit4)]
+            )
+
+        # Middle classes use the number as they are, smaller classes are oversampled
+        oversample_count = 1000
+        logger.info(
+            f"For classes between {cap_count_limit4} and {oversample_count}, just use "
+            "all samples"
+        )
+        train_df = pd.concat(
+            [
+                train_df,
+                train_base_df.groupby(class_balancing_column)
+                .filter(lambda x: len(x) < cap_count_limit4)
+                .groupby(class_balancing_column)
+                .filter(lambda x: len(x) >= oversample_count),
+            ]
+        )
+        # For smaller classes, oversample...
+        logger.info(
+            f"For classes smaller than {oversample_count}, oversample to "
+            f"{oversample_count}"
+        )
+        train_capped_df = (
+            train_base_df.groupby(class_balancing_column)
+            .filter(lambda x: len(x) < oversample_count)
+            .groupby(class_balancing_column, group_keys=False)
+        )
+        if len(train_capped_df) > 0:
+            train_df = pd.concat(
+                [
+                    train_df,
+                    train_capped_df.apply(
+                        pd.DataFrame.sample, oversample_count, replace=True
+                    ),
+                ]
+            )
+
+    elif balancing_strategy == "BALANCING_STRATEGY_PROPORTIONAL_GROUPS":
+        # Balance the train data, but still use some larger samples for the classes
+        # that have a lot of members in the input dataset
+        # Remark: with the upper limit of 10.000 this gives still OK results overall,
+        #     and also the smaller classes give some results with upper limit of 4000
+        #     results significantly less good.
+
+        # For the larger classes, leave the samples larger but cap
+        upper_count_limit1 = 100000
+        upper_train_limit1 = 30000
+        logger.info(
+            f"Cap balancing classes over {upper_count_limit1} to {upper_train_limit1}"
+        )
+        train_df = (
+            train_base_df.groupby(class_balancing_column)
+            .filter(lambda x: len(x) >= upper_count_limit1)
+            .groupby(class_balancing_column, group_keys=False)
+            .apply(pd.DataFrame.sample, upper_train_limit1)
+        )
+        upper_count_limit2 = 50000
+        upper_train_limit2 = 20000
+        logger.info(
+            f"Cap balancing classes between {upper_count_limit2} and "
+            f"{upper_count_limit1} to {upper_train_limit2}"
+        )
+        train_limit2_df = (
+            train_base_df.groupby(class_balancing_column)
+            .filter(lambda x: len(x) < upper_count_limit1)
+            .groupby(class_balancing_column)
+            .filter(lambda x: len(x) >= upper_count_limit2)
+            .groupby(class_balancing_column, group_keys=False)
+        )
+        if len(train_limit2_df) > 0:
+            train_df = pd.concat(
+                [
+                    train_df,
+                    train_limit2_df.apply(pd.DataFrame.sample, upper_train_limit2),
+                ]
+            )
+        upper_count_limit3 = 20000
+        upper_train_limit3 = 10000
+        logger.info(
+            f"Cap balancing classes between {upper_count_limit3} and "
+            f"{upper_count_limit2} to {upper_train_limit3}"
+        )
+        train_limit3_df = (
+            train_base_df.groupby(class_balancing_column)
+            .filter(lambda x: len(x) < upper_count_limit2)
+            .groupby(class_balancing_column)
+            .filter(lambda x: len(x) >= upper_count_limit3)
+            .groupby(class_balancing_column, group_keys=False)
+        )
+        if len(train_limit3_df) > 0:
+            train_df = pd.concat(
+                [
+                    train_df,
+                    train_limit3_df.apply(pd.DataFrame.sample, upper_train_limit3),
+                ]
+            )
+        upper_count_limit4 = 10000
+        upper_train_limit4 = 5000
+        logger.info(
+            f"Cap balancing classes between {upper_count_limit4} and "
+            f"{upper_count_limit3} to {upper_train_limit4}"
+        )
+        train_limit4_df = (
+            train_base_df.groupby(class_balancing_column)
+            .filter(lambda x: len(x) < upper_count_limit3)
+            .groupby(class_balancing_column)
+            .filter(lambda x: len(x) >= upper_count_limit4)
+            .groupby(class_balancing_column, group_keys=False)
+        )
+        if len(train_limit4_df) > 0:
+            train_df = pd.concat(
+                [
+                    train_df,
+                    train_limit4_df.apply(pd.DataFrame.sample, upper_train_limit4),
+                ]
+            )
+        # For smaller balancing classes, just use all samples
+        train_df = pd.concat(
+            [
+                train_df,
+                train_base_df.groupby(class_balancing_column).filter(
+                    lambda x: len(x) < upper_count_limit4
+                ),
+            ]
+        )
+
+    elif balancing_strategy == "BALANCING_STRATEGY_UPPER_LIMIT":
+        # Balance the train data, but still use some larger samples for the classes
+        # that have a lot of members in the input dataset
+        # Remark: with the upper limit of 10.000 this gives still OK results overall,
+        #     and also the smaller classes give some results with upper limit of 4000
+        #     results significantly less good.
+
+        # For the larger classes, favor them by leaving the samples larger but cap at
+        # upper_limit
+        upper_limit = 10000
+        logger.info(f"Cap over {upper_limit}...")
+        train_df = (
+            train_base_df.groupby(class_balancing_column)
+            .filter(lambda x: len(x) >= upper_limit)
+            .groupby(class_balancing_column, group_keys=False)
+            .apply(pd.DataFrame.sample, upper_limit)
+        )
+        # For smaller classes, just use all samples
+        train_df = pd.concat(
+            [
+                train_df,
+                train_base_df.groupby(class_balancing_column).filter(
+                    lambda x: len(x) < upper_limit
+                ),
+            ]
+        )
+
+    elif balancing_strategy == "BALANCING_STRATEGY_EQUAL":
+        # In theory the most logical way to balance: make sure all classes have the
+        # same amount of training data by undersampling the largest classes and
+        # oversampling the small classes.
+        train_df = train_base_df.groupby(
+            class_balancing_column, group_keys=False
+        ).apply(pd.DataFrame.sample, 2000, replace=True)
+
+    else:
+        raise Exception(f"Unknown balancing strategy, STOP!: {balancing_strategy}")
+
+    # Log the resulting numbers per class in the train sample
+    with pd.option_context(
+        "display.max_rows", None, "display.max_columns", None
+    ):  # type: ignore
+        count_per_class = train_df.groupby(
+            class_balancing_column, as_index=False
+        ).size()
+        logger.info(
+            "Number of elements per class_balancing_column in train dataset:\n"
+            f"{count_per_class}"
+        )
+        if class_balancing_column != class_column:
+            count_per_class = train_df.groupby(class_column, as_index=False).size()
+            logger.info(
+                "Number of elements per class_column in train dataset:\n"
+                f"{count_per_class}"
+            )
+
+    # Log the resulting numbers per class in the test sample
+    with pd.option_context(
+        "display.max_rows", None, "display.max_columns", None
+    ):  # type: ignore
+        count_per_class = test_df.groupby(class_balancing_column, as_index=False).size()
+        logger.info(
+            "Number of elements per class_balancing_column in test dataset:\n"
+            f"{count_per_class}"
+        )
+        if class_balancing_column != class_column:
+            count_per_class = test_df.groupby(class_column, as_index=False).size()
+            logger.info(
+                "Number of elements per class_column in test dataset:\n"
+                f"{count_per_class}"
+            )
+
+    # Write to output files
+    logger.info("Write the output files")
+    train_df.set_index(conf.columns["id"], inplace=True)
+    test_df.set_index(conf.columns["id"], inplace=True)
+    pdh.to_file(train_df, output_parcel_train_path)  # The ID column is the index...
+    pdh.to_file(test_df, output_parcel_test_path)  # The ID column is the index...
```

### Comparing `cropclassification-0.1.0a2/cropclassification/preprocess/classification_preprocess_BEFL.py` & `cropclassification-0.1.1/cropclassification/preprocess/_classification_preprocess_BEFL.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,1007 +1,1076 @@
-# -*- coding: utf-8 -*-
-"""
-Create the parcel classes that will be used for the classification.
-
-This implementation will create +- 40 classes.
-parcel that don't have a clear classification in the input file get class 'UNKNOWN'.
-"""
-
-import logging
-from pathlib import Path
-
-import geofileops as gfo
-
-import cropclassification.helpers.config_helper as conf
-import cropclassification.helpers.pandas_helper as pdh
-
-# Get a logger...
-logger = logging.getLogger(__name__)
-
-# define some specific BEFL column names
-column_BEFL_earlylate = "MON_EARLY_LATE"  # Is it an early or a late crop?
-column_BEFL_gesp_pm = "GESP_PM"  # Gespecialiseerde productiemethode
-column_BEFL_gis_area = "GRAF_OPP"  # GIS Area
-column_BEFL_status_perm_grass = "STAT_BGV"  # Status permanent grassland
-column_BEFL_crop = "GWSCOD_H"
-column_BEFL_crop_declared = "GWSCOD_H_A"
-column_BEFL_crop_gt_verified = "HOOFDTEELT_CTRL_COD"
-column_BEFL_crop_gt_unverified = "HOOFDTEELT_CTRL_COD_ORIG"
-column_BEFL_latecrop = "GWSCOD_N"
-
-# BEFL specific columns we want keep
-columns_BEFL_to_keep = [
-    column_BEFL_earlylate,
-    column_BEFL_gesp_pm,
-    column_BEFL_gis_area,
-    column_BEFL_status_perm_grass,
-    column_BEFL_crop_gt_verified,
-    column_BEFL_crop_gt_unverified,
-    column_BEFL_crop,
-    column_BEFL_crop_declared,
-    column_BEFL_latecrop,
-]
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def prepare_input(
-    input_parcel_path: Path,
-    classtype_to_prepare: str,
-    classes_refe_path: Path,
-    output_dir: Path,
-):
-    """
-    This function creates a file that is compliant with the assumptions used by the rest of the
-    classification functionality.
-
-    It should be a csv file with the following columns:
-        - object_id: column with a unique identifier
-        - classname: a string column with a readable name of the classes that will be classified to
-    """
-    # Check if input parameters are OK
-    if not input_parcel_path.exists():
-        raise Exception(f"Input file doesn't exist: {input_parcel_path}")
-    else:
-        logger.info(f"Process input file {input_parcel_path}")
-
-    # Read input file
-    logger.info(f"Read parceldata from {input_parcel_path}")
-    if gfo.is_geofile(input_parcel_path):
-        parceldata_df = gfo.read_file(input_parcel_path)
-    else:
-        parceldata_df = pdh.read_file(input_parcel_path)
-    logger.info(f"Read Parceldata ready, info(): {parceldata_df.info()}")
-
-    # Check if the id column is present...
-    if conf.columns["id"] not in parceldata_df.columns:
-        message = f"Column {conf.columns['id']} not found in input parcel file: {input_parcel_path}. Make sure the column is present or change the column name in global_constants.py"
-        logger.critical(message)
-        raise Exception(message)
-
-    # Now start prepare
-    if classtype_to_prepare == "CROPGROUP":
-        parceldata_df = prepare_input_cropgroup(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop_declared,
-            column_output_class=conf.columns["class_declared"],
-            classes_refe_path=classes_refe_path,
-        )
-        return prepare_input_cropgroup(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop,
-            column_output_class=conf.columns["class"],
-            classes_refe_path=classes_refe_path,
-        )
-    elif classtype_to_prepare == "CROPGROUP-GROUNDTRUTH":
-        return prepare_input_cropgroup(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop_gt_verified,
-            column_output_class=conf.columns["class_groundtruth"],
-            classes_refe_path=classes_refe_path,
-        )
-    elif classtype_to_prepare == "CROPGROUP-EARLY":
-        parceldata_df = prepare_input_cropgroup_early(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop_declared,
-            column_output_class=conf.columns["class_declared"],
-            classes_refe_path=classes_refe_path,
-        )
-        return prepare_input_cropgroup_early(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop,
-            column_output_class=conf.columns["class"],
-            classes_refe_path=classes_refe_path,
-        )
-    elif classtype_to_prepare == "CROPGROUP-EARLY-GROUNDTRUTH":
-        return prepare_input_cropgroup_early(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop_gt_verified,
-            column_output_class=conf.columns["class_groundtruth"],
-            classes_refe_path=classes_refe_path,
-        )
-    elif classtype_to_prepare == "LANDCOVER":
-        parceldata_df = prepare_input_landcover(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop_declared,
-            column_output_class=conf.columns["class_declared"],
-            classes_refe_path=classes_refe_path,
-        )
-        return prepare_input_landcover(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop,
-            column_output_class=conf.columns["class"],
-            classes_refe_path=classes_refe_path,
-        )
-    elif classtype_to_prepare == "MULTICROP":
-        parceldata_df = prepare_input_landcover(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop_declared,
-            column_output_class=conf.columns["class_declared"],
-            classes_refe_path=classes_refe_path,
-        )
-        return prepare_input_landcover(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop,
-            column_output_class=conf.columns["class"],
-            classes_refe_path=classes_refe_path,
-        )
-    elif classtype_to_prepare == "LANDCOVER-GROUNDTRUTH":
-        return prepare_input_landcover(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop_gt_verified,
-            column_output_class=conf.columns["class_groundtruth"],
-            classes_refe_path=classes_refe_path,
-        )
-    elif classtype_to_prepare == "LANDCOVER-EARLY":
-        parceldata_df = prepare_input_landcover_early(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop_declared,
-            column_output_class=conf.columns["class_declared"],
-            classes_refe_path=classes_refe_path,
-        )
-        return prepare_input_landcover_early(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop,
-            column_output_class=conf.columns["class"],
-            classes_refe_path=classes_refe_path,
-        )
-    elif classtype_to_prepare == "LANDCOVER-EARLY-GROUNDTRUTH":
-        return prepare_input_landcover_early(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop_gt_verified,
-            column_output_class=conf.columns["class_groundtruth"],
-            classes_refe_path=classes_refe_path,
-        )
-    elif classtype_to_prepare == "POPULAR-CROP":
-        parceldata_df = prepare_input_most_popular_crop(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop_declared,
-            column_output_class=conf.columns["class_declared"],
-            classes_refe_path=classes_refe_path,
-        )
-        return prepare_input_most_popular_crop(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop,
-            column_output_class=conf.columns["class"],
-            classes_refe_path=classes_refe_path,
-        )
-    elif classtype_to_prepare == "POPULAR-CROP-GROUNDTRUTH":
-        return prepare_input_most_popular_crop(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop_gt_verified,
-            column_output_class=conf.columns["class_groundtruth"],
-            classes_refe_path=classes_refe_path,
-        )
-    elif classtype_to_prepare == "LATECROP":
-        parceldata_df = prepare_input_latecrop(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_latecrop,
-            column_output_class=conf.columns["class_declared"],
-            classes_refe_path=classes_refe_path,
-        )
-        return prepare_input_latecrop(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_latecrop,
-            column_output_class=conf.columns["class"],
-            classes_refe_path=classes_refe_path,
-        )
-    elif classtype_to_prepare == "FABACEAE":
-        parceldata_df = prepare_input_fabaceae(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop,
-            column_output_class=conf.columns["class_declared"],
-            classes_refe_path=classes_refe_path,
-        )
-        return prepare_input_fabaceae(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop,
-            column_output_class=conf.columns["class"],
-            classes_refe_path=classes_refe_path,
-        )
-    elif classtype_to_prepare == "FABACEAE-GROUNDTRUTH":
-        return prepare_input_fabaceae(
-            parceldata_df=parceldata_df,
-            column_BEFL_cropcode=column_BEFL_crop_gt_verified,
-            column_output_class=conf.columns["class_groundtruth"],
-            classes_refe_path=classes_refe_path,
-        )
-    else:
-        message = (
-            f"Unknown value for parameter classtype_to_prepare: {classtype_to_prepare}"
-        )
-        logger.critical(message)
-        raise Exception(message)
-
-
-def prepare_input_cropgroup(
-    parceldata_df,
-    column_BEFL_cropcode: str,
-    column_output_class: str,
-    classes_refe_path: Path,
-):
-    """
-    This function creates a file that is compliant with the assumptions used by the rest of the
-    classification functionality.
-
-    It should be a csv file with the following columns:
-        - object_id: column with a unique identifier
-        - classname: a string column with a readable name of the classes that will be classified to
-
-    This specific implementation converts the typiscal export format used in BE-Flanders to
-    this format.
-    """
-    # Check if parameters are OK and init some extra params
-    # --------------------------------------------------------------------------
-    if not classes_refe_path.exists():
-        raise Exception(f"Input classes file doesn't exist: {classes_refe_path}")
-
-    # Convert the crop to unicode, in case the input is int...
-    if column_BEFL_cropcode in parceldata_df.columns:
-        parceldata_df[column_BEFL_cropcode] = parceldata_df[
-            column_BEFL_cropcode
-        ].astype("unicode")
-
-    # Read and cleanup the mapping table from crop codes to classes
-    # --------------------------------------------------------------------------
-    logger.info(f"Read classes conversion table from {classes_refe_path}")
-    classes_df = pdh.read_file(classes_refe_path)
-    logger.info(f"Read classes conversion table ready, info(): {classes_df.info()}")
-
-    # Because the file was read as ansi, and gewas is int, so the data needs to be converted to
-    # unicode to be able to do comparisons with the other data
-    classes_df[column_BEFL_cropcode] = classes_df["CROPCODE"].astype("unicode")
-
-    # Map column with the classname to orig classname
-    column_output_class_orig = conf.columns["class"] + "_orig"
-    classes_df[column_output_class_orig] = classes_df[conf.columns["class_refe"]]
-
-    # Remove unneeded columns
-    for column in classes_df.columns:
-        if (
-            column not in [column_output_class_orig, column_BEFL_cropcode]
-            and column not in columns_BEFL_to_keep
-        ):
-            classes_df.drop(column, axis=1, inplace=True)
-
-    # Set the index
-    classes_df.set_index(column_BEFL_cropcode, inplace=True, verify_integrity=True)
-
-    # Get only the columns in the classes_df that don't exist yet in parceldata_df
-    cols_to_join = classes_df.columns.difference(parceldata_df.columns)
-
-    # Join/merge the classname
-    logger.info("Add the classes to the parceldata")
-    parceldata_df = parceldata_df.merge(
-        classes_df[cols_to_join],
-        how="left",
-        left_on=column_BEFL_cropcode,
-        right_index=True,
-        validate="many_to_one",
-    )
-
-    # Copy orig classname to classification classname
-    parceldata_df.insert(
-        loc=0, column=column_output_class, value=parceldata_df[column_output_class_orig]
-    )
-
-    # For rows with no class, set to UNKNOWN
-    parceldata_df.fillna(value={column_output_class: "UNKNOWN"}, inplace=True)
-
-    # If a column with extra info exists, use it as well to fine-tune the classification classes.
-    if column_BEFL_gesp_pm in parceldata_df.columns:
-        # Serres, tijdelijke overkappingen en loodsen
-        parceldata_df.loc[
-            parceldata_df[column_BEFL_gesp_pm].isin(["SER", "SGM"]), column_output_class
-        ] = "MON_OVERK_LOO"
-        parceldata_df.loc[
-            parceldata_df[column_BEFL_gesp_pm].isin(["PLA", "PLO", "NPO"]),
-            column_output_class,
-        ] = "MON_OVERK_LOO"
-        parceldata_df.loc[
-            parceldata_df[column_BEFL_gesp_pm] == "LOO", column_output_class
-        ] = "MON_OVERK_LOO"  # Een loods is hetzelfde als een stal...
-        parceldata_df.loc[
-            parceldata_df[column_BEFL_gesp_pm] == "CON", column_output_class
-        ] = "MON_CONTAINERS"  # Containers, niet op volle grond...
-        # TODO: CIV, containers in volle grond, lijkt niet zo specifiek te zijn...
-        # parceldata_df.loc[parceldata_df[column_BEFL_gesp_pm] == 'CIV', class_columnname] = 'MON_CONTAINERS'   # Containers, niet op volle grond...
-    else:
-        logger.warning(
-            f"The column {column_BEFL_gesp_pm} doesn't exist, so this part of the code was skipped!"
-        )
-
-    # Some extra cleanup: classes starting with 'nvt' or empty ones
-    # logger.info("Set classes that are still empty, not specific enough or that contain to little values to 'UNKNOWN'")
-    # parceldata_df.loc[parceldata_df[column_output_class].str.startswith('nvt', na=True),
-    #                  column_output_class] = 'UNKNOWN'
-
-    # 'MON_ANDERE_SUBSID_GEWASSEN': very low classification rate (< 1%), as it is a group with several very different classes in it
-    # 'MON_AARDBEIEN': low classification rate (~10%), as many parcel actually are temporary greenhouses but aren't correctly applied
-    # 'MON_BRAAK': very low classification rate (< 1%), spread over a lot of classes, but most popular are MON_BOOM, MON_GRASSEN, MON_FRUIT
-    # 'MON_KLAVER': log classification rate (25%), spread over quite some classes, but MON GRASSES has 20% as well.
-    # 'MON_MENGSEL': 25% correct classifications: rest spread over many other classes. Too heterogenous in group?
-    # 'MON_POEL': 0% correct classifications: most are classified as MON_CONTAINER, MON_FRUIT. Almost nothing was misclassified as being POEL
-    # 'MON_RAAPACHTIGEN': 25% correct classifications: rest spread over many other classes
-    # 'MON_STRUIK': 10%
-    #    TODO: nakijken, wss opsplitsen of toevoegen aan MON_BOOMKWEEK???
-    # classes_badresults = ['MON_ANDERE_SUBSID_GEWASSEN', 'MON_AARDBEIEN', 'MON_BRAAK', 'MON_KLAVER',
-    #                      'MON_MENGSEL', 'MON_POEL', 'MON_RAAPACHTIGEN', 'MON_STRUIK']
-    # parceldata_df.loc[parceldata_df[column_output_class].isin(classes_badresults),
-    #                  column_output_class] = 'UNKNOWN'
-
-    # MON_BONEN en MON_WIKKEN have omongst each other a very large percentage of false
-    # positives/negatives, so they seem very similar... lets create a class that combines both
-    # parceldata_df.loc[parceldata_df[column_output_class].isin(['MON_BONEN', 'MON_WIKKEN']),
-    #                  column_output_class] = 'MON_BONEN_WIKKEN'
-
-    # MON_BOOM includes now also the growing new plants/trees, which is too differenct from grown
-    # trees -> put growing new trees is seperate group
-    # parceldata_df.loc[parceldata_df[column_BEFL_cropcode].isin(['9602', '9603', '9604', '9560']),
-    #                  column_output_class] = 'MON_BOOMKWEEK'
-
-    # 'MON_FRUIT': has a good accuracy (91%), but also has as much false positives (115% -> mainly
-    #              'MON_GRASSEN' that are (mis)classified as 'MON_FRUIT')
-    # 'MON_BOOM': has very bad accuracy (28%) and also very much false positives (450% -> mainly
-    #              'MON_GRASSEN' that are misclassified as 'MON_BOOM')
-    # MON_FRUIT and MON_BOOM are permanent anyway, so not mandatory that they are checked in
-    # monitoring process.
-    # Conclusion: put MON_BOOM and MON_FRUIT to IGNORE_DIFFICULT_PERMANENT_CLASS
-    # parceldata_df.loc[parceldata_df[column_output_class].isin(['MON_BOOM', 'MON_FRUIT']),
-    #                  column_output_class] = 'IGNORE_DIFFICULT_PERMANENT_CLASS'
-
-    # Set classes with very few elements to IGNORE_NOT_ENOUGH_SAMPLES!
-    for _, row in (
-        parceldata_df.groupby(column_output_class)
-        .size()
-        .reset_index(name="count")
-        .iterrows()
-    ):
-        if row["count"] <= 50:
-            logger.info(
-                f"Class <{row[column_output_class]}> only contains {row['count']} elements, so put them to IGNORE_NOT_ENOUGH_SAMPLES"
-            )
-            parceldata_df.loc[
-                parceldata_df[column_output_class] == row[column_output_class],
-                column_output_class,
-            ] = "IGNORE_NOT_ENOUGH_SAMPLES"
-
-    # Drop the columns that aren't useful at all
-    for column in parceldata_df.columns:
-        if (
-            column
-            not in [
-                column_output_class,
-                conf.columns["id"],
-                conf.columns["class_groundtruth"],
-                conf.columns["class_declared"],
-            ]
-            and column not in conf.preprocess.getlist("extra_export_columns")
-            and column not in columns_BEFL_to_keep
-        ):
-            parceldata_df.drop(column, axis=1, inplace=True)
-        elif column == column_BEFL_gesp_pm:
-            parceldata_df[column_BEFL_gesp_pm] = parceldata_df[
-                column_BEFL_gesp_pm
-            ].str.replace(",", ";")
-
-    return parceldata_df
-
-
-def prepare_input_fabaceae(
-    parceldata_df,
-    column_BEFL_cropcode: str,
-    column_output_class: str,
-    classes_refe_path: Path,
-):
-    """
-    This function creates a file that is compliant with the assumptions used by the rest of the
-    classification functionality.
-
-    It should be a csv file with the following columns:
-        - object_id: column with a unique identifier
-        - classname: a string column with a readable name of the classes that will be classified to
-
-    This specific implementation converts the typiscal export format used in BE-Flanders to
-    this format.
-    """
-    # Check if parameters are OK and init some extra params
-    # --------------------------------------------------------------------------
-    if not classes_refe_path.exists():
-        raise Exception(f"Input classes file doesn't exist: {classes_refe_path}")
-
-    # Convert the crop to unicode, in case the input is int...
-    if column_BEFL_cropcode in parceldata_df.columns:
-        parceldata_df[column_BEFL_cropcode] = parceldata_df[
-            column_BEFL_cropcode
-        ].astype("unicode")
-
-    # Read and cleanup the mapping table from crop codes to classes
-    # --------------------------------------------------------------------------
-    logger.info(f"Read classes conversion table from {classes_refe_path}")
-    classes_df = pdh.read_file(classes_refe_path)
-    logger.info(f"Read classes conversion table ready, info(): {classes_df.info()}")
-
-    # Because the file was read as ansi, and gewas is int, so the data needs to be converted to
-    # unicode to be able to do comparisons with the other data
-    classes_df[column_BEFL_cropcode] = classes_df["CROPCODE"].astype("unicode")
-
-    # Map column with the classname to orig classname
-    column_output_class_orig = conf.columns["class"] + "_orig"
-    classes_df[column_output_class_orig] = classes_df[conf.columns["class_refe"]]
-
-    # Remove unneeded columns
-    for column in classes_df.columns:
-        if (
-            column not in [column_output_class_orig, column_BEFL_cropcode]
-            and column not in columns_BEFL_to_keep
-        ):
-            classes_df.drop(column, axis=1, inplace=True)
-
-    # Set the index
-    classes_df.set_index(column_BEFL_cropcode, inplace=True, verify_integrity=True)
-
-    # Get only the columns in the classes_df that don't exist yet in parceldata_df
-    cols_to_join = classes_df.columns.difference(parceldata_df.columns)
-
-    # Filter the parcels to only keep the classes we are interested in
-    # TODO: this shouldn't be hardcoded!
-    parceldata_df = parceldata_df.loc[
-        parceldata_df[column_BEFL_cropcode].isin(["60", "700", "660", "732", "723"])
-    ]
-
-    # Join/merge the classname
-    logger.info("Add the classes to the parceldata")
-    parceldata_df = parceldata_df.merge(
-        classes_df[cols_to_join],
-        how="left",
-        left_on=column_BEFL_cropcode,
-        right_index=True,
-        validate="many_to_one",
-    )
-
-    # Copy orig classname to classification classname
-    parceldata_df.insert(
-        loc=0, column=column_output_class, value=parceldata_df[column_output_class_orig]
-    )
-
-    # For rows with no class, set to UNKNOWN
-    parceldata_df.fillna(value={column_output_class: "UNKNOWN"}, inplace=True)
-
-    # If a column with extra info exists, use it as well to fine-tune the classification classes.
-    if column_BEFL_gesp_pm in parceldata_df.columns:
-        # Serres, tijdelijke overkappingen en loodsen
-        parceldata_df.loc[
-            parceldata_df[column_BEFL_gesp_pm].isin(["SER", "SGM"]), column_output_class
-        ] = "MON_OVERK_LOO"
-        parceldata_df.loc[
-            parceldata_df[column_BEFL_gesp_pm].isin(["PLA", "PLO", "NPO"]),
-            column_output_class,
-        ] = "MON_OVERK_LOO"
-        parceldata_df.loc[
-            parceldata_df[column_BEFL_gesp_pm] == "LOO", column_output_class
-        ] = "MON_OVERK_LOO"  # Een loods is hetzelfde als een stal...
-        parceldata_df.loc[
-            parceldata_df[column_BEFL_gesp_pm] == "CON", column_output_class
-        ] = "MON_CONTAINERS"  # Containers, niet op volle grond...
-        # TODO: CIV, containers in volle grond, lijkt niet zo specifiek te zijn...
-        # parceldata_df.loc[parceldata_df[column_BEFL_gesp_pm] == 'CIV', class_columnname] = 'MON_CONTAINERS'   # Containers, niet op volle grond...
-    else:
-        logger.warning(
-            f"The column {column_BEFL_gesp_pm} doesn't exist, so this part of the code was skipped!"
-        )
-
-    # Some extra cleanup: classes starting with 'nvt' or empty ones
-    # logger.info("Set classes that are still empty, not specific enough or that contain to little values to 'UNKNOWN'")
-    # parceldata_df.loc[parceldata_df[column_output_class].str.startswith('nvt', na=True),
-    #                  column_output_class] = 'UNKNOWN'
-
-    # 'MON_ANDERE_SUBSID_GEWASSEN': very low classification rate (< 1%), as it is a group with several very different classes in it
-    # 'MON_AARDBEIEN': low classification rate (~10%), as many parcel actually are temporary greenhouses but aren't correctly applied
-    # 'MON_BRAAK': very low classification rate (< 1%), spread over a lot of classes, but most popular are MON_BOOM, MON_GRASSEN, MON_FRUIT
-    # 'MON_KLAVER': log classification rate (25%), spread over quite some classes, but MON GRASSES has 20% as well.
-    # 'MON_MENGSEL': 25% correct classifications: rest spread over many other classes. Too heterogenous in group?
-    # 'MON_POEL': 0% correct classifications: most are classified as MON_CONTAINER, MON_FRUIT. Almost nothing was misclassified as being POEL
-    # 'MON_RAAPACHTIGEN': 25% correct classifications: rest spread over many other classes
-    # 'MON_STRUIK': 10%
-    #    TODO: nakijken, wss opsplitsen of toevoegen aan MON_BOOMKWEEK???
-    # classes_badresults = ['MON_ANDERE_SUBSID_GEWASSEN', 'MON_AARDBEIEN', 'MON_BRAAK', 'MON_KLAVER',
-    #                      'MON_MENGSEL', 'MON_POEL', 'MON_RAAPACHTIGEN', 'MON_STRUIK']
-    # parceldata_df.loc[parceldata_df[column_output_class].isin(classes_badresults),
-    #                  column_output_class] = 'UNKNOWN'
-
-    # MON_BONEN en MON_WIKKEN have omongst each other a very large percentage of false
-    # positives/negatives, so they seem very similar... lets create a class that combines both
-    # parceldata_df.loc[parceldata_df[column_output_class].isin(['MON_BONEN', 'MON_WIKKEN']),
-    #                  column_output_class] = 'MON_BONEN_WIKKEN'
-
-    # MON_BOOM includes now also the growing new plants/trees, which is too differenct from grown
-    # trees -> put growing new trees is seperate group
-    # parceldata_df.loc[parceldata_df[column_BEFL_cropcode].isin(['9602', '9603', '9604', '9560']),
-    #                  column_output_class] = 'MON_BOOMKWEEK'
-
-    # 'MON_FRUIT': has a good accuracy (91%), but also has as much false positives (115% -> mainly
-    #              'MON_GRASSEN' that are (mis)classified as 'MON_FRUIT')
-    # 'MON_BOOM': has very bad accuracy (28%) and also very much false positives (450% -> mainly
-    #              'MON_GRASSEN' that are misclassified as 'MON_BOOM')
-    # MON_FRUIT and MON_BOOM are permanent anyway, so not mandatory that they are checked in
-    # monitoring process.
-    # Conclusion: put MON_BOOM and MON_FRUIT to IGNORE_DIFFICULT_PERMANENT_CLASS
-    # parceldata_df.loc[parceldata_df[column_output_class].isin(['MON_BOOM', 'MON_FRUIT']),
-    #                  column_output_class] = 'IGNORE_DIFFICULT_PERMANENT_CLASS'
-
-    # Set classes with very few elements to IGNORE_NOT_ENOUGH_SAMPLES!
-    for _, row in (
-        parceldata_df.groupby(column_output_class)
-        .size()
-        .reset_index(name="count")
-        .iterrows()
-    ):
-        if row["count"] <= 50:
-            logger.info(
-                f"Class <{row[column_output_class]}> only contains {row['count']} elements, so put them to IGNORE_NOT_ENOUGH_SAMPLES"
-            )
-            parceldata_df.loc[
-                parceldata_df[column_output_class] == row[column_output_class],
-                column_output_class,
-            ] = "IGNORE_NOT_ENOUGH_SAMPLES"
-
-    # Drop the columns that aren't useful at all
-    for column in parceldata_df.columns:
-        if (
-            column
-            not in [
-                column_output_class,
-                conf.columns["id"],
-                conf.columns["class_groundtruth"],
-                conf.columns["class_declared"],
-            ]
-            and column not in conf.preprocess.getlist("extra_export_columns")
-            and column not in columns_BEFL_to_keep
-        ):
-            parceldata_df.drop(column, axis=1, inplace=True)
-        elif column == column_BEFL_gesp_pm:
-            parceldata_df[column_BEFL_gesp_pm] = parceldata_df[
-                column_BEFL_gesp_pm
-            ].str.replace(",", ";")
-
-    return parceldata_df
-
-
-def prepare_input_latecrop(
-    parceldata_df,
-    column_BEFL_cropcode: str,
-    column_output_class: str,
-    classes_refe_path: Path,
-):
-    """
-    This function creates a file that is compliant with the assumptions used by the rest of the
-    classification functionality.
-
-    It should be a csv file with the following columns:
-        - object_id: column with a unique identifier
-        - classname: a string column with a readable name of the classes that will be classified to
-
-    This specific implementation converts the typiscal export format used in BE-Flanders to
-    this format.
-    """
-    # Check if parameters are OK and init some extra params
-    # --------------------------------------------------------------------------
-    if not classes_refe_path.exists():
-        raise Exception(f"Input classes file doesn't exist: {classes_refe_path}")
-
-    # Convert the crop to unicode, in case the input is int...
-    if column_BEFL_cropcode in parceldata_df.columns:
-        parceldata_df[column_BEFL_cropcode] = parceldata_df[
-            column_BEFL_cropcode
-        ].astype("unicode")
-
-    # Read and cleanup the mapping table from crop codes to classes
-    # --------------------------------------------------------------------------
-    logger.info(f"Read classes conversion table from {classes_refe_path}")
-    classes_df = pdh.read_file(classes_refe_path)
-    logger.info(f"Read classes conversion table ready, info(): {classes_df.info()}")
-
-    # Because the file was read as ansi, and gewas is int, so the data needs to be converted to
-    # unicode to be able to do comparisons with the other data
-    classes_df[column_BEFL_cropcode] = classes_df["CROPCODE"].astype("unicode")
-
-    # Map column with the classname to orig classname
-    column_output_class_orig = conf.columns["class"] + "_orig"
-    classes_df[column_output_class_orig] = classes_df[conf.columns["class_refe"]]
-
-    # Remove unneeded columns
-    for column in classes_df.columns:
-        if (
-            column
-            not in [
-                column_output_class_orig,
-                column_BEFL_cropcode,
-                conf.columns["class_declared"],
-                conf.columns["class"],
-            ]
-            and column not in columns_BEFL_to_keep
-        ):
-            classes_df.drop(column, axis=1, inplace=True)
-
-    # Set the index
-    classes_df.set_index(column_BEFL_cropcode, inplace=True, verify_integrity=True)
-
-    # Get only the columns in the classes_df that don't exist yet in parceldata_df
-    cols_to_join = classes_df.columns.difference(parceldata_df.columns)
-
-    # Join/merge the classname
-    logger.info("Add the classes to the parceldata")
-    parceldata_df = parceldata_df.merge(
-        classes_df[cols_to_join],
-        how="left",
-        left_on=column_BEFL_cropcode,
-        right_index=True,
-        validate="many_to_one",
-    )
-
-    # Copy orig classname to classification classname
-    parceldata_df.insert(
-        loc=0, column=column_output_class, value=parceldata_df[column_output_class_orig]
-    )
-
-    # For rows with no class, set to UNKNOWN
-    parceldata_df.fillna(value={column_output_class: "UNKNOWN"}, inplace=True)
-
-    # If a column with extra info exists, use it as well to fine-tune the classification classes.
-    if column_BEFL_gesp_pm in parceldata_df.columns:
-        # Serres, tijdelijke overkappingen en loodsen
-        parceldata_df.loc[
-            parceldata_df[column_BEFL_gesp_pm].isin(["SER", "SGM"]), column_output_class
-        ] = "MON_OVERK_LOO"
-        parceldata_df.loc[
-            parceldata_df[column_BEFL_gesp_pm].isin(["PLA", "PLO", "NPO"]),
-            column_output_class,
-        ] = "MON_OVERK_LOO"
-        parceldata_df.loc[
-            parceldata_df[column_BEFL_gesp_pm] == "LOO", column_output_class
-        ] = "MON_OVERK_LOO"  # Een loods is hetzelfde als een stal...
-        parceldata_df.loc[
-            parceldata_df[column_BEFL_gesp_pm] == "CON", column_output_class
-        ] = "MON_CONTAINERS"  # Containers, niet op volle grond...
-        # TODO: CIV, containers in volle grond, lijkt niet zo specifiek te zijn...
-        # parceldata_df.loc[parceldata_df[column_BEFL_gesp_pm] == 'CIV', class_columnname] = 'MON_CONTAINERS'   # Containers, niet op volle grond...
-    else:
-        logger.warning(
-            f"The column {column_BEFL_gesp_pm} doesn't exist, so this part of the code was skipped!"
-        )
-
-    # Set classes with very few elements to IGNORE_NOT_ENOUGH_SAMPLES!
-    for _, row in (
-        parceldata_df.groupby(column_output_class)
-        .size()
-        .reset_index(name="count")
-        .iterrows()
-    ):
-        if row["count"] <= 50:
-            logger.info(
-                f"Class <{row[column_output_class]}> only contains {row['count']} elements, so put them to IGNORE_NOT_ENOUGH_SAMPLES"
-            )
-            parceldata_df.loc[
-                parceldata_df[column_output_class] == row[column_output_class],
-                column_output_class,
-            ] = "IGNORE_NOT_ENOUGH_SAMPLES"
-
-    # Drop the columns that aren't useful at all
-    for column in parceldata_df.columns:
-        if (
-            column
-            not in [
-                column_output_class,
-                conf.columns["id"],
-                conf.columns["class_groundtruth"],
-                conf.columns["class_declared"],
-            ]
-            and column not in conf.preprocess.getlist("extra_export_columns")
-            and column not in columns_BEFL_to_keep
-        ):
-            parceldata_df.drop(column, axis=1, inplace=True)
-        elif column == column_BEFL_gesp_pm:
-            parceldata_df[column_BEFL_gesp_pm] = parceldata_df[
-                column_BEFL_gesp_pm
-            ].str.replace(",", ";")
-
-    return parceldata_df
-
-
-def prepare_input_cropgroup_early(
-    parceldata_df,
-    column_BEFL_cropcode: str,
-    column_output_class: str,
-    classes_refe_path: Path,
-):
-    """
-    Prepare a dataframe based on the BEFL input file so it onclused a classname
-    column ready to classify the cropgroups for early crops.
-    """
-    # First run the standard landcover prepare
-    parceldata_df = prepare_input_cropgroup(
-        parceldata_df, column_BEFL_cropcode, column_output_class, classes_refe_path
-    )
-
-    # Set late crops to ignore
-    parceldata_df.loc[
-        parceldata_df[column_BEFL_earlylate] != "MON_TEELTEN_VROEGE",
-        column_output_class,
-    ] = "IGNORE_LATE_CROP"
-
-    # Set new grass to ignore
-    if column_BEFL_status_perm_grass in parceldata_df.columns:
-        parceldata_df.loc[
-            (parceldata_df[column_BEFL_cropcode] == "60")
-            & (
-                (parceldata_df[column_BEFL_status_perm_grass] == "BG1")
-                | (parceldata_df[column_BEFL_status_perm_grass].isnull())
-            ),
-            column_output_class,
-        ] = "IGNORE_NEW_GRASSLAND"
-    else:
-        logger.warning(
-            f"Source file doesn't contain column {column_BEFL_status_perm_grass}!"
-        )
-
-    return parceldata_df
-
-
-def prepare_input_landcover(
-    parceldata_df,
-    column_BEFL_cropcode: str,
-    column_output_class: str,
-    classes_refe_path: Path,
-):
-    """
-    This function creates a file that is compliant with the assumptions used by the rest of the
-    classification functionality.
-
-    It should be a csv file with the following columns:
-        - object_id: column with a unique identifier
-        - classname: a string column with a readable name of the classes that will be classified to
-
-    This specific implementation converts the typiscal export format used in BE-Flanders to
-    this format.
-    """
-    # Check if parameters are OK and init some extra params
-    # --------------------------------------------------------------------------
-    if not classes_refe_path.exists():
-        raise Exception(f"Input classes file doesn't exist: {classes_refe_path}")
-
-    # Convert the crop to unicode, in case the input is int...
-    if column_BEFL_cropcode in parceldata_df.columns:
-        parceldata_df[column_BEFL_cropcode] = parceldata_df[
-            column_BEFL_cropcode
-        ].astype("unicode")
-
-    # Read and cleanup the mapping table from crop codes to classes
-    # --------------------------------------------------------------------------
-    logger.info(f"Read classes conversion table from {classes_refe_path}")
-    classes_df = pdh.read_file(classes_refe_path)
-    logger.info(f"Read classes conversion table ready, info(): {classes_df.info()}")
-
-    # Because the file was read as ansi, and gewas is int, so the data needs to be converted to
-    # unicode to be able to do comparisons with the other data
-    classes_df[column_BEFL_cropcode] = classes_df["CROPCODE"].astype("unicode")
-
-    # Map column MON_group to orig classname
-    column_output_class_orig = column_output_class + "_orig"
-    classes_df[column_output_class_orig] = classes_df[conf.columns["class_refe"]]
-
-    # Remove unneeded columns
-    for column in classes_df.columns:
-        if (
-            column not in [column_output_class_orig, column_BEFL_cropcode]
-            and column not in columns_BEFL_to_keep
-        ):
-            classes_df.drop(column, axis=1, inplace=True)
-
-    # Set the index
-    classes_df.set_index(column_BEFL_cropcode, inplace=True, verify_integrity=True)
-
-    # Get only the columns in the classes_df that don't exist yet in parceldata_df
-    cols_to_join = classes_df.columns.difference(parceldata_df.columns)
-
-    # Join/merge the classname
-    logger.info("Add the classes to the parceldata")
-    parceldata_df = parceldata_df.merge(
-        classes_df[cols_to_join],
-        how="left",
-        left_on=column_BEFL_cropcode,
-        right_index=True,
-        validate="many_to_one",
-    )
-
-    # Copy orig classname to classification classname
-    parceldata_df.insert(
-        loc=0, column=column_output_class, value=parceldata_df[column_output_class_orig]
-    )
-
-    # If a column with extra info exists, use it as well to fine-tune the classification classes.
-    if column_BEFL_gesp_pm in parceldata_df.columns:
-        # Serres, tijdelijke overkappingen en loodsen
-        parceldata_df.loc[
-            parceldata_df[column_BEFL_gesp_pm].isin(
-                ["SER", "PLA", "PLO", "SGM", "NPO", "LOO"]
-            ),
-            column_output_class,
-        ] = "MON_LC_OVERK_LOO"
-        # Containers
-        parceldata_df.loc[
-            parceldata_df[column_BEFL_gesp_pm].isin(["CON"]), column_output_class
-        ] = "MON_LC_IGNORE_DIFFICULT_PERMANENT_CLASS_NS"
-        # TODO: CIV, containers in volle grond, lijkt niet zo specifiek te zijn...
-        # parceldata_df.loc[parceldata_df[column_BEFL_gesp_pm] == 'CIV', class_columnname] = 'MON_CONTAINERS'   # Containers, niet op volle grond...
-    else:
-        logger.warning(
-            f"The column {column_BEFL_gesp_pm} doesn't exist, so this part of the code was skipped!"
-        )
-
-    # Some extra cleanup: classes starting with 'nvt' or empty ones
-    logger.info(
-        "Set classes that are still empty, not specific enough or that contain to little values to 'UNKNOWN'"
-    )
-    parceldata_df.loc[
-        parceldata_df[column_output_class].str.startswith("nvt", na=True),
-        column_output_class,
-    ] = "MON_LC_UNKNOWN"
-
-    # Drop the columns that aren't useful at all
-    for column in parceldata_df.columns:
-        if (
-            column
-            not in [
-                column_output_class,
-                conf.columns["id"],
-                conf.columns["class_groundtruth"],
-                conf.columns["class_declared"],
-            ]
-            and column not in conf.preprocess.getlist("extra_export_columns")
-            and column not in columns_BEFL_to_keep
-        ):
-            parceldata_df.drop(column, axis=1, inplace=True)
-        elif column == column_BEFL_gesp_pm:
-            parceldata_df[column_BEFL_gesp_pm] = parceldata_df[
-                column_BEFL_gesp_pm
-            ].str.replace(",", ";")
-
-    return parceldata_df
-
-
-def prepare_input_landcover_early(
-    parceldata_df,
-    column_BEFL_cropcode: str,
-    column_output_class: str,
-    classes_refe_path: Path,
-):
-    """
-    Prepare a dataframe based on the BEFL input file so it onclused a classname
-    column ready to classify the landcover for early crops.
-    """
-    # First run the standard landcover prepare
-    parceldata_df = prepare_input_landcover(
-        parceldata_df, column_BEFL_cropcode, column_output_class, classes_refe_path
-    )
-
-    # Set crops not in early crops to ignore
-    parceldata_df.loc[
-        parceldata_df[column_BEFL_earlylate] != "MON_TEELTEN_VROEGE",
-        column_output_class,
-    ] = "IGNORE_LATE_CROP"
-
-    # Set new grass to ignore
-    if column_BEFL_status_perm_grass in parceldata_df.columns:
-        parceldata_df.loc[
-            (parceldata_df[column_BEFL_cropcode] == "60")
-            & (
-                (parceldata_df[column_BEFL_status_perm_grass] == "BG1")
-                | (parceldata_df[column_BEFL_status_perm_grass].isnull())
-            ),
-            column_output_class,
-        ] = "IGNORE_NEW_GRASSLAND"
-    else:
-        logger.warning(
-            f"Source file doesn't contain column {column_BEFL_status_perm_grass}, so new grassland cannot be ignored!"
-        )
-
-    return parceldata_df
-
-
-def prepare_input_most_popular_crop(
-    parceldata_df,
-    column_BEFL_cropcode: str,
-    column_output_class: str,
-    classes_refe_path: Path,
-):
-    """
-    This function creates a file that is compliant with the assumptions used by the rest of the
-    classification functionality.
-
-    It should be a csv file with the following columns:
-        - object_id: column with a unique identifier
-        - classname: a string column with a readable name of the classes that will be classified to
-
-    This specific implementation converts the typiscal export format used in BE-Flanders to this
-    format.
-    """
-
-    # Add columns for the class to use...
-    parceldata_df.insert(0, column_output_class, None)
-
-    parceldata_df.loc[
-        parceldata_df[column_BEFL_cropcode].isin(["60", "700", "3432"]),
-        column_output_class,
-    ] = "Grassland"  # Grassland
-    parceldata_df.loc[
-        parceldata_df[column_BEFL_cropcode].isin(["201", "202"]), column_output_class
-    ] = "Maize"  # Maize
-    parceldata_df.loc[
-        parceldata_df[column_BEFL_cropcode].isin(["901", "904"]), column_output_class
-    ] = "Potatoes"  # Potatoes
-    parceldata_df.loc[
-        parceldata_df[column_BEFL_cropcode].isin(["311", "36"]), column_output_class
-    ] = "WinterWheat"  # Winter wheat of spelt
-    parceldata_df.loc[
-        parceldata_df[column_BEFL_cropcode].isin(["91"]), column_output_class
-    ] = "SugarBeat"  # Sugar beat
-    parceldata_df.loc[
-        parceldata_df[column_BEFL_cropcode].isin(["321"]), column_output_class
-    ] = "WinterBarley"  # Winter barley
-    parceldata_df.loc[
-        parceldata_df[column_BEFL_cropcode].isin(["71"]), column_output_class
-    ] = "FodderBeat"  # Fodder beat
-
-    # Some extra cleanup: classes starting with 'nvt' or empty ones
-    logger.info(
-        "Set classes that are empty to 'IGNORE_UNIMPORTANT_CLASS' so they are ignored further on..."
-    )
-    parceldata_df.loc[
-        parceldata_df[column_output_class].isnull(), column_output_class
-    ] = "IGNORE_UNIMPORTANT_CLASS"
-
-    # Drop the columns that aren't useful at all
-    for column in parceldata_df.columns:
-        if (
-            column not in [conf.columns["id"], column_output_class]
-            and column not in conf.preprocess.getlist("extra_export_columns")
-            and column not in columns_BEFL_to_keep
-            and not column == column_BEFL_cropcode
-        ):
-            parceldata_df.drop(column, axis=1, inplace=True)
-        elif column == column_BEFL_gesp_pm:
-            parceldata_df[column_BEFL_gesp_pm] = parceldata_df[
-                column_BEFL_gesp_pm
-            ].str.replace(",", ";")
-
-    # Return result
-    return parceldata_df
-
-
-# If the script is run directly...
-if __name__ == "__main__":
-
-    logger.critical("Not implemented exception!")
-    raise Exception("Not implemented")
+# -*- coding: utf-8 -*-
+"""
+Create the parcel classes that will be used for the classification.
+
+This implementation will create +- 40 classes.
+parcel that don't have a clear classification in the input file get class 'UNKNOWN'.
+"""
+
+import logging
+from pathlib import Path
+
+import geofileops as gfo
+
+import cropclassification.helpers.config_helper as conf
+import cropclassification.helpers.pandas_helper as pdh
+
+# Get a logger...
+logger = logging.getLogger(__name__)
+
+# define some specific BEFL column names
+column_BEFL_earlylate = "MON_EARLY_LATE"  # Is it an early or a late crop?
+column_BEFL_gesp_pm = "GESP_PM"  # Gespecialiseerde productiemethode
+column_BEFL_gis_area = "GRAF_OPP"  # GIS Area
+column_BEFL_status_perm_grass = "STAT_BGV"  # Status permanent grassland
+column_BEFL_crop = "GWSCOD_H"
+column_BEFL_crop_declared = "GWSCOD_H_A"
+column_BEFL_crop_gt_verified = "HOOFDTEELT_CTRL_COD"
+column_BEFL_crop_gt_unverified = "HOOFDTEELT_CTRL_COD_ORIG"
+column_BEFL_latecrop = "GWSCOD_N"
+
+# BEFL specific columns we want keep
+columns_BEFL_to_keep = [
+    column_BEFL_earlylate,
+    column_BEFL_gesp_pm,
+    column_BEFL_gis_area,
+    column_BEFL_status_perm_grass,
+    column_BEFL_crop_gt_verified,
+    column_BEFL_crop_gt_unverified,
+    column_BEFL_crop,
+    column_BEFL_crop_declared,
+    column_BEFL_latecrop,
+]
+
+# -------------------------------------------------------------
+# The real work
+# -------------------------------------------------------------
+
+
+def prepare_input(
+    input_parcel_path: Path,
+    classtype_to_prepare: str,
+    classes_refe_path: Path,
+    output_dir: Path,
+):
+    """
+    This function creates a file that is compliant with the assumptions used by the rest
+    of the classification functionality.
+
+    It should be a csv file with the following columns:
+        - object_id: column with a unique identifier
+        - classname: a string column with a readable name of the classes that will be
+          classified to
+    """
+    # Check if input parameters are OK
+    if not input_parcel_path.exists():
+        raise Exception(f"Input file doesn't exist: {input_parcel_path}")
+    else:
+        logger.info(f"Process input file {input_parcel_path}")
+
+    # Read input file
+    logger.info(f"Read parceldata from {input_parcel_path}")
+    if gfo.is_geofile(input_parcel_path):
+        parceldata_df = gfo.read_file(input_parcel_path)
+    else:
+        parceldata_df = pdh.read_file(input_parcel_path)
+    logger.info(f"Read Parceldata ready, info(): {parceldata_df.info()}")
+
+    # Check if the id column is present...
+    if conf.columns["id"] not in parceldata_df.columns:
+        message = (
+            f"Column {conf.columns['id']} not found in input parcel file: "
+            f"{input_parcel_path}. Make sure the column is present or change the "
+            "column name in global_constants.py"
+        )
+        logger.critical(message)
+        raise Exception(message)
+
+    # Now start prepare
+    if classtype_to_prepare == "CROPGROUP":
+        parceldata_df = prepare_input_cropgroup(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop_declared,
+            column_output_class=conf.columns["class_declared"],
+            classes_refe_path=classes_refe_path,
+        )
+        return prepare_input_cropgroup(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop,
+            column_output_class=conf.columns["class"],
+            classes_refe_path=classes_refe_path,
+        )
+    elif classtype_to_prepare == "CROPGROUP-GROUNDTRUTH":
+        return prepare_input_cropgroup(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop_gt_verified,
+            column_output_class=conf.columns["class_groundtruth"],
+            classes_refe_path=classes_refe_path,
+        )
+    elif classtype_to_prepare == "CROPGROUP-EARLY":
+        parceldata_df = prepare_input_cropgroup_early(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop_declared,
+            column_output_class=conf.columns["class_declared"],
+            classes_refe_path=classes_refe_path,
+        )
+        return prepare_input_cropgroup_early(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop,
+            column_output_class=conf.columns["class"],
+            classes_refe_path=classes_refe_path,
+        )
+    elif classtype_to_prepare == "CROPGROUP-EARLY-GROUNDTRUTH":
+        return prepare_input_cropgroup_early(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop_gt_verified,
+            column_output_class=conf.columns["class_groundtruth"],
+            classes_refe_path=classes_refe_path,
+        )
+    elif classtype_to_prepare == "LANDCOVER":
+        parceldata_df = prepare_input_landcover(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop_declared,
+            column_output_class=conf.columns["class_declared"],
+            classes_refe_path=classes_refe_path,
+        )
+        return prepare_input_landcover(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop,
+            column_output_class=conf.columns["class"],
+            classes_refe_path=classes_refe_path,
+        )
+    elif classtype_to_prepare == "MULTICROP":
+        parceldata_df = prepare_input_landcover(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop_declared,
+            column_output_class=conf.columns["class_declared"],
+            classes_refe_path=classes_refe_path,
+        )
+        return prepare_input_landcover(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop,
+            column_output_class=conf.columns["class"],
+            classes_refe_path=classes_refe_path,
+        )
+    elif classtype_to_prepare == "LANDCOVER-GROUNDTRUTH":
+        return prepare_input_landcover(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop_gt_verified,
+            column_output_class=conf.columns["class_groundtruth"],
+            classes_refe_path=classes_refe_path,
+        )
+    elif classtype_to_prepare == "LANDCOVER-EARLY":
+        parceldata_df = prepare_input_landcover_early(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop_declared,
+            column_output_class=conf.columns["class_declared"],
+            classes_refe_path=classes_refe_path,
+        )
+        return prepare_input_landcover_early(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop,
+            column_output_class=conf.columns["class"],
+            classes_refe_path=classes_refe_path,
+        )
+    elif classtype_to_prepare == "LANDCOVER-EARLY-GROUNDTRUTH":
+        return prepare_input_landcover_early(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop_gt_verified,
+            column_output_class=conf.columns["class_groundtruth"],
+            classes_refe_path=classes_refe_path,
+        )
+    elif classtype_to_prepare == "POPULAR-CROP":
+        parceldata_df = prepare_input_most_popular_crop(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop_declared,
+            column_output_class=conf.columns["class_declared"],
+            classes_refe_path=classes_refe_path,
+        )
+        return prepare_input_most_popular_crop(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop,
+            column_output_class=conf.columns["class"],
+            classes_refe_path=classes_refe_path,
+        )
+    elif classtype_to_prepare == "POPULAR-CROP-GROUNDTRUTH":
+        return prepare_input_most_popular_crop(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop_gt_verified,
+            column_output_class=conf.columns["class_groundtruth"],
+            classes_refe_path=classes_refe_path,
+        )
+    elif classtype_to_prepare == "LATECROP":
+        parceldata_df = prepare_input_latecrop(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_latecrop,
+            column_output_class=conf.columns["class_declared"],
+            classes_refe_path=classes_refe_path,
+        )
+        return prepare_input_latecrop(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_latecrop,
+            column_output_class=conf.columns["class"],
+            classes_refe_path=classes_refe_path,
+        )
+    elif classtype_to_prepare == "FABACEAE":
+        parceldata_df = prepare_input_fabaceae(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop,
+            column_output_class=conf.columns["class_declared"],
+            classes_refe_path=classes_refe_path,
+        )
+        return prepare_input_fabaceae(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop,
+            column_output_class=conf.columns["class"],
+            classes_refe_path=classes_refe_path,
+        )
+    elif classtype_to_prepare == "FABACEAE-GROUNDTRUTH":
+        return prepare_input_fabaceae(
+            parceldata_df=parceldata_df,
+            column_BEFL_cropcode=column_BEFL_crop_gt_verified,
+            column_output_class=conf.columns["class_groundtruth"],
+            classes_refe_path=classes_refe_path,
+        )
+    else:
+        message = (
+            f"Unknown value for parameter classtype_to_prepare: {classtype_to_prepare}"
+        )
+        logger.critical(message)
+        raise Exception(message)
+
+
+def prepare_input_cropgroup(
+    parceldata_df,
+    column_BEFL_cropcode: str,
+    column_output_class: str,
+    classes_refe_path: Path,
+):
+    """
+    This function creates a file that is compliant with the assumptions used by the rest
+    of the classification functionality.
+
+    It should be a csv file with the following columns:
+        - object_id: column with a unique identifier
+        - classname: a string column with a readable name of the classes that will be
+          classified to
+
+    This specific implementation converts the typiscal export format used in BE-Flanders
+    to this format.
+    """
+    # Check if parameters are OK and init some extra params
+    # --------------------------------------------------------------------------
+    if not classes_refe_path.exists():
+        raise Exception(f"Input classes file doesn't exist: {classes_refe_path}")
+
+    # Convert the crop to unicode, in case the input is int...
+    if column_BEFL_cropcode in parceldata_df.columns:
+        parceldata_df[column_BEFL_cropcode] = parceldata_df[
+            column_BEFL_cropcode
+        ].astype("unicode")
+
+    # Read and cleanup the mapping table from crop codes to classes
+    # --------------------------------------------------------------------------
+    logger.info(f"Read classes conversion table from {classes_refe_path}")
+    classes_df = pdh.read_file(classes_refe_path)
+    logger.info(f"Read classes conversion table ready, info(): {classes_df.info()}")
+
+    # Because the file was read as ansi, and gewas is int, so the data needs to be
+    # converted to unicode to be able to do comparisons with the other data
+    classes_df[column_BEFL_cropcode] = classes_df["CROPCODE"].astype("unicode")
+
+    # Map column with the classname to orig classname
+    column_output_class_orig = conf.columns["class"] + "_orig"
+    classes_df[column_output_class_orig] = classes_df[conf.columns["class_refe"]]
+
+    # Remove unneeded columns
+    for column in classes_df.columns:
+        if (
+            column not in [column_output_class_orig, column_BEFL_cropcode]
+            and column not in columns_BEFL_to_keep
+        ):
+            classes_df.drop(column, axis=1, inplace=True)
+
+    # Set the index
+    classes_df.set_index(column_BEFL_cropcode, inplace=True, verify_integrity=True)
+
+    # Get only the columns in the classes_df that don't exist yet in parceldata_df
+    cols_to_join = classes_df.columns.difference(parceldata_df.columns)
+
+    # Join/merge the classname
+    logger.info("Add the classes to the parceldata")
+    parceldata_df = parceldata_df.merge(
+        classes_df[cols_to_join],
+        how="left",
+        left_on=column_BEFL_cropcode,
+        right_index=True,
+        validate="many_to_one",
+    )
+
+    # Copy orig classname to classification classname
+    parceldata_df.insert(
+        loc=0, column=column_output_class, value=parceldata_df[column_output_class_orig]
+    )
+
+    # For rows with no class, set to UNKNOWN
+    parceldata_df.fillna(value={column_output_class: "UNKNOWN"}, inplace=True)
+
+    # If a column with extra info exists, use it as well to fine-tune the classification
+    # classes.
+    if column_BEFL_gesp_pm in parceldata_df.columns:
+        # Serres, tijdelijke overkappingen en loodsen
+        parceldata_df.loc[
+            parceldata_df[column_BEFL_gesp_pm].isin(["SER", "SGM"]), column_output_class
+        ] = "MON_OVERK_LOO"
+        parceldata_df.loc[
+            parceldata_df[column_BEFL_gesp_pm].isin(["PLA", "PLO", "NPO"]),
+            column_output_class,
+        ] = "MON_OVERK_LOO"
+        parceldata_df.loc[
+            parceldata_df[column_BEFL_gesp_pm] == "LOO", column_output_class
+        ] = "MON_OVERK_LOO"  # Een loods is hetzelfde als een stal...
+        parceldata_df.loc[
+            parceldata_df[column_BEFL_gesp_pm] == "CON", column_output_class
+        ] = "MON_CONTAINERS"  # Containers, niet op volle grond...
+        # TODO: CIV, containers in volle grond, lijkt niet zo specifiek te zijn...
+        # parceldata_df.loc[
+        #     parceldata_df[column_BEFL_gesp_pm] == 'CIV', class_columnname
+        # ] = 'MON_CONTAINERS'   # Containers, niet op volle grond...
+    else:
+        logger.warning(
+            f"The column {column_BEFL_gesp_pm} doesn't exist, so this part of the code "
+            "was skipped!"
+        )
+
+    # Some extra cleanup: classes starting with 'nvt' or empty ones
+    # logger.info(
+    #     "Set classes that are still empty, not specific enough or that contain to "
+    #     "little values to 'UNKNOWN'"
+    # )
+    # parceldata_df.loc[
+    #     parceldata_df[column_output_class].str.startswith('nvt', na=True),
+    #     column_output_class
+    # ] = 'UNKNOWN'
+
+    # 'MON_ANDERE_SUBSID_GEWASSEN': very low classification rate (< 1%), as it is a
+    #      group with several very different classes in it
+    # 'MON_AARDBEIEN': low classification rate (~10%), as many parcel actually are
+    #      temporary greenhouses but aren't correctly applied
+    # 'MON_BRAAK': very low classification rate (< 1%), spread over a lot of classes,
+    #      but most popular are MON_BOOM, MON_GRASSEN, MON_FRUIT
+    # 'MON_KLAVER': log classification rate (25%), spread over quite some classes, but
+    #      MON GRASSES has 20% as well.
+    # 'MON_MENGSEL': 25% correct classifications: rest spread over many other classes.
+    #      Too heterogenous in group?
+    # 'MON_POEL': 0% correct classifications: most are classified as MON_CONTAINER,
+    #      MON_FRUIT. Almost nothing was misclassified as being POEL
+    # 'MON_RAAPACHTIGEN': 25% correct classifications: rest spread over many other
+    #      classes
+    # 'MON_STRUIK': 10%
+    #    TODO: nakijken, wss opsplitsen of toevoegen aan MON_BOOMKWEEK???
+    # classes_badresults = [
+    #     'MON_ANDERE_SUBSID_GEWASSEN', 'MON_AARDBEIEN', 'MON_BRAAK', 'MON_KLAVER',
+    #     'MON_MENGSEL', 'MON_POEL', 'MON_RAAPACHTIGEN', 'MON_STRUIK'
+    # ]
+    # parceldata_df.loc[
+    #     parceldata_df[column_output_class].isin(classes_badresults),
+    #     column_output_class
+    # ] = 'UNKNOWN'
+
+    # MON_BONEN en MON_WIKKEN have omongst each other a very large percentage of false
+    # positives/negatives, so they seem very similar... lets create a class that
+    # combines both
+    # parceldata_df.loc[parceldata_df[
+    #     column_output_class].isin(['MON_BONEN', 'MON_WIKKEN']),
+    #     column_output_class
+    # ] = 'MON_BONEN_WIKKEN'
+
+    # MON_BOOM includes now also the growing new plants/trees, which is too differenct
+    # from grown trees -> put growing new trees is seperate group
+    # parceldata_df.loc[parceldata_df[
+    #     column_BEFL_cropcode].isin(['9602', '9603', '9604', '9560']),
+    #     column_output_class
+    # ] = 'MON_BOOMKWEEK'
+
+    # 'MON_FRUIT': has a good accuracy (91%), but also has as much false positives
+    #     (115% -> mainly 'MON_GRASSEN' that are (mis)classified as 'MON_FRUIT')
+    # 'MON_BOOM': has very bad accuracy (28%) and also very much false positives
+    #     (450% -> mainly 'MON_GRASSEN' that are misclassified as 'MON_BOOM')
+    # MON_FRUIT and MON_BOOM are permanent anyway, so not mandatory that they are
+    # checked in monitoring process.
+    # Conclusion: put MON_BOOM and MON_FRUIT to IGNORE_DIFFICULT_PERMANENT_CLASS
+    # parceldata_df.loc[parceldata_df[
+    #     column_output_class].isin(['MON_BOOM', 'MON_FRUIT']),
+    #     column_output_class
+    # ] = 'IGNORE_DIFFICULT_PERMANENT_CLASS'
+
+    # Set classes with very few elements to IGNORE_NOT_ENOUGH_SAMPLES!
+    for _, row in (
+        parceldata_df.groupby(column_output_class)
+        .size()
+        .reset_index(name="count")
+        .iterrows()
+    ):
+        if row["count"] <= 50:
+            logger.info(
+                f"Class <{row[column_output_class]}> only contains {row['count']} "
+                "elements, so put them to IGNORE_NOT_ENOUGH_SAMPLES"
+            )
+            parceldata_df.loc[
+                parceldata_df[column_output_class] == row[column_output_class],
+                column_output_class,
+            ] = "IGNORE_NOT_ENOUGH_SAMPLES"
+
+    # Drop the columns that aren't useful at all
+    for column in parceldata_df.columns:
+        if (
+            column
+            not in [
+                column_output_class,
+                conf.columns["id"],
+                conf.columns["class_groundtruth"],
+                conf.columns["class_declared"],
+            ]
+            and column not in conf.preprocess.getlist("extra_export_columns")
+            and column not in columns_BEFL_to_keep
+        ):
+            parceldata_df.drop(column, axis=1, inplace=True)
+        elif column == column_BEFL_gesp_pm:
+            parceldata_df[column_BEFL_gesp_pm] = parceldata_df[
+                column_BEFL_gesp_pm
+            ].str.replace(",", ";")
+
+    return parceldata_df
+
+
+def prepare_input_fabaceae(
+    parceldata_df,
+    column_BEFL_cropcode: str,
+    column_output_class: str,
+    classes_refe_path: Path,
+):
+    """
+    This function creates a file that is compliant with the assumptions used by the rest
+    of the classification functionality.
+
+    It should be a csv file with the following columns:
+        - object_id: column with a unique identifier
+        - classname: a string column with a readable name of the classes that will be
+          classified to
+
+    This specific implementation converts the typiscal export format used in BE-Flanders
+    to this format.
+    """
+    # Check if parameters are OK and init some extra params
+    # --------------------------------------------------------------------------
+    if not classes_refe_path.exists():
+        raise Exception(f"Input classes file doesn't exist: {classes_refe_path}")
+
+    # Convert the crop to unicode, in case the input is int...
+    if column_BEFL_cropcode in parceldata_df.columns:
+        parceldata_df[column_BEFL_cropcode] = parceldata_df[
+            column_BEFL_cropcode
+        ].astype("unicode")
+
+    # Read and cleanup the mapping table from crop codes to classes
+    # --------------------------------------------------------------------------
+    logger.info(f"Read classes conversion table from {classes_refe_path}")
+    classes_df = pdh.read_file(classes_refe_path)
+    logger.info(f"Read classes conversion table ready, info(): {classes_df.info()}")
+
+    # Because the file was read as ansi, and gewas is int, so the data needs to be
+    # converted to unicode to be able to do comparisons with the other data
+    classes_df[column_BEFL_cropcode] = classes_df["CROPCODE"].astype("unicode")
+
+    # Map column with the classname to orig classname
+    column_output_class_orig = conf.columns["class"] + "_orig"
+    classes_df[column_output_class_orig] = classes_df[conf.columns["class_refe"]]
+
+    # Remove unneeded columns
+    for column in classes_df.columns:
+        if (
+            column not in [column_output_class_orig, column_BEFL_cropcode]
+            and column not in columns_BEFL_to_keep
+        ):
+            classes_df.drop(column, axis=1, inplace=True)
+
+    # Set the index
+    classes_df.set_index(column_BEFL_cropcode, inplace=True, verify_integrity=True)
+
+    # Get only the columns in the classes_df that don't exist yet in parceldata_df
+    cols_to_join = classes_df.columns.difference(parceldata_df.columns)
+
+    # Filter the parcels to only keep the classes we are interested in
+    # TODO: this shouldn't be hardcoded!
+    parceldata_df = parceldata_df.loc[
+        parceldata_df[column_BEFL_cropcode].isin(["60", "700", "660", "732", "723"])
+    ]
+
+    # Join/merge the classname
+    logger.info("Add the classes to the parceldata")
+    parceldata_df = parceldata_df.merge(
+        classes_df[cols_to_join],
+        how="left",
+        left_on=column_BEFL_cropcode,
+        right_index=True,
+        validate="many_to_one",
+    )
+
+    # Copy orig classname to classification classname
+    parceldata_df.insert(
+        loc=0, column=column_output_class, value=parceldata_df[column_output_class_orig]
+    )
+
+    # For rows with no class, set to UNKNOWN
+    parceldata_df.fillna(value={column_output_class: "UNKNOWN"}, inplace=True)
+
+    # If a column with extra info exists, use it as well to fine-tune the classification
+    # classes.
+    if column_BEFL_gesp_pm in parceldata_df.columns:
+        # Serres, tijdelijke overkappingen en loodsen
+        parceldata_df.loc[
+            parceldata_df[column_BEFL_gesp_pm].isin(["SER", "SGM"]), column_output_class
+        ] = "MON_OVERK_LOO"
+        parceldata_df.loc[
+            parceldata_df[column_BEFL_gesp_pm].isin(["PLA", "PLO", "NPO"]),
+            column_output_class,
+        ] = "MON_OVERK_LOO"
+        parceldata_df.loc[
+            parceldata_df[column_BEFL_gesp_pm] == "LOO", column_output_class
+        ] = "MON_OVERK_LOO"  # Een loods is hetzelfde als een stal...
+        parceldata_df.loc[
+            parceldata_df[column_BEFL_gesp_pm] == "CON", column_output_class
+        ] = "MON_CONTAINERS"  # Containers, niet op volle grond...
+        # TODO: CIV, containers in volle grond, lijkt niet zo specifiek te zijn...
+        # parceldata_df.loc[
+        #     parceldata_df[column_BEFL_gesp_pm] == 'CIV', class_columnname
+        # ] = 'MON_CONTAINERS'   # Containers, niet op volle grond...
+    else:
+        logger.warning(
+            f"The column {column_BEFL_gesp_pm} doesn't exist, so this part of the code "
+            "was skipped!"
+        )
+
+    # Some extra cleanup: classes starting with 'nvt' or empty ones
+    # logger.info(
+    #     "Set classes that are still empty, not specific enough or that contain to "
+    #     "little values to 'UNKNOWN'"
+    # )
+    # parceldata_df.loc[
+    #     parceldata_df[column_output_class].str.startswith('nvt', na=True),
+    #     column_output_class
+    # ] = 'UNKNOWN'
+
+    # 'MON_ANDERE_SUBSID_GEWASSEN': very low classification rate (< 1%), as it is a
+    #     group with several very different classes in it
+    # 'MON_AARDBEIEN': low classification rate (~10%), as many parcel actually are
+    #     temporary greenhouses but aren't correctly applied
+    # 'MON_BRAAK': very low classification rate (< 1%), spread over a lot of classes,
+    #     but most popular are MON_BOOM, MON_GRASSEN, MON_FRUIT
+    # 'MON_KLAVER': log classification rate (25%), spread over quite some classes, but
+    #     MON GRASSES has 20% as well.
+    # 'MON_MENGSEL': 25% correct classifications: rest spread over many other classes.
+    #     Too heterogenous in group?
+    # 'MON_POEL': 0% correct classifications: most are classified as MON_CONTAINER,
+    #     MON_FRUIT. Almost nothing was misclassified as being POEL
+    # 'MON_RAAPACHTIGEN': 25% correct classifications: rest spread over many other
+    #     classes
+    # 'MON_STRUIK': 10%
+    #    TODO: nakijken, wss opsplitsen of toevoegen aan MON_BOOMKWEEK???
+    # classes_badresults = [
+    #     'MON_ANDERE_SUBSID_GEWASSEN', 'MON_AARDBEIEN', 'MON_BRAAK', 'MON_KLAVER',
+    #     'MON_MENGSEL', 'MON_POEL', 'MON_RAAPACHTIGEN', 'MON_STRUIK'
+    # ]
+    # parceldata_df.loc[parceldata_df[column_output_class].isin(classes_badresults),
+    #                  column_output_class] = 'UNKNOWN'
+
+    # MON_BONEN en MON_WIKKEN have omongst each other a very large percentage of false
+    # positives/negatives, so they seem very similar... lets create a class that
+    # combines both
+    # parceldata_df.loc[
+    #     parceldata_df[column_output_class].isin(['MON_BONEN', 'MON_WIKKEN']),
+    #     column_output_class
+    # ] = 'MON_BONEN_WIKKEN'
+
+    # MON_BOOM includes now also the growing new plants/trees, which is too differenct
+    # from grown trees -> put growing new trees is seperate group
+    # parceldata_df.loc[
+    #     parceldata_df[column_BEFL_cropcode].isin(['9602', '9603', '9604', '9560']),
+    #     column_output_class
+    # ] = 'MON_BOOMKWEEK'
+
+    # 'MON_FRUIT': has a good accuracy (91%), but also has as much false positives
+    #     (115% -> mainly 'MON_GRASSEN' that are (mis)classified as 'MON_FRUIT')
+    # 'MON_BOOM': has very bad accuracy (28%) and also very much false positives
+    #     (450% -> mainly 'MON_GRASSEN' that are misclassified as 'MON_BOOM')
+    # MON_FRUIT and MON_BOOM are permanent anyway, so not mandatory that they are
+    # checked in monitoring process.
+    # Conclusion: put MON_BOOM and MON_FRUIT to IGNORE_DIFFICULT_PERMANENT_CLASS
+    # parceldata_df.loc[
+    #     parceldata_df[column_output_class].isin(['MON_BOOM', 'MON_FRUIT']),
+    #     column_output_class
+    # ] = 'IGNORE_DIFFICULT_PERMANENT_CLASS'
+
+    # Set classes with very few elements to IGNORE_NOT_ENOUGH_SAMPLES!
+    for _, row in (
+        parceldata_df.groupby(column_output_class)
+        .size()
+        .reset_index(name="count")
+        .iterrows()
+    ):
+        if row["count"] <= 50:
+            logger.info(
+                f"Class <{row[column_output_class]}> only contains {row['count']} "
+                "elements, so put them to IGNORE_NOT_ENOUGH_SAMPLES"
+            )
+            parceldata_df.loc[
+                parceldata_df[column_output_class] == row[column_output_class],
+                column_output_class,
+            ] = "IGNORE_NOT_ENOUGH_SAMPLES"
+
+    # Drop the columns that aren't useful at all
+    for column in parceldata_df.columns:
+        if (
+            column
+            not in [
+                column_output_class,
+                conf.columns["id"],
+                conf.columns["class_groundtruth"],
+                conf.columns["class_declared"],
+            ]
+            and column not in conf.preprocess.getlist("extra_export_columns")
+            and column not in columns_BEFL_to_keep
+        ):
+            parceldata_df.drop(column, axis=1, inplace=True)
+        elif column == column_BEFL_gesp_pm:
+            parceldata_df[column_BEFL_gesp_pm] = parceldata_df[
+                column_BEFL_gesp_pm
+            ].str.replace(",", ";")
+
+    return parceldata_df
+
+
+def prepare_input_latecrop(
+    parceldata_df,
+    column_BEFL_cropcode: str,
+    column_output_class: str,
+    classes_refe_path: Path,
+):
+    """
+    This function creates a file that is compliant with the assumptions used by the rest
+    of the classification functionality.
+
+    It should be a csv file with the following columns:
+        - object_id: column with a unique identifier
+        - classname: a string column with a readable name of the classes that will be
+          classified to
+
+    This specific implementation converts the typiscal export format used in BE-Flanders
+    to this format.
+    """
+    # Check if parameters are OK and init some extra params
+    # --------------------------------------------------------------------------
+    if not classes_refe_path.exists():
+        raise Exception(f"Input classes file doesn't exist: {classes_refe_path}")
+
+    # Convert the crop to unicode, in case the input is int...
+    if column_BEFL_cropcode in parceldata_df.columns:
+        parceldata_df[column_BEFL_cropcode] = parceldata_df[
+            column_BEFL_cropcode
+        ].astype("unicode")
+
+    # Read and cleanup the mapping table from crop codes to classes
+    # --------------------------------------------------------------------------
+    logger.info(f"Read classes conversion table from {classes_refe_path}")
+    classes_df = pdh.read_file(classes_refe_path)
+    logger.info(f"Read classes conversion table ready, info(): {classes_df.info()}")
+
+    # Because the file was read as ansi, and gewas is int, so the data needs to be
+    # converted to unicode to be able to do comparisons with the other data
+    classes_df[column_BEFL_cropcode] = classes_df["CROPCODE"].astype("unicode")
+
+    # Map column with the classname to orig classname
+    column_output_class_orig = conf.columns["class"] + "_orig"
+    classes_df[column_output_class_orig] = classes_df[conf.columns["class_refe"]]
+
+    # Remove unneeded columns
+    for column in classes_df.columns:
+        if (
+            column
+            not in [
+                column_output_class_orig,
+                column_BEFL_cropcode,
+                conf.columns["class_declared"],
+                conf.columns["class"],
+            ]
+            and column not in columns_BEFL_to_keep
+        ):
+            classes_df.drop(column, axis=1, inplace=True)
+
+    # Set the index
+    classes_df.set_index(column_BEFL_cropcode, inplace=True, verify_integrity=True)
+
+    # Get only the columns in the classes_df that don't exist yet in parceldata_df
+    cols_to_join = classes_df.columns.difference(parceldata_df.columns)
+
+    # Join/merge the classname
+    logger.info("Add the classes to the parceldata")
+    parceldata_df = parceldata_df.merge(
+        classes_df[cols_to_join],
+        how="left",
+        left_on=column_BEFL_cropcode,
+        right_index=True,
+        validate="many_to_one",
+    )
+
+    # Copy orig classname to classification classname
+    parceldata_df.insert(
+        loc=0, column=column_output_class, value=parceldata_df[column_output_class_orig]
+    )
+
+    # For rows with no class, set to UNKNOWN
+    parceldata_df.fillna(value={column_output_class: "UNKNOWN"}, inplace=True)
+
+    # If a column with extra info exists, use it as well to fine-tune the classification
+    # classes.
+    if column_BEFL_gesp_pm in parceldata_df.columns:
+        # Serres, tijdelijke overkappingen en loodsen
+        parceldata_df.loc[
+            parceldata_df[column_BEFL_gesp_pm].isin(["SER", "SGM"]), column_output_class
+        ] = "MON_OVERK_LOO"
+        parceldata_df.loc[
+            parceldata_df[column_BEFL_gesp_pm].isin(["PLA", "PLO", "NPO"]),
+            column_output_class,
+        ] = "MON_OVERK_LOO"
+        parceldata_df.loc[
+            parceldata_df[column_BEFL_gesp_pm] == "LOO", column_output_class
+        ] = "MON_OVERK_LOO"  # Een loods is hetzelfde als een stal...
+        parceldata_df.loc[
+            parceldata_df[column_BEFL_gesp_pm] == "CON", column_output_class
+        ] = "MON_CONTAINERS"  # Containers, niet op volle grond...
+        # TODO: CIV, containers in volle grond, lijkt niet zo specifiek te zijn...
+        # parceldata_df.loc[
+        #     parceldata_df[column_BEFL_gesp_pm] == 'CIV', class_columnname
+        # ] = 'MON_CONTAINERS'   # Containers, niet op volle grond...
+    else:
+        logger.warning(
+            f"The column {column_BEFL_gesp_pm} doesn't exist, so this part of the code "
+            "was skipped!"
+        )
+
+    # Set classes with very few elements to IGNORE_NOT_ENOUGH_SAMPLES!
+    for _, row in (
+        parceldata_df.groupby(column_output_class)
+        .size()
+        .reset_index(name="count")
+        .iterrows()
+    ):
+        if row["count"] <= 50:
+            logger.info(
+                f"Class <{row[column_output_class]}> only contains {row['count']} "
+                "elements, so put them to IGNORE_NOT_ENOUGH_SAMPLES"
+            )
+            parceldata_df.loc[
+                parceldata_df[column_output_class] == row[column_output_class],
+                column_output_class,
+            ] = "IGNORE_NOT_ENOUGH_SAMPLES"
+
+    # Drop the columns that aren't useful at all
+    for column in parceldata_df.columns:
+        if (
+            column
+            not in [
+                column_output_class,
+                conf.columns["id"],
+                conf.columns["class_groundtruth"],
+                conf.columns["class_declared"],
+            ]
+            and column not in conf.preprocess.getlist("extra_export_columns")
+            and column not in columns_BEFL_to_keep
+        ):
+            parceldata_df.drop(column, axis=1, inplace=True)
+        elif column == column_BEFL_gesp_pm:
+            parceldata_df[column_BEFL_gesp_pm] = parceldata_df[
+                column_BEFL_gesp_pm
+            ].str.replace(",", ";")
+
+    return parceldata_df
+
+
+def prepare_input_cropgroup_early(
+    parceldata_df,
+    column_BEFL_cropcode: str,
+    column_output_class: str,
+    classes_refe_path: Path,
+):
+    """
+    Prepare a dataframe based on the BEFL input file so it onclused a classname
+    column ready to classify the cropgroups for early crops.
+    """
+    # First run the standard landcover prepare
+    parceldata_df = prepare_input_cropgroup(
+        parceldata_df, column_BEFL_cropcode, column_output_class, classes_refe_path
+    )
+
+    # Set late crops to ignore
+    parceldata_df.loc[
+        parceldata_df[column_BEFL_earlylate] != "MON_TEELTEN_VROEGE",
+        column_output_class,
+    ] = "IGNORE_LATE_CROP"
+
+    # Set new grass to ignore
+    if column_BEFL_status_perm_grass in parceldata_df.columns:
+        parceldata_df.loc[
+            (parceldata_df[column_BEFL_cropcode] == "60")
+            & (
+                (parceldata_df[column_BEFL_status_perm_grass] == "BG1")
+                | (parceldata_df[column_BEFL_status_perm_grass].isnull())
+            ),
+            column_output_class,
+        ] = "IGNORE_NEW_GRASSLAND"
+    else:
+        logger.warning(
+            f"Source file doesn't contain column {column_BEFL_status_perm_grass}!"
+        )
+
+    return parceldata_df
+
+
+def prepare_input_landcover(
+    parceldata_df,
+    column_BEFL_cropcode: str,
+    column_output_class: str,
+    classes_refe_path: Path,
+):
+    """
+    This function creates a file that is compliant with the assumptions used by the rest
+    of the classification functionality.
+
+    It should be a csv file with the following columns:
+        - object_id: column with a unique identifier
+        - classname: a string column with a readable name of the classes that will be
+          classified to
+
+    This specific implementation converts the typiscal export format used in BE-Flanders
+    to this format.
+    """
+    # Check if parameters are OK and init some extra params
+    # --------------------------------------------------------------------------
+    if not classes_refe_path.exists():
+        raise Exception(f"Input classes file doesn't exist: {classes_refe_path}")
+
+    # Convert the crop to unicode, in case the input is int...
+    if column_BEFL_cropcode in parceldata_df.columns:
+        parceldata_df[column_BEFL_cropcode] = parceldata_df[
+            column_BEFL_cropcode
+        ].astype("unicode")
+
+    # Read and cleanup the mapping table from crop codes to classes
+    # --------------------------------------------------------------------------
+    logger.info(f"Read classes conversion table from {classes_refe_path}")
+    classes_df = pdh.read_file(classes_refe_path)
+    logger.info(f"Read classes conversion table ready, info(): {classes_df.info()}")
+
+    # Because the file was read as ansi, and gewas is int, so the data needs to be
+    # converted to unicode to be able to do comparisons with the other data
+    classes_df[column_BEFL_cropcode] = classes_df["CROPCODE"].astype("unicode")
+
+    # Map column MON_group to orig classname
+    column_output_class_orig = column_output_class + "_orig"
+    classes_df[column_output_class_orig] = classes_df[conf.columns["class_refe"]]
+
+    # Remove unneeded columns
+    for column in classes_df.columns:
+        if (
+            column not in [column_output_class_orig, column_BEFL_cropcode]
+            and column not in columns_BEFL_to_keep
+        ):
+            classes_df.drop(column, axis=1, inplace=True)
+
+    # Set the index
+    classes_df.set_index(column_BEFL_cropcode, inplace=True, verify_integrity=True)
+
+    # Get only the columns in the classes_df that don't exist yet in parceldata_df
+    cols_to_join = classes_df.columns.difference(parceldata_df.columns)
+
+    # Join/merge the classname
+    logger.info("Add the classes to the parceldata")
+    parceldata_df = parceldata_df.merge(
+        classes_df[cols_to_join],
+        how="left",
+        left_on=column_BEFL_cropcode,
+        right_index=True,
+        validate="many_to_one",
+    )
+
+    # Copy orig classname to classification classname
+    parceldata_df.insert(
+        loc=0, column=column_output_class, value=parceldata_df[column_output_class_orig]
+    )
+
+    # If a column with extra info exists, use it as well to fine-tune the classification
+    # classes.
+    if column_BEFL_gesp_pm in parceldata_df.columns:
+        # Serres, tijdelijke overkappingen en loodsen
+        parceldata_df.loc[
+            parceldata_df[column_BEFL_gesp_pm].isin(
+                ["SER", "PLA", "PLO", "SGM", "NPO", "LOO"]
+            ),
+            column_output_class,
+        ] = "MON_LC_OVERK_LOO"
+        # Containers
+        parceldata_df.loc[
+            parceldata_df[column_BEFL_gesp_pm].isin(["CON"]), column_output_class
+        ] = "MON_LC_IGNORE_DIFFICULT_PERMANENT_CLASS_NS"
+        # TODO: CIV, containers in volle grond, lijkt niet zo specifiek te zijn...
+        # parceldata_df.loc[
+        #     parceldata_df[column_BEFL_gesp_pm] == 'CIV', class_columnname
+        # ] = 'MON_CONTAINERS'   # Containers, niet op volle grond...
+    else:
+        logger.warning(
+            f"The column {column_BEFL_gesp_pm} doesn't exist, so this part of the code "
+            "was skipped!"
+        )
+
+    # Some extra cleanup: classes starting with 'nvt' or empty ones
+    logger.info(
+        "Set classes that are still empty, not specific enough or that contain to "
+        "little values to 'UNKNOWN'"
+    )
+    parceldata_df.loc[
+        parceldata_df[column_output_class].str.startswith("nvt", na=True),
+        column_output_class,
+    ] = "MON_LC_UNKNOWN"
+
+    # Drop the columns that aren't useful at all
+    for column in parceldata_df.columns:
+        if (
+            column
+            not in [
+                column_output_class,
+                conf.columns["id"],
+                conf.columns["class_groundtruth"],
+                conf.columns["class_declared"],
+            ]
+            and column not in conf.preprocess.getlist("extra_export_columns")
+            and column not in columns_BEFL_to_keep
+        ):
+            parceldata_df.drop(column, axis=1, inplace=True)
+        elif column == column_BEFL_gesp_pm:
+            parceldata_df[column_BEFL_gesp_pm] = parceldata_df[
+                column_BEFL_gesp_pm
+            ].str.replace(",", ";")
+
+    return parceldata_df
+
+
+def prepare_input_landcover_early(
+    parceldata_df,
+    column_BEFL_cropcode: str,
+    column_output_class: str,
+    classes_refe_path: Path,
+):
+    """
+    Prepare a dataframe based on the BEFL input file so it onclused a classname
+    column ready to classify the landcover for early crops.
+    """
+    # First run the standard landcover prepare
+    parceldata_df = prepare_input_landcover(
+        parceldata_df, column_BEFL_cropcode, column_output_class, classes_refe_path
+    )
+
+    # Set crops not in early crops to ignore
+    parceldata_df.loc[
+        parceldata_df[column_BEFL_earlylate] != "MON_TEELTEN_VROEGE",
+        column_output_class,
+    ] = "IGNORE_LATE_CROP"
+
+    # Set new grass to ignore
+    if column_BEFL_status_perm_grass in parceldata_df.columns:
+        parceldata_df.loc[
+            (parceldata_df[column_BEFL_cropcode] == "60")
+            & (
+                (parceldata_df[column_BEFL_status_perm_grass] == "BG1")
+                | (parceldata_df[column_BEFL_status_perm_grass].isnull())
+            ),
+            column_output_class,
+        ] = "IGNORE_NEW_GRASSLAND"
+    else:
+        logger.warning(
+            f"Source file doesn't contain column {column_BEFL_status_perm_grass}, so "
+            "new grassland cannot be ignored!"
+        )
+
+    return parceldata_df
+
+
+def prepare_input_most_popular_crop(
+    parceldata_df,
+    column_BEFL_cropcode: str,
+    column_output_class: str,
+    classes_refe_path: Path,
+):
+    """
+    This function creates a file that is compliant with the assumptions used by the rest
+    of the classification functionality.
+
+    It should be a csv file with the following columns:
+        - object_id: column with a unique identifier
+        - classname: a string column with a readable name of the classes that will be
+          classified to
+
+    This specific implementation converts the typiscal export format used in BE-Flanders
+    to this format.
+    """
+
+    # Add columns for the class to use...
+    parceldata_df.insert(0, column_output_class, None)
+
+    parceldata_df.loc[
+        parceldata_df[column_BEFL_cropcode].isin(["60", "700", "3432"]),
+        column_output_class,
+    ] = "Grassland"  # Grassland
+    parceldata_df.loc[
+        parceldata_df[column_BEFL_cropcode].isin(["201", "202"]), column_output_class
+    ] = "Maize"  # Maize
+    parceldata_df.loc[
+        parceldata_df[column_BEFL_cropcode].isin(["901", "904"]), column_output_class
+    ] = "Potatoes"  # Potatoes
+    parceldata_df.loc[
+        parceldata_df[column_BEFL_cropcode].isin(["311", "36"]), column_output_class
+    ] = "WinterWheat"  # Winter wheat of spelt
+    parceldata_df.loc[
+        parceldata_df[column_BEFL_cropcode].isin(["91"]), column_output_class
+    ] = "SugarBeat"  # Sugar beat
+    parceldata_df.loc[
+        parceldata_df[column_BEFL_cropcode].isin(["321"]), column_output_class
+    ] = "WinterBarley"  # Winter barley
+    parceldata_df.loc[
+        parceldata_df[column_BEFL_cropcode].isin(["71"]), column_output_class
+    ] = "FodderBeat"  # Fodder beat
+
+    # Some extra cleanup: classes starting with 'nvt' or empty ones
+    logger.info(
+        "Set classes that are empty to 'IGNORE_UNIMPORTANT_CLASS' so they are ignored "
+        "further on..."
+    )
+    parceldata_df.loc[
+        parceldata_df[column_output_class].isnull(), column_output_class
+    ] = "IGNORE_UNIMPORTANT_CLASS"
+
+    # Drop the columns that aren't useful at all
+    for column in parceldata_df.columns:
+        if (
+            column not in [conf.columns["id"], column_output_class]
+            and column not in conf.preprocess.getlist("extra_export_columns")
+            and column not in columns_BEFL_to_keep
+            and not column == column_BEFL_cropcode
+        ):
+            parceldata_df.drop(column, axis=1, inplace=True)
+        elif column == column_BEFL_gesp_pm:
+            parceldata_df[column_BEFL_gesp_pm] = parceldata_df[
+                column_BEFL_gesp_pm
+            ].str.replace(",", ";")
+
+    # Return result
+    return parceldata_df
```

### Comparing `cropclassification-0.1.0a2/cropclassification/preprocess/timeseries.py` & `cropclassification-0.1.1/cropclassification/preprocess/timeseries.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,286 +1,306 @@
-# -*- coding: utf-8 -*-
-"""
-This module contains general functions that apply to timeseries data...
-"""
-
-import logging
-import os
-from pathlib import Path
-from typing import List
-
-import pandas as pd
-
-import cropclassification.helpers.config_helper as conf
-import cropclassification.helpers.pandas_helper as pdh
-import cropclassification.preprocess.timeseries_util as ts_util
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
-
-
-def calc_timeseries_data(
-    input_parcel_path: Path,
-    input_country_code: str,
-    start_date_str: str,
-    end_date_str: str,
-    sensordata_to_get: List[str],
-    base_filename: str,
-    dest_data_dir: Path,
-):
-    """
-    Calculate timeseries data for the input parcels
-
-    Args:
-        input_parcel_path (str): [description]
-        input_country_code (str): [description]
-        start_date_str (str): [description]
-        end_date_str (str): [description]
-        sensordata_to_get (List[str]): an array with data you want to be calculated:
-                check out the constants starting with DATA_TO_GET... for the options.
-        base_filename (str): [description]
-        dest_data_dir (str): [description]
-    """
-    # Check some variables...
-    if sensordata_to_get is None:
-        raise Exception("sensordata_to_get cannot be None")
-    if not dest_data_dir.exists():
-        os.makedirs(dest_data_dir)
-
-    # As we want a weekly calculation, get nearest monday for start and stop day
-    start_date = ts_util.get_monday(
-        start_date_str
-    )  # output: vb 2018_2_1 - maandag van week 2 van 2018
-    end_date = ts_util.get_monday(end_date_str)
-    start_date_monday = start_date.strftime("%Y-%m-%d")  # terug omzetten naar Y/M/D
-    end_date_monday = end_date.strftime("%Y-%m-%d")
-
-    logger.info(
-        f"Start date {start_date_str} converted to monday before: {start_date}, end "
-        f"date {end_date_str} as well: {end_date}"
-    )
-    timeseries_calc_type = conf.timeseries["timeseries_calc_type"]
-    if timeseries_calc_type == "gee":
-        # Start!
-        import cropclassification.preprocess.timeseries_calc_gee as ts_calc_gee
-
-        return ts_calc_gee.calc_timeseries_data(
-            input_parcel_path=input_parcel_path,
-            input_country_code=input_country_code,
-            start_date_str=start_date_monday,
-            end_date_str=end_date_monday,
-            sensordata_to_get=sensordata_to_get,
-            base_filename=base_filename,
-            dest_data_dir=dest_data_dir,
-        )
-    elif timeseries_calc_type == "onda":
-        # Start!
-        # TODO: start calculation of per image data on DIAS
-        # import cropclassification.preprocess.timeseries_calc_dias_onda_per_image as
-        # ts_calc
-        timeseries_per_image_dir = conf.dirs.getpath("timeseries_per_image_dir")
-
-        # Now all image data is available per image, calculate periodic data
-        return ts_util.calculate_periodic_data(
-            input_parcel_path=input_parcel_path,
-            input_base_dir=timeseries_per_image_dir,
-            start_date_str=start_date_str,
-            end_date_str=end_date_str,
-            sensordata_to_get=sensordata_to_get,
-            dest_data_dir=dest_data_dir,
-        )
-    else:
-        message = f"Unsupported timeseries calculation type: {timeseries_calc_type}"
-        logger.error(message)
-        raise Exception(message)
-
-
-def collect_and_prepare_timeseries_data(
-    input_parcel_path: Path,
-    timeseries_dir: Path,
-    base_filename: str,
-    output_path: Path,
-    start_date_str: str,
-    end_date_str: str,
-    sensordata_to_use: List[str],
-    parceldata_aggregations_to_use: List[str],
-    force: bool = False,
-):
-    """
-    Collect all timeseries data to use for the classification and prepare it by applying
-    scaling,... as needed.
-    """
-
-    # Some constants to choose which type of data to use in the marker.
-    # Remark: the string needs to be the same as the end of the name of the columns in the csv files!
-    # TODO: I'm not really happy with both a list in the ini file + here... not sure what the
-    #       cleanest solution is though...
-    PARCELDATA_AGGRAGATION_MEAN = conf.general[
-        "PARCELDATA_AGGRAGATION_MEAN"
-    ]  # Mean value of the pixels values in a parcel.
-    PARCELDATA_AGGRAGATION_STDDEV = conf.general[
-        "PARCELDATA_AGGRAGATION_STDDEV"
-    ]  # std dev of the values of the pixels in a parcel
-
-    # Constants for types of sensor data
-    SENSORDATA_S1 = conf.general["SENSORDATA_S1"]  # Sentinel 1 data
-    SENSORDATA_S1DB = conf.general["SENSORDATA_S1DB"]  # Sentinel 1 data, in dB
-    SENSORDATA_S1_ASCDESC = conf.general[
-        "SENSORDATA_S1_ASCDESC"
-    ]  # Sentinel 1 data, divided in Ascending and Descending passes
-    SENSORDATA_S1DB_ASCDESC = conf.general[
-        "SENSORDATA_S1DB_ASCDESC"
-    ]  # Sentinel 1 data, in dB, divided in Ascending and Descending passes
-    SENSORDATA_S2 = conf.general["SENSORDATA_S2"]  # Sentinel 2 data
-    SENSORDATA_S2gt95 = conf.general[
-        "SENSORDATA_S2gt95"
-    ]  # Sentinel 2 data (B2,B3,B4,B8) IF available for 95% or area
-    SENSORDATA_S1_COHERENCE = conf.general["SENSORDATA_S1_COHERENCE"]
-
-    # If force == False Check and the output file exists already, stop.
-    if force is False and output_path.exists() is True:
-        logger.warning(
-            f"Output file already exists and force == False, so stop: {output_path}"
-        )
-        return
-
-    # Init the result with the id's of the parcels we want to treat
-    result_df = pdh.read_file(input_parcel_path, columns=[conf.columns["id"]])
-    if result_df.index.name != conf.columns["id"]:
-        result_df.set_index(conf.columns["id"], inplace=True)
-    nb_input_parcels = len(result_df.index)
-    logger.info(
-        f"Parceldata aggregations that need to be used: {parceldata_aggregations_to_use}"
-    )
-    logger.setLevel(logging.DEBUG)
-
-    # Loop over all input timeseries data to find the data we really need
-    data_ext = conf.general["data_ext"]
-    path_start = timeseries_dir / f"{base_filename}_{start_date_str}{data_ext}"
-    path_end = timeseries_dir / f"{base_filename}_{end_date_str}{data_ext}"
-    logger.debug(f"path_start_date: {path_start}")
-    logger.debug(f"path_end_date: {path_end}")
-
-    ts_data_files = timeseries_dir.glob(f"{base_filename}_*{data_ext}")
-    for curr_path in sorted(ts_data_files):
-
-        # Only process data that is of the right sensor types
-        sensor_type = curr_path.stem.split("_")[-1]
-        if sensor_type not in sensordata_to_use:
-            logger.debug(
-                f"SKIP: file is not in sensor types asked ({sensordata_to_use}): {curr_path}"
-            )
-            continue
-        # The only data we want to process is the data in the range of dates
-        if (str(curr_path) < str(path_start)) or (str(curr_path) >= str(path_end)):
-            logger.debug(f"SKIP: File is not in date range asked: {curr_path}")
-            continue
-        # An empty file signifies that there wasn't any valable data for that
-        # period/sensor/...
-        if os.path.getsize(curr_path) == 0:
-            logger.info(f"SKIP: file is empty: {curr_path}")
-            continue
-
-        # Read data, and check if there is enough data in it
-        data_read_df = pdh.read_file(curr_path)
-        nb_data_read = len(data_read_df.index)
-        data_available_pct = nb_data_read * 100 / nb_input_parcels
-        min_parcels_with_data_pct = conf.timeseries.getfloat(
-            "min_parcels_with_data_pct"
-        )
-        if data_available_pct < min_parcels_with_data_pct:
-            logger.info(
-                f"SKIP: only data for {data_available_pct:.2f}% of parcels, should be "
-                f"> {min_parcels_with_data_pct}%: {curr_path}"
-            )
-            continue
-
-        # Start processing the file
-        logger.info(f"Process file: {curr_path}")
-        if data_read_df.index.name != conf.columns["id"]:
-            data_read_df.set_index(conf.columns["id"], inplace=True)
-
-        # Loop over columns to check if there are columns that need to be dropped.
-        for column in data_read_df.columns:
-
-            # If it is the id column, continue
-            if column == conf.columns["id"]:
-                continue
-
-            # Check if the column is "asked"
-            column_ok = False
-            for parceldata_aggregation in parceldata_aggregations_to_use:
-                if column.endswith("_" + parceldata_aggregation):
-                    column_ok = True
-            if column_ok is False:
-                # Drop column if it doesn't end with something in parcel_data_aggregations_to_use
-                logger.debug(
-                    f"Drop column as it's column aggregation isn't to be used: {column}"
-                )
-                data_read_df.drop(column, axis=1, inplace=True)
-                continue
-
-            # Check if the column contains data for enough parcels
-            valid_input_data_pct = (
-                1 - (data_read_df[column].isnull().sum() / nb_input_parcels)
-            ) * 100
-            if valid_input_data_pct < min_parcels_with_data_pct:
-                # If the number of nan values for the column > x %, drop column
-                logger.warn(
-                    f"Drop column as it contains only {valid_input_data_pct:.2f}% real "
-                    f"data compared to input (= not nan) which is "
-                    f"< {min_parcels_with_data_pct}%!: {column}"
-                )
-                data_read_df.drop(column, axis=1, inplace=True)
-
-        # If S2, rescale data
-        if sensor_type.startswith(SENSORDATA_S2):
-            for column in data_read_df.columns:
-                logger.info(
-                    f"Column contains S2 data, so scale it by dividing by 10.000: {column}"
-                )
-                data_read_df[column] = data_read_df[column] / 10000
-
-        # If S1 coherence, rescale data
-        if sensor_type == SENSORDATA_S1_COHERENCE:
-            for column in data_read_df.columns:
-                logger.info(
-                    f"Column contains S1 Coherence data, so scale it by dividing by 300: {column}"
-                )
-                data_read_df[column] = data_read_df[column] / 300
-
-        # Join the data to the result...
-        result_df = result_df.join(data_read_df, how="left")
-
-    # Remove rows with many null values from result
-    max_number_null = int(0.6 * len(result_df.columns))
-    parcel_many_null_df = result_df[result_df.isnull().sum(axis=1) > max_number_null]
-    if len(parcel_many_null_df.index) > 0:
-        # Write the rows with empty data to a file
-        parcel_many_null_path = Path(f"{str(output_path)}_rows_many_null.sqlite")
-        logger.warn(
-            f"Write {len(parcel_many_null_df.index)} rows with > {max_number_null} of "
-            f"{len(result_df.columns)} columns==null to {parcel_many_null_path}"
-        )
-        pdh.to_file(parcel_many_null_df, parcel_many_null_path)
-
-        # Now remove them from result
-        result_df = result_df[result_df.isnull().sum(axis=1) <= max_number_null]
-
-    # For rows with some null values, set them to 0
-    # TODO: first rough test of using interpolation doesn't give a difference, maybe
-    # better if smarter interpolation is used (= only between the different types of
-    # data: S1_GRD_VV, S1_GRD_VH, S1_COH_VV, S1_COH_VH, ASC?, DESC?, S2
-    # result_df.interpolate(inplace=True)
-    result_df.fillna(0, inplace=True)
-
-    # Write output file...
-    logger.info(f"Write output to file, start: {output_path}")
-    pdh.to_file(result_df, output_path)
-    logger.info(f"Write output to file, ready (with shape: {result_df.shape})")
+# -*- coding: utf-8 -*-
+"""
+This module contains general functions that apply to timeseries data...
+"""
+
+from datetime import datetime
+import logging
+import os
+from pathlib import Path
+from typing import Dict, List
+
+import cropclassification.helpers.config_helper as conf
+import cropclassification.helpers.pandas_helper as pdh
+import cropclassification.preprocess._timeseries_helper as ts_helper
+
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+
+# Get a logger...
+logger = logging.getLogger(__name__)
+
+# The real work
+# -------------------------------------------------------------
+
+
+def calc_timeseries_data(
+    input_parcel_path: Path,
+    start_date_str: str,
+    end_date_str: str,
+    sensordata_to_get: Dict[str, conf.SensorData],
+    dest_data_dir: Path,
+):
+    """
+    Calculate timeseries data for the input parcels
+
+    Args:
+        input_parcel_path (str): [description]
+        start_date_str (str): [description]
+        end_date_str (str): [description]
+        sensordata_to_get (List[str]): an array with data you want to be calculated:
+            check out the constants starting with DATA_TO_GET... for the options.
+        dest_data_dir (str): [description]
+    """
+    # Check some variables...
+    if sensordata_to_get is None:
+        raise Exception("sensordata_to_get cannot be None")
+    if not dest_data_dir.exists():
+        dest_data_dir.mkdir(parents=True, exist_ok=True)
+
+    # As we want a weekly calculation, get nearest monday for start and stop day
+    start_date = ts_helper.get_monday(
+        start_date_str
+    )  # output: vb 2018_2_1 - maandag van week 2 van 2018
+    end_date = ts_helper.get_monday(end_date_str)
+
+    logger.info(
+        f"Start date {start_date_str} converted to monday before: {start_date}, end "
+        f"date {end_date_str} as well: {end_date}"
+    )
+    sensordata_to_get_onda = [
+        sensor for sensor in sensordata_to_get if sensor not in conf.image_profiles
+    ]
+    sensordata_to_get_openeo = [
+        sensor for sensor in sensordata_to_get if sensor in conf.image_profiles
+    ]
+
+    if len(sensordata_to_get_onda) > 0:
+        # Start!
+        # TODO: start calculation of per image data on DIAS
+        # import cropclassification.preprocess.timeseries_calc_dias_onda_per_image as
+        # ts_calc
+
+        # Now all image data is available per image, calculate periodic data
+        ts_helper.calculate_periodic_timeseries(
+            parcel_path=input_parcel_path,
+            timeseries_per_image_dir=conf.dirs.getpath("timeseries_per_image_dir"),
+            start_date=start_date,
+            end_date=end_date,
+            sensordata_to_get=sensordata_to_get_onda,
+            dest_data_dir=dest_data_dir,
+        )
+    if len(sensordata_to_get_openeo) > 0:
+        # Pepare periodic images + calculate base timeseries on them
+        import cropclassification.preprocess._timeseries_calc_openeo as ts_calc_openeo
+
+        sensordata_to_get_info_openeo = [
+            conf.image_profiles[sensordatatype]
+            for sensordatatype in sensordata_to_get_openeo
+        ]
+        ts_calc_openeo.calculate_periodic_timeseries(
+            input_parcel_path=input_parcel_path,
+            start_date=start_date,
+            end_date=end_date,
+            sensordata_to_get=sensordata_to_get_info_openeo,
+            dest_image_data_dir=conf.dirs.getpath("images_periodic_dir"),
+            dest_data_dir=dest_data_dir,
+        )
+
+
+def collect_and_prepare_timeseries_data(
+    input_parcel_path: Path,
+    timeseries_dir: Path,
+    base_filename: str,
+    output_path: Path,
+    start_date_str: str,
+    end_date_str: str,
+    sensordata_to_use: Dict[str, conf.SensorData],
+    parceldata_aggregations_to_use: List[str],
+    force: bool = False,
+):
+    """
+    Collect all timeseries data to use for the classification and prepare it by applying
+    scaling,... as needed.
+    """
+
+    # If force == False Check and the output file exists already, stop.
+    if force is False and output_path.exists() is True:
+        logger.warning(
+            f"Output file already exists and force == False, so stop: {output_path}"
+        )
+        return
+    start_date = datetime.fromisoformat(start_date_str)
+    end_date = datetime.fromisoformat(end_date_str)
+
+    # Init the result with the id's of the parcels we want to treat
+    result_df = pdh.read_file(input_parcel_path, columns=[conf.columns["id"]])
+    if result_df.index.name != conf.columns["id"]:
+        result_df.set_index(conf.columns["id"], inplace=True)
+    nb_input_parcels = len(result_df.index)
+    logger.info(f"Parceldata aggregations to use: {parceldata_aggregations_to_use}")
+    logger.setLevel(logging.DEBUG)
+
+    # Loop over all input timeseries data to find the data we really need
+    glob_pattern = f"*{conf.general['data_ext']}"
+    ts_data_paths = list(timeseries_dir.glob(glob_pattern))
+    if len(ts_data_paths) == 0:
+        raise ValueError(f"No timeseries data found for pattern {glob_pattern}")
+
+    for curr_path in sorted(ts_data_paths):
+        # Only process data that is of the right sensor types
+        fileinfo = ts_helper.get_fileinfo_timeseries_periods(curr_path)
+        image_profile = fileinfo["image_profile"].lower()
+        if image_profile not in sensordata_to_use:
+            logger.debug(
+                f"SKIP: file not needed (only {sensordata_to_use}): {curr_path}"
+            )
+            continue
+        # The only data we want to process is the data in the range of dates
+        if fileinfo["start_date"] < start_date or fileinfo["end_date"] >= end_date:
+            logger.debug(f"SKIP: file doesn't match the period asked: {curr_path}")
+            continue
+        band = fileinfo["band"]
+        if band not in sensordata_to_use[image_profile].bands:
+            logger.debug(f"SKIP: file doesn't match the bands asked: {curr_path}")
+            continue
+        time_dimension_reducer_asked = sensordata_to_use[
+            image_profile
+        ].imageprofile.process_options.get("time_dimension_reducer")
+        if time_dimension_reducer_asked is not None:
+            time_dimension_reducer = fileinfo.get("time_dimension_reducer")
+            if time_dimension_reducer is None:
+                logger.warning(
+                    f"SKIP: time_dimension_reducer {time_dimension_reducer_asked} "
+                    f"asked, but not known for file: {curr_path}"
+                )
+                continue
+            elif time_dimension_reducer != time_dimension_reducer_asked:
+                logger.debug(
+                    f"SKIP: file doesn't match the time reducer asked: {curr_path}"
+                )
+                continue
+
+        # An empty file signifies that there wasn't any valable data for that
+        # period/sensor/...
+        if os.path.getsize(curr_path) == 0:
+            logger.info(f"SKIP: file is empty: {curr_path}")
+            continue
+
+        # Read data, and check if there is enough data in it
+        data_read_df = pdh.read_file(curr_path)
+        nb_data_read = len(data_read_df.index)
+        data_available_pct = nb_data_read * 100 / nb_input_parcels
+        min_parcels_with_data_pct = conf.timeseries.getfloat(
+            "min_parcels_with_data_pct"
+        )
+        if data_available_pct < min_parcels_with_data_pct:
+            logger.info(
+                f"SKIP: only data for {data_available_pct:.2f}% of parcels, should be "
+                f"> {min_parcels_with_data_pct}%: {curr_path}"
+            )
+            continue
+
+        # Start processing the file
+        logger.info(f"Process file: {curr_path}")
+        if data_read_df.index.name != conf.columns["id"]:
+            data_read_df.set_index(conf.columns["id"], inplace=True)
+
+        # Loop over columns to check if there are columns that need to be dropped.
+        columns_to_rename = {}
+        for column in data_read_df.columns:
+            # If it is the id column, continue
+            if column == conf.columns["id"]:
+                continue
+
+            # Check if the column is "asked"
+            column_ok = False
+            for parceldata_aggregation in parceldata_aggregations_to_use:
+                if column.endswith("_" + parceldata_aggregation):
+                    column_ok = True
+                elif column == parceldata_aggregation:
+                    curr_start_date_str = fileinfo["start_date"].strftime("%Y%m%d")
+                    columns_to_rename[
+                        column
+                    ] = f"{image_profile}_{curr_start_date_str}_{band}_{column}"
+                    column_ok = True
+            if not column_ok:
+                # Drop column if it doesn't end with something in
+                # parcel_data_aggregations_to_use
+                logger.debug(
+                    "Drop column as it's column aggregation isn't to be used: "
+                    f"{curr_path.stem}.{column}"
+                )
+                data_read_df.drop(column, axis=1, inplace=True)
+                continue
+
+            # Check if the column contains data for enough parcels
+            valid_input_data_pct = (
+                1 - (data_read_df[column].isnull().sum() / nb_input_parcels)
+            ) * 100
+            if valid_input_data_pct < min_parcels_with_data_pct:
+                # If the number of nan values for the column > x %, drop column
+                logger.warn(
+                    f"Drop column as it contains only {valid_input_data_pct:.2f}% real "
+                    f"data compared to input (= not nan) which is "
+                    f"< {min_parcels_with_data_pct}%!: {curr_path.stem}.{column}"
+                )
+                data_read_df.drop(column, axis=1, inplace=True)
+
+        # If there are columns that need renaming, do so
+        if len(columns_to_rename) > 0:
+            data_read_df = data_read_df.rename(columns=columns_to_rename)
+
+        # If S2, rescale data
+        if image_profile.startswith("s2"):
+            for column in data_read_df.columns:
+                logger.info(
+                    f"Column with s2 data: divide by 10.000, clip to upper=1: {column}"
+                )
+                data_read_df[column] = data_read_df[column] / 10000
+                data_read_df[column] = data_read_df[column].clip(upper=1)
+
+        # If s1 grd, rescale data
+        if image_profile.startswith("s1-grd"):
+            for column in data_read_df.columns:
+                logger.info(f"Column with s1-grd data: clip to upper=1: {column}")
+                data_read_df[column] = data_read_df[column].clip(upper=1)
+
+        # If s1 coherence, rescale data
+        if image_profile in ["s1coh", "s1-coh"]:
+            for column in data_read_df.columns:
+                logger.info(
+                    f"Column with s1 coherence: scale it by dividing by 300: {column}"
+                )
+                data_read_df[column] = data_read_df[column] / 300
+
+        # Join the data to the result...
+        result_df = result_df.join(data_read_df, how="left")
+
+    # No timeseries data was found, so stop
+    if len(result_df.columns) == 0:
+        raise ValueError("data collection resulted in 0 columns")
+
+    # Remove rows with many null values from result
+    max_number_null = int(0.6 * len(result_df.columns))
+    parcel_many_null_df = result_df[result_df.isnull().sum(axis=1) > max_number_null]
+    if len(parcel_many_null_df.index) > 0:
+        # Write the rows with empty data to a file
+        parcel_many_null_path = Path(f"{str(output_path)}_rows_many_null.sqlite")
+        logger.warn(
+            f"Write {len(parcel_many_null_df.index)} rows with > {max_number_null} of "
+            f"{len(result_df.columns)} columns==null to {parcel_many_null_path}"
+        )
+        pdh.to_file(parcel_many_null_df, parcel_many_null_path)
+
+        # Now remove them from result
+        result_df = result_df[result_df.isnull().sum(axis=1) <= max_number_null]
+
+    # Check if there are values not in the range -1 till +1
+    gt1_df = result_df[result_df > 1].dropna()
+    ltm1_df = result_df[result_df < -1].dropna()
+    if gt1_df.size > 0:
+        logger.warning(f"result_df containes values > 1: {gt1_df}")
+    if ltm1_df.size > 0:
+        logger.warning(f"result_df containes values < -1: {ltm1_df}")
+
+    # For rows with some null values, set them to 0
+    # TODO: first rough test of using interpolation doesn't give a difference, maybe
+    # better if smarter interpolation is used (= only between the different types of
+    # data: S1_GRD_VV, S1_GRD_VH, S1_COH_VV, S1_COH_VH, ASC?, DESC?, S2
+    # result_df.interpolate(inplace=True)
+    result_df.fillna(0, inplace=True)
+
+    # Write output file...
+    logger.info(f"Write output to file, start: {output_path}")
+    pdh.to_file(result_df, output_path)
+    logger.info(f"Write output to file, ready (with shape: {result_df.shape})")
```

### Comparing `cropclassification-0.1.0a2/cropclassification/preprocess/timeseries_util.py` & `cropclassification-0.1.1/cropclassification/preprocess/_timeseries_helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,588 +1,659 @@
-# -*- coding: utf-8 -*-
-"""
-Calculates periodic timeseries for input parcels.
-"""
-
-from datetime import datetime
-import logging
-import gc
-import os
-from pathlib import Path
-from typing import List, Optional
-
-import geofileops as gfo
-import numpy as np
-import pandas as pd
-
-# Import local stuff
-import cropclassification.helpers.config_helper as conf
-import cropclassification.helpers.pandas_helper as pdh
-
-# -------------------------------------------------------------
-# First define/init some general variables/constants
-# -------------------------------------------------------------
-# Get a logger...
-logger = logging.getLogger(__name__)
-
-IMAGETYPE_S1_GRD = "S1_GRD"
-IMAGETYPE_S1_COHERENCE = "S1_COH"
-IMAGETYPE_S2_L2A = "S2_L2A"
-
-
-def prepare_input(
-    input_parcel_path: Path,
-    output_imagedata_parcel_input_path: Path,
-    output_parcel_nogeo_path: Optional[Path] = None,
-    force: bool = False,
-):
-    """
-    This function creates a file that is preprocessed to be a good input file for
-    timeseries extraction of sentinel images.
-
-    Args
-        input_parcel_path (Path): input file
-        output_imagedata_parcel_input_path (Path): prepared output file
-        output_parcel_nogeo_path (Path): output file with a copy of the non-geo data
-        force: force creation, even if output file(s) exist already
-
-    """
-    # Check if parameters are OK and init some extra params
-    if not input_parcel_path.exists():
-        raise Exception(f"Input file doesn't exist: {input_parcel_path}")
-
-    # Check if the input file has a projection specified
-    if gfo.get_crs(input_parcel_path) is None:
-        message = (
-            "The parcel input file doesn't have a projection/crs specified, so STOP: "
-            f"{input_parcel_path}"
-        )
-        logger.critical(message)
-        raise Exception(message)
-
-    # If force == False Check and the output file exists already, stop.
-    if (
-        force is False
-        and output_imagedata_parcel_input_path.exists()
-        and (output_parcel_nogeo_path is None or output_parcel_nogeo_path.exists())
-    ):
-        logger.warning(
-            "prepare_input: force == False and output files exist, so stop: "
-            + f"{output_imagedata_parcel_input_path}, "
-            + f"{output_parcel_nogeo_path}"
-        )
-        return
-
-    logger.info(f"Process input file {input_parcel_path}")
-
-    # Create temp dir to store temporary data for tracebility
-    temp_output_dir = output_imagedata_parcel_input_path.parent / "temp"
-    if not temp_output_dir.exists():
-        os.mkdir(temp_output_dir)
-
-    # Read the parcel data and write nogeo version
-    parceldata_gdf = gfo.read_file(input_parcel_path)
-    logger.info(f"Parceldata read, shape: {parceldata_gdf.shape}")
-
-    # Check if the id column is present and set as index
-    if conf.columns["id"] in parceldata_gdf.columns:
-        parceldata_gdf.set_index(conf.columns["id"], inplace=True)
-    else:
-        message = (
-            f"STOP: Column {conf.columns['id']} not found in input parcel file: "
-            f"{input_parcel_path}. Make sure the column is present or change the "
-            "column name in global_constants.py"
-        )
-        logger.critical(message)
-        raise Exception(message)
-
-    if output_parcel_nogeo_path is not None and (
-        force is True or not output_parcel_nogeo_path.exists()
-    ):
-        logger.info(f"Save non-geo data to {output_parcel_nogeo_path}")
-        parceldata_nogeo_df = parceldata_gdf.drop(["geometry"], axis=1)
-        pdh.to_file(parceldata_nogeo_df, output_parcel_nogeo_path)
-
-    # Do the necessary conversions and write buffered file
-
-    # If force == False Check and the output file exists already, stop.
-    if force is False and output_imagedata_parcel_input_path.exists():
-        logger.warning(
-            "prepare_input: force == False and output files exist, so stop: "
-            f"{output_imagedata_parcel_input_path}"
-        )
-        return
-
-    logger.info("Apply buffer on parcel")
-    parceldata_buf_gdf = parceldata_gdf.copy()
-
-    # resolution = number of segments per circle
-    buffer_size = -conf.marker.getint("buffer")
-    parceldata_buf_gdf[conf.columns["geom"]] = parceldata_buf_gdf[
-        conf.columns["geom"]
-    ].buffer(buffer_size, resolution=5)
-
-    # Export buffered geometries that result in empty geometries
-    logger.info("Export parcels that are empty after buffer")
-    parceldata_buf_empty_df = parceldata_buf_gdf.loc[
-        parceldata_buf_gdf[conf.columns["geom"]].is_empty == True
-    ]
-    if len(parceldata_buf_empty_df.index) > 0:
-        parceldata_buf_empty_df.drop(conf.columns["geom"], axis=1, inplace=True)
-        temp_empty_path = (
-            temp_output_dir / f"{output_imagedata_parcel_input_path.stem}_empty.sqlite"
-        )
-        pdh.to_file(parceldata_buf_empty_df, temp_empty_path)
-
-    # Export parcels that don't result in a (multi)polygon
-    parceldata_buf_notempty_gdf = parceldata_buf_gdf.loc[
-        parceldata_buf_gdf[conf.columns["geom"]].is_empty == False
-    ]
-    parceldata_buf_nopoly_gdf = parceldata_buf_notempty_gdf.loc[
-        ~parceldata_buf_notempty_gdf[conf.columns["geom"]].geom_type.isin(
-            ["Polygon", "MultiPolygon"]
-        )
-    ]
-    if len(parceldata_buf_nopoly_gdf.index) > 0:
-        logger.info("Export parcels that are no (multi)polygons after buffer")
-        parceldata_buf_nopoly_gdf.drop(conf.columns["geom"], axis=1, inplace=True)
-        temp_nopoly_path = (
-            temp_output_dir / f"{output_imagedata_parcel_input_path.stem}_nopoly.sqlite"
-        )
-        gfo.to_file(parceldata_buf_nopoly_gdf, temp_nopoly_path)
-
-    # Export parcels that are (multi)polygons after buffering
-    parceldata_buf_poly_gdf = parceldata_buf_notempty_gdf.loc[
-        parceldata_buf_notempty_gdf[conf.columns["geom"]].geom_type.isin(
-            ["Polygon", "MultiPolygon"]
-        )
-    ]
-    for column in parceldata_buf_poly_gdf.columns:
-        if column not in [conf.columns["id"], conf.columns["geom"]]:
-            parceldata_buf_poly_gdf.drop(column, axis=1, inplace=True)
-    logger.info(
-        "Export parcels that are (multi)polygons after buffer to"
-        f"{output_imagedata_parcel_input_path}"
-    )
-    gfo.to_file(parceldata_buf_poly_gdf, output_imagedata_parcel_input_path)
-    logger.info(parceldata_buf_poly_gdf)
-
-    message = (
-        "The buffered file just has been prepared, so probably you now you probably "
-        "need to sync it to the DIAS and start the timeseries data extraction before "
-        "proceding!"
-    )
-    logger.warning(message)
-    raise Exception(message)
-
-
-def calculate_periodic_data(
-    input_parcel_path: Path,
-    input_base_dir: Path,
-    start_date_str: str,
-    end_date_str: str,
-    sensordata_to_get: List[str],
-    dest_data_dir: Path,
-    force: bool = False,
-):
-    """
-    This function creates a file that is a weekly summarize of timeseries images from
-    DIAS.
-
-    TODO: add possibility to choose which values to extract (mean, min, max,...)?
-
-    Args:
-        input_parcel_path (Path): [description]
-        input_base_dir (Path): [description]
-        start_date_str (str): Start date in format %Y-%m-%d. Needs to be aligned
-            already on the periods wanted + data on this date is included.
-        end_date_str (str): End date in format %Y-%m-%d. Needs to be aligned already on
-            the periods wanted + data on this date is excluded.
-        sensordata_to_get ([]):
-        dest_data_dir (Path): [description]
-        force (bool, optional): [description]. Defaults to False.
-    """
-    logger.info("calculate_periodic_data")
-
-    # Init
-    input_dir = input_base_dir / input_parcel_path.stem
-
-    # TODO: in config?
-    input_ext = ".sqlite"
-    output_ext = ".sqlite"
-
-    start_date = datetime.strptime(start_date_str, "%Y-%m-%d")
-    end_date = datetime.strptime(end_date_str, "%Y-%m-%d")
-    year = start_date_str.split("-")[0]
-
-    # Prepare output dir
-    test = False
-    if test is True:
-        dest_data_dir = Path(f"{str(dest_data_dir)}_test")
-    if not dest_data_dir.exists():
-        os.mkdir(dest_data_dir)
-
-    # Create Dataframe with all files with their info
-    logger.debug("Create Dataframe with all files and their properties")
-    file_info_list = []
-    for filename in os.listdir(input_dir):
-        if filename.endswith(input_ext):
-            # Get seperate filename parts
-            file_info = get_file_info(input_dir / filename)
-            file_info_list.append(file_info)
-
-    all_inputfiles_df = pd.DataFrame(file_info_list)
-
-    # Loop over the data we need to get
-    id_column = conf.columns["id"]
-    for sensordata_type in sensordata_to_get:
-
-        logger.debug(
-            "Get files we need based on start- & stopdates, sensordata_to_get,..."
-        )
-        orbits = [None]
-        if sensordata_type == conf.general["SENSORDATA_S1_ASCDESC"]:
-            # Filter files to the ones we need
-            satellitetype = "S1"
-            imagetype = IMAGETYPE_S1_GRD
-            bands = ["VV", "VH"]
-            orbits = ["ASC", "DESC"]
-            needed_inputfiles_df = all_inputfiles_df.loc[
-                (all_inputfiles_df.date >= start_date)
-                & (all_inputfiles_df.date < end_date)
-                & (all_inputfiles_df.imagetype == imagetype)
-                & (all_inputfiles_df.band.isin(bands))
-                & (all_inputfiles_df.orbit.isin(orbits))
-            ]
-        elif sensordata_type == conf.general["SENSORDATA_S2gt95"]:
-            satellitetype = "S2"
-            imagetype = IMAGETYPE_S2_L2A
-            bands = ["B02-10m", "B03-10m", "B04-10m", "B08-10m", "B11-20m", "B12-20m"]
-            needed_inputfiles_df = all_inputfiles_df.loc[
-                (all_inputfiles_df.date >= start_date)
-                & (all_inputfiles_df.date < end_date)
-                & (all_inputfiles_df.imagetype == imagetype)
-                & (all_inputfiles_df.band.isin(bands))
-            ]
-        elif sensordata_type == conf.general["SENSORDATA_S1_COHERENCE"]:
-            satellitetype = "S1"
-            imagetype = IMAGETYPE_S1_COHERENCE
-            bands = ["VV", "VH"]
-            orbits = ["ASC", "DESC"]
-            needed_inputfiles_df = all_inputfiles_df.loc[
-                (all_inputfiles_df.date >= start_date)
-                & (all_inputfiles_df.date < end_date)
-                & (all_inputfiles_df.imagetype == imagetype)
-                & (all_inputfiles_df.band.isin(bands))
-            ]
-        else:
-            raise Exception(f"Unsupported sensordata_type: {sensordata_type}")
-
-        # There should also be one pixcount file
-        pixcount_filename = f"{input_parcel_path.stem}_weekly_pixcount{output_ext}"
-        pixcount_path = dest_data_dir / pixcount_filename
-
-        # For each week
-        start_week = int(datetime.strftime(start_date, "%W"))
-        end_week = int(datetime.strftime(end_date, "%W"))
-        for period_index in range(start_week, end_week):
-
-            # Get the date of the first day of period period_index
-            # (eg. monday for a week)
-            period_date = datetime.strptime(
-                str(year) + "_" + str(period_index) + "_1", "%Y_%W_%w"
-            )
-
-            # New file name
-            period_date_str_long = period_date.strftime("%Y-%m-%d")
-            period_data_filename = f"{input_parcel_path.stem}_weekly_{period_date_str_long}_{sensordata_type}{output_ext}"
-            period_data_path = dest_data_dir / period_data_filename
-
-            # Check if output file exists already
-            if period_data_path.exists() and pixcount_path.exists():
-                if force is False:
-                    logger.info(
-                        f"SKIP: force is False and file exists: {period_data_path}"
-                    )
-                    continue
-                else:
-                    os.remove(period_data_path)
-
-            # Loop over bands and orbits (all combinations of bands and orbits!)
-            logger.info(f"Calculate file: {period_data_filename}")
-            period_data_df = None
-            gc.collect()  # Try to evade memory errors
-            for band, orbit in [(band, orbit) for band in bands for orbit in orbits]:
-
-                # Get list of files needed for this period, band
-                period_files_df = needed_inputfiles_df.loc[
-                    (needed_inputfiles_df.week == period_index)
-                    & (needed_inputfiles_df.band == band)
-                ]
-
-                # If an orbit to be filtered was specified, filter
-                if orbit is not None:
-                    period_files_df = period_files_df.loc[
-                        (period_files_df.orbit == orbit)
-                    ]
-
-                if len(period_files_df) == 0:
-                    logger.warn("No input files found!")
-
-                # Loop all period_files
-                period_band_data_df = None
-                statistic_columns_dict = {
-                    "count": [],
-                    "max": [],
-                    "mean": [],
-                    "median": [],
-                    "min": [],
-                    "std": [],
-                }
-                for j, imagedata_path in enumerate(period_files_df.path.tolist()):
-
-                    # If file has filesize == 0, skip
-                    imagedata_path = Path(imagedata_path)
-                    if imagedata_path.stat().st_size == 0:
-                        continue
-
-                    # Read the file (but only the columns we need)
-                    columns = [column for column in statistic_columns_dict]
-                    columns.append(id_column)
-
-                    image_data_df = pdh.read_file(imagedata_path, columns=columns)
-                    image_data_df.set_index(id_column, inplace=True)
-                    image_data_df.index.name = id_column
-
-                    # Remove rows with nan values
-                    nb_before_dropna = len(image_data_df.index)
-                    image_data_df.dropna(inplace=True)
-                    nb_after_dropna = len(image_data_df.index)
-                    if nb_after_dropna != nb_before_dropna:
-                        logger.warning(
-                            f"Before dropna: {nb_before_dropna}, after: "
-                            f"{nb_after_dropna} for file {imagedata_path}"
-                        )
-                    if nb_after_dropna == 0:
-                        continue
-
-                    # recalculate duplicate rows (the -5 buffer can cause break ups?)
-                    image_data_recalculate_df = (
-                        image_data_df.loc[image_data_df.index.duplicated()]
-                        .groupby(id_column)
-                        .agg({column: "mean" for column in statistic_columns_dict})
-                    )
-                    image_data_df = image_data_df.loc[~image_data_df.index.duplicated()]
-                    image_data_df.append(image_data_recalculate_df)
-
-                    # Rename columns so column names stay unique
-                    for statistic_column in statistic_columns_dict:
-                        new_column_name = statistic_column + str(j + 1)
-                        image_data_df.rename(
-                            columns={statistic_column: new_column_name}, inplace=True
-                        )
-                        image_data_df[new_column_name] = image_data_df[
-                            new_column_name
-                        ].astype(float)
-                        statistic_columns_dict[statistic_column].append(new_column_name)
-
-                    # Create 1 dataframe for all weekfiles
-                    #   - one row for each code_obj
-                    #   - using concat (code_obj = index)
-                    if period_band_data_df is None:
-                        period_band_data_df = image_data_df
-                    else:
-                        period_band_data_df = pd.concat(
-                            [period_band_data_df, image_data_df], axis=1, sort=False
-                        )
-                        # Apparently concat removes the index name in some situations
-                        period_band_data_df.index.name = id_column
-
-                # Calculate max, mean, min, ...
-                if period_band_data_df is not None:
-                    logger.debug("Calculate max, mean, min, ...")
-                    period_date_str_short = period_date.strftime("%Y%m%d")
-                    # Remark: prefix column names: sqlite doesn't like a numeric start
-                    if orbit is None:
-                        column_basename = (
-                            f"TS_{period_date_str_short}_{imagetype}_{band}"
-                        )
-                    else:
-                        column_basename = (
-                            f"TS_{period_date_str_short}_{imagetype}_{orbit}_{band}"
-                        )
-
-                    # Number of pixels
-                    # TODO: onderzoeken hoe aantal pixels best bijgehouden wordt:
-                    # afwijkingen weglaten ? max nemen ? ...
-                    period_band_data_df[f"{column_basename}_count"] = np.nanmax(
-                        period_band_data_df[statistic_columns_dict["count"]], axis=1
-                    )
-                    # Maximum of all max columns
-                    period_band_data_df[f"{column_basename}_max"] = np.nanmax(
-                        period_band_data_df[statistic_columns_dict["max"]], axis=1
-                    )
-                    # Mean of all mean columns
-                    period_band_data_df[f"{column_basename}_mean"] = np.nanmean(
-                        period_band_data_df[statistic_columns_dict["mean"]], axis=1
-                    )
-                    # Mean of all median columns
-                    period_band_data_df[f"{column_basename}_median"] = np.nanmean(
-                        period_band_data_df[statistic_columns_dict["median"]], axis=1
-                    )
-                    # Minimum of all min columns
-                    period_band_data_df[f"{column_basename}_min"] = np.nanmin(
-                        period_band_data_df[statistic_columns_dict["min"]], axis=1
-                    )
-                    # Mean of all std columns
-                    period_band_data_df[f"{column_basename}_std"] = np.nanmean(
-                        period_band_data_df[statistic_columns_dict["std"]], axis=1
-                    )
-                    # Number of Files used
-                    period_band_data_df[
-                        f"{column_basename}_used_files"
-                    ] = period_band_data_df[statistic_columns_dict["max"]].count(axis=1)
-
-                    # Only keep the columns we want to keep
-                    columns_to_keep = [
-                        f"{column_basename}_count",
-                        f"{column_basename}_max",
-                        f"{column_basename}_mean",
-                        f"{column_basename}_median",
-                        f"{column_basename}_min",
-                        f"{column_basename}_std",
-                        f"{column_basename}_used_files",
-                    ]
-                    period_band_data_df = period_band_data_df[columns_to_keep]
-
-                    # Merge the data with the other bands/orbits for this period
-                    if period_data_df is None:
-                        period_data_df = period_band_data_df
-                    else:
-                        period_data_df = pd.concat(
-                            [period_band_data_df, period_data_df], axis=1, sort=False
-                        )
-                        # Apparently concat removes the index name in some situations
-                        period_data_df.index.name = id_column
-
-            if period_data_df is not None:
-                logger.info(f"Write new file: {period_data_filename}")
-                pdh.to_file(period_data_df, period_data_path)
-
-                # Create pixcount file if it doesn't exist yet...
-                if not pixcount_path.exists():
-                    pixcount_s1s2_column = conf.columns["pixcount_s1s2"]
-
-                    # Get max count of all count columns available
-                    columns_to_use = [
-                        column
-                        for column in period_data_df.columns
-                        if column.endswith("_count")
-                    ]
-                    period_data_df[pixcount_s1s2_column] = np.nanmax(
-                        period_data_df[columns_to_use], axis=1
-                    )
-
-                    pixcount_df = period_data_df[pixcount_s1s2_column]
-                    pixcount_df.fillna(value=0, inplace=True)
-                    pdh.to_file(pixcount_df, pixcount_path)
-
-
-def get_file_info(path: Path) -> dict:
-    """
-    This function gets info of a timeseries data file.
-
-    Args:
-        path (Path): The path to the file to get info about.
-
-    Returns:
-        dict: a dict containing info about the file
-    """
-
-    try:
-        # Split name on parcelinfo versus imageinfo
-        filename_splitted = path.stem.split("__")
-        filename_parcelinfo = filename_splitted[0]
-        filename_imageinfo = filename_splitted[1]
-
-        # Extract imageinfo
-        imageinfo_values = filename_imageinfo.split("_")
-
-        # Satellite
-        satellite = imageinfo_values[0]
-
-        # Get the date taken from the filename, depending on the satellite type
-        # Remark: the datetime is in this format: '20180101T055812'
-        imagetype = None
-        filedatetime = None
-        if satellite.startswith("S1"):
-            # Check if it is a GRDH image
-            if imageinfo_values[2] == "GRDH":
-                imagetype = IMAGETYPE_S1_GRD
-                filedatetime = imageinfo_values[4]
-            elif imageinfo_values[1].startswith("S1"):
-                imagetype = IMAGETYPE_S1_COHERENCE
-                filedatetime = imageinfo_values[2]
-        elif satellite.startswith("S2"):
-            imagetype = IMAGETYPE_S2_L2A
-            filedatetime = imageinfo_values[2]
-
-        if imagetype is None or filedatetime is None:
-            raise Exception(f"Unsupported file: {path}")
-
-        filedate = filedatetime.split("T")[0]
-        parseddate = datetime.strptime(filedate, "%Y%m%d")
-        fileweek = int(parseddate.strftime("%W"))
-
-        # Get the band
-        fileband = imageinfo_values[-1]  # =last value
-
-        # For S1 images, get the orbit
-        if satellite.startswith("S1"):
-            fileorbit = imageinfo_values[-2]  # =2nd last value
-        else:
-            fileorbit = None
-
-        # The file paths of these files sometimes are longer than 256
-        # characters, so use trick on windows to support this anyway
-        path_safe = path.as_posix()
-        if os.name == "nt" and len(path.as_posix()) > 240:
-            if path_safe.startswith("//"):
-                path_safe = f"//?/UNC/{path_safe}"
-            else:
-                path_safe = f"//?/{path_safe}"
-
-        filenameparts = {
-            "path": path_safe,
-            "imagetype": imagetype,
-            "filestem": path.stem,
-            "date": parseddate,
-            "week": fileweek,
-            "band": fileband,
-            "orbit": fileorbit,
-        }  # ASC/DESC
-
-    except Exception as ex:
-        message = f"Error extracting info from filename {path}"
-        logger.exception(message)
-        raise Exception(message) from ex
-
-    return filenameparts
-
-
-def get_monday(input_date: str) -> datetime:
-    """
-    This function gets the first monday before the date provided.
-    She is being used to adapt start_date and end_date so they are mondays, so it
-    becomes easier to reuse timeseries data
-       - inputformat:  %Y-%m-%d
-       - outputformat: datetime
-    """
-    parseddate = datetime.strptime(input_date, "%Y-%m-%d")
-    year_week = parseddate.strftime("%Y_%W")
-    year_week_monday = datetime.strptime(year_week + "_1", "%Y_%W_%w")
-    return year_week_monday
-
-
-# If the script is run directly...
-if __name__ == "__main__":
-    raise Exception("Not implemented")
+# -*- coding: utf-8 -*-
+"""
+Calculates periodic timeseries for input parcels.
+"""
+
+from datetime import datetime, timedelta
+import logging
+import gc
+import os
+from pathlib import Path
+from typing import List, Optional, Union
+
+import geofileops as gfo
+import numpy as np
+import pandas as pd
+
+# Import local stuff
+import cropclassification.helpers.config_helper as conf
+import cropclassification.helpers.pandas_helper as pdh
+
+# -------------------------------------------------------------
+# First define/init some general variables/constants
+# -------------------------------------------------------------
+# Get a logger...
+logger = logging.getLogger(__name__)
+
+IMAGETYPE_S1_GRD = "S1_GRD"
+IMAGETYPE_S1_COHERENCE = "S1_COH"
+IMAGETYPE_S2_L2A = "S2_L2A"
+
+
+def prepare_input(
+    input_parcel_path: Path,
+    output_imagedata_parcel_input_path: Path,
+    output_parcel_nogeo_path: Optional[Path] = None,
+    force: bool = False,
+) -> bool:
+    """
+    This function creates a file that is preprocessed to be a good input file for
+    timeseries extraction of sentinel images.
+
+    Args
+        input_parcel_path (Path): input file
+        output_imagedata_parcel_input_path (Path): prepared output file
+        output_parcel_nogeo_path (Path): output file with a copy of the non-geo data
+        force: force creation, even if output file(s) exist already
+    """
+    # Check if parameters are OK and init some extra params
+    if not input_parcel_path.exists():
+        raise Exception(f"Input file doesn't exist: {input_parcel_path}")
+
+    # Check if the input file has a projection specified
+    if gfo.get_crs(input_parcel_path) is None:
+        message = (
+            "The parcel input file doesn't have a projection/crs specified, so STOP: "
+            f"{input_parcel_path}"
+        )
+        logger.critical(message)
+        raise Exception(message)
+
+    # If force == False Check and the output file exists already, stop.
+    if (
+        force is False
+        and output_imagedata_parcel_input_path.exists()
+        and (output_parcel_nogeo_path is None or output_parcel_nogeo_path.exists())
+    ):
+        logger.warning(
+            "prepare_input: force is False and output files exist, so stop: "
+            + f"{output_imagedata_parcel_input_path}, "
+            + f"{output_parcel_nogeo_path}"
+        )
+        return False
+
+    logger.info(f"Process input file {input_parcel_path}")
+
+    # Create temp dir to store temporary data for tracebility
+    temp_output_dir = output_imagedata_parcel_input_path.parent / "temp"
+    if not temp_output_dir.exists():
+        os.mkdir(temp_output_dir)
+
+    # Read the parcel data and write nogeo version
+    parceldata_gdf = gfo.read_file(input_parcel_path)
+    logger.info(f"Parceldata read, shape: {parceldata_gdf.shape}")
+
+    # Check if the id column is present and set as index
+    if conf.columns["id"] in parceldata_gdf.columns:
+        parceldata_gdf.set_index(conf.columns["id"], inplace=True)
+    else:
+        message = (
+            f"STOP: Column {conf.columns['id']} not found in input parcel file: "
+            f"{input_parcel_path}. Make sure the column is present or change the "
+            "column name in global_constants.py"
+        )
+        logger.critical(message)
+        raise Exception(message)
+
+    if output_parcel_nogeo_path is not None and (
+        force is True or not output_parcel_nogeo_path.exists()
+    ):
+        logger.info(f"Save non-geo data to {output_parcel_nogeo_path}")
+        parceldata_nogeo_df = parceldata_gdf.drop(["geometry"], axis=1)
+        pdh.to_file(parceldata_nogeo_df, output_parcel_nogeo_path)
+
+    # Do the necessary conversions and write buffered file
+
+    # If force == False Check and the output file exists already, stop.
+    if force is False and output_imagedata_parcel_input_path.exists():
+        logger.warning(
+            "prepare_input: force is False and output files exist, so stop: "
+            f"{output_imagedata_parcel_input_path}"
+        )
+        return False
+
+    # Apply buffer
+    parceldata_buf_gdf = parceldata_gdf.copy()
+    # resolution = number of segments per circle
+    buffer_size = -conf.marker.getint("buffer")
+    logger.info(f"Apply buffer of {buffer_size} on parcel")
+    parceldata_buf_gdf[conf.columns["geom"]] = parceldata_buf_gdf[
+        conf.columns["geom"]
+    ].buffer(buffer_size, resolution=5)
+
+    # Export buffered geometries that result in empty geometries
+    logger.info("Export parcels that are empty after buffer")
+    parceldata_buf_empty_df = parceldata_buf_gdf.loc[
+        parceldata_buf_gdf[conf.columns["geom"]].is_empty
+    ].copy()
+    if len(parceldata_buf_empty_df.index) > 0:
+        parceldata_buf_empty_df.drop(conf.columns["geom"], axis=1, inplace=True)
+        temp_empty_path = (
+            temp_output_dir / f"{output_imagedata_parcel_input_path.stem}_empty.sqlite"
+        )
+        pdh.to_file(parceldata_buf_empty_df, temp_empty_path)
+
+    # Export parcels that don't result in an empty geometry
+    parceldata_buf_notempty_gdf = parceldata_buf_gdf.loc[
+        ~parceldata_buf_gdf[conf.columns["geom"]].is_empty
+    ]
+    parceldata_buf_nopoly_gdf = parceldata_buf_notempty_gdf.loc[
+        ~parceldata_buf_notempty_gdf[conf.columns["geom"]].geom_type.isin(
+            ["Polygon", "MultiPolygon"]
+        )
+    ]
+    if len(parceldata_buf_nopoly_gdf.index) > 0:
+        logger.info("Export parcels that are no (multi)polygons after buffer")
+        parceldata_buf_nopoly_df = parceldata_buf_nopoly_gdf.drop(
+            conf.columns["geom"], axis=1
+        )
+        temp_nopoly_path = (
+            temp_output_dir / f"{output_imagedata_parcel_input_path.stem}_nopoly.sqlite"
+        )
+        pdh.to_file(parceldata_buf_nopoly_df, temp_nopoly_path)
+
+    # Export parcels that are (multi)polygons after buffering
+    parceldata_buf_poly_gdf = parceldata_buf_notempty_gdf.loc[
+        parceldata_buf_notempty_gdf[conf.columns["geom"]].geom_type.isin(
+            ["Polygon", "MultiPolygon"]
+        )
+    ]
+    for column in parceldata_buf_poly_gdf.columns:
+        if column not in [conf.columns["id"], conf.columns["geom"]]:
+            parceldata_buf_poly_gdf.drop(column, axis=1, inplace=True)
+    logger.info(
+        "Export parcels that are (multi)polygons after buffer to"
+        f"{output_imagedata_parcel_input_path}"
+    )
+    parceldata_buf_poly_gdf.to_file(
+        output_imagedata_parcel_input_path, engine="pyogrio"
+    )
+    logger.info(parceldata_buf_poly_gdf)
+
+    return True
+
+
+def calculate_periodic_timeseries(
+    parcel_path: Path,
+    timeseries_per_image_dir: Path,
+    start_date: datetime,
+    end_date: datetime,
+    sensordata_to_get: List[str],
+    dest_data_dir: Path,
+    force: bool = False,
+):
+    """
+    This function creates a file that is a weekly aggregation of timeseries files.
+
+    TODO: add possibility to choose which values to extract (mean, min, max,...)?
+
+    Args:
+        parcel_path (Path): [description]
+        timeseries_per_image_dir (Path): [description]
+        start_date (datetime): Start date. Needs to be aligned
+            already on the periods wanted + data on this date is included.
+        end_date (datetime): End date. Needs to be aligned already on
+            the periods wanted + data on this date is excluded.
+        sensordata_to_get ([]):
+        dest_data_dir (Path): [description]
+        force (bool, optional): [description]. Defaults to False.
+    """
+    logger.info("calculate_periodic_data")
+
+    # Init
+    # TODO: in config?
+    input_ext = ".sqlite"
+    output_ext = ".sqlite"
+
+    year = start_date.year
+
+    # Prepare output dir
+    dest_data_dir.mkdir(parents=True, exist_ok=True)
+
+    # Create Dataframe with all files with their info
+    logger.debug("Create Dataframe with all files and their properties")
+    file_info_list = []
+    for filename in os.listdir(timeseries_per_image_dir):
+        if filename.endswith(input_ext):
+            # Get seperate filename parts
+            file_info = get_fileinfo_timeseries(input_dir / filename)
+            file_info_list.append(file_info)
+
+    all_inputfiles_df = pd.DataFrame(file_info_list)
+
+    # Loop over the data we need to get
+    id_column = conf.columns["id"]
+    for sensordata_type in sensordata_to_get:
+        logger.debug(
+            "Get files we need based on start- & stopdates, sensordata_to_get,..."
+        )
+        orbits = [None]
+        if sensordata_type == "S1AscDesc":
+            # Filter files to the ones we need
+            # satellitetype = "S1"
+            imagetype = IMAGETYPE_S1_GRD
+            bands = ["VV", "VH"]
+            orbits = ["ASC", "DESC"]
+            needed_inputfiles_df = all_inputfiles_df.loc[
+                (all_inputfiles_df.date >= start_date)
+                & (all_inputfiles_df.date < end_date)
+                & (all_inputfiles_df.imagetype == imagetype)
+                & (all_inputfiles_df.band.isin(bands))
+                & (all_inputfiles_df.orbit.isin(orbits))
+            ]
+        elif sensordata_type == "S1Coh":
+            satellitetype = "S1"
+            imagetype = IMAGETYPE_S1_COHERENCE
+            bands = ["VV", "VH"]
+            orbits = ["ASC", "DESC"]
+            needed_inputfiles_df = all_inputfiles_df.loc[
+                (all_inputfiles_df.date >= start_date)
+                & (all_inputfiles_df.date < end_date)
+                & (all_inputfiles_df.imagetype == imagetype)
+                & (all_inputfiles_df.band.isin(bands))
+            ]
+        elif sensordata_type == "S2gt95":
+            satellitetype = "S2"
+            imagetype = IMAGETYPE_S2_L2A
+            bands = ["B02-10m", "B03-10m", "B04-10m", "B08-10m", "B11-20m", "B12-20m"]
+            needed_inputfiles_df = all_inputfiles_df.loc[
+                (all_inputfiles_df.date >= start_date)
+                & (all_inputfiles_df.date < end_date)
+                & (all_inputfiles_df.imagetype == imagetype)
+                & (all_inputfiles_df.band.isin(bands))
+            ]
+        elif sensordata_type == "S2-landcover":
+            satellitetype = "S2"
+            imagetype = IMAGETYPE_S2_L2A
+            bands = ["landcover"]
+            needed_inputfiles_df = all_inputfiles_df.loc[
+                (all_inputfiles_df.date >= start_date)
+                & (all_inputfiles_df.date < end_date)
+                & (all_inputfiles_df.imagetype == imagetype)
+                & (all_inputfiles_df.band.isin(bands))
+            ]
+        elif sensordata_type == "S2-ndvi":
+            satellitetype = "S2"
+            imagetype = IMAGETYPE_S2_L2A
+            bands = ["ndvi"]
+            needed_inputfiles_df = all_inputfiles_df.loc[
+                (all_inputfiles_df.date >= start_date)
+                & (all_inputfiles_df.date < end_date)
+                & (all_inputfiles_df.imagetype == imagetype)
+                & (all_inputfiles_df.band.isin(bands))
+            ]
+        else:
+            raise ValueError(f"Unsupported sensordata_type: {sensordata_type}")
+
+        # There should also be one pixcount file
+        pixcount_filename = f"{parcel_path.stem}_weekly_pixcount{output_ext}"
+        pixcount_path = dest_data_dir / pixcount_filename
+
+        # For each week
+        start_week = int(datetime.strftime(start_date, "%W"))
+        end_week = int(datetime.strftime(end_date, "%W"))
+        for period_index in range(start_week, end_week):
+            # Get the date of the first day of period period_index
+            # (eg. monday for a week)
+            period_date = datetime.strptime(
+                str(year) + "_" + str(period_index) + "_1", "%Y_%W_%w"
+            )
+
+            # New file name
+            period_date_str_long = period_date.strftime("%Y-%m-%d")
+            period_data_filename = (
+                f"{parcel_path.stem}_weekly_{period_date_str_long}_{sensordata_type}"
+                f"{output_ext}"
+            )
+            period_data_path = dest_data_dir / period_data_filename
+
+            # Check if output file exists already
+            if period_data_path.exists() and pixcount_path.exists():
+                if force is False:
+                    logger.info(
+                        f"SKIP: force is False and file exists: {period_data_path}"
+                    )
+                    continue
+                else:
+                    os.remove(period_data_path)
+
+            # Loop over bands and orbits (all combinations of bands and orbits!)
+            logger.info(f"Calculate file: {period_data_filename}")
+            period_data_df = None
+            gc.collect()  # Try to evade memory errors
+            for band, orbit in [(band, orbit) for band in bands for orbit in orbits]:
+                # Get list of files needed for this period, band
+                period_files_df = needed_inputfiles_df.loc[
+                    (needed_inputfiles_df.week == period_index)
+                    & (needed_inputfiles_df.band == band)
+                ]
+
+                # If an orbit to be filtered was specified, filter
+                if orbit is not None:
+                    period_files_df = period_files_df.loc[
+                        (period_files_df.orbit == orbit)
+                    ]
+
+                if len(period_files_df) == 0:
+                    logger.warn("No input files found!")
+
+                # Loop all period_files
+                period_band_data_df = None
+                statistic_columns_dict = {
+                    "count": [],
+                    "max": [],
+                    "mean": [],
+                    "median": [],
+                    "min": [],
+                    "std": [],
+                }
+                for j, imagedata_path in enumerate(period_files_df.path.tolist()):
+                    # If file has filesize == 0, skip
+                    imagedata_path = Path(imagedata_path)
+                    if imagedata_path.stat().st_size == 0:
+                        continue
+
+                    # Read the file (but only the columns we need)
+                    columns = [column for column in statistic_columns_dict]
+                    columns.append(id_column)
+
+                    image_data_df = pdh.read_file(imagedata_path, columns=columns)
+                    image_data_df.set_index(id_column, inplace=True)
+                    image_data_df.index.name = id_column
+
+                    # Remove rows with nan values
+                    nb_before_dropna = len(image_data_df.index)
+                    image_data_df.dropna(inplace=True)
+                    nb_after_dropna = len(image_data_df.index)
+                    if nb_after_dropna != nb_before_dropna:
+                        logger.warning(
+                            f"Before dropna: {nb_before_dropna}, after: "
+                            f"{nb_after_dropna} for file {imagedata_path}"
+                        )
+                    if nb_after_dropna == 0:
+                        continue
+
+                    # recalculate duplicate rows (the -5 buffer can cause break ups?)
+                    image_data_recalculate_df = (
+                        image_data_df.loc[image_data_df.index.duplicated()]
+                        .groupby(id_column)
+                        .agg({column: "mean" for column in statistic_columns_dict})
+                    )
+                    image_data_df = image_data_df.loc[~image_data_df.index.duplicated()]
+                    image_data_df = pd.concat(
+                        [image_data_df, image_data_recalculate_df]
+                    )
+
+                    # Rename columns so column names stay unique
+                    for statistic_column in statistic_columns_dict:
+                        new_column_name = statistic_column + str(j + 1)
+                        image_data_df.rename(
+                            columns={statistic_column: new_column_name}, inplace=True
+                        )
+                        image_data_df[new_column_name] = image_data_df[
+                            new_column_name
+                        ].astype(float)
+                        statistic_columns_dict[statistic_column].append(new_column_name)
+
+                    # Create 1 dataframe for all weekfiles
+                    #   - one row for each code_obj
+                    #   - using concat (code_obj = index)
+                    if period_band_data_df is None:
+                        period_band_data_df = image_data_df
+                    else:
+                        period_band_data_df = pd.concat(
+                            [period_band_data_df, image_data_df], axis=1, sort=False
+                        )
+                        # Apparently concat removes the index name in some situations
+                        period_band_data_df.index.name = id_column
+
+                # Calculate max, mean, min, ...
+                if period_band_data_df is not None:
+                    logger.debug("Calculate max, mean, min, ...")
+                    period_date_str_short = period_date.strftime("%Y%m%d")
+                    # Remark: prefix column names: sqlite doesn't like a numeric start
+                    if orbit is None:
+                        column_basename = (
+                            f"TS_{period_date_str_short}_{imagetype}_{band}"
+                        )
+                    else:
+                        column_basename = (
+                            f"TS_{period_date_str_short}_{imagetype}_{orbit}_{band}"
+                        )
+
+                    # Number of pixels
+                    # TODO: onderzoeken hoe aantal pixels best bijgehouden wordt:
+                    # afwijkingen weglaten ? max nemen ? ...
+                    period_band_data_df[f"{column_basename}_count"] = np.nanmax(
+                        period_band_data_df[statistic_columns_dict["count"]], axis=1
+                    )
+                    # Maximum of all max columns
+                    period_band_data_df[f"{column_basename}_max"] = np.nanmax(
+                        period_band_data_df[statistic_columns_dict["max"]], axis=1
+                    )
+                    # Mean of all mean columns
+                    period_band_data_df[f"{column_basename}_mean"] = np.nanmean(
+                        period_band_data_df[statistic_columns_dict["mean"]], axis=1
+                    )
+                    # Mean of all median columns
+                    period_band_data_df[f"{column_basename}_median"] = np.nanmean(
+                        period_band_data_df[statistic_columns_dict["median"]], axis=1
+                    )
+                    # Minimum of all min columns
+                    period_band_data_df[f"{column_basename}_min"] = np.nanmin(
+                        period_band_data_df[statistic_columns_dict["min"]], axis=1
+                    )
+                    # Mean of all std columns
+                    period_band_data_df[f"{column_basename}_std"] = np.nanmean(
+                        period_band_data_df[statistic_columns_dict["std"]], axis=1
+                    )
+                    # Number of Files used
+                    period_band_data_df[
+                        f"{column_basename}_used_files"
+                    ] = period_band_data_df[statistic_columns_dict["max"]].count(axis=1)
+
+                    # Only keep the columns we want to keep
+                    columns_to_keep = [
+                        f"{column_basename}_count",
+                        f"{column_basename}_max",
+                        f"{column_basename}_mean",
+                        f"{column_basename}_median",
+                        f"{column_basename}_min",
+                        f"{column_basename}_std",
+                        f"{column_basename}_used_files",
+                    ]
+                    period_band_data_df = period_band_data_df[columns_to_keep]
+
+                    # Merge the data with the other bands/orbits for this period
+                    if period_data_df is None:
+                        period_data_df = period_band_data_df
+                    else:
+                        period_data_df = pd.concat(
+                            [period_band_data_df, period_data_df], axis=1, sort=False
+                        )
+                        # Apparently concat removes the index name in some situations
+                        period_data_df.index.name = id_column
+
+            if period_data_df is not None:
+                logger.info(f"Write new file: {period_data_filename}")
+                pdh.to_file(period_data_df, period_data_path)
+
+                # Create pixcount file if it doesn't exist yet...
+                if not pixcount_path.exists():
+                    pixcount_s1s2_column = conf.columns["pixcount_s1s2"]
+
+                    # Get max count of all count columns available
+                    columns_to_use = [
+                        column
+                        for column in period_data_df.columns
+                        if column.endswith("_count")
+                    ]
+                    period_data_df[pixcount_s1s2_column] = np.nanmax(
+                        period_data_df[columns_to_use], axis=1
+                    )
+
+                    pixcount_df = period_data_df[pixcount_s1s2_column]
+                    pixcount_df.fillna(value=0, inplace=True)
+                    pdh.to_file(pixcount_df, pixcount_path)
+
+
+def get_fileinfo_timeseries(path: Path) -> dict:
+    """
+    This function gets info of a timeseries data file.
+
+    Args:
+        path (Path): The path to the file to get info about.
+
+    Returns:
+        dict: a dict containing info about the file
+    """
+
+    try:
+        # Split name on parcelinfo versus imageinfo
+        filename_splitted = path.stem.split("__")
+        parcel_part = filename_splitted[0]
+        imageinfo_part = filename_splitted[1]
+
+        # Extract imageinfo
+        imageinfo_values = imageinfo_part.split("_")
+        orbit = None
+        image_profile = None
+        time_dimension_reducer = None
+        if "-" in imageinfo_values[0]:
+            # OpenEO mosaic filename format
+            image_profile = imageinfo_values[0]
+            imageprofile_parts = image_profile.split("-")
+            satellite = imageprofile_parts[0]
+            product = imageprofile_parts[1]
+            if satellite == "s1":
+                if product in ["asc", "desc"]:
+                    imagetype = IMAGETYPE_S1_GRD
+                    orbit = product
+                else:
+                    imagetype = IMAGETYPE_S1_COHERENCE
+            elif satellite == "s2":
+                imagetype = IMAGETYPE_S2_L2A
+            else:
+                raise ValueError(f"invalid imageprofile in {path}")
+
+            start_date = datetime.fromisoformat(imageinfo_values[1])
+            end_date = datetime.fromisoformat(imageinfo_values[2])
+            time_dimension_reducer = imageinfo_values[4]
+            band = imageinfo_values[-1]  # =last value
+
+        else:
+            # ONDA/ESA filename format
+            # Satellite
+            satellite = imageinfo_values[0].lower()
+            # Get the date taken from the filename, depending on the satellite type
+            # Remark: the datetime is in this format: '20180101T055812'
+            if satellite.startswith("s1"):
+                # Check if it is a GRDH image
+                if imageinfo_values[2] == "GRDH":
+                    imagetype = IMAGETYPE_S1_GRD
+                    filedatetime = imageinfo_values[4]
+                elif imageinfo_values[1].startswith("S1"):
+                    imagetype = IMAGETYPE_S1_COHERENCE
+                    filedatetime = imageinfo_values[2]
+                else:
+                    raise ValueError(f"Unsupported file: {path}")
+                # Also get the orbit
+                orbit = imageinfo_values[-2].lower()  # =2nd last value
+
+            elif satellite.startswith("s2"):
+                imagetype = IMAGETYPE_S2_L2A
+                filedatetime = imageinfo_values[2]
+            else:
+                raise ValueError(f"Unsupported file: {path}")
+
+            # Parse the data found
+            filedate = filedatetime.split("T")[0]
+            parseddate = datetime.strptime(filedate, "%Y%m%d")
+            start_date = parseddate
+            end_date = start_date
+
+            # Get the band
+            band = imageinfo_values[-1]  # =last value
+
+        # Week
+        fileweek = int(start_date.strftime("%W"))
+
+        # The file paths of these files sometimes are longer than 256
+        # characters, so use trick on windows to support this anyway
+        path_safe = path.as_posix()
+        if os.name == "nt" and len(path.as_posix()) > 240:
+            if path_safe.startswith("//"):
+                path_safe = f"//?/UNC/{path_safe}"
+            else:
+                path_safe = f"//?/{path_safe}"
+
+        image_metadata = {
+            "path": path_safe,
+            "parcel_stem": parcel_part,
+            "imagetype": imagetype,
+            "filestem": path.stem,
+            "start_date": start_date,
+            "end_date": end_date,
+            "week": fileweek,
+            "band": band,
+            "orbit": orbit,  # ASC/DESC
+        }
+        if time_dimension_reducer is not None:
+            image_metadata["time_dimension_reducer"] = time_dimension_reducer
+        if image_profile is not None:
+            image_metadata["image_profile"] = image_profile
+
+    except Exception as ex:
+        message = f"Error extracting info from filename {path}"
+        logger.exception(message)
+        raise Exception(message) from ex
+
+    return image_metadata
+
+
+def get_fileinfo_timeseries_periods(path: Path) -> dict:
+    """
+    This function gets info of a period timeseries data file.
+
+    Args:
+        path (Path): The path to the file to get info about.
+
+    Returns:
+        dict: a dict containing info about the file
+    """
+    # If there is no double underscore in name: "old file type"
+    if "__" not in path.stem:
+        stem_parts = path.stem.split("_")
+        if len(stem_parts) < 4:
+            raise ValueError(f"stem doesn't contain enough parts: {path.name}")
+        period_name = stem_parts[-3]
+        start_date = datetime.fromisoformat(stem_parts[-2])
+        if period_name.lower() == "weekly":
+            end_date = start_date + timedelta(days=6)
+        else:
+            raise ValueError(f"unsupported period_name in {path}")
+        return {
+            "path": path,
+            "parcel_stem": "_".join(stem_parts[0:-3]),
+            "period_name": period_name,
+            "start_date": start_date,
+            "end_date": end_date,
+            "image_profile": stem_parts[-1],
+        }
+
+    return get_fileinfo_timeseries(path)
+
+
+def get_monday(date: Union[str, datetime]) -> datetime:
+    """
+    This function gets the first monday before the date provided.
+    It is being used to adapt start_date and end_date so they are mondays, so it
+    becomes easier to reuse timeseries data
+       - inputformat:  %Y-%m-%d
+       - outputformat: datetime
+    """
+    if isinstance(date, str):
+        date = datetime.strptime(date, "%Y-%m-%d")
+
+    year_week = date.strftime("%Y_%W")
+    year_week_monday = datetime.strptime(year_week + "_1", "%Y_%W_%w")
+    return year_week_monday
```

### Comparing `cropclassification-0.1.0a2/cropclassification.egg-info/PKG-INFO` & `cropclassification-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,60 @@
-Metadata-Version: 2.1
-Name: cropclassification
-Version: 0.1.0a2
-Summary: Package to classify crops based on sentinel images.
-Home-page: https://github.com/theroggy/cropclassification
-Author: Pieter Roggemans
-Author-email: pieter.roggemans@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
-# Crop classification
-This is a collection of scripts that can help to classify crops using Sentinel data. 
-
-Probably this documentation won't suffice to get you started, but you are free to reach out for more info if you are really interested.
-
-In general, you should also be aware that the package isn't really meant to be an easy-to-use solution for crop classification. It is rather a quite specialised solution for our specific needs. Nonetheless we want to make the code public so if anyone is interested, they can have a look and possibly get some inspiration.
-
-## Installation manual
-1. Install conda
-
-As the scripts are written in Python, you need to use a package manager to be able to install the packages the scripts depend on. The rest of the installation manual assumes you use anaconda and python 3.6+. The installer for anaconda can be found here: https://www.anaconda.com/download/.
-
-2. Create new environment and install dependencies
-
-Once you have anaconda installed, you can open an anaconda terminal window and follow the following steps:
-
-      1. Create and activate a new conda environment
-      ```
-      conda create --name cropclassification
-      conda activate cropclassification
-      conda config --env --add channels conda-forge
-      conda config --env --set channel_priority strict
-      ```
-      2. Install the dependencies for the crop classification scripts:
-      ```
-      conda install python=3.9 geopandas geofileops "h5py<3" psutil rasterio "rasterstats<0.16.0" scikit-learn
-      ```
-      3. If it was the first time you installed anaconda/geopandas, you might have to restart your computer to proceed
-      4. Start the anaconda terminal window again and activate the environment
-      ```
-      conda activate cropclassification
-      ```
-      5. Now install cropclassification and dependencies that need pip with pip
-      ```
-      pip install cropclassification
-      ```
-4. Calculate time series 
-
-To calculate time series, you need to run `cropclassification -t <tasks_dir>`, with a 'calc_timeseries' type of task in the tasks dir 
-on a server that has access to sentinel CARD images.
-
-Mind: the sentinel CARD image structure as expected for timeseries calculation depends on the image type:
-  * for Sentinel 2 images this is the standard S2 L2A format as available on the open acces copernicus hub.
-  * for Sentinel 1 backscatter and sentinel 1 coherence data this is a non-standardized data structure as there isn't a standard format (yet) for level 2 processed sentinel 1 images (as far as I know). Check out the code to see the expected data structure ;-). 
-
-5. Start a crop classification
-
-Run `cropclassification -t <tasks_dir>`, with a 'calc_marker' type of task in the tasks dir.
-
-
+Metadata-Version: 2.1
+Name: cropclassification
+Version: 0.1.1
+Summary: Package to classify crops based on sentinel images.
+Home-page: https://github.com/theroggy/cropclassification
+Author: Pieter Roggemans
+Author-email: pieter.roggemans@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
+# Crop classification
+This is a collection of scripts that can help to classify crops using Sentinel data. 
+
+Probably this documentation won't suffice to get you started, but you are free to reach out for more info if you are really interested.
+
+In general, you should also be aware that the package isn't really meant to be an easy-to-use solution for crop classification. It is rather a quite specialised solution for our specific needs. Nonetheless we want to make the code public so if anyone is interested, they can have a look and possibly get some inspiration.
+
+## Installation manual
+1. Install conda
+
+As the scripts are written in Python, you need to use a package manager to be able to install the packages the scripts depend on. The rest of the installation manual assumes you use anaconda and python 3.6+. The installer for anaconda can be found here: https://www.anaconda.com/download/.
+
+2. Create new environment and install dependencies
+
+Once you have anaconda installed, you can open an anaconda terminal window and follow the following steps:
+
+      1. Create and activate a new conda environment
+      ```
+      conda create --name cropclassification
+      conda activate cropclassification
+      conda config --env --add channels conda-forge
+      conda config --env --set channel_priority strict
+      ```
+      2. Install the dependencies for the crop classification scripts:
+      ```
+      conda install python=3.9 geopandas geofileops "h5py<3" openeo psutil qgis rasterio rasterstats scikit-learn
+      ```
+      3. If it was the first time you installed anaconda/geopandas, you might have to restart your computer to proceed
+      4. Start the anaconda terminal window again and activate the environment
+      ```
+      conda activate cropclassification
+      ```
+      5. Now install cropclassification and dependencies that need pip with pip
+      ```
+      pip install cropclassification
+      ```
+4. Calculate time series 
+
+To calculate time series, you need to run `cropclassification -t <tasks_dir>`, with a 'calc_timeseries' type of task in the tasks dir 
+on a server that has access to sentinel CARD images.
+
+Mind: the sentinel CARD image structure as expected for timeseries calculation depends on the image type:
+  * for Sentinel 2 images this is the standard S2 L2A format as available on the open acces copernicus hub.
+  * for Sentinel 1 backscatter and sentinel 1 coherence data this is a non-standardized data structure as there isn't a standard format (yet) for level 2 processed sentinel 1 images (as far as I know). Check out the code to see the expected data structure ;-). 
+
+5. Start a crop classification
+
+Run `cropclassification -t <tasks_dir>`, with a 'calc_marker' type of task in the tasks dir.
```

### Comparing `cropclassification-0.1.0a2/cropclassification.egg-info/SOURCES.txt` & `cropclassification-0.1.1/cropclassification.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -28,13 +28,23 @@
 cropclassification/postprocess/html_rapport_test.py
 cropclassification/predict/__init__.py
 cropclassification/predict/classification.py
 cropclassification/predict/classification_keras.py
 cropclassification/predict/classification_sklearn.py
 cropclassification/predict/multicrop.py
 cropclassification/preprocess/__init__.py
+cropclassification/preprocess/_classification_preprocess_BEFL.py
+cropclassification/preprocess/_timeseries_calc_openeo.py
+cropclassification/preprocess/_timeseries_helper.py
 cropclassification/preprocess/classification_preprocess.py
-cropclassification/preprocess/classification_preprocess_BEFL.py
 cropclassification/preprocess/timeseries.py
-cropclassification/preprocess/timeseries_calc_dias_onda_per_image.py
-cropclassification/preprocess/timeseries_calc_gee.py
-cropclassification/preprocess/timeseries_util.py
+cropclassification/util/__init__.py
+cropclassification/util/geoops_util.py
+cropclassification/util/io_util.py
+cropclassification/util/openeo_util.py
+cropclassification/util/zonal_stats_bulk/__init__.py
+cropclassification/util/zonal_stats_bulk/_general_helper.py
+cropclassification/util/zonal_stats_bulk/_raster_helper.py
+cropclassification/util/zonal_stats_bulk/_vector_helper.py
+cropclassification/util/zonal_stats_bulk/_zonal_stats_bulk_pyqgis.py
+cropclassification/util/zonal_stats_bulk/_zonal_stats_bulk_rs.py
+tests/test_calc_timeseries.py
```

### Comparing `cropclassification-0.1.0a2/setup.py` & `cropclassification-0.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-with open("cropclassification/version.txt", mode="r") as file:
-    version = file.readline()
-
-setuptools.setup(
-    name="cropclassification",
-    version=version,
-    author="Pieter Roggemans",
-    author_email="pieter.roggemans@gmail.com",
-    description="Package to classify crops based on sentinel images.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/theroggy/cropclassification",
-    packages=setuptools.find_packages(),
-    include_package_data=True,
-    install_requires=[
-        "geofileops",
-        "geopandas",
-        "psutil",
-        "rasterio",
-        "rasterstats",
-        "scikit-learn",
-        "tensorflow",
-    ],
-    entry_points="""
-        [console_scripts]
-        cropclassification=cropclassification.cropclassification:main
-        """,
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "Operating System :: OS Independent",
-    ],
-    python_requires=">=3.9",
-)
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+with open("cropclassification/version.txt", mode="r") as file:
+    version = file.readline()
+
+setuptools.setup(
+    name="cropclassification",
+    version=version,
+    author="Pieter Roggemans",
+    author_email="pieter.roggemans@gmail.com",
+    description="Package to classify crops based on sentinel images.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/theroggy/cropclassification",
+    packages=setuptools.find_packages(),
+    include_package_data=True,
+    install_requires=[
+        "geofileops",
+        "geopandas",
+        "openeo",
+        "psutil",
+        "rasterio",
+        "rasterstats",
+        "scikit-learn",
+        "tensorflow",
+    ],
+    entry_points="""
+        [console_scripts]
+        cropclassification=cropclassification.cropclassification:main
+        """,
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Operating System :: OS Independent",
+    ],
+    python_requires=">=3.9",
+)
```

