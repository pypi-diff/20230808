# Comparing `tmp/shapelets-platform-2.0.98.tar.gz` & `tmp/shapelets-platform-2.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapelets-platform-2.0.98.tar", last modified: Thu Aug  3 08:21:52 2023, max compression
+gzip compressed data, was "shapelets-platform-2.0.99.tar", last modified: Tue Aug  8 12:14:46 2023, max compression
```

## Comparing `shapelets-platform-2.0.98.tar` & `shapelets-platform-2.0.99.tar`

### file list

```diff
@@ -1,276 +1,276 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.291156 shapelets-platform-2.0.98/
--rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/COPYING.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1140 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (123)      144 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     6253 2023-08-03 08:21:52.295156 shapelets-platform-2.0.98/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4546 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1562 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/noxfile.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1219 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)     2856 2023-08-03 08:21:52.295156 shapelets-platform-2.0.98/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     4030 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.191154 shapelets-platform-2.0.98/src/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.199154 shapelets-platform-2.0.98/src/shapelets/
--rw-r--r--   0 vsts      (1001) docker     (123)      924 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8739 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/_api.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19266 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/_cli.py
--rw-r--r--   0 vsts      (1001) docker     (123)    52017 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/_relations.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4154 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/_uom.py
--rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-08-03 08:21:47.000000 shapelets-platform-2.0.98/src/shapelets/_version.py
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/_version.pyi
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.203154 shapelets-platform-2.0.98/src/shapelets/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)      242 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    70200 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/data_app.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/data_app_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.203154 shapelets-platform-2.0.98/src/shapelets/apps/widgets/
--rw-r--r--   0 vsts      (1001) docker     (123)      752 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3150 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/attribute_names.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.211155 shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/
--rw-r--r--   0 vsts      (1001) docker     (123)      768 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3364 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/altair_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2129 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/bar_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2584 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/folium_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2627 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/heatmap.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1783 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/histogram.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19323 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/line_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2129 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/pie_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/plotly_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2138 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/polar_area.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2937 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/radar_area.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4385 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/scatter_plot.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.211155 shapelets-platform-2.0.98/src/shapelets/apps/widgets/contexts/
--rw-r--r--   0 vsts      (1001) docker     (123)      504 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/contexts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1167 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/contexts/filtering_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1164 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/contexts/metadata_field.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1505 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/contexts/metadata_filter.py
--rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/contexts/temporal_context.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.223155 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/
--rw-r--r--   0 vsts      (1001) docker     (123)     1357 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2014 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/button.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/checkbox.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2243 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/collection_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8331 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/datetime_range_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8706 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/datetime_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4164 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/gauge.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8126 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/image.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1315 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/list.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5929 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/metric.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2108 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11032 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/number_input.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7391 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/progress.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9101 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/radio_group.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.223155 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/resources/
--rw-r--r--   0 vsts      (1001) docker     (123)    18534 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg
--rw-r--r--   0 vsts      (1001) docker     (123)     4631 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/ring.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10545 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1907 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/sequence_list.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1929 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/sequence_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14849 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/slider.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9255 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/table.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5969 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/text.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9017 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/text_input.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5622 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/timer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/datetime_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.227155 shapelets-platform-2.0.98/src/shapelets/apps/widgets/layouts/
--rw-r--r--   0 vsts      (1001) docker     (123)      359 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/layouts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/layouts/grid_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6038 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/layouts/horizontal_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1464 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/layouts/panel.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5000 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/layouts/tabs_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5660 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/layouts/vertical_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2756 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/util.py
--rw-r--r--   0 vsts      (1001) docker     (123)    26169 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/apps/widgets/widget.py
--rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4551 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/iris.csv
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.227155 shapelets-platform-2.0.98/src/shapelets/svr/
--rw-r--r--   0 vsts      (1001) docker     (123)    10262 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2459 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/app.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.231155 shapelets-platform-2.0.98/src/shapelets/svr/authn/
--rw-r--r--   0 vsts      (1001) docker     (123)     2484 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/authn/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8820 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/authn/authhttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10269 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/authn/authrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9665 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/authn/authservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5550 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/authn/gc_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2162 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/authn/iauthrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8976 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/authn/iauthservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.231155 shapelets-platform-2.0.98/src/shapelets/svr/data/
--rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/data/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.239155 shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/
--rw-r--r--   0 vsts      (1001) docker     (123)     7227 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      841 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/access_token_credentials.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3381 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/azure_gen1.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5728 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/azure_gen2.py
--rw-r--r--   0 vsts      (1001) docker     (123)      799 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/driver.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1311 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/dynamic_credentials.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1756 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/fsspec_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/fsspec_vfs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2429 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3806 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/fsspec_vfs_file.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2814 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/ftp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1837 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/local.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2029 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/protocols.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3512 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/smb.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3562 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/vfs_sample_config.toml
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.243155 shapelets-platform-2.0.98/src/shapelets/svr/dataapps/
--rw-r--r--   0 vsts      (1001) docker     (123)      792 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/dataapps/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3264 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/dataapps/dataapps_ws.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9912 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/dataapps/dataappshttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    25885 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/dataapps/dataappsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2415 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/dataapps/dataappsservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/dataapps/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1781 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/dataapps/idataappsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1515 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/dataapps/idataappsservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.243155 shapelets-platform-2.0.98/src/shapelets/svr/db/
--rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.247155 shapelets-platform-2.0.98/src/shapelets/svr/db/native/
--rw-r--r--   0 vsts      (1001) docker     (123)      235 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/db/native/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9162 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/db/native/database.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2242 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/db/native/settings.py
--rw-r--r--   0 vsts      (1001) docker     (123)      811 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/db/schema_builder.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3449 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/db/schema_v1.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3517 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/db/schema_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3956 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/db/schema_v3.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5579 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/db/schema_v4.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2021 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/db/setup.py
--rw-r--r--   0 vsts      (1001) docker     (123)      509 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/docs.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.251155 shapelets-platform-2.0.98/src/shapelets/svr/execution/
--rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/execution/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1710 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/execution/executionhttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/execution/executionrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2088 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/execution/executionservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/execution/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)      265 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/execution/iexecutionrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)      337 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/execution/iexecutionservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.255155 shapelets-platform-2.0.98/src/shapelets/svr/groups/
--rw-r--r--   0 vsts      (1001) docker     (123)      788 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/groups/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1603 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/groups/groupservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4410 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/groups/groupshttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5028 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/groups/groupsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)      458 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/groups/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/groups/igroupsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2633 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/groups/igroupsservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.255155 shapelets-platform-2.0.98/src/shapelets/svr/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      369 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      826 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/model/dataapps.py
--rw-r--r--   0 vsts      (1001) docker     (123)      179 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/model/function.py
--rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/model/groups.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/model/principals.py
--rw-r--r--   0 vsts      (1001) docker     (123)      867 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/model/users.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.263155 shapelets-platform-2.0.98/src/shapelets/svr/mustang/
--rw-r--r--   0 vsts      (1001) docker     (123)     2474 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/mustang/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18919 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/mustang/asttranslation.py
--rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/mustang/conversions.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13383 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/mustang/core.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35472 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/mustang/decompiling.py
--rw-r--r--   0 vsts      (1001) docker     (123)      874 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/mustang/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/mustang/hashdict.py
--rw-r--r--   0 vsts      (1001) docker     (123)      121 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/mustang/identifier.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5662 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/mustang/ormtypes.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.263155 shapelets-platform-2.0.98/src/shapelets/svr/mustang/prototypes/
--rw-r--r--   0 vsts      (1001) docker     (123)    18157 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/mustang/prototypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      267 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/mustang/python_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/mustang/serialization.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11997 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/mustang/sqlbuilding.py
--rw-r--r--   0 vsts      (1001) docker     (123)    66067 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/mustang/sqltranslation.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4102 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/server.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.267155 shapelets-platform-2.0.98/src/shapelets/svr/settings/
--rw-r--r--   0 vsts      (1001) docker     (123)      650 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/settings/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5189 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/settings/client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2155 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/settings/defaults.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/settings/functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/settings/http.py
--rw-r--r--   0 vsts      (1001) docker     (123)      707 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/settings/reload.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6905 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/settings/server.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6374 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/settings/settings.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5534 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/settings/settings.toml
--rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/settings/ssl.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/settings/telemetry.py
--rw-r--r--   0 vsts      (1001) docker     (123)      758 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/settings/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.271155 shapelets-platform-2.0.98/src/shapelets/svr/telemetry/
--rw-r--r--   0 vsts      (1001) docker     (123)      329 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/telemetry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      140 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/telemetry/itelemetryservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2613 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/telemetry/sysinfo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1778 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/telemetry/telemetryservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.271155 shapelets-platform-2.0.98/src/shapelets/svr/users/
--rw-r--r--   0 vsts      (1001) docker     (123)      685 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/users/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/users/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/users/iusersrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2653 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/users/iusersservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5587 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/users/usershttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13629 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/users/usersrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3583 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/users/usersservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.275155 shapelets-platform-2.0.98/src/shapelets/svr/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6279 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/utils/crypto.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1677 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/svr/utils/flexbytes.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.275155 shapelets-platform-2.0.98/src/shapelets/svr/www/
--rw-r--r--   0 vsts      (1001) docker     (123)   136375 2023-08-03 08:21:47.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/altair.json
--rw-r--r--   0 vsts      (1001) docker     (123)     4655 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/asset-manifest.json
--rw-r--r--   0 vsts      (1001) docker     (123)      246 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/custom_sample.js
--rw-r--r--   0 vsts      (1001) docker     (123)   109691 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/dataapp.json
--rw-r--r--   0 vsts      (1001) docker     (123)    17042 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/favicon.ico
--rw-r--r--   0 vsts      (1001) docker     (123)     4111 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/index.html
--rw-r--r--   0 vsts      (1001) docker     (123)      292 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/manifest.json
--rw-r--r--   0 vsts      (1001) docker     (123)       67 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/robots.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.191154 shapelets-platform-2.0.98/src/shapelets/svr/www/static/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.275155 shapelets-platform-2.0.98/src/shapelets/svr/www/static/css/
--rw-r--r--   0 vsts      (1001) docker     (123)    90519 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css
--rw-r--r--   0 vsts      (1001) docker     (123)    80997 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/css/main.6638be9e.chunk.css
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.287155 shapelets-platform-2.0.98/src/shapelets/svr/www/static/js/
--rw-r--r--   0 vsts      (1001) docker     (123)  7622607 2023-08-03 08:21:47.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/js/2.379683b2.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)    15949 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/js/2.379683b2.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)   173524 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)      808 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)    21772 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)      188 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)   808300 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/js/main.a03762f7.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)     2357 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/js/runtime-main.197d60a0.js
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.291156 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/
--rw-r--r--   0 vsts      (1001) docker     (123)      771 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1155 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/audit.cb539a06.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1129 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/bin.7e762965.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1274 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      918 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/clear.27b15301.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2092 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/collections.06fdf54a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1432 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3206 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3225 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2684 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1493 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/date-time.a1e86419.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1047 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/download-image.87310709.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/filter.cec803b8.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1531 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1476 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      852 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    21416 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    15532 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png
--rw-r--r--   0 vsts      (1001) docker     (123)    15668 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png
--rw-r--r--   0 vsts      (1001) docker     (123)     1265 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/logout.57c593a5.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1035 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2616 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2628 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/pdf.5d189efa.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      536 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      429 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/shapelets-vertical-line.2ebc031a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      935 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/share.bc9a8370.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      868 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1004 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/single-plot.864a583b.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3704 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      521 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    19199 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png
--rw-r--r--   0 vsts      (1001) docker     (123)    18616 2023-08-03 08:21:46.000000 shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/wave-top.6d51781b.png
--rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-08-03 08:08:17.000000 shapelets-platform-2.0.98/src/shapelets/systemd_template.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-03 08:21:52.291156 shapelets-platform-2.0.98/src/shapelets_platform.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     6253 2023-08-03 08:21:47.000000 shapelets-platform-2.0.98/src/shapelets_platform.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)    10804 2023-08-03 08:21:51.000000 shapelets-platform-2.0.98/src/shapelets_platform.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-03 08:21:47.000000 shapelets-platform-2.0.98/src/shapelets_platform.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-08-03 08:21:47.000000 shapelets-platform-2.0.98/src/shapelets_platform.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)     1146 2023-08-03 08:21:47.000000 shapelets-platform-2.0.98/src/shapelets_platform.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-08-03 08:21:47.000000 shapelets-platform-2.0.98/src/shapelets_platform.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.537252 shapelets-platform-2.0.99/
+-rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/COPYING.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1140 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/LICENSE.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      144 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     6253 2023-08-08 12:14:46.537252 shapelets-platform-2.0.99/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4546 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1562 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/noxfile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1219 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)     2856 2023-08-08 12:14:46.537252 shapelets-platform-2.0.99/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     4030 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.449251 shapelets-platform-2.0.99/src/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.457251 shapelets-platform-2.0.99/src/shapelets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      924 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8739 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/_api.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19266 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/_cli.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    52017 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/_relations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4154 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/_uom.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-08-08 12:14:42.000000 shapelets-platform-2.0.99/src/shapelets/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/_version.pyi
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.457251 shapelets-platform-2.0.99/src/shapelets/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)      242 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    70200 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/data_app.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/data_app_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.461251 shapelets-platform-2.0.99/src/shapelets/apps/widgets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      752 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3150 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/attribute_names.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.465251 shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      768 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3364 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/altair_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2129 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/bar_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2584 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/folium_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2627 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/heatmap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1783 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/histogram.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19323 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/line_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2129 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/pie_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/plotly_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2138 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/polar_area.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2937 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/radar_area.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4385 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/scatter_plot.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.465251 shapelets-platform-2.0.99/src/shapelets/apps/widgets/contexts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      504 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/contexts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1167 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/contexts/filtering_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1164 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/contexts/metadata_field.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1505 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/contexts/metadata_filter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/contexts/temporal_context.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.473251 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1357 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2014 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/button.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/checkbox.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2243 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/collection_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8331 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/datetime_range_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8706 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/datetime_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4164 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/gauge.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8126 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/image.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1315 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/list.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5929 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/metric.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2108 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11032 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/number_input.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7391 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/progress.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9101 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/radio_group.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.473251 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/resources/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18534 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg
+-rw-r--r--   0 vsts      (1001) docker     (123)     4631 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/ring.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10545 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1907 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/sequence_list.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1929 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/sequence_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14849 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/slider.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9255 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5969 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/text.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9017 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/text_input.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5622 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/timer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/datetime_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.477251 shapelets-platform-2.0.99/src/shapelets/apps/widgets/layouts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      359 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/layouts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/layouts/grid_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6511 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/layouts/horizontal_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1464 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/layouts/panel.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5389 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/layouts/tabs_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6147 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/layouts/vertical_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2756 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    26169 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/apps/widgets/widget.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4551 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/iris.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.477251 shapelets-platform-2.0.99/src/shapelets/svr/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10262 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2459 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/app.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.481251 shapelets-platform-2.0.99/src/shapelets/svr/authn/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2484 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/authn/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8820 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/authn/authhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10269 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/authn/authrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9665 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/authn/authservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5550 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/authn/gc_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2162 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/authn/iauthrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8976 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/authn/iauthservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.481251 shapelets-platform-2.0.99/src/shapelets/svr/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/data/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.485251 shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7227 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      841 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/access_token_credentials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3381 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/azure_gen1.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5728 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/azure_gen2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      799 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/driver.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1311 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/dynamic_credentials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1756 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/fsspec_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/fsspec_vfs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2429 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3806 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/fsspec_vfs_file.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2814 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/ftp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1837 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/local.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2029 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3512 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/smb.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3562 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/vfs_sample_config.toml
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.489251 shapelets-platform-2.0.99/src/shapelets/svr/dataapps/
+-rw-r--r--   0 vsts      (1001) docker     (123)      792 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/dataapps/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3264 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/dataapps/dataapps_ws.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9912 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/dataapps/dataappshttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    25885 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/dataapps/dataappsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2415 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/dataapps/dataappsservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/dataapps/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1781 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/dataapps/idataappsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1515 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/dataapps/idataappsservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.493251 shapelets-platform-2.0.99/src/shapelets/svr/db/
+-rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.493251 shapelets-platform-2.0.99/src/shapelets/svr/db/native/
+-rw-r--r--   0 vsts      (1001) docker     (123)      235 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/db/native/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9162 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/db/native/database.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2242 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/db/native/settings.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      811 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/db/schema_builder.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3449 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/db/schema_v1.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3517 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/db/schema_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3956 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/db/schema_v3.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5579 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/db/schema_v4.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2021 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/db/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      509 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/docs.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.497251 shapelets-platform-2.0.99/src/shapelets/svr/execution/
+-rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/execution/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1710 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/execution/executionhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/execution/executionrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2088 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/execution/executionservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/execution/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      265 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/execution/iexecutionrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      337 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/execution/iexecutionservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.497251 shapelets-platform-2.0.99/src/shapelets/svr/groups/
+-rw-r--r--   0 vsts      (1001) docker     (123)      788 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/groups/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1603 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/groups/groupservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4410 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/groups/groupshttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5028 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/groups/groupsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      458 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/groups/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/groups/igroupsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2633 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/groups/igroupsservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.501251 shapelets-platform-2.0.99/src/shapelets/svr/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      369 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      826 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/model/dataapps.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      179 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/model/function.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/model/groups.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/model/principals.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      867 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/model/users.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.505251 shapelets-platform-2.0.99/src/shapelets/svr/mustang/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2474 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/mustang/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18919 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/mustang/asttranslation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/mustang/conversions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13383 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/mustang/core.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    35472 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/mustang/decompiling.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      874 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/mustang/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/mustang/hashdict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      121 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/mustang/identifier.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5662 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/mustang/ormtypes.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.509251 shapelets-platform-2.0.99/src/shapelets/svr/mustang/prototypes/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18157 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/mustang/prototypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      267 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/mustang/python_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/mustang/serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11997 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/mustang/sqlbuilding.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    66067 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/mustang/sqltranslation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4102 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/server.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.513251 shapelets-platform-2.0.99/src/shapelets/svr/settings/
+-rw-r--r--   0 vsts      (1001) docker     (123)      650 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/settings/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5189 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/settings/client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2155 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/settings/defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/settings/functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/settings/http.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      707 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/settings/reload.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6905 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/settings/server.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6374 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/settings/settings.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5534 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/settings/settings.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/settings/ssl.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/settings/telemetry.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      758 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/settings/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.513251 shapelets-platform-2.0.99/src/shapelets/svr/telemetry/
+-rw-r--r--   0 vsts      (1001) docker     (123)      329 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/telemetry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      140 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/telemetry/itelemetryservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2613 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/telemetry/sysinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1778 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/telemetry/telemetryservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.517251 shapelets-platform-2.0.99/src/shapelets/svr/users/
+-rw-r--r--   0 vsts      (1001) docker     (123)      685 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/users/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/users/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/users/iusersrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2653 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/users/iusersservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5587 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/users/usershttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13629 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/users/usersrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3583 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/users/usersservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.517251 shapelets-platform-2.0.99/src/shapelets/svr/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6279 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/utils/crypto.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1677 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/svr/utils/flexbytes.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.517251 shapelets-platform-2.0.99/src/shapelets/svr/www/
+-rw-r--r--   0 vsts      (1001) docker     (123)   136375 2023-08-08 12:14:37.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/altair.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     4655 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/asset-manifest.json
+-rw-r--r--   0 vsts      (1001) docker     (123)      246 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/custom_sample.js
+-rw-r--r--   0 vsts      (1001) docker     (123)   109691 2023-08-08 12:14:41.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/dataapp.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    17042 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/favicon.ico
+-rw-r--r--   0 vsts      (1001) docker     (123)     4111 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/index.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      292 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/manifest.json
+-rw-r--r--   0 vsts      (1001) docker     (123)       67 2023-08-08 12:14:37.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/robots.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.449251 shapelets-platform-2.0.99/src/shapelets/svr/www/static/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.521251 shapelets-platform-2.0.99/src/shapelets/svr/www/static/css/
+-rw-r--r--   0 vsts      (1001) docker     (123)    90519 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css
+-rw-r--r--   0 vsts      (1001) docker     (123)    80997 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/css/main.6638be9e.chunk.css
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.529251 shapelets-platform-2.0.99/src/shapelets/svr/www/static/js/
+-rw-r--r--   0 vsts      (1001) docker     (123)  7622969 2023-08-08 12:14:42.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/js/2.20645982.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    15949 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/js/2.20645982.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)   173524 2023-08-08 12:14:40.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      808 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)    21772 2023-08-08 12:14:37.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      188 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)   810003 2023-08-08 12:14:37.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/js/main.613e103b.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)     2357 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/js/runtime-main.197d60a0.js
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.537252 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/
+-rw-r--r--   0 vsts      (1001) docker     (123)      771 2023-08-08 12:14:37.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1155 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/audit.cb539a06.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1129 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/bin.7e762965.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1274 2023-08-08 12:14:40.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      918 2023-08-08 12:14:37.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/clear.27b15301.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2092 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/collections.06fdf54a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1432 2023-08-08 12:14:37.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3206 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3225 2023-08-08 12:14:37.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2684 2023-08-08 12:14:37.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1493 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/date-time.a1e86419.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1047 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/download-image.87310709.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-08-08 12:14:37.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/filter.cec803b8.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1531 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1476 2023-08-08 12:14:40.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      852 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    21416 2023-08-08 12:14:37.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    15532 2023-08-08 12:14:37.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png
+-rw-r--r--   0 vsts      (1001) docker     (123)    15668 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     1265 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/logout.57c593a5.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1035 2023-08-08 12:14:37.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2616 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2628 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/pdf.5d189efa.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      536 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-08-08 12:14:40.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      429 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/shapelets-vertical-line.2ebc031a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      935 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/share.bc9a8370.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      868 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1004 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/single-plot.864a583b.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3704 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      521 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    19199 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png
+-rw-r--r--   0 vsts      (1001) docker     (123)    18616 2023-08-08 12:14:36.000000 shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/wave-top.6d51781b.png
+-rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-08-08 11:14:13.000000 shapelets-platform-2.0.99/src/shapelets/systemd_template.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 12:14:46.537252 shapelets-platform-2.0.99/src/shapelets_platform.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6253 2023-08-08 12:14:42.000000 shapelets-platform-2.0.99/src/shapelets_platform.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)    10804 2023-08-08 12:14:46.000000 shapelets-platform-2.0.99/src/shapelets_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-08 12:14:42.000000 shapelets-platform-2.0.99/src/shapelets_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-08-08 12:14:42.000000 shapelets-platform-2.0.99/src/shapelets_platform.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     1146 2023-08-08 12:14:42.000000 shapelets-platform-2.0.99/src/shapelets_platform.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-08-08 12:14:42.000000 shapelets-platform-2.0.99/src/shapelets_platform.egg-info/top_level.txt
```

### Comparing `shapelets-platform-2.0.98/LICENSE.md` & `shapelets-platform-2.0.99/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/PKG-INFO` & `shapelets-platform-2.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapelets-platform
-Version: 2.0.98
+Version: 2.0.99
 Summary: Data Scientist platform
 Home-page: https://shapelets.io
 Author: Shapelets Dev Team
 Author-email: info@shapelets.io
 Maintainer: Shapelets Dev Team
 Maintainer-email: info@shapelets.io
 Project-URL: Homepage, https://shapelets.io/
```

### Comparing `shapelets-platform-2.0.98/README.md` & `shapelets-platform-2.0.99/README.md`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/noxfile.py` & `shapelets-platform-2.0.99/noxfile.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/pyproject.toml` & `shapelets-platform-2.0.99/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/setup.cfg` & `shapelets-platform-2.0.99/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 	pandas ~= 2.0
 	psutil ~= 5.9
 	pyarrow ~= 12.0
 	py-cpuinfo ~= 9.0
 	pydantic ~= 1.10
 	PyNaCl ~= 1.5
 	requests ~= 2.31
-	shapelets_native == 2.0.98
+	shapelets_native == 2.0.99
 	tabulate ~= 0.9
 	tomlkit ~= 0.12
 	typing_extensions ~= 4.7
 	uvicorn ~= 0.23
 	websocket-client ~= 1.5
 	websockets ~= 10.3
 	lockfile ~= 0.12; platform_system!="Windows"
```

### Comparing `shapelets-platform-2.0.98/setup.py` & `shapelets-platform-2.0.99/setup.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/__init__.py` & `shapelets-platform-2.0.99/src/shapelets/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/_api.py` & `shapelets-platform-2.0.99/src/shapelets/_api.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/_cli.py` & `shapelets-platform-2.0.99/src/shapelets/_cli.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/_relations.py` & `shapelets-platform-2.0.99/src/shapelets/_relations.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/_uom.py` & `shapelets-platform-2.0.99/src/shapelets/_uom.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/data_app.py` & `shapelets-platform-2.0.99/src/shapelets/apps/data_app.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/data_app_utils.py` & `shapelets-platform-2.0.99/src/shapelets/apps/data_app_utils.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/__init__.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/attribute_names.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/attribute_names.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/__init__.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/altair_chart.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/altair_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/bar_chart.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/bar_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/folium_chart.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/folium_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/heatmap.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/heatmap.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/histogram.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/histogram.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/line_chart.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/line_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/pie_chart.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/pie_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/plotly_chart.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/polar_area.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/polar_area.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/radar_area.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/radar_area.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/charts/scatter_plot.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/charts/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/contexts/filtering_context.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/contexts/filtering_context.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/contexts/metadata_field.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/contexts/metadata_field.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/contexts/metadata_filter.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/contexts/metadata_filter.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/contexts/temporal_context.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/contexts/temporal_context.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/__init__.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/button.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/button.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/checkbox.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/checkbox.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/collection_selector.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/collection_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/datetime_range_selector.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/datetime_range_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/datetime_selector.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/datetime_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/gauge.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/gauge.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/image.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/image.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/list.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/list.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/metric.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/metric.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/number_input.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/number_input.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/progress.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/progress.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/radio_group.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/radio_group.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/ring.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/ring.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/selector.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/sequence_list.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/sequence_list.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/sequence_selector.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/sequence_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/slider.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/slider.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/table.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/table.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/text.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/text.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/text_input.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/text_input.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/controllers/timer.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/controllers/timer.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/datetime_utils.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/layouts/grid_layout.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/layouts/grid_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/layouts/horizontal_layout.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/layouts/horizontal_layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import uuid
 
 from dataclasses import dataclass, field
 from typing import Optional
 from typing_extensions import Literal
 
 from ..widget import Widget, AttributeNames
@@ -136,14 +138,24 @@
         """
         total = 0
         for key, (width, offset) in self.placements.items():
             total += width
             if total > 100:
                 raise Exception("The total width of the widgets cannot be over a 100")
 
+    def replace_widget(self, new_widget: HorizontalLayoutWidget):
+        """
+        Replace the current values of the widget for the values of a similar widget type.
+        """
+        self.panel_title = new_widget.panel_title
+        self.horizontal_align = new_widget.horizontal_align
+        self.vertical_align = new_widget.vertical_align
+        self.widgets = new_widget.widgets
+        self.placements = new_widget.placements
+
     def place(self, widget: Widget, width: Optional[float] = None, offset: Optional[int] = None):
         """
         Place widget inside layout
         param widget: widget to place.
         param width: understood as a percentage.
         param offset: distance with the next widget.
         """
```

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/layouts/panel.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/layouts/panel.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/layouts/tabs_layout.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/layouts/tabs_layout.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,14 +50,24 @@
 
     *Currently this widget cannot be used as input in a binding function.*              
     """
 
     tabs: Optional[Tuple[str, StateControl]] = field(default_factory=lambda: [])
     position: Optional[Literal["top", "bottom" "left", "right"]] = "bottom"
 
+    def replace_widget(self, new_widget: TabsLayout):
+        """
+        Replace the current values of the widget for the values of a similar widget type.
+        """
+        self.panel_title = new_widget.panel_title
+        self.tabs = new_widget.tabs
+        self.position = new_widget.position
+        self.widgets = new_widget.widgets
+        self.placements = new_widget.placements
+
     def add_tab(self, tab_title: str, component: StateControl) -> TabsLayout:
         if self.tabs is None:
             element = tab_title, component
             self.tabs = [element]
         else:
             my_list = list(self.tabs)
             element = tab_title, component
```

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/layouts/vertical_layout.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/layouts/vertical_layout.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import uuid
 
 from dataclasses import dataclass, field
 from typing import List, Optional
 from typing_extensions import Literal
 
 from ..widget import Widget, AttributeNames
@@ -119,14 +121,25 @@
                          compatibility=tuple([list.__name__, List._name, VerticalLayout.__name__]),
                          **additional)
         self.span = span
         self.offset = offset
         self.vertical_align = vertical_align
         self.placements = dict()
 
+    def replace_widget(self, new_widget: VerticalLayoutWidget):
+        """
+        Replace the current values of the widget for the values of a similar widget type.
+        """
+        self.panel_title = new_widget.panel_title
+        self.vertical_align = new_widget.vertical_align
+        self.span = new_widget.span
+        self.offset = new_widget.offset
+        self.widgets = new_widget.widgets
+        self.placements = new_widget.placements
+
     def place(self, widget: Widget, width: Optional[float] = None, offset: Optional[int] = None):
         """
         Place widget inside layout
         param widget: widget to place.
         param width: understood as a percentage.
         param offset: distance with the next widget.
         """
```

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/util.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/util.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/apps/widgets/widget.py` & `shapelets-platform-2.0.99/src/shapelets/apps/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/functions.py` & `shapelets-platform-2.0.99/src/shapelets/functions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/iris.csv` & `shapelets-platform-2.0.99/src/shapelets/iris.csv`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/__init__.py` & `shapelets-platform-2.0.99/src/shapelets/svr/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/app.py` & `shapelets-platform-2.0.99/src/shapelets/svr/app.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/authn/__init__.py` & `shapelets-platform-2.0.99/src/shapelets/svr/authn/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/authn/authhttp.py` & `shapelets-platform-2.0.99/src/shapelets/svr/authn/authhttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/authn/authrepo.py` & `shapelets-platform-2.0.99/src/shapelets/svr/authn/authrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/authn/authservice.py` & `shapelets-platform-2.0.99/src/shapelets/svr/authn/authservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/authn/gc_client.py` & `shapelets-platform-2.0.99/src/shapelets/svr/authn/gc_client.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/authn/iauthrepo.py` & `shapelets-platform-2.0.99/src/shapelets/svr/authn/iauthrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/authn/iauthservice.py` & `shapelets-platform-2.0.99/src/shapelets/svr/authn/iauthservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/data/__init__.py` & `shapelets-platform-2.0.99/src/shapelets/svr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/__init__.py` & `shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/access_token_credentials.py` & `shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/access_token_credentials.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/azure_gen1.py` & `shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/azure_gen1.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/azure_gen2.py` & `shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/azure_gen2.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/driver.py` & `shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/driver.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/dynamic_credentials.py` & `shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/dynamic_credentials.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/fsspec_config.py` & `shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/fsspec_config.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/fsspec_vfs.py` & `shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/fsspec_vfs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py` & `shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/fsspec_vfs_file.py` & `shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/fsspec_vfs_file.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/ftp.py` & `shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/ftp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/local.py` & `shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/local.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/protocols.py` & `shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/protocols.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/smb.py` & `shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/smb.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/data/vfs/vfs_sample_config.toml` & `shapelets-platform-2.0.99/src/shapelets/svr/data/vfs/vfs_sample_config.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/dataapps/__init__.py` & `shapelets-platform-2.0.99/src/shapelets/svr/dataapps/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/dataapps/dataapps_ws.py` & `shapelets-platform-2.0.99/src/shapelets/svr/dataapps/dataapps_ws.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/dataapps/dataappshttp.py` & `shapelets-platform-2.0.99/src/shapelets/svr/dataapps/dataappshttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/dataapps/dataappsrepo.py` & `shapelets-platform-2.0.99/src/shapelets/svr/dataapps/dataappsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/dataapps/dataappsservice.py` & `shapelets-platform-2.0.99/src/shapelets/svr/dataapps/dataappsservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/dataapps/http_docs.py` & `shapelets-platform-2.0.99/src/shapelets/svr/dataapps/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/dataapps/idataappsrepo.py` & `shapelets-platform-2.0.99/src/shapelets/svr/dataapps/idataappsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/dataapps/idataappsservice.py` & `shapelets-platform-2.0.99/src/shapelets/svr/dataapps/idataappsservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/db/native/database.py` & `shapelets-platform-2.0.99/src/shapelets/svr/db/native/database.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/db/native/settings.py` & `shapelets-platform-2.0.99/src/shapelets/svr/db/native/settings.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/db/schema_builder.py` & `shapelets-platform-2.0.99/src/shapelets/svr/db/schema_builder.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/db/schema_v1.py` & `shapelets-platform-2.0.99/src/shapelets/svr/db/schema_v1.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/db/schema_v2.py` & `shapelets-platform-2.0.99/src/shapelets/svr/db/schema_v2.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/db/schema_v3.py` & `shapelets-platform-2.0.99/src/shapelets/svr/db/schema_v3.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/db/schema_v4.py` & `shapelets-platform-2.0.99/src/shapelets/svr/db/schema_v4.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/db/setup.py` & `shapelets-platform-2.0.99/src/shapelets/svr/db/setup.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/execution/__init__.py` & `shapelets-platform-2.0.99/src/shapelets/svr/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/execution/executionhttp.py` & `shapelets-platform-2.0.99/src/shapelets/svr/execution/executionhttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/execution/executionservice.py` & `shapelets-platform-2.0.99/src/shapelets/svr/execution/executionservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/execution/http_docs.py` & `shapelets-platform-2.0.99/src/shapelets/svr/execution/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/groups/__init__.py` & `shapelets-platform-2.0.99/src/shapelets/svr/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/groups/groupservice.py` & `shapelets-platform-2.0.99/src/shapelets/svr/groups/groupservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/groups/groupshttp.py` & `shapelets-platform-2.0.99/src/shapelets/svr/groups/groupshttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/groups/groupsrepo.py` & `shapelets-platform-2.0.99/src/shapelets/svr/groups/groupsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/groups/igroupsrepo.py` & `shapelets-platform-2.0.99/src/shapelets/svr/groups/igroupsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/groups/igroupsservice.py` & `shapelets-platform-2.0.99/src/shapelets/svr/groups/igroupsservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/model/dataapps.py` & `shapelets-platform-2.0.99/src/shapelets/svr/model/dataapps.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/model/principals.py` & `shapelets-platform-2.0.99/src/shapelets/svr/model/principals.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/model/users.py` & `shapelets-platform-2.0.99/src/shapelets/svr/model/users.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/mustang/__init__.py` & `shapelets-platform-2.0.99/src/shapelets/svr/mustang/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/mustang/asttranslation.py` & `shapelets-platform-2.0.99/src/shapelets/svr/mustang/asttranslation.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/mustang/conversions.py` & `shapelets-platform-2.0.99/src/shapelets/svr/mustang/conversions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/mustang/core.py` & `shapelets-platform-2.0.99/src/shapelets/svr/mustang/core.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/mustang/decompiling.py` & `shapelets-platform-2.0.99/src/shapelets/svr/mustang/decompiling.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/mustang/exceptions.py` & `shapelets-platform-2.0.99/src/shapelets/svr/mustang/exceptions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/mustang/hashdict.py` & `shapelets-platform-2.0.99/src/shapelets/svr/mustang/hashdict.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/mustang/ormtypes.py` & `shapelets-platform-2.0.99/src/shapelets/svr/mustang/ormtypes.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/mustang/prototypes/__init__.py` & `shapelets-platform-2.0.99/src/shapelets/svr/mustang/prototypes/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/mustang/serialization.py` & `shapelets-platform-2.0.99/src/shapelets/svr/mustang/serialization.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/mustang/sqlbuilding.py` & `shapelets-platform-2.0.99/src/shapelets/svr/mustang/sqlbuilding.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/mustang/sqltranslation.py` & `shapelets-platform-2.0.99/src/shapelets/svr/mustang/sqltranslation.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/server.py` & `shapelets-platform-2.0.99/src/shapelets/svr/server.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/settings/__init__.py` & `shapelets-platform-2.0.99/src/shapelets/svr/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/settings/client.py` & `shapelets-platform-2.0.99/src/shapelets/svr/settings/client.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/settings/defaults.py` & `shapelets-platform-2.0.99/src/shapelets/svr/settings/defaults.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/settings/functions.py` & `shapelets-platform-2.0.99/src/shapelets/svr/settings/functions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/settings/http.py` & `shapelets-platform-2.0.99/src/shapelets/svr/settings/http.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/settings/reload.py` & `shapelets-platform-2.0.99/src/shapelets/svr/settings/reload.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/settings/server.py` & `shapelets-platform-2.0.99/src/shapelets/svr/settings/server.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/settings/settings.py` & `shapelets-platform-2.0.99/src/shapelets/svr/settings/settings.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/settings/settings.toml` & `shapelets-platform-2.0.99/src/shapelets/svr/settings/settings.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/settings/ssl.py` & `shapelets-platform-2.0.99/src/shapelets/svr/settings/ssl.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/settings/telemetry.py` & `shapelets-platform-2.0.99/src/shapelets/svr/settings/telemetry.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/settings/websocket.py` & `shapelets-platform-2.0.99/src/shapelets/svr/settings/websocket.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/telemetry/sysinfo.py` & `shapelets-platform-2.0.99/src/shapelets/svr/telemetry/sysinfo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/telemetry/telemetryservice.py` & `shapelets-platform-2.0.99/src/shapelets/svr/telemetry/telemetryservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/users/__init__.py` & `shapelets-platform-2.0.99/src/shapelets/svr/users/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/users/http_docs.py` & `shapelets-platform-2.0.99/src/shapelets/svr/users/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/users/iusersrepo.py` & `shapelets-platform-2.0.99/src/shapelets/svr/users/iusersrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/users/iusersservice.py` & `shapelets-platform-2.0.99/src/shapelets/svr/users/iusersservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/users/usershttp.py` & `shapelets-platform-2.0.99/src/shapelets/svr/users/usershttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/users/usersrepo.py` & `shapelets-platform-2.0.99/src/shapelets/svr/users/usersrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/users/usersservice.py` & `shapelets-platform-2.0.99/src/shapelets/svr/users/usersservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/utils/crypto.py` & `shapelets-platform-2.0.99/src/shapelets/svr/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/utils/flexbytes.py` & `shapelets-platform-2.0.99/src/shapelets/svr/utils/flexbytes.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/altair.json` & `shapelets-platform-2.0.99/src/shapelets/svr/www/altair.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/asset-manifest.json` & `shapelets-platform-2.0.99/src/shapelets/svr/www/asset-manifest.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8350840336134453%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/2.20645982.chunk.js'), (4, "*

 * *                  "'static/js/main.613e103b.chunk.js')], delete: [4, 2]}",*

 * * "'files'": "{'main.js': '/app/static/js/main.613e103b.chunk.js', 'static/js/2.20645982.chunk.js': "*

 * *            "'/app/static/js/2.20645982.chunk.js', 'static/js/2.20645982.chunk.js.LICENSE.txt': "*

 * *            "'/app/static/js/2.20645982.chunk.js.LICENSE.txt', delete: "*

 * *            "['static/js/2.379683b2.chunk.js', 'static/js/2.379683b2.chunk.js.LICENSE.txt']} […]*

```diff
@@ -1,23 +1,23 @@
 {
     "entrypoints": [
         "static/js/runtime-main.197d60a0.js",
         "static/css/2.5f981f7f.chunk.css",
-        "static/js/2.379683b2.chunk.js",
+        "static/js/2.20645982.chunk.js",
         "static/css/main.6638be9e.chunk.css",
-        "static/js/main.a03762f7.chunk.js"
+        "static/js/main.613e103b.chunk.js"
     ],
     "files": {
         "index.html": "/app/index.html",
         "main.css": "/app/static/css/main.6638be9e.chunk.css",
-        "main.js": "/app/static/js/main.a03762f7.chunk.js",
+        "main.js": "/app/static/js/main.613e103b.chunk.js",
         "runtime-main.js": "/app/static/js/runtime-main.197d60a0.js",
         "static/css/2.5f981f7f.chunk.css": "/app/static/css/2.5f981f7f.chunk.css",
-        "static/js/2.379683b2.chunk.js": "/app/static/js/2.379683b2.chunk.js",
-        "static/js/2.379683b2.chunk.js.LICENSE.txt": "/app/static/js/2.379683b2.chunk.js.LICENSE.txt",
+        "static/js/2.20645982.chunk.js": "/app/static/js/2.20645982.chunk.js",
+        "static/js/2.20645982.chunk.js.LICENSE.txt": "/app/static/js/2.20645982.chunk.js.LICENSE.txt",
         "static/js/3.43e88e5e.chunk.js": "/app/static/js/3.43e88e5e.chunk.js",
         "static/js/3.43e88e5e.chunk.js.LICENSE.txt": "/app/static/js/3.43e88e5e.chunk.js.LICENSE.txt",
         "static/js/4.153f1d29.chunk.js": "/app/static/js/4.153f1d29.chunk.js",
         "static/js/4.153f1d29.chunk.js.LICENSE.txt": "/app/static/js/4.153f1d29.chunk.js.LICENSE.txt",
         "static/media/LoginPage.less": "/app/static/media/login-background.fa1c48cf.svg",
         "static/media/ShapeletsWave.less": "/app/static/media/wave-top.6d51781b.png",
         "static/media/angle-arrow.fd898372.svg": "/app/static/media/angle-arrow.fd898372.svg",
```

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/dataapp.json` & `shapelets-platform-2.0.99/src/shapelets/svr/www/dataapp.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/favicon.ico` & `shapelets-platform-2.0.99/src/shapelets/svr/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/index.html` & `shapelets-platform-2.0.99/src/shapelets/svr/www/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><base href="/app/"/><meta charset="utf-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><meta name="theme-color" content="#000000"/><meta name="author" content="Grumpy Cat Software S.L."/><meta property="og:type" content="website"/><meta property="og:image" itemprop="image" content="https://shapelets.io/doc/_static/shapeletslogo.png"/><meta property="og:url" content="/"/><meta property="og:site_name" content="Shapelets"/><meta name="description" content="Shapelets is an open source framework for time series analysis in big data environments. Easy to integrate with any database, high-performance (GPUs, CPU and multicore) and scalable."/><link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet"/><link rel="shortcut icon" href="favicon.ico"/><link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/leaflet/1.3.1/leaflet.css"/><link rel="stylesheet" href="//cdn.rawgit.com/konpa/devicon/df6431e323547add1b4cf45992913f15286456d3/devicon.min.css"/><link rel="preconnect" href="https://fonts.googleapis.com"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin/><link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet"/><link rel="manifest" href="/app/manifest.json"/><title>Shapelets</title><link href="/app/static/css/2.5f981f7f.chunk.css" rel="stylesheet"><link href="/app/static/css/main.6638be9e.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="ShapeletsUI"></div><script>!function(e){function t(t){for(var n,a,i=t[0],c=t[1],l=t[2],f=0,p=[];f<i.length;f++)a=i[f],Object.prototype.hasOwnProperty.call(o,a)&&o[a]&&p.push(o[a][0]),o[a]=0;for(n in c)Object.prototype.hasOwnProperty.call(c,n)&&(e[n]=c[n]);for(s&&s(t);p.length;)p.shift()();return u.push.apply(u,l||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,i=1;i<r.length;i++){var c=r[i];0!==o[c]&&(n=!1)}n&&(u.splice(t--,1),e=a(a.s=r[0]))}return e}var n={},o={1:0},u=[];function a(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,a),r.l=!0,r.exports}a.e=function(e){var t=[],r=o[e];if(0!==r)if(r)t.push(r[2]);else{var n=new Promise((function(t,n){r=o[e]=[t,n]}));t.push(r[2]=n);var u,i=document.createElement("script");i.charset="utf-8",i.timeout=120,a.nc&&i.setAttribute("nonce",a.nc),i.src=function(e){return a.p+"static/js/"+({}[e]||e)+"."+{3:"43e88e5e",4:"153f1d29"}[e]+".chunk.js"}(e);var c=new Error;u=function(t){i.onerror=i.onload=null,clearTimeout(l);var r=o[e];if(0!==r){if(r){var n=t&&("load"===t.type?"missing":t.type),u=t&&t.target&&t.target.src;c.message="Loading chunk "+e+" failed.\n("+n+": "+u+")",c.name="ChunkLoadError",c.type=n,c.request=u,r[1](c)}o[e]=void 0}};var l=setTimeout((function(){u({type:"timeout",target:i})}),12e4);i.onerror=i.onload=u,document.head.appendChild(i)}return Promise.all(t)},a.m=e,a.c=n,a.d=function(e,t,r){a.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},a.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},a.t=function(e,t){if(1&t&&(e=a(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(a.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)a.d(r,n,function(t){return e[t]}.bind(null,n));return r},a.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return a.d(t,"a",t),t},a.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},a.p="/app/",a.oe=function(e){throw console.error(e),e};var i=this["webpackJsonp@shapelets/cristal-ui"]=this["webpackJsonp@shapelets/cristal-ui"]||[],c=i.push.bind(i);i.push=t,i=i.slice();for(var l=0;l<i.length;l++)t(i[l]);var s=c;r()}([])</script><script src="/app/static/js/2.379683b2.chunk.js"></script><script src="/app/static/js/main.a03762f7.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><base href="/app/"/><meta charset="utf-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><meta name="theme-color" content="#000000"/><meta name="author" content="Grumpy Cat Software S.L."/><meta property="og:type" content="website"/><meta property="og:image" itemprop="image" content="https://shapelets.io/doc/_static/shapeletslogo.png"/><meta property="og:url" content="/"/><meta property="og:site_name" content="Shapelets"/><meta name="description" content="Shapelets is an open source framework for time series analysis in big data environments. Easy to integrate with any database, high-performance (GPUs, CPU and multicore) and scalable."/><link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet"/><link rel="shortcut icon" href="favicon.ico"/><link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/leaflet/1.3.1/leaflet.css"/><link rel="stylesheet" href="//cdn.rawgit.com/konpa/devicon/df6431e323547add1b4cf45992913f15286456d3/devicon.min.css"/><link rel="preconnect" href="https://fonts.googleapis.com"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin/><link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet"/><link rel="manifest" href="/app/manifest.json"/><title>Shapelets</title><link href="/app/static/css/2.5f981f7f.chunk.css" rel="stylesheet"><link href="/app/static/css/main.6638be9e.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="ShapeletsUI"></div><script>!function(e){function t(t){for(var n,a,i=t[0],c=t[1],l=t[2],f=0,p=[];f<i.length;f++)a=i[f],Object.prototype.hasOwnProperty.call(o,a)&&o[a]&&p.push(o[a][0]),o[a]=0;for(n in c)Object.prototype.hasOwnProperty.call(c,n)&&(e[n]=c[n]);for(s&&s(t);p.length;)p.shift()();return u.push.apply(u,l||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,i=1;i<r.length;i++){var c=r[i];0!==o[c]&&(n=!1)}n&&(u.splice(t--,1),e=a(a.s=r[0]))}return e}var n={},o={1:0},u=[];function a(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,a),r.l=!0,r.exports}a.e=function(e){var t=[],r=o[e];if(0!==r)if(r)t.push(r[2]);else{var n=new Promise((function(t,n){r=o[e]=[t,n]}));t.push(r[2]=n);var u,i=document.createElement("script");i.charset="utf-8",i.timeout=120,a.nc&&i.setAttribute("nonce",a.nc),i.src=function(e){return a.p+"static/js/"+({}[e]||e)+"."+{3:"43e88e5e",4:"153f1d29"}[e]+".chunk.js"}(e);var c=new Error;u=function(t){i.onerror=i.onload=null,clearTimeout(l);var r=o[e];if(0!==r){if(r){var n=t&&("load"===t.type?"missing":t.type),u=t&&t.target&&t.target.src;c.message="Loading chunk "+e+" failed.\n("+n+": "+u+")",c.name="ChunkLoadError",c.type=n,c.request=u,r[1](c)}o[e]=void 0}};var l=setTimeout((function(){u({type:"timeout",target:i})}),12e4);i.onerror=i.onload=u,document.head.appendChild(i)}return Promise.all(t)},a.m=e,a.c=n,a.d=function(e,t,r){a.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},a.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},a.t=function(e,t){if(1&t&&(e=a(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(a.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)a.d(r,n,function(t){return e[t]}.bind(null,n));return r},a.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return a.d(t,"a",t),t},a.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},a.p="/app/",a.oe=function(e){throw console.error(e),e};var i=this["webpackJsonp@shapelets/cristal-ui"]=this["webpackJsonp@shapelets/cristal-ui"]||[],c=i.push.bind(i);i.push=t,i=i.slice();for(var l=0;l<i.length;l++)t(i[l]);var s=c;r()}([])</script><script src="/app/static/js/2.20645982.chunk.js"></script><script src="/app/static/js/main.613e103b.chunk.js"></script></body></html>
```

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/css/main.6638be9e.chunk.css` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/css/main.6638be9e.chunk.css`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/js/2.379683b2.chunk.js` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/js/2.20645982.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 2.379683b2.chunk.js.LICENSE.txt */
+/*! For license information please see 2.20645982.chunk.js.LICENSE.txt */
 (this["webpackJsonp@shapelets/cristal-ui"] = this["webpackJsonp@shapelets/cristal-ui"] || []).push([
     [2],
     [function(t, e, n) {
         "use strict";
         t.exports = n(866)
     }, function(t, e, n) {
         "use strict";
@@ -265612,14 +265612,34 @@
                         return i(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return [4, this.httpClient.fetch({
                                         method: "GET",
                                         url: o.toUrl(this.httpClient.url, this.urlBase, t),
                                         params: {
+                                            id: t
+                                        },
+                                        withCredentials: !0
+                                    })];
+                                case 1:
+                                    if (200 !== (e = n.sent()).status) throw this.httpClient.error(e);
+                                    return [2, e.data]
+                            }
+                        }))
+                    }))
+                }, t.prototype.findOneByName = function(t) {
+                    return r(this, void 0, void 0, (function() {
+                        var e;
+                        return i(this, (function(n) {
+                            switch (n.label) {
+                                case 0:
+                                    return [4, this.httpClient.fetch({
+                                        method: "GET",
+                                        url: o.toUrl(this.httpClient.url, this.urlBase, "name", t),
+                                        params: {
                                             dataAppName: t
                                         },
                                         withCredentials: !0
                                     })];
                                 case 1:
                                     if (200 !== (e = n.sent()).status) throw this.httpClient.error(e);
                                     return [2, e.data]
```

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/js/2.379683b2.chunk.js.LICENSE.txt` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/js/2.20645982.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/js/4.153f1d29.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/js/main.a03762f7.chunk.js` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/js/main.613e103b.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -13690,25 +13690,28 @@
                                                             parameters: c,
                                                             result: o.result
                                                         }, n.prev = 6, n.next = 9, t.getDataAppFunctionResult(l);
                                                     case 9:
                                                         void 0 !== typeof(u = n.sent) && void 0 !== u.type && (d = [], void 0 !== (p = u.properties.widgets) && p.forEach((function(e) {
                                                             t.buildWidgets(e, d)
                                                         })), d.length > 1 && (t.makeActionableWidgets(d), d.forEach((function(e) {
-                                                            void 0 !== e.bind && null !== e.bind && e.bind.forEach((function(e) {
-                                                                var a = e.parameters.length > 1 ? {
-                                                                        name: e.parameters.name,
-                                                                        type: e.parameters.type,
-                                                                        default: e.parameters.default
-                                                                    } : [],
-                                                                    n = {
-                                                                        body: e.fn,
-                                                                        parameters: a,
-                                                                        result: e.result
-                                                                    };
+                                                            e.otherWidgets = d, void 0 !== e.bind && null !== e.bind && e.bind.forEach((function(e) {
+                                                                var a = [];
+                                                                void 0 !== e.parameters && e.parameters.forEach((function(e) {
+                                                                    a.push({
+                                                                        name: e.name,
+                                                                        type: e.type,
+                                                                        default: e.default
+                                                                    })
+                                                                }));
+                                                                var n = {
+                                                                    body: e.fn,
+                                                                    parameters: a,
+                                                                    result: e.result
+                                                                };
                                                                 t.functions[e.fn] = n
                                                             }))
                                                         }))), e.functionWidgets = d), e.setProperties(Object(s.a)({}, u.properties)), n.next = 17;
                                                         break;
                                                     case 14:
                                                         n.prev = 14, n.t0 = n.catch(6), H.a.error({
                                                             message: "".concat(n.t0, ". Runtime error executing ").concat(i.fn)
@@ -13844,15 +13847,15 @@
                                                 break
                                             }
                                             return e.next = 3, s.props.dataAppStore.findDataAppByVersion(t, a, r);
                                         case 3:
                                             e.t0 = e.sent, e.next = 9;
                                             break;
                                         case 6:
-                                            return e.next = 8, s.props.dataAppStore.findOne(t);
+                                            return e.next = 8, s.props.dataAppStore.findOneByName(t);
                                         case 8:
                                             e.t0 = e.sent;
                                         case 9:
                                             return i = e.t0, o = s.headerEditedLocale(), c = ve.a.unix(i.updateDate).locale(o), s.props.headerService.setEdited(c.format("D MMMM YYYY HH:mm:ss")), e.next = 15, s.props.dataAppStore.getDataAppSpec(i.specId);
                                         case 15:
                                             l = e.sent, u = sr({
                                                 spec: l,
@@ -13872,41 +13875,65 @@
                                 return e.apply(this, arguments)
                             }
                         }(), s.state = {}, s
                     }
                     return Object(o.a)(a, [{
                         key: "componentDidMount",
                         value: function() {
-                            var e = this,
-                                t = this.props.match.params,
-                                a = t.id,
-                                s = t.major,
-                                i = t.minor;
-                            this.getDataAppByName(a, s, i), this.wsConnection = this.props.dataAppStore.onReloadDataApp(a, function() {
-                                var t = Object(r.a)(Object(n.a)().mark((function t(a) {
-                                    var s, r, i, o;
-                                    return Object(n.a)().wrap((function(t) {
-                                        for (;;) switch (t.prev = t.next) {
-                                            case 0:
-                                                a.includes("delete") ? (H.a.error({
-                                                    message: "".concat(a.split(":")[0], " with version ").concat(a.split(":")[3], " has been deleted")
-                                                }), e.props.history.push(Ai.dataApps.path)) : (H.a.success({
-                                                    message: "".concat(a.split(":")[1], " with version ").concat(a.split(":")[3], " has been updated")
-                                                }), s = a.split(":")[1], r = a.split(":")[3], i = Number(r.split(".")[0]), o = Number(r.split(".")[1]), e.updatePage(s, i, o));
-                                            case 1:
-                                            case "end":
-                                                return t.stop()
-                                        }
-                                    }), t)
-                                })));
-                                return function(e) {
-                                    return t.apply(this, arguments)
-                                }
-                            }())
-                        }
+                            var e = Object(r.a)(Object(n.a)().mark((function e() {
+                                var t, a, s, i, o, c = this;
+                                return Object(n.a)().wrap((function(e) {
+                                    for (;;) switch (e.prev = e.next) {
+                                        case 0:
+                                            return t = this.props.match.params, a = t.id, s = t.major, i = t.minor, e.next = 3, this.props.userStore.findMe();
+                                        case 3:
+                                            o = e.sent, this.getDataAppByName(a, s, i), this.wsConnection = this.props.dataAppStore.onReloadDataApp(a, function() {
+                                                var e = Object(r.a)(Object(n.a)().mark((function e(t) {
+                                                    var a, s, r, i, l, u;
+                                                    return Object(n.a)().wrap((function(e) {
+                                                        for (;;) switch (e.prev = e.next) {
+                                                            case 0:
+                                                                if (!t.includes("delete")) {
+                                                                    e.next = 7;
+                                                                    break
+                                                                }
+                                                                a = t.split(":")[0], s = t.split(":")[3], r = t.split(":")[5], String(o.uid) === s && (H.a.error({
+                                                                    message: "".concat(a, " with version ").concat(r, " has been deleted")
+                                                                }), c.props.history.push(Ai.dataApp.path)), e.next = 15;
+                                                                break;
+                                                            case 7:
+                                                                if (i = t.split(":")[1], l = t.split(":")[3], String(o.uid) !== l) {
+                                                                    e.next = 15;
+                                                                    break
+                                                                }
+                                                                return e.next = 12, c.props.dataAppStore.findOne(i);
+                                                            case 12:
+                                                                u = e.sent, H.a.success({
+                                                                    message: "".concat(u.name, " with version ").concat(u.major, ".").concat(u.minor, " has been updated")
+                                                                }), c.updatePage(u.name, u.major, u.minor);
+                                                            case 15:
+                                                            case "end":
+                                                                return e.stop()
+                                                        }
+                                                    }), e)
+                                                })));
+                                                return function(t) {
+                                                    return e.apply(this, arguments)
+                                                }
+                                            }());
+                                        case 6:
+                                        case "end":
+                                            return e.stop()
+                                    }
+                                }), e, this)
+                            })));
+                            return function() {
+                                return e.apply(this, arguments)
+                            }
+                        }()
                     }, {
                         key: "componentWillUnmount",
                         value: function() {
                             this.wsConnection && this.wsConnection()
                         }
                     }, {
                         key: "headerEditedLocale",
@@ -14571,39 +14598,70 @@
                                 key: t
                             })
                         }, s.state = {}, s
                     }
                     return Object(o.a)(a, [{
                         key: "componentDidMount",
                         value: function() {
-                            var e = this;
-                            document.title = this.props.intl.formatMessage(y.a.dataAppsTitle), this.props.headerService.setTitle(this.props.intl.formatMessage(y.a.dataApps)), this.props.headerService.setVersion(void 0), this.props.headerService.setActions(void 0), this.props.headerService.setFilters({
-                                name: !0,
-                                description: !0
-                            }), this.props.headerService.setOnChange(this.onChangeFilter), this.props.headerService.setOnClear(this.onClearFilter), this.getDataApps(), this.wsConnection = this.props.dataAppStore.onReloadDataApp("*", function() {
-                                var t = Object(r.a)(Object(n.a)().mark((function t(a) {
-                                    return Object(n.a)().wrap((function(t) {
-                                        for (;;) switch (t.prev = t.next) {
-                                            case 0:
-                                                a.includes("*:delete") ? H.a.error({
-                                                    message: "".concat(a.split(":")[3], " with version ").concat(a.split(":")[5], " has been deleted")
-                                                }) : H.a.success({
-                                                    message: "".concat(a.split(":")[2], " with version ").concat(a.split(":")[4], " has been updated")
-                                                }), e.getDataApps();
-                                            case 2:
-                                            case "end":
-                                                return t.stop()
-                                        }
-                                    }), t)
-                                })));
-                                return function(e) {
-                                    return t.apply(this, arguments)
-                                }
-                            }())
-                        }
+                            var e = Object(r.a)(Object(n.a)().mark((function e() {
+                                var t, a = this;
+                                return Object(n.a)().wrap((function(e) {
+                                    for (;;) switch (e.prev = e.next) {
+                                        case 0:
+                                            return document.title = this.props.intl.formatMessage(y.a.dataAppsTitle), this.props.headerService.setTitle(this.props.intl.formatMessage(y.a.dataApps)), this.props.headerService.setVersion(void 0), this.props.headerService.setActions(void 0), this.props.headerService.setFilters({
+                                                name: !0,
+                                                description: !0
+                                            }), this.props.headerService.setOnChange(this.onChangeFilter), this.props.headerService.setOnClear(this.onClearFilter), this.getDataApps(), e.next = 10, this.props.userStore.findMe();
+                                        case 10:
+                                            t = e.sent, this.wsConnection = this.props.dataAppStore.onReloadDataApp("*", function() {
+                                                var e = Object(r.a)(Object(n.a)().mark((function e(s) {
+                                                    var r, i, o, c, l, u;
+                                                    return Object(n.a)().wrap((function(e) {
+                                                        for (;;) switch (e.prev = e.next) {
+                                                            case 0:
+                                                                if (!s.includes("*:delete")) {
+                                                                    e.next = 7;
+                                                                    break
+                                                                }
+                                                                r = s.split(":")[3], i = s.split(":")[5], o = s.split(":")[7], String(t.uid) === i && H.a.error({
+                                                                    message: "".concat(r, " with version ").concat(o, " has been deleted")
+                                                                }), e.next = 14;
+                                                                break;
+                                                            case 7:
+                                                                if (c = s.split(":")[2], l = s.split(":")[4], String(t.uid) !== l) {
+                                                                    e.next = 14;
+                                                                    break
+                                                                }
+                                                                return e.next = 12, a.props.dataAppStore.findOne(c);
+                                                            case 12:
+                                                                u = e.sent, H.a.success({
+                                                                    message: "".concat(u.name, " with version ").concat(u.major, ".").concat(u.minor, " has been updated")
+                                                                });
+                                                            case 14:
+                                                                a.getDataApps();
+                                                            case 15:
+                                                            case "end":
+                                                                return e.stop()
+                                                        }
+                                                    }), e)
+                                                })));
+                                                return function(t) {
+                                                    return e.apply(this, arguments)
+                                                }
+                                            }());
+                                        case 12:
+                                        case "end":
+                                            return e.stop()
+                                    }
+                                }), e, this)
+                            })));
+                            return function() {
+                                return e.apply(this, arguments)
+                            }
+                        }()
                     }, {
                         key: "componentWillUnmount",
                         value: function() {
                             this.props.headerService.setFilters(), this.props.headerService.setOnChange(), this.props.headerService.setOnClear(), this.wsConnection && this.wsConnection()
                         }
                     }, {
                         key: "render",
@@ -14982,36 +15040,67 @@
                                 }
                             })]
                         }, o.state = {}, o
                     }
                     return Object(o.a)(a, [{
                         key: "componentDidMount",
                         value: function() {
-                            var e = this;
-                            this.getDataApps(), this.wsConnection = this.props.dataAppStore.onReloadDataApp("*", function() {
-                                var t = Object(r.a)(Object(n.a)().mark((function t(a) {
-                                    return Object(n.a)().wrap((function(t) {
-                                        for (;;) switch (t.prev = t.next) {
-                                            case 0:
-                                                a.includes("*:delete") ? H.a.error({
-                                                    message: "".concat(a.split(":")[3], " with version ").concat(a.split(":")[5], " has been deleted")
-                                                }) : H.a.success({
-                                                    message: "".concat(a.split(":")[2], " with version ").concat(a.split(":")[4], " has been updated")
-                                                }), e.getDataApps();
-                                            case 2:
-                                            case "end":
-                                                return t.stop()
-                                        }
-                                    }), t)
-                                })));
-                                return function(e) {
-                                    return t.apply(this, arguments)
-                                }
-                            }())
-                        }
+                            var e = Object(r.a)(Object(n.a)().mark((function e() {
+                                var t, a = this;
+                                return Object(n.a)().wrap((function(e) {
+                                    for (;;) switch (e.prev = e.next) {
+                                        case 0:
+                                            return this.getDataApps(), e.next = 3, this.props.userStore.findMe();
+                                        case 3:
+                                            t = e.sent, this.wsConnection = this.props.dataAppStore.onReloadDataApp("*", function() {
+                                                var e = Object(r.a)(Object(n.a)().mark((function e(s) {
+                                                    var r, i, o, c, l, u;
+                                                    return Object(n.a)().wrap((function(e) {
+                                                        for (;;) switch (e.prev = e.next) {
+                                                            case 0:
+                                                                if (console.log("Section ", s), !s.includes("*:delete")) {
+                                                                    e.next = 8;
+                                                                    break
+                                                                }
+                                                                r = s.split(":")[3], i = s.split(":")[5], o = s.split(":")[7], String(t.uid) === i && H.a.error({
+                                                                    message: "".concat(r, " with version ").concat(o, " has been deleted")
+                                                                }), e.next = 15;
+                                                                break;
+                                                            case 8:
+                                                                if (c = s.split(":")[2], l = s.split(":")[4], String(t.uid) !== l) {
+                                                                    e.next = 15;
+                                                                    break
+                                                                }
+                                                                return e.next = 13, a.props.dataAppStore.findOne(c);
+                                                            case 13:
+                                                                u = e.sent, H.a.success({
+                                                                    message: "".concat(u.name, " with version ").concat(u.major, ".").concat(u.minor, " has been updated")
+                                                                });
+                                                            case 15:
+                                                                a.getDataApps();
+                                                            case 16:
+                                                            case "end":
+                                                                return e.stop()
+                                                        }
+                                                    }), e)
+                                                })));
+                                                return function(t) {
+                                                    return e.apply(this, arguments)
+                                                }
+                                            }());
+                                        case 5:
+                                        case "end":
+                                            return e.stop()
+                                    }
+                                }), e, this)
+                            })));
+                            return function() {
+                                return e.apply(this, arguments)
+                            }
+                        }()
                     }, {
                         key: "componentWillUnmount",
                         value: function() {
                             this.wsConnection && this.wsConnection()
                         }
                     }, {
                         key: "render",
@@ -20722,14 +20811,16 @@
                         return a.shapeletsAPI.dataAppAPI.findAll()
                     }, this.findAllByUsers = function() {
                         return a.shapeletsAPI.dataAppAPI.findAllByUsers()
                     }, this.findAllByGroups = function() {
                         return a.shapeletsAPI.dataAppAPI.findAllByGroups()
                     }, this.findOne = function(e) {
                         return a.shapeletsAPI.dataAppAPI.findOne(e)
+                    }, this.findOneByName = function(e) {
+                        return a.shapeletsAPI.dataAppAPI.findOneByName(e)
                     }, this.createOne = function(e) {
                         return a.shapeletsAPI.dataAppAPI.createOne(e)
                     }, this.updateOne = function(e) {
                         return a.shapeletsAPI.dataAppAPI.updateOne(e)
                     }, this.findVersions = function(e) {
                         return a.shapeletsAPI.dataAppAPI.findVersions(e)
                     }, this.getDataAppSpec = function(e) {
```

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/js/runtime-main.197d60a0.js` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/js/runtime-main.197d60a0.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/audit.cb539a06.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/audit.cb539a06.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/bin.7e762965.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/bin.7e762965.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/clear.27b15301.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/clear.27b15301.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/collections.06fdf54a.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/collections.06fdf54a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/date-time.a1e86419.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/date-time.a1e86419.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/download-image.87310709.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/download-image.87310709.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/filter.cec803b8.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/filter.cec803b8.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/logout.57c593a5.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/logout.57c593a5.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/pdf.5d189efa.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/pdf.5d189efa.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/share.bc9a8370.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/share.bc9a8370.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/single-plot.864a583b.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/single-plot.864a583b.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets/svr/www/static/media/wave-top.6d51781b.png` & `shapelets-platform-2.0.99/src/shapelets/svr/www/static/media/wave-top.6d51781b.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.98/src/shapelets_platform.egg-info/PKG-INFO` & `shapelets-platform-2.0.99/src/shapelets_platform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapelets-platform
-Version: 2.0.98
+Version: 2.0.99
 Summary: Data Scientist platform
 Home-page: https://shapelets.io
 Author: Shapelets Dev Team
 Author-email: info@shapelets.io
 Maintainer: Shapelets Dev Team
 Maintainer-email: info@shapelets.io
 Project-URL: Homepage, https://shapelets.io/
```

### Comparing `shapelets-platform-2.0.98/src/shapelets_platform.egg-info/SOURCES.txt` & `shapelets-platform-2.0.99/src/shapelets_platform.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -184,21 +184,21 @@
 src/shapelets/svr/www/dataapp.json
 src/shapelets/svr/www/favicon.ico
 src/shapelets/svr/www/index.html
 src/shapelets/svr/www/manifest.json
 src/shapelets/svr/www/robots.txt
 src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css
 src/shapelets/svr/www/static/css/main.6638be9e.chunk.css
-src/shapelets/svr/www/static/js/2.379683b2.chunk.js
-src/shapelets/svr/www/static/js/2.379683b2.chunk.js.LICENSE.txt
+src/shapelets/svr/www/static/js/2.20645982.chunk.js
+src/shapelets/svr/www/static/js/2.20645982.chunk.js.LICENSE.txt
 src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js
 src/shapelets/svr/www/static/js/3.43e88e5e.chunk.js.LICENSE.txt
 src/shapelets/svr/www/static/js/4.153f1d29.chunk.js
 src/shapelets/svr/www/static/js/4.153f1d29.chunk.js.LICENSE.txt
-src/shapelets/svr/www/static/js/main.a03762f7.chunk.js
+src/shapelets/svr/www/static/js/main.613e103b.chunk.js
 src/shapelets/svr/www/static/js/runtime-main.197d60a0.js
 src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg
 src/shapelets/svr/www/static/media/audit.cb539a06.svg
 src/shapelets/svr/www/static/media/bin.7e762965.svg
 src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg
 src/shapelets/svr/www/static/media/clear.27b15301.svg
 src/shapelets/svr/www/static/media/collections.06fdf54a.svg
```

### Comparing `shapelets-platform-2.0.98/src/shapelets_platform.egg-info/requires.txt` & `shapelets-platform-2.0.99/src/shapelets_platform.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 pandas~=2.0
 psutil~=5.9
 pyarrow~=12.0
 py-cpuinfo~=9.0
 pydantic~=1.10
 PyNaCl~=1.5
 requests~=2.31
-shapelets_native==2.0.98
+shapelets_native==2.0.99
 tabulate~=0.9
 tomlkit~=0.12
 typing_extensions~=4.7
 uvicorn~=0.23
 websocket-client~=1.5
 websockets~=10.3
```

