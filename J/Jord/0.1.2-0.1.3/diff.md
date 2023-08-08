# Comparing `tmp/Jord-0.1.2.tar.gz` & `tmp/Jord-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jord-0.1.2.tar", last modified: Tue Aug  1 06:14:07 2023, max compression
+gzip compressed data, was "Jord-0.1.3.tar", last modified: Tue Aug  8 06:54:15 2023, max compression
```

## Comparing `Jord-0.1.2.tar` & `Jord-0.1.3.tar`

### file list

```diff
@@ -1,151 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.328316 Jord-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.308315 Jord-0.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-08-01 06:13:58.000000 Jord-0.1.2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-01 06:13:58.000000 Jord-0.1.2/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 06:13:58.000000 Jord-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:13:58.000000 Jord-0.1.2/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.312315 Jord-0.1.2/Jord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-08-01 06:14:07.000000 Jord-0.1.2/Jord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-08-01 06:14:07.000000 Jord-0.1.2/Jord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:14:07.000000 Jord-0.1.2/Jord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-01 06:14:07.000000 Jord-0.1.2/Jord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 06:14:07.000000 Jord-0.1.2/Jord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 06:13:58.000000 Jord-0.1.2/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-08-01 06:13:58.000000 Jord-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-01 06:13:58.000000 Jord-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-08-01 06:14:07.328316 Jord-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-01 06:13:58.000000 Jord-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-01 06:13:58.000000 Jord-0.1.2/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.312315 Jord-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 06:13:58.000000 Jord-0.1.2/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.312315 Jord-0.1.2/jord/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.312315 Jord-0.1.2/jord/gdal_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/cloning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/importing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/gdal_utilities/spatial_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.312315 Jord-0.1.2/jord/geojson_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/geojson_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/geojson_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/geojson_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.312315 Jord-0.1.2/jord/geopandas_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/geopandas_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/geopandas_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/geopandas_utilities/geometry_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/geopandas_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.316315 Jord-0.1.2/jord/pillow_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/pillow_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/pillow_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/pillow_utilities/exif.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/pillow_utilities/tiff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.316315 Jord-0.1.2/jord/qgis_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/categorisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.316315 Jord-0.1.2/jord/qgis_utilities/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/configuration/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/configuration/plugin_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/configuration/project_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.316315 Jord-0.1.2/jord/qgis_utilities/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/conversion/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/conversion/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.316315 Jord-0.1.2/jord/qgis_utilities/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/helpers/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.320315 Jord-0.1.2/jord/qgis_utilities/numpy_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/numpy_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/numpy_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/numpy_utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/numpy_utilities/data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/numpy_utilities/rasters.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/plugin_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.320315 Jord-0.1.2/jord/qgis_utilities/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/qlive_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/qlive_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/qlive_utilities/procedure_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/qlive_utilities/rpc_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.320315 Jord-0.1.2/jord/qgis_utilities/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/shapely_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/shapely_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qgis_utilities/styling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.320315 Jord-0.1.2/jord/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.320315 Jord-0.1.2/jord/qlive_utilities/clients/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/clients/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/clients/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/clients/interfaced.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/procedures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/qgis_layer_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/serialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qlive_utilities/uri_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.320315 Jord-0.1.2/jord/qt_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qt_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19517 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/qt_utilities/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.320315 Jord-0.1.2/jord/rasterio_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/rasterio_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/rasterio_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.324316 Jord-0.1.2/jord/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.324316 Jord-0.1.2/jord/shapely_utilities/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/analysis/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/analysis/degrees_of_freedom.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/analysis/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/clamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/geometry_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/mirroring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/points.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/sanitise_poly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.324316 Jord-0.1.2/jord/shapely_utilities/serialisation/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/serialisation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/serialisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/serialisation/well_known_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/serialisation/well_known_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/shapely_utilities/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.324316 Jord-0.1.2/jord/spatialite_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/spatialite_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/spatialite_utilities/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.324316 Jord-0.1.2/jord/torch_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/torch_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/torch_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-01 06:13:58.000000 Jord-0.1.2/jord/torch_utilities/geodata_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-01 06:13:58.000000 Jord-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 06:13:58.000000 Jord-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-01 06:14:07.328316 Jord-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-08-01 06:13:58.000000 Jord-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.328316 Jord-0.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:14:07.328316 Jord-0.1.2/tests/qgis/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-01 06:13:58.000000 Jord-0.1.2/tests/qgis/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-08-01 06:13:58.000000 Jord-0.1.2/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-01 06:13:58.000000 Jord-0.1.2/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.461615 Jord-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.441615 Jord-0.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-08-08 06:54:10.000000 Jord-0.1.3/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-08 06:54:10.000000 Jord-0.1.3/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-08 06:54:10.000000 Jord-0.1.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:10.000000 Jord-0.1.3/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.441615 Jord-0.1.3/Jord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-08-08 06:54:15.000000 Jord-0.1.3/Jord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-08 06:54:15.000000 Jord-0.1.3/Jord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 06:54:15.000000 Jord-0.1.3/Jord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-08 06:54:15.000000 Jord-0.1.3/Jord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 06:54:15.000000 Jord-0.1.3/Jord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 06:54:10.000000 Jord-0.1.3/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-08-08 06:54:10.000000 Jord-0.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-08 06:54:10.000000 Jord-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-08-08 06:54:15.461615 Jord-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-08 06:54:10.000000 Jord-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-08 06:54:10.000000 Jord-0.1.3/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.441615 Jord-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-08 06:54:10.000000 Jord-0.1.3/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.441615 Jord-0.1.3/jord/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.445615 Jord-0.1.3/jord/gdal_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/gdal_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/gdal_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/gdal_utilities/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/gdal_utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/gdal_utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/gdal_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/gdal_utilities/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/gdal_utilities/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/gdal_utilities/spatial_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.445615 Jord-0.1.3/jord/geojson_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/geojson_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/geojson_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/geojson_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.445615 Jord-0.1.3/jord/geopandas_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/geopandas_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/geopandas_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/geopandas_utilities/geometry_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/geopandas_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.445615 Jord-0.1.3/jord/pillow_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/pillow_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/pillow_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/pillow_utilities/exif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/pillow_utilities/tiff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.449615 Jord-0.1.3/jord/qgis_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/categorisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.449615 Jord-0.1.3/jord/qgis_utilities/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/configuration/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/configuration/plugin_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/configuration/project_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.449615 Jord-0.1.3/jord/qgis_utilities/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/conversion/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/conversion/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12952 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.453615 Jord-0.1.3/jord/qgis_utilities/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/helpers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/helpers/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/helpers/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/helpers/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/helpers/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/helpers/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/helpers/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/helpers/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.453615 Jord-0.1.3/jord/qgis_utilities/numpy_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/numpy_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/numpy_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/numpy_utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/numpy_utilities/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/numpy_utilities/rasters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/plugin_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qgis_utilities/styling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.453615 Jord-0.1.3/jord/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qlive_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qlive_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qlive_utilities/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.457615 Jord-0.1.3/jord/qlive_utilities/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qlive_utilities/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qlive_utilities/clients/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qlive_utilities/clients/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qlive_utilities/clients/interfaced.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qlive_utilities/procedures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qlive_utilities/qgis_layer_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qlive_utilities/serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qlive_utilities/uri_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.457615 Jord-0.1.3/jord/qt_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qt_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19517 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/qt_utilities/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.457615 Jord-0.1.3/jord/rasterio_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/rasterio_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/rasterio_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.457615 Jord-0.1.3/jord/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.461615 Jord-0.1.3/jord/shapely_utilities/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/analysis/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/analysis/degrees_of_freedom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/analysis/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/clamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/geometry_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34069 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/mirroring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/rings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.461615 Jord-0.1.3/jord/shapely_utilities/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/serialisation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/serialisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/serialisation/fiona_utilties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/serialisation/well_known_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/serialisation/well_known_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/shapely_utilities/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.461615 Jord-0.1.3/jord/spatialite_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/spatialite_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/spatialite_utilities/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.461615 Jord-0.1.3/jord/torch_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/torch_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/torch_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-08 06:54:10.000000 Jord-0.1.3/jord/torch_utilities/geodata_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-08 06:54:10.000000 Jord-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 06:54:10.000000 Jord-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-08 06:54:15.465615 Jord-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-08-08 06:54:10.000000 Jord-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.461615 Jord-0.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:54:15.461615 Jord-0.1.3/tests/qgis/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 06:54:10.000000 Jord-0.1.3/tests/qgis/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-08-08 06:54:10.000000 Jord-0.1.3/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-08 06:54:10.000000 Jord-0.1.3/tests/test_sanity.py
```

### Comparing `Jord-0.1.2/.github/CODE_OF_CONDUCT.md` & `Jord-0.1.3/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/.github/CONTRIBUTING.md` & `Jord-0.1.3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/Jord.egg-info/SOURCES.txt` & `Jord-0.1.3/Jord.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -67,21 +67,14 @@
 jord/qgis_utilities/helpers/timestamp.py
 jord/qgis_utilities/numpy_utilities/README.md
 jord/qgis_utilities/numpy_utilities/__init__.py
 jord/qgis_utilities/numpy_utilities/conversion.py
 jord/qgis_utilities/numpy_utilities/data_type.py
 jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
 jord/qgis_utilities/numpy_utilities/rasters.py
-jord/qgis_utilities/qlive_utilities/README.md
-jord/qgis_utilities/qlive_utilities/__init__.py
-jord/qgis_utilities/qlive_utilities/procedure_implementation.py
-jord/qgis_utilities/qlive_utilities/rpc_protocol.py
-jord/qgis_utilities/shapely_utilities/README.md
-jord/qgis_utilities/shapely_utilities/__init__.py
-jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py
 jord/qlive_utilities/README.md
 jord/qlive_utilities/__init__.py
 jord/qlive_utilities/client.py
 jord/qlive_utilities/procedures.py
 jord/qlive_utilities/qgis_layer_creation.py
 jord/qlive_utilities/serialisation.py
 jord/qlive_utilities/uri_utilities.py
@@ -93,28 +86,29 @@
 jord/qt_utilities/enums.py
 jord/rasterio_utilities/README.md
 jord/rasterio_utilities/__init__.py
 jord/shapely_utilities/README.md
 jord/shapely_utilities/__init__.py
 jord/shapely_utilities/clamp.py
 jord/shapely_utilities/geometry_types.py
-jord/shapely_utilities/iteration.py
 jord/shapely_utilities/lines.py
 jord/shapely_utilities/mirroring.py
 jord/shapely_utilities/morphology.py
 jord/shapely_utilities/points.py
+jord/shapely_utilities/polygons.py
 jord/shapely_utilities/projection.py
-jord/shapely_utilities/sanitise_poly.py
+jord/shapely_utilities/rings.py
 jord/shapely_utilities/transformation.py
 jord/shapely_utilities/analysis/README.md
 jord/shapely_utilities/analysis/__init__.py
 jord/shapely_utilities/analysis/degrees_of_freedom.py
 jord/shapely_utilities/analysis/tracing.py
 jord/shapely_utilities/serialisation/README.md
 jord/shapely_utilities/serialisation/__init__.py
+jord/shapely_utilities/serialisation/fiona_utilties.py
 jord/shapely_utilities/serialisation/well_known_binary.py
 jord/shapely_utilities/serialisation/well_known_text.py
 jord/spatialite_utilities/__init__.py
 jord/spatialite_utilities/loading.py
 jord/torch_utilities/README.md
 jord/torch_utilities/__init__.py
 jord/torch_utilities/geodata_dataset.py
```

### Comparing `Jord-0.1.2/Jord.egg-info/requires.txt` & `Jord-0.1.3/Jord.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 numpy>=1.20.2
 warg>=1.1.6
 apppath>=1.0.2
 sorcery
 pyzmq
 tqdm
+sympy
 
 [all]
+mock
+Pillow
 pytest>=4.4.1
+tqdm
+pyzmq
+sphinx>=4.0.1
+apppath>=1.0.2
+sphinxcontrib-programoutput
+numpy>=1.20.2
+pip>=22.1.2
 coveralls>=1.6.0
+pytest-cov>=2.11.1
+sympy
 furo
-Pillow
-numpy>=1.20.2
 warg>=1.1.6
-mock
-apppath>=1.0.2
+pytest>=4.3.0
 sorcery
 pre-commit>=2.17.0
-tqdm
-sphinxcontrib-programoutput
-twine>=1.13.0
-sphinx>=4.0.1
-wheel>=0.33.0
 black[jupyter]>=21.5b0
-pip>=22.1.2
-pytest>=4.3.0
-pyzmq
-pytest-cov>=2.11.1
+wheel>=0.33.0
+twine>=1.13.0
 
 [dev]
+mock
 pytest>=4.4.1
+tqdm
+pyzmq
+sphinx>=4.0.1
+apppath>=1.0.2
+sphinxcontrib-programoutput
+numpy>=1.20.2
+pip>=22.1.2
 coveralls>=1.6.0
+pytest-cov>=2.11.1
+twine>=1.13.0
+sympy
 furo
-mock
-numpy>=1.20.2
 warg>=1.1.6
-apppath>=1.0.2
+pytest>=4.3.0
 sorcery
 pre-commit>=2.17.0
-sphinxcontrib-programoutput
-tqdm
-twine>=1.13.0
-sphinx>=4.0.1
-wheel>=0.33.0
 black[jupyter]>=21.5b0
-pip>=22.1.2
-pytest>=4.3.0
-pyzmq
-pytest-cov>=2.11.1
+wheel>=0.33.0
 
 [docs]
-sphinx>=4.0.1
 sphinxcontrib-programoutput
+sphinx>=4.0.1
 furo
 
 [extra]
 
 [gdal]
 
 [pil]
```

### Comparing `Jord-0.1.2/LICENSE.md` & `Jord-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/README.md` & `Jord-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -4,16 +4,16 @@
   <img src=".github/images/header.svg" alt='header' />
 </p>
 
 <h1 align="center">Jord</h1>
 
 <!--# Jord-->
 
-| [![Build Status](https://travis-ci.org/aivclab/jord.svg?branch=master)](https://travis-ci.org/aivclab/jord) | [![Coverage Status](https://coveralls.io/repos/github/aivclab/vision/badge.svg?branch=master)](https://coveralls.io/github/aivclab/vision?branch=master) | [![GitHub Issues](https://img.shields.io/github/issues/aivclab/vision.svg?style=flat)](https://github.com/aivclab/vision/issues) | [![GitHub Forks](https://img.shields.io/github/forks/aivclab/vision.svg?style=flat)](https://github.com/aivclab/vision/network) | [![GitHub Stars](https://img.shields.io/github/stars/aivclab/vision.svg?style=flat)](https://github.com/aivclab/vision/stargazers) | [![GitHub License](https://img.shields.io/github/license/aivclab/vision.svg?style=flat)](https://github.com/aivclab/vision/blob/master/LICENSE.md) |
-|-------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|
+| [![Build Status](https://travis-ci.org/automaps/jord.svg?branch=master)](https://travis-ci.org/automaps/jord) | [![Coverage Status](https://coveralls.io/repos/github/automaps/jord/badge.svg?branch=master)](https://coveralls.io/github/automaps/jord?branch=master) | [![GitHub Issues](https://img.shields.io/github/issues/automaps/jord.svg?style=flat)](https://github.com/automaps/jord/issues) | [![GitHub Forks](https://img.shields.io/github/forks/automaps/jord.svg?style=flat)](https://github.com/automaps/jord/network) | [![GitHub Stars](https://img.shields.io/github/stars/automaps/jord.svg?style=flat)](https://github.com/automaps/jord/stargazers) | [![GitHub License](https://img.shields.io/github/license/automaps/jord.svg?style=flat)](https://github.com/automaps/jord/blob/master/LICENSE.md) |
+|--------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
 
 <p align="center" width="100%">
   <a href="https://www.python.org/">
     <img alt="python" src=".github/images/python.svg" height="40" align="left">
   </a>
   <a href="http://pytorch.org/" style="float: right;">
     <img alt="pytorch" src=".github/images/pytorch.svg" height="40" align="right" >
@@ -27,8 +27,8 @@
     <img alt="tqdm" src=".github/images/tqdm.gif" height="40" align="center">
   </a>
 </p>
 
 # Authors
 
 * **Christian Heider Nielsen** - [cnheider](https://github.com/cnheider)
-* [Other contributors](https://github.com/aivclab/jord/contributors)
+* [Other contributors](https://github.com/automaps/jord/contributors)
```

#### html2text {}

```diff
@@ -1,28 +1,27 @@
                                    [header]
                               ****** Jord ******
- | [![Build Status](https://travis-ci.org/aivclab/jord.svg?branch=master)]
-(https://travis-ci.org/aivclab/jord) | [![Coverage Status](https://
-coveralls.io/repos/github/aivclab/vision/badge.svg?branch=master)](https://
-coveralls.io/github/aivclab/vision?branch=master) | [![GitHub Issues](https://
-img.shields.io/github/issues/aivclab/vision.svg?style=flat)](https://
-github.com/aivclab/vision/issues) | [![GitHub Forks](https://img.shields.io/
-github/forks/aivclab/vision.svg?style=flat)](https://github.com/aivclab/vision/
-network) | [![GitHub Stars](https://img.shields.io/github/stars/aivclab/
-vision.svg?style=flat)](https://github.com/aivclab/vision/stargazers) | [!
-[GitHub License](https://img.shields.io/github/license/aivclab/
-vision.svg?style=flat)](https://github.com/aivclab/vision/blob/master/
-LICENSE.md) | |----------------------------------------------------------------
----------------------------------------------|---------------------------------
+ | [![Build Status](https://travis-ci.org/automaps/jord.svg?branch=master)]
+(https://travis-ci.org/automaps/jord) | [![Coverage Status](https://
+coveralls.io/repos/github/automaps/jord/badge.svg?branch=master)](https://
+coveralls.io/github/automaps/jord?branch=master) | [![GitHub Issues](https://
+img.shields.io/github/issues/automaps/jord.svg?style=flat)](https://github.com/
+automaps/jord/issues) | [![GitHub Forks](https://img.shields.io/github/forks/
+automaps/jord.svg?style=flat)](https://github.com/automaps/jord/network) | [!
+[GitHub Stars](https://img.shields.io/github/stars/automaps/
+jord.svg?style=flat)](https://github.com/automaps/jord/stargazers) | [![GitHub
+License](https://img.shields.io/github/license/automaps/jord.svg?style=flat)]
+(https://github.com/automaps/jord/blob/master/LICENSE.md) | |------------------
 -------------------------------------------------------------------------------
-------------------------------------------|------------------------------------
+-------------|-----------------------------------------------------------------
 -------------------------------------------------------------------------------
----------------|---------------------------------------------------------------
-------------------------------------------------------------------|------------
+--------|----------------------------------------------------------------------
+----------------------------------------------------------|--------------------
 -------------------------------------------------------------------------------
------------------------------------------|-------------------------------------
+----------------------------|--------------------------------------------------
 -------------------------------------------------------------------------------
---------------------------------|
+-|-----------------------------------------------------------------------------
+---------------------------------------------------------------------|
                               [python] [pytorch]
                                 [numpy] [tqdm]
 # Authors * **Christian Heider Nielsen** - [cnheider](https://github.com/
-cnheider) * [Other contributors](https://github.com/aivclab/jord/contributors)
+cnheider) * [Other contributors](https://github.com/automaps/jord/contributors)
```

### Comparing `Jord-0.1.2/SECURITY.md` & `Jord-0.1.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/__init__.py` & `Jord-0.1.3/jord/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from importlib.metadata import PackageNotFoundError
 from warg import package_is_editable
 from apppath import AppPath
 from warg import dist_is_editable
 
 __project__ = "Jord"
 __author__ = "Christian Heider Nielsen"
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __doc__ = r"""
 .. module:: jord
    :platform: Unix, Windows
    :synopsis: A set of general tools build for geo data.
 
 .. moduleauthor:: Christian Heider Nielsen <christian.heider@alexandra.dk>
```

### Comparing `Jord-0.1.2/jord/gdal_utilities/__init__.py` & `Jord-0.1.3/jord/gdal_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/gdal_utilities/cloning.py` & `Jord-0.1.3/jord/gdal_utilities/cloning.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/gdal_utilities/context.py` & `Jord-0.1.3/jord/gdal_utilities/context.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/gdal_utilities/conversion.py` & `Jord-0.1.3/jord/gdal_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/gdal_utilities/importing.py` & `Jord-0.1.3/jord/gdal_utilities/importing.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/gdal_utilities/persistence.py` & `Jord-0.1.3/jord/gdal_utilities/persistence.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/geojson_utilities/geometry_types.py` & `Jord-0.1.3/jord/geojson_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/geopandas_utilities/geometry_filtering.py` & `Jord-0.1.3/jord/geopandas_utilities/geometry_filtering.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/categorisation.py` & `Jord-0.1.3/jord/qgis_utilities/categorisation.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/configuration/plugin_settings.py` & `Jord-0.1.3/jord/qgis_utilities/configuration/plugin_settings.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/configuration/project_settings.py` & `Jord-0.1.3/jord/qgis_utilities/configuration/project_settings.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/enums.py` & `Jord-0.1.3/jord/qgis_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/geometry_types.py` & `Jord-0.1.3/jord/qgis_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/helpers/actions.py` & `Jord-0.1.3/jord/qgis_utilities/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/helpers/drawing.py` & `Jord-0.1.3/jord/qgis_utilities/helpers/drawing.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/helpers/environment.py` & `Jord-0.1.3/jord/qgis_utilities/helpers/environment.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/helpers/models.py` & `Jord-0.1.3/jord/qgis_utilities/helpers/models.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/helpers/progress_bar.py` & `Jord-0.1.3/jord/qgis_utilities/helpers/progress_bar.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/helpers/sessions.py` & `Jord-0.1.3/jord/qgis_utilities/helpers/sessions.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/helpers/signals.py` & `Jord-0.1.3/jord/qgis_utilities/helpers/signals.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/helpers/timestamp.py` & `Jord-0.1.3/jord/qgis_utilities/helpers/timestamp.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/numpy_utilities/conversion.py` & `Jord-0.1.3/jord/qgis_utilities/numpy_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/numpy_utilities/data_type.py` & `Jord-0.1.3/jord/qgis_utilities/numpy_utilities/data_type.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py` & `Jord-0.1.3/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qgis_utilities/styling.py` & `Jord-0.1.3/jord/qgis_utilities/styling.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qlive_utilities/client.py` & `Jord-0.1.3/jord/qlive_utilities/client.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qlive_utilities/clients/auto.py` & `Jord-0.1.3/jord/qlive_utilities/clients/auto.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,65 +10,70 @@
 
 __all__ = ["AutoQliveClient"]
 
 from jord.qlive_utilities.clients.arguments import partial_satisfied
 
 
 class AutoQliveClient(QliveClient):
+    """
+    Has no client side validation of data, but exposes function if available in QliveRPCMethodEnum and QliveRPCMethodMap
+    """
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         for method in QliveRPCMethodEnum:
-            actual_callable = QliveRPCMethodMap[method]
+            if method in QliveRPCMethodMap:
+                actual_callable = QliveRPCMethodMap[method]
 
-            if False:
-                partial_build_package = partial(build_package, method)
-                if False and partial_satisfied(
-                    partial_build_package
-                ):  # TODO: RESOLVE PARTIAL APPLICATION SATISFACTION.
+                if False:
+                    partial_build_package = partial(build_package, method)
+                    if False and partial_satisfied(
+                        partial_build_package
+                    ):  # TODO: RESOLVE PARTIAL APPLICATION SATISFACTION.
 
-                    def a():
-                        self.send(partial_build_package())
+                        def a():
+                            self.send(partial_build_package())
 
-                    rpc_method = a
-                elif True:
+                        rpc_method = a
+                    elif True:
 
-                    def a(*args):
-                        self.send(partial_build_package(*args))
+                        def a(*args):
+                            self.send(partial_build_package(*args))
 
-                    rpc_method = a
-                elif False:
+                        rpc_method = a
+                    elif False:
 
-                    def a(**kwargs):
-                        self.send(partial_build_package(**kwargs))
+                        def a(**kwargs):
+                            self.send(partial_build_package(**kwargs))
 
-                    rpc_method = a
-                elif False:
+                        rpc_method = a
+                    elif False:
 
-                    def a(*args, **kwargs):
-                        self.send(partial_build_package(*args, **kwargs))
+                        def a(*args, **kwargs):
+                            self.send(partial_build_package(*args, **kwargs))
 
-                    rpc_method = a
+                        rpc_method = a
+                    else:
+                        raise NotImplementedError
+                elif False:
+                    rpc_method = lambda *args: self.send(
+                        partial(build_package, method)(*args)
+                    )
+                elif False:
+                    rpc_method = lambda *args: self.send(build_package(method, *args))
                 else:
-                    raise NotImplementedError
-            elif False:
-                rpc_method = lambda *args: self.send(
-                    partial(build_package, method)(*args)
-                )
-            elif False:
-                rpc_method = lambda *args: self.send(build_package(method, *args))
-            else:
 
-                def wrapped(method_, *args_) -> Callable:
-                    return self.send(build_package(method_, *args_))
+                    def wrapped(method_, *args_, **_kwargs) -> Callable:
+                        return self.send(build_package(method_, *args_, **_kwargs))
 
-                rpc_method = partial(wrapped, method)
+                    rpc_method = partial(wrapped, method)
 
-            rpc_method.__doc__ = actual_callable.__doc__
-            setattr(self, method.value, rpc_method)
+                rpc_method.__doc__ = actual_callable.__doc__
+                setattr(self, method.value, rpc_method)
 
 
 if __name__ == "__main__":
     # QliveClient().clear_all()
     # QliveClient().remove_layers()
     # print(QliveClient().clear_all.__doc__)
     # print(QliveClient().__dict__)
```

### Comparing `Jord-0.1.2/jord/qlive_utilities/procedures.py` & `Jord-0.1.3/jord/qlive_utilities/procedures.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import time
 import uuid
 from enum import Enum
-from typing import Mapping, Any, Tuple
+from typing import Mapping, Any, Tuple, Iterable
 
 import numpy
 import shapely.geometry.base
 import tqdm
 from pandas import DataFrame
 from shapely.geometry.base import BaseGeometry
 from warg import ensure_existence
 from warg import passes_kws_to, Number
 
 from jord import PROJECT_APP_PATH
-from jord.qlive_utilities.qgis_layer_creation import add_qgis_geometry
+from jord.qlive_utilities.qgis_layer_creation import (
+    add_qgis_single_feature_layer,
+    add_qgis_multi_feature_layer,
+)
 
 APPEND_TIMESTAMP = True
 SKIP_MEMORY_LAYER_CHECK_AT_CLOSE = True
 PIXEL_SIZE = 1
 DEFAULT_NUMBER = 0
 CONTRAST_ENHANCE = True
 DEFAULT_LAYER_NAME = "TemporaryLayer"
@@ -24,28 +27,285 @@
 VERBOSE = False
 
 __all__ = [
     "add_raster",
     "add_rasters",
     "add_wkt",
     "add_wkts",
+    "add_wkt_layer",
     "add_wkb",
     "add_wkbs",
+    "add_wkb_layer",
     "add_dataframe",
     "add_dataframes",
+    "add_dataframe_layer",
     "add_geojson",
+    "add_geojsons",
+    "add_geojson_layer",
     "add_shapely_geometry",
     "add_shapely_geometries",
+    "add_shapely_layer",
     "clear_all",
     "remove_layers",
+    "remove_layer",
     "QliveRPCMethodEnum",
     "QliveRPCMethodMap",
 ]
 
 
+@passes_kws_to(add_qgis_single_feature_layer)
+def add_wkb(qgis_instance_handle: Any, wkb: str, **kwargs) -> None:
+    """
+
+    :param qgis_instance_handle:
+    :param wkb:
+    :param kwargs:
+    :return:
+    """
+    # noinspection PyUnresolvedReferences
+    from qgis.core import QgsGeometry
+
+    add_qgis_single_feature_layer(
+        qgis_instance_handle, QgsGeometry.fromWkb(wkb), **kwargs
+    )
+
+
+@passes_kws_to(add_wkb)
+def add_wkbs(qgis_instance_handle: Any, wkbs: Mapping[str, str], **kwargs) -> None:
+    """
+
+    :param qgis_instance_handle:
+    :param wkbs:
+    :param kwargs:
+    :return:
+    """
+    for layer_name, wkb in wkbs.items():
+        add_wkb(qgis_instance_handle, wkb, name=layer_name, **kwargs)
+
+
+@passes_kws_to(add_qgis_multi_feature_layer)
+def add_wkb_layer(qgis_instance_handle: Any, wkbs: Iterable[str], **kwargs) -> None:
+    # noinspection PyUnresolvedReferences
+    from qgis.core import QgsGeometry
+
+    add_qgis_multi_feature_layer(
+        qgis_instance_handle, [QgsGeometry.fromWkb(wkb) for wkb in wkbs], **kwargs
+    )
+
+
+@passes_kws_to(add_qgis_single_feature_layer)
+def add_wkt(qgis_instance_handle: Any, wkt: str, **kwargs) -> None:
+    """
+
+    :param qgis_instance_handle:
+    :param wkt:
+    :param kwargs:
+    :return:
+    """
+    # noinspection PyUnresolvedReferences
+    from qgis.core import QgsGeometry
+
+    add_qgis_single_feature_layer(
+        qgis_instance_handle, QgsGeometry.fromWkt(wkt), **kwargs
+    )
+
+
+@passes_kws_to(add_wkt)
+def add_wkts(qgis_instance_handle: Any, wkts: Mapping[str, str], **kwargs) -> None:
+    """
+
+    :param qgis_instance_handle:
+    :param wkts:
+    :param kwargs:
+    :return:
+    """
+    for layer_name, wkt in wkts.items():
+        add_wkt(qgis_instance_handle, wkt, name=layer_name, **kwargs)
+
+
+@passes_kws_to(add_qgis_multi_feature_layer)
+def add_wkt_layer(qgis_instance_handle: Any, wkts: Iterable[str], **kwargs) -> None:
+    # noinspection PyUnresolvedReferences
+    from qgis.core import QgsGeometry
+
+    add_qgis_multi_feature_layer(
+        qgis_instance_handle, [QgsGeometry.fromWkt(wkt) for wkt in wkts], **kwargs
+    )
+
+
+@passes_kws_to(add_wkt)
+def add_shapely_geometry(
+    qgis_instance_handle: Any, geom: BaseGeometry, **kwargs
+) -> None:
+    """
+    Add a shapely geometry
+
+    :param geom:
+    :param qgis_instance_handle:
+    :return:
+    """
+
+    add_wkt(qgis_instance_handle, geom.wkt, **kwargs)
+
+
+@passes_kws_to(add_shapely_geometry)
+def add_shapely_geometries(
+    qgis_instance_handle: Any, geometries: Mapping, **kwargs
+) -> None:
+    """
+
+    :param geometries:
+    :param qgis_instance_handle:
+    :param kwargs:
+    :return:
+    """
+    for layer_name, geometry in geometries.items():
+        add_shapely_geometry(qgis_instance_handle, geometry, name=layer_name, **kwargs)
+
+
+@passes_kws_to(add_wkt_layer)
+def add_shapely_layer(
+    qgis_instance_handle: Any,
+    geoms: Iterable[shapely.geometry.base.BaseGeometry],
+    **kwargs,
+) -> None:
+    # assert geoms[0] == #TODO: SAME TYPE
+    add_wkt_layer(qgis_instance_handle, [geom.wkt for geom in geoms], **kwargs)
+
+
+@passes_kws_to(add_wkb)  # OR add_wkt
+def add_dataframe(qgis_instance_handle: Any, dataframe: DataFrame, **kwargs) -> None:
+    """
+
+    :param qgis_instance_handle:
+    :param dataframe:
+    :param kwargs:
+    :return:
+    """
+    from geopandas import GeoDataFrame
+    from jord.geopandas_utilities import split_on_geom_type
+
+    if isinstance(dataframe, GeoDataFrame):
+        columns_to_include = ("layer",)
+        geom_dict = split_on_geom_type(dataframe)
+        for df in geom_dict.values():
+            if False:
+                for w in df.geometry.to_wkt():
+                    add_wkt(qgis_instance_handle, w, **kwargs)
+            else:
+                for w in df.geometry.to_wkb():
+                    add_wkb(qgis_instance_handle, w, **kwargs)
+
+    elif isinstance(dataframe, DataFrame) and False:
+        geometry_column = "geometry"
+        if isinstance(
+            dataframe[geometry_column][0], shapely.geometry.base.BaseGeometry
+        ):
+            a = dataframe[geometry_column][0]
+            # if a.geom_type == "MultiPolygon":
+
+            wkts = [d.wkt for d in dataframe[geometry_column]]
+        elif isinstance(dataframe[geometry_column][0], str):
+            wkts = dataframe[geometry_column]
+        else:
+            raise NotImplemented
+
+        for row in wkts:
+            add_wkt(qgis_instance_handle, row, **kwargs)
+    else:
+        if VERBOSE:
+            print("SKIP!")
+
+
+@passes_kws_to(add_qgis_single_feature_layer)
+def add_dataframes(
+    qgis_instance_handle: Any, dataframes: Mapping[str, DataFrame], **kwargs
+) -> None:
+    ...
+
+
+def add_dataframe_layer(
+    qgis_instance_handle: Any, geoms: Iterable[DataFrame], **kwargs
+) -> None:
+    ...
+
+
+@passes_kws_to(add_shapely_geometry)
+def add_geojson(qgis_instance_handle: Any, geojson_: str, **kwargs) -> None:
+    """
+
+    :param geojson_:
+    :param qgis_instance_handle:
+    :param kwargs:
+    :return:
+    """
+    # meta_data = ''
+    add_shapely_geometry(qgis_instance_handle, shapely.from_geojson(geojson_), **kwargs)
+
+
+@passes_kws_to(add_shapely_geometry)
+def add_geojsons(
+    qgis_instance_handle: Any, geojsons: Mapping[str, str], **kwargs
+) -> None:
+    """
+
+    :param qgis_instance_handle:
+    :param geojsons:
+    :param kwargs:
+    :return:
+    """
+    for layer_name, geojson_ in geojsons.items():
+        add_shapely_geometry(
+            qgis_instance_handle,
+            shapely.from_geojson(geojson_),
+            name=layer_name,
+            **kwargs,
+        )
+
+
+@passes_kws_to(add_shapely_layer)
+def add_geojson_layer(
+    qgis_instance_handle: Any, geojsons: Iterable[str], **kwargs
+) -> None:
+    add_shapely_layer(
+        qgis_instance_handle,
+        [shapely.from_geojson(geojson_) for geojson_ in geojsons],
+        **kwargs,
+    )
+
+
+def remove_layers(qgis_instance_handle: Any, *args) -> None:
+    """
+    clear all the added layers
+
+    :param qgis_instance_handle:
+    :param args:
+    :return: None
+    :rtype: None
+    """
+    qgis_instance_handle.on_clear_temporary()
+
+
+def remove_layer(qgis_instance_handle: Any, name: str) -> None:
+    ...
+    # qgis_instance_handle.on_clear_temporary()
+
+
+def clear_all(qgis_instance_handle: Any, *args) -> None:  # TODO: REMOVE THIS!
+    """
+    clear all the added layers
+
+    :param qgis_instance_handle:
+    :return:
+    """
+    remove_layers(qgis_instance_handle)
+    if VERBOSE:
+        print("CLEAR ALL!")
+
+
 def add_raster(
     qgis_instance_handle: Any,
     raster: numpy.ndarray,
     name: str = DEFAULT_LAYER_NAME,
     centroid: Tuple[Number, Number] = None,
     extent_tuple: Tuple[Number, Number, Number, Number] = None,
     pixel_size: Tuple[Number, Number] = PIXEL_SIZE,
@@ -53,14 +313,15 @@
     default_value: Number = DEFAULT_NUMBER,
     field: str = None,
     no_data_value: int = -1,
 ) -> None:
     """
     add a raster
 
+    :param no_data_value:
     :param qgis_instance_handle:
     :param raster:
     :param name:
     :param centroid:
     :param extent_tuple:
     :param pixel_size:
     :param crs_str:
@@ -89,55 +350,67 @@
     if len(rest_size) == 0:
         raster = numpy.expand_dims(raster, axis=-1)
 
     *_, num_bands = raster.shape
 
     data_type = get_qgis_type(raster.dtype).value
 
+    # QgsWkbTypes.displayString(gPolygon.wkbType())
+
     extent = QgsRectangle()
 
     if extent_tuple:
         extent.setXMinimum(extent_tuple[0])
         extent.setYMinimum(extent_tuple[1])
         extent.setXMaximum(extent_tuple[2])
         extent.setYMaximum(extent_tuple[3])
     else:
-        if centroid is None:
-            centroid = (0, 0)  # (x_size, y_size)
+        raster_half_size = (PIXEL_SIZE * (x_size / 2.0), PIXEL_SIZE * (y_size / 2.0))
 
-        raster_half_size = (PIXEL_SIZE * x_size / 2, PIXEL_SIZE * y_size / 2)
+        raster_half_size = raster_half_size[1], raster_half_size[0]
 
-        if False:
-            raster_half_size = raster_half_size[1], raster_half_size[0]
+        if centroid is None:
+            centroid = (0, 0)  # raster_half_size
 
         extent.setXMinimum(centroid[0] - raster_half_size[0])
-        extent.setYMinimum(centroid[1] - raster_half_size[1])
         extent.setXMaximum(centroid[0] + raster_half_size[0])
+
+        extent.setYMinimum(centroid[1] - raster_half_size[1])
         extent.setYMaximum(centroid[1] + raster_half_size[1])
 
     if APPEND_TIMESTAMP:
         name += f"_{time.time()}"
 
     temp_file = (
         ensure_existence(PROJECT_APP_PATH.user_data / "rasters") / f"{uuid.uuid4()}.tif"
     )
-    writer = QgsRasterFileWriter(temp_file)
-    provider = writer.createMultiBandRaster(
-        dataType=data_type.value,
-        width=x_size,
-        height=y_size,
-        extent=extent,
-        crs=QgsCoordinateReferenceSystem(crs_str),
-        nBands=num_bands,
-    )
-
-    if VERBOSE:
-        print("drawing")
+    writer = QgsRasterFileWriter(str(temp_file))
 
-    w_pixels, h_pixels = x_size, y_size
+    if num_bands > 1:
+        provider = writer.createMultiBandRaster(
+            dataType=data_type,
+            width=x_size,
+            height=y_size,
+            extent=extent,
+            crs=QgsCoordinateReferenceSystem(crs_str),
+            nBands=num_bands,
+        )
+    else:
+        provider = writer.createOneBandRaster(
+            dataType=data_type,
+            width=x_size,
+            height=y_size,
+            extent=extent,
+            crs=QgsCoordinateReferenceSystem(crs_str),
+        )
+
+    w_pixels, h_pixels = (
+        x_size,
+        y_size,
+    )  # TODO: FIGURE OUT HOW TO HANDLE NON SQUARE RASTERS! SCALE DIMS BY SOME AMOUNT.
 
     with RasterDataProviderEditSession(provider):
         progress = range(0, num_bands)
 
         if VERBOSE:
             progress = tqdm.tqdm(progress)
 
@@ -147,28 +420,26 @@
             )
             provider.setNoDataValue(bandNo=ith_band + 1, noDataValue=no_data_value)
 
             for wp in range(0, w_pixels):
                 for hp in range(0, h_pixels):
                     value = raster[wp][hp][ith_band]
                     if value == numpy.nan:
-                        block.setIsNoData(wp, hp)
-                        continue
-                    if False:
-                        value = int(value) * 255
+                        if block.setIsNoData(wp, hp):
+                            continue
                     block.setValue(wp, hp, value)
 
             if VERBOSE:
                 print("writing block on band", ith_band + 1)
 
             provider.writeBlock(block, band=ith_band + 1, xOffset=0, yOffset=0)
 
             del block
 
-    layer = QgsRasterLayer(temp_file, name, "gdal")
+    layer = QgsRasterLayer(str(temp_file), name, "gdal")
 
     if num_bands == 1:
         # this is needed for the min and max value to refresh in the layer panel
         renderer = layer.renderer()
 
         gray_renderer = QgsSingleBandGrayRenderer(provider, 1)
 
@@ -218,197 +489,40 @@
     :param kwargs:
     :return:
     """
     for layer_name, raster in rasters.items():
         add_raster(qgis_instance_handle, raster, name=layer_name, **kwargs)
 
 
-@passes_kws_to(add_qgis_geometry)
-def add_wkb(qgis_instance_handle: Any, wkb: str, **kwargs) -> None:
-    """
-
-    :param qgis_instance_handle:
-    :param wkb:
-    :param kwargs:
-    :return:
-    """
-    # noinspection PyUnresolvedReferences
-    from qgis.core import QgsGeometry
-
-    add_qgis_geometry(qgis_instance_handle, QgsGeometry.fromWkb(wkb), **kwargs)
-
-
-@passes_kws_to(add_qgis_geometry)
-def add_wkt(qgis_instance_handle: Any, wkt: str, **kwargs) -> None:
-    """
-
-    :param qgis_instance_handle:
-    :param wkt:
-    :param kwargs:
-    :return:
-    """
-    # noinspection PyUnresolvedReferences
-    from qgis.core import QgsGeometry
-
-    add_qgis_geometry(qgis_instance_handle, QgsGeometry.fromWkt(wkt), **kwargs)
-
-
-@passes_kws_to(add_wkb)
-def add_wkbs(qgis_instance_handle: Any, wkbs: Mapping[str, str], **kwargs) -> None:
-    """
-
-    :param qgis_instance_handle:
-    :param wkbs:
-    :param kwargs:
-    :return:
-    """
-    for layer_name, wkb in wkbs.items():
-        add_wkb(qgis_instance_handle, wkb, name=layer_name, **kwargs)
-
-
-@passes_kws_to(add_wkt)
-def add_wkts(qgis_instance_handle: Any, wkts: Mapping[str, str], **kwargs) -> None:
-    """
-
-    :param qgis_instance_handle:
-    :param wkts:
-    :param kwargs:
-    :return:
-    """
-    for layer_name, wkt in wkts.items():
-        add_wkt(qgis_instance_handle, wkt, name=layer_name, **kwargs)
-
-
-@passes_kws_to(add_qgis_geometry)
-def add_dataframes(
-    qgis_instance_handle: Any, dataframes: Mapping[str, DataFrame], **kwargs
-) -> None:
-    ...
-
-
-@passes_kws_to(add_qgis_geometry)
-def add_dataframe(qgis_instance_handle: Any, dataframe: DataFrame, **kwargs) -> None:
-    """
-
-    :param qgis_instance_handle:
-    :param dataframe:
-    :param kwargs:
-    :return:
-    """
-    from geopandas import GeoDataFrame
-    from jord.geopandas_utilities import split_on_geom_type
-
-    if isinstance(dataframe, GeoDataFrame):
-        columns_to_include = ("layer",)
-        geom_dict = split_on_geom_type(dataframe)
-        for df in geom_dict.values():
-            if False:
-                for w in df.geometry.to_wkt():
-                    add_wkt(qgis_instance_handle, w)
-            else:
-                for w in df.geometry.to_wkb():
-                    add_wkb(qgis_instance_handle, w)
-
-    elif isinstance(dataframe, DataFrame) and False:
-        geometry_column = "geometry"
-        if isinstance(
-            dataframe[geometry_column][0], shapely.geometry.base.BaseGeometry
-        ):
-            a = dataframe[geometry_column][0]
-            # if a.geom_type == "MultiPolygon":
-
-            wkts = [d.wkt for d in dataframe[geometry_column]]
-        elif isinstance(dataframe[geometry_column][0], str):
-            wkts = dataframe[geometry_column]
-        else:
-            raise NotImplemented
-
-        for row in wkts:
-            add_wkt(qgis_instance_handle, row)
-    else:
-        if VERBOSE:
-            print("SKIP!")
-
-
-@passes_kws_to(add_qgis_geometry)
-def add_geojson(qgis_instance_handle: Any, geojson: str, **kwargs) -> None:
-    """
-
-    :param qgis_instance_handle:
-    :param dataframe:
-    :param kwargs:
-    :return:
-    """
-    geom = shapely.from_geojson(geojson)
-    add_shapely_geometry(geom)
-
-
-def remove_layers(qgis_instance_handle: Any, *args) -> None:
-    """
-    clear all the added layers
-
-    :param qgis_instance_handle:
-    :param args:
-    :return:
-    """
-    qgis_instance_handle.on_clear_temporary()
-
-
-def clear_all(qgis_instance_handle: Any, *args) -> None:  # TODO: REMOVE THIS!
-    """
-    clear all the added layers
-
-    :param qgis_instance_handle:
-    :return:
-    """
-    remove_layers(qgis_instance_handle)
-    if VERBOSE:
-        print("CLEAR ALL!")
-
-
-def add_shapely_geometry(
-    qgis_instance_handle: Any, geom: BaseGeometry, **kwargs
-) -> None:
-    """
-    Add a shapely geometry
-
-    :param qgis_instance_handle:
-    :param args:
-    :return:
-    """
-
-    add_wkt(qgis_instance_handle, geom.wkt)
-
-
-@passes_kws_to(add_shapely_geometry)
-def add_shapely_geometries(
-    qgis_instance_handle: Any, geometries: Mapping, **kwargs
-) -> None:
-    """
-
-    :param qgis_instance_handle:
-    :param wkbs:
-    :param kwargs:
-    :return:
-    """
-    for layer_name, geometry in geometries.items():
-        add_shapely_geometry(qgis_instance_handle, geometry, name=layer_name, **kwargs)
-
-
 class QliveRPCMethodEnum(Enum):
     # add_layers = add_layers.__name__
+
     remove_layers = remove_layers.__name__
     clear_all = clear_all.__name__
+    remove_layer = remove_layer.__name__
+
     add_wkt = add_wkt.__name__
-    add_wkb = add_wkb.__name__
     add_wkts = add_wkts.__name__
+    add_wkt_layer = add_wkt_layer.__name__
+
+    add_wkb = add_wkb.__name__
     add_wkbs = add_wkbs.__name__
+    add_wkb_layer = add_wkb_layer.__name__
+
     add_dataframe = add_dataframe.__name__
     add_dataframes = add_dataframes.__name__
+    add_dataframe_layer = add_dataframe_layer.__name__
+
     add_shapely_geometry = add_shapely_geometry.__name__
     add_shapely_geometries = add_shapely_geometries.__name__
+    add_shapely_layer = add_shapely_layer.__name__
+
+    add_geojson = add_geojson.__name__
+    add_geojsons = add_geojsons.__name__
+    add_geojson_layer = add_geojson_layer.__name__
+
     add_raster = add_raster.__name__
     add_rasters = add_rasters.__name__
 
 
 funcs = locals()  # In local scope for name
 QliveRPCMethodMap = {e: funcs[e.value] for e in QliveRPCMethodEnum}
```

### Comparing `Jord-0.1.2/jord/qlive_utilities/qgis_layer_creation.py` & `Jord-0.1.3/jord/qlive_utilities/qgis_layer_creation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import time
-from typing import Any, Optional, Mapping
+from typing import Any, Optional, Mapping, Iterable
 
 from warg import passes_kws_to
 
 from jord.geojson_utilities import GeoJsonGeometryTypesEnum
 
 APPEND_TIMESTAMP = True
 SKIP_MEMORY_LAYER_CHECK_AT_CLOSE = True
@@ -12,18 +12,22 @@
 DEFAULT_NUMBER = 0
 CONTRAST_ENHANCE = True
 DEFAULT_LAYER_NAME = "TemporaryLayer"
 DEFAULT_LAYER_CRS = "EPSG:4326"
 VERBOSE = False
 
 
-__all__ = ["add_qgis_geometry", "add_qgis_geometries"]
+__all__ = [
+    "add_qgis_single_feature_layer",
+    "add_qgis_single_geometry_layers",
+    "add_qgis_multi_feature_layer",
+]
 
 
-def add_qgis_geometry(
+def add_qgis_single_feature_layer(
     qgis_instance_handle: Any,
     geom,  #: QgsGeometry,
     name: Optional[str] = None,
     crs: Optional[str] = None,
     fields: Mapping[str, Any] = None,
     index: bool = False,
     categorise_by_attribute: Optional[str] = None,
@@ -46,15 +50,15 @@
     from qgis.core import QgsVectorLayer, QgsFeature
 
     # uri = geom.type()
     # uri = geom.wkbType()
     # uri = geom.wktTypeStr()
 
     geom_type = json.loads(geom.asJson())["type"]
-    uri = geom_type
+    uri = geom_type  # TODO: URI MIGHT BE NONE?
 
     if name is None:
         name = DEFAULT_LAYER_NAME
 
     if crs is None:
         crs = DEFAULT_LAYER_CRS
 
@@ -63,15 +67,15 @@
         layer_name += f"_{time.time()}"
 
     if geom_type == GeoJsonGeometryTypesEnum.geometry_collection.value.__name__:
         gm_group = qgis_instance_handle.temporary_group.addGroup(layer_name)
 
         for g in geom.asGeometryCollection():  # TODO: Look into recursion?
             uri = json.loads(g.asJson())["type"]
-            sub_type = uri
+            sub_type = uri  # TODO: URI MIGHT BE NONE?
 
             if crs:
                 uri += f"?crs={crs}"
 
             if fields:
                 for k, v in fields.items():
                     uri += f"&field={k}:{v}"
@@ -94,15 +98,15 @@
     elif geom_type == GeoJsonGeometryTypesEnum.multi_line_string.value.__name__:
         ...
     elif geom_type == GeoJsonGeometryTypesEnum.multi_polygon.value.__name__:
         gm_group = qgis_instance_handle.temporary_group.addGroup(layer_name)
 
         g = geom
         uri = json.loads(g.asJson())["type"]
-        sub_type = uri
+        sub_type = uri  # TODO: URI MIGHT BE NONE?
 
         if crs:
             uri += f"?crs={crs}"
 
         if fields:
             for k, v in fields.items():
                 uri += f"&field={k}:{v}"
@@ -143,13 +147,80 @@
         if SKIP_MEMORY_LAYER_CHECK_AT_CLOSE:
             layer.setCustomProperty("skipMemoryLayersCheck", 1)
 
         qgis_instance_handle.qgis_project.addMapLayer(layer, False)
         qgis_instance_handle.temporary_group.insertLayer(0, layer)
 
 
-@passes_kws_to(add_qgis_geometry)
-def add_qgis_geometries(
-    qgis_instance_handle: Any, geoms, **kwargs  # Mapping[str, QgsGeometry]
+@passes_kws_to(add_qgis_single_feature_layer)
+def add_qgis_single_geometry_layers(
+    qgis_instance_handle: Any, geoms: Mapping, **kwargs  # [str,QgsGeometry]
 ) -> None:
     for name, geom in geoms.items():
-        add_qgis_geometry(qgis_instance_handle, geom, name, **kwargs)
+        add_qgis_single_feature_layer(qgis_instance_handle, geom, name, **kwargs)
+
+
+def add_qgis_multi_feature_layer(
+    qgis_instance_handle: Any,
+    geoms: Iterable,  # [QgsGeometry]
+    name: Optional[str] = None,
+    crs: Optional[str] = None,
+    fields: Mapping[str, Any] = None,
+    index: bool = False,
+) -> None:
+    # noinspection PyUnresolvedReferences
+    from qgis.core import QgsVectorLayer, QgsFeature
+
+    # uri = geom.type()
+    # uri = geom.wkbType()
+    # uri = geom.wktTypeStr()
+
+    if name is None:
+        name = DEFAULT_LAYER_NAME
+
+    if crs is None:
+        crs = DEFAULT_LAYER_CRS
+
+    layer_name = f"{name}"
+    if APPEND_TIMESTAMP:
+        layer_name += f"_{time.time()}"
+
+    geom_type = None
+    uri = None
+    features = []
+
+    for geom in geoms:
+        geom_type_ = json.loads(geom.asJson())["type"]
+        if geom_type is None:
+            geom_type = geom_type_
+            uri = geom_type  # TODO: URI MIGHT BE NONE?
+
+        assert geom_type_ == geom_type
+
+        if geom_type == GeoJsonGeometryTypesEnum.geometry_collection.value.__name__:
+            for g in geom.asGeometryCollection():  # TODO: Look into recursion?
+                add_qgis_multi_feature_layer(
+                    qgis_instance_handle, g, f'{name}_{json.loads(g.asJson())["type"]}'
+                )
+            return
+        else:
+            feat = QgsFeature()
+            feat.setGeometry(geom)
+            features.append(feat)
+
+    if crs:
+        uri += f"?crs={crs}"
+
+    if fields:
+        for k, v in fields.items():
+            uri += f"&field={k}:{v}"
+
+    uri += f'&index={"yes" if index else "no"}'
+
+    layer = QgsVectorLayer(uri, layer_name, "memory")
+    layer.dataProvider().addFeatures(features)
+
+    if SKIP_MEMORY_LAYER_CHECK_AT_CLOSE:
+        layer.setCustomProperty("skipMemoryLayersCheck", 1)
+
+    qgis_instance_handle.qgis_project.addMapLayer(layer, False)
+    qgis_instance_handle.temporary_group.insertLayer(0, layer)
```

### Comparing `Jord-0.1.2/jord/qlive_utilities/serialisation.py` & `Jord-0.1.3/jord/qlive_utilities/serialisation.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     json, pickle = assigned_names()
 
 
 SERIALISATION_METHOD = SerialisationMethodEnum.pickle
 VERBOSE = False
 
 
-def build_package(method: QliveRPCMethodEnum, *args: Any) -> bytes:
+def build_package(method: QliveRPCMethodEnum, *args: Any, **kwargs) -> bytes:
     """
 
     :param method:
     :param args:
     :return:
     """
     if VERBOSE:
@@ -34,17 +34,19 @@
         assert isinstance(method, str), method
         method = QliveRPCMethodEnum(method)
 
     if VERBOSE:
         print(type(method.value), method.value, args)
 
     if SERIALISATION_METHOD == SerialisationMethodEnum.pickle:
-        return pickle.dumps({"method": method.value, "args": args})
+        return pickle.dumps({"method": method.value, "args": args, "kwargs": kwargs})
     elif SERIALISATION_METHOD == SERIALISATION_METHOD.json:
-        return json.dump({"method": method.value, "args": args})  # TODO: ?
+        return json.dump(
+            {"method": method.value, "args": args, "kwargs": kwargs}
+        )  # TODO: ?
         # return base64.b64encode(str({"method": method.value, "args": args}).encode("ascii"))
     else:
         raise NotImplemented
 
 
 def read_package(package: bytes) -> Tuple[QliveRPCMethodEnum, Sequence[str]]:
     """
@@ -63,12 +65,16 @@
             )
         )
         res_dict = json.loads(str_dict)  # convert string dictionary to dict format
     elif SERIALISATION_METHOD == SerialisationMethodEnum.pickle:
         res_dict = pickle.loads(package)
     else:
         raise NotImplemented
-    return QliveRPCMethodMap[QliveRPCMethodEnum(res_dict["method"])], res_dict["args"]
+    return (
+        QliveRPCMethodMap[QliveRPCMethodEnum(res_dict["method"])],
+        res_dict["args"],
+        res_dict["kwargs"],
+    )
 
 
 if __name__ == "__main__":
     print(read_package(build_package(method=QliveRPCMethodEnum.add_wkt)))
```

### Comparing `Jord-0.1.2/jord/qlive_utilities/uri_utilities.py` & `Jord-0.1.3/jord/qlive_utilities/uri_utilities.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/qt_utilities/enums.py` & `Jord-0.1.3/jord/qt_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/shapely_utilities/__init__.py` & `Jord-0.1.3/jord/shapely_utilities/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,13 +13,13 @@
     __doc__ += this_init_file.read()
 
 from .analysis import *
 from .clamp import *
 from .lines import *
 from .morphology import *
 from .points import *
-from .sanitise_poly import *
+from .polygons import *
 from .serialisation import *
 from .geometry_types import *
-from .iteration import *
 from .projection import *
 from .transformation import *
+from .rings import *
```

### Comparing `Jord-0.1.2/jord/shapely_utilities/clamp.py` & `Jord-0.1.3/jord/shapely_utilities/clamp.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/shapely_utilities/geometry_types.py` & `Jord-0.1.3/jord/shapely_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/shapely_utilities/mirroring.py` & `Jord-0.1.3/jord/shapely_utilities/mirroring.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/shapely_utilities/morphology.py` & `Jord-0.1.3/jord/shapely_utilities/morphology.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/shapely_utilities/projection.py` & `Jord-0.1.3/jord/shapely_utilities/points.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,107 +1,146 @@
-from typing import Sequence, Tuple
+from typing import Sequence, List, Optional, Union, Tuple, Iterable, Generator
 
-from shapely.geometry import Polygon, Point, LineString
 from shapely.geometry.base import BaseGeometry
+from warg import Number
+import numpy
+from shapely.geometry import LineString, Point, MultiPoint
+
+__all__ = [
+    "unique_line_points",
+    "nearest_neighbor_within",
+    "azimuth",
+    "shift_point",
+    "closest_object",
+]
 
-from jord.shapely_utilities import pairs
 
+def unique_line_points(lines: Sequence[LineString]) -> List[Point]:
+    """
 
-__all__ = ["project_point_to_object", "project_point_to_line", "nearest_geometry"]
 
+    :param lines:
+    :return: Return list of unique vertices from list of LineStrings.
+    :rtype: List[Point]
+    """
 
-def project_point_to_object(point: Point, geometry: BaseGeometry) -> Point:
-    """Find the nearest point in geometry, measured from given point.
+    vertices = []
 
-    :param point: a shapely Point
-    :param geometry: a shapely geometry object (LineString, Polygon)
+    for line in lines:
+        vertices.extend(list(line.coords))
 
-    :return: a shapely Point that lies on geometry closest to point
-    """
-    nearest_point = None
-    min_dist = float("inf")
+    return [Point(p) for p in set(vertices)]
 
-    if isinstance(geometry, Polygon):
-        for seg_start, seg_end in pairs(list(geometry.exterior.coords)):
-            line_start = Point(seg_start)
-            line_end = Point(seg_end)
 
-            intersection_point = project_point_to_line(point, line_start, line_end)
-            cur_dist = point.distance(intersection_point)
+def nearest_neighbor_within(others: Sequence, point, max_distance) -> Optional[Point]:
+    """Find the nearest point among others up to a maximum distance.
 
-            if cur_dist < min_dist:
-                min_dist = cur_dist
-                nearest_point = intersection_point
 
-    elif isinstance(geometry, LineString):
-        for seg_start, seg_end in pairs(list(geometry.coords)):
-            line_start = Point(seg_start)
-            line_end = Point(seg_end)
+    :param others: a list of Points or a MultiPoint
+    :param point: a Point
+    :param max_distance: maximum distance to search for the nearest neighbor
 
-            intersection_point = project_point_to_line(point, line_start, line_end)
-            cur_dist = point.distance(intersection_point)
+    :return: A shapely Point if one is within max_distance, None otherwise
+    :rtype: Optional[Point]
+    """
+    search_region = point.buffer(max_distance)
+    interesting_points = search_region.intersection(MultiPoint(others))
 
-            if cur_dist < min_dist:
-                min_dist = cur_dist
-                nearest_point = intersection_point
+    if not interesting_points:
+        closest_point = None
+    elif isinstance(interesting_points, Point):
+        closest_point = interesting_points
     else:
-        raise NotImplementedError(
-            "project_point_to_object not implemented for"
-            + " geometry type '"
-            + geometry.type
-            + "'."
-        )
-    return nearest_point
+        distances = [
+            point.distance(ip) for ip in interesting_points if point.distance(ip) > 0
+        ]
+        closest_point = interesting_points[distances.index(min(distances))]
+
+    return closest_point
 
 
-def project_point_to_line(point: Point, line_start: Point, line_end: Point) -> Point:
-    """Find the nearest point on a straight line, measured from given point.
+def closest_object(
+    geometries: Iterable[BaseGeometry], point: Point
+) -> Tuple[BaseGeometry, float, int]:
+    """Find the nearest geometry among a list, measured from fixed point.
 
-    Source: http://gis.stackexchange.com/a/438/19627
+    Args:
+        geometries: a list of shapely geometry objects
+        point: a shapely Point
+
+    Returns:
+        Tuple (geom, min_dist, min_index) of the geometry with minimum distance
+        to point, its distance min_dist and the list index of geom, so that
+        geom = geometries[min_index].
+    """
+    if isinstance(geometries, Generator):
+        geometries = list(geometries)
 
-    :param point: a shapely Point object
-    :param line_start: the line starting point as a shapely Point
-    :param line_end: the line end point as a shapely Point
+    min_dist, min_index = min(
+        (point.distance(geom), k) for (k, geom) in enumerate(geometries)
+    )
 
-    :return: a shapely Point that lies on the straight line closest to point
+    return geometries[min_index], min_dist, min_index
 
 
+def shift_point(
+    c1: Union[Point, Tuple[Number, Number]],
+    c2: Union[Point, Tuple[Number, Number]],
+    offset: float,
+) -> Point:
     """
-    line_magnitude = line_start.distance(line_end)
-
-    u = (
-        (point.x - line_start.x) * (line_end.x - line_start.x)
-        + (point.y - line_start.y) * (line_end.y - line_start.y)
-    ) / (line_magnitude**2)
 
-    # closest point does not fall within the line segment,
-    # take the shorter distance to an endpoint
-    if u < 0.00001 or u > 1:
-        ix = point.distance(line_start)
-        iy = point.distance(line_end)
+    shift points with offset in orientation of line c1->c2
+    """
 
-        if ix > iy:
-            return line_end
+    if isinstance(c1, Point):
+        x1, y1 = c1.coords[0]
+    else:
+        x1, y1 = c1
 
-        else:
-            return line_start
+    if isinstance(c2, Point):
+        x2, y2 = c2.coords[0]
+    else:
+        x2, y2 = c2
 
-    ix = line_start.x + u * (line_end.x - line_start.x)
-    iy = line_start.y + u * (line_end.y - line_start.y)
-    return Point([ix, iy])
+    if ((x1 - x2) == 0) and ((y1 - y2) == 0):  # zero length line
+        x_new, y_new = x1, y1
+    else:
+        rel_length = numpy.minimum(
+            offset / numpy.sqrt((x1 - x2) ** 2 + (y1 - y2) ** 2), 1
+        )
+        x_new = x1 + (x2 - x1) * rel_length
+        y_new = y1 + (y2 - y1) * rel_length
 
+    return Point(x_new, y_new)
 
-def nearest_geometry(
-    geometries: Sequence[BaseGeometry], point: Point
-) -> Tuple[BaseGeometry, float, int]:
-    """Find the nearest geometry among a list, measured from fixed point.
 
-    :param geometries: a list of shapely geometry objects
-    :param point: a shapely Point
+def azimuth(point1: Point, point2: Point) -> float:
+    """
+    The clockwise angle from North to line of two points
 
-    :return:        Tuple (geom, min_dist, min_index) of the geometry with minimum distance        to point, its distance min_dist and the list index of geom, so that        geom = geometries[min_index].
+    :param point1:
+    :type point1: Point
+    :param point2:
+    :type point2: Point
+    :return: angle
+    :rtype: float
     """
-    min_dist, min_index = min(
-        (point.distance(geom), k) for (k, geom) in enumerate(geometries)
-    )
 
-    return geometries[min_index], min_dist, min_index
+    angle = numpy.arctan2(point2.x - point1.x, point2.y - point1.y)
+    # Gets the angle between the first and last coordinate of a linestring
+
+    return (
+        numpy.degrees(angle) if angle >= 0 else numpy.degrees(angle) + 360
+    ) % 180  # Modulo is used on the angle to produce a result between 0 and 180 degrees
+
+
+if __name__ == "__main__":
+    print(azimuth(Point(0, 0), Point(1, 1)))
+    print(azimuth(Point(1, 1), Point(0, 0)))
+
+    print(shift_point(Point(1, 1), Point(0, 0), 1))
+    print(shift_point(Point(1, 1), Point(0, 0), 2))
+    print(shift_point(Point(1, 1), Point(0, 0), 3))
+
+    print(shift_point(Point(0, 0), Point(1, 1), 1))
+    print(shift_point(Point(0, 0), Point(1, 1), 0))
```

### Comparing `Jord-0.1.2/jord/shapely_utilities/sanitise_poly.py` & `Jord-0.1.3/jord/shapely_utilities/polygons.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import statistics
-from typing import Union, Tuple, List
+from typing import Union, Tuple, List, Sequence
 
 from shapely.geometry import (
     LineString,
     LinearRing,
     MultiLineString,
     MultiPolygon,
     Polygon,
 )
 from shapely.geometry.base import BaseGeometry
 
-__all__ = ["zero_buffer", "sanitise", "deflimmer", "clean_geometry"]
+__all__ = ["zero_buffer", "sanitise", "deflimmer", "clean_geometry", "explode_polygons"]
 
+from warg import pairs
 from jord.shapely_utilities.morphology import opening, closing
+from jord.shapely_utilities.rings import ensure_ccw_ring, ensure_cw_ring
 
 
 def zero_buffer(
     geom: BaseGeometry,
 ) -> Union[
     BaseGeometry
     # Point,
@@ -111,30 +113,36 @@
     return (
         statistics.mean(poly_areas),
         statistics.stdev(poly_areas) if len(poly_areas) > 1 else 0,
     )
 
 
 def prune_area(geom: BaseGeometry, eps: float = 1e-7) -> BaseGeometry:
+    raise NotImplementedError
     poly_areas = []
     if isinstance(geom, Polygon):
         poly_areas.append(geom.area)
     elif isinstance(geom, MultiPolygon):
         for po in geom.geoms:
             poly_areas.append(po.area)
 
+    return poly_areas
+
 
 def prune_rings(geom: BaseGeometry, eps: float = 1e-7) -> BaseGeometry:
+    raise NotImplementedError
     poly_areas = []
     if isinstance(geom, Polygon):
         poly_areas.append(geom.area)
     elif isinstance(geom, MultiPolygon):
         for po in geom.geoms:
             poly_areas.append(po.area)
 
+    return poly_areas
+
 
 def sanitise(geom: BaseGeometry, *args: callable) -> BaseGeometry:
     """
 
     #A positive distance produces a dilation, a negative distance an erosion. A very small or zero distance may sometimes be used to “tidy” a polygon.
 
     """
@@ -144,14 +152,79 @@
 
     for f in args:
         geom = f(geom)
 
     return geom
 
 
+def ensure_ccw_poly(polygon: Polygon) -> Polygon:
+    """
+    This function checks if the polygon is counter-clockwise if not it is reversed
+
+
+    :param polygon: The polygon to check
+    :return: Returns the polygon turned clockwise
+    """
+
+    return Polygon(
+        shell=ensure_ccw_ring(polygon.exterior),
+        holes=[ensure_ccw_ring(hole) for hole in polygon.interiors],
+    )
+
+
+def ensure_cw_poly(polygon: Polygon) -> Polygon:
+    """
+    This function checks if the polygon is clockwise if not it is reversed
+
+
+    :param polygon: The polygon to check
+    :return: Returns the polygon turned clockwise
+    """
+
+    return Polygon(
+        shell=ensure_cw_ring(polygon.exterior),
+        holes=[ensure_cw_ring(hole) for hole in polygon.interiors],
+    )
+
+
+def explode_polygons(
+    polygons: Union[Polygon, MultiPolygon, Sequence[Polygon]],
+    return_index: bool = False,
+) -> Union[Sequence[LineString], Tuple[Sequence[LineString], Sequence[int]]]:
+    """
+    returns main line features that make up the polygons
+
+    :param polygons:
+    :param return_index:
+    :return:
+    """
+    lines_out = []
+    index = []
+
+    if isinstance(polygons, Polygon):
+        polygons = [polygons]
+
+    if isinstance(polygons, MultiPolygon):
+        polygons = polygons.geoms
+
+    for i, l in enumerate(polygons):
+        for s in [LineString(s) for s in pairs(l.exterior.coords)]:
+            lines_out.append(s)
+            index.append(i)
+
+        for p in l.interiors:
+            lines_out.append(LineString(p.coords))
+            index.append(i)
+
+    if return_index:
+        return lines_out, index
+
+    return lines_out
+
+
 if __name__ == "__main__":
 
     def aishdjauisd():
         # Import constructors for creating geometry collections
         from shapely.geometry import MultiPoint, MultiLineString
 
         # Import necessary geometric objects from shapely module
```

### Comparing `Jord-0.1.2/jord/shapely_utilities/serialisation/well_known_binary.py` & `Jord-0.1.3/jord/shapely_utilities/serialisation/well_known_binary.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/jord/shapely_utilities/serialisation/well_known_text.py` & `Jord-0.1.3/jord/shapely_utilities/serialisation/well_known_text.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/setup.py` & `Jord-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `Jord-0.1.2/tests/test_import.py` & `Jord-0.1.3/tests/test_import.py`

 * *Files identical despite different names*

