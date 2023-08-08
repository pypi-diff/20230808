# Comparing `tmp/copernicus_marine_client-0.8.7.tar.gz` & `tmp/copernicus_marine_client-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copernicus_marine_client-0.8.7.tar", max compression
+gzip compressed data, was "copernicus_marine_client-0.8.8.tar", max compression
```

## Comparing `copernicus_marine_client-0.8.7.tar` & `copernicus_marine_client-0.8.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    10338 2023-07-18 12:07:01.367586 copernicus_marine_client-0.8.7/README.md
--rw-r--r--   0        0        0     3171 2023-07-19 14:56:29.896705 copernicus_marine_client-0.8.7/copernicus_marine_client/__init__.py
--rw-r--r--   0        0        0       10 2023-02-28 13:18:03.224455 copernicus_marine_client-0.8.7/copernicus_marine_client/catalogue_parser/__init__.py
--rw-r--r--   0        0        0    22039 2023-07-19 14:56:29.896705 copernicus_marine_client-0.8.7/copernicus_marine_client/catalogue_parser/catalogue_parser.py
--rw-r--r--   0        0        0     6162 2023-07-19 12:55:05.604908 copernicus_marine_client-0.8.7/copernicus_marine_client/catalogue_parser/request_structure.py
--rw-r--r--   0        0        0       10 2023-02-28 13:18:03.224455 copernicus_marine_client-0.8.7/copernicus_marine_client/command_line_interface/__init__.py
--rw-r--r--   0        0        0      994 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.7/copernicus_marine_client/command_line_interface/copernicus_marine.py
--rw-r--r--   0        0        0     3539 2023-07-17 16:09:12.015945 copernicus_marine_client-0.8.7/copernicus_marine_client/command_line_interface/group_describe.py
--rw-r--r--   0        0        0     4907 2023-07-19 14:56:34.580720 copernicus_marine_client-0.8.7/copernicus_marine_client/command_line_interface/group_login.py
--rw-r--r--   0        0        0     8870 2023-07-17 09:14:07.365808 copernicus_marine_client-0.8.7/copernicus_marine_client/command_line_interface/group_native.py
--rw-r--r--   0        0        0    17056 2023-07-19 14:56:29.900705 copernicus_marine_client-0.8.7/copernicus_marine_client/command_line_interface/group_subset.py
--rw-r--r--   0        0        0     5953 2023-07-19 14:56:34.580720 copernicus_marine_client-0.8.7/copernicus_marine_client/configuration_files_creator.py
--rw-r--r--   0        0        0     7642 2023-07-18 12:07:01.367586 copernicus_marine_client-0.8.7/copernicus_marine_client/download_functions/download_ftp.py
--rw-r--r--   0        0        0     4209 2023-07-18 12:07:01.367586 copernicus_marine_client-0.8.7/copernicus_marine_client/download_functions/download_motu.py
--rw-r--r--   0        0        0     1328 2023-07-18 12:07:01.367586 copernicus_marine_client-0.8.7/copernicus_marine_client/download_functions/download_native.py
--rw-r--r--   0        0        0     8748 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.7/copernicus_marine_client/download_functions/download_opendap.py
--rw-r--r--   0        0        0     7994 2023-07-19 14:56:40.352739 copernicus_marine_client-0.8.7/copernicus_marine_client/download_functions/download_s3native.py
--rw-r--r--   0        0        0     4395 2023-07-18 12:07:01.371586 copernicus_marine_client-0.8.7/copernicus_marine_client/download_functions/download_zarr.py
--rw-r--r--   0        0        0     6966 2023-07-18 12:07:01.371586 copernicus_marine_client-0.8.7/copernicus_marine_client/download_functions/subset_xarray.py
--rw-r--r--   0        0        0      768 2023-07-04 12:33:19.408010 copernicus_marine_client-0.8.7/copernicus_marine_client/logging_conf.json
--rw-r--r--   0        0        0      623 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.7/copernicus_marine_client/utils.py
--rw-r--r--   0        0        0      887 2023-07-19 15:46:15.399516 copernicus_marine_client-0.8.7/pyproject.toml
--rw-r--r--   0        0        0    11876 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.7/setup.py
--rw-r--r--   0        0        0    11273 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0    10338 2023-07-18 12:07:01.367586 copernicus_marine_client-0.8.8/README.md
+-rw-r--r--   0        0        0     3171 2023-07-20 14:10:39.999004 copernicus_marine_client-0.8.8/copernicus_marine_client/__init__.py
+-rw-r--r--   0        0        0       10 2023-02-28 13:18:03.224455 copernicus_marine_client-0.8.8/copernicus_marine_client/catalogue_parser/__init__.py
+-rw-r--r--   0        0        0    22039 2023-07-20 16:18:47.508466 copernicus_marine_client-0.8.8/copernicus_marine_client/catalogue_parser/catalogue_parser.py
+-rw-r--r--   0        0        0     6162 2023-07-19 12:55:05.604908 copernicus_marine_client-0.8.8/copernicus_marine_client/catalogue_parser/request_structure.py
+-rw-r--r--   0        0        0       10 2023-02-28 13:18:03.224455 copernicus_marine_client-0.8.8/copernicus_marine_client/command_line_interface/__init__.py
+-rw-r--r--   0        0        0      994 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.8/copernicus_marine_client/command_line_interface/copernicus_marine.py
+-rw-r--r--   0        0        0     3539 2023-07-20 16:18:47.508466 copernicus_marine_client-0.8.8/copernicus_marine_client/command_line_interface/group_describe.py
+-rw-r--r--   0        0        0     4907 2023-07-20 14:09:35.966782 copernicus_marine_client-0.8.8/copernicus_marine_client/command_line_interface/group_login.py
+-rw-r--r--   0        0        0     8870 2023-07-17 09:14:07.365808 copernicus_marine_client-0.8.8/copernicus_marine_client/command_line_interface/group_native.py
+-rw-r--r--   0        0        0    17056 2023-07-20 16:18:47.508466 copernicus_marine_client-0.8.8/copernicus_marine_client/command_line_interface/group_subset.py
+-rw-r--r--   0        0        0     5953 2023-07-20 14:09:35.966782 copernicus_marine_client-0.8.8/copernicus_marine_client/configuration_files_creator.py
+-rw-r--r--   0        0        0     7642 2023-07-18 12:07:01.367586 copernicus_marine_client-0.8.8/copernicus_marine_client/download_functions/download_ftp.py
+-rw-r--r--   0        0        0     4209 2023-07-18 12:07:01.367586 copernicus_marine_client-0.8.8/copernicus_marine_client/download_functions/download_motu.py
+-rw-r--r--   0        0        0     1328 2023-07-18 12:07:01.367586 copernicus_marine_client-0.8.8/copernicus_marine_client/download_functions/download_native.py
+-rw-r--r--   0        0        0     8748 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.8/copernicus_marine_client/download_functions/download_opendap.py
+-rw-r--r--   0        0        0     7994 2023-07-20 14:09:35.966782 copernicus_marine_client-0.8.8/copernicus_marine_client/download_functions/download_s3native.py
+-rw-r--r--   0        0        0     4395 2023-07-18 12:07:01.371586 copernicus_marine_client-0.8.8/copernicus_marine_client/download_functions/download_zarr.py
+-rw-r--r--   0        0        0     6972 2023-07-20 16:25:04.973802 copernicus_marine_client-0.8.8/copernicus_marine_client/download_functions/subset_xarray.py
+-rw-r--r--   0        0        0      768 2023-07-04 12:33:19.408010 copernicus_marine_client-0.8.8/copernicus_marine_client/logging_conf.json
+-rw-r--r--   0        0        0      623 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.8/copernicus_marine_client/utils.py
+-rw-r--r--   0        0        0      887 2023-07-20 16:36:51.280319 copernicus_marine_client-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0    11876 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.8/setup.py
+-rw-r--r--   0        0        0    11273 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.8/PKG-INFO
```

### Comparing `copernicus_marine_client-0.8.7/README.md` & `copernicus_marine_client-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/__init__.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/__init__.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/catalogue_parser/catalogue_parser.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/catalogue_parser/catalogue_parser.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/catalogue_parser/request_structure.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/catalogue_parser/request_structure.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/command_line_interface/copernicus_marine.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/command_line_interface/copernicus_marine.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/command_line_interface/group_describe.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/command_line_interface/group_describe.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/command_line_interface/group_login.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/command_line_interface/group_login.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/command_line_interface/group_native.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/command_line_interface/group_native.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/command_line_interface/group_subset.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/command_line_interface/group_subset.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/configuration_files_creator.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/configuration_files_creator.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/download_functions/download_ftp.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/download_functions/download_ftp.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/download_functions/download_motu.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/download_functions/download_motu.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/download_functions/download_native.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/download_functions/download_native.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/download_functions/download_opendap.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/download_functions/download_opendap.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/download_functions/download_s3native.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/download_functions/download_s3native.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/download_functions/download_zarr.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/download_functions/download_zarr.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/download_functions/subset_xarray.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/download_functions/subset_xarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             if coord_label in dataset.coords:
                 attrs = dataset[coord_label].attrs
                 if attrs["valid_min"]:
                     attrs["valid_min"] += 180
                 if attrs["valid_max"]:
                     attrs["valid_max"] += 180
                 dataset = dataset.assign_coords(
-                    {coord_label: (dataset[coord_label] + 180.0)}
+                    {coord_label: (dataset[coord_label] + 360.0) % 360}
                 ).sortby(coord_label)
                 dataset[coord_label].attrs = attrs
         return dataset
 
     if minimal_longitude is not None or maximal_longitude is not None:
         if minimal_longitude is not None and maximal_longitude is not None:
             if minimal_longitude > maximal_longitude:
```

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/logging_conf.json` & `copernicus_marine_client-0.8.8/copernicus_marine_client/logging_conf.json`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/copernicus_marine_client/utils.py` & `copernicus_marine_client-0.8.8/copernicus_marine_client/utils.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.7/pyproject.toml` & `copernicus_marine_client-0.8.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copernicus-marine-client"
-version = "0.8.7"
+version = "0.8.8"
 description = ""
 authors = ["jsouchard <jsouchard@mercator-ocean.fr>"]
 readme = "README.md"
 packages = [{include = "copernicus_marine_client"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `copernicus_marine_client-0.8.7/setup.py` & `copernicus_marine_client-0.8.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 entry_points = \
 {'console_scripts': ['copernicus-marine = '
                      'copernicus_marine_client.command_line_interface.copernicus_marine:command_line_interface']}
 
 setup_kwargs = {
     'name': 'copernicus-marine-client',
-    'version': '0.8.7',
+    'version': '0.8.8',
     'description': '',
     'long_description': '# Copernicus Marine Service client\n\nA library to facilitate the access of Copernicus Marine Service products and datasets.\n\n## Introduction\n\nThis package allows to recover products and datasets information from Command Line Interface or with Python code,\nas well as download subsets and native files.\n\n## Command Line Interface (CLI)\n\n### Command *describe*\n\nRetrieve information about all products as JSON:\n\n```txt\n> copernicus-marine describe\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n    }\n    ...\n  ]\n}\n```\n\nRetrieve all information about datasets as JSON:\n\n```txt\n> copernicus-marine describe --include-datasets\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n      "datasets": [\n        {\n          "dataset_id": "antarctic_omi_si_extent",\n          "dataset_name": "antarctic_omi_si_extent",\n          "services": [\n            {\n              "protocol": "ftp",\n              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"\n            }\n          ],\n          "variables": []\n        }\n      ]\n    },\n    ...\n  ]\n}\n```\n\n### Command *login*\n\nCreate the configuration files for access to the copernicus marine service:\n\'.dodsrc\', \'.netrc\', \'.motuclient-python.ini\'.\nThe directory to store these configuration files can be modified by the user using the "config-file-directory" option\nbut beware as it should also be passed to the *subset* and *native* command afterwards.\nBy default, if the configuration files already exist, the user is asked for confirmation to overwrite them.\n\nExample:\n```\n> copernicus marine login\n< Username :\n< Password :\n> INFO     - root - Configuration files stored in ${HOME}\\.copernicus_marine_client\n```\n\n### Command *subset*\n\nDownload a dataset subset, based on dataset id, variable names and attributes slices:\n\n```txt\n> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\n< Username:\n< Password:\n< Trying to download as one file...\n```\n\nFile downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options). If the output-filename argument ends with \'.nc\' suffix, the file will be downloaded as a netCDF file.\n\nOptions `--minimal-longitude FLOAT` and `--maximal-longitude FLOAT` work as follow:\n1. If `maximal-longitude - minimal-longitude >= 360`, return the full dataset.\n2. Else:\n    - If the requested range **does not cross** the antemeridian, the result dataset will be between -180° and 180°.\n    - If it **does cross** the antemeridian, the result dataset will be between 0° and 360°.\n\nNote that you can request any longitudes you want. A modulus is applied to bring the result between -180° and 360°. For example, if you request [530°, 560°], the result dataset will be in [170°, 190°].\n\n### Command *native*\n\nDownload a native file (or files), based on dataset id or path to files:\n\nExample:\n\n```txt\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/\n\n< Username:\n< Password:\n< You requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB\n\nTotal size of the download: 19.62 MB\n\n\nDo you want to proceed with download? [y/N]:\n```\n\nFile(s) downloaded to ./{path}/{filename} if not specified otherwise:\n\n- "--output-path" specifies a directory to dump the files in\n- "--no-directories" to not recreate the folder structure\n\nIf not specified otherwise, after the header display with a summary of the request,\nthe user is asked for confirmation:\n\n- "--no-confirmation" to turn down the confirmation prompt\n- "--show-outputnames" to display the full paths of the outputs files\n\nOption `--filter TEXT` allows to specify a Unix shell-style wildcard pattern (see [fnmatch — Unix filename pattern matching](https://docs.python.org/3/library/fnmatch.html)) and select specific files. It work with both `--dataset-id` and `--dataset-url` options.\n\nOption `--regex TEXT` allows to specify a regular expression and select specific files. It work with both `--dataset-id` and `--dataset-url` options.\n\nExample:\n```\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m --regex ".*2022(08|09|10).nc"\nPassword:\nYou requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\n\nTotal size of the download: 9.82 MB\n\n\nDo you want to proceed with download? [y/N]:\n```\n\n### The overwrite option\n\nBoth `native` and `subset` commands provide an `--overwrite-ouput-data` option.\nWhen not provided (default behavior), once the download has been accepted (or if the `--force-download` option was provided), if the file already exists on destination, then a new one with a unique index will be created.\nOn the other hand, if the `--overwrite-ouput-data` option is provided and the file already exists, then it\'ll be overwritten.\n\n### The `--help` argument\n\nIn any case, please remember that you can call the `--help` argument on any CLI option. This may save you some time or find what you need.\n\n## Python functions\n\nThe library also provide python functions to help with catalogue\nbrowsing and datasets download in scripts.\n\n### Basic example\n\nIn this example 4 steps are performed:\n  1- Fetch the catalogue to select a dataset\n  2- Construct a SubsetRequest for this dataset\n  3- Download the subset as a zarr store\n  4- Open the subset as an xarray dataset\n\n```python\nimport copernicus_marine_client as cmc\n\n# Step 1: Fetch catalogue and parse information on dataset\ncatalogue = cmc.fetch_catalogue()\ndataset_id = "cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m"\nassert dataset_id in cmc.get_all_dataset_ids()\ndataset = catalogue.filter([dataset_id]).products[0].datasets[0]\n# Object "dataset" can be used to display all the metadata necessary to build a SubsetRequest\nvariable = [\n    variable for variable in dataset.variables if variable.short_name in ["zooc"]\n][0]\ncoordinates = {\n    coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value)\n    for coordinate in variable.coordinates\n}\n\n# Step 2: Construct the request based on parsed information\nsubset_request = cmc.SubsetRequest(\n    dataset_id="cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m",\n    start_datetime="2023-04-20",\n    end_datetime="2023-04-21",\n    minimal_latitude=30.0,\n    maximal_latitude=30.1,\n    minimal_longitude=0.1,\n    maximal_longitude=0.2,\n    minimal_depth=100,\n    maximal_depth=1000,\n    variables=["zooc"],\n    force_protocol="zarr-map",\n    output_directory="data_folder",\n    output_filename="datastore.zarr",\n    force_download=True,\n)\n\n# Step 3: Download the subset based on request content\nfilename = cmc.download_subset(\n    login="FAKE_LOGIN", password="FAKE_PASSWORD", subset_request=subset_request\n)\n\n# Step 4: Open the downloaded subset as an xarray dataset\nsubset = cmc.open_dataset(filepath=filename, engine="zarr", out_type="xarray")\n```\n\n## Installation\n\nUsing pip, for example:\n\n```shell\npip install copernicus-marine-client\n```\n\n## Technical details\n\nThis module is organized around two capabilities:\n\n- a catalogue, parsed from web requests, that contains informations on the available datasets\n- a downloader, to simplify the download of dataset files or subsets\n\nThe catalogue can be displayed by the user and is used by the downloader to link the user\nrequests with files or subset of files to retrieve.\nThe downloader will help the user download the needed datasets.\n\nA rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.\n\nFor subset command, the format is:\n\n```python\n@dataclass\nclass SubsetRequest:\n    dataset_url: Optional[str] = None\n    dataset_id: Optional[str] = None\n    variables: Optional[List[str]] = None\n    minimal_longitude: Optional[float] = None\n    maximal_longitude: Optional[float] = None\n    minimal_latitude: Optional[float] = None\n    maximal_latitude: Optional[float] = None\n    minimal_depth: Optional[float] = None\n    maximal_depth: Optional[float] = None\n    start_datetime: Optional[datetime] = None\n    end_datetime: Optional[datetime] = None\n    output_directory: Optional[str] = None\n    output_filename: Optional[str] = None\n    force_download: Optional[bool] = None\n    force_protocol: Optional[str] = None\n```\n',
     'author': 'jsouchard',
     'author_email': 'jsouchard@mercator-ocean.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `copernicus_marine_client-0.8.7/PKG-INFO` & `copernicus_marine_client-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copernicus-marine-client
-Version: 0.8.7
+Version: 0.8.8
 Summary: 
 Author: jsouchard
 Author-email: jsouchard@mercator-ocean.fr
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

