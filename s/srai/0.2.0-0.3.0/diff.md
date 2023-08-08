# Comparing `tmp/srai-0.2.0.tar.gz` & `tmp/srai-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srai-0.2.0.tar", last modified: Wed Jul  5 10:29:09 2023, max compression
+gzip compressed data, was "srai-0.3.0.tar", last modified: Tue Aug  8 00:01:05 2023, max compression
```

## Comparing `srai-0.2.0.tar` & `srai-0.3.0.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0    10760 2023-07-05 10:28:47.765951 srai-0.2.0/LICENSE.md
--rw-r--r--   0        0        0    16727 2023-07-05 10:28:47.765951 srai-0.2.0/README.md
--rw-r--r--   0        0        0     4627 2023-07-05 10:29:09.566147 srai-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      404 2023-07-05 10:28:47.777951 srai-0.2.0/srai/__init__.py
--rw-r--r--   0        0        0      155 2023-07-05 10:28:47.777951 srai-0.2.0/srai/constants.py
--rw-r--r--   0        0        0      798 2023-07-05 10:28:47.777951 srai-0.2.0/srai/embedders/__init__.py
--rw-r--r--   0        0        0     4848 2023-07-05 10:28:47.777951 srai-0.2.0/srai/embedders/_base.py
--rw-r--r--   0        0        0     8327 2023-07-05 10:28:47.777951 srai-0.2.0/srai/embedders/contextual_count_embedder.py
--rw-r--r--   0        0        0     4857 2023-07-05 10:28:47.777951 srai-0.2.0/srai/embedders/count_embedder.py
--rw-r--r--   0        0        0      136 2023-07-05 10:28:47.777951 srai-0.2.0/srai/embedders/gtfs2vec/__init__.py
--rw-r--r--   0        0        0    11278 2023-07-05 10:28:47.777951 srai-0.2.0/srai/embedders/gtfs2vec/embedder.py
--rw-r--r--   0        0        0     2283 2023-07-05 10:28:47.777951 srai-0.2.0/srai/embedders/gtfs2vec/model.py
--rw-r--r--   0        0        0      247 2023-07-05 10:28:47.781951 srai-0.2.0/srai/embedders/hex2vec/__init__.py
--rw-r--r--   0        0        0    10683 2023-07-05 10:28:47.781951 srai-0.2.0/srai/embedders/hex2vec/embedder.py
--rw-r--r--   0        0        0     6822 2023-07-05 10:28:47.781951 srai-0.2.0/srai/embedders/hex2vec/model.py
--rw-r--r--   0        0        0     6319 2023-07-05 10:28:47.781951 srai-0.2.0/srai/embedders/hex2vec/neighbour_dataset.py
--rw-r--r--   0        0        0      153 2023-07-05 10:28:47.781951 srai-0.2.0/srai/embedders/highway2vec/__init__.py
--rw-r--r--   0        0        0     7935 2023-07-05 10:28:47.781951 srai-0.2.0/srai/embedders/highway2vec/embedder.py
--rw-r--r--   0        0        0     2860 2023-07-05 10:28:47.781951 srai-0.2.0/srai/embedders/highway2vec/model.py
--rw-r--r--   0        0        0      580 2023-07-05 10:28:47.781951 srai-0.2.0/srai/exceptions.py
--rw-r--r--   0        0        0      531 2023-07-05 10:28:47.781951 srai-0.2.0/srai/joiners/__init__.py
--rw-r--r--   0        0        0      731 2023-07-05 10:28:47.781951 srai-0.2.0/srai/joiners/_base.py
--rw-r--r--   0        0        0     3836 2023-07-05 10:28:47.781951 srai-0.2.0/srai/joiners/intersection_joiner.py
--rw-r--r--   0        0        0      725 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/__init__.py
--rw-r--r--   0        0        0      591 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/_base.py
--rw-r--r--   0        0        0     2195 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/geoparquet_loader.py
--rw-r--r--   0        0        0     5371 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/gtfs_loader.py
--rw-r--r--   0        0        0      257 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/__init__.py
--rw-r--r--   0        0        0     6424 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/_base.py
--rw-r--r--   0        0        0      469 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/filters/__init__.py
--rw-r--r--   0        0        0     2011 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/filters/_typing.py
--rw-r--r--   0        0        0     5324 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/filters/base_osm_groups.py
--rw-r--r--   0        0        0     8849 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/filters/geofabrik.py
--rw-r--r--   0        0        0    15758 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/filters/hex2vec.py
--rw-r--r--   0        0        0     2438 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/filters/popular.py
--rw-r--r--   0        0        0     5536 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/osm_online_loader.py
--rw-r--r--   0        0        0     5772 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/osm_pbf_loader.py
--rw-r--r--   0        0        0     2777 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/osm_tile_data_collector.py
--rw-r--r--   0        0        0     4703 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/osm_tile_loader.py
--rw-r--r--   0        0        0    10106 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/pbf_file_downloader.py
--rw-r--r--   0        0        0    11124 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_loaders/pbf_file_handler.py
--rw-r--r--   0        0        0      118 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_way_loader/__init__.py
--rw-r--r--   0        0        0     7587 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_way_loader/constants.py
--rw-r--r--   0        0        0    13854 2023-07-05 10:28:47.781951 srai-0.2.0/srai/loaders/osm_way_loader/osm_way_loader.py
--rw-r--r--   0        0        0      467 2023-07-05 10:28:47.781951 srai-0.2.0/srai/neighbourhoods/__init__.py
--rw-r--r--   0        0        0     3679 2023-07-05 10:28:47.781951 srai-0.2.0/srai/neighbourhoods/_base.py
--rw-r--r--   0        0        0     2887 2023-07-05 10:28:47.781951 srai-0.2.0/srai/neighbourhoods/adjacency_neighbourhood.py
--rw-r--r--   0        0        0     3221 2023-07-05 10:28:47.781951 srai-0.2.0/srai/neighbourhoods/h3_neighbourhood.py
--rw-r--r--   0        0        0      496 2023-07-05 10:28:47.781951 srai-0.2.0/srai/plotting/__init__.py
--rw-r--r--   0        0        0    11189 2023-07-05 10:28:47.781951 srai-0.2.0/srai/plotting/folium_wrapper.py
--rw-r--r--   0        0        0    14174 2023-07-05 10:28:47.781951 srai-0.2.0/srai/plotting/plotly_wrapper.py
--rw-r--r--   0        0        0      934 2023-07-05 10:28:47.781951 srai-0.2.0/srai/regionalizers/__init__.py
--rw-r--r--   0        0        0      957 2023-07-05 10:28:47.781951 srai-0.2.0/srai/regionalizers/_base.py
--rw-r--r--   0        0        0    11462 2023-07-05 10:28:47.781951 srai-0.2.0/srai/regionalizers/_spherical_voronoi.py
--rw-r--r--   0        0        0    15475 2023-07-05 10:28:47.781951 srai-0.2.0/srai/regionalizers/administrative_boundary_regionalizer.py
--rw-r--r--   0        0        0     6651 2023-07-05 10:28:47.781951 srai-0.2.0/srai/regionalizers/h3_regionalizer.py
--rw-r--r--   0        0        0     3142 2023-07-05 10:28:47.781951 srai-0.2.0/srai/regionalizers/s2_regionalizer.py
--rw-r--r--   0        0        0     4163 2023-07-05 10:28:47.781951 srai-0.2.0/srai/regionalizers/slippy_map_regionalizer.py
--rw-r--r--   0        0        0     5940 2023-07-05 10:28:47.781951 srai-0.2.0/srai/regionalizers/voronoi_regionalizer.py
--rw-r--r--   0        0        0      654 2023-07-05 10:28:47.781951 srai-0.2.0/srai/utils/__init__.py
--rw-r--r--   0        0        0     2910 2023-07-05 10:28:47.781951 srai-0.2.0/srai/utils/_optional.py
--rw-r--r--   0        0        0      239 2023-07-05 10:28:47.781951 srai-0.2.0/srai/utils/_pytorch_stubs.py
--rw-r--r--   0        0        0      999 2023-07-05 10:28:47.781951 srai-0.2.0/srai/utils/download.py
--rw-r--r--   0        0        0      944 2023-07-05 10:28:47.781951 srai-0.2.0/srai/utils/geocode.py
--rw-r--r--   0        0        0     2521 2023-07-05 10:28:47.781951 srai-0.2.0/srai/utils/geometry.py
--rw-r--r--   0        0        0     1153 2023-07-05 10:28:47.781951 srai-0.2.0/srai/utils/merge.py
--rw-r--r--   0        0        0      717 2023-07-05 10:28:47.781951 srai-0.2.0/srai/utils/typing.py
--rw-r--r--   0        0        0       29 2023-07-05 10:28:47.781951 srai-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     7806 2023-07-05 10:28:47.781951 srai-0.2.0/tests/embedders/conftest.py
--rw-r--r--   0        0        0      534 2023-07-05 10:28:47.781951 srai-0.2.0/tests/embedders/hex2vec/constants.py
--rw-r--r--   0        0        0     2600 2023-07-05 10:28:47.781951 srai-0.2.0/tests/embedders/hex2vec/generation.py
--rw-r--r--   0        0        0     2716 2023-07-05 10:28:47.781951 srai-0.2.0/tests/embedders/hex2vec/test_embedder.py
--rw-r--r--   0        0        0    97383 2023-07-05 10:28:47.781951 srai-0.2.0/tests/embedders/hex2vec/test_files/poz_8_features.parquet
--rw-r--r--   0        0        0   111218 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
--rw-r--r--   0        0        0    14226 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
--rw-r--r--   0        0        0    14498 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_files/poz_8_result.parquet
--rw-r--r--   0        0        0    89227 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_files/wro_9_features.parquet
--rw-r--r--   0        0        0    86944 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
--rw-r--r--   0        0        0    16794 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
--rw-r--r--   0        0        0    15781 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_files/wro_9_result.parquet
--rw-r--r--   0        0        0     1061 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_model.py
--rw-r--r--   0        0        0     3037 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/hex2vec/test_neighbour_dataset.py
--rw-r--r--   0        0        0    24053 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/test_contextual_count_embedder.py
--rw-r--r--   0        0        0     8273 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/test_count_embedder.py
--rw-r--r--   0        0        0     7091 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/test_gtfs2vec_embedder.py
--rw-r--r--   0        0        0     3630 2023-07-05 10:28:47.785951 srai-0.2.0/tests/embedders/test_highway2vec_embedder.py
--rw-r--r--   0        0        0     1765 2023-07-05 10:28:47.785951 srai-0.2.0/tests/joiners/conftest.py
--rw-r--r--   0        0        0     2529 2023-07-05 10:28:47.785951 srai-0.2.0/tests/joiners/test_intersection_joiner.py
--rw-r--r--   0        0        0     3001 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/conftest.py
--rw-r--r--   0        0        0     4284 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/conftest.py
--rw-r--r--   0        0        0     4824 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/filters/popular_filter_example.json
--rw-r--r--   0        0        0     3413 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
--rw-r--r--   0        0        0     3276 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
--rw-r--r--   0        0        0      342 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
--rw-r--r--   0        0        0      100 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
--rw-r--r--   0        0        0      770 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
--rw-r--r--   0        0        0    73746 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
--rw-r--r--   0        0        0     1013 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
--rw-r--r--   0        0        0   111539 2023-07-05 10:28:47.785951 srai-0.2.0/tests/loaders/osm_loaders/test_files/poland.geojson
--rw-r--r--   0        0        0   252620 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
--rw-r--r--   0        0        0     2811 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_loaders/test_osm_online_loader.py
--rw-r--r--   0        0        0     8690 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_loaders/test_osm_pbf_loader.py
--rw-r--r--   0        0        0     3156 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
--rw-r--r--   0        0        0     3165 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_loaders/test_osm_tile_loader.py
--rw-r--r--   0        0        0     3353 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_way_loader/files/1f0fafc11b7ab7aea5124d2a89c634fc.pkl
--rw-r--r--   0        0        0     2804 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_way_loader/files/20c9119c4dcc233c37382696f483239e.pkl
--rw-r--r--   0        0        0     3822 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_way_loader/files/4310fe8d3c435f2a83fac55fc79f9166.pkl
--rw-r--r--   0        0        0     5109 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_way_loader/files/7be5387a594790ea98ef0bd07bfcb58e.pkl
--rw-r--r--   0        0        0     3822 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_way_loader/files/97e1befc51831ce8f8f482077f5042f2.pkl
--rw-r--r--   0        0        0      629 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_way_loader/files/eebaa127015feec3e21491d4c32e4efe.pkl
--rw-r--r--   0        0        0    10789 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/osm_way_loader/test_osm_way_loader.py
--rw-r--r--   0        0        0    27801 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/test_files/example.parquet
--rw-r--r--   0        0        0     2181 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/test_geoparquet_loader.py
--rw-r--r--   0        0        0     3176 2023-07-05 10:28:47.789951 srai-0.2.0/tests/loaders/test_gtfs_loader.py
--rw-r--r--   0        0        0     4755 2023-07-05 10:28:47.789951 srai-0.2.0/tests/miscellaneous/test_optional_dependencies.py
--rw-r--r--   0        0        0     4028 2023-07-05 10:28:47.789951 srai-0.2.0/tests/neighbourhoods/h3/test_no_regions.py
--rw-r--r--   0        0        0     5668 2023-07-05 10:28:47.789951 srai-0.2.0/tests/neighbourhoods/h3/test_with_regions.py
--rw-r--r--   0        0        0     8063 2023-07-05 10:28:47.789951 srai-0.2.0/tests/neighbourhoods/test_adjacency_neighbourhood.py
--rw-r--r--   0        0        0     5586 2023-07-05 10:28:47.789951 srai-0.2.0/tests/neighbourhoods/test_neighbourhood.py
--rw-r--r--   0        0        0     3667 2023-07-05 10:28:47.789951 srai-0.2.0/tests/regionalizers/conftest.py
--rw-r--r--   0        0        0     6505 2023-07-05 10:28:47.789951 srai-0.2.0/tests/regionalizers/test_administrative_boundary_regionalizer.py
--rw-r--r--   0        0        0     2208 2023-07-05 10:28:47.789951 srai-0.2.0/tests/regionalizers/test_h3_regionalizer.py
--rw-r--r--   0        0        0     1841 2023-07-05 10:28:47.789951 srai-0.2.0/tests/regionalizers/test_s2_regionalizer.py
--rw-r--r--   0        0        0     2689 2023-07-05 10:28:47.789951 srai-0.2.0/tests/regionalizers/test_slippy_map_regionalizer.py
--rw-r--r--   0        0        0     4983 2023-07-05 10:28:47.789951 srai-0.2.0/tests/regionalizers/test_voronoi_regionalizer.py
--rw-r--r--   0        0        0    18930 1970-01-01 00:00:00.000000 srai-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10760 2023-08-07 23:59:29.812539 srai-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0    16648 2023-08-07 23:59:29.812539 srai-0.3.0/README.md
+-rw-r--r--   0        0        0     4814 2023-08-08 00:01:05.409001 srai-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      427 2023-08-07 23:59:29.828540 srai-0.3.0/srai/__init__.py
+-rw-r--r--   0        0        0     2910 2023-08-07 23:59:29.828540 srai-0.3.0/srai/_optional.py
+-rw-r--r--   0        0        0      717 2023-08-07 23:59:29.828540 srai-0.3.0/srai/_typing.py
+-rw-r--r--   0        0        0      155 2023-08-07 23:59:29.828540 srai-0.3.0/srai/constants.py
+-rw-r--r--   0        0        0      798 2023-08-07 23:59:29.828540 srai-0.3.0/srai/embedders/__init__.py
+-rw-r--r--   0        0        0     4852 2023-08-07 23:59:29.828540 srai-0.3.0/srai/embedders/_base.py
+-rw-r--r--   0        0        0      239 2023-08-07 23:59:29.828540 srai-0.3.0/srai/embedders/_pytorch_stubs.py
+-rw-r--r--   0        0        0     8327 2023-08-07 23:59:29.828540 srai-0.3.0/srai/embedders/contextual_count_embedder.py
+-rw-r--r--   0        0        0     4857 2023-08-07 23:59:29.828540 srai-0.3.0/srai/embedders/count_embedder.py
+-rw-r--r--   0        0        0      136 2023-08-07 23:59:29.828540 srai-0.3.0/srai/embedders/gtfs2vec/__init__.py
+-rw-r--r--   0        0        0    11272 2023-08-07 23:59:29.828540 srai-0.3.0/srai/embedders/gtfs2vec/embedder.py
+-rw-r--r--   0        0        0     2277 2023-08-07 23:59:29.828540 srai-0.3.0/srai/embedders/gtfs2vec/model.py
+-rw-r--r--   0        0        0      247 2023-08-07 23:59:29.828540 srai-0.3.0/srai/embedders/hex2vec/__init__.py
+-rw-r--r--   0        0        0    10697 2023-08-07 23:59:29.828540 srai-0.3.0/srai/embedders/hex2vec/embedder.py
+-rw-r--r--   0        0        0     6816 2023-08-07 23:59:29.828540 srai-0.3.0/srai/embedders/hex2vec/model.py
+-rw-r--r--   0        0        0     6317 2023-08-07 23:59:29.828540 srai-0.3.0/srai/embedders/hex2vec/neighbour_dataset.py
+-rw-r--r--   0        0        0      153 2023-08-07 23:59:29.828540 srai-0.3.0/srai/embedders/highway2vec/__init__.py
+-rw-r--r--   0        0        0     7929 2023-08-07 23:59:29.828540 srai-0.3.0/srai/embedders/highway2vec/embedder.py
+-rw-r--r--   0        0        0     2854 2023-08-07 23:59:29.828540 srai-0.3.0/srai/embedders/highway2vec/model.py
+-rw-r--r--   0        0        0      580 2023-08-07 23:59:29.828540 srai-0.3.0/srai/exceptions.py
+-rw-r--r--   0        0        0     3538 2023-08-07 23:59:29.828540 srai-0.3.0/srai/geometry.py
+-rw-r--r--   0        0        0     8145 2023-08-07 23:59:29.828540 srai-0.3.0/srai/h3.py
+-rw-r--r--   0        0        0      531 2023-08-07 23:59:29.828540 srai-0.3.0/srai/joiners/__init__.py
+-rw-r--r--   0        0        0      731 2023-08-07 23:59:29.828540 srai-0.3.0/srai/joiners/_base.py
+-rw-r--r--   0        0        0     3836 2023-08-07 23:59:29.828540 srai-0.3.0/srai/joiners/intersection_joiner.py
+-rw-r--r--   0        0        0      820 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/__init__.py
+-rw-r--r--   0        0        0      591 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/_base.py
+-rw-r--r--   0        0        0      999 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/download.py
+-rw-r--r--   0        0        0     2195 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/geoparquet_loader.py
+-rw-r--r--   0        0        0     5365 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/gtfs_loader.py
+-rw-r--r--   0        0        0      257 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_loaders/__init__.py
+-rw-r--r--   0        0        0     6394 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_loaders/_base.py
+-rw-r--r--   0        0        0      471 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_loaders/filters/__init__.py
+-rw-r--r--   0        0        0     1978 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_loaders/filters/_typing.py
+-rw-r--r--   0        0        0     5314 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_loaders/filters/base_osm_groups.py
+-rw-r--r--   0        0        0     8839 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_loaders/filters/geofabrik.py
+-rw-r--r--   0        0        0    15750 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_loaders/filters/hex2vec.py
+-rw-r--r--   0        0        0     2430 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_loaders/filters/popular.py
+-rw-r--r--   0        0        0     5506 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_loaders/osm_online_loader.py
+-rw-r--r--   0        0        0     5742 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_loaders/osm_pbf_loader.py
+-rw-r--r--   0        0        0     2777 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_loaders/osm_tile_data_collector.py
+-rw-r--r--   0        0        0     4697 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_loaders/osm_tile_loader.py
+-rw-r--r--   0        0        0    10309 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_loaders/pbf_file_downloader.py
+-rw-r--r--   0        0        0    11116 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_loaders/pbf_file_handler.py
+-rw-r--r--   0        0        0      124 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_way_loader/__init__.py
+-rw-r--r--   0        0        0     7587 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_way_loader/constants.py
+-rw-r--r--   0        0        0    13854 2023-08-07 23:59:29.832540 srai-0.3.0/srai/loaders/osm_way_loader/osm_way_loader.py
+-rw-r--r--   0        0        0      467 2023-08-07 23:59:29.832540 srai-0.3.0/srai/neighbourhoods/__init__.py
+-rw-r--r--   0        0        0     6089 2023-08-07 23:59:29.832540 srai-0.3.0/srai/neighbourhoods/_base.py
+-rw-r--r--   0        0        0     3592 2023-08-07 23:59:29.832540 srai-0.3.0/srai/neighbourhoods/adjacency_neighbourhood.py
+-rw-r--r--   0        0        0     4417 2023-08-07 23:59:29.832540 srai-0.3.0/srai/neighbourhoods/h3_neighbourhood.py
+-rw-r--r--   0        0        0      496 2023-08-07 23:59:29.832540 srai-0.3.0/srai/plotting/__init__.py
+-rw-r--r--   0        0        0    11161 2023-08-07 23:59:29.832540 srai-0.3.0/srai/plotting/folium_wrapper.py
+-rw-r--r--   0        0        0    14145 2023-08-07 23:59:29.832540 srai-0.3.0/srai/plotting/plotly_wrapper.py
+-rw-r--r--   0        0        0     1006 2023-08-07 23:59:29.832540 srai-0.3.0/srai/regionalizers/__init__.py
+-rw-r--r--   0        0        0      957 2023-08-07 23:59:29.832540 srai-0.3.0/srai/regionalizers/_base.py
+-rw-r--r--   0        0        0    15027 2023-08-07 23:59:29.832540 srai-0.3.0/srai/regionalizers/_spherical_voronoi.py
+-rw-r--r--   0        0        0    15405 2023-08-07 23:59:29.832540 srai-0.3.0/srai/regionalizers/administrative_boundary_regionalizer.py
+-rw-r--r--   0        0        0      944 2023-08-07 23:59:29.832540 srai-0.3.0/srai/regionalizers/geocode.py
+-rw-r--r--   0        0        0     2611 2023-08-07 23:59:29.832540 srai-0.3.0/srai/regionalizers/h3_regionalizer.py
+-rw-r--r--   0        0        0     3142 2023-08-07 23:59:29.832540 srai-0.3.0/srai/regionalizers/s2_regionalizer.py
+-rw-r--r--   0        0        0     4163 2023-08-07 23:59:29.832540 srai-0.3.0/srai/regionalizers/slippy_map_regionalizer.py
+-rw-r--r--   0        0        0     6386 2023-08-07 23:59:29.832540 srai-0.3.0/srai/regionalizers/voronoi_regionalizer.py
+-rw-r--r--   0        0        0       29 2023-08-07 23:59:29.832540 srai-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     7806 2023-08-07 23:59:29.832540 srai-0.3.0/tests/embedders/conftest.py
+-rw-r--r--   0        0        0      534 2023-08-07 23:59:29.832540 srai-0.3.0/tests/embedders/hex2vec/constants.py
+-rw-r--r--   0        0        0     2597 2023-08-07 23:59:29.832540 srai-0.3.0/tests/embedders/hex2vec/generation.py
+-rw-r--r--   0        0        0     2716 2023-08-07 23:59:29.832540 srai-0.3.0/tests/embedders/hex2vec/test_embedder.py
+-rw-r--r--   0        0        0    97383 2023-08-07 23:59:29.832540 srai-0.3.0/tests/embedders/hex2vec/test_files/poz_8_features.parquet
+-rw-r--r--   0        0        0   111218 2023-08-07 23:59:29.836540 srai-0.3.0/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
+-rw-r--r--   0        0        0    14226 2023-08-07 23:59:29.836540 srai-0.3.0/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
+-rw-r--r--   0        0        0    14498 2023-08-07 23:59:29.836540 srai-0.3.0/tests/embedders/hex2vec/test_files/poz_8_result.parquet
+-rw-r--r--   0        0        0    89227 2023-08-07 23:59:29.836540 srai-0.3.0/tests/embedders/hex2vec/test_files/wro_9_features.parquet
+-rw-r--r--   0        0        0    86944 2023-08-07 23:59:29.836540 srai-0.3.0/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
+-rw-r--r--   0        0        0    16794 2023-08-07 23:59:29.836540 srai-0.3.0/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
+-rw-r--r--   0        0        0    15781 2023-08-07 23:59:29.836540 srai-0.3.0/tests/embedders/hex2vec/test_files/wro_9_result.parquet
+-rw-r--r--   0        0        0     1061 2023-08-07 23:59:29.836540 srai-0.3.0/tests/embedders/hex2vec/test_model.py
+-rw-r--r--   0        0        0     3037 2023-08-07 23:59:29.836540 srai-0.3.0/tests/embedders/hex2vec/test_neighbour_dataset.py
+-rw-r--r--   0        0        0    24053 2023-08-07 23:59:29.836540 srai-0.3.0/tests/embedders/test_contextual_count_embedder.py
+-rw-r--r--   0        0        0     8273 2023-08-07 23:59:29.836540 srai-0.3.0/tests/embedders/test_count_embedder.py
+-rw-r--r--   0        0        0     7091 2023-08-07 23:59:29.836540 srai-0.3.0/tests/embedders/test_gtfs2vec_embedder.py
+-rw-r--r--   0        0        0     3630 2023-08-07 23:59:29.836540 srai-0.3.0/tests/embedders/test_highway2vec_embedder.py
+-rw-r--r--   0        0        0     2862 2023-08-07 23:59:29.836540 srai-0.3.0/tests/h3/conftest.py
+-rw-r--r--   0        0        0     3060 2023-08-07 23:59:29.836540 srai-0.3.0/tests/h3/test_ij_coordinates.py
+-rw-r--r--   0        0        0     3072 2023-08-07 23:59:29.836540 srai-0.3.0/tests/h3/test_shapely_conversion.py
+-rw-r--r--   0        0        0     1765 2023-08-07 23:59:29.836540 srai-0.3.0/tests/joiners/conftest.py
+-rw-r--r--   0        0        0     2529 2023-08-07 23:59:29.836540 srai-0.3.0/tests/joiners/test_intersection_joiner.py
+-rw-r--r--   0        0        0     3001 2023-08-07 23:59:29.836540 srai-0.3.0/tests/loaders/conftest.py
+-rw-r--r--   0        0        0     4284 2023-08-07 23:59:29.836540 srai-0.3.0/tests/loaders/osm_loaders/conftest.py
+-rw-r--r--   0        0        0     4824 2023-08-07 23:59:29.836540 srai-0.3.0/tests/loaders/osm_loaders/filters/popular_filter_example.json
+-rw-r--r--   0        0        0     3396 2023-08-07 23:59:29.836540 srai-0.3.0/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
+-rw-r--r--   0        0        0     3276 2023-08-07 23:59:29.836540 srai-0.3.0/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
+-rw-r--r--   0        0        0      342 2023-08-07 23:59:29.836540 srai-0.3.0/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
+-rw-r--r--   0        0        0      100 2023-08-07 23:59:29.836540 srai-0.3.0/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
+-rw-r--r--   0        0        0      770 2023-08-07 23:59:29.836540 srai-0.3.0/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
+-rw-r--r--   0        0        0    73746 2023-08-07 23:59:29.836540 srai-0.3.0/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
+-rw-r--r--   0        0        0     1013 2023-08-07 23:59:29.836540 srai-0.3.0/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
+-rw-r--r--   0        0        0   111539 2023-08-07 23:59:29.840540 srai-0.3.0/tests/loaders/osm_loaders/test_files/poland.geojson
+-rw-r--r--   0        0        0   252620 2023-08-07 23:59:29.840540 srai-0.3.0/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
+-rw-r--r--   0        0        0     2803 2023-08-07 23:59:29.840540 srai-0.3.0/tests/loaders/osm_loaders/test_osm_online_loader.py
+-rw-r--r--   0        0        0     8657 2023-08-07 23:59:29.840540 srai-0.3.0/tests/loaders/osm_loaders/test_osm_pbf_loader.py
+-rw-r--r--   0        0        0     3156 2023-08-07 23:59:29.840540 srai-0.3.0/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
+-rw-r--r--   0        0        0     3165 2023-08-07 23:59:29.840540 srai-0.3.0/tests/loaders/osm_loaders/test_osm_tile_loader.py
+-rw-r--r--   0        0        0     3803 2023-08-07 23:59:29.840540 srai-0.3.0/tests/loaders/osm_way_loader/test_files/graph_1.pkl
+-rw-r--r--   0        0        0     3334 2023-08-07 23:59:29.840540 srai-0.3.0/tests/loaders/osm_way_loader/test_files/graph_2.pkl
+-rw-r--r--   0        0        0     5099 2023-08-07 23:59:29.840540 srai-0.3.0/tests/loaders/osm_way_loader/test_files/graph_3.pkl
+-rw-r--r--   0        0        0     3803 2023-08-07 23:59:29.840540 srai-0.3.0/tests/loaders/osm_way_loader/test_files/graph_4.pkl
+-rw-r--r--   0        0        0    10974 2023-08-07 23:59:29.840540 srai-0.3.0/tests/loaders/osm_way_loader/test_osm_way_loader.py
+-rw-r--r--   0        0        0    27801 2023-08-07 23:59:29.840540 srai-0.3.0/tests/loaders/test_files/example.parquet
+-rw-r--r--   0        0        0     2181 2023-08-07 23:59:29.840540 srai-0.3.0/tests/loaders/test_geoparquet_loader.py
+-rw-r--r--   0        0        0     3176 2023-08-07 23:59:29.840540 srai-0.3.0/tests/loaders/test_gtfs_loader.py
+-rw-r--r--   0        0        0     4766 2023-08-07 23:59:29.840540 srai-0.3.0/tests/miscellaneous/test_optional_dependencies.py
+-rw-r--r--   0        0        0     8363 2023-08-07 23:59:29.840540 srai-0.3.0/tests/neighbourhoods/h3/test_no_regions.py
+-rw-r--r--   0        0        0     9170 2023-08-07 23:59:29.840540 srai-0.3.0/tests/neighbourhoods/h3/test_with_regions.py
+-rw-r--r--   0        0        0    11432 2023-08-07 23:59:29.840540 srai-0.3.0/tests/neighbourhoods/test_adjacency_neighbourhood.py
+-rw-r--r--   0        0        0    11029 2023-08-07 23:59:29.840540 srai-0.3.0/tests/neighbourhoods/test_neighbourhood.py
+-rw-r--r--   0        0        0     3754 2023-08-07 23:59:29.840540 srai-0.3.0/tests/regionalizers/conftest.py
+-rw-r--r--   0        0        0     6508 2023-08-07 23:59:29.840540 srai-0.3.0/tests/regionalizers/test_administrative_boundary_regionalizer.py
+-rw-r--r--   0        0        0     2208 2023-08-07 23:59:29.840540 srai-0.3.0/tests/regionalizers/test_h3_regionalizer.py
+-rw-r--r--   0        0        0     1841 2023-08-07 23:59:29.840540 srai-0.3.0/tests/regionalizers/test_s2_regionalizer.py
+-rw-r--r--   0        0        0     2689 2023-08-07 23:59:29.840540 srai-0.3.0/tests/regionalizers/test_slippy_map_regionalizer.py
+-rw-r--r--   0        0        0     7704 2023-08-07 23:59:29.840540 srai-0.3.0/tests/regionalizers/test_voronoi_regionalizer.py
+-rw-r--r--   0        0        0    18899 1970-01-01 00:00:00.000000 srai-0.3.0/PKG-INFO
```

### Comparing `srai-0.2.0/LICENSE.md` & `srai-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/README.md` & `srai-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -93,16 +93,16 @@
 * `OSMOnlineLoader` - downloads data from OpenStreetMap API using [osmnx](https://github.com/gboeing/osmnx) - this is faster for smaller areas or tags counts
 * `OSMPbfLoader` - loads data from automatically downloaded PBF file from [protomaps](https://protomaps.com/) - this is faster for larger areas or tags counts
 
 Example with `OSMOnlineLoader`:
 
 ```python
 from srai.loaders import OSMOnlineLoader
-from srai.utils import geocode_to_region_gdf
 from srai.plotting import plot_regions
+from srai.regionalizers import geocode_to_region_gdf
 
 query = {"leisure": "park"}
 area = geocode_to_region_gdf("Wrocław, Poland")
 loader = OSMOnlineLoader()
 
 parks_gdf = loader.load(area, query)
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0)"], tiles_style="CartoDB positron")
@@ -114,21 +114,20 @@
 </p>
 
 ### Downloading road network
 
 Road network downloading is a special case of OSM data downloading. To download road network for a given area, use `OSMWayLoader` class:
 
 ```python
-from srai.loaders import OSMWayLoader
-from srai.loaders.osm_way_loader import NetworkType
-from srai.utils import geocode_to_region_gdf
+from srai.loaders import OSMNetworkType, OSMWayLoader
 from srai.plotting import plot_regions
+from srai.regionalizers import geocode_to_region_gdf
 
 area = geocode_to_region_gdf("Utrecht, Netherlands")
-loader = OSMWayLoader(NetworkType.BIKE)
+loader = OSMWayLoader(OSMNetworkType.BIKE)
 
 nodes, edges = loader.load(area)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
 edges[["geometry"]].explore(m=folium_map, color="seagreen")
 ```
 
@@ -139,17 +138,17 @@
 ### Downloading GTFS data
 
 To extract features from GTFS use `GTFSLoader`. It will extract trip count and available directions for each stop in 1h time windows.
 
 ```python
 from pathlib import Path
 
-from srai.loaders import GTFSLoader
-from srai.utils import geocode_to_region_gdf, download_file
+from srai.loaders import GTFSLoader, download_file
 from srai.plotting import plot_regions
+from srai.regionalizers import geocode_to_region_gdf
 
 area = geocode_to_region_gdf("Vienna, Austria")
 gtfs_file = Path("vienna_gtfs.zip")
 download_file("https://transitfeeds.com/p/stadt-wien/888/latest/download", gtfs_file.as_posix())
 loader = GTFSLoader()
 
 features = loader.load(gtfs_file)
@@ -170,16 +169,15 @@
 * `S2Regionalizer` - regionalization using [Google's S2 library](https://github.com/google/s2geometry)
 * `VoronoiRegionalizer` - regionalization using Voronoi diagram
 * `AdministativeBoundaryRegionalizer` - regionalization using administrative boundaries
 
 Example:
 
 ```python
-from srai.regionalizers import H3Regionalizer
-from srai.utils import geocode_to_region_gdf
+from srai.regionalizers import H3Regionalizer, geocode_to_region_gdf
 
 area = geocode_to_region_gdf("Berlin, Germany")
 regionalizer = H3Regionalizer(resolution=7)
 
 regions = regionalizer.transform(area)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
@@ -203,16 +201,15 @@
 All of those methods share the same API. All of them require results from `Loader` (load features), `Regionalizer` (split area into regions) and `Joiner` (join features to regions) to work. An example using `CountEmbedder`:
 
 ```python
 from srai.embedders import CountEmbedder
 from srai.joiners import IntersectionJoiner
 from srai.loaders import OSMOnlineLoader
 from srai.plotting import plot_regions, plot_numeric_data
-from srai.regionalizers import H3Regionalizer
-from srai.utils import geocode_to_region_gdf
+from srai.regionalizers import H3Regionalizer, geocode_to_region_gdf
 
 loader = OSMOnlineLoader()
 regionalizer = H3Regionalizer(resolution=9)
 joiner = IntersectionJoiner()
 
 query = {"amenity": "bicycle_parking"}
 area = geocode_to_region_gdf("Malmö, Sweden")
@@ -235,16 +232,15 @@
 
 ```python
 from srai.embedders import Hex2VecEmbedder
 from srai.joiners import IntersectionJoiner
 from srai.loaders import OSMPbfLoader
 from srai.loaders.osm_loaders.filters import HEX2VEC_FILTER
 from srai.neighbourhoods.h3_neighbourhood import H3Neighbourhood
-from srai.regionalizers import H3Regionalizer
-from srai.utils import geocode_to_region_gdf
+from srai.regionalizers import H3Regionalizer, geocode_to_region_gdf
 from srai.plotting import plot_regions, plot_numeric_data
 
 loader = OSMPbfLoader()
 regionalizer = H3Regionalizer(resolution=11)
 joiner = IntersectionJoiner()
 
 area = geocode_to_region_gdf("City of London")
```

#### html2text {}

```diff
@@ -53,103 +53,103 @@
 17z2OYZG82FZNRK86Kt-eSgbJn9m7meSH?usp=sharing) ### Downloading OSM data To
 download OSM data for a given area, using a set of tags use one of `OSMLoader`
 classes: * `OSMOnlineLoader` - downloads data from OpenStreetMap API using
 [osmnx](https://github.com/gboeing/osmnx) - this is faster for smaller areas or
 tags counts * `OSMPbfLoader` - loads data from automatically downloaded PBF
 file from [protomaps](https://protomaps.com/) - this is faster for larger areas
 or tags counts Example with `OSMOnlineLoader`: ```python from srai.loaders
-import OSMOnlineLoader from srai.utils import geocode_to_region_gdf from
-srai.plotting import plot_regions query = {"leisure": "park"} area =
-geocode_to_region_gdf("WrocÅaw, Poland") loader = OSMOnlineLoader() parks_gdf
-= loader.load(area, query) folium_map = plot_regions(area, colormap=["rgba
-(0,0,0,0)"], tiles_style="CartoDB positron") parks_gdf.explore(m=folium_map,
-color="forestgreen") ```
+import OSMOnlineLoader from srai.plotting import plot_regions from
+srai.regionalizers import geocode_to_region_gdf query = {"leisure": "park"}
+area = geocode_to_region_gdf("WrocÅaw, Poland") loader = OSMOnlineLoader()
+parks_gdf = loader.load(area, query) folium_map = plot_regions(area, colormap=
+["rgba(0,0,0,0)"], tiles_style="CartoDB positron") parks_gdf.explore
+(m=folium_map, color="forestgreen") ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                            downloading_osm_data.jpg]
 ### Downloading road network Road network downloading is a special case of OSM
 data downloading. To download road network for a given area, use `OSMWayLoader`
-class: ```python from srai.loaders import OSMWayLoader from
-srai.loaders.osm_way_loader import NetworkType from srai.utils import
-geocode_to_region_gdf from srai.plotting import plot_regions area =
-geocode_to_region_gdf("Utrecht, Netherlands") loader = OSMWayLoader
-(NetworkType.BIKE) nodes, edges = loader.load(area) folium_map = plot_regions
-(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron") edges[
-["geometry"]].explore(m=folium_map, color="seagreen") ```
+class: ```python from srai.loaders import OSMNetworkType, OSMWayLoader from
+srai.plotting import plot_regions from srai.regionalizers import
+geocode_to_region_gdf area = geocode_to_region_gdf("Utrecht, Netherlands")
+loader = OSMWayLoader(OSMNetworkType.BIKE) nodes, edges = loader.load(area)
+folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"],
+tiles_style="CartoDB positron") edges[["geometry"]].explore(m=folium_map,
+color="seagreen") ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                       downloading_road_network_data.jpg]
 ### Downloading GTFS data To extract features from GTFS use `GTFSLoader`. It
 will extract trip count and available directions for each stop in 1h time
-windows. ```python from pathlib import Path from srai.loaders import GTFSLoader
-from srai.utils import geocode_to_region_gdf, download_file from srai.plotting
-import plot_regions area = geocode_to_region_gdf("Vienna, Austria") gtfs_file =
-Path("vienna_gtfs.zip") download_file("https://transitfeeds.com/p/stadt-wien/
-888/latest/download", gtfs_file.as_posix()) loader = GTFSLoader() features =
-loader.load(gtfs_file) folium_map = plot_regions(area, colormap=["rgba
-(0,0,0,0.1)"], tiles_style="CartoDB positron") features[["trips_at_8",
-"geometry"]].explore("trips_at_8", m=folium_map) ```
+windows. ```python from pathlib import Path from srai.loaders import
+GTFSLoader, download_file from srai.plotting import plot_regions from
+srai.regionalizers import geocode_to_region_gdf area = geocode_to_region_gdf
+("Vienna, Austria") gtfs_file = Path("vienna_gtfs.zip") download_file("https://
+transitfeeds.com/p/stadt-wien/888/latest/download", gtfs_file.as_posix())
+loader = GTFSLoader() features = loader.load(gtfs_file) folium_map =
+plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB
+positron") features[["trips_at_8", "geometry"]].explore("trips_at_8",
+m=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                           downloading_gtfs_data.jpg]
 ### Regionalization Regionalization is a process of dividing a given area into
 smaller regions. This can be done in a variety of ways: * `H3Regionalizer` -
 regionalization using [Uber's H3 library](https://github.com/uber/h3) *
 `S2Regionalizer` - regionalization using [Google's S2 library](https://
 github.com/google/s2geometry) * `VoronoiRegionalizer` - regionalization using
 Voronoi diagram * `AdministativeBoundaryRegionalizer` - regionalization using
 administrative boundaries Example: ```python from srai.regionalizers import
-H3Regionalizer from srai.utils import geocode_to_region_gdf area =
-geocode_to_region_gdf("Berlin, Germany") regionalizer = H3Regionalizer
-(resolution=7) regions = regionalizer.transform(area) folium_map = plot_regions
-(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
-plot_regions(regions_gdf=regions, map=folium_map) ```
+H3Regionalizer, geocode_to_region_gdf area = geocode_to_region_gdf("Berlin,
+Germany") regionalizer = H3Regionalizer(resolution=7) regions =
+regionalizer.transform(area) folium_map = plot_regions(area, colormap=["rgba
+(0,0,0,0.1)"], tiles_style="CartoDB positron") plot_regions
+(regions_gdf=regions, map=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                              regionalization.jpg]
 ### Embedding Embedding is a process of mapping regions into a vector space.
 This can be done in a variety of ways: * `Hex2VecEmbedder` - embedding using
 hex2vec[1] algorithm * `GTFS2VecEmbedder` - embedding using GTFS2Vec[2]
 algorithm * `CountEmbedder` - embedding based on features counts *
 `ContextualCountEmbedder` - embedding based on features counts with
 neighbourhood context (proposed in [3]) * `Highway2VecEmbedder` - embedding
 using Highway2Vec[4] algorithm All of those methods share the same API. All of
 them require results from `Loader` (load features), `Regionalizer` (split area
 into regions) and `Joiner` (join features to regions) to work. An example using
 `CountEmbedder`: ```python from srai.embedders import CountEmbedder from
 srai.joiners import IntersectionJoiner from srai.loaders import OSMOnlineLoader
 from srai.plotting import plot_regions, plot_numeric_data from
-srai.regionalizers import H3Regionalizer from srai.utils import
-geocode_to_region_gdf loader = OSMOnlineLoader() regionalizer = H3Regionalizer
-(resolution=9) joiner = IntersectionJoiner() query = {"amenity":
-"bicycle_parking"} area = geocode_to_region_gdf("MalmÃ¶, Sweden") features =
-loader.load(area, query) regions = regionalizer.transform(area) joint =
-joiner.transform(regions, features) embedder = CountEmbedder() embeddings =
-embedder.transform(regions, features, joint) folium_map = plot_regions(area,
-colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron") plot_numeric_data
-(regions, embeddings, "amenity_bicycle_parking", map=folium_map) ```
+srai.regionalizers import H3Regionalizer, geocode_to_region_gdf loader =
+OSMOnlineLoader() regionalizer = H3Regionalizer(resolution=9) joiner =
+IntersectionJoiner() query = {"amenity": "bicycle_parking"} area =
+geocode_to_region_gdf("MalmÃ¶, Sweden") features = loader.load(area, query)
+regions = regionalizer.transform(area) joint = joiner.transform(regions,
+features) embedder = CountEmbedder() embeddings = embedder.transform(regions,
+features, joint) folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"],
+tiles_style="CartoDB positron") plot_numeric_data(regions, embeddings,
+"amenity_bicycle_parking", map=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                          embedding_count_embedder.jpg]
 `CountEmbedder` is a simple method, which does not require fitting. Other
 methods, such as `Hex2VecEmbedder` or `GTFS2VecEmbedder` require fitting and
 can be used in a similar way to `scikit-learn` estimators: ```python from
 srai.embedders import Hex2VecEmbedder from srai.joiners import
 IntersectionJoiner from srai.loaders import OSMPbfLoader from
 srai.loaders.osm_loaders.filters import HEX2VEC_FILTER from
 srai.neighbourhoods.h3_neighbourhood import H3Neighbourhood from
-srai.regionalizers import H3Regionalizer from srai.utils import
-geocode_to_region_gdf from srai.plotting import plot_regions, plot_numeric_data
-loader = OSMPbfLoader() regionalizer = H3Regionalizer(resolution=11) joiner =
-IntersectionJoiner() area = geocode_to_region_gdf("City of London") features =
-loader.load(area, HEX2VEC_FILTER) regions = regionalizer.transform(area) joint
-= joiner.transform(regions, features) embedder = Hex2VecEmbedder()
-neighbourhood = H3Neighbourhood(regions_gdf=regions) embedder = Hex2VecEmbedder
-([15, 10, 3]) # Option 1: fit and transform # embedder.fit(regions, features,
-joint, neighbourhood, batch_size=128) # embeddings = embedder.transform
-(regions, features, joint) # Option 2: fit_transform embeddings =
-embedder.fit_transform(regions, features, joint, neighbourhood, batch_size=128)
-folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"],
-tiles_style="CartoDB positron") plot_numeric_data(regions, embeddings, 0,
-map=folium_map) ```
+srai.regionalizers import H3Regionalizer, geocode_to_region_gdf from
+srai.plotting import plot_regions, plot_numeric_data loader = OSMPbfLoader()
+regionalizer = H3Regionalizer(resolution=11) joiner = IntersectionJoiner() area
+= geocode_to_region_gdf("City of London") features = loader.load(area,
+HEX2VEC_FILTER) regions = regionalizer.transform(area) joint = joiner.transform
+(regions, features) embedder = Hex2VecEmbedder() neighbourhood =
+H3Neighbourhood(regions_gdf=regions) embedder = Hex2VecEmbedder([15, 10, 3]) #
+Option 1: fit and transform # embedder.fit(regions, features, joint,
+neighbourhood, batch_size=128) # embeddings = embedder.transform(regions,
+features, joint) # Option 2: fit_transform embeddings = embedder.fit_transform
+(regions, features, joint, neighbourhood, batch_size=128) folium_map =
+plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB
+positron") plot_numeric_data(regions, embeddings, 0, map=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                         embedding_hex2vec_embedder.jpg]
 ### Pre-trained models usage We provide pre-trained models for some of the
 embedding methods. To use them, simply download them from [here](https://
 drive.google.com/drive/folders/14sH33-
 kNxA0q1O1abPWTpuix8raR_XbD?usp=drive_link) and load them using `load` method:
 ```python from srai.embedders import Hex2VecEmbedder model_path = "path/to/
```

### Comparing `srai-0.2.0/pyproject.toml` & `srai-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "srai"
-version = "0.2.0"
+version = "0.3.0"
 description = "A set of python modules for geospatial machine learning and data mining"
 authors = [
     { name = "SRAI Lab", email = "spatialrepresentationsforai@gmail.com" },
     { name = "Piotr Gramacki" },
     { name = "Kacper Leśniara" },
     { name = "Kamil Raczycki" },
     { name = "Szymon Woźniak" },
@@ -14,21 +14,21 @@
     "geopandas",
     "shapely",
     "h3>=4.0.0b1",
     "numpy",
     "geoparquet",
     "pyfunctional",
     "rtree",
-    "scipy",
     "pyarrow",
     "topojson",
     "tqdm",
     "s2",
     "typeguard",
     "requests",
+    "h3ronpy>=0.17.4",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
@@ -53,21 +53,22 @@
 Repository = "https://github.com/srai-lab/srai"
 Documentation = "https://srai-lab.github.io/srai"
 Changelog = "https://github.com/srai-lab/srai/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 osm = [
     "osmium",
-    "osmnx<=1.4.0",
+    "osmnx",
     "overpass",
     "pillow",
 ]
 voronoi = [
     "pymap3d",
     "haversine",
+    "scipy",
     "spherical-geometry",
 ]
 gtfs = [
     "gtfs-kit",
 ]
 plotting = [
     "folium",
@@ -131,14 +132,17 @@
 performance = [
     "scalene",
 ]
 license = [
     "licensecheck",
 ]
 
+[tool.pdm.scripts]
+post_install = "pre-commit install"
+
 [tool.black]
 line-length = 100
 target-version = [
     "py38",
     "py39",
     "py310",
     "py311",
@@ -196,25 +200,31 @@
 tab-width = 4
 blank = false
 pre-summary-newline = true
 close-quotes-on-newline = true
 wrap-one-line = true
 
 [tool.bumpver]
-current_version = "0.2.0"
+current_version = "0.3.0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "chore: bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
-    "current_version = \"{version}\"",
-    "version = \"{version}\"",
+    "^current_version = \"{version}\"$",
+    "^version = \"{version}\"$",
+]
+"srai/__init__.py" = [
+    "^__version__ = \"{version}\"$",
+]
+"CITATION.cff" = [
+    "^version: {version}$",
 ]
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
 markers = [
```

### Comparing `srai-0.2.0/srai/embedders/__init__.py` & `srai-0.3.0/srai/embedders/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/embedders/_base.py` & `srai-0.3.0/srai/embedders/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from srai.constants import GEOMETRY_COLUMN
 
 try:  # pragma: no cover
     from pytorch_lightning import LightningModule
 
 except ImportError:
-    from srai.utils._pytorch_stubs import LightningModule
+    from srai.embedders._pytorch_stubs import LightningModule
 
 
 class Model(LightningModule):  # type: ignore
     """Class for model based on LightningModule."""
 
     def get_config(self) -> Dict[str, Any]:
         """Get model config."""
```

### Comparing `srai-0.2.0/srai/embedders/contextual_count_embedder.py` & `srai-0.3.0/srai/embedders/contextual_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/embedders/count_embedder.py` & `srai-0.3.0/srai/embedders/count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/embedders/gtfs2vec/embedder.py` & `srai-0.3.0/srai/embedders/gtfs2vec/embedder.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Type, Union
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 
+from srai._optional import import_optional_dependencies
 from srai.embedders import Embedder, ModelT
 from srai.embedders.gtfs2vec.model import GTFS2VecModel
 from srai.exceptions import ModelNotFitException
 from srai.loaders.gtfs_loader import GTFS2VEC_DIRECTIONS_PREFIX, GTFS2VEC_TRIPS_PREFIX
-from srai.utils._optional import import_optional_dependencies
 
 
 class GTFS2VecEmbedder(Embedder):
     """GTFS2Vec Embedder."""
 
     def __init__(
         self, hidden_size: int = 48, embedding_size: int = 64, skip_autoencoder: bool = False
```

### Comparing `srai-0.2.0/srai/embedders/gtfs2vec/model.py` & `srai-0.3.0/srai/embedders/gtfs2vec/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 This module contains embedding model from gtfs2vec paper [1].
 
 References:
     1. https://doi.org/10.1145/3486640.3491392
 """
 from typing import TYPE_CHECKING, Any
 
+from srai._optional import import_optional_dependencies
 from srai.embedders import Model
-from srai.utils._optional import import_optional_dependencies
 
 if TYPE_CHECKING:  # pragma: no cover
     import torch
 
 
 class GTFS2VecModel(Model):
     """Autoencoder based embedding model for gtfs2vec."""
```

### Comparing `srai-0.2.0/srai/embedders/hex2vec/embedder.py` & `srai-0.3.0/srai/embedders/hex2vec/embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 
+from srai._optional import import_optional_dependencies
 from srai.embedders import CountEmbedder, ModelT
 from srai.embedders.hex2vec.model import Hex2VecModel
 from srai.embedders.hex2vec.neighbour_dataset import NeighbourDataset
 from srai.exceptions import ModelNotFitException
 from srai.neighbourhoods import Neighbourhood
-from srai.utils._optional import import_optional_dependencies
 
 T = TypeVar("T")
 
 
 class Hex2VecEmbedder(CountEmbedder):
     """Hex2Vec Embedder."""
 
@@ -122,18 +122,18 @@
         import pytorch_lightning as pl
         from torch.utils.data import DataLoader
 
         trainer_kwargs = self._prepare_trainer_kwargs(trainer_kwargs)
 
         counts_df = self._get_raw_counts(regions_gdf, features_gdf, joint_gdf)
 
-        if self.expected_output_features is None:  # type: ignore
+        if self.expected_output_features is None:  # type: ignore[has-type]
             self.expected_output_features = pd.Series(counts_df.columns)
 
-        num_features = len(self.expected_output_features)  # type: ignore
+        num_features = len(self.expected_output_features)  # type: ignore[arg-type]
         self._model = Hex2VecModel(
             layer_sizes=[num_features, *self._encoder_sizes], learning_rate=learning_rate
         )
         dataset = NeighbourDataset(counts_df, neighbourhood, negative_sample_k_distance)
         dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=True)
 
         trainer = pl.Trainer(**trainer_kwargs)
```

### Comparing `srai-0.2.0/srai/embedders/hex2vec/model.py` & `srai-0.3.0/srai/embedders/hex2vec/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 This module contains the embedding model from Hex2Vec paper[1].
 
 References:
     [1] https://dl.acm.org/doi/10.1145/3486635.3491076
 """
 from typing import TYPE_CHECKING, List, Tuple
 
+from srai._optional import import_optional_dependencies
 from srai.embedders import Model
-from srai.utils._optional import import_optional_dependencies
 
 if TYPE_CHECKING:  # pragma: no cover
     import torch
 
 
 class Hex2VecModel(Model):
     """
```

### Comparing `srai-0.2.0/srai/embedders/hex2vec/neighbour_dataset.py` & `srai-0.3.0/srai/embedders/hex2vec/neighbour_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 """
 from typing import TYPE_CHECKING, Any, Dict, Generic, List, NamedTuple, Set, TypeVar
 
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 
+from srai._optional import import_optional_dependencies
 from srai.neighbourhoods import Neighbourhood
-from srai.utils._optional import import_optional_dependencies
 
 if TYPE_CHECKING:  # pragma: no cover
     import torch
 
 try:  # pragma: no cover
     from torch.utils.data import Dataset
 
 except ImportError:
-    from srai.utils._pytorch_stubs import Dataset
+    from srai.embedders._pytorch_stubs import Dataset
 
 
 T = TypeVar("T")
 
 
 class NeighbourDatasetItem(NamedTuple):
     """
```

### Comparing `srai-0.2.0/srai/embedders/highway2vec/embedder.py` & `srai-0.3.0/srai/embedders/highway2vec/embedder.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 import json
 from pathlib import Path
 from typing import Any, Dict, Optional, Type, Union
 
 import geopandas as gpd
 import pandas as pd
 
+from srai._optional import import_optional_dependencies
 from srai.embedders import Embedder, ModelT
 from srai.exceptions import ModelNotFitException
-from srai.utils._optional import import_optional_dependencies
 
 from .model import Highway2VecModel
 
 
 class Highway2VecEmbedder(Embedder):
     """Highway2Vec Embedder."""
```

### Comparing `srai-0.2.0/srai/embedders/highway2vec/model.py` & `srai-0.3.0/srai/embedders/highway2vec/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 This module contains the embedding model from the `highway2vec` paper [1].
 
 References:
     1. https://doi.org/10.1145/3557918.3565865
 """
 from typing import TYPE_CHECKING
 
+from srai._optional import import_optional_dependencies
 from srai.embedders import Model
-from srai.utils._optional import import_optional_dependencies
 
 if TYPE_CHECKING:  # pragma: no cover
     import torch
 
 
 class Highway2VecModel(Model):
     """Autoencoder based embedding model for highway2vec."""
```

### Comparing `srai-0.2.0/srai/exceptions.py` & `srai-0.3.0/srai/exceptions.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/joiners/__init__.py` & `srai-0.3.0/srai/joiners/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/joiners/_base.py` & `srai-0.3.0/srai/joiners/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/joiners/intersection_joiner.py` & `srai-0.3.0/srai/joiners/intersection_joiner.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/loaders/__init__.py` & `srai-0.3.0/srai/loaders/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 
 We want to unify loading from different data sources into a single interface. Thanks to this, we
 have a unified spatial data format, which makes it possible to feed them into any of the embedding
 methods available in this library.
 """
 
 from ._base import Loader
+from .download import download_file
 from .geoparquet_loader import GeoparquetLoader
 from .gtfs_loader import GTFSLoader
 from .osm_loaders import OSMLoader, OSMOnlineLoader, OSMPbfLoader, OSMTileLoader
-from .osm_way_loader import OSMWayLoader
+from .osm_way_loader import OSMNetworkType, OSMWayLoader
 
 __all__ = [
     "Loader",
     "GeoparquetLoader",
     "GTFSLoader",
     "OSMLoader",
     "OSMWayLoader",
     "OSMOnlineLoader",
     "OSMPbfLoader",
     "OSMTileLoader",
+    "OSMNetworkType",
+    "download_file",
 ]
```

### Comparing `srai-0.2.0/srai/loaders/_base.py` & `srai-0.3.0/srai/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/loaders/geoparquet_loader.py` & `srai-0.3.0/srai/loaders/geoparquet_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/loaders/gtfs_loader.py` & `srai-0.3.0/srai/loaders/gtfs_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import geopandas as gpd
 import pandas as pd
 from shapely.geometry import Point
 
+from srai._optional import import_optional_dependencies
 from srai.constants import GEOMETRY_COLUMN, WGS84_CRS
 from srai.loaders import Loader
-from srai.utils._optional import import_optional_dependencies
 
 if TYPE_CHECKING:  # pragma: no cover
     from gtfs_kit import Feed
 
 GTFS2VEC_DIRECTIONS_PREFIX = "directions_at_"
 GTFS2VEC_TRIPS_PREFIX = "trips_at_"
```

### Comparing `srai-0.2.0/srai/loaders/osm_loaders/filters/_typing.py` & `srai-0.3.0/srai/loaders/osm_loaders/filters/_typing.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """Module contains a dedicated type alias for OSM tags filter."""
 from typing import Dict, List, Union, cast
 
-from srai.utils.typing import is_expected_type
+from srai._typing import is_expected_type
 
-osm_tags_type = Dict[str, Union[List[str], str, bool]]
+OsmTagsFilter = Dict[str, Union[List[str], str, bool]]
 
-grouped_osm_tags_type = Dict[str, Dict[str, Union[List[str], str, bool]]]
+GroupedOsmTagsFilter = Dict[str, OsmTagsFilter]
 
 
-def merge_grouped_osm_tags_type(grouped_filter: grouped_osm_tags_type) -> osm_tags_type:
+def merge_grouped_osm_tags_filter(grouped_filter: GroupedOsmTagsFilter) -> OsmTagsFilter:
     """
     Merge grouped osm tags filter into a base one.
 
     Function merges all filter categories into a single one for an OSM loader to use.
 
     Args:
-        grouped_filter (grouped_osm_tags_type): Grouped filter to be merged into a single one.
+        grouped_filter (GroupedOsmTagsFilter): Grouped filter to be merged into a single one.
 
     Returns:
         osm_tags_type: Merged filter.
     """
-    if not is_expected_type(grouped_filter, grouped_osm_tags_type):
+    if not is_expected_type(grouped_filter, GroupedOsmTagsFilter):
         raise ValueError(
-            "Provided filter doesn't match required `grouped_osm_tags_type` definition."
+            "Provided filter doesn't match required `GroupedOsmTagsFilter` definition."
         )
 
-    result: osm_tags_type = {}
+    result: OsmTagsFilter = {}
     for sub_filter in grouped_filter.values():
         for osm_tag_key, osm_tag_value in sub_filter.items():
             if osm_tag_key not in result:
                 result[osm_tag_key] = []
 
             # If filter is already a positive boolean, skip
             if isinstance(result[osm_tag_key], bool) and result[osm_tag_key]:
```

### Comparing `srai-0.2.0/srai/loaders/osm_loaders/filters/base_osm_groups.py` & `srai-0.3.0/srai/loaders/osm_loaders/filters/base_osm_groups.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 This module contains the grouped OSM tags filter that was used in ARIC@SIGSPATIAL 2021 paper [1].
 
 References:
     1. https://doi.org/10.1145/3486626.3493434
     1. https://arxiv.org/abs/2111.00990
 """
-from srai.loaders.osm_loaders.filters._typing import grouped_osm_tags_type
+from srai.loaders.osm_loaders.filters import GroupedOsmTagsFilter
 
-BASE_OSM_GROUPS_FILTER: grouped_osm_tags_type = {
+BASE_OSM_GROUPS_FILTER: GroupedOsmTagsFilter = {
     "water": {"natual": ["water", "bay", "beach", "coastline"], "waterway": ["riverbank"]},
     "aerialway": {
         "aerialway": [
             "cable_car",
             "gondola",
             "mixed_lift",
             "chair_lift",
```

### Comparing `srai-0.2.0/srai/loaders/osm_loaders/filters/geofabrik.py` & `srai-0.3.0/srai/loaders/osm_loaders/filters/geofabrik.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 Based on the document version `0.7.12`.
 
 Note: not all definitions from the document are implemented, such as boundaries or places.
 
 References:
     1. https://www.geofabrik.de/data/geofabrik-osm-gis-standard-0.7.pdf
 """
-from srai.loaders.osm_loaders.filters._typing import grouped_osm_tags_type
+from srai.loaders.osm_loaders.filters import GroupedOsmTagsFilter
 
-GEOFABRIK_LAYERS: grouped_osm_tags_type = {
+GEOFABRIK_LAYERS: GroupedOsmTagsFilter = {
     "public": {
         "amenity": [
             "police",
             "fire_station",
             "post_box",
             "post_office",
             "telephone",
```

### Comparing `srai-0.2.0/srai/loaders/osm_loaders/filters/hex2vec.py` & `srai-0.3.0/srai/loaders/osm_loaders/filters/hex2vec.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Hex2Vec filter.
 
 This module contains the OSM tags filter that was used in Hex2Vec [1].
 
 References:
     1. https://dl.acm.org/doi/10.1145/3486635.3491076
 """
-from srai.loaders.osm_loaders.filters._typing import osm_tags_type
+from srai.loaders.osm_loaders.filters import OsmTagsFilter
 
-HEX2VEC_FILTER: osm_tags_type = {
+HEX2VEC_FILTER: OsmTagsFilter = {
     "aeroway": [
         "aerodrome",
         "apron",
         "gate",
         "hangar",
         "helipad",
         "heliport",
```

### Comparing `srai-0.2.0/srai/loaders/osm_loaders/filters/popular.py` & `srai-0.3.0/srai/loaders/osm_loaders/filters/popular.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     1. https://taginfo.openstreetmap.org/
 """
 from typing import Any, Dict, List
 
 import requests
 from functional import seq
 
-from srai.loaders.osm_loaders.filters._typing import osm_tags_type
+from srai.loaders.osm_loaders.filters import OsmTagsFilter
 
 _TAGINFO_API_ADDRESS = "https://taginfo.openstreetmap.org"
 _TAGINFO_API_TAGS = _TAGINFO_API_ADDRESS + "/api/4/tags/popular"
 
 
 def get_popular_tags(
     in_wiki_only: bool = False, min_count: int = 0, min_fraction: float = 0.0
-) -> osm_tags_type:
+) -> OsmTagsFilter:
     """
     Download the OSM's most popular tags from taginfo api.
 
     This is a wrapper around the `popular` taginfo api endpoint [1].
     It queries the API, and optionally filters the results
     according to argument values.
 
@@ -49,19 +49,19 @@
     taginfo_api_response.raise_for_status()
     taginfo_data = taginfo_api_response.json()["data"]
     return _parse_taginfo_response(taginfo_data, in_wiki_only, min_count, min_fraction)
 
 
 def _parse_taginfo_response(
     taginfo_data: List[Dict[str, Any]], in_wiki_only: bool, min_count: int, min_fraction: float
-) -> osm_tags_type:
+) -> OsmTagsFilter:
     result_tags = (
         seq(taginfo_data)
         .filter(lambda t: t["count_all"] >= min_count)
         .filter(lambda t: t["count_all_fraction"] >= min_fraction)
     )
     if in_wiki_only:
         result_tags = result_tags.filter(lambda t: t["in_wiki"])
-    taginfo_grouped: osm_tags_type = (
+    taginfo_grouped: OsmTagsFilter = (
         result_tags.map(lambda t: (t["key"], t["value"])).group_by_key().to_dict()
     )
     return taginfo_grouped
```

### Comparing `srai-0.2.0/srai/loaders/osm_loaders/osm_online_loader.py` & `srai-0.3.0/srai/loaders/osm_loaders/osm_online_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,18 @@
 from typing import List, Tuple, Union
 
 import geopandas as gpd
 import pandas as pd
 from functional import seq
 from tqdm import tqdm
 
+from srai._optional import import_optional_dependencies
 from srai.constants import FEATURES_INDEX, GEOMETRY_COLUMN, WGS84_CRS
 from srai.loaders.osm_loaders._base import OSMLoader
-from srai.loaders.osm_loaders.filters._typing import (
-    grouped_osm_tags_type,
-    osm_tags_type,
-)
-from srai.utils._optional import import_optional_dependencies
+from srai.loaders.osm_loaders.filters import GroupedOsmTagsFilter, OsmTagsFilter
 
 
 class OSMOnlineLoader(OSMLoader):
     """
     OSMOnlineLoader.
 
     OSM(OpenStreetMap)[1] online loader is a loader capable of downloading objects
@@ -44,28 +41,28 @@
     def __init__(self) -> None:
         """Initialize OSMOnlineLoader."""
         import_optional_dependencies(dependency_group="osm", modules=["osmnx"])
 
     def load(
         self,
         area: gpd.GeoDataFrame,
-        tags: Union[osm_tags_type, grouped_osm_tags_type],
+        tags: Union[OsmTagsFilter, GroupedOsmTagsFilter],
     ) -> gpd.GeoDataFrame:
         """
         Download OSM features with specified tags for a given area.
 
         The loader first downloads all objects with `tags`. It returns a GeoDataFrame containing
         the `geometry` column and columns for tag keys.
 
         Note: Some key/value pairs might be missing from the resulting GeoDataFrame,
             simply because there are no such objects in the given area.
 
         Args:
             area (gpd.GeoDataFrame): Area for which to download objects.
-            tags (Union[osm_tags_type, grouped_osm_tags_type]): A dictionary
+            tags (Union[OsmTagsFilter, GroupedOsmTagsFilter]): A dictionary
                 specifying which tags to download.
                 The keys should be OSM tags (e.g. `building`, `amenity`).
                 The values should either be `True` for retrieving all objects with the tag,
                 string for retrieving a single tag-value pair
                 or list of strings for retrieving all values specified in the list.
                 `tags={'leisure': 'park}` would return parks from the area.
                 `tags={'leisure': 'park, 'amenity': True, 'shop': ['bakery', 'bicycle']}`
@@ -98,15 +95,15 @@
                 results.append(geometries[[GEOMETRY_COLUMN, key]])
 
         result_gdf = self._group_gdfs(results).set_crs(WGS84_CRS)
         result_gdf = self._flatten_index(result_gdf)
 
         return self._parse_features_gdf_to_groups(result_gdf, tags)
 
-    def _flatten_tags(self, tags: osm_tags_type) -> List[Tuple[str, Union[str, bool]]]:
+    def _flatten_tags(self, tags: OsmTagsFilter) -> List[Tuple[str, Union[str, bool]]]:
         tags_flat: List[Tuple[str, Union[str, bool]]] = (
             seq(tags.items())
             .starmap(lambda k, v: product([k], v if isinstance(v, list) else [v]))
             .flatten()
             .list()
         )
         return tags_flat
```

### Comparing `srai-0.2.0/srai/loaders/osm_loaders/osm_pbf_loader.py` & `srai-0.3.0/srai/loaders/osm_loaders/osm_pbf_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,21 +5,18 @@
 """
 from pathlib import Path
 from typing import Hashable, List, Mapping, Optional, Sequence, Union
 
 import geopandas as gpd
 import pandas as pd
 
+from srai._optional import import_optional_dependencies
 from srai.constants import FEATURES_INDEX, GEOMETRY_COLUMN, WGS84_CRS
 from srai.loaders.osm_loaders._base import OSMLoader
-from srai.loaders.osm_loaders.filters._typing import (
-    grouped_osm_tags_type,
-    osm_tags_type,
-)
-from srai.utils._optional import import_optional_dependencies
+from srai.loaders.osm_loaders.filters import GroupedOsmTagsFilter, OsmTagsFilter
 
 
 class OSMPbfLoader(OSMLoader):
     """
     OSMPbfLoader.
 
     OSM(OpenStreetMap)[1] PBF(Protocolbuffer Binary Format)[2] loader is a loader
@@ -54,15 +51,15 @@
         import_optional_dependencies(dependency_group="osm", modules=["osmium"])
         self.pbf_file = pbf_file
         self.download_directory = download_directory
 
     def load(
         self,
         area: gpd.GeoDataFrame,
-        tags: Union[osm_tags_type, grouped_osm_tags_type],
+        tags: Union[OsmTagsFilter, GroupedOsmTagsFilter],
     ) -> gpd.GeoDataFrame:
         """
         Load OSM features with specified tags for a given area from an `*.osm.pbf` file.
 
         The loader will use provided `*.osm.pbf` file, or download extracts
         using `PbfFileDownloader`. Later it will parse and filter features from files
         using `PbfFileHandler`. It will return a GeoDataFrame containing the `geometry` column
@@ -74,15 +71,15 @@
         Note: If you want to extract data for a big area (like country, or more), it's encouraged
             to use existing `*.osm.pbf` extracts from GeoFabrik (https://download.geofabrik.de/)
             or BBBike (https://extract.bbbike.org/). You can provide those predownloaded files in
             the constructor of the `OSMPbfLoader`.
 
         Args:
             area (gpd.GeoDataFrame): Area for which to download objects.
-            tags (Union[osm_tags_type, grouped_osm_tags_type]): A dictionary
+            tags (Union[OsmTagsFilter, GroupedOsmTagsFilter]): A dictionary
                 specifying which tags to download.
                 The keys should be OSM tags (e.g. `building`, `amenity`).
                 The values should either be `True` for retrieving all objects with the tag,
                 string for retrieving a single tag-value pair
                 or list of strings for retrieving all values specified in the list.
                 `tags={'leisure': 'park}` would return parks from the area.
                 `tags={'leisure': 'park, 'amenity': True, 'shop': ['bakery', 'bicycle']}`
```

### Comparing `srai-0.2.0/srai/loaders/osm_loaders/osm_tile_data_collector.py` & `srai-0.3.0/srai/loaders/osm_loaders/osm_tile_data_collector.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/loaders/osm_loaders/osm_tile_loader.py` & `srai-0.3.0/srai/loaders/osm_loaders/osm_tile_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from typing import Any, Optional, Union
 from urllib.parse import urljoin
 
 import geopandas as gpd
 import pandas as pd
 import requests
 
+from srai._optional import import_optional_dependencies
 from srai.regionalizers.slippy_map_regionalizer import SlippyMapRegionalizer
-from srai.utils._optional import import_optional_dependencies
 
 from .osm_tile_data_collector import (
     DataCollector,
     DataCollectorType,
     InMemoryDataCollector,
     get_collector,
 )
```

### Comparing `srai-0.2.0/srai/loaders/osm_loaders/pbf_file_downloader.py` & `srai-0.3.0/srai/loaders/osm_loaders/pbf_file_downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 import geopandas as gpd
 import requests
 import shapely.wkt as wktlib
 import topojson as tp
 from shapely.geometry import Polygon, mapping
 from shapely.geometry.base import BaseGeometry
-from shapely.validation import make_valid
 from tqdm import tqdm
 
 from srai.constants import WGS84_CRS
-from srai.utils import buffer_geometry, download_file, flatten_geometry, remove_interiors
+from srai.geometry import buffer_geometry, flatten_geometry, remove_interiors
+from srai.loaders import download_file
 
 
 class PbfFileDownloader:
     """
     PbfFileDownloader.
 
     PBF(Protocolbuffer Binary Format)[1] file downloader is a downloader
@@ -215,48 +215,55 @@
         """
         Prepare polygon for download.
 
         Function buffers the polygon, closes internal holes and simplifies its boundary to 1000
         points.
 
         Makes sure that the generated polygon with fully cover the original one by increasing the
-        buffer size incrementally.
+        buffer size incrementally. Buffering is applied to the last simplified geometry to speed up
+        the process.
         """
         is_fully_covered = False
         buffer_size_meters = 50
+
+        polygon_to_buffer = polygon
+
         while not is_fully_covered:
-            buffered_polygon = buffer_geometry(polygon, meters=buffer_size_meters)
-            simplified_polygon = self._simplify_polygon(buffered_polygon)
+            buffered_polygon = buffer_geometry(polygon_to_buffer, meters=buffer_size_meters)
+            simplified_polygon = self._simplify_polygon(buffered_polygon, 1000)
             closed_polygon = remove_interiors(simplified_polygon)
             is_fully_covered = polygon.covered_by(closed_polygon)
             buffer_size_meters += 50
+
+            polygon_to_buffer = closed_polygon
+
         return closed_polygon
 
-    def _simplify_polygon(self, polygon: Polygon) -> Polygon:
-        """Simplify a polygon boundary to up to 1000 points."""
+    def _simplify_polygon(self, polygon: Polygon, exterior_max_points: int = 1000) -> Polygon:
+        """Simplify a polygon boundary to up to provided number of points."""
         simplified_polygon = polygon
 
         for simplify_tolerance in self.SIMPLIFICATION_TOLERANCE_VALUES:
             simplified_polygon = (
                 tp.Topology(
                     polygon,
                     toposimplify=simplify_tolerance,
                     prevent_oversimplify=True,
                 )
                 .to_gdf(winding_order="CW_CCW", crs=WGS84_CRS, validate=True)
                 .geometry[0]
             )
-            simplified_polygon = make_valid(simplified_polygon)
-            if len(simplified_polygon.exterior.coords) < 1000:
+
+            if len(simplified_polygon.exterior.coords) < exterior_max_points:
                 break
 
-        if len(simplified_polygon.exterior.coords) > 1000:
+        if len(simplified_polygon.exterior.coords) > exterior_max_points:
             simplified_polygon = polygon.convex_hull
 
-        if len(simplified_polygon.exterior.coords) > 1000:
+        if len(simplified_polygon.exterior.coords) > exterior_max_points:
             simplified_polygon = polygon.minimum_rotated_rectangle
 
         return simplified_polygon
 
     def _get_geometry_hash(self, geometry: BaseGeometry) -> str:
         """Generate SHA256 hash based on WKT representation of the polygon."""
         wkt_string = wktlib.dumps(geometry)
```

### Comparing `srai-0.2.0/srai/loaders/osm_loaders/pbf_file_handler.py` & `srai-0.3.0/srai/loaders/osm_loaders/pbf_file_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import shapely.wkb as wkblib
 from osmium.osm.types import T_obj
 from shapely.geometry import MultiPolygon, Polygon
 from shapely.geometry.base import BaseGeometry
 from tqdm import tqdm
 
 from srai.constants import FEATURES_INDEX, WGS84_CRS
-from srai.loaders.osm_loaders.filters._typing import osm_tags_type
+from srai.loaders.osm_loaders.filters import OsmTagsFilter
 
 if TYPE_CHECKING:
     import os
 
 
 class PbfFileHandler(osmium.SimpleHandler):  # type: ignore
     """
@@ -42,15 +42,15 @@
         3. https://osmcode.org/pyosmium/
     """
 
     _PBAR_FORMAT = "[{}] Parsing pbf file #{}"
 
     def __init__(
         self,
-        tags: Optional[osm_tags_type] = None,
+        tags: Optional[OsmTagsFilter] = None,
         region_geometry: Optional[BaseGeometry] = None,
     ) -> None:
         """
         Initialize PbfFileHandler.
 
         Args:
             tags (osm_tags_type, optional): A dictionary
```

### Comparing `srai-0.2.0/srai/loaders/osm_way_loader/constants.py` & `srai-0.3.0/srai/loaders/osm_way_loader/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/loaders/osm_way_loader/osm_way_loader.py` & `srai-0.3.0/srai/loaders/osm_way_loader/osm_way_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import shapely.geometry as shpg
 from functional import seq
 from tqdm.auto import tqdm
 
+from srai._optional import import_optional_dependencies
 from srai.constants import FEATURES_INDEX, GEOMETRY_COLUMN, WGS84_CRS
 from srai.exceptions import LoadedDataIsEmptyException
 from srai.loaders import Loader
-from srai.utils._optional import import_optional_dependencies
 
 from . import constants
 
 logger = logging.getLogger(__name__)
 
 
-class NetworkType(str, Enum):
+class OSMNetworkType(str, Enum):
     """
     Type of the street network.
 
     See [1] for more details.
 
     References:
         1. https://osmnx.readthedocs.io/en/stable/osmnx.html#osmnx.graph.graph_from_place
@@ -51,15 +51,15 @@
     from OpenStreetMap. As the OSM data is often noisy, it can also take an opinionated approach
     to preprocessing it, with standardisation in mind - e.g. unification of units,
     discarding non-wiki values and rounding them.
     """
 
     def __init__(
         self,
-        network_type: Union[NetworkType, str],
+        network_type: Union[OSMNetworkType, str],
         contain_within_area: bool = False,
         preprocess: bool = True,
         wide: bool = True,
         metadata: bool = False,
         osm_way_tags: Dict[str, List[str]] = constants.OSM_WAY_TAGS,
     ) -> None:
         """
```

### Comparing `srai-0.2.0/srai/neighbourhoods/adjacency_neighbourhood.py` & `srai-0.3.0/srai/neighbourhoods/adjacency_neighbourhood.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Adjacency neighbourhood.
 
 This module contains the AdjacencyNeighbourhood class, that allows to get the neighbours of any
 region based on its borders.
 """
-from typing import Dict, Hashable, Set
+from typing import Dict, Hashable, Optional, Set
 
 import geopandas as gpd
 
 from srai.constants import GEOMETRY_COLUMN
 from srai.neighbourhoods import Neighbourhood
 
 
@@ -19,52 +19,64 @@
     This class allows to get the neighbours of any region based on common border. Additionally, a
     lookup table is implemented to accelerate repeated queries.
 
     By default, a lookup table will be populated lazily based on queries. A dedicated function
     `generate_neighbourhoods` allows for precalculation of all the neighbourhoods at once.
     """
 
-    def __init__(self, regions_gdf: gpd.GeoDataFrame) -> None:
+    def __init__(self, regions_gdf: gpd.GeoDataFrame, include_center: bool = False) -> None:
         """
         Init AdjacencyNeighbourhood.
 
         Args:
             regions_gdf (gpd.GeoDataFrame): regions for which a neighbourhood will be calculated.
+            include_center (bool): Whether to include the region itself in the neighbours.
+            This is the default value used for all the methods of the class,
+            unless overridden in the function call.
 
         Raises:
             ValueError: If regions_gdf doesn't have geometry column.
         """
+        super().__init__(include_center)
         if GEOMETRY_COLUMN not in regions_gdf.columns:
             raise ValueError("Regions must have a geometry column.")
         self.regions_gdf = regions_gdf
         self.lookup: Dict[Hashable, Set[Hashable]] = {}
 
     def generate_neighbourhoods(self) -> None:
         """Generate the lookup table for all regions."""
         for region_id in self.regions_gdf.index:
             if region_id not in self.lookup:
                 self.lookup[region_id] = self._get_adjacent_neighbours(region_id)
 
-    def get_neighbours(self, index: Hashable) -> Set[Hashable]:
+    def get_neighbours(
+        self, index: Hashable, include_center: Optional[bool] = None
+    ) -> Set[Hashable]:
         """
         Get the direct neighbours of any region using its index.
 
         Args:
             index (Hashable): Unique identifier of the region.
+            include_center (Optional[bool]): Whether to include the region itself in the neighbours.
+            If None, the value set in __init__ is used. Defaults to None.
 
         Returns:
             Set[Hashable]: Indexes of the neighbours.
         """
         if self._index_incorrect(index):
             return set()
 
         if index not in self.lookup:
             self.lookup[index] = self._get_adjacent_neighbours(index)
 
-        return self.lookup[index]
+        neighbours = self.lookup[index]
+        neighbours = self._handle_center(
+            index, 1, neighbours, at_distance=False, include_center_override=include_center
+        )
+        return neighbours
 
     def _get_adjacent_neighbours(self, index: Hashable) -> Set[Hashable]:
         """
         Get the direct neighbours of a region using `touches` [1] operator from the Shapely library.
 
         Args:
             index (Hashable): Unique identifier of the region.
```

### Comparing `srai-0.2.0/srai/neighbourhoods/h3_neighbourhood.py` & `srai-0.3.0/srai/neighbourhoods/h3_neighbourhood.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,83 +14,102 @@
 class H3Neighbourhood(Neighbourhood[str]):
     """
     H3 Neighbourhood.
 
     This class allows to get the neighbours of an H3 region.
     """
 
-    def __init__(self, regions_gdf: Optional[gpd.GeoDataFrame] = None) -> None:
+    def __init__(
+        self, regions_gdf: Optional[gpd.GeoDataFrame] = None, include_center: bool = False
+    ) -> None:
         """
         Initializes the H3Neighbourhood.
 
         If a regions GeoDataFrame is provided, only the neighbours
         that are in the regions GeoDataFrame will be returned by the methods of this instance.
         NOTICE: If a region is a part of the k-th ring of a region
             and is included in the GeoDataFrame, it will be returned
             by get_neighbours_at_distance method with distance k
             even when there is no path of length k between the two regions.
 
         Args:
             regions_gdf (Optional[gpd.GeoDataFrame], optional): The regions that are being analyzed.
                 The H3Neighbourhood will only look for neighbours among these regions.
                 Defaults to None.
+            include_center (bool): Whether to include the region itself in the neighbours.
+            This is the default value used for all the methods of the class,
+            unless overridden in the function call.
         """
-        super().__init__()
+        super().__init__(include_center)
         self._available_indices: Optional[Set[str]] = None
         if regions_gdf is not None:
             self._available_indices = set(regions_gdf.index)
 
-    def get_neighbours(self, index: str) -> Set[str]:
+    def get_neighbours(self, index: str, include_center: Optional[bool] = None) -> Set[str]:
         """
         Get the direct neighbours of an H3 region using its index.
 
         Args:
             index (str): H3 index of the region.
+            include_center (Optional[bool]): Whether to include the region itself in the neighbours.
+            If None, the value set in __init__ is used. Defaults to None.
 
         Returns:
             Set[str]: Indexes of the neighbours.
         """
-        return self.get_neighbours_up_to_distance(index, 1)
+        return self.get_neighbours_up_to_distance(index, 1, include_center)
 
-    def get_neighbours_up_to_distance(self, index: str, distance: int) -> Set[str]:
+    def get_neighbours_up_to_distance(
+        self, index: str, distance: int, include_center: Optional[bool] = None
+    ) -> Set[str]:
         """
         Get the neighbours of an H3 region up to a certain distance.
 
         Args:
             index (str): H3 index of the region.
             distance (int): Distance to the neighbours.
+            include_center (Optional[bool]): Whether to include the region itself in the neighbours.
+            If None, the value set in __init__ is used. Defaults to None.
 
         Returns:
             Set[str]: Indexes of the neighbours up to the given distance.
         """
         if self._distance_incorrect(distance):
             return set()
 
         neighbours: Set[str] = h3.grid_disk(index, distance)
-        neighbours.discard(index)
+        neighbours = self._handle_center(
+            index, distance, neighbours, at_distance=False, include_center_override=include_center
+        )
         return self._select_available(neighbours)
 
-    def get_neighbours_at_distance(self, index: str, distance: int) -> Set[str]:
+    def get_neighbours_at_distance(
+        self, index: str, distance: int, include_center: Optional[bool] = None
+    ) -> Set[str]:
         """
         Get the neighbours of an H3 region at a certain distance.
 
         Args:
             index (str): H3 index of the region.
             distance (int): Distance to the neighbours.
+            include_center (Optional[bool]): Whether to include the region itself in the neighbours.
+            If None, the value set in __init__ is used. Defaults to None.
 
         Returns:
             Set[str]: Indexes of the neighbours at the given distance.
         """
         if self._distance_incorrect(distance):
             return set()
 
         neighbours: Set[str] = h3.grid_ring(index, distance)
-        neighbours.discard(index)
+        neighbours = self._handle_center(
+            index, distance, neighbours, at_distance=True, include_center_override=include_center
+        )
         return self._select_available(neighbours)
 
     def _select_available(self, indices: Set[str]) -> Set[str]:
         if self._available_indices is None:
             return indices
         return indices.intersection(self._available_indices)
 
     def _distance_incorrect(self, distance: int) -> bool:
-        return distance <= 0
+        return distance < 0
```

### Comparing `srai-0.2.0/srai/plotting/folium_wrapper.py` & `srai-0.3.0/srai/plotting/folium_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,31 +3,28 @@
 
 This module contains functions for quick plotting of analysed gdfs using Geopandas `explore()`
 function.
 """
 from itertools import cycle, islice
 from typing import List, Optional, Set, Union
 
-from srai.utils._optional import import_optional_dependencies
-
-import_optional_dependencies(dependency_group="plotting", modules=["folium", "plotly"])
-
-# flake8: noqa E402
-
 import branca.colormap as cm
 import folium
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import plotly.express as px
 
+from srai._optional import import_optional_dependencies
 from srai.constants import REGIONS_INDEX
 from srai.neighbourhoods import Neighbourhood
 from srai.neighbourhoods._base import IndexType
 
+import_optional_dependencies(dependency_group="plotting", modules=["folium", "plotly"])
+
 
 def plot_regions(
     regions_gdf: gpd.GeoDataFrame,
     tiles_style: str = "OpenStreetMap",
     height: Union[str, float] = "100%",
     width: Union[str, float] = "100%",
     colormap: Union[str, List[str]] = px.colors.qualitative.Bold,
```

### Comparing `srai-0.2.0/srai/plotting/plotly_wrapper.py` & `srai-0.3.0/srai/plotting/plotly_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """
 Plotly wrapper.
 
 This module contains functions for quick plotting of analysed gdfs using Plotly library.
 """
 from typing import Any, Dict, List, Optional, Set
 
-from srai.utils._optional import import_optional_dependencies
-
-import_optional_dependencies(dependency_group="plotting", modules=["plotly"])
-
-# flake8: noqa E402
-
 import geopandas as gpd
 import numpy as np
 import plotly.express as px
 import plotly.graph_objs as go
 from shapely.geometry import Point
 
+from srai._optional import import_optional_dependencies
 from srai.constants import REGIONS_INDEX, WGS84_CRS
 from srai.neighbourhoods import Neighbourhood
 from srai.neighbourhoods._base import IndexType
 
+import_optional_dependencies(dependency_group="plotting", modules=["plotly"])
+
 
 def plot_regions(
     regions_gdf: gpd.GeoDataFrame,
     return_plot: bool = False,
     mapbox_style: str = "open-street-map",
     mapbox_accesstoken: Optional[str] = None,
     renderer: Optional[str] = None,
@@ -346,12 +343,11 @@
 
     Args:
         regions_gdf (gpd.GeoDataFrame): Region indexes and geometries.
 
     Returns:
         float: zoom level for a mapbox plot.
     """
-
     minx, miny, maxx, maxy = regions_gdf.geometry.total_bounds
     max_bound = max(abs(maxx - minx), abs(maxy - miny)) * 111
     zoom = float(12.5 - np.log(max_bound))
     return zoom
```

### Comparing `srai-0.2.0/srai/regionalizers/__init__.py` & `srai-0.3.0/srai/regionalizers/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 this module, we aggregate different regionalization methods under a common `Regionalizer` interface.
 We include both pre-defined spatial indexes (e.g. H3 or S2), data-based ones (e.g. Voronoi) and OSM-
 based ones (e.g. administrative boundaries).
 """
 
 from ._base import Regionalizer
 from .administrative_boundary_regionalizer import AdministrativeBoundaryRegionalizer
+from .geocode import geocode_to_region_gdf
 from .h3_regionalizer import H3Regionalizer
 from .s2_regionalizer import S2Regionalizer
 from .slippy_map_regionalizer import SlippyMapRegionalizer
 from .voronoi_regionalizer import VoronoiRegionalizer
 
 __all__ = [
     "Regionalizer",
     "AdministrativeBoundaryRegionalizer",
     "H3Regionalizer",
     "S2Regionalizer",
     "VoronoiRegionalizer",
     "SlippyMapRegionalizer",
+    "geocode_to_region_gdf",
 ]
```

### Comparing `srai-0.2.0/srai/regionalizers/_base.py` & `srai-0.3.0/srai/regionalizers/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/regionalizers/_spherical_voronoi.py` & `srai-0.3.0/srai/regionalizers/_spherical_voronoi.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,31 +2,45 @@
 Spherical voronoi utils.
 
 This module contains spherical voronoi implementation based on SphericalVoronoi function from scipy
 library.
 """
 
 from functools import partial
-from math import ceil, sqrt
+from math import ceil
 from multiprocessing import cpu_count
-from typing import List, Optional, Tuple
+from typing import Hashable, List, Optional, Tuple, Union
 
+import geopandas as gpd
 import numpy as np
 import numpy.typing as npt
 from haversine import haversine
 from pymap3d import Ellipsoid, ecef2geodetic, geodetic2ecef
 from scipy.spatial import SphericalVoronoi, geometric_slerp
-from shapely.geometry import MultiPolygon, Point, Polygon, box
+from shapely.geometry import (
+    GeometryCollection,
+    LineString,
+    MultiLineString,
+    MultiPolygon,
+    Point,
+    Polygon,
+    box,
+)
+from shapely.validation import make_valid
 from spherical_geometry.polygon import SphericalPolygon
 from tqdm import tqdm
 from tqdm.contrib.concurrent import process_map
 
+from srai.constants import WGS84_CRS
+
 SPHERE_PARTS: List[SphericalPolygon] = []
 SPHERE_PARTS_BOUNDING_BOXES: List[Polygon] = []
 
+SCIPY_THRESHOLD = 1e-8
+
 
 def _generate_sphere_parts() -> None:
     global SPHERE_PARTS, SPHERE_PARTS_BOUNDING_BOXES  # noqa: PLW0603
 
     if not SPHERE_PARTS:
         # LON: 0; LAT: 0
         POINT_FRONT = (1.0, 0.0, 0.0)
@@ -51,172 +65,188 @@
             box(minx=0, miny=0, maxx=180, maxy=90),
             box(minx=0, miny=-90, maxx=180, maxy=0),
             box(minx=-180, miny=-90, maxx=0, maxy=0),
             box(minx=-180, miny=0, maxx=0, maxy=90),
         ]
 
 
-class SphereEllipsoid(Ellipsoid):  # type: ignore
-    """A sphere ellipsoid."""
-
-    def __init__(self) -> None:
-        """
-        Sphere ellipsoid extends Ellipsoid from pymap3d [1] library.
-
-        Class is used for mapping lat/lon coordinates
-        from and to cartesian x/y/z values on a unit sphere.
-        Required for spherical voronoi algorithm.
-
-        References:
-            1. https://github.com/geospace-code/pymap3d
-        """
-        self.semimajor_axis = 1
-        self.semiminor_axis = 1
-        self.flattening = (self.semimajor_axis - self.semiminor_axis) / self.semimajor_axis
-        self.thirdflattening = (self.semimajor_axis - self.semiminor_axis) / (
-            self.semimajor_axis + self.semiminor_axis
-        )
-        self.eccentricity = sqrt(2 * self.flattening - self.flattening**2)
-
-
-def map_to_geocentric(lon: float, lat: float, ell: Ellipsoid) -> Tuple[float, float, float]:
+def generate_voronoi_regions(
+    seeds: Union[gpd.GeoDataFrame, List[Point]],
+    max_meters_between_points: int = 10_000,
+    num_of_multiprocessing_workers: int = -1,
+    multiprocessing_activation_threshold: Optional[int] = None,
+) -> List[MultiPolygon]:
     """
-    Wrapper for a geodetic2ecef function from pymap3d library.
+    Generate Thessien polygons for a given list of seeds.
+
+    Function generates Thessien polygons on a sphere using
+    SphericalVoronoi algorithm from scipy library.
 
     Args:
-        lon (float): longitude of a point in a wgs84 crs.
-        lat (float): latitude of a point in a wgs84 crs.
-        ell (Ellipsoid): an ellipsoid.
+        seeds (Union[gpd.GeoDataFrame, List[Point]]): Seeds used for generating regions.
+            If list, the points are expected to be in WGS84 coordinates (lat, lon).
+            Otherwise, a GeoDataFrame will be transformed into WGS84.
+        max_meters_between_points (int, optional): Maximal distance in meters between two points
+            in the resulting polygon. Higher number results lower resolution of a polygon.
+            Defaults to 10_000 (10 kilometers).
+        num_of_multiprocessing_workers (int, optional): Number of workers used for multiprocessing.
+            Defaults to -1 which results in a total number of available cpu threads.
+            `0` and `1` values disable multiprocessing.
+            Similar to `n_jobs` parameter from `scikit-learn` library.
+        multiprocessing_activation_threshold (int, optional): Number of seeds required to start
+            processing on multiple processes. Activating multiprocessing for a small
+            amount of points might not be feasible. Defaults to 100.
 
     Returns:
-        Tuple[float, float, float]: (x, y, z) coordinates tuple.
+        List[MultiPolygon]: List of MultiPolygons cut into up to 4 polygons based
+            on quadrants of a sphere.
+
+    Raises:
+        ValueError: If less than 4 seeds are provided.
+        ValueError: If any seed is duplicated.
+        ValueError: If any seed is outside WGS84 coordinates domain.
     """
-    x, y, z = geodetic2ecef(lat, lon, 0, ell=ell)
-    return x, y, z
+    if isinstance(seeds, gpd.GeoDataFrame):
+        seeds, region_ids = _generate_seeds(seeds)
+    else:
+        region_ids = list(range(len(seeds)))
 
+    if len(seeds) < 4:
+        raise ValueError("Minimum 4 seeds are required.")
 
-def map_from_geocentric(x: float, y: float, z: float, ell: Ellipsoid) -> Tuple[float, float]:
-    """
-    Wrapper for a ecef2geodetic function from pymap3d library.
+    duplicated_seeds_ids = _get_duplicated_seeds_ids(seeds, region_ids)
+    if duplicated_seeds_ids:
+        raise ValueError(f"Duplicate seeds present: {duplicated_seeds_ids}.")
 
-    Args:
-        x (float): X cartesian coordinate.
-        y (float): Y cartesian coordinate.
-        z (float): Z cartesian coordinate.
-        ell (Ellipsoid): an ellipsoid.
+    if not _check_if_in_bounds(seeds):
+        raise ValueError("Seeds outside Earth WGS84 bounding box.")
 
-    Returns:
-        Tuple[float, float]: longitude and latitude coordinates in a wgs84 crs.
-    """
-    lat, lon, _ = ecef2geodetic(x, y, z, ell=ell)
-    return lon, lat
+    num_of_multiprocessing_workers = _parse_num_of_multiprocessing_workers(
+        num_of_multiprocessing_workers
+    )
+    multiprocessing_activation_threshold = _parse_multiprocessing_activation_threshold(
+        multiprocessing_activation_threshold
+    )
 
+    unit_sphere_ellipsoid = Ellipsoid(
+        semimajor_axis=1, semiminor_axis=1, name="Unit Sphere", model="Unit"
+    )
+    mapped_points = [_map_to_geocentric(pt.x, pt.y, unit_sphere_ellipsoid) for pt in seeds]
+    sphere_points = np.array([[pt[0], pt[1], pt[2]] for pt in mapped_points])
 
-def _fix_lat_lon(
-    lon: float,
-    lat: float,
-    bbox: Tuple[float, float, float, float],
-) -> Tuple[float, float]:
-    """
-    Fix point signs and rounding.
+    radius = 1
+    center = np.array([0, 0, 0])
+    sv = SphericalVoronoi(sphere_points, radius, center, threshold=SCIPY_THRESHOLD)
+    sv.sort_vertices_of_regions()
 
-    Rounds latitude and longitude to 8 decimal places.
-    Checks if any point is on a boundary and flips its sign
-    to ensure validity of a polygon.
+    create_regions_func = partial(
+        _create_region,
+        sv=sv,
+        ell=unit_sphere_ellipsoid,
+        max_meters_between_points=max_meters_between_points,
+    )
 
-    Args:
-        lon (float): Longitude of a point.
-        lat (float): Latitude of a point.
-        bbox (Tuple[float, float, float, float]): Current sphere octant bounding box.
+    total_regions = len(sv.regions)
+    region_ids = list(range(total_regions))
 
-    Returns:
-        Tuple[float, float]: Longitude and latitude of a point.
-    """
-    min_lon, min_lat, max_lon, max_lat = bbox
+    generated_regions: List[MultiPolygon]
 
-    # round imperfections
-    lon = round(lon, 8)
-    lat = round(lat, 8)
+    if num_of_multiprocessing_workers > 1 and total_regions >= multiprocessing_activation_threshold:
+        generated_regions = process_map(
+            create_regions_func,
+            region_ids,
+            desc="Generating regions",
+            max_workers=num_of_multiprocessing_workers,
+            chunksize=ceil(total_regions / (4 * num_of_multiprocessing_workers)),
+        )
+    else:
+        generated_regions = [
+            create_regions_func(region_id=region_id)
+            for region_id in tqdm(region_ids, desc="Generating regions")
+        ]
 
-    # switch signs
-    if lon and abs(lon) == abs(min_lon):
-        lon = min_lon
-    elif lon and abs(lon) == abs(max_lon):
-        lon = max_lon
-    if lat and abs(lat) == abs(min_lat):
-        lat = min_lat
-    elif lat and abs(lat) == abs(max_lat):
-        lat = max_lat
+    return generated_regions
 
-    return lon, lat
 
+def _parse_num_of_multiprocessing_workers(num_of_multiprocessing_workers: int) -> int:
+    if num_of_multiprocessing_workers == 0:
+        num_of_multiprocessing_workers = 1
+    elif num_of_multiprocessing_workers < 0:
+        num_of_multiprocessing_workers = cpu_count()
 
-def _create_polygon(
-    spherical_polygon_points: npt.NDArray[np.float32],
-    bbox: Polygon,
-    se: SphereEllipsoid,
-    max_step: int,
-) -> Polygon:
-    """
-    Map polygon from a sphere to Shapely polygon.
+    return num_of_multiprocessing_workers
+
+
+def _parse_multiprocessing_activation_threshold(
+    multiprocessing_activation_threshold: Optional[int],
+) -> int:
+    if not multiprocessing_activation_threshold:
+        multiprocessing_activation_threshold = 100
+
+    return multiprocessing_activation_threshold
+
+
+def _generate_seeds(gdf: gpd.GeoDataFrame) -> Tuple[List[Point], List[Hashable]]:
+    """Transform GeoDataFrame into list of Points with index."""
+    seeds_wgs84 = gdf.to_crs(crs=WGS84_CRS)
+    region_ids: List[Hashable] = []
+    seeds: List[Point] = []
+
+    for index, row in seeds_wgs84.iterrows():
+        candidate_point = row.geometry.centroid
+        if not candidate_point.is_empty:
+            region_ids.append(index)
+            seeds.append(candidate_point)
+
+    return seeds, region_ids
+
+
+def _get_duplicated_seeds_ids(seeds: List[Point], region_ids: List[Hashable]) -> List[Hashable]:
+    """Return all seeds ids that overlap with another using quick sjoin operation."""
+    gdf = gpd.GeoDataFrame(data={"geometry": seeds}, index=region_ids, crs=WGS84_CRS)
+    duplicated_seeds = gdf.sjoin(gdf).index.value_counts().loc[lambda x: x > 1]
+    duplicated_seeds_ids: List[Hashable] = duplicated_seeds.index.to_list()
+    return duplicated_seeds_ids
+
+
+def _check_if_in_bounds(seeds: List[Point]) -> bool:
+    """Check if all seeds are within bounds."""
+    wgs84_earth_bbox = (box(minx=-180, miny=-90, maxx=180, maxy=90),)
+    return all(point.covered_by(wgs84_earth_bbox) for point in seeds)
 
-    Function maps and interpolates points from a sphere
-    into a wgs84 crs while keeping integrity across all coordinates.
+
+def _map_to_geocentric(lon: float, lat: float, ell: Ellipsoid) -> Tuple[float, float, float]:
+    """
+    Wrapper for a geodetic2ecef function from pymap3d library.
 
     Args:
-        spherical_polygon_points (npt.NDArray): List of spherical points.
-        bbox (Polygon): Current sphere octant bounding box.
-        se (SphereEllipsoid): SphereEllipsoid object.
-        max_step (int): Max step between interpolated points on an arc.
+        lon (float): longitude of a point in a wgs84 crs.
+        lat (float): latitude of a point in a wgs84 crs.
+        ell (Ellipsoid): an ellipsoid.
 
     Returns:
-        Polygon: Mapped polygon in wgs84 crs.
+        Tuple[float, float, float]: (x, y, z) coordinates tuple.
     """
-    polygon_points = []
-    prev_lon = None
-    prev_lat = None
-    n = len(spherical_polygon_points)
-    bbox_bounds = bbox.bounds
-    for i in range(n):
-        start = spherical_polygon_points[i]
-        end = spherical_polygon_points[(i + 1) % n]
-        start_lon, start_lat = map_from_geocentric(start[0], start[1], start[2], se)
-        end_lon, end_lat = map_from_geocentric(end[0], end[1], end[2], se)
-        haversine_distance = haversine((start_lat, start_lon), (end_lat, end_lon), unit="m")
-        steps = ceil(haversine_distance / max_step)
-        t_vals = np.linspace(0, 1, steps)
-        for pt in geometric_slerp(start, end, t_vals):
-            lon, lat = map_from_geocentric(pt[0], pt[1], pt[2], se)
-            lon, lat = _fix_lat_lon(lon, lat, bbox_bounds)
-            if prev_lon is not None and abs(prev_lon - lon) >= 90:
-                sign = 1 if lat > 0 else -1
-                max_lat = sign * max(abs(prev_lat), abs(lat))
-                if polygon_points[-1] != (prev_lon, max_lat):
-                    polygon_points.append((prev_lon, max_lat))
-                if polygon_points[-1] != (lon, lat):
-                    polygon_points.append((lon, max_lat))
-            polygon_points.append((lon, lat))
-            prev_lon = lon
-            prev_lat = lat
-
-    polygon = Polygon(polygon_points)
-    polygon = polygon.intersection(bbox)
-    return polygon
+    x, y, z = geodetic2ecef(lat, lon, 0, ell=ell)
+    return x, y, z
 
 
 def _create_region(
-    region_id: int, sv: SphericalVoronoi, se: SphereEllipsoid, max_meters_between_points: int
+    region_id: int,
+    sv: SphericalVoronoi,
+    ell: Ellipsoid,
+    max_meters_between_points: int,
 ) -> MultiPolygon:
     """
     Parse spherical region into a WGS84 MultiPolygon.
 
     Args:
         region_id (int): Index of region in SphericalVoronoi result.
         sv (SphericalVoronoi): SphericalVoronoi object.
-        se (SphereEllipsoid): SphereEllipsoid object.
+        ell (Ellipsoid): Ellipsoid object.
         max_meters_between_points (int): maximal distance between points
             during interpolation of two vertices on a sphere.
 
     Returns:
         MultiPolygon: Parsed region in WGS84 coordinates.
     """
     region = sv.regions[region_id]
@@ -231,92 +261,166 @@
 
     multi_polygon_parts: List[Polygon] = []
     for sphere_intersection_part, bbox in sphere_intersection_parts:
         for spherical_polygon_points in sphere_intersection_part.points:
             polygon = _create_polygon(
                 spherical_polygon_points=spherical_polygon_points,
                 bbox=bbox,
-                se=se,
+                ell=ell,
                 max_step=max_meters_between_points,
             )
-            multi_polygon_parts.append(polygon)
+            if isinstance(polygon, Polygon):
+                multi_polygon_parts.append(polygon)
+            elif isinstance(polygon, MultiPolygon):
+                multi_polygon_parts.extend(polygon.geoms)
+            elif isinstance(polygon, (LineString, MultiLineString, Point)):
+                pass
+            else:
+                raise RuntimeError(str(type(polygon)))
 
     multi_polygon = MultiPolygon(multi_polygon_parts)
     return multi_polygon
 
 
-def generate_voronoi_regions(
-    seeds: List[Point],
-    max_meters_between_points: int,
-    num_of_multiprocessing_workers: int = -1,
-    multiprocessing_activation_threshold: Optional[int] = None,
-) -> List[MultiPolygon]:
+def _create_polygon(
+    spherical_polygon_points: npt.NDArray[np.float32],
+    bbox: Polygon,
+    ell: Ellipsoid,
+    max_step: int,
+) -> Polygon:
     """
-    Generate Thessien polygons for a given list of seeds.
+    Map polygon from a sphere to Shapely polygon.
 
-    Function generates Thessien polygons on a sphere using
-    SphericalVoronoi algorithm from scipy library.
+    Function maps and interpolates points from a sphere
+    into a wgs84 crs while keeping integrity across all coordinates.
 
     Args:
-        seeds (List[Point]): List of seeds used for generating regions.
-        max_meters_between_points (int): maximal distance between points
-            during interpolation of two vertices on a sphere.
-        num_of_multiprocessing_workers (int): Number of workers used for multiprocessing.
-            Defaults to -1 which results in a total number of available cpu threads.
-            `0` and `1` values disable multiprocessing.
-            Similar to `n_jobs` parameter from `scikit-learn` library.
-        multiprocessing_activation_threshold (int, optional): Number of seeds required to start
-            processing on multiple processes. Activating multiprocessing for a small
-            amount of points might not be feasible. Defaults to 100.
+        spherical_polygon_points (npt.NDArray): List of spherical points.
+        bbox (Polygon): Current sphere octant bounding box.
+        ell (Ellipsoid): Ellipsoid object.
+        max_step (int): Max step between interpolated points on an arc.
 
     Returns:
-        List[MultiPolygon]: List of regions cut into up to 8 polygons based
-        on 8 parts of a sphere.
+        Polygon: Mapped polygon in wgs84 crs.
+    """
+    polygon_points: List[Tuple[float, float]] = []
 
-    Raises:
-        ValueError: If less than 4 seeds are provided.
+    n = len(spherical_polygon_points)
+    bbox_bounds = bbox.bounds
+    for i in range(n):
+        start = spherical_polygon_points[i]
+        end = spherical_polygon_points[(i + 1) % n]
+        start_lon, start_lat = _map_from_geocentric(start[0], start[1], start[2], ell)
+        end_lon, end_lat = _map_from_geocentric(end[0], end[1], end[2], ell)
+        haversine_distance = haversine((start_lat, start_lon), (end_lat, end_lon), unit="m")
+        steps = ceil(haversine_distance / max_step)
+        t_vals = np.linspace(0, 1, steps)
+
+        reverse_slerp = end_lat > start_lat or (start_lat == end_lat and end_lon > start_lon)
+        if reverse_slerp:
+            start, end = end, start
+
+        edge_points = _interpolate_edge(
+            start_point=start, end_point=end, step_ticks=t_vals, ell=ell, bbox_bounds=bbox_bounds
+        )
+
+        polygon_points.extend(edge_points if not reverse_slerp else reversed(edge_points))
+
+    polygon = Polygon(polygon_points)
+    polygon = make_valid(polygon)
+    polygon = polygon.intersection(bbox)
+    if isinstance(polygon, GeometryCollection):
+        for geometry in polygon.geoms:
+            if isinstance(geometry, (Polygon, MultiPolygon)):
+                polygon = geometry
+                break
+        else:
+            raise RuntimeError(
+                f"Intersection with a quadrant did not produce any Polygon. ({polygon})"
+            )
+
+    return polygon
+
+
+def _interpolate_edge(
+    start_point: Tuple[float, float],
+    end_point: Tuple[float, float],
+    step_ticks: List[float],
+    ell: Ellipsoid,
+    bbox_bounds: Tuple[float, float, float, float],
+) -> List[Tuple[float, float]]:
+    edge_points: List[Tuple[float, float]] = []
+
+    prev_lon = None
+    prev_lat = None
+
+    for pt in geometric_slerp(start_point, end_point, step_ticks, tol=SCIPY_THRESHOLD):
+        lon, lat = _map_from_geocentric(pt[0], pt[1], pt[2], ell)
+        lon, lat = _fix_lat_lon(lon, lat, bbox_bounds)
+        if prev_lon is not None and abs(prev_lon - lon) >= 90:
+            sign = 1 if lat > 0 else -1
+            max_lat = sign * max(abs(prev_lat), abs(lat))
+            if edge_points[-1] != (prev_lon, max_lat):
+                edge_points.append((prev_lon, max_lat))
+            if edge_points[-1] != (lon, lat):
+                edge_points.append((lon, max_lat))
+        edge_points.append((lon, lat))
+        prev_lon = lon
+        prev_lat = lat
+
+    return edge_points
+
+
+def _map_from_geocentric(x: float, y: float, z: float, ell: Ellipsoid) -> Tuple[float, float]:
     """
-    if len(seeds) < 4:
-        raise ValueError("Minimum 4 seeds are required.")
+    Wrapper for a ecef2geodetic function from pymap3d library.
 
-    if num_of_multiprocessing_workers == 0:
-        num_of_multiprocessing_workers = 1
-    elif num_of_multiprocessing_workers < 0:
-        num_of_multiprocessing_workers = cpu_count()
+    Args:
+        x (float): X cartesian coordinate.
+        y (float): Y cartesian coordinate.
+        z (float): Z cartesian coordinate.
+        ell (Ellipsoid): an ellipsoid.
 
-    if not multiprocessing_activation_threshold:
-        multiprocessing_activation_threshold = 100
+    Returns:
+        Tuple[float, float]: longitude and latitude coordinates in a wgs84 crs.
+    """
+    lat, lon, _ = ecef2geodetic(x, y, z, ell=ell)
+    return lon, lat
 
-    se = SphereEllipsoid()
-    mapped_points = [map_to_geocentric(pt.x, pt.y, se) for pt in seeds]
-    sphere_points = np.array([[pt[0], pt[1], pt[2]] for pt in mapped_points])
 
-    radius = 1
-    center = np.array([0, 0, 0])
-    sv = SphericalVoronoi(sphere_points, radius, center, threshold=1e-8)
-    sv.sort_vertices_of_regions()
+def _fix_lat_lon(
+    lon: float,
+    lat: float,
+    bbox: Tuple[float, float, float, float],
+) -> Tuple[float, float]:
+    """
+    Fix point signs and rounding.
 
-    create_regions_func = partial(
-        _create_region, sv=sv, se=se, max_meters_between_points=max_meters_between_points
-    )
+    Rounds latitude and longitude to 8 decimal places.
+    Checks if any point is on a boundary and flips its sign
+    to ensure validity of a polygon.
 
-    total_regions = len(sv.regions)
-    region_ids = list(range(total_regions))
+    Args:
+        lon (float): Longitude of a point.
+        lat (float): Latitude of a point.
+        bbox (Tuple[float, float, float, float]): Current sphere octant bounding box.
 
-    generated_regions: List[MultiPolygon] = []
-    if num_of_multiprocessing_workers > 1 and total_regions >= multiprocessing_activation_threshold:
-        generated_regions.extend(
-            process_map(
-                create_regions_func,
-                region_ids,
-                desc="Generating regions",
-                max_workers=num_of_multiprocessing_workers,
-                chunksize=ceil(total_regions / (4 * num_of_multiprocessing_workers)),
-            )
-        )
-    else:
-        generated_regions.extend(
-            create_regions_func(region_id=region_id)
-            for region_id in tqdm(region_ids, desc="Generating regions")
-        )
+    Returns:
+        Tuple[float, float]: Longitude and latitude of a point.
+    """
+    min_lon, min_lat, max_lon, max_lat = bbox
 
-    return generated_regions
+    # round imperfections
+    lon = round(lon, 8)
+    lat = round(lat, 8)
+
+    # switch signs
+    if lon and abs(lon) == abs(min_lon):
+        lon = min_lon
+    elif lon and abs(lon) == abs(max_lon):
+        lon = max_lon
+    if lat and abs(lat) == abs(min_lat):
+        lat = min_lat
+    elif lat and abs(lat) == abs(max_lat):
+        lat = max_lat
+
+    return lon, lat
```

### Comparing `srai-0.2.0/srai/regionalizers/administrative_boundary_regionalizer.py` & `srai-0.3.0/srai/regionalizers/administrative_boundary_regionalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """
 Administrative Boundary Regionalizer.
 
 This module contains administrative boundary regionalizer implementation.
 """
+import hashlib
+import json
 import time
+from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 import geopandas as gpd
 import topojson as tp
 from shapely.geometry import MultiPolygon, Point, Polygon
 from shapely.geometry.base import BaseGeometry
 from shapely.ops import unary_union
 from shapely.validation import make_valid
 from tqdm import tqdm
 
+from srai._optional import import_optional_dependencies
 from srai.constants import GEOMETRY_COLUMN, REGIONS_INDEX, WGS84_CRS
+from srai.geometry import flatten_geometry_series
 from srai.regionalizers import Regionalizer
-from srai.utils import flatten_geometry_series
-from srai.utils._optional import import_optional_dependencies
 
 
 class AdministrativeBoundaryRegionalizer(Regionalizer):
     """
     AdministrativeBoundaryRegionalizer.
 
     Administrative boundary regionalizer allows the given geometries to be divided
@@ -143,18 +146,16 @@
 
         regions_dicts = self._generate_regions_from_all_geometries(gdf_wgs84)
 
         if not regions_dicts:
             import warnings
 
             warnings.warn(
-                (
-                    "Couldn't find any administrative boundaries with"
-                    f" `admin_level`={self.admin_level}."
-                ),
+                "Couldn't find any administrative boundaries with"
+                f" `admin_level`={self.admin_level}.",
                 RuntimeWarning,
                 stacklevel=2,
             )
 
             return self._get_empty_geodataframe(gdf_wgs84)
 
         regions_gdf = gpd.GeoDataFrame(data=regions_dicts, crs=WGS84_CRS).set_index(REGIONS_INDEX)
@@ -214,42 +215,44 @@
 
         return generated_regions
 
     def _query_overpass(self, query: str) -> List[Dict[str, Any]]:
         """
         Query Overpass and catch exceptions.
 
-        Since `overpass` library doesn't have useful http error wrapping like `osmnx` does [1],
-        this method allows for retry after waiting some time. Additionally, caching mechanism
-        uses `osmnx` internal methods built for this purpose.
+        This method allows for retry after waiting some time, and caches the response.
 
         Args:
             query (str): Overpass query.
 
         Raises:
             ex: If exception is different than urllib.request.HTTPError or
                 HTTP code is different than 429 or 504.
 
         Returns:
             List[Dict[str, Any]]: Query elements result from Overpass.
-
-        References:
-            1. https://github.com/gboeing/osmnx/blob/main/osmnx/downloader.py#L712
         """
-        from osmnx.downloader import _retrieve_from_cache, _save_to_cache
         from overpass import MultipleRequestsError, ServerLoadError
 
+        h = hashlib.new("sha256")
+        h.update(query.encode())
+        query_hash = h.hexdigest()
+        query_file_path = Path("cache").resolve() / f"{query_hash}.json"
+
         while True:
             try:
-                query_result = _retrieve_from_cache(url=query, check_remark=False)
-                if query_result is None:
+                if not query_file_path.exists():
                     query_result = self.overpass_api.get(
                         query, verbosity="ids tags", responseformat="json"
                     )
-                    _save_to_cache(url=query, response_json=query_result, sc=200)
+                    query_file_path.parent.mkdir(parents=True, exist_ok=True)
+                    query_file_path.write_text(json.dumps(query_result))
+                else:
+                    query_result = json.loads(query_file_path.read_text())
+
                 elements: List[Dict[str, Any]] = query_result["elements"]
                 return elements
             except (MultipleRequestsError, ServerLoadError):
                 time.sleep(60)
 
     def _generate_query_for_single_geometry(self, g: BaseGeometry) -> str:
         """Generate Overpass query for a geometry."""
```

### Comparing `srai-0.2.0/srai/regionalizers/s2_regionalizer.py` & `srai-0.3.0/srai/regionalizers/s2_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/regionalizers/slippy_map_regionalizer.py` & `srai-0.3.0/srai/regionalizers/slippy_map_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/regionalizers/voronoi_regionalizer.py` & `srai-0.3.0/srai/regionalizers/voronoi_regionalizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Voronoi Regionalizer.
 
 This module contains voronoi regionalizer implementation.
 """
 
-from typing import Hashable, List, Optional
+from typing import Hashable, List, Optional, Union
 
 import geopandas as gpd
 from shapely.geometry import Point, box
 
+from srai._optional import import_optional_dependencies
 from srai.constants import GEOMETRY_COLUMN, REGIONS_INDEX, WGS84_CRS
 from srai.regionalizers import Regionalizer
-from srai.utils._optional import import_optional_dependencies
 
 
 class VoronoiRegionalizer(Regionalizer):
     """
     VoronoiRegionalizer.
 
     Voronoi [1] regionalizer allows the given geometries to be divided
@@ -26,29 +26,30 @@
     References:
         1. https://en.wikipedia.org/wiki/Voronoi_diagram
         2. https://docs.scipy.org/doc/scipy-1.9.2/reference/generated/scipy.spatial.SphericalVoronoi.html
     """  # noqa: W505, E501
 
     def __init__(
         self,
-        seeds: gpd.GeoDataFrame,
+        seeds: Union[gpd.GeoDataFrame, List[Point]],
         max_meters_between_points: int = 10_000,
         num_of_multiprocessing_workers: int = -1,
         multiprocessing_activation_threshold: Optional[int] = None,
     ) -> None:
         """
         Init VoronoiRegionalizer.
 
         All (multi)polygons from seeds GeoDataFrame will be transformed to their centroids,
         because scipy function requires only points as an input.
 
         Args:
-            seeds (gpd.GeoDataFrame): GeoDataFrame with seeds for
-                creating a tessellation. Minimum 4 seeds are required.
-                Seeds cannot lie on a single arc. Empty seeds will be removed.
+            seeds (Union[gpd.GeoDataFrame, List[Point]]): List of points or a GeoDataFrame
+                with seeds for creating a tessellation. Every non-point geometry will be mapped
+                to a centroid. Minimum 4 seeds are required. Seeds cannot lie on a single arc.
+                Empty seeds will be removed.
             max_meters_between_points (int): Maximal distance in meters between two points
                 in a resulting polygon. Higher number results lower resolution of a polygon.
             num_of_multiprocessing_workers (int): Number of workers used for
                 multiprocessing. Defaults to `-1` which results in a total number of available
                 cpu threads. `0` and `1` values disable multiprocessing.
                 Similar to `n_jobs` parameter from `scikit-learn` library.
             multiprocessing_activation_threshold (int, optional): Number of seeds required to start
@@ -57,27 +58,29 @@
 
         Raises:
             ValueError: If any seed is duplicated.
             ValueError: If less than 4 seeds are provided.
             ValueError: If provided seeds geodataframe has no crs defined.
         """
         import_optional_dependencies(
-            dependency_group="voronoi", modules=["haversine", "pymap3d", "spherical_geometry"]
+            dependency_group="voronoi",
+            modules=["haversine", "pymap3d", "scipy", "spherical_geometry"],
         )
-        seeds_wgs84 = seeds.to_crs(crs=WGS84_CRS)
         self.region_ids: List[Hashable] = []
         self.seeds: List[Point] = []
+
+        if isinstance(seeds, gpd.GeoDataFrame):
+            self._parse_geodataframe_seeds(seeds_gdf=seeds)
+        else:
+            self.seeds = seeds
+            self.region_ids = list(range(len(seeds)))
+
         self.max_meters_between_points = max_meters_between_points
         self.num_of_multiprocessing_workers = num_of_multiprocessing_workers
         self.multiprocessing_activation_threshold = multiprocessing_activation_threshold
-        for index, row in seeds_wgs84.iterrows():
-            candidate_point = row.geometry.centroid
-            if not candidate_point.is_empty:
-                self.region_ids.append(index)
-                self.seeds.append(candidate_point)
 
         if len(self.seeds) < 4:
             raise ValueError("Minimum 4 seeds are required.")
 
         duplicated_seeds_ids = self._get_duplicated_seeds_ids()
         if duplicated_seeds_ids:
             raise ValueError(f"Duplicate seeds present: {duplicated_seeds_ids}.")
@@ -120,14 +123,22 @@
         regions_gdf = gpd.GeoDataFrame(
             data={GEOMETRY_COLUMN: generated_regions}, index=self.region_ids, crs=WGS84_CRS
         )
         regions_gdf.index.rename(REGIONS_INDEX, inplace=True)
         clipped_regions_gdf = regions_gdf.clip(mask=gdf_wgs84, keep_geom_type=False)
         return clipped_regions_gdf
 
+    def _parse_geodataframe_seeds(self, seeds_gdf: gpd.GeoDataFrame) -> None:
+        seeds_wgs84 = seeds_gdf.to_crs(crs=WGS84_CRS)
+        for index, row in seeds_wgs84.iterrows():
+            candidate_point = row.geometry.centroid
+            if not candidate_point.is_empty:
+                self.region_ids.append(index)
+                self.seeds.append(candidate_point)
+
     def _get_duplicated_seeds_ids(self) -> List[Hashable]:
         """Return all seeds ids that overlap with another using quick sjoin operation."""
         gdf = gpd.GeoDataFrame(
             data={GEOMETRY_COLUMN: self.seeds}, index=self.region_ids, crs=WGS84_CRS
         )
         duplicated_seeds = gdf.sjoin(gdf).index.value_counts().loc[lambda x: x > 1]
         duplicated_seeds_ids: List[Hashable] = duplicated_seeds.index.to_list()
```

### Comparing `srai-0.2.0/srai/utils/_optional.py` & `srai-0.3.0/srai/_optional.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/utils/download.py` & `srai-0.3.0/srai/loaders/download.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/utils/geocode.py` & `srai-0.3.0/srai/regionalizers/geocode.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/srai/utils/geometry.py` & `srai-0.3.0/srai/geometry.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Utility geometry operations functions."""
-from typing import List
+from typing import List, Union
 
 import geopandas as gpd
 import pyproj
 from functional import seq
-from shapely.geometry import Polygon
+from shapely.geometry import MultiPolygon, Polygon
 from shapely.geometry.base import BaseGeometry, BaseMultipartGeometry
 from shapely.ops import transform as shapely_transform
 
 
 def flatten_geometry_series(geometry_series: gpd.GeoSeries) -> List[BaseGeometry]:
     """Flatten all geometries from a series into a list of BaseGeometries."""
     geometries: List[BaseGeometry] = (
@@ -67,7 +67,43 @@
     wgs84_to_aeqd = pyproj.Transformer.from_proj(wgs84_proj, aeqd_proj, always_xy=True).transform
     aeqd_to_wgs84 = pyproj.Transformer.from_proj(aeqd_proj, wgs84_proj, always_xy=True).transform
 
     projected_geometry = shapely_transform(wgs84_to_aeqd, geometry)
     bufferred_projected_geometry = projected_geometry.buffer(meters)
 
     return shapely_transform(aeqd_to_wgs84, bufferred_projected_geometry)
+
+
+def merge_disjointed_polygons(polygons: List[Union[Polygon, MultiPolygon]]) -> MultiPolygon:
+    """
+    Merges all polygons into a single MultiPolygon.
+
+    Input polygons are expected to be disjointed.
+
+    Args:
+        polygons (List[Union[Polygon, MultiPolygon]]): List of polygons to merge
+
+    Returns:
+        MultiPolygon: Merged polygon
+    """
+    single_polygons = []
+    for geom in polygons:
+        if isinstance(geom, Polygon):
+            single_polygons.append(geom)
+        else:
+            single_polygons.extend(geom.geoms)
+    return MultiPolygon(single_polygons)
+
+
+def merge_disjointed_gdf_geometries(gdf: gpd.GeoDataFrame) -> MultiPolygon:
+    """
+    Merges geometries from a GeoDataFrame into a single MultiPolygon.
+
+    Input geometries are expected to be disjointed.
+
+    Args:
+        gdf (gpd.GeoDataFrame): GeoDataFrame with geometries to merge.
+
+    Returns:
+        MultiPolygon: Merged polygon
+    """
+    return merge_disjointed_polygons(list(gdf.geometry))
```

### Comparing `srai-0.2.0/srai/utils/typing.py` & `srai-0.3.0/srai/_typing.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/conftest.py` & `srai-0.3.0/tests/embedders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/hex2vec/constants.py` & `srai-0.3.0/tests/embedders/hex2vec/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/hex2vec/generation.py` & `srai-0.3.0/tests/embedders/hex2vec/generation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 """Test case generation for Hex2VecEmbedder."""
 from pathlib import Path
 from typing import Optional
 
 import geopandas as gpd
+import h3
+from h3ronpy.pandas.vector import cells_to_polygons
 from pytorch_lightning import seed_everything
 
-from srai.constants import WGS84_CRS
+from srai.constants import REGIONS_INDEX, WGS84_CRS
 from srai.embedders.hex2vec.embedder import Hex2VecEmbedder
 from srai.joiners import IntersectionJoiner
 from srai.loaders.osm_loaders import OSMPbfLoader
-from srai.loaders.osm_loaders.filters import osm_tags_type
+from srai.loaders.osm_loaders.filters import OsmTagsFilter
 from srai.neighbourhoods import H3Neighbourhood
-from srai.regionalizers import H3Regionalizer
-from srai.utils import geocode_to_region_gdf
+from srai.regionalizers import geocode_to_region_gdf
 from tests.embedders.hex2vec.constants import ENCODER_SIZES, TRAINER_KWARGS
 
 
 def generate_test_case(
     test_case_name: str,
     geocoding_name: str,
     root_region_index: str,
     h3_res: int,
     radius: int,
     seed: int,
-    tags: Optional[osm_tags_type] = None,
+    tags: Optional[OsmTagsFilter] = None,
 ) -> None:
     """Generate test case for Hex2VecEmbedder."""
     if tags is None:
         tags = {"leisure": "park", "amenity": "restaurant"}
     neighbourhood = H3Neighbourhood()
     regions_indexes = neighbourhood.get_neighbours_up_to_distance(root_region_index, radius)
     regions_indexes.add(root_region_index)
     regions_indexes = list(regions_indexes)  # type: ignore
-    regionalizer = H3Regionalizer(h3_res)
 
-    geoms = [regionalizer._h3_index_to_shapely_polygon(r) for r in regions_indexes]
+    geoms = cells_to_polygons([h3.str_to_int(r) for r in regions_indexes]).values
     regions_gdf = gpd.GeoDataFrame(index=regions_indexes, geometry=geoms, crs=WGS84_CRS)
-    regions_gdf.index.name = "region_id"
+    regions_gdf.index.name = REGIONS_INDEX
 
     area_gdf = geocode_to_region_gdf(geocoding_name)
     loader = OSMPbfLoader()
     features_all = loader.load(area_gdf, tags=tags)
 
     joiner = IntersectionJoiner()
     joint_gdf = joiner.transform(regions_gdf, features_all)
```

### Comparing `srai-0.2.0/tests/embedders/hex2vec/test_embedder.py` & `srai-0.3.0/tests/embedders/hex2vec/test_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/hex2vec/test_files/poz_8_features.parquet` & `srai-0.3.0/tests/embedders/hex2vec/test_files/poz_8_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/hex2vec/test_files/poz_8_joint.parquet` & `srai-0.3.0/tests/embedders/hex2vec/test_files/poz_8_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/hex2vec/test_files/poz_8_regions.parquet` & `srai-0.3.0/tests/embedders/hex2vec/test_files/poz_8_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/hex2vec/test_files/poz_8_result.parquet` & `srai-0.3.0/tests/embedders/hex2vec/test_files/poz_8_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/hex2vec/test_files/wro_9_features.parquet` & `srai-0.3.0/tests/embedders/hex2vec/test_files/wro_9_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/hex2vec/test_files/wro_9_joint.parquet` & `srai-0.3.0/tests/embedders/hex2vec/test_files/wro_9_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/hex2vec/test_files/wro_9_regions.parquet` & `srai-0.3.0/tests/embedders/hex2vec/test_files/wro_9_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/hex2vec/test_files/wro_9_result.parquet` & `srai-0.3.0/tests/embedders/hex2vec/test_files/wro_9_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/hex2vec/test_model.py` & `srai-0.3.0/tests/embedders/hex2vec/test_model.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/hex2vec/test_neighbour_dataset.py` & `srai-0.3.0/tests/embedders/hex2vec/test_neighbour_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/test_contextual_count_embedder.py` & `srai-0.3.0/tests/embedders/test_contextual_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/test_count_embedder.py` & `srai-0.3.0/tests/embedders/test_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/test_gtfs2vec_embedder.py` & `srai-0.3.0/tests/embedders/test_gtfs2vec_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/embedders/test_highway2vec_embedder.py` & `srai-0.3.0/tests/embedders/test_highway2vec_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/joiners/conftest.py` & `srai-0.3.0/tests/joiners/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/joiners/test_intersection_joiner.py` & `srai-0.3.0/tests/joiners/test_intersection_joiner.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/loaders/conftest.py` & `srai-0.3.0/tests/loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/loaders/osm_loaders/conftest.py` & `srai-0.3.0/tests/loaders/osm_loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/loaders/osm_loaders/filters/popular_filter_example.json` & `srai-0.3.0/tests/loaders/osm_loaders/filters/popular_filter_example.json`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/loaders/osm_loaders/filters/test_merge_filter_types.py` & `srai-0.3.0/tests/loaders/osm_loaders/filters/test_merge_filter_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 """Tests for merging OSM Loaders filters."""
 from contextlib import nullcontext as does_not_raise
 from typing import Any
 from unittest import TestCase
 
 import pytest
 
-from srai.loaders.osm_loaders.filters._typing import (
-    merge_grouped_osm_tags_type,
-    osm_tags_type,
-)
+from srai.loaders.osm_loaders.filters import OsmTagsFilter, merge_grouped_osm_tags_filter
 
 ut = TestCase()
 
 
 @pytest.mark.parametrize(  # type: ignore
     "grouped_filter,expected_result_filter,expectation",
     [
@@ -89,13 +86,13 @@
             },
             {"tag_a": ["A", "C", "D"], "tag_b": ["B", "E"]},
             does_not_raise(),
         ),
     ],
 )
 def test_merge_grouped_filters(
-    grouped_filter: Any, expected_result_filter: osm_tags_type, expectation: Any
+    grouped_filter: Any, expected_result_filter: OsmTagsFilter, expectation: Any
 ) -> None:
     """Test merging grouped tags filter into a base osm filter."""
     with expectation:
-        merged_filters = merge_grouped_osm_tags_type(grouped_filter)
+        merged_filters = merge_grouped_osm_tags_filter(grouped_filter)
         ut.assertDictEqual(expected_result_filter, merged_filters)
```

### Comparing `srai-0.2.0/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py` & `srai-0.3.0/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf` & `srai-0.3.0/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf` & `srai-0.3.0/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf` & `srai-0.3.0/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/loaders/osm_loaders/test_files/poland.geojson` & `srai-0.3.0/tests/loaders/osm_loaders/test_files/poland.geojson`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson` & `srai-0.3.0/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/loaders/osm_loaders/test_osm_online_loader.py` & `srai-0.3.0/tests/loaders/osm_loaders/test_osm_online_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 
 import geopandas as gpd
 import pytest
 from pandas.testing import assert_frame_equal
 
 from srai.constants import WGS84_CRS
 from srai.loaders.osm_loaders import OSMOnlineLoader
-from srai.loaders.osm_loaders.filters._typing import osm_tags_type
+from srai.loaders.osm_loaders.filters import OsmTagsFilter
 
 if TYPE_CHECKING:
     from shapely.geometry import Polygon
 
 
 @pytest.fixture  # type: ignore
 def mock_osmnx(
     mocker, two_polygons_area_gdf, area_with_no_objects_gdf, amenities_gdf, building_gdf
 ):
     """Patch `ox.geometries_from_polygon` to return data from predefined gdfs."""
     gdfs = {"amenity": amenities_gdf, "building": building_gdf}
     polygon_1, polygon_2 = two_polygons_area_gdf["geometry"]
     empty_polygon = area_with_no_objects_gdf["geometry"][0]
 
-    def mock_geometries_from_polygon(polygon: "Polygon", tags: osm_tags_type) -> gpd.GeoDataFrame:
+    def mock_geometries_from_polygon(polygon: "Polygon", tags: OsmTagsFilter) -> gpd.GeoDataFrame:
         tag_key, tag_value = list(tags.items())[0]
         gdf = gdfs[tag_key]
         if tag_value is True:
             tag_res = gdf
         else:
             tag_res = gdf.loc[gdf[tag_key] == tag_value]
         if tag_res.empty:
@@ -62,15 +62,15 @@
             {"amenity": ["restaurant", "bar"], "building": True},
             "empty_result_gdf",
         ),
     ],
 )
 def test_osm_online_loader(
     area_gdf_fixture: str,
-    query: osm_tags_type,
+    query: OsmTagsFilter,
     expected_result_gdf_fixture: str,
     request: Any,
 ):
     """Test `OSMOnlineLoader.load()`."""
     _ = request.getfixturevalue("mock_osmnx")
     area_gdf = request.getfixturevalue(area_gdf_fixture)
     expected_result_gdf = request.getfixturevalue(expected_result_gdf_fixture)
```

### Comparing `srai-0.2.0/tests/loaders/osm_loaders/test_osm_pbf_loader.py` & `srai-0.3.0/tests/loaders/osm_loaders/test_osm_pbf_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,20 @@
 import geopandas as gpd
 import pytest
 from shapely.geometry import MultiPolygon, Point, Polygon
 from shapely.geometry.base import BaseGeometry
 
 from srai.constants import REGIONS_INDEX, WGS84_CRS
 from srai.loaders.osm_loaders import OSMPbfLoader
-from srai.loaders.osm_loaders.filters import BASE_OSM_GROUPS_FILTER, HEX2VEC_FILTER
-from srai.loaders.osm_loaders.filters._typing import grouped_osm_tags_type, osm_tags_type
+from srai.loaders.osm_loaders.filters import (
+    BASE_OSM_GROUPS_FILTER,
+    HEX2VEC_FILTER,
+    GroupedOsmTagsFilter,
+    OsmTagsFilter,
+)
 from srai.loaders.osm_loaders.pbf_file_downloader import PbfFileDownloader
 from srai.loaders.osm_loaders.pbf_file_handler import PbfFileHandler
 
 
 @pytest.mark.parametrize(  # type: ignore
     "test_polygon",
     [
@@ -161,15 +165,15 @@
             0,
             0,
         ),
     ],
 )
 def test_pbf_handler(
     test_file_name: str,
-    query: osm_tags_type,
+    query: OsmTagsFilter,
     expected_result_length: int,
     expected_features_columns_length: int,
 ):
     """Test proper files loading in `PbfFileHandler`."""
     handler = PbfFileHandler(tags=query)
     features_gdf = handler.get_features_gdf(
         file_paths=[Path(__file__).parent / "test_files" / test_file_name]
@@ -234,15 +238,15 @@
             0,
         ),
     ],
 )
 def test_osm_pbf_loader(
     test_geometries: List[BaseGeometry],
     pbf_file: Path,
-    query: Union[osm_tags_type, grouped_osm_tags_type],
+    query: Union[OsmTagsFilter, GroupedOsmTagsFilter],
     expected_result_length: int,
     expected_features_columns_length: int,
 ):
     """Test `OSMPbfLoader.load()`."""
     download_directory = Path(__file__).parent / "test_files"
     area = gpd.GeoDataFrame(
         geometry=test_geometries,
```

### Comparing `srai-0.2.0/tests/loaders/osm_loaders/test_osm_tile_data_collector.py` & `srai-0.3.0/tests/loaders/osm_loaders/test_osm_tile_data_collector.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/loaders/osm_loaders/test_osm_tile_loader.py` & `srai-0.3.0/tests/loaders/osm_loaders/test_osm_tile_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/loaders/osm_way_loader/files/1f0fafc11b7ab7aea5124d2a89c634fc.pkl` & `srai-0.3.0/tests/loaders/osm_way_loader/test_files/graph_2.pkl`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 950e 0d00 0000 0000 008c 1d6e 6574  .............net
+00000000: 8004 95fb 0c00 0000 0000 008c 1d6e 6574  .............net
 00000010: 776f 726b 782e 636c 6173 7365 732e 6d75  workx.classes.mu
 00000020: 6c74 6964 6967 7261 7068 948c 0c4d 756c  ltidigraph...Mul
 00000030: 7469 4469 4772 6170 6894 9394 2981 947d  tiDiGraph...)..}
 00000040: 9428 8c05 6772 6170 6894 7d94 288c 0c63  .(..graph.}.(..c
 00000050: 7265 6174 6564 5f64 6174 6594 8c13 3230  reated_date...20
 00000060: 3233 2d30 332d 3134 2032 333a 3237 3a35  23-03-14 23:27:5
 00000070: 3694 8c0c 6372 6561 7465 645f 7769 7468  6...created_with
@@ -44,167 +44,166 @@
 000002b0: 6c65 6e67 7468 948c 156e 756d 7079 2e63  length...numpy.c
 000002c0: 6f72 652e 6d75 6c74 6961 7272 6179 948c  ore.multiarray..
 000002d0: 0673 6361 6c61 7294 9394 8c05 6e75 6d70  .scalar.....nump
 000002e0: 7994 8c05 6474 7970 6594 9394 8c02 6638  y...dtype.....f8
 000002f0: 9489 8887 9452 9428 4b03 8c01 3c94 4e4e  .....R.(K...<.NN
 00000300: 4e4a ffff ffff 4aff ffff ff4b 0074 9462  NJ....J....K.t.b
 00000310: 4308 ae47 e17a 141e 4c40 9486 9452 948c  C..G.z..L@...R..
-00000320: 0867 656f 6d65 7472 7994 8c1b 7368 6170  .geometry...shap
-00000330: 656c 792e 6765 6f6d 6574 7279 2e6c 696e  ely.geometry.lin
-00000340: 6573 7472 696e 6794 8c0a 4c69 6e65 5374  estring...LineSt
-00000350: 7269 6e67 9493 9429 5294 4359 0102 0000  ring...)R.CY....
-00000360: 0005 0000 00d7 1eac b5e6 1931 40c9 e30e  ...........1@...
-00000370: 400f 8e49 40ef a2f9 ade7 1931 4046 674f  @..I@......1@FgO
-00000380: b80d 8e49 402a 8d98 d9e7 1931 401d 8c7d  ...I@*.....1@..}
-00000390: 6e0d 8e49 4037 1cf1 bff0 1931 40a1 3f7e  n..I@7.....1@.?~
-000003a0: 80ff 8d49 4031 7326 12f1 1931 40ad bf25  ...I@1s&...1@..%
-000003b0: 00ff 8d49 4094 6275 7373 4a84 cd7c 0e7d  ...I@.bussJ..|.}
-000003c0: 948a 0593 5585 b700 7d94 4b00 7d94 2868  ....U...}.K.}.(h
-000003d0: 214a 4dc9 5901 6822 6823 6824 6825 6826  !JM.Y.h"h#h$h%h&
-000003e0: 6827 6828 6829 682a 8968 2b88 682c 682f  h'h(h)h*.h+.h,h/
-000003f0: 6835 4308 cdcc cccc ccc4 5b40 9486 9452  h5C.......[@...R
-00000400: 9468 3b68 3e29 5294 4349 0102 0000 0004  .h;h>)R.CI......
-00000410: 0000 0015 5800 5306 1a31 40e7 1890 bdde  ....X.S..1@.....
-00000420: 8d49 40f7 cec3 6405 1a31 407b a41c 27e0  .I@...d..1@{..'.
-00000430: 8d49 4073 bed8 7bf1 1931 4090 920d 5afe  .I@s..{..1@...Z.
-00000440: 8d49 4049 e306 32f1 1931 400d 9a4c cbfe  .I@I..2..1@..L..
-00000450: 8d49 4094 6275 7373 8a05 9355 85b7 007d  .I@.buss...U...}
-00000460: 9428 8a05 5d33 da2c 017d 944b 007d 9428  .(..]3.,.}.K.}.(
-00000470: 6821 4a4d c959 0168 2268 2368 2468 2568  h!JM.Y.h"h#h$h%h
-00000480: 2668 2768 2868 2968 2a89 682b 8868 2c68  &h'h(h)h*.h+.h,h
-00000490: 2f68 3543 0837 8941 60e5 d0e6 3f94 8694  /h5C.7.A`...?...
-000004a0: 5294 7573 4a84 cd7c 0e7d 944b 007d 9428  R.usJ..|.}.K.}.(
-000004b0: 6821 4a4d c959 0168 2268 2368 2468 2568  h!JM.Y.h"h#h$h%h
-000004c0: 2668 2768 2868 2968 2a89 682b 8968 2c68  &h'h(h)h*.h+.h,h
-000004d0: 2f68 3543 08cd cccc cccc c45b 4094 8694  /h5C.......[@...
-000004e0: 5294 683b 683e 2952 9443 4901 0200 0000  R.h;h>)R.CI.....
-000004f0: 0400 0000 49e3 0632 f119 3140 0d9a 4ccb  ....I..2..1@..L.
-00000500: fe8d 4940 73be d87b f119 3140 9092 0d5a  ..I@s..{..1@...Z
-00000510: fe8d 4940 f7ce c364 051a 3140 7ba4 1c27  ..I@...d..1@{..'
-00000520: e08d 4940 1558 0053 061a 3140 e718 90bd  ..I@.X.S..1@....
-00000530: de8d 4940 9462 7573 8a05 9755 85b7 007d  ..I@.bus...U...}
-00000540: 944b 007d 9428 6821 4a65 6b17 1268 248c  .K.}.(h!Jek..h$.
-00000550: 0470 6174 6894 682a 8968 2b89 682c 682f  .path.h*.h+.h,h/
-00000560: 6835 4308 ae47 e17a 144e 4140 9486 9452  h5C..G.z.NA@...R
-00000570: 9468 3b68 3e29 5294 4359 0102 0000 0005  .h;h>)R.CY......
-00000580: 0000 0049 e306 32f1 1931 400d 9a4c cbfe  ...I..2..1@..L..
-00000590: 8d49 40e3 59dd 45f3 1931 40b9 c903 ecfe  .I@.Y.E..1@.....
-000005a0: 8d49 40fa 8106 f6f3 1931 4048 84eb f6fe  .I@......1@H....
-000005b0: 8d49 404b b9b1 8f04 1a31 40ad 01a5 fcff  .I@K.....1@.....
-000005c0: 8d49 40b6 fc1b 0f11 1a31 4089 9b53 c900  .I@......1@..S..
-000005d0: 8e49 4094 6275 7375 8a05 9755 85b7 007d  .I@.busu...U...}
-000005e0: 9428 8a05 9355 85b7 007d 944b 007d 9428  .(...U...}.K.}.(
-000005f0: 6821 4a65 6b17 1268 2468 5868 2a89 682b  h!Jek..h$hXh*.h+
-00000600: 8868 2c68 2f68 3543 08af 47e1 7a14 4e41  .h,h/h5C..G.z.NA
-00000610: 4094 8694 5294 683b 683e 2952 9443 5901  @...R.h;h>)R.CY.
-00000620: 0200 0000 0500 0000 b6fc 1b0f 111a 3140  ..............1@
-00000630: 899b 53c9 008e 4940 4bb9 b18f 041a 3140  ..S...I@K.....1@
-00000640: ad01 a5fc ff8d 4940 fa81 06f6 f319 3140  ......I@......1@
-00000650: 4884 ebf6 fe8d 4940 e359 dd45 f319 3140  H.....I@.Y.E..1@
-00000660: b9c9 03ec fe8d 4940 49e3 0632 f119 3140  ......I@I..2..1@
-00000670: 0d9a 4ccb fe8d 4940 9462 7573 8a05 b98c  ..L...I@.bus....
-00000680: e063 017d 944b 007d 9428 6821 4a07 98b0  .c.}.K.}.(h!J...
-00000690: 2568 248c 0470 6174 6894 682a 8968 2b88  %h$..path.h*.h+.
-000006a0: 682c 682f 6835 4308 6666 6666 66ee 5a40  h,h/h5C.fffff.Z@
-000006b0: 9486 9452 9468 3b68 3e29 5294 4369 0102  ...R.h;h>)R.Ci..
-000006c0: 0000 0006 0000 00b6 fc1b 0f11 1a31 4089  .............1@.
-000006d0: 9b53 c900 8e49 40d3 8558 fd11 1a31 40d6  .S...I@..X...1@.
-000006e0: 5240 daff 8d49 40cb 2c42 b115 1a31 40c7  R@...I@.,B...1@.
-000006f0: 139c 55fa 8d49 4075 5ebe 501b 1a31 4025  ..U..I@u^.P..1@%
-00000700: c56c 6ef1 8d49 403c bd52 9621 1a31 4078  .ln..I@<.R.!.1@x
-00000710: 58f2 c2e7 8d49 40ff dab0 5c25 1a31 40bc  X....I@...\%.1@.
-00000720: 5f60 b1e1 8d49 4094 6275 7375 8a05 7f6d  _`...I@.busu...m
-00000730: c727 017d 948a 055d 33da 2c01 7d94 288a  .'.}...]3.,.}.(.
-00000740: 0593 5585 b700 7d94 4b00 7d94 2868 214a  ..U...}.K.}.(h!J
-00000750: 4dc9 5901 6822 6823 6824 6825 6826 6827  M.Y.h"h#h$h%h&h'
-00000760: 6828 6829 682a 8968 2b89 682c 682f 6835  h(h)h*.h+.h,h/h5
-00000770: 4308 3789 4160 e5d0 e63f 9486 9452 9475  C.7.A`...?...R.u
-00000780: 734a 83cd 7c0e 7d94 4b00 7d94 2868 214a  sJ..|.}.K.}.(h!J
-00000790: 4dc9 5901 6822 6823 6824 6825 6826 6827  M.Y.h"h#h$h%h&h'
-000007a0: 6828 6829 682a 8968 2b88 682c 682f 6835  h(h)h*.h+.h,h/h5
-000007b0: 4308 ae47 e17a 141e 4c40 9486 9452 9468  C..G.z..L@...R.h
-000007c0: 3b68 3e29 5294 4359 0102 0000 0005 0000  ;h>)R.CY........
-000007d0: 0031 7326 12f1 1931 40ad bf25 00ff 8d49  .1s&...1@..%...I
-000007e0: 4037 1cf1 bff0 1931 40a1 3f7e 80ff 8d49  @7.....1@.?~...I
-000007f0: 402a 8d98 d9e7 1931 401d 8c7d 6e0d 8e49  @*.....1@..}n..I
-00000800: 40ef a2f9 ade7 1931 4046 674f b80d 8e49  @......1@FgO...I
-00000810: 40d7 1eac b5e6 1931 40c9 e30e 400f 8e49  @......1@...@..I
-00000820: 4094 6275 738a 055e 33da 2c01 7d94 4b00  @.bus..^3.,.}.K.
-00000830: 7d94 2868 214a 6882 d31e 6824 8c07 7365  }.(h!Jh...h$..se
-00000840: 7276 6963 6594 682a 8968 2b88 682c 682f  rvice.h*.h+.h,h/
-00000850: 6835 4308 60e5 d022 db09 4240 9486 9452  h5C.`.."..B@...R
-00000860: 9468 3b68 3e29 5294 4369 0102 0000 0006  .h;h>)R.Ci......
-00000870: 0000 0031 7326 12f1 1931 40ad bf25 00ff  ...1s&...1@..%..
-00000880: 8d49 4020 e05a 37ef 1931 4054 8ec9 e2fe  .I@ .Z7..1@T....
-00000890: 8d49 409e 49f6 63ee 1931 4007 955d d5fe  .I@.I.c..1@..]..
-000008a0: 8d49 405e 91a9 ccde 1931 40a2 17a4 cffd  .I@^.....1@.....
-000008b0: 8d49 40f4 6a25 19de 1931 407e 9de5 c3fd  .I@.j%...1@~....
-000008c0: 8d49 408a ffe0 e8cf 1931 408b 9356 d7fc  .I@......1@..V..
-000008d0: 8d49 4094 6275 7375 8a05 5e33 da2c 017d  .I@.busu..^3.,.}
-000008e0: 9428 8a05 5d33 da2c 017d 944b 007d 9428  .(..]3.,.}.K.}.(
-000008f0: 6821 4a68 82d3 1e68 2468 7e68 2a89 682b  h!Jh...h$h~h*.h+
-00000900: 8968 2c68 2f68 3543 0860 e5d0 22db 0942  .h,h/h5C.`.."..B
-00000910: 4094 8694 5294 683b 683e 2952 9443 6901  @...R.h;h>)R.Ci.
-00000920: 0200 0000 0600 0000 8aff e0e8 cf19 3140  ..............1@
-00000930: 8b93 56d7 fc8d 4940 f46a 2519 de19 3140  ..V...I@.j%...1@
-00000940: 7e9d e5c3 fd8d 4940 5e91 a9cc de19 3140  ~.....I@^.....1@
-00000950: a217 a4cf fd8d 4940 9e49 f663 ee19 3140  ......I@.I.c..1@
-00000960: 0795 5dd5 fe8d 4940 20e0 5a37 ef19 3140  ..]...I@ .Z7..1@
-00000970: 548e c9e2 fe8d 4940 3173 2612 f119 3140  T.....I@1s&...1@
-00000980: adbf 2500 ff8d 4940 9462 7573 8a05 5f33  ..%...I@.bus.._3
-00000990: da2c 017d 944b 007d 9428 6821 4a69 82d3  .,.}.K.}.(h!Ji..
-000009a0: 1e68 248c 0773 6572 7669 6365 9468 2a89  .h$..service.h*.
-000009b0: 682b 8968 2c68 2f68 3543 0883 c0ca a145  h+.h,h/h5C.....E
-000009c0: b61d 4094 8694 5294 683b 683e 2952 9443  ..@...R.h;h>)R.C
-000009d0: 3901 0200 0000 0300 0000 8aff e0e8 cf19  9...............
-000009e0: 3140 8b93 56d7 fc8d 4940 cbee 6e0a d019  1@..V...I@..n...
-000009f0: 3140 bae9 e0aa fc8d 4940 6bb2 eb83 d119  1@......I@k.....
-00000a00: 3140 a323 14b6 fa8d 4940 9462 7573 758a  1@.#....I@.busu.
-00000a10: 055f 33da 2c01 7d94 8a05 5e33 da2c 017d  ._3.,.}...^3.,.}
-00000a20: 944b 007d 9428 6821 4a69 82d3 1e68 2468  .K.}.(h!Ji...h$h
-00000a30: 8e68 2a89 682b 8868 2c68 2f68 3543 0883  .h*.h+.h,h/h5C..
-00000a40: c0ca a145 b61d 4094 8694 5294 683b 683e  ...E..@...R.h;h>
-00000a50: 2952 9443 3901 0200 0000 0300 0000 6bb2  )R.C9.........k.
-00000a60: eb83 d119 3140 a323 14b6 fa8d 4940 cbee  ....1@.#....I@..
-00000a70: 6e0a d019 3140 bae9 e0aa fc8d 4940 8aff  n...1@......I@..
-00000a80: e0e8 cf19 3140 8b93 56d7 fc8d 4940 9462  ....1@..V...I@.b
-00000a90: 7573 738a 05b9 8ce0 6301 7d94 8a05 9755  uss.....c.}....U
-00000aa0: 85b7 007d 944b 007d 9428 6821 4a07 98b0  ...}.K.}.(h!J...
-00000ab0: 2568 2468 6868 2a89 682b 8968 2c68 2f68  %h$hhh*.h+.h,h/h
-00000ac0: 3543 0866 6666 6666 ee5a 4094 8694 5294  5C.fffff.Z@...R.
-00000ad0: 683b 683e 2952 9443 6901 0200 0000 0600  h;h>)R.Ci.......
-00000ae0: 0000 ffda b05c 251a 3140 bc5f 60b1 e18d  .....\%.1@._`...
-00000af0: 4940 3cbd 5296 211a 3140 7858 f2c2 e78d  I@<.R.!.1@xX....
-00000b00: 4940 755e be50 1b1a 3140 25c5 6c6e f18d  I@u^.P..1@%.ln..
-00000b10: 4940 cb2c 42b1 151a 3140 c713 9c55 fa8d  I@.,B...1@...U..
-00000b20: 4940 d385 58fd 111a 3140 d652 40da ff8d  I@..X...1@.R@...
-00000b30: 4940 b6fc 1b0f 111a 3140 899b 53c9 008e  I@......1@..S...
-00000b40: 4940 9462 7573 7375 8c05 5f73 7563 6394  I@.bussu.._succ.
-00000b50: 681d 8c05 5f70 7265 6494 7d94 284a 83cd  h..._pred.}.(J..
-00000b60: 7c0e 7d94 8a05 5d33 da2c 0168 7573 4a84  |.}...]3.,.husJ.
-00000b70: cd7c 0e7d 948a 0593 5585 b700 684f 738a  .|.}....U...hOs.
-00000b80: 0593 5585 b700 7d94 284a 84cd 7c0e 6842  ..U...}.(J..|.hB
-00000b90: 8a05 9755 85b7 0068 5f8a 055d 33da 2c01  ...U...h_..]3.,.
-00000ba0: 6870 758a 0597 5585 b700 7d94 288a 0593  hpu...U...}.(...
-00000bb0: 5585 b700 6856 8a05 b98c e063 0168 9d75  U...hV.....c.h.u
-00000bc0: 8a05 7f6d c727 017d 948a 055d 33da 2c01  ...m.'.}...]3.,.
-00000bd0: 7d94 284a 83cd 7c0e 681f 8a05 9355 85b7  }.(J..|.h....U..
-00000be0: 0068 4a8a 055e 33da 2c01 6885 758a 055e  .hJ..^3.,.h.u..^
-00000bf0: 33da 2c01 7d94 288a 055d 33da 2c01 687c  3.,.}.(..]3.,.h|
-00000c00: 8a05 5f33 da2c 0168 9575 8a05 5f33 da2c  .._3.,.h.u.._3.,
-00000c10: 017d 948a 055e 33da 2c01 688c 738a 05b9  .}...^3.,.h.s...
-00000c20: 8ce0 6301 7d94 8a05 9755 85b7 0068 6673  ..c.}....U...hfs
-00000c30: 758c 0361 646a 948c 1a6e 6574 776f 726b  u..adj...network
-00000c40: 782e 636c 6173 7365 732e 636f 7265 7669  x.classes.corevi
-00000c50: 6577 7394 8c12 4d75 6c74 6941 646a 6163  ews...MultiAdjac
-00000c60: 656e 6379 5669 6577 9493 9429 8194 7d94  encyView...)..}.
-00000c70: 8c06 5f61 746c 6173 9468 1d73 628c 056e  .._atlas.h.sb..n
-00000c80: 6f64 6573 948c 1c6e 6574 776f 726b 782e  odes...networkx.
-00000c90: 636c 6173 7365 732e 7265 706f 7274 7669  classes.reportvi
-00000ca0: 6577 7394 8c08 4e6f 6465 5669 6577 9493  ews...NodeView..
-00000cb0: 9429 8194 7d94 8c06 5f6e 6f64 6573 9468  .)..}..._nodes.h
-00000cc0: 0f73 628c 0473 7563 6394 68b3 2981 947d  .sb..succ.h.)..}
-00000cd0: 9468 b668 1d73 628c 0565 6467 6573 9468  .h.h.sb..edges.h
-00000ce0: b88c 104f 7574 4d75 6c74 6945 6467 6556  ...OutMultiEdgeV
-00000cf0: 6965 7794 9394 2981 947d 9428 8c06 5f67  iew...)..}.(.._g
-00000d00: 7261 7068 9468 038c 085f 6164 6a64 6963  raph.h..._adjdic
-00000d10: 7494 681d 7562 7562 2e                   t.h.ubub.
+00000320: 0867 656f 6d65 7472 7994 8c0a 7368 6170  .geometry...shap
+00000330: 656c 792e 696f 948c 0866 726f 6d5f 776b  ely.io...from_wk
+00000340: 6294 9394 4359 0102 0000 0005 0000 00d7  b...CY..........
+00000350: 1eac b5e6 1931 40c9 e30e 400f 8e49 40ef  .....1@...@..I@.
+00000360: a2f9 ade7 1931 4046 674f b80d 8e49 402a  .....1@FgO...I@*
+00000370: 8d98 d9e7 1931 401d 8c7d 6e0d 8e49 4037  .....1@..}n..I@7
+00000380: 1cf1 bff0 1931 40a1 3f7e 80ff 8d49 4031  .....1@.?~...I@1
+00000390: 7326 12f1 1931 40ad bf25 00ff 8d49 4094  s&...1@..%...I@.
+000003a0: 8594 5294 7573 734a 84cd 7c0e 7d94 8a05  ..R.ussJ..|.}...
+000003b0: 9355 85b7 007d 944b 007d 9428 6821 4a4d  .U...}.K.}.(h!JM
+000003c0: c959 0168 2268 2368 2468 2568 2668 2768  .Y.h"h#h$h%h&h'h
+000003d0: 2868 2968 2a89 682b 8868 2c68 2f68 3543  (h)h*.h+.h,h/h5C
+000003e0: 08cd cccc cccc c45b 4094 8694 5294 683b  .......[@...R.h;
+000003f0: 683e 4349 0102 0000 0004 0000 0015 5800  h>CI..........X.
+00000400: 5306 1a31 40e7 1890 bdde 8d49 40f7 cec3  S..1@......I@...
+00000410: 6405 1a31 407b a41c 27e0 8d49 4073 bed8  d..1@{..'..I@s..
+00000420: 7bf1 1931 4090 920d 5afe 8d49 4049 e306  {..1@...Z..I@I..
+00000430: 32f1 1931 400d 9a4c cbfe 8d49 4094 8594  2..1@..L...I@...
+00000440: 5294 7573 738a 0593 5585 b700 7d94 288a  R.uss...U...}.(.
+00000450: 055d 33da 2c01 7d94 4b00 7d94 2868 214a  .]3.,.}.K.}.(h!J
+00000460: 4dc9 5901 6822 6823 6824 6825 6826 6827  M.Y.h"h#h$h%h&h'
+00000470: 6828 6829 682a 8968 2b88 682c 682f 6835  h(h)h*.h+.h,h/h5
+00000480: 4308 3789 4160 e5d0 e63f 9486 9452 9475  C.7.A`...?...R.u
+00000490: 734a 84cd 7c0e 7d94 4b00 7d94 2868 214a  sJ..|.}.K.}.(h!J
+000004a0: 4dc9 5901 6822 6823 6824 6825 6826 6827  M.Y.h"h#h$h%h&h'
+000004b0: 6828 6829 682a 8968 2b89 682c 682f 6835  h(h)h*.h+.h,h/h5
+000004c0: 4308 cdcc cccc ccc4 5b40 9486 9452 9468  C.......[@...R.h
+000004d0: 3b68 3e43 4901 0200 0000 0400 0000 49e3  ;h>CI.........I.
+000004e0: 0632 f119 3140 0d9a 4ccb fe8d 4940 73be  .2..1@..L...I@s.
+000004f0: d87b f119 3140 9092 0d5a fe8d 4940 f7ce  .{..1@...Z..I@..
+00000500: c364 051a 3140 7ba4 1c27 e08d 4940 1558  .d..1@{..'..I@.X
+00000510: 0053 061a 3140 e718 90bd de8d 4940 9485  .S..1@......I@..
+00000520: 9452 9475 738a 0597 5585 b700 7d94 4b00  .R.us...U...}.K.
+00000530: 7d94 2868 214a 656b 1712 6824 8c04 7061  }.(h!Jek..h$..pa
+00000540: 7468 9468 2a89 682b 8968 2c68 2f68 3543  th.h*.h+.h,h/h5C
+00000550: 08ae 47e1 7a14 4e41 4094 8694 5294 683b  ..G.z.NA@...R.h;
+00000560: 683e 4359 0102 0000 0005 0000 0049 e306  h>CY.........I..
+00000570: 32f1 1931 400d 9a4c cbfe 8d49 40e3 59dd  2..1@..L...I@.Y.
+00000580: 45f3 1931 40b9 c903 ecfe 8d49 40fa 8106  E..1@......I@...
+00000590: f6f3 1931 4048 84eb f6fe 8d49 404b b9b1  ...1@H.....I@K..
+000005a0: 8f04 1a31 40ad 01a5 fcff 8d49 40b6 fc1b  ...1@......I@...
+000005b0: 0f11 1a31 4089 9b53 c900 8e49 4094 8594  ...1@..S...I@...
+000005c0: 5294 7573 758a 0597 5585 b700 7d94 288a  R.usu...U...}.(.
+000005d0: 0593 5585 b700 7d94 4b00 7d94 2868 214a  ..U...}.K.}.(h!J
+000005e0: 656b 1712 6824 685b 682a 8968 2b88 682c  ek..h$h[h*.h+.h,
+000005f0: 682f 6835 4308 af47 e17a 144e 4140 9486  h/h5C..G.z.NA@..
+00000600: 9452 9468 3b68 3e43 5901 0200 0000 0500  .R.h;h>CY.......
+00000610: 0000 b6fc 1b0f 111a 3140 899b 53c9 008e  ........1@..S...
+00000620: 4940 4bb9 b18f 041a 3140 ad01 a5fc ff8d  I@K.....1@......
+00000630: 4940 fa81 06f6 f319 3140 4884 ebf6 fe8d  I@......1@H.....
+00000640: 4940 e359 dd45 f319 3140 b9c9 03ec fe8d  I@.Y.E..1@......
+00000650: 4940 49e3 0632 f119 3140 0d9a 4ccb fe8d  I@I..2..1@..L...
+00000660: 4940 9485 9452 9475 738a 05b9 8ce0 6301  I@...R.us.....c.
+00000670: 7d94 4b00 7d94 2868 214a 0798 b025 6824  }.K.}.(h!J...%h$
+00000680: 8c04 7061 7468 9468 2a89 682b 8868 2c68  ..path.h*.h+.h,h
+00000690: 2f68 3543 0866 6666 6666 ee5a 4094 8694  /h5C.fffff.Z@...
+000006a0: 5294 683b 683e 4369 0102 0000 0006 0000  R.h;h>Ci........
+000006b0: 00b6 fc1b 0f11 1a31 4089 9b53 c900 8e49  .......1@..S...I
+000006c0: 40d3 8558 fd11 1a31 40d6 5240 daff 8d49  @..X...1@.R@...I
+000006d0: 40cb 2c42 b115 1a31 40c7 139c 55fa 8d49  @.,B...1@...U..I
+000006e0: 4075 5ebe 501b 1a31 4025 c56c 6ef1 8d49  @u^.P..1@%.ln..I
+000006f0: 403c bd52 9621 1a31 4078 58f2 c2e7 8d49  @<.R.!.1@xX....I
+00000700: 40ff dab0 5c25 1a31 40bc 5f60 b1e1 8d49  @...\%.1@._`...I
+00000710: 4094 8594 5294 7573 758a 057f 6dc7 2701  @...R.usu...m.'.
+00000720: 7d94 8a05 5d33 da2c 017d 9428 8a05 9355  }...]3.,.}.(...U
+00000730: 85b7 007d 944b 007d 9428 6821 4a4d c959  ...}.K.}.(h!JM.Y
+00000740: 0168 2268 2368 2468 2568 2668 2768 2868  .h"h#h$h%h&h'h(h
+00000750: 2968 2a89 682b 8968 2c68 2f68 3543 0837  )h*.h+.h,h/h5C.7
+00000760: 8941 60e5 d0e6 3f94 8694 5294 7573 4a83  .A`...?...R.usJ.
+00000770: cd7c 0e7d 944b 007d 9428 6821 4a4d c959  .|.}.K.}.(h!JM.Y
+00000780: 0168 2268 2368 2468 2568 2668 2768 2868  .h"h#h$h%h&h'h(h
+00000790: 2968 2a89 682b 8868 2c68 2f68 3543 08ae  )h*.h+.h,h/h5C..
+000007a0: 47e1 7a14 1e4c 4094 8694 5294 683b 683e  G.z..L@...R.h;h>
+000007b0: 4359 0102 0000 0005 0000 0031 7326 12f1  CY.........1s&..
+000007c0: 1931 40ad bf25 00ff 8d49 4037 1cf1 bff0  .1@..%...I@7....
+000007d0: 1931 40a1 3f7e 80ff 8d49 402a 8d98 d9e7  .1@.?~...I@*....
+000007e0: 1931 401d 8c7d 6e0d 8e49 40ef a2f9 ade7  .1@..}n..I@.....
+000007f0: 1931 4046 674f b80d 8e49 40d7 1eac b5e6  .1@FgO...I@.....
+00000800: 1931 40c9 e30e 400f 8e49 4094 8594 5294  .1@...@..I@...R.
+00000810: 7573 8a05 5e33 da2c 017d 944b 007d 9428  us..^3.,.}.K.}.(
+00000820: 6821 4a68 82d3 1e68 248c 0773 6572 7669  h!Jh...h$..servi
+00000830: 6365 9468 2a89 682b 8868 2c68 2f68 3543  ce.h*.h+.h,h/h5C
+00000840: 0860 e5d0 22db 0942 4094 8694 5294 683b  .`.."..B@...R.h;
+00000850: 683e 4369 0102 0000 0006 0000 0031 7326  h>Ci.........1s&
+00000860: 12f1 1931 40ad bf25 00ff 8d49 4020 e05a  ...1@..%...I@ .Z
+00000870: 37ef 1931 4054 8ec9 e2fe 8d49 409e 49f6  7..1@T.....I@.I.
+00000880: 63ee 1931 4007 955d d5fe 8d49 405e 91a9  c..1@..]...I@^..
+00000890: ccde 1931 40a2 17a4 cffd 8d49 40f4 6a25  ...1@......I@.j%
+000008a0: 19de 1931 407e 9de5 c3fd 8d49 408a ffe0  ...1@~.....I@...
+000008b0: e8cf 1931 408b 9356 d7fc 8d49 4094 8594  ...1@..V...I@...
+000008c0: 5294 7573 758a 055e 33da 2c01 7d94 288a  R.usu..^3.,.}.(.
+000008d0: 055d 33da 2c01 7d94 4b00 7d94 2868 214a  .]3.,.}.K.}.(h!J
+000008e0: 6882 d31e 6824 6885 682a 8968 2b89 682c  h...h$h.h*.h+.h,
+000008f0: 682f 6835 4308 60e5 d022 db09 4240 9486  h/h5C.`.."..B@..
+00000900: 9452 9468 3b68 3e43 6901 0200 0000 0600  .R.h;h>Ci.......
+00000910: 0000 8aff e0e8 cf19 3140 8b93 56d7 fc8d  ........1@..V...
+00000920: 4940 f46a 2519 de19 3140 7e9d e5c3 fd8d  I@.j%...1@~.....
+00000930: 4940 5e91 a9cc de19 3140 a217 a4cf fd8d  I@^.....1@......
+00000940: 4940 9e49 f663 ee19 3140 0795 5dd5 fe8d  I@.I.c..1@..]...
+00000950: 4940 20e0 5a37 ef19 3140 548e c9e2 fe8d  I@ .Z7..1@T.....
+00000960: 4940 3173 2612 f119 3140 adbf 2500 ff8d  I@1s&...1@..%...
+00000970: 4940 9485 9452 9475 738a 055f 33da 2c01  I@...R.us.._3.,.
+00000980: 7d94 4b00 7d94 2868 214a 6982 d31e 6824  }.K.}.(h!Ji...h$
+00000990: 8c07 7365 7276 6963 6594 682a 8968 2b89  ..service.h*.h+.
+000009a0: 682c 682f 6835 4308 83c0 caa1 45b6 1d40  h,h/h5C.....E..@
+000009b0: 9486 9452 9468 3b68 3e43 3901 0200 0000  ...R.h;h>C9.....
+000009c0: 0300 0000 8aff e0e8 cf19 3140 8b93 56d7  ..........1@..V.
+000009d0: fc8d 4940 cbee 6e0a d019 3140 bae9 e0aa  ..I@..n...1@....
+000009e0: fc8d 4940 6bb2 eb83 d119 3140 a323 14b6  ..I@k.....1@.#..
+000009f0: fa8d 4940 9485 9452 9475 7375 8a05 5f33  ..I@...R.usu.._3
+00000a00: da2c 017d 948a 055e 33da 2c01 7d94 4b00  .,.}...^3.,.}.K.
+00000a10: 7d94 2868 214a 6982 d31e 6824 6897 682a  }.(h!Ji...h$h.h*
+00000a20: 8968 2b88 682c 682f 6835 4308 83c0 caa1  .h+.h,h/h5C.....
+00000a30: 45b6 1d40 9486 9452 9468 3b68 3e43 3901  E..@...R.h;h>C9.
+00000a40: 0200 0000 0300 0000 6bb2 eb83 d119 3140  ........k.....1@
+00000a50: a323 14b6 fa8d 4940 cbee 6e0a d019 3140  .#....I@..n...1@
+00000a60: bae9 e0aa fc8d 4940 8aff e0e8 cf19 3140  ......I@......1@
+00000a70: 8b93 56d7 fc8d 4940 9485 9452 9475 7373  ..V...I@...R.uss
+00000a80: 8a05 b98c e063 017d 948a 0597 5585 b700  .....c.}....U...
+00000a90: 7d94 4b00 7d94 2868 214a 0798 b025 6824  }.K.}.(h!J...%h$
+00000aa0: 686d 682a 8968 2b89 682c 682f 6835 4308  hmh*.h+.h,h/h5C.
+00000ab0: 6666 6666 66ee 5a40 9486 9452 9468 3b68  fffff.Z@...R.h;h
+00000ac0: 3e43 6901 0200 0000 0600 0000 ffda b05c  >Ci............\
+00000ad0: 251a 3140 bc5f 60b1 e18d 4940 3cbd 5296  %.1@._`...I@<.R.
+00000ae0: 211a 3140 7858 f2c2 e78d 4940 755e be50  !.1@xX....I@u^.P
+00000af0: 1b1a 3140 25c5 6c6e f18d 4940 cb2c 42b1  ..1@%.ln..I@.,B.
+00000b00: 151a 3140 c713 9c55 fa8d 4940 d385 58fd  ..1@...U..I@..X.
+00000b10: 111a 3140 d652 40da ff8d 4940 b6fc 1b0f  ..1@.R@...I@....
+00000b20: 111a 3140 899b 53c9 008e 4940 9485 9452  ..1@..S...I@...R
+00000b30: 9475 7373 758c 055f 7375 6363 9468 1d8c  .ussu.._succ.h..
+00000b40: 055f 7072 6564 947d 9428 4a83 cd7c 0e7d  ._pred.}.(J..|.}
+00000b50: 948a 055d 33da 2c01 687b 734a 84cd 7c0e  ...]3.,.h{sJ..|.
+00000b60: 7d94 8a05 9355 85b7 0068 5173 8a05 9355  }....U...hQs...U
+00000b70: 85b7 007d 9428 4a84 cd7c 0e68 438a 0597  ...}.(J..|.hC...
+00000b80: 5585 b700 6863 8a05 5d33 da2c 0168 7675  U...hc..]3.,.hvu
+00000b90: 8a05 9755 85b7 007d 9428 8a05 9355 85b7  ...U...}.(...U..
+00000ba0: 0068 598a 05b9 8ce0 6301 68a8 758a 057f  .hY.....c.h.u...
+00000bb0: 6dc7 2701 7d94 8a05 5d33 da2c 017d 9428  m.'.}...]3.,.}.(
+00000bc0: 4a83 cd7c 0e68 1f8a 0593 5585 b700 684c  J..|.h....U...hL
+00000bd0: 8a05 5e33 da2c 0168 8d75 8a05 5e33 da2c  ..^3.,.h.u..^3.,
+00000be0: 017d 9428 8a05 5d33 da2c 0168 838a 055f  .}.(..]3.,.h..._
+00000bf0: 33da 2c01 689f 758a 055f 33da 2c01 7d94  3.,.h.u.._3.,.}.
+00000c00: 8a05 5e33 da2c 0168 9573 8a05 b98c e063  ..^3.,.h.s.....c
+00000c10: 017d 948a 0597 5585 b700 686b 7375 8c03  .}....U...hksu..
+00000c20: 6164 6a94 8c1a 6e65 7477 6f72 6b78 2e63  adj...networkx.c
+00000c30: 6c61 7373 6573 2e63 6f72 6576 6965 7773  lasses.coreviews
+00000c40: 948c 124d 756c 7469 4164 6a61 6365 6e63  ...MultiAdjacenc
+00000c50: 7956 6965 7794 9394 2981 947d 948c 065f  yView...)..}..._
+00000c60: 6174 6c61 7394 681d 7362 8c05 6e6f 6465  atlas.h.sb..node
+00000c70: 7394 8c1c 6e65 7477 6f72 6b78 2e63 6c61  s...networkx.cla
+00000c80: 7373 6573 2e72 6570 6f72 7476 6965 7773  sses.reportviews
+00000c90: 948c 084e 6f64 6556 6965 7794 9394 2981  ...NodeView...).
+00000ca0: 947d 948c 065f 6e6f 6465 7394 680f 7362  .}..._nodes.h.sb
+00000cb0: 8c04 7375 6363 9468 bf29 8194 7d94 68c2  ..succ.h.)..}.h.
+00000cc0: 681d 7362 8c05 6564 6765 7394 68c4 8c10  h.sb..edges.h...
+00000cd0: 4f75 744d 756c 7469 4564 6765 5669 6577  OutMultiEdgeView
+00000ce0: 9493 9429 8194 7d94 288c 065f 6772 6170  ...)..}.(.._grap
+00000cf0: 6894 6803 8c08 5f61 646a 6469 6374 9468  h.h..._adjdict.h
+00000d00: 1d75 6275 622e                           .ubub.
```

### Comparing `srai-0.2.0/tests/loaders/osm_way_loader/files/4310fe8d3c435f2a83fac55fc79f9166.pkl` & `srai-0.3.0/tests/loaders/osm_way_loader/test_files/graph_1.pkl`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 95e3 0e00 0000 0000 008c 1d6e 6574  .............net
+00000000: 8004 95d0 0e00 0000 0000 008c 1d6e 6574  .............net
 00000010: 776f 726b 782e 636c 6173 7365 732e 6d75  workx.classes.mu
 00000020: 6c74 6964 6967 7261 7068 948c 0c4d 756c  ltidigraph...Mul
 00000030: 7469 4469 4772 6170 6894 9394 2981 947d  tiDiGraph...)..}
 00000040: 9428 8c05 6772 6170 6894 7d94 288c 0c63  .(..graph.}.(..c
 00000050: 7265 6174 6564 5f64 6174 6594 8c13 3230  reated_date...20
 00000060: 3233 2d30 332d 3134 2032 333a 3237 3a35  23-03-14 23:27:5
 00000070: 3894 8c0c 6372 6561 7465 645f 7769 7468  8...created_with
@@ -40,200 +40,199 @@
 00000270: 7468 948c 156e 756d 7079 2e63 6f72 652e  th...numpy.core.
 00000280: 6d75 6c74 6961 7272 6179 948c 0673 6361  multiarray...sca
 00000290: 6c61 7294 9394 8c05 6e75 6d70 7994 8c05  lar.....numpy...
 000002a0: 6474 7970 6594 9394 8c02 6638 9489 8887  dtype.....f8....
 000002b0: 9452 9428 4b03 8c01 3c94 4e4e 4e4a ffff  .R.(K...<.NNNJ..
 000002c0: ffff 4aff ffff ff4b 0074 9462 4308 3333  ..J....K.t.bC.33
 000002d0: 3333 3323 5440 9486 9452 948c 0867 656f  333#T@...R...geo
-000002e0: 6d65 7472 7994 8c1b 7368 6170 656c 792e  metry...shapely.
-000002f0: 6765 6f6d 6574 7279 2e6c 696e 6573 7472  geometry.linestr
-00000300: 696e 6794 8c0a 4c69 6e65 5374 7269 6e67  ing...LineString
-00000310: 9493 9429 5294 4359 0102 0000 0005 0000  ...)R.CY........
-00000320: 00d7 1eac b5e6 1931 40c9 e30e 400f 8e49  .......1@...@..I
-00000330: 40aa 9b8b bfed 1931 4087 acc9 ae0f 8e49  @......1@......I
-00000340: 40b5 e1b0 34f0 1931 40da d836 d60f 8e49  @...4..1@..6...I
-00000350: 4091 4028 942a 1a31 40af 0562 7e13 8e49  @.@(.*.1@..b~..I
-00000360: 40d5 1cc5 de30 1a31 4073 d30b e313 8e49  @....0.1@s.....I
-00000370: 4094 6275 734a 84cd 7c0e 7d94 4b00 7d94  @.busJ..|.}.K.}.
-00000380: 2868 204a 4dc9 5901 6822 8c10 416e 6472  (h JM.Y.h"..Andr
-00000390: 7a65 6a61 2050 6f74 6562 6e69 9468 248c  zeja Potebni.h$.
-000003a0: 0b72 6573 6964 656e 7469 616c 9468 268c  .residential.h&.
-000003b0: 0233 3094 6828 8c07 6173 7068 616c 7494  .30.h(..asphalt.
-000003c0: 6821 8968 2c89 682d 6830 6836 4308 dcf9  h!.h,.h-h0h6C...
-000003d0: 7e6a bc00 6540 9486 9452 9468 3c68 3f29  ~j..e@...R.h<h?)
-000003e0: 5294 4399 0102 0000 0009 0000 00d7 1eac  R.C.............
-000003f0: b5e6 1931 40c9 e30e 400f 8e49 40ef a2f9  ...1@...@..I@...
-00000400: ade7 1931 4046 674f b80d 8e49 402a 8d98  ...1@FgO...I@*..
-00000410: d9e7 1931 401d 8c7d 6e0d 8e49 4037 1cf1  ...1@..}n..I@7..
-00000420: bff0 1931 40a1 3f7e 80ff 8d49 4031 7326  ...1@.?~...I@1s&
-00000430: 12f1 1931 40ad bf25 00ff 8d49 4049 e306  ...1@..%...I@I..
-00000440: 32f1 1931 400d 9a4c cbfe 8d49 4073 bed8  2..1@..L...I@s..
-00000450: 7bf1 1931 4090 920d 5afe 8d49 40f7 cec3  {..1@...Z..I@...
-00000460: 6405 1a31 407b a41c 27e0 8d49 4015 5800  d..1@{..'..I@.X.
-00000470: 5306 1a31 40e7 1890 bdde 8d49 4094 6275  S..1@......I@.bu
-00000480: 7375 4a84 cd7c 0e7d 9428 8a05 0055 a8b2  suJ..|.}.(...U..
-00000490: 007d 944b 007d 9428 6820 5d94 284a 0d71  .}.K.}.(h ].(J.q
-000004a0: 751e 4a4d c959 0165 6822 6844 6824 6845  u.JM.Y.eh"hDh$hE
-000004b0: 6826 6846 6828 6847 6821 8968 2c89 682d  h&hFh(hGh!.h,.h-
-000004c0: 6830 6836 4308 6f12 83c0 cab1 6a40 9486  h0h6C.o.....j@..
-000004d0: 9452 9468 2a8c 0379 6573 9468 3c68 3f29  .R.h*..yes.h<h?)
-000004e0: 5294 4379 0102 0000 0007 0000 0015 5800  R.Cy..........X.
-000004f0: 5306 1a31 40e7 1890 bdde 8d49 40f0 f1ae  S..1@......I@...
-00000500: 1f07 1a31 40d0 381e 7ddd 8d49 40f9 090c  ...1@.8.}..I@...
-00000510: fe23 1a31 40be 0ba5 40b0 8d49 40b1 e144  .#.1@...@..I@..D
-00000520: 4f25 1a31 4041 5d49 97a3 8d49 4082 5da8  O%.1@A]I...I@.].
-00000530: 5725 1a31 402f c445 49a3 8d49 4040 ca3e  W%.1@/.EI..I@@.>
-00000540: 7e25 1a31 40dd f934 dda1 8d49 402e bb71  ~%.1@..4...I@..q
-00000550: 9c25 1a31 4072 497a bda0 8d49 4094 6275  .%.1@rIz...I@.bu
-00000560: 734a 83cd 7c0e 7d94 4b00 7d94 2868 204a  sJ..|.}.K.}.(h J
-00000570: 4dc9 5901 6822 6844 6824 6845 6826 6846  M.Y.h"hDh$hEh&hF
-00000580: 6828 6847 6821 8968 2c88 682d 6830 6836  h(hGh!.h,.h-h0h6
-00000590: 4308 dbf9 7e6a bc00 6540 9486 9452 9468  C...~j..e@...R.h
-000005a0: 3c68 3f29 5294 4399 0102 0000 0009 0000  <h?)R.C.........
-000005b0: 0015 5800 5306 1a31 40e7 1890 bdde 8d49  ..X.S..1@......I
-000005c0: 40f7 cec3 6405 1a31 407b a41c 27e0 8d49  @...d..1@{..'..I
-000005d0: 4073 bed8 7bf1 1931 4090 920d 5afe 8d49  @s..{..1@...Z..I
-000005e0: 4049 e306 32f1 1931 400d 9a4c cbfe 8d49  @I..2..1@..L...I
-000005f0: 4031 7326 12f1 1931 40ad bf25 00ff 8d49  @1s&...1@..%...I
-00000600: 4037 1cf1 bff0 1931 40a1 3f7e 80ff 8d49  @7.....1@.?~...I
-00000610: 402a 8d98 d9e7 1931 401d 8c7d 6e0d 8e49  @*.....1@..}n..I
-00000620: 40ef a2f9 ade7 1931 4046 674f b80d 8e49  @......1@FgO...I
-00000630: 40d7 1eac b5e6 1931 40c9 e30e 400f 8e49  @......1@...@..I
-00000640: 4094 6275 734a dd76 cb0e 7d94 4b00 7d94  @.busJ.v..}.K.}.
-00000650: 2868 204a 4ec9 5901 6822 8c11 5069 6572  (h JN.Y.h"..Pier
-00000660: 7773 7a65 6a20 4479 7769 7a6a 6994 6824  wszej Dywizji.h$
-00000670: 8c0b 7265 7369 6465 6e74 6961 6c94 6826  ..residential.h&
-00000680: 8c02 3330 9468 288c 0761 7370 6861 6c74  ..30.h(..asphalt
-00000690: 9468 2a8c 0379 6573 9468 2189 682c 8968  .h*..yes.h!.h,.h
-000006a0: 2d68 3068 3643 08e2 7a14 ae47 295a 4094  -h0h6C..z..G)Z@.
-000006b0: 8694 5294 683c 683f 2952 9443 6901 0200  ..R.h<h?)R.Ci...
-000006c0: 0000 0600 0000 1558 0053 061a 3140 e718  .......X.S..1@..
-000006d0: 90bd de8d 4940 95f6 6118 0b1a 3140 4cb0  ....I@..a...1@L.
-000006e0: ee0e df8d 4940 1230 babc 391a 3140 09e3  ....I@.0..9.1@..
-000006f0: 022b e28d 4940 d23e b1a9 4e1a 3140 2c85  .+..I@.>..N.1@,.
-00000700: 9be7 e38d 4940 0429 67de 601a 3140 0d66  ....I@.)g.`.1@.f
-00000710: b8a6 e58d 4940 91d1 a68f 651a 3140 d261  ....I@....e.1@.a
-00000720: 742f e68d 4940 9462 7573 4afa 286f 127d  t/..I@.busJ.(o.}
-00000730: 944b 007d 9428 6820 4ae5 a4ad 0168 228c  .K.}.(h J....h".
-00000740: 1150 6965 7277 737a 656a 2044 7977 697a  .Pierwszej Dywiz
-00000750: 6a69 9468 248c 0d6c 6976 696e 675f 7374  ji.h$..living_st
-00000760: 7265 6574 9468 2189 682c 8968 2d68 3068  reet.h!.h,.h-h0h
-00000770: 3643 0838 b4c8 76be a75d 4094 8694 5294  6C.8..v..]@...R.
-00000780: 683c 683f 2952 9443 8901 0200 0000 0800  h<h?)R.C........
-00000790: 0000 1558 0053 061a 3140 e718 90bd de8d  ...X.S..1@......
-000007a0: 4940 a5a8 8eb0 031a 3140 6a6d 7594 de8d  I@......1@jmu...
-000007b0: 4940 6aaa 82ac 021a 3140 5f35 8584 de8d  I@j.....1@_5....
-000007c0: 4940 431d 56b8 e519 3140 d757 b2be dc8d  I@C.V...1@.W....
-000007d0: 4940 c567 fc0c b919 3140 f634 1603 da8d  I@.g....1@.4....
-000007e0: 4940 b0e9 9cfa 9b19 3140 44d8 953b d88d  I@......1@D..;..
-000007f0: 4940 16e3 5707 9b19 3140 cd5f 7c2c d88d  I@..W...1@._|,..
-00000800: 4940 7062 a307 9919 3140 4aaf 720d d88d  I@pb....1@J.r...
-00000810: 4940 9462 7573 754a dd76 cb0e 7d94 4a84  I@.busuJ.v..}.J.
-00000820: cd7c 0e7d 944b 007d 9428 6820 4a4e c959  .|.}.K.}.(h JN.Y
-00000830: 0168 2268 6068 2468 6168 2668 6268 2868  .h"h`h$hah&hbh(h
-00000840: 6368 2a68 6468 2189 682c 8868 2d68 3068  ch*hdh!.h,.h-h0h
-00000850: 3643 08e1 7a14 ae47 295a 4094 8694 5294  6C..z..G)Z@...R.
-00000860: 683c 683f 2952 9443 6901 0200 0000 0600  h<h?)R.Ci.......
-00000870: 0000 91d1 a68f 651a 3140 d261 742f e68d  ......e.1@.at/..
-00000880: 4940 0429 67de 601a 3140 0d66 b8a6 e58d  I@.)g.`.1@.f....
-00000890: 4940 d23e b1a9 4e1a 3140 2c85 9be7 e38d  I@.>..N.1@,.....
-000008a0: 4940 1230 babc 391a 3140 09e3 022b e28d  I@.0..9.1@...+..
-000008b0: 4940 95f6 6118 0b1a 3140 4cb0 ee0e df8d  I@..a...1@L.....
-000008c0: 4940 1558 0053 061a 3140 e718 90bd de8d  I@.X.S..1@......
-000008d0: 4940 9462 7573 734a fa28 6f12 7d94 284a  I@.bussJ.(o.}.(J
-000008e0: 1629 6f12 7d94 4b00 7d94 2868 204a e2a4  .)o.}.K.}.(h J..
-000008f0: ad01 6822 8c1c 5075 c582 6b6f 776e 696b  ..h"..Pu..kownik
-00000900: 6120 4672 616e 6369 737a 6b61 204e 756c  a Franciszka Nul
-00000910: 6c61 9468 248c 0b72 6573 6964 656e 7469  la.h$..residenti
-00000920: 616c 9468 268c 0233 3094 6821 8968 2c89  al.h&..30.h!.h,.
-00000930: 682d 6830 6836 4308 ed51 b81e 85d3 6440  h-h0h6C..Q....d@
-00000940: 9486 9452 9468 3c68 3f29 5294 43a9 0102  ...R.h<h?)R.C...
-00000950: 0000 000a 0000 0070 62a3 0799 1931 404a  .......pb....1@J
-00000960: af72 0dd8 8d49 40ee 2763 7c98 1931 4008  .r...I@.'c|..1@.
-00000970: 0264 e8d8 8d49 407e 1ccd 9195 1931 4089  .d...I@~.....1@.
-00000980: 44a1 65dd 8d49 40f5 dc9d 1095 1931 40be  D.e..I@......1@.
-00000990: e199 2bde 8d49 4043 1ec1 8d94 1931 4046  ..+..I@C.....1@F
-000009a0: 7ded f4de 8d49 401c c2e7 3d84 1931 408d  }....I@...=..1@.
-000009b0: 77ec 0cf8 8d49 404d ae18 6481 1931 40de  w....I@M..d..1@.
-000009c0: 077b 6efc 8d49 40cd 4301 367b 1931 40f1  .{n..I@.C.6{.1@.
-000009d0: dd41 4706 8e49 40c7 e2ed f77a 1931 4020  .AG..I@....z.1@ 
-000009e0: ec14 ab06 8e49 4068 c647 307a 1931 404f  .....I@h.G0z.1@O
-000009f0: 6a79 2f08 8e49 4094 6275 734a 84cd 7c0e  jy/..I@.busJ..|.
-00000a00: 7d94 4b00 7d94 2868 204a e5a4 ad01 6822  }.K.}.(h J....h"
-00000a10: 686c 6824 686d 6821 8968 2c88 682d 6830  hlh$hmh!.h,.h-h0
-00000a20: 6836 4308 38b4 c876 bea7 5d40 9486 9452  h6C.8..v..]@...R
-00000a30: 9468 3c68 3f29 5294 4389 0102 0000 0008  .h<h?)R.C.......
-00000a40: 0000 0070 62a3 0799 1931 404a af72 0dd8  ...pb....1@J.r..
-00000a50: 8d49 4016 e357 079b 1931 40cd 5f7c 2cd8  .I@..W...1@._|,.
-00000a60: 8d49 40b0 e99c fa9b 1931 4044 d895 3bd8  .I@......1@D..;.
-00000a70: 8d49 40c5 67fc 0cb9 1931 40f6 3416 03da  .I@.g....1@.4...
-00000a80: 8d49 4043 1d56 b8e5 1931 40d7 57b2 bedc  .I@C.V...1@.W...
-00000a90: 8d49 406a aa82 ac02 1a31 405f 3585 84de  .I@j.....1@_5...
-00000aa0: 8d49 40a5 a88e b003 1a31 406a 6d75 94de  .I@......1@jmu..
-00000ab0: 8d49 4015 5800 5306 1a31 40e7 1890 bdde  .I@.X.S..1@.....
-00000ac0: 8d49 4094 6275 7375 4a16 296f 127d 9428  .I@.busuJ.)o.}.(
-00000ad0: 4a83 cd7c 0e7d 944b 007d 9428 6820 4a4c  J..|.}.K.}.(h JL
-00000ae0: c959 0168 2188 6822 6823 6824 6825 6826  .Y.h!.h"h#h$h%h&
-00000af0: 6827 6828 6829 682a 682b 682c 8968 2d68  h'h(h)h*h+h,.h-h
-00000b00: 3068 3643 0895 438b 6ce7 835d 4094 8694  0h6C..C.l..]@...
-00000b10: 5294 683c 683f 2952 9443 4901 0200 0000  R.h<h?)R.CI.....
-00000b20: 0400 0000 68c6 4730 7a19 3140 4f6a 792f  ....h.G0z.1@Ojy/
-00000b30: 088e 4940 ee7d 05c4 7f19 3140 d87b 968c  ..I@.}....1@.{..
-00000b40: 088e 4940 8738 317f e019 3140 46d7 e0d8  ..I@.81...1@F...
-00000b50: 0e8e 4940 d71e acb5 e619 3140 c9e3 0e40  ..I@......1@...@
-00000b60: 0f8e 4940 9462 7573 4afa 286f 127d 944b  ..I@.busJ.(o.}.K
-00000b70: 007d 9428 6820 4ae2 a4ad 0168 2268 7e68  .}.(h J....h"h~h
-00000b80: 2468 7f68 2668 8068 2189 682c 8868 2d68  $h.h&h.h!.h,.h-h
-00000b90: 3068 3643 08eb 51b8 1e85 d364 4094 8694  0h6C..Q....d@...
-00000ba0: 5294 683c 683f 2952 9443 a901 0200 0000  R.h<h?)R.C......
-00000bb0: 0a00 0000 68c6 4730 7a19 3140 4f6a 792f  ....h.G0z.1@Ojy/
-00000bc0: 088e 4940 c7e2 edf7 7a19 3140 20ec 14ab  ..I@....z.1@ ...
-00000bd0: 068e 4940 cd43 0136 7b19 3140 f1dd 4147  ..I@.C.6{.1@..AG
-00000be0: 068e 4940 4dae 1864 8119 3140 de07 7b6e  ..I@M..d..1@..{n
-00000bf0: fc8d 4940 1cc2 e73d 8419 3140 8d77 ec0c  ..I@...=..1@.w..
-00000c00: f88d 4940 431e c18d 9419 3140 467d edf4  ..I@C.....1@F}..
-00000c10: de8d 4940 f5dc 9d10 9519 3140 bee1 992b  ..I@......1@...+
-00000c20: de8d 4940 7e1c cd91 9519 3140 8944 a165  ..I@~.....1@.D.e
-00000c30: dd8d 4940 ee27 637c 9819 3140 0802 64e8  ..I@.'c|..1@..d.
-00000c40: d88d 4940 7062 a307 9919 3140 4aaf 720d  ..I@pb....1@J.r.
-00000c50: d88d 4940 9462 7573 758a 0500 55a8 b200  ..I@.busu...U...
-00000c60: 7d94 4a84 cd7c 0e7d 944b 007d 9428 6820  }.J..|.}.K.}.(h 
-00000c70: 5d94 284a 4dc9 5901 4a0d 7175 1e65 6822  ].(JM.Y.J.qu.eh"
-00000c80: 8c10 416e 6472 7a65 6a61 2050 6f74 6562  ..Andrzeja Poteb
-00000c90: 6e69 9468 248c 0b72 6573 6964 656e 7469  ni.h$..residenti
-00000ca0: 616c 9468 268c 0233 3094 6828 8c07 6173  al.h&..30.h(..as
-00000cb0: 7068 616c 7494 682a 6854 6821 8968 2c88  phalt.h*hTh!.h,.
-00000cc0: 682d 6830 6836 4308 6e12 83c0 cab1 6a40  h-h0h6C.n.....j@
-00000cd0: 9486 9452 9468 3c68 3f29 5294 4379 0102  ...R.h<h?)R.Cy..
-00000ce0: 0000 0007 0000 002e bb71 9c25 1a31 4072  .........q.%.1@r
-00000cf0: 497a bda0 8d49 4040 ca3e 7e25 1a31 40dd  Iz...I@@.>~%.1@.
-00000d00: f934 dda1 8d49 4082 5da8 5725 1a31 402f  .4...I@.].W%.1@/
-00000d10: c445 49a3 8d49 40b1 e144 4f25 1a31 4041  .EI..I@..DO%.1@A
-00000d20: 5d49 97a3 8d49 40f9 090c fe23 1a31 40be  ]I...I@....#.1@.
-00000d30: 0ba5 40b0 8d49 40f0 f1ae 1f07 1a31 40d0  ..@..I@......1@.
-00000d40: 381e 7ddd 8d49 4015 5800 5306 1a31 40e7  8.}..I@.X.S..1@.
-00000d50: 1890 bdde 8d49 4094 6275 7373 758c 055f  .....I@.bussu.._
-00000d60: 7375 6363 9468 1b8c 055f 7072 6564 947d  succ.h..._pred.}
-00000d70: 9428 4a82 cd7c 0e7d 944a 83cd 7c0e 681e  .(J..|.}.J..|.h.
-00000d80: 734a 83cd 7c0e 7d94 284a 84cd 7c0e 6857  sJ..|.}.(J..|.hW
-00000d90: 4a16 296f 1268 8e75 4a84 cd7c 0e7d 9428  J.)o.h.uJ..|.}.(
-00000da0: 4a83 cd7c 0e68 424a dd76 cb0e 6874 4afa  J..|.hBJ.v..htJ.
-00000db0: 286f 1268 868a 0500 55a8 b200 689d 754a  (o.h....U...h.uJ
-00000dc0: dd76 cb0e 7d94 4a84 cd7c 0e68 5e73 4afa  .v..}.J..|.h^sJ.
-00000dd0: 286f 127d 9428 4a84 cd7c 0e68 6a4a 1629  (o.}.(J..|.hjJ.)
-00000de0: 6f12 6895 754a 1629 6f12 7d94 4afa 286f  o.h.uJ.)o.}.J.(o
-00000df0: 1268 7c73 8a05 0055 a8b2 007d 944a 84cd  .h|s...U...}.J..
-00000e00: 7c0e 684e 7375 8c03 6164 6a94 8c1a 6e65  |.hNsu..adj...ne
-00000e10: 7477 6f72 6b78 2e63 6c61 7373 6573 2e63  tworkx.classes.c
-00000e20: 6f72 6576 6965 7773 948c 124d 756c 7469  oreviews...Multi
-00000e30: 4164 6a61 6365 6e63 7956 6965 7794 9394  AdjacencyView...
-00000e40: 2981 947d 948c 065f 6174 6c61 7394 681b  )..}..._atlas.h.
-00000e50: 7362 8c05 6e6f 6465 7394 8c1c 6e65 7477  sb..nodes...netw
-00000e60: 6f72 6b78 2e63 6c61 7373 6573 2e72 6570  orkx.classes.rep
-00000e70: 6f72 7476 6965 7773 948c 084e 6f64 6556  ortviews...NodeV
-00000e80: 6965 7794 9394 2981 947d 948c 065f 6e6f  iew...)..}..._no
-00000e90: 6465 7394 680f 7362 8c04 7375 6363 9468  des.h.sb..succ.h
-00000ea0: b629 8194 7d94 68b9 681b 7362 8c05 6564  .)..}.h.h.sb..ed
-00000eb0: 6765 7394 68bb 8c10 4f75 744d 756c 7469  ges.h...OutMulti
-00000ec0: 4564 6765 5669 6577 9493 9429 8194 7d94  EdgeView...)..}.
-00000ed0: 288c 065f 6772 6170 6894 6803 8c08 5f61  (.._graph.h..._a
-00000ee0: 646a 6469 6374 9468 1b75 6275 622e       djdict.h.ubub.
+000002e0: 6d65 7472 7994 8c0a 7368 6170 656c 792e  metry...shapely.
+000002f0: 696f 948c 0866 726f 6d5f 776b 6294 9394  io...from_wkb...
+00000300: 4359 0102 0000 0005 0000 00d7 1eac b5e6  CY..............
+00000310: 1931 40c9 e30e 400f 8e49 40aa 9b8b bfed  .1@...@..I@.....
+00000320: 1931 4087 acc9 ae0f 8e49 40b5 e1b0 34f0  .1@......I@...4.
+00000330: 1931 40da d836 d60f 8e49 4091 4028 942a  .1@..6...I@.@(.*
+00000340: 1a31 40af 0562 7e13 8e49 40d5 1cc5 de30  .1@..b~..I@....0
+00000350: 1a31 4073 d30b e313 8e49 4094 8594 5294  .1@s.....I@...R.
+00000360: 7573 4a84 cd7c 0e7d 944b 007d 9428 6820  usJ..|.}.K.}.(h 
+00000370: 4a4d c959 0168 228c 1041 6e64 727a 656a  JM.Y.h"..Andrzej
+00000380: 6120 506f 7465 626e 6994 6824 8c0b 7265  a Potebni.h$..re
+00000390: 7369 6465 6e74 6961 6c94 6826 8c02 3330  sidential.h&..30
+000003a0: 9468 288c 0761 7370 6861 6c74 9468 2189  .h(..asphalt.h!.
+000003b0: 682c 8968 2d68 3068 3643 08dc f97e 6abc  h,.h-h0h6C...~j.
+000003c0: 0065 4094 8694 5294 683c 683f 4399 0102  .e@...R.h<h?C...
+000003d0: 0000 0009 0000 00d7 1eac b5e6 1931 40c9  .............1@.
+000003e0: e30e 400f 8e49 40ef a2f9 ade7 1931 4046  ..@..I@......1@F
+000003f0: 674f b80d 8e49 402a 8d98 d9e7 1931 401d  gO...I@*.....1@.
+00000400: 8c7d 6e0d 8e49 4037 1cf1 bff0 1931 40a1  .}n..I@7.....1@.
+00000410: 3f7e 80ff 8d49 4031 7326 12f1 1931 40ad  ?~...I@1s&...1@.
+00000420: bf25 00ff 8d49 4049 e306 32f1 1931 400d  .%...I@I..2..1@.
+00000430: 9a4c cbfe 8d49 4073 bed8 7bf1 1931 4090  .L...I@s..{..1@.
+00000440: 920d 5afe 8d49 40f7 cec3 6405 1a31 407b  ..Z..I@...d..1@{
+00000450: a41c 27e0 8d49 4015 5800 5306 1a31 40e7  ..'..I@.X.S..1@.
+00000460: 1890 bdde 8d49 4094 8594 5294 7573 754a  .....I@...R.usuJ
+00000470: 84cd 7c0e 7d94 288a 0500 55a8 b200 7d94  ..|.}.(...U...}.
+00000480: 4b00 7d94 2868 205d 9428 4a0d 7175 1e4a  K.}.(h ].(J.qu.J
+00000490: 4dc9 5901 6568 2268 4568 2468 4668 2668  M.Y.eh"hEh$hFh&h
+000004a0: 4768 2868 4868 2189 682c 8968 2d68 3068  Gh(hHh!.h,.h-h0h
+000004b0: 3643 086f 1283 c0ca b16a 4094 8694 5294  6C.o.....j@...R.
+000004c0: 682a 8c03 7965 7394 683c 683f 4379 0102  h*..yes.h<h?Cy..
+000004d0: 0000 0007 0000 0015 5800 5306 1a31 40e7  ........X.S..1@.
+000004e0: 1890 bdde 8d49 40f0 f1ae 1f07 1a31 40d0  .....I@......1@.
+000004f0: 381e 7ddd 8d49 40f9 090c fe23 1a31 40be  8.}..I@....#.1@.
+00000500: 0ba5 40b0 8d49 40b1 e144 4f25 1a31 4041  ..@..I@..DO%.1@A
+00000510: 5d49 97a3 8d49 4082 5da8 5725 1a31 402f  ]I...I@.].W%.1@/
+00000520: c445 49a3 8d49 4040 ca3e 7e25 1a31 40dd  .EI..I@@.>~%.1@.
+00000530: f934 dda1 8d49 402e bb71 9c25 1a31 4072  .4...I@..q.%.1@r
+00000540: 497a bda0 8d49 4094 8594 5294 7573 4a83  Iz...I@...R.usJ.
+00000550: cd7c 0e7d 944b 007d 9428 6820 4a4d c959  .|.}.K.}.(h JM.Y
+00000560: 0168 2268 4568 2468 4668 2668 4768 2868  .h"hEh$hFh&hGh(h
+00000570: 4868 2189 682c 8868 2d68 3068 3643 08db  Hh!.h,.h-h0h6C..
+00000580: f97e 6abc 0065 4094 8694 5294 683c 683f  .~j..e@...R.h<h?
+00000590: 4399 0102 0000 0009 0000 0015 5800 5306  C...........X.S.
+000005a0: 1a31 40e7 1890 bdde 8d49 40f7 cec3 6405  .1@......I@...d.
+000005b0: 1a31 407b a41c 27e0 8d49 4073 bed8 7bf1  .1@{..'..I@s..{.
+000005c0: 1931 4090 920d 5afe 8d49 4049 e306 32f1  .1@...Z..I@I..2.
+000005d0: 1931 400d 9a4c cbfe 8d49 4031 7326 12f1  .1@..L...I@1s&..
+000005e0: 1931 40ad bf25 00ff 8d49 4037 1cf1 bff0  .1@..%...I@7....
+000005f0: 1931 40a1 3f7e 80ff 8d49 402a 8d98 d9e7  .1@.?~...I@*....
+00000600: 1931 401d 8c7d 6e0d 8e49 40ef a2f9 ade7  .1@..}n..I@.....
+00000610: 1931 4046 674f b80d 8e49 40d7 1eac b5e6  .1@FgO...I@.....
+00000620: 1931 40c9 e30e 400f 8e49 4094 8594 5294  .1@...@..I@...R.
+00000630: 7573 4add 76cb 0e7d 944b 007d 9428 6820  usJ.v..}.K.}.(h 
+00000640: 4a4e c959 0168 228c 1150 6965 7277 737a  JN.Y.h"..Pierwsz
+00000650: 656a 2044 7977 697a 6a69 9468 248c 0b72  ej Dywizji.h$..r
+00000660: 6573 6964 656e 7469 616c 9468 268c 0233  esidential.h&..3
+00000670: 3094 6828 8c07 6173 7068 616c 7494 682a  0.h(..asphalt.h*
+00000680: 8c03 7965 7394 6821 8968 2c89 682d 6830  ..yes.h!.h,.h-h0
+00000690: 6836 4308 e27a 14ae 4729 5a40 9486 9452  h6C..z..G)Z@...R
+000006a0: 9468 3c68 3f43 6901 0200 0000 0600 0000  .h<h?Ci.........
+000006b0: 1558 0053 061a 3140 e718 90bd de8d 4940  .X.S..1@......I@
+000006c0: 95f6 6118 0b1a 3140 4cb0 ee0e df8d 4940  ..a...1@L.....I@
+000006d0: 1230 babc 391a 3140 09e3 022b e28d 4940  .0..9.1@...+..I@
+000006e0: d23e b1a9 4e1a 3140 2c85 9be7 e38d 4940  .>..N.1@,.....I@
+000006f0: 0429 67de 601a 3140 0d66 b8a6 e58d 4940  .)g.`.1@.f....I@
+00000700: 91d1 a68f 651a 3140 d261 742f e68d 4940  ....e.1@.at/..I@
+00000710: 9485 9452 9475 734a fa28 6f12 7d94 4b00  ...R.usJ.(o.}.K.
+00000720: 7d94 2868 204a e5a4 ad01 6822 8c11 5069  }.(h J....h"..Pi
+00000730: 6572 7773 7a65 6a20 4479 7769 7a6a 6994  erwszej Dywizji.
+00000740: 6824 8c0d 6c69 7669 6e67 5f73 7472 6565  h$..living_stree
+00000750: 7494 6821 8968 2c89 682d 6830 6836 4308  t.h!.h,.h-h0h6C.
+00000760: 38b4 c876 bea7 5d40 9486 9452 9468 3c68  8..v..]@...R.h<h
+00000770: 3f43 8901 0200 0000 0800 0000 1558 0053  ?C...........X.S
+00000780: 061a 3140 e718 90bd de8d 4940 a5a8 8eb0  ..1@......I@....
+00000790: 031a 3140 6a6d 7594 de8d 4940 6aaa 82ac  ..1@jmu...I@j...
+000007a0: 021a 3140 5f35 8584 de8d 4940 431d 56b8  ..1@_5....I@C.V.
+000007b0: e519 3140 d757 b2be dc8d 4940 c567 fc0c  ..1@.W....I@.g..
+000007c0: b919 3140 f634 1603 da8d 4940 b0e9 9cfa  ..1@.4....I@....
+000007d0: 9b19 3140 44d8 953b d88d 4940 16e3 5707  ..1@D..;..I@..W.
+000007e0: 9b19 3140 cd5f 7c2c d88d 4940 7062 a307  ..1@._|,..I@pb..
+000007f0: 9919 3140 4aaf 720d d88d 4940 9485 9452  ..1@J.r...I@...R
+00000800: 9475 7375 4add 76cb 0e7d 944a 84cd 7c0e  .usuJ.v..}.J..|.
+00000810: 7d94 4b00 7d94 2868 204a 4ec9 5901 6822  }.K.}.(h JN.Y.h"
+00000820: 6864 6824 6865 6826 6866 6828 6867 682a  hdh$heh&hfh(hgh*
+00000830: 6868 6821 8968 2c88 682d 6830 6836 4308  hhh!.h,.h-h0h6C.
+00000840: e17a 14ae 4729 5a40 9486 9452 9468 3c68  .z..G)Z@...R.h<h
+00000850: 3f43 6901 0200 0000 0600 0000 91d1 a68f  ?Ci.............
+00000860: 651a 3140 d261 742f e68d 4940 0429 67de  e.1@.at/..I@.)g.
+00000870: 601a 3140 0d66 b8a6 e58d 4940 d23e b1a9  `.1@.f....I@.>..
+00000880: 4e1a 3140 2c85 9be7 e38d 4940 1230 babc  N.1@,.....I@.0..
+00000890: 391a 3140 09e3 022b e28d 4940 95f6 6118  9.1@...+..I@..a.
+000008a0: 0b1a 3140 4cb0 ee0e df8d 4940 1558 0053  ..1@L.....I@.X.S
+000008b0: 061a 3140 e718 90bd de8d 4940 9485 9452  ..1@......I@...R
+000008c0: 9475 7373 4afa 286f 127d 9428 4a16 296f  .ussJ.(o.}.(J.)o
+000008d0: 127d 944b 007d 9428 6820 4ae2 a4ad 0168  .}.K.}.(h J....h
+000008e0: 228c 1c50 75c5 826b 6f77 6e69 6b61 2046  "..Pu..kownika F
+000008f0: 7261 6e63 6973 7a6b 6120 4e75 6c6c 6194  ranciszka Nulla.
+00000900: 6824 8c0b 7265 7369 6465 6e74 6961 6c94  h$..residential.
+00000910: 6826 8c02 3330 9468 2189 682c 8968 2d68  h&..30.h!.h,.h-h
+00000920: 3068 3643 08ed 51b8 1e85 d364 4094 8694  0h6C..Q....d@...
+00000930: 5294 683c 683f 43a9 0102 0000 000a 0000  R.h<h?C.........
+00000940: 0070 62a3 0799 1931 404a af72 0dd8 8d49  .pb....1@J.r...I
+00000950: 40ee 2763 7c98 1931 4008 0264 e8d8 8d49  @.'c|..1@..d...I
+00000960: 407e 1ccd 9195 1931 4089 44a1 65dd 8d49  @~.....1@.D.e..I
+00000970: 40f5 dc9d 1095 1931 40be e199 2bde 8d49  @......1@...+..I
+00000980: 4043 1ec1 8d94 1931 4046 7ded f4de 8d49  @C.....1@F}....I
+00000990: 401c c2e7 3d84 1931 408d 77ec 0cf8 8d49  @...=..1@.w....I
+000009a0: 404d ae18 6481 1931 40de 077b 6efc 8d49  @M..d..1@..{n..I
+000009b0: 40cd 4301 367b 1931 40f1 dd41 4706 8e49  @.C.6{.1@..AG..I
+000009c0: 40c7 e2ed f77a 1931 4020 ec14 ab06 8e49  @....z.1@ .....I
+000009d0: 4068 c647 307a 1931 404f 6a79 2f08 8e49  @h.G0z.1@Ojy/..I
+000009e0: 4094 8594 5294 7573 4a84 cd7c 0e7d 944b  @...R.usJ..|.}.K
+000009f0: 007d 9428 6820 4ae5 a4ad 0168 2268 7168  .}.(h J....h"hqh
+00000a00: 2468 7268 2189 682c 8868 2d68 3068 3643  $hrh!.h,.h-h0h6C
+00000a10: 0838 b4c8 76be a75d 4094 8694 5294 683c  .8..v..]@...R.h<
+00000a20: 683f 4389 0102 0000 0008 0000 0070 62a3  h?C..........pb.
+00000a30: 0799 1931 404a af72 0dd8 8d49 4016 e357  ...1@J.r...I@..W
+00000a40: 079b 1931 40cd 5f7c 2cd8 8d49 40b0 e99c  ...1@._|,..I@...
+00000a50: fa9b 1931 4044 d895 3bd8 8d49 40c5 67fc  ...1@D..;..I@.g.
+00000a60: 0cb9 1931 40f6 3416 03da 8d49 4043 1d56  ...1@.4....I@C.V
+00000a70: b8e5 1931 40d7 57b2 bedc 8d49 406a aa82  ...1@.W....I@j..
+00000a80: ac02 1a31 405f 3585 84de 8d49 40a5 a88e  ...1@_5....I@...
+00000a90: b003 1a31 406a 6d75 94de 8d49 4015 5800  ...1@jmu...I@.X.
+00000aa0: 5306 1a31 40e7 1890 bdde 8d49 4094 8594  S..1@......I@...
+00000ab0: 5294 7573 754a 1629 6f12 7d94 284a 83cd  R.usuJ.)o.}.(J..
+00000ac0: 7c0e 7d94 4b00 7d94 2868 204a 4cc9 5901  |.}.K.}.(h JL.Y.
+00000ad0: 6821 8868 2268 2368 2468 2568 2668 2768  h!.h"h#h$h%h&h'h
+00000ae0: 2868 2968 2a68 2b68 2c89 682d 6830 6836  (h)h*h+h,.h-h0h6
+00000af0: 4308 9543 8b6c e783 5d40 9486 9452 9468  C..C.l..]@...R.h
+00000b00: 3c68 3f43 4901 0200 0000 0400 0000 68c6  <h?CI.........h.
+00000b10: 4730 7a19 3140 4f6a 792f 088e 4940 ee7d  G0z.1@Ojy/..I@.}
+00000b20: 05c4 7f19 3140 d87b 968c 088e 4940 8738  ....1@.{....I@.8
+00000b30: 317f e019 3140 46d7 e0d8 0e8e 4940 d71e  1...1@F.....I@..
+00000b40: acb5 e619 3140 c9e3 0e40 0f8e 4940 9485  ....1@...@..I@..
+00000b50: 9452 9475 734a fa28 6f12 7d94 4b00 7d94  .R.usJ.(o.}.K.}.
+00000b60: 2868 204a e2a4 ad01 6822 6885 6824 6886  (h J....h"h.h$h.
+00000b70: 6826 6887 6821 8968 2c88 682d 6830 6836  h&h.h!.h,.h-h0h6
+00000b80: 4308 eb51 b81e 85d3 6440 9486 9452 9468  C..Q....d@...R.h
+00000b90: 3c68 3f43 a901 0200 0000 0a00 0000 68c6  <h?C..........h.
+00000ba0: 4730 7a19 3140 4f6a 792f 088e 4940 c7e2  G0z.1@Ojy/..I@..
+00000bb0: edf7 7a19 3140 20ec 14ab 068e 4940 cd43  ..z.1@ .....I@.C
+00000bc0: 0136 7b19 3140 f1dd 4147 068e 4940 4dae  .6{.1@..AG..I@M.
+00000bd0: 1864 8119 3140 de07 7b6e fc8d 4940 1cc2  .d..1@..{n..I@..
+00000be0: e73d 8419 3140 8d77 ec0c f88d 4940 431e  .=..1@.w....I@C.
+00000bf0: c18d 9419 3140 467d edf4 de8d 4940 f5dc  ....1@F}....I@..
+00000c00: 9d10 9519 3140 bee1 992b de8d 4940 7e1c  ....1@...+..I@~.
+00000c10: cd91 9519 3140 8944 a165 dd8d 4940 ee27  ....1@.D.e..I@.'
+00000c20: 637c 9819 3140 0802 64e8 d88d 4940 7062  c|..1@..d...I@pb
+00000c30: a307 9919 3140 4aaf 720d d88d 4940 9485  ....1@J.r...I@..
+00000c40: 9452 9475 7375 8a05 0055 a8b2 007d 944a  .R.usu...U...}.J
+00000c50: 84cd 7c0e 7d94 4b00 7d94 2868 205d 9428  ..|.}.K.}.(h ].(
+00000c60: 4a4d c959 014a 0d71 751e 6568 228c 1041  JM.Y.J.qu.eh"..A
+00000c70: 6e64 727a 656a 6120 506f 7465 626e 6994  ndrzeja Potebni.
+00000c80: 6824 8c0b 7265 7369 6465 6e74 6961 6c94  h$..residential.
+00000c90: 6826 8c02 3330 9468 288c 0761 7370 6861  h&..30.h(..aspha
+00000ca0: 6c74 9468 2a68 5668 2189 682c 8868 2d68  lt.h*hVh!.h,.h-h
+00000cb0: 3068 3643 086e 1283 c0ca b16a 4094 8694  0h6C.n.....j@...
+00000cc0: 5294 683c 683f 4379 0102 0000 0007 0000  R.h<h?Cy........
+00000cd0: 002e bb71 9c25 1a31 4072 497a bda0 8d49  ...q.%.1@rIz...I
+00000ce0: 4040 ca3e 7e25 1a31 40dd f934 dda1 8d49  @@.>~%.1@..4...I
+00000cf0: 4082 5da8 5725 1a31 402f c445 49a3 8d49  @.].W%.1@/.EI..I
+00000d00: 40b1 e144 4f25 1a31 4041 5d49 97a3 8d49  @..DO%.1@A]I...I
+00000d10: 40f9 090c fe23 1a31 40be 0ba5 40b0 8d49  @....#.1@...@..I
+00000d20: 40f0 f1ae 1f07 1a31 40d0 381e 7ddd 8d49  @......1@.8.}..I
+00000d30: 4015 5800 5306 1a31 40e7 1890 bdde 8d49  @.X.S..1@......I
+00000d40: 4094 8594 5294 7573 7375 8c05 5f73 7563  @...R.ussu.._suc
+00000d50: 6394 681b 8c05 5f70 7265 6494 7d94 284a  c.h..._pred.}.(J
+00000d60: 82cd 7c0e 7d94 4a83 cd7c 0e68 1e73 4a83  ..|.}.J..|.h.sJ.
+00000d70: cd7c 0e7d 9428 4a84 cd7c 0e68 5a4a 1629  .|.}.(J..|.hZJ.)
+00000d80: 6f12 6897 754a 84cd 7c0e 7d94 284a 83cd  o.h.uJ..|.}.(J..
+00000d90: 7c0e 6843 4add 76cb 0e68 7a4a fa28 6f12  |.hCJ.v..hzJ.(o.
+00000da0: 688e 8a05 0055 a8b2 0068 a875 4add 76cb  h....U...h.uJ.v.
+00000db0: 0e7d 944a 84cd 7c0e 6862 734a fa28 6f12  .}.J..|.hbsJ.(o.
+00000dc0: 7d94 284a 84cd 7c0e 686f 4a16 296f 1268  }.(J..|.hoJ.)o.h
+00000dd0: 9f75 4a16 296f 127d 944a fa28 6f12 6883  .uJ.)o.}.J.(o.h.
+00000de0: 738a 0500 55a8 b200 7d94 4a84 cd7c 0e68  s...U...}.J..|.h
+00000df0: 5073 758c 0361 646a 948c 1a6e 6574 776f  Psu..adj...netwo
+00000e00: 726b 782e 636c 6173 7365 732e 636f 7265  rkx.classes.core
+00000e10: 7669 6577 7394 8c12 4d75 6c74 6941 646a  views...MultiAdj
+00000e20: 6163 656e 6379 5669 6577 9493 9429 8194  acencyView...)..
+00000e30: 7d94 8c06 5f61 746c 6173 9468 1b73 628c  }..._atlas.h.sb.
+00000e40: 056e 6f64 6573 948c 1c6e 6574 776f 726b  .nodes...network
+00000e50: 782e 636c 6173 7365 732e 7265 706f 7274  x.classes.report
+00000e60: 7669 6577 7394 8c08 4e6f 6465 5669 6577  views...NodeView
+00000e70: 9493 9429 8194 7d94 8c06 5f6e 6f64 6573  ...)..}..._nodes
+00000e80: 9468 0f73 628c 0473 7563 6394 68c2 2981  .h.sb..succ.h.).
+00000e90: 947d 9468 c568 1b73 628c 0565 6467 6573  .}.h.h.sb..edges
+00000ea0: 9468 c78c 104f 7574 4d75 6c74 6945 6467  .h...OutMultiEdg
+00000eb0: 6556 6965 7794 9394 2981 947d 9428 8c06  eView...)..}.(..
+00000ec0: 5f67 7261 7068 9468 038c 085f 6164 6a64  _graph.h..._adjd
+00000ed0: 6963 7494 681b 7562 7562 2e              ict.h.ubub.
```

### Comparing `srai-0.2.0/tests/loaders/osm_way_loader/files/7be5387a594790ea98ef0bd07bfcb58e.pkl` & `srai-0.3.0/tests/loaders/osm_way_loader/test_files/graph_3.pkl`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 95ea 1300 0000 0000 008c 1d6e 6574  .............net
+00000000: 8004 95e0 1300 0000 0000 008c 1d6e 6574  .............net
 00000010: 776f 726b 782e 636c 6173 7365 732e 6d75  workx.classes.mu
 00000020: 6c74 6964 6967 7261 7068 948c 0c4d 756c  ltidigraph...Mul
 00000030: 7469 4469 4772 6170 6894 9394 2981 947d  tiDiGraph...)..}
 00000040: 9428 8c05 6772 6170 6894 7d94 288c 0c63  .(..graph.}.(..c
 00000050: 7265 6174 6564 5f64 6174 6594 8c13 3230  reated_date...20
 00000060: 3233 2d30 332d 3134 2032 333a 3237 3a35  23-03-14 23:27:5
 00000070: 3794 8c0c 6372 6561 7465 645f 7769 7468  7...created_with
@@ -49,272 +49,271 @@
 00000300: 156e 756d 7079 2e63 6f72 652e 6d75 6c74  .numpy.core.mult
 00000310: 6961 7272 6179 948c 0673 6361 6c61 7294  iarray...scalar.
 00000320: 9394 8c05 6e75 6d70 7994 8c05 6474 7970  ....numpy...dtyp
 00000330: 6594 9394 8c02 6638 9489 8887 9452 9428  e.....f8.....R.(
 00000340: 4b03 8c01 3c94 4e4e 4e4a ffff ffff 4aff  K...<.NNNJ....J.
 00000350: ffff ff4b 0074 9462 4308 3333 3333 3323  ...K.t.bC.33333#
 00000360: 5440 9486 9452 948c 0867 656f 6d65 7472  T@...R...geometr
-00000370: 7994 8c1b 7368 6170 656c 792e 6765 6f6d  y...shapely.geom
-00000380: 6574 7279 2e6c 696e 6573 7472 696e 6794  etry.linestring.
-00000390: 8c0a 4c69 6e65 5374 7269 6e67 9493 9429  ..LineString...)
-000003a0: 5294 4359 0102 0000 0005 0000 00d7 1eac  R.CY............
-000003b0: b5e6 1931 40c9 e30e 400f 8e49 40aa 9b8b  ...1@...@..I@...
-000003c0: bfed 1931 4087 acc9 ae0f 8e49 40b5 e1b0  ...1@......I@...
-000003d0: 34f0 1931 40da d836 d60f 8e49 4091 4028  4..1@..6...I@.@(
-000003e0: 942a 1a31 40af 0562 7e13 8e49 40d5 1cc5  .*.1@..b~..I@...
-000003f0: de30 1a31 4073 d30b e313 8e49 4094 6275  .0.1@s.....I@.bu
-00000400: 734a 84cd 7c0e 7d94 4b00 7d94 2868 244a  sJ..|.}.K.}.(h$J
-00000410: 4dc9 5901 6826 8c10 416e 6472 7a65 6a61  M.Y.h&..Andrzeja
-00000420: 2050 6f74 6562 6e69 9468 288c 0b72 6573   Potebni.h(..res
-00000430: 6964 656e 7469 616c 9468 2a8c 0233 3094  idential.h*..30.
-00000440: 682c 8c07 6173 7068 616c 7494 6825 8968  h,..asphalt.h%.h
-00000450: 3089 6831 6834 683a 4308 dcf9 7e6a bc00  0.h1h4h:C...~j..
-00000460: 6540 9486 9452 9468 4068 4329 5294 4399  e@...R.h@hC)R.C.
-00000470: 0102 0000 0009 0000 00d7 1eac b5e6 1931  ...............1
-00000480: 40c9 e30e 400f 8e49 40ef a2f9 ade7 1931  @...@..I@......1
-00000490: 4046 674f b80d 8e49 402a 8d98 d9e7 1931  @FgO...I@*.....1
-000004a0: 401d 8c7d 6e0d 8e49 4037 1cf1 bff0 1931  @..}n..I@7.....1
-000004b0: 40a1 3f7e 80ff 8d49 4031 7326 12f1 1931  @.?~...I@1s&...1
-000004c0: 40ad bf25 00ff 8d49 4049 e306 32f1 1931  @..%...I@I..2..1
-000004d0: 400d 9a4c cbfe 8d49 4073 bed8 7bf1 1931  @..L...I@s..{..1
-000004e0: 4090 920d 5afe 8d49 40f7 cec3 6405 1a31  @...Z..I@...d..1
-000004f0: 407b a41c 27e0 8d49 4015 5800 5306 1a31  @{..'..I@.X.S..1
-00000500: 40e7 1890 bdde 8d49 4094 6275 7375 4a84  @......I@.busuJ.
-00000510: cd7c 0e7d 9428 8a05 0055 a8b2 007d 944b  .|.}.(...U...}.K
-00000520: 007d 9428 6824 5d94 284a 0d71 751e 4a4d  .}.(h$].(J.qu.JM
-00000530: c959 0165 6826 6848 6828 6849 682a 684a  .Y.eh&hHh(hIh*hJ
-00000540: 682c 684b 6825 8968 3089 6831 6834 683a  h,hKh%.h0.h1h4h:
-00000550: 4308 6f12 83c0 cab1 6a40 9486 9452 9468  C.o.....j@...R.h
-00000560: 2e8c 0379 6573 9468 4068 4329 5294 4379  ...yes.h@hC)R.Cy
-00000570: 0102 0000 0007 0000 0015 5800 5306 1a31  ..........X.S..1
-00000580: 40e7 1890 bdde 8d49 40f0 f1ae 1f07 1a31  @......I@......1
-00000590: 40d0 381e 7ddd 8d49 40f9 090c fe23 1a31  @.8.}..I@....#.1
-000005a0: 40be 0ba5 40b0 8d49 40b1 e144 4f25 1a31  @...@..I@..DO%.1
-000005b0: 4041 5d49 97a3 8d49 4082 5da8 5725 1a31  @A]I...I@.].W%.1
-000005c0: 402f c445 49a3 8d49 4040 ca3e 7e25 1a31  @/.EI..I@@.>~%.1
-000005d0: 40dd f934 dda1 8d49 402e bb71 9c25 1a31  @..4...I@..q.%.1
-000005e0: 4072 497a bda0 8d49 4094 6275 734a 83cd  @rIz...I@.busJ..
-000005f0: 7c0e 7d94 4b00 7d94 2868 244a 4dc9 5901  |.}.K.}.(h$JM.Y.
-00000600: 6826 6848 6828 6849 682a 684a 682c 684b  h&hHh(hIh*hJh,hK
-00000610: 6825 8968 3088 6831 6834 683a 4308 dbf9  h%.h0.h1h4h:C...
-00000620: 7e6a bc00 6540 9486 9452 9468 4068 4329  ~j..e@...R.h@hC)
-00000630: 5294 4399 0102 0000 0009 0000 0015 5800  R.C...........X.
-00000640: 5306 1a31 40e7 1890 bdde 8d49 40f7 cec3  S..1@......I@...
-00000650: 6405 1a31 407b a41c 27e0 8d49 4073 bed8  d..1@{..'..I@s..
-00000660: 7bf1 1931 4090 920d 5afe 8d49 4049 e306  {..1@...Z..I@I..
-00000670: 32f1 1931 400d 9a4c cbfe 8d49 4031 7326  2..1@..L...I@1s&
-00000680: 12f1 1931 40ad bf25 00ff 8d49 4037 1cf1  ...1@..%...I@7..
-00000690: bff0 1931 40a1 3f7e 80ff 8d49 402a 8d98  ...1@.?~...I@*..
-000006a0: d9e7 1931 401d 8c7d 6e0d 8e49 40ef a2f9  ...1@..}n..I@...
-000006b0: ade7 1931 4046 674f b80d 8e49 40d7 1eac  ...1@FgO...I@...
-000006c0: b5e6 1931 40c9 e30e 400f 8e49 4094 6275  ...1@...@..I@.bu
-000006d0: 734a dd76 cb0e 7d94 4b00 7d94 2868 244a  sJ.v..}.K.}.(h$J
-000006e0: 4ec9 5901 6826 8c11 5069 6572 7773 7a65  N.Y.h&..Pierwsze
-000006f0: 6a20 4479 7769 7a6a 6994 6828 8c0b 7265  j Dywizji.h(..re
-00000700: 7369 6465 6e74 6961 6c94 682a 8c02 3330  sidential.h*..30
-00000710: 9468 2c8c 0761 7370 6861 6c74 9468 2e8c  .h,..asphalt.h..
-00000720: 0379 6573 9468 2589 6830 8968 3168 3468  .yes.h%.h0.h1h4h
-00000730: 3a43 08e2 7a14 ae47 295a 4094 8694 5294  :C..z..G)Z@...R.
-00000740: 6840 6843 2952 9443 6901 0200 0000 0600  h@hC)R.Ci.......
-00000750: 0000 1558 0053 061a 3140 e718 90bd de8d  ...X.S..1@......
-00000760: 4940 95f6 6118 0b1a 3140 4cb0 ee0e df8d  I@..a...1@L.....
-00000770: 4940 1230 babc 391a 3140 09e3 022b e28d  I@.0..9.1@...+..
-00000780: 4940 d23e b1a9 4e1a 3140 2c85 9be7 e38d  I@.>..N.1@,.....
-00000790: 4940 0429 67de 601a 3140 0d66 b8a6 e58d  I@.)g.`.1@.f....
-000007a0: 4940 91d1 a68f 651a 3140 d261 742f e68d  I@....e.1@.at/..
-000007b0: 4940 9462 7573 4afa 286f 127d 944b 007d  I@.busJ.(o.}.K.}
-000007c0: 9428 6824 4ae5 a4ad 0168 268c 1150 6965  .(h$J....h&..Pie
-000007d0: 7277 737a 656a 2044 7977 697a 6a69 9468  rwszej Dywizji.h
-000007e0: 288c 0d6c 6976 696e 675f 7374 7265 6574  (..living_street
-000007f0: 9468 2589 6830 8968 3168 3468 3a43 0838  .h%.h0.h1h4h:C.8
-00000800: b4c8 76be a75d 4094 8694 5294 6840 6843  ..v..]@...R.h@hC
-00000810: 2952 9443 8901 0200 0000 0800 0000 1558  )R.C...........X
-00000820: 0053 061a 3140 e718 90bd de8d 4940 a5a8  .S..1@......I@..
-00000830: 8eb0 031a 3140 6a6d 7594 de8d 4940 6aaa  ....1@jmu...I@j.
-00000840: 82ac 021a 3140 5f35 8584 de8d 4940 431d  ....1@_5....I@C.
-00000850: 56b8 e519 3140 d757 b2be dc8d 4940 c567  V...1@.W....I@.g
-00000860: fc0c b919 3140 f634 1603 da8d 4940 b0e9  ....1@.4....I@..
-00000870: 9cfa 9b19 3140 44d8 953b d88d 4940 16e3  ....1@D..;..I@..
-00000880: 5707 9b19 3140 cd5f 7c2c d88d 4940 7062  W...1@._|,..I@pb
-00000890: a307 9919 3140 4aaf 720d d88d 4940 9462  ....1@J.r...I@.b
-000008a0: 7573 754a dd76 cb0e 7d94 4a84 cd7c 0e7d  usuJ.v..}.J..|.}
-000008b0: 944b 007d 9428 6824 4a4e c959 0168 2668  .K.}.(h$JN.Y.h&h
-000008c0: 6468 2868 6568 2a68 6668 2c68 6768 2e68  dh(heh*hfh,hgh.h
-000008d0: 6868 2589 6830 8868 3168 3468 3a43 08e1  hh%.h0.h1h4h:C..
-000008e0: 7a14 ae47 295a 4094 8694 5294 6840 6843  z..G)Z@...R.h@hC
-000008f0: 2952 9443 6901 0200 0000 0600 0000 91d1  )R.Ci...........
-00000900: a68f 651a 3140 d261 742f e68d 4940 0429  ..e.1@.at/..I@.)
-00000910: 67de 601a 3140 0d66 b8a6 e58d 4940 d23e  g.`.1@.f....I@.>
-00000920: b1a9 4e1a 3140 2c85 9be7 e38d 4940 1230  ..N.1@,.....I@.0
-00000930: babc 391a 3140 09e3 022b e28d 4940 95f6  ..9.1@...+..I@..
-00000940: 6118 0b1a 3140 4cb0 ee0e df8d 4940 1558  a...1@L.....I@.X
-00000950: 0053 061a 3140 e718 90bd de8d 4940 9462  .S..1@......I@.b
-00000960: 7573 734a 9928 6f12 7d94 4a9a 286f 127d  ussJ.(o.}.J.(o.}
-00000970: 944b 007d 9428 6824 4af0 a4ad 0168 268c  .K.}.(h$J....h&.
-00000980: 1753 7465 6661 6e69 6920 5365 6d70 6fc5  .Stefanii Sempo.
-00000990: 826f 7773 6b69 656a 9468 288c 0b72 6573  .owskiej.h(..res
-000009a0: 6964 656e 7469 616c 9468 2a8c 0233 3094  idential.h*..30.
-000009b0: 682c 8c07 6173 7068 616c 7494 682e 8c03  h,..asphalt.h...
-000009c0: 7965 7394 6825 8968 3089 6831 6834 683a  yes.h%.h0.h1h4h:
-000009d0: 4308 0781 9543 8bcc 5740 9486 9452 9468  C....C..W@...R.h
-000009e0: 4068 4329 5294 4349 0102 0000 0004 0000  @hC)R.CI........
-000009f0: 0087 7945 a632 1931 407d fe20 3768 8d49  ..yE.2.1@}. 7h.I
-00000a00: 40f4 22c9 6251 1931 40a7 21aa f067 8d49  @.".bQ.1@.!..g.I
-00000a10: 406a 23e8 7981 1931 409c 7928 c066 8d49  @j#.y..1@.y(.f.I
-00000a20: 401e 7bac cf8b 1931 4043 1aba 7e66 8d49  @.{....1@C..~f.I
-00000a30: 4094 6275 7373 4a9a 286f 127d 9428 4aa6  @.bussJ.(o.}.(J.
-00000a40: 286f 127d 944b 007d 9428 6824 4ad0 a4ad  (o.}.K.}.(h$J...
-00000a50: 0168 268c 104a 616e 7573 7a61 204b 6f72  .h&..Janusza Kor
-00000a60: 637a 616b 6194 6828 8c0b 7265 7369 6465  czaka.h(..reside
-00000a70: 6e74 6961 6c94 682a 8c02 3330 9468 2c8c  ntial.h*..30.h,.
-00000a80: 0761 7370 6861 6c74 9468 2e8c 0379 6573  .asphalt.h...yes
-00000a90: 9468 2589 6830 8968 3168 3468 3a43 0875  .h%.h0.h1h4h:C.u
-00000aa0: 9318 0456 3e5f 4094 8694 5294 6840 6843  ...V>_@...R.h@hC
-00000ab0: 2952 9443 5901 0200 0000 0500 0000 1e7b  )R.CY..........{
-00000ac0: accf 8b19 3140 431a ba7e 668d 4940 dd1b  ....1@C..~f.I@..
-00000ad0: 8d8d 8a19 3140 e48d 8296 648d 4940 12ef  ....1@....d.I@..
-00000ae0: 4adc 7419 3140 01ba d4ad 438d 4940 d604  J.t.1@....C.I@..
-00000af0: acb0 7419 3140 7edb b86a 438d 4940 b9d7  ..t.1@~..jC.I@..
-00000b00: 930a 7419 3140 7f99 396e 428d 4940 9462  ..t.1@..9nB.I@.b
-00000b10: 7573 4a9c 286f 127d 944b 007d 9428 6824  usJ.(o.}.K.}.(h$
-00000b20: 4af0 a4ad 0168 2668 8268 2868 8368 2a68  J....h&h.h(h.h*h
-00000b30: 8468 2c68 8568 2e68 8668 2589 6830 8968  .h,h.h.h.h%.h0.h
-00000b40: 3168 3468 3a43 08de 2406 8195 1354 4094  1h4h:C..$....T@.
-00000b50: 8694 5294 6840 6843 2952 9443 4901 0200  ..R.h@hC)R.CI...
-00000b60: 0000 0400 0000 1e7b accf 8b19 3140 431a  .......{....1@C.
-00000b70: ba7e 668d 4940 2d16 759c 9119 3140 6c6b  .~f.I@-.u...1@lk
-00000b80: 555c 668d 4940 8506 62d9 cc19 3140 8b42  U\f.I@..b...1@.B
-00000b90: 812d 658d 4940 7af1 8f08 d719 3140 ea1c  .-e.I@z.....1@..
-00000ba0: a8f8 648d 4940 9462 7573 4a99 286f 127d  ..d.I@.busJ.(o.}
-00000bb0: 944b 007d 9428 6824 4af0 a4ad 0168 2668  .K.}.(h$J....h&h
-00000bc0: 8268 2868 8368 2a68 8468 2c68 8568 2e68  .h(h.h*h.h,h.h.h
-00000bd0: 8668 2589 6830 8868 3168 3468 3a43 0806  .h%.h0.h1h4h:C..
-00000be0: 8195 438b cc57 4094 8694 5294 6840 6843  ..C..W@...R.h@hC
-00000bf0: 2952 9443 4901 0200 0000 0400 0000 1e7b  )R.CI..........{
-00000c00: accf 8b19 3140 431a ba7e 668d 4940 6a23  ....1@C..~f.I@j#
-00000c10: e879 8119 3140 9c79 28c0 668d 4940 f422  .y..1@.y(.f.I@."
-00000c20: c962 5119 3140 a721 aaf0 678d 4940 8779  .bQ.1@.!..g.I@.y
-00000c30: 45a6 3219 3140 7dfe 2037 688d 4940 9462  E.2.1@}. 7h.I@.b
-00000c40: 7573 754a 9c28 6f12 7d94 4a9a 286f 127d  usuJ.(o.}.J.(o.}
-00000c50: 944b 007d 9428 6824 4af0 a4ad 0168 2668  .K.}.(h$J....h&h
-00000c60: 8268 2868 8368 2a68 8468 2c68 8568 2e68  .h(h.h*h.h,h.h.h
-00000c70: 8668 2589 6830 8868 3168 3468 3a43 08dd  .h%.h0.h1h4h:C..
-00000c80: 2406 8195 1354 4094 8694 5294 6840 6843  $....T@...R.h@hC
-00000c90: 2952 9443 4901 0200 0000 0400 0000 7af1  )R.CI.........z.
-00000ca0: 8f08 d719 3140 ea1c a8f8 648d 4940 8506  ....1@....d.I@..
-00000cb0: 62d9 cc19 3140 8b42 812d 658d 4940 2d16  b...1@.B.-e.I@-.
-00000cc0: 759c 9119 3140 6c6b 555c 668d 4940 1e7b  u...1@lkU\f.I@.{
-00000cd0: accf 8b19 3140 431a ba7e 668d 4940 9462  ....1@C..~f.I@.b
-00000ce0: 7573 734a a628 6f12 7d94 4a9a 286f 127d  ussJ.(o.}.J.(o.}
-00000cf0: 944b 007d 9428 6824 4ad0 a4ad 0168 2668  .K.}.(h$J....h&h
-00000d00: 8f68 2868 9068 2a68 9168 2c68 9268 2e68  .h(h.h*h.h,h.h.h
-00000d10: 9368 2589 6830 8868 3168 3468 3a43 0875  .h%.h0.h1h4h:C.u
-00000d20: 9318 0456 3e5f 4094 8694 5294 6840 6843  ...V>_@...R.h@hC
-00000d30: 2952 9443 5901 0200 0000 0500 0000 b9d7  )R.CY...........
-00000d40: 930a 7419 3140 7f99 396e 428d 4940 d604  ..t.1@..9nB.I@..
-00000d50: acb0 7419 3140 7edb b86a 438d 4940 12ef  ..t.1@~..jC.I@..
-00000d60: 4adc 7419 3140 01ba d4ad 438d 4940 dd1b  J.t.1@....C.I@..
-00000d70: 8d8d 8a19 3140 e48d 8296 648d 4940 1e7b  ....1@....d.I@.{
-00000d80: accf 8b19 3140 431a ba7e 668d 4940 9462  ....1@C..~f.I@.b
-00000d90: 7573 734a fa28 6f12 7d94 284a 1629 6f12  ussJ.(o.}.(J.)o.
-00000da0: 7d94 4b00 7d94 2868 244a e2a4 ad01 6826  }.K.}.(h$J....h&
-00000db0: 8c1c 5075 c582 6b6f 776e 696b 6120 4672  ..Pu..kownika Fr
-00000dc0: 616e 6369 737a 6b61 204e 756c 6c61 9468  anciszka Nulla.h
-00000dd0: 288c 0b72 6573 6964 656e 7469 616c 9468  (..residential.h
-00000de0: 2a8c 0233 3094 6825 8968 3089 6831 6834  *..30.h%.h0.h1h4
-00000df0: 683a 4308 ed51 b81e 85d3 6440 9486 9452  h:C..Q....d@...R
-00000e00: 9468 4068 4329 5294 43a9 0102 0000 000a  .h@hC)R.C.......
-00000e10: 0000 0070 62a3 0799 1931 404a af72 0dd8  ...pb....1@J.r..
-00000e20: 8d49 40ee 2763 7c98 1931 4008 0264 e8d8  .I@.'c|..1@..d..
-00000e30: 8d49 407e 1ccd 9195 1931 4089 44a1 65dd  .I@~.....1@.D.e.
-00000e40: 8d49 40f5 dc9d 1095 1931 40be e199 2bde  .I@......1@...+.
-00000e50: 8d49 4043 1ec1 8d94 1931 4046 7ded f4de  .I@C.....1@F}...
-00000e60: 8d49 401c c2e7 3d84 1931 408d 77ec 0cf8  .I@...=..1@.w...
-00000e70: 8d49 404d ae18 6481 1931 40de 077b 6efc  .I@M..d..1@..{n.
-00000e80: 8d49 40cd 4301 367b 1931 40f1 dd41 4706  .I@.C.6{.1@..AG.
-00000e90: 8e49 40c7 e2ed f77a 1931 4020 ec14 ab06  .I@....z.1@ ....
-00000ea0: 8e49 4068 c647 307a 1931 404f 6a79 2f08  .I@h.G0z.1@Ojy/.
-00000eb0: 8e49 4094 6275 734a 84cd 7c0e 7d94 4b00  .I@.busJ..|.}.K.
-00000ec0: 7d94 2868 244a e5a4 ad01 6826 6870 6828  }.(h$J....h&hph(
-00000ed0: 6871 6825 8968 3088 6831 6834 683a 4308  hqh%.h0.h1h4h:C.
-00000ee0: 38b4 c876 bea7 5d40 9486 9452 9468 4068  8..v..]@...R.h@h
-00000ef0: 4329 5294 4389 0102 0000 0008 0000 0070  C)R.C..........p
-00000f00: 62a3 0799 1931 404a af72 0dd8 8d49 4016  b....1@J.r...I@.
-00000f10: e357 079b 1931 40cd 5f7c 2cd8 8d49 40b0  .W...1@._|,..I@.
-00000f20: e99c fa9b 1931 4044 d895 3bd8 8d49 40c5  .....1@D..;..I@.
-00000f30: 67fc 0cb9 1931 40f6 3416 03da 8d49 4043  g....1@.4....I@C
-00000f40: 1d56 b8e5 1931 40d7 57b2 bedc 8d49 406a  .V...1@.W....I@j
-00000f50: aa82 ac02 1a31 405f 3585 84de 8d49 40a5  .....1@_5....I@.
-00000f60: a88e b003 1a31 406a 6d75 94de 8d49 4015  .....1@jmu...I@.
-00000f70: 5800 5306 1a31 40e7 1890 bdde 8d49 4094  X.S..1@......I@.
-00000f80: 6275 7375 4a16 296f 127d 9428 4a83 cd7c  busuJ.)o.}.(J..|
-00000f90: 0e7d 944b 007d 9428 6824 4a4c c959 0168  .}.K.}.(h$JL.Y.h
-00000fa0: 2588 6826 6827 6828 6829 682a 682b 682c  %.h&h'h(h)h*h+h,
-00000fb0: 682d 682e 682f 6830 8968 3168 3468 3a43  h-h.h/h0.h1h4h:C
-00000fc0: 0895 438b 6ce7 835d 4094 8694 5294 6840  ..C.l..]@...R.h@
-00000fd0: 6843 2952 9443 4901 0200 0000 0400 0000  hC)R.CI.........
-00000fe0: 68c6 4730 7a19 3140 4f6a 792f 088e 4940  h.G0z.1@Ojy/..I@
-00000ff0: ee7d 05c4 7f19 3140 d87b 968c 088e 4940  .}....1@.{....I@
-00001000: 8738 317f e019 3140 46d7 e0d8 0e8e 4940  .81...1@F.....I@
-00001010: d71e acb5 e619 3140 c9e3 0e40 0f8e 4940  ......1@...@..I@
-00001020: 9462 7573 4afa 286f 127d 944b 007d 9428  .busJ.(o.}.K.}.(
-00001030: 6824 4ae2 a4ad 0168 2668 ba68 2868 bb68  h$J....h&h.h(h.h
-00001040: 2a68 bc68 2589 6830 8868 3168 3468 3a43  *h.h%.h0.h1h4h:C
-00001050: 08eb 51b8 1e85 d364 4094 8694 5294 6840  ..Q....d@...R.h@
-00001060: 6843 2952 9443 a901 0200 0000 0a00 0000  hC)R.C..........
-00001070: 68c6 4730 7a19 3140 4f6a 792f 088e 4940  h.G0z.1@Ojy/..I@
-00001080: c7e2 edf7 7a19 3140 20ec 14ab 068e 4940  ....z.1@ .....I@
-00001090: cd43 0136 7b19 3140 f1dd 4147 068e 4940  .C.6{.1@..AG..I@
-000010a0: 4dae 1864 8119 3140 de07 7b6e fc8d 4940  M..d..1@..{n..I@
-000010b0: 1cc2 e73d 8419 3140 8d77 ec0c f88d 4940  ...=..1@.w....I@
-000010c0: 431e c18d 9419 3140 467d edf4 de8d 4940  C.....1@F}....I@
-000010d0: f5dc 9d10 9519 3140 bee1 992b de8d 4940  ......1@...+..I@
-000010e0: 7e1c cd91 9519 3140 8944 a165 dd8d 4940  ~.....1@.D.e..I@
-000010f0: ee27 637c 9819 3140 0802 64e8 d88d 4940  .'c|..1@..d...I@
-00001100: 7062 a307 9919 3140 4aaf 720d d88d 4940  pb....1@J.r...I@
-00001110: 9462 7573 758a 0500 55a8 b200 7d94 4a84  .busu...U...}.J.
-00001120: cd7c 0e7d 944b 007d 9428 6824 5d94 284a  .|.}.K.}.(h$].(J
-00001130: 4dc9 5901 4a0d 7175 1e65 6826 8c10 416e  M.Y.J.qu.eh&..An
-00001140: 6472 7a65 6a61 2050 6f74 6562 6e69 9468  drzeja Potebni.h
-00001150: 288c 0b72 6573 6964 656e 7469 616c 9468  (..residential.h
-00001160: 2a8c 0233 3094 682c 8c07 6173 7068 616c  *..30.h,..asphal
-00001170: 7494 682e 6858 6825 8968 3088 6831 6834  t.h.hXh%.h0.h1h4
-00001180: 683a 4308 6e12 83c0 cab1 6a40 9486 9452  h:C.n.....j@...R
-00001190: 9468 4068 4329 5294 4379 0102 0000 0007  .h@hC)R.Cy......
-000011a0: 0000 002e bb71 9c25 1a31 4072 497a bda0  .....q.%.1@rIz..
-000011b0: 8d49 4040 ca3e 7e25 1a31 40dd f934 dda1  .I@@.>~%.1@..4..
-000011c0: 8d49 4082 5da8 5725 1a31 402f c445 49a3  .I@.].W%.1@/.EI.
-000011d0: 8d49 40b1 e144 4f25 1a31 4041 5d49 97a3  .I@..DO%.1@A]I..
-000011e0: 8d49 40f9 090c fe23 1a31 40be 0ba5 40b0  .I@....#.1@...@.
-000011f0: 8d49 40f0 f1ae 1f07 1a31 40d0 381e 7ddd  .I@......1@.8.}.
-00001200: 8d49 4015 5800 5306 1a31 40e7 1890 bdde  .I@.X.S..1@.....
-00001210: 8d49 4094 6275 7373 758c 055f 7375 6363  .I@.bussu.._succ
-00001220: 9468 1f8c 055f 7072 6564 947d 9428 4a82  .h..._pred.}.(J.
-00001230: cd7c 0e7d 944a 83cd 7c0e 6822 734a 83cd  .|.}.J..|.h"sJ..
-00001240: 7c0e 7d94 284a 84cd 7c0e 685b 4a16 296f  |.}.(J..|.h[J.)o
-00001250: 1268 ca75 4a84 cd7c 0e7d 9428 4a83 cd7c  .h.uJ..|.}.(J..|
-00001260: 0e68 464a dd76 cb0e 6878 4afa 286f 1268  .hFJ.v..hxJ.(o.h
-00001270: c28a 0500 55a8 b200 68d9 754a dd76 cb0e  ....U...h.uJ.v..
-00001280: 7d94 4a84 cd7c 0e68 6273 4a99 286f 127d  }.J..|.hbsJ.(o.}
-00001290: 944a 9a28 6f12 68a0 734a 9a28 6f12 7d94  .J.(o.h.sJ.(o.}.
-000012a0: 284a 9928 6f12 6880 4a9c 286f 1268 a84a  (J.(o.h.J.(o.h.J
-000012b0: a628 6f12 68b0 754a 9c28 6f12 7d94 4a9a  .(o.h.uJ.(o.}.J.
-000012c0: 286f 1268 9973 4aa6 286f 127d 944a 9a28  (o.h.sJ.(o.}.J.(
-000012d0: 6f12 688d 734a fa28 6f12 7d94 284a 84cd  o.h.sJ.(o.}.(J..
-000012e0: 7c0e 686e 4a16 296f 1268 d175 4a16 296f  |.hnJ.)o.h.uJ.)o
-000012f0: 127d 944a fa28 6f12 68b8 738a 0500 55a8  .}.J.(o.h.s...U.
-00001300: b200 7d94 4a84 cd7c 0e68 5273 758c 0361  ..}.J..|.hRsu..a
-00001310: 646a 948c 1a6e 6574 776f 726b 782e 636c  dj...networkx.cl
-00001320: 6173 7365 732e 636f 7265 7669 6577 7394  asses.coreviews.
-00001330: 8c12 4d75 6c74 6941 646a 6163 656e 6379  ..MultiAdjacency
-00001340: 5669 6577 9493 9429 8194 7d94 8c06 5f61  View...)..}..._a
-00001350: 746c 6173 9468 1f73 628c 056e 6f64 6573  tlas.h.sb..nodes
-00001360: 948c 1c6e 6574 776f 726b 782e 636c 6173  ...networkx.clas
-00001370: 7365 732e 7265 706f 7274 7669 6577 7394  ses.reportviews.
-00001380: 8c08 4e6f 6465 5669 6577 9493 9429 8194  ..NodeView...)..
-00001390: 7d94 8c06 5f6e 6f64 6573 9468 0f73 628c  }..._nodes.h.sb.
-000013a0: 0473 7563 6394 68f6 2981 947d 9468 f968  .succ.h.)..}.h.h
-000013b0: 1f73 628c 0565 6467 6573 9468 fb8c 104f  .sb..edges.h...O
-000013c0: 7574 4d75 6c74 6945 6467 6556 6965 7794  utMultiEdgeView.
-000013d0: 9394 2981 947d 9428 8c06 5f67 7261 7068  ..)..}.(.._graph
-000013e0: 9468 038c 085f 6164 6a64 6963 7494 681f  .h..._adjdict.h.
-000013f0: 7562 7562 2e                             ubub.
+00000370: 7994 8c0a 7368 6170 656c 792e 696f 948c  y...shapely.io..
+00000380: 0866 726f 6d5f 776b 6294 9394 4359 0102  .from_wkb...CY..
+00000390: 0000 0005 0000 00d7 1eac b5e6 1931 40c9  .............1@.
+000003a0: e30e 400f 8e49 40aa 9b8b bfed 1931 4087  ..@..I@......1@.
+000003b0: acc9 ae0f 8e49 40b5 e1b0 34f0 1931 40da  .....I@...4..1@.
+000003c0: d836 d60f 8e49 4091 4028 942a 1a31 40af  .6...I@.@(.*.1@.
+000003d0: 0562 7e13 8e49 40d5 1cc5 de30 1a31 4073  .b~..I@....0.1@s
+000003e0: d30b e313 8e49 4094 8594 5294 7573 4a84  .....I@...R.usJ.
+000003f0: cd7c 0e7d 944b 007d 9428 6824 4a4d c959  .|.}.K.}.(h$JM.Y
+00000400: 0168 268c 1041 6e64 727a 656a 6120 506f  .h&..Andrzeja Po
+00000410: 7465 626e 6994 6828 8c0b 7265 7369 6465  tebni.h(..reside
+00000420: 6e74 6961 6c94 682a 8c02 3330 9468 2c8c  ntial.h*..30.h,.
+00000430: 0761 7370 6861 6c74 9468 2589 6830 8968  .asphalt.h%.h0.h
+00000440: 3168 3468 3a43 08dc f97e 6abc 0065 4094  1h4h:C...~j..e@.
+00000450: 8694 5294 6840 6843 4399 0102 0000 0009  ..R.h@hCC.......
+00000460: 0000 00d7 1eac b5e6 1931 40c9 e30e 400f  .........1@...@.
+00000470: 8e49 40ef a2f9 ade7 1931 4046 674f b80d  .I@......1@FgO..
+00000480: 8e49 402a 8d98 d9e7 1931 401d 8c7d 6e0d  .I@*.....1@..}n.
+00000490: 8e49 4037 1cf1 bff0 1931 40a1 3f7e 80ff  .I@7.....1@.?~..
+000004a0: 8d49 4031 7326 12f1 1931 40ad bf25 00ff  .I@1s&...1@..%..
+000004b0: 8d49 4049 e306 32f1 1931 400d 9a4c cbfe  .I@I..2..1@..L..
+000004c0: 8d49 4073 bed8 7bf1 1931 4090 920d 5afe  .I@s..{..1@...Z.
+000004d0: 8d49 40f7 cec3 6405 1a31 407b a41c 27e0  .I@...d..1@{..'.
+000004e0: 8d49 4015 5800 5306 1a31 40e7 1890 bdde  .I@.X.S..1@.....
+000004f0: 8d49 4094 8594 5294 7573 754a 84cd 7c0e  .I@...R.usuJ..|.
+00000500: 7d94 288a 0500 55a8 b200 7d94 4b00 7d94  }.(...U...}.K.}.
+00000510: 2868 245d 9428 4a0d 7175 1e4a 4dc9 5901  (h$].(J.qu.JM.Y.
+00000520: 6568 2668 4968 2868 4a68 2a68 4b68 2c68  eh&hIh(hJh*hKh,h
+00000530: 4c68 2589 6830 8968 3168 3468 3a43 086f  Lh%.h0.h1h4h:C.o
+00000540: 1283 c0ca b16a 4094 8694 5294 682e 8c03  .....j@...R.h...
+00000550: 7965 7394 6840 6843 4379 0102 0000 0007  yes.h@hCCy......
+00000560: 0000 0015 5800 5306 1a31 40e7 1890 bdde  ....X.S..1@.....
+00000570: 8d49 40f0 f1ae 1f07 1a31 40d0 381e 7ddd  .I@......1@.8.}.
+00000580: 8d49 40f9 090c fe23 1a31 40be 0ba5 40b0  .I@....#.1@...@.
+00000590: 8d49 40b1 e144 4f25 1a31 4041 5d49 97a3  .I@..DO%.1@A]I..
+000005a0: 8d49 4082 5da8 5725 1a31 402f c445 49a3  .I@.].W%.1@/.EI.
+000005b0: 8d49 4040 ca3e 7e25 1a31 40dd f934 dda1  .I@@.>~%.1@..4..
+000005c0: 8d49 402e bb71 9c25 1a31 4072 497a bda0  .I@..q.%.1@rIz..
+000005d0: 8d49 4094 8594 5294 7573 4a83 cd7c 0e7d  .I@...R.usJ..|.}
+000005e0: 944b 007d 9428 6824 4a4d c959 0168 2668  .K.}.(h$JM.Y.h&h
+000005f0: 4968 2868 4a68 2a68 4b68 2c68 4c68 2589  Ih(hJh*hKh,hLh%.
+00000600: 6830 8868 3168 3468 3a43 08db f97e 6abc  h0.h1h4h:C...~j.
+00000610: 0065 4094 8694 5294 6840 6843 4399 0102  .e@...R.h@hCC...
+00000620: 0000 0009 0000 0015 5800 5306 1a31 40e7  ........X.S..1@.
+00000630: 1890 bdde 8d49 40f7 cec3 6405 1a31 407b  .....I@...d..1@{
+00000640: a41c 27e0 8d49 4073 bed8 7bf1 1931 4090  ..'..I@s..{..1@.
+00000650: 920d 5afe 8d49 4049 e306 32f1 1931 400d  ..Z..I@I..2..1@.
+00000660: 9a4c cbfe 8d49 4031 7326 12f1 1931 40ad  .L...I@1s&...1@.
+00000670: bf25 00ff 8d49 4037 1cf1 bff0 1931 40a1  .%...I@7.....1@.
+00000680: 3f7e 80ff 8d49 402a 8d98 d9e7 1931 401d  ?~...I@*.....1@.
+00000690: 8c7d 6e0d 8e49 40ef a2f9 ade7 1931 4046  .}n..I@......1@F
+000006a0: 674f b80d 8e49 40d7 1eac b5e6 1931 40c9  gO...I@......1@.
+000006b0: e30e 400f 8e49 4094 8594 5294 7573 4add  ..@..I@...R.usJ.
+000006c0: 76cb 0e7d 944b 007d 9428 6824 4a4e c959  v..}.K.}.(h$JN.Y
+000006d0: 0168 268c 1150 6965 7277 737a 656a 2044  .h&..Pierwszej D
+000006e0: 7977 697a 6a69 9468 288c 0b72 6573 6964  ywizji.h(..resid
+000006f0: 656e 7469 616c 9468 2a8c 0233 3094 682c  ential.h*..30.h,
+00000700: 8c07 6173 7068 616c 7494 682e 8c03 7965  ..asphalt.h...ye
+00000710: 7394 6825 8968 3089 6831 6834 683a 4308  s.h%.h0.h1h4h:C.
+00000720: e27a 14ae 4729 5a40 9486 9452 9468 4068  .z..G)Z@...R.h@h
+00000730: 4343 6901 0200 0000 0600 0000 1558 0053  CCi..........X.S
+00000740: 061a 3140 e718 90bd de8d 4940 95f6 6118  ..1@......I@..a.
+00000750: 0b1a 3140 4cb0 ee0e df8d 4940 1230 babc  ..1@L.....I@.0..
+00000760: 391a 3140 09e3 022b e28d 4940 d23e b1a9  9.1@...+..I@.>..
+00000770: 4e1a 3140 2c85 9be7 e38d 4940 0429 67de  N.1@,.....I@.)g.
+00000780: 601a 3140 0d66 b8a6 e58d 4940 91d1 a68f  `.1@.f....I@....
+00000790: 651a 3140 d261 742f e68d 4940 9485 9452  e.1@.at/..I@...R
+000007a0: 9475 734a fa28 6f12 7d94 4b00 7d94 2868  .usJ.(o.}.K.}.(h
+000007b0: 244a e5a4 ad01 6826 8c11 5069 6572 7773  $J....h&..Pierws
+000007c0: 7a65 6a20 4479 7769 7a6a 6994 6828 8c0d  zej Dywizji.h(..
+000007d0: 6c69 7669 6e67 5f73 7472 6565 7494 6825  living_street.h%
+000007e0: 8968 3089 6831 6834 683a 4308 38b4 c876  .h0.h1h4h:C.8..v
+000007f0: bea7 5d40 9486 9452 9468 4068 4343 8901  ..]@...R.h@hCC..
+00000800: 0200 0000 0800 0000 1558 0053 061a 3140  .........X.S..1@
+00000810: e718 90bd de8d 4940 a5a8 8eb0 031a 3140  ......I@......1@
+00000820: 6a6d 7594 de8d 4940 6aaa 82ac 021a 3140  jmu...I@j.....1@
+00000830: 5f35 8584 de8d 4940 431d 56b8 e519 3140  _5....I@C.V...1@
+00000840: d757 b2be dc8d 4940 c567 fc0c b919 3140  .W....I@.g....1@
+00000850: f634 1603 da8d 4940 b0e9 9cfa 9b19 3140  .4....I@......1@
+00000860: 44d8 953b d88d 4940 16e3 5707 9b19 3140  D..;..I@..W...1@
+00000870: cd5f 7c2c d88d 4940 7062 a307 9919 3140  ._|,..I@pb....1@
+00000880: 4aaf 720d d88d 4940 9485 9452 9475 7375  J.r...I@...R.usu
+00000890: 4add 76cb 0e7d 944a 84cd 7c0e 7d94 4b00  J.v..}.J..|.}.K.
+000008a0: 7d94 2868 244a 4ec9 5901 6826 6868 6828  }.(h$JN.Y.h&hhh(
+000008b0: 6869 682a 686a 682c 686b 682e 686c 6825  hih*hjh,hkh.hlh%
+000008c0: 8968 3088 6831 6834 683a 4308 e17a 14ae  .h0.h1h4h:C..z..
+000008d0: 4729 5a40 9486 9452 9468 4068 4343 6901  G)Z@...R.h@hCCi.
+000008e0: 0200 0000 0600 0000 91d1 a68f 651a 3140  ............e.1@
+000008f0: d261 742f e68d 4940 0429 67de 601a 3140  .at/..I@.)g.`.1@
+00000900: 0d66 b8a6 e58d 4940 d23e b1a9 4e1a 3140  .f....I@.>..N.1@
+00000910: 2c85 9be7 e38d 4940 1230 babc 391a 3140  ,.....I@.0..9.1@
+00000920: 09e3 022b e28d 4940 95f6 6118 0b1a 3140  ...+..I@..a...1@
+00000930: 4cb0 ee0e df8d 4940 1558 0053 061a 3140  L.....I@.X.S..1@
+00000940: e718 90bd de8d 4940 9485 9452 9475 7373  ......I@...R.uss
+00000950: 4a99 286f 127d 944a 9a28 6f12 7d94 4b00  J.(o.}.J.(o.}.K.
+00000960: 7d94 2868 244a f0a4 ad01 6826 8c17 5374  }.(h$J....h&..St
+00000970: 6566 616e 6969 2053 656d 706f c582 6f77  efanii Sempo..ow
+00000980: 736b 6965 6a94 6828 8c0b 7265 7369 6465  skiej.h(..reside
+00000990: 6e74 6961 6c94 682a 8c02 3330 9468 2c8c  ntial.h*..30.h,.
+000009a0: 0761 7370 6861 6c74 9468 2e8c 0379 6573  .asphalt.h...yes
+000009b0: 9468 2589 6830 8968 3168 3468 3a43 0807  .h%.h0.h1h4h:C..
+000009c0: 8195 438b cc57 4094 8694 5294 6840 6843  ..C..W@...R.h@hC
+000009d0: 4349 0102 0000 0004 0000 0087 7945 a632  CI..........yE.2
+000009e0: 1931 407d fe20 3768 8d49 40f4 22c9 6251  .1@}. 7h.I@.".bQ
+000009f0: 1931 40a7 21aa f067 8d49 406a 23e8 7981  .1@.!..g.I@j#.y.
+00000a00: 1931 409c 7928 c066 8d49 401e 7bac cf8b  .1@.y(.f.I@.{...
+00000a10: 1931 4043 1aba 7e66 8d49 4094 8594 5294  .1@C..~f.I@...R.
+00000a20: 7573 734a 9a28 6f12 7d94 284a a628 6f12  ussJ.(o.}.(J.(o.
+00000a30: 7d94 4b00 7d94 2868 244a d0a4 ad01 6826  }.K.}.(h$J....h&
+00000a40: 8c10 4a61 6e75 737a 6120 4b6f 7263 7a61  ..Janusza Korcza
+00000a50: 6b61 9468 288c 0b72 6573 6964 656e 7469  ka.h(..residenti
+00000a60: 616c 9468 2a8c 0233 3094 682c 8c07 6173  al.h*..30.h,..as
+00000a70: 7068 616c 7494 682e 8c03 7965 7394 6825  phalt.h...yes.h%
+00000a80: 8968 3089 6831 6834 683a 4308 7593 1804  .h0.h1h4h:C.u...
+00000a90: 563e 5f40 9486 9452 9468 4068 4343 5901  V>_@...R.h@hCCY.
+00000aa0: 0200 0000 0500 0000 1e7b accf 8b19 3140  .........{....1@
+00000ab0: 431a ba7e 668d 4940 dd1b 8d8d 8a19 3140  C..~f.I@......1@
+00000ac0: e48d 8296 648d 4940 12ef 4adc 7419 3140  ....d.I@..J.t.1@
+00000ad0: 01ba d4ad 438d 4940 d604 acb0 7419 3140  ....C.I@....t.1@
+00000ae0: 7edb b86a 438d 4940 b9d7 930a 7419 3140  ~..jC.I@....t.1@
+00000af0: 7f99 396e 428d 4940 9485 9452 9475 734a  ..9nB.I@...R.usJ
+00000b00: 9c28 6f12 7d94 4b00 7d94 2868 244a f0a4  .(o.}.K.}.(h$J..
+00000b10: ad01 6826 6889 6828 688a 682a 688b 682c  ..h&h.h(h.h*h.h,
+00000b20: 688c 682e 688d 6825 8968 3089 6831 6834  h.h.h.h%.h0.h1h4
+00000b30: 683a 4308 de24 0681 9513 5440 9486 9452  h:C..$....T@...R
+00000b40: 9468 4068 4343 4901 0200 0000 0400 0000  .h@hCCI.........
+00000b50: 1e7b accf 8b19 3140 431a ba7e 668d 4940  .{....1@C..~f.I@
+00000b60: 2d16 759c 9119 3140 6c6b 555c 668d 4940  -.u...1@lkU\f.I@
+00000b70: 8506 62d9 cc19 3140 8b42 812d 658d 4940  ..b...1@.B.-e.I@
+00000b80: 7af1 8f08 d719 3140 ea1c a8f8 648d 4940  z.....1@....d.I@
+00000b90: 9485 9452 9475 734a 9928 6f12 7d94 4b00  ...R.usJ.(o.}.K.
+00000ba0: 7d94 2868 244a f0a4 ad01 6826 6889 6828  }.(h$J....h&h.h(
+00000bb0: 688a 682a 688b 682c 688c 682e 688d 6825  h.h*h.h,h.h.h.h%
+00000bc0: 8968 3088 6831 6834 683a 4308 0681 9543  .h0.h1h4h:C....C
+00000bd0: 8bcc 5740 9486 9452 9468 4068 4343 4901  ..W@...R.h@hCCI.
+00000be0: 0200 0000 0400 0000 1e7b accf 8b19 3140  .........{....1@
+00000bf0: 431a ba7e 668d 4940 6a23 e879 8119 3140  C..~f.I@j#.y..1@
+00000c00: 9c79 28c0 668d 4940 f422 c962 5119 3140  .y(.f.I@.".bQ.1@
+00000c10: a721 aaf0 678d 4940 8779 45a6 3219 3140  .!..g.I@.yE.2.1@
+00000c20: 7dfe 2037 688d 4940 9485 9452 9475 7375  }. 7h.I@...R.usu
+00000c30: 4a9c 286f 127d 944a 9a28 6f12 7d94 4b00  J.(o.}.J.(o.}.K.
+00000c40: 7d94 2868 244a f0a4 ad01 6826 6889 6828  }.(h$J....h&h.h(
+00000c50: 688a 682a 688b 682c 688c 682e 688d 6825  h.h*h.h,h.h.h.h%
+00000c60: 8968 3088 6831 6834 683a 4308 dd24 0681  .h0.h1h4h:C..$..
+00000c70: 9513 5440 9486 9452 9468 4068 4343 4901  ..T@...R.h@hCCI.
+00000c80: 0200 0000 0400 0000 7af1 8f08 d719 3140  ........z.....1@
+00000c90: ea1c a8f8 648d 4940 8506 62d9 cc19 3140  ....d.I@..b...1@
+00000ca0: 8b42 812d 658d 4940 2d16 759c 9119 3140  .B.-e.I@-.u...1@
+00000cb0: 6c6b 555c 668d 4940 1e7b accf 8b19 3140  lkU\f.I@.{....1@
+00000cc0: 431a ba7e 668d 4940 9485 9452 9475 7373  C..~f.I@...R.uss
+00000cd0: 4aa6 286f 127d 944a 9a28 6f12 7d94 4b00  J.(o.}.J.(o.}.K.
+00000ce0: 7d94 2868 244a d0a4 ad01 6826 6897 6828  }.(h$J....h&h.h(
+00000cf0: 6898 682a 6899 682c 689a 682e 689b 6825  h.h*h.h,h.h.h.h%
+00000d00: 8968 3088 6831 6834 683a 4308 7593 1804  .h0.h1h4h:C.u...
+00000d10: 563e 5f40 9486 9452 9468 4068 4343 5901  V>_@...R.h@hCCY.
+00000d20: 0200 0000 0500 0000 b9d7 930a 7419 3140  ............t.1@
+00000d30: 7f99 396e 428d 4940 d604 acb0 7419 3140  ..9nB.I@....t.1@
+00000d40: 7edb b86a 438d 4940 12ef 4adc 7419 3140  ~..jC.I@..J.t.1@
+00000d50: 01ba d4ad 438d 4940 dd1b 8d8d 8a19 3140  ....C.I@......1@
+00000d60: e48d 8296 648d 4940 1e7b accf 8b19 3140  ....d.I@.{....1@
+00000d70: 431a ba7e 668d 4940 9485 9452 9475 7373  C..~f.I@...R.uss
+00000d80: 4afa 286f 127d 9428 4a16 296f 127d 944b  J.(o.}.(J.)o.}.K
+00000d90: 007d 9428 6824 4ae2 a4ad 0168 268c 1c50  .}.(h$J....h&..P
+00000da0: 75c5 826b 6f77 6e69 6b61 2046 7261 6e63  u..kownika Franc
+00000db0: 6973 7a6b 6120 4e75 6c6c 6194 6828 8c0b  iszka Nulla.h(..
+00000dc0: 7265 7369 6465 6e74 6961 6c94 682a 8c02  residential.h*..
+00000dd0: 3330 9468 2589 6830 8968 3168 3468 3a43  30.h%.h0.h1h4h:C
+00000de0: 08ed 51b8 1e85 d364 4094 8694 5294 6840  ..Q....d@...R.h@
+00000df0: 6843 43a9 0102 0000 000a 0000 0070 62a3  hCC..........pb.
+00000e00: 0799 1931 404a af72 0dd8 8d49 40ee 2763  ...1@J.r...I@.'c
+00000e10: 7c98 1931 4008 0264 e8d8 8d49 407e 1ccd  |..1@..d...I@~..
+00000e20: 9195 1931 4089 44a1 65dd 8d49 40f5 dc9d  ...1@.D.e..I@...
+00000e30: 1095 1931 40be e199 2bde 8d49 4043 1ec1  ...1@...+..I@C..
+00000e40: 8d94 1931 4046 7ded f4de 8d49 401c c2e7  ...1@F}....I@...
+00000e50: 3d84 1931 408d 77ec 0cf8 8d49 404d ae18  =..1@.w....I@M..
+00000e60: 6481 1931 40de 077b 6efc 8d49 40cd 4301  d..1@..{n..I@.C.
+00000e70: 367b 1931 40f1 dd41 4706 8e49 40c7 e2ed  6{.1@..AG..I@...
+00000e80: f77a 1931 4020 ec14 ab06 8e49 4068 c647  .z.1@ .....I@h.G
+00000e90: 307a 1931 404f 6a79 2f08 8e49 4094 8594  0z.1@Ojy/..I@...
+00000ea0: 5294 7573 4a84 cd7c 0e7d 944b 007d 9428  R.usJ..|.}.K.}.(
+00000eb0: 6824 4ae5 a4ad 0168 2668 7568 2868 7668  h$J....h&huh(hvh
+00000ec0: 2589 6830 8868 3168 3468 3a43 0838 b4c8  %.h0.h1h4h:C.8..
+00000ed0: 76be a75d 4094 8694 5294 6840 6843 4389  v..]@...R.h@hCC.
+00000ee0: 0102 0000 0008 0000 0070 62a3 0799 1931  .........pb....1
+00000ef0: 404a af72 0dd8 8d49 4016 e357 079b 1931  @J.r...I@..W...1
+00000f00: 40cd 5f7c 2cd8 8d49 40b0 e99c fa9b 1931  @._|,..I@......1
+00000f10: 4044 d895 3bd8 8d49 40c5 67fc 0cb9 1931  @D..;..I@.g....1
+00000f20: 40f6 3416 03da 8d49 4043 1d56 b8e5 1931  @.4....I@C.V...1
+00000f30: 40d7 57b2 bedc 8d49 406a aa82 ac02 1a31  @.W....I@j.....1
+00000f40: 405f 3585 84de 8d49 40a5 a88e b003 1a31  @_5....I@......1
+00000f50: 406a 6d75 94de 8d49 4015 5800 5306 1a31  @jmu...I@.X.S..1
+00000f60: 40e7 1890 bdde 8d49 4094 8594 5294 7573  @......I@...R.us
+00000f70: 754a 1629 6f12 7d94 284a 83cd 7c0e 7d94  uJ.)o.}.(J..|.}.
+00000f80: 4b00 7d94 2868 244a 4cc9 5901 6825 8868  K.}.(h$JL.Y.h%.h
+00000f90: 2668 2768 2868 2968 2a68 2b68 2c68 2d68  &h'h(h)h*h+h,h-h
+00000fa0: 2e68 2f68 3089 6831 6834 683a 4308 9543  .h/h0.h1h4h:C..C
+00000fb0: 8b6c e783 5d40 9486 9452 9468 4068 4343  .l..]@...R.h@hCC
+00000fc0: 4901 0200 0000 0400 0000 68c6 4730 7a19  I.........h.G0z.
+00000fd0: 3140 4f6a 792f 088e 4940 ee7d 05c4 7f19  1@Ojy/..I@.}....
+00000fe0: 3140 d87b 968c 088e 4940 8738 317f e019  1@.{....I@.81...
+00000ff0: 3140 46d7 e0d8 0e8e 4940 d71e acb5 e619  1@F.....I@......
+00001000: 3140 c9e3 0e40 0f8e 4940 9485 9452 9475  1@...@..I@...R.u
+00001010: 734a fa28 6f12 7d94 4b00 7d94 2868 244a  sJ.(o.}.K.}.(h$J
+00001020: e2a4 ad01 6826 68c7 6828 68c8 682a 68c9  ....h&h.h(h.h*h.
+00001030: 6825 8968 3088 6831 6834 683a 4308 eb51  h%.h0.h1h4h:C..Q
+00001040: b81e 85d3 6440 9486 9452 9468 4068 4343  ....d@...R.h@hCC
+00001050: a901 0200 0000 0a00 0000 68c6 4730 7a19  ..........h.G0z.
+00001060: 3140 4f6a 792f 088e 4940 c7e2 edf7 7a19  1@Ojy/..I@....z.
+00001070: 3140 20ec 14ab 068e 4940 cd43 0136 7b19  1@ .....I@.C.6{.
+00001080: 3140 f1dd 4147 068e 4940 4dae 1864 8119  1@..AG..I@M..d..
+00001090: 3140 de07 7b6e fc8d 4940 1cc2 e73d 8419  1@..{n..I@...=..
+000010a0: 3140 8d77 ec0c f88d 4940 431e c18d 9419  1@.w....I@C.....
+000010b0: 3140 467d edf4 de8d 4940 f5dc 9d10 9519  1@F}....I@......
+000010c0: 3140 bee1 992b de8d 4940 7e1c cd91 9519  1@...+..I@~.....
+000010d0: 3140 8944 a165 dd8d 4940 ee27 637c 9819  1@.D.e..I@.'c|..
+000010e0: 3140 0802 64e8 d88d 4940 7062 a307 9919  1@..d...I@pb....
+000010f0: 3140 4aaf 720d d88d 4940 9485 9452 9475  1@J.r...I@...R.u
+00001100: 7375 8a05 0055 a8b2 007d 944a 84cd 7c0e  su...U...}.J..|.
+00001110: 7d94 4b00 7d94 2868 245d 9428 4a4d c959  }.K.}.(h$].(JM.Y
+00001120: 014a 0d71 751e 6568 268c 1041 6e64 727a  .J.qu.eh&..Andrz
+00001130: 656a 6120 506f 7465 626e 6994 6828 8c0b  eja Potebni.h(..
+00001140: 7265 7369 6465 6e74 6961 6c94 682a 8c02  residential.h*..
+00001150: 3330 9468 2c8c 0761 7370 6861 6c74 9468  30.h,..asphalt.h
+00001160: 2e68 5a68 2589 6830 8868 3168 3468 3a43  .hZh%.h0.h1h4h:C
+00001170: 086e 1283 c0ca b16a 4094 8694 5294 6840  .n.....j@...R.h@
+00001180: 6843 4379 0102 0000 0007 0000 002e bb71  hCCy...........q
+00001190: 9c25 1a31 4072 497a bda0 8d49 4040 ca3e  .%.1@rIz...I@@.>
+000011a0: 7e25 1a31 40dd f934 dda1 8d49 4082 5da8  ~%.1@..4...I@.].
+000011b0: 5725 1a31 402f c445 49a3 8d49 40b1 e144  W%.1@/.EI..I@..D
+000011c0: 4f25 1a31 4041 5d49 97a3 8d49 40f9 090c  O%.1@A]I...I@...
+000011d0: fe23 1a31 40be 0ba5 40b0 8d49 40f0 f1ae  .#.1@...@..I@...
+000011e0: 1f07 1a31 40d0 381e 7ddd 8d49 4015 5800  ...1@.8.}..I@.X.
+000011f0: 5306 1a31 40e7 1890 bdde 8d49 4094 8594  S..1@......I@...
+00001200: 5294 7573 7375 8c05 5f73 7563 6394 681f  R.ussu.._succ.h.
+00001210: 8c05 5f70 7265 6494 7d94 284a 82cd 7c0e  .._pred.}.(J..|.
+00001220: 7d94 4a83 cd7c 0e68 2273 4a83 cd7c 0e7d  }.J..|.h"sJ..|.}
+00001230: 9428 4a84 cd7c 0e68 5e4a 1629 6f12 68d9  .(J..|.h^J.)o.h.
+00001240: 754a 84cd 7c0e 7d94 284a 83cd 7c0e 6847  uJ..|.}.(J..|.hG
+00001250: 4add 76cb 0e68 7e4a fa28 6f12 68d0 8a05  J.v..h~J.(o.h...
+00001260: 0055 a8b2 0068 ea75 4add 76cb 0e7d 944a  .U...h.uJ.v..}.J
+00001270: 84cd 7c0e 6866 734a 9928 6f12 7d94 4a9a  ..|.hfsJ.(o.}.J.
+00001280: 286f 1268 aa73 4a9a 286f 127d 9428 4a99  (o.h.sJ.(o.}.(J.
+00001290: 286f 1268 874a 9c28 6f12 68b3 4aa6 286f  (o.h.J.(o.h.J.(o
+000012a0: 1268 bc75 4a9c 286f 127d 944a 9a28 6f12  .h.uJ.(o.}.J.(o.
+000012b0: 68a2 734a a628 6f12 7d94 4a9a 286f 1268  h.sJ.(o.}.J.(o.h
+000012c0: 9573 4afa 286f 127d 9428 4a84 cd7c 0e68  .sJ.(o.}.(J..|.h
+000012d0: 734a 1629 6f12 68e1 754a 1629 6f12 7d94  sJ.)o.h.uJ.)o.}.
+000012e0: 4afa 286f 1268 c573 8a05 0055 a8b2 007d  J.(o.h.s...U...}
+000012f0: 944a 84cd 7c0e 6854 7375 8c03 6164 6a94  .J..|.hTsu..adj.
+00001300: 8c1a 6e65 7477 6f72 6b78 2e63 6c61 7373  ..networkx.class
+00001310: 6573 2e63 6f72 6576 6965 7773 948c 124d  es.coreviews...M
+00001320: 756c 7469 4164 6a61 6365 6e63 7956 6965  ultiAdjacencyVie
+00001330: 7794 9394 2981 947d 948c 065f 6174 6c61  w...)..}..._atla
+00001340: 7394 681f 7362 8c05 6e6f 6465 7394 8c1c  s.h.sb..nodes...
+00001350: 6e65 7477 6f72 6b78 2e63 6c61 7373 6573  networkx.classes
+00001360: 2e72 6570 6f72 7476 6965 7773 948c 084e  .reportviews...N
+00001370: 6f64 6556 6965 7794 9394 2981 947d 948c  odeView...)..}..
+00001380: 065f 6e6f 6465 7394 680f 7362 8c04 7375  ._nodes.h.sb..su
+00001390: 6363 946a 0801 0000 2981 947d 946a 0b01  cc.j....)..}.j..
+000013a0: 0000 681f 7362 8c05 6564 6765 7394 6a0d  ..h.sb..edges.j.
+000013b0: 0100 008c 104f 7574 4d75 6c74 6945 6467  .....OutMultiEdg
+000013c0: 6556 6965 7794 9394 2981 947d 9428 8c06  eView...)..}.(..
+000013d0: 5f67 7261 7068 9468 038c 085f 6164 6a64  _graph.h..._adjd
+000013e0: 6963 7494 681f 7562 7562 2e              ict.h.ubub.
```

### Comparing `srai-0.2.0/tests/loaders/osm_way_loader/files/97e1befc51831ce8f8f482077f5042f2.pkl` & `srai-0.3.0/tests/loaders/osm_way_loader/test_files/graph_4.pkl`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 95e3 0e00 0000 0000 008c 1d6e 6574  .............net
+00000000: 8004 95d0 0e00 0000 0000 008c 1d6e 6574  .............net
 00000010: 776f 726b 782e 636c 6173 7365 732e 6d75  workx.classes.mu
 00000020: 6c74 6964 6967 7261 7068 948c 0c4d 756c  ltidigraph...Mul
 00000030: 7469 4469 4772 6170 6894 9394 2981 947d  tiDiGraph...)..}
 00000040: 9428 8c05 6772 6170 6894 7d94 288c 0c63  .(..graph.}.(..c
 00000050: 7265 6174 6564 5f64 6174 6594 8c13 3230  reated_date...20
 00000060: 3233 2d30 332d 3134 2032 333a 3237 3a35  23-03-14 23:27:5
 00000070: 3994 8c0c 6372 6561 7465 645f 7769 7468  9...created_with
@@ -40,200 +40,199 @@
 00000270: 7468 948c 156e 756d 7079 2e63 6f72 652e  th...numpy.core.
 00000280: 6d75 6c74 6961 7272 6179 948c 0673 6361  multiarray...sca
 00000290: 6c61 7294 9394 8c05 6e75 6d70 7994 8c05  lar.....numpy...
 000002a0: 6474 7970 6594 9394 8c02 6638 9489 8887  dtype.....f8....
 000002b0: 9452 9428 4b03 8c01 3c94 4e4e 4e4a ffff  .R.(K...<.NNNJ..
 000002c0: ffff 4aff ffff ff4b 0074 9462 4308 3333  ..J....K.t.bC.33
 000002d0: 3333 3323 5440 9486 9452 948c 0867 656f  333#T@...R...geo
-000002e0: 6d65 7472 7994 8c1b 7368 6170 656c 792e  metry...shapely.
-000002f0: 6765 6f6d 6574 7279 2e6c 696e 6573 7472  geometry.linestr
-00000300: 696e 6794 8c0a 4c69 6e65 5374 7269 6e67  ing...LineString
-00000310: 9493 9429 5294 4359 0102 0000 0005 0000  ...)R.CY........
-00000320: 00d7 1eac b5e6 1931 40c9 e30e 400f 8e49  .......1@...@..I
-00000330: 40aa 9b8b bfed 1931 4087 acc9 ae0f 8e49  @......1@......I
-00000340: 40b5 e1b0 34f0 1931 40da d836 d60f 8e49  @...4..1@..6...I
-00000350: 4091 4028 942a 1a31 40af 0562 7e13 8e49  @.@(.*.1@..b~..I
-00000360: 40d5 1cc5 de30 1a31 4073 d30b e313 8e49  @....0.1@s.....I
-00000370: 4094 6275 734a 84cd 7c0e 7d94 4b00 7d94  @.busJ..|.}.K.}.
-00000380: 2868 204a 4dc9 5901 6822 8c10 416e 6472  (h JM.Y.h"..Andr
-00000390: 7a65 6a61 2050 6f74 6562 6e69 9468 248c  zeja Potebni.h$.
-000003a0: 0b72 6573 6964 656e 7469 616c 9468 268c  .residential.h&.
-000003b0: 0233 3094 6828 8c07 6173 7068 616c 7494  .30.h(..asphalt.
-000003c0: 6821 8968 2c89 682d 6830 6836 4308 dcf9  h!.h,.h-h0h6C...
-000003d0: 7e6a bc00 6540 9486 9452 9468 3c68 3f29  ~j..e@...R.h<h?)
-000003e0: 5294 4399 0102 0000 0009 0000 00d7 1eac  R.C.............
-000003f0: b5e6 1931 40c9 e30e 400f 8e49 40ef a2f9  ...1@...@..I@...
-00000400: ade7 1931 4046 674f b80d 8e49 402a 8d98  ...1@FgO...I@*..
-00000410: d9e7 1931 401d 8c7d 6e0d 8e49 4037 1cf1  ...1@..}n..I@7..
-00000420: bff0 1931 40a1 3f7e 80ff 8d49 4031 7326  ...1@.?~...I@1s&
-00000430: 12f1 1931 40ad bf25 00ff 8d49 4049 e306  ...1@..%...I@I..
-00000440: 32f1 1931 400d 9a4c cbfe 8d49 4073 bed8  2..1@..L...I@s..
-00000450: 7bf1 1931 4090 920d 5afe 8d49 40f7 cec3  {..1@...Z..I@...
-00000460: 6405 1a31 407b a41c 27e0 8d49 4015 5800  d..1@{..'..I@.X.
-00000470: 5306 1a31 40e7 1890 bdde 8d49 4094 6275  S..1@......I@.bu
-00000480: 7375 4a84 cd7c 0e7d 9428 8a05 0055 a8b2  suJ..|.}.(...U..
-00000490: 007d 944b 007d 9428 6820 5d94 284a 0d71  .}.K.}.(h ].(J.q
-000004a0: 751e 4a4d c959 0165 6822 6844 6824 6845  u.JM.Y.eh"hDh$hE
-000004b0: 6826 6846 6828 6847 6821 8968 2c89 682d  h&hFh(hGh!.h,.h-
-000004c0: 6830 6836 4308 6f12 83c0 cab1 6a40 9486  h0h6C.o.....j@..
-000004d0: 9452 9468 2a8c 0379 6573 9468 3c68 3f29  .R.h*..yes.h<h?)
-000004e0: 5294 4379 0102 0000 0007 0000 0015 5800  R.Cy..........X.
-000004f0: 5306 1a31 40e7 1890 bdde 8d49 40f0 f1ae  S..1@......I@...
-00000500: 1f07 1a31 40d0 381e 7ddd 8d49 40f9 090c  ...1@.8.}..I@...
-00000510: fe23 1a31 40be 0ba5 40b0 8d49 40b1 e144  .#.1@...@..I@..D
-00000520: 4f25 1a31 4041 5d49 97a3 8d49 4082 5da8  O%.1@A]I...I@.].
-00000530: 5725 1a31 402f c445 49a3 8d49 4040 ca3e  W%.1@/.EI..I@@.>
-00000540: 7e25 1a31 40dd f934 dda1 8d49 402e bb71  ~%.1@..4...I@..q
-00000550: 9c25 1a31 4072 497a bda0 8d49 4094 6275  .%.1@rIz...I@.bu
-00000560: 734a 83cd 7c0e 7d94 4b00 7d94 2868 204a  sJ..|.}.K.}.(h J
-00000570: 4dc9 5901 6822 6844 6824 6845 6826 6846  M.Y.h"hDh$hEh&hF
-00000580: 6828 6847 6821 8968 2c88 682d 6830 6836  h(hGh!.h,.h-h0h6
-00000590: 4308 dbf9 7e6a bc00 6540 9486 9452 9468  C...~j..e@...R.h
-000005a0: 3c68 3f29 5294 4399 0102 0000 0009 0000  <h?)R.C.........
-000005b0: 0015 5800 5306 1a31 40e7 1890 bdde 8d49  ..X.S..1@......I
-000005c0: 40f7 cec3 6405 1a31 407b a41c 27e0 8d49  @...d..1@{..'..I
-000005d0: 4073 bed8 7bf1 1931 4090 920d 5afe 8d49  @s..{..1@...Z..I
-000005e0: 4049 e306 32f1 1931 400d 9a4c cbfe 8d49  @I..2..1@..L...I
-000005f0: 4031 7326 12f1 1931 40ad bf25 00ff 8d49  @1s&...1@..%...I
-00000600: 4037 1cf1 bff0 1931 40a1 3f7e 80ff 8d49  @7.....1@.?~...I
-00000610: 402a 8d98 d9e7 1931 401d 8c7d 6e0d 8e49  @*.....1@..}n..I
-00000620: 40ef a2f9 ade7 1931 4046 674f b80d 8e49  @......1@FgO...I
-00000630: 40d7 1eac b5e6 1931 40c9 e30e 400f 8e49  @......1@...@..I
-00000640: 4094 6275 734a dd76 cb0e 7d94 4b00 7d94  @.busJ.v..}.K.}.
-00000650: 2868 204a 4ec9 5901 6822 8c11 5069 6572  (h JN.Y.h"..Pier
-00000660: 7773 7a65 6a20 4479 7769 7a6a 6994 6824  wszej Dywizji.h$
-00000670: 8c0b 7265 7369 6465 6e74 6961 6c94 6826  ..residential.h&
-00000680: 8c02 3330 9468 288c 0761 7370 6861 6c74  ..30.h(..asphalt
-00000690: 9468 2a8c 0379 6573 9468 2189 682c 8968  .h*..yes.h!.h,.h
-000006a0: 2d68 3068 3643 08e2 7a14 ae47 295a 4094  -h0h6C..z..G)Z@.
-000006b0: 8694 5294 683c 683f 2952 9443 6901 0200  ..R.h<h?)R.Ci...
-000006c0: 0000 0600 0000 1558 0053 061a 3140 e718  .......X.S..1@..
-000006d0: 90bd de8d 4940 95f6 6118 0b1a 3140 4cb0  ....I@..a...1@L.
-000006e0: ee0e df8d 4940 1230 babc 391a 3140 09e3  ....I@.0..9.1@..
-000006f0: 022b e28d 4940 d23e b1a9 4e1a 3140 2c85  .+..I@.>..N.1@,.
-00000700: 9be7 e38d 4940 0429 67de 601a 3140 0d66  ....I@.)g.`.1@.f
-00000710: b8a6 e58d 4940 91d1 a68f 651a 3140 d261  ....I@....e.1@.a
-00000720: 742f e68d 4940 9462 7573 4afa 286f 127d  t/..I@.busJ.(o.}
-00000730: 944b 007d 9428 6820 4ae5 a4ad 0168 228c  .K.}.(h J....h".
-00000740: 1150 6965 7277 737a 656a 2044 7977 697a  .Pierwszej Dywiz
-00000750: 6a69 9468 248c 0d6c 6976 696e 675f 7374  ji.h$..living_st
-00000760: 7265 6574 9468 2189 682c 8968 2d68 3068  reet.h!.h,.h-h0h
-00000770: 3643 0838 b4c8 76be a75d 4094 8694 5294  6C.8..v..]@...R.
-00000780: 683c 683f 2952 9443 8901 0200 0000 0800  h<h?)R.C........
-00000790: 0000 1558 0053 061a 3140 e718 90bd de8d  ...X.S..1@......
-000007a0: 4940 a5a8 8eb0 031a 3140 6a6d 7594 de8d  I@......1@jmu...
-000007b0: 4940 6aaa 82ac 021a 3140 5f35 8584 de8d  I@j.....1@_5....
-000007c0: 4940 431d 56b8 e519 3140 d757 b2be dc8d  I@C.V...1@.W....
-000007d0: 4940 c567 fc0c b919 3140 f634 1603 da8d  I@.g....1@.4....
-000007e0: 4940 b0e9 9cfa 9b19 3140 44d8 953b d88d  I@......1@D..;..
-000007f0: 4940 16e3 5707 9b19 3140 cd5f 7c2c d88d  I@..W...1@._|,..
-00000800: 4940 7062 a307 9919 3140 4aaf 720d d88d  I@pb....1@J.r...
-00000810: 4940 9462 7573 754a dd76 cb0e 7d94 4a84  I@.busuJ.v..}.J.
-00000820: cd7c 0e7d 944b 007d 9428 6820 4a4e c959  .|.}.K.}.(h JN.Y
-00000830: 0168 2268 6068 2468 6168 2668 6268 2868  .h"h`h$hah&hbh(h
-00000840: 6368 2a68 6468 2189 682c 8868 2d68 3068  ch*hdh!.h,.h-h0h
-00000850: 3643 08e1 7a14 ae47 295a 4094 8694 5294  6C..z..G)Z@...R.
-00000860: 683c 683f 2952 9443 6901 0200 0000 0600  h<h?)R.Ci.......
-00000870: 0000 91d1 a68f 651a 3140 d261 742f e68d  ......e.1@.at/..
-00000880: 4940 0429 67de 601a 3140 0d66 b8a6 e58d  I@.)g.`.1@.f....
-00000890: 4940 d23e b1a9 4e1a 3140 2c85 9be7 e38d  I@.>..N.1@,.....
-000008a0: 4940 1230 babc 391a 3140 09e3 022b e28d  I@.0..9.1@...+..
-000008b0: 4940 95f6 6118 0b1a 3140 4cb0 ee0e df8d  I@..a...1@L.....
-000008c0: 4940 1558 0053 061a 3140 e718 90bd de8d  I@.X.S..1@......
-000008d0: 4940 9462 7573 734a fa28 6f12 7d94 284a  I@.bussJ.(o.}.(J
-000008e0: 1629 6f12 7d94 4b00 7d94 2868 204a e2a4  .)o.}.K.}.(h J..
-000008f0: ad01 6822 8c1c 5075 c582 6b6f 776e 696b  ..h"..Pu..kownik
-00000900: 6120 4672 616e 6369 737a 6b61 204e 756c  a Franciszka Nul
-00000910: 6c61 9468 248c 0b72 6573 6964 656e 7469  la.h$..residenti
-00000920: 616c 9468 268c 0233 3094 6821 8968 2c89  al.h&..30.h!.h,.
-00000930: 682d 6830 6836 4308 ed51 b81e 85d3 6440  h-h0h6C..Q....d@
-00000940: 9486 9452 9468 3c68 3f29 5294 43a9 0102  ...R.h<h?)R.C...
-00000950: 0000 000a 0000 0070 62a3 0799 1931 404a  .......pb....1@J
-00000960: af72 0dd8 8d49 40ee 2763 7c98 1931 4008  .r...I@.'c|..1@.
-00000970: 0264 e8d8 8d49 407e 1ccd 9195 1931 4089  .d...I@~.....1@.
-00000980: 44a1 65dd 8d49 40f5 dc9d 1095 1931 40be  D.e..I@......1@.
-00000990: e199 2bde 8d49 4043 1ec1 8d94 1931 4046  ..+..I@C.....1@F
-000009a0: 7ded f4de 8d49 401c c2e7 3d84 1931 408d  }....I@...=..1@.
-000009b0: 77ec 0cf8 8d49 404d ae18 6481 1931 40de  w....I@M..d..1@.
-000009c0: 077b 6efc 8d49 40cd 4301 367b 1931 40f1  .{n..I@.C.6{.1@.
-000009d0: dd41 4706 8e49 40c7 e2ed f77a 1931 4020  .AG..I@....z.1@ 
-000009e0: ec14 ab06 8e49 4068 c647 307a 1931 404f  .....I@h.G0z.1@O
-000009f0: 6a79 2f08 8e49 4094 6275 734a 84cd 7c0e  jy/..I@.busJ..|.
-00000a00: 7d94 4b00 7d94 2868 204a e5a4 ad01 6822  }.K.}.(h J....h"
-00000a10: 686c 6824 686d 6821 8968 2c88 682d 6830  hlh$hmh!.h,.h-h0
-00000a20: 6836 4308 38b4 c876 bea7 5d40 9486 9452  h6C.8..v..]@...R
-00000a30: 9468 3c68 3f29 5294 4389 0102 0000 0008  .h<h?)R.C.......
-00000a40: 0000 0070 62a3 0799 1931 404a af72 0dd8  ...pb....1@J.r..
-00000a50: 8d49 4016 e357 079b 1931 40cd 5f7c 2cd8  .I@..W...1@._|,.
-00000a60: 8d49 40b0 e99c fa9b 1931 4044 d895 3bd8  .I@......1@D..;.
-00000a70: 8d49 40c5 67fc 0cb9 1931 40f6 3416 03da  .I@.g....1@.4...
-00000a80: 8d49 4043 1d56 b8e5 1931 40d7 57b2 bedc  .I@C.V...1@.W...
-00000a90: 8d49 406a aa82 ac02 1a31 405f 3585 84de  .I@j.....1@_5...
-00000aa0: 8d49 40a5 a88e b003 1a31 406a 6d75 94de  .I@......1@jmu..
-00000ab0: 8d49 4015 5800 5306 1a31 40e7 1890 bdde  .I@.X.S..1@.....
-00000ac0: 8d49 4094 6275 7375 4a16 296f 127d 9428  .I@.busuJ.)o.}.(
-00000ad0: 4a83 cd7c 0e7d 944b 007d 9428 6820 4a4c  J..|.}.K.}.(h JL
-00000ae0: c959 0168 2188 6822 6823 6824 6825 6826  .Y.h!.h"h#h$h%h&
-00000af0: 6827 6828 6829 682a 682b 682c 8968 2d68  h'h(h)h*h+h,.h-h
-00000b00: 3068 3643 0895 438b 6ce7 835d 4094 8694  0h6C..C.l..]@...
-00000b10: 5294 683c 683f 2952 9443 4901 0200 0000  R.h<h?)R.CI.....
-00000b20: 0400 0000 68c6 4730 7a19 3140 4f6a 792f  ....h.G0z.1@Ojy/
-00000b30: 088e 4940 ee7d 05c4 7f19 3140 d87b 968c  ..I@.}....1@.{..
-00000b40: 088e 4940 8738 317f e019 3140 46d7 e0d8  ..I@.81...1@F...
-00000b50: 0e8e 4940 d71e acb5 e619 3140 c9e3 0e40  ..I@......1@...@
-00000b60: 0f8e 4940 9462 7573 4afa 286f 127d 944b  ..I@.busJ.(o.}.K
-00000b70: 007d 9428 6820 4ae2 a4ad 0168 2268 7e68  .}.(h J....h"h~h
-00000b80: 2468 7f68 2668 8068 2189 682c 8868 2d68  $h.h&h.h!.h,.h-h
-00000b90: 3068 3643 08eb 51b8 1e85 d364 4094 8694  0h6C..Q....d@...
-00000ba0: 5294 683c 683f 2952 9443 a901 0200 0000  R.h<h?)R.C......
-00000bb0: 0a00 0000 68c6 4730 7a19 3140 4f6a 792f  ....h.G0z.1@Ojy/
-00000bc0: 088e 4940 c7e2 edf7 7a19 3140 20ec 14ab  ..I@....z.1@ ...
-00000bd0: 068e 4940 cd43 0136 7b19 3140 f1dd 4147  ..I@.C.6{.1@..AG
-00000be0: 068e 4940 4dae 1864 8119 3140 de07 7b6e  ..I@M..d..1@..{n
-00000bf0: fc8d 4940 1cc2 e73d 8419 3140 8d77 ec0c  ..I@...=..1@.w..
-00000c00: f88d 4940 431e c18d 9419 3140 467d edf4  ..I@C.....1@F}..
-00000c10: de8d 4940 f5dc 9d10 9519 3140 bee1 992b  ..I@......1@...+
-00000c20: de8d 4940 7e1c cd91 9519 3140 8944 a165  ..I@~.....1@.D.e
-00000c30: dd8d 4940 ee27 637c 9819 3140 0802 64e8  ..I@.'c|..1@..d.
-00000c40: d88d 4940 7062 a307 9919 3140 4aaf 720d  ..I@pb....1@J.r.
-00000c50: d88d 4940 9462 7573 758a 0500 55a8 b200  ..I@.busu...U...
-00000c60: 7d94 4a84 cd7c 0e7d 944b 007d 9428 6820  }.J..|.}.K.}.(h 
-00000c70: 5d94 284a 4dc9 5901 4a0d 7175 1e65 6822  ].(JM.Y.J.qu.eh"
-00000c80: 8c10 416e 6472 7a65 6a61 2050 6f74 6562  ..Andrzeja Poteb
-00000c90: 6e69 9468 248c 0b72 6573 6964 656e 7469  ni.h$..residenti
-00000ca0: 616c 9468 268c 0233 3094 6828 8c07 6173  al.h&..30.h(..as
-00000cb0: 7068 616c 7494 682a 6854 6821 8968 2c88  phalt.h*hTh!.h,.
-00000cc0: 682d 6830 6836 4308 6e12 83c0 cab1 6a40  h-h0h6C.n.....j@
-00000cd0: 9486 9452 9468 3c68 3f29 5294 4379 0102  ...R.h<h?)R.Cy..
-00000ce0: 0000 0007 0000 002e bb71 9c25 1a31 4072  .........q.%.1@r
-00000cf0: 497a bda0 8d49 4040 ca3e 7e25 1a31 40dd  Iz...I@@.>~%.1@.
-00000d00: f934 dda1 8d49 4082 5da8 5725 1a31 402f  .4...I@.].W%.1@/
-00000d10: c445 49a3 8d49 40b1 e144 4f25 1a31 4041  .EI..I@..DO%.1@A
-00000d20: 5d49 97a3 8d49 40f9 090c fe23 1a31 40be  ]I...I@....#.1@.
-00000d30: 0ba5 40b0 8d49 40f0 f1ae 1f07 1a31 40d0  ..@..I@......1@.
-00000d40: 381e 7ddd 8d49 4015 5800 5306 1a31 40e7  8.}..I@.X.S..1@.
-00000d50: 1890 bdde 8d49 4094 6275 7373 758c 055f  .....I@.bussu.._
-00000d60: 7375 6363 9468 1b8c 055f 7072 6564 947d  succ.h..._pred.}
-00000d70: 9428 4a82 cd7c 0e7d 944a 83cd 7c0e 681e  .(J..|.}.J..|.h.
-00000d80: 734a 83cd 7c0e 7d94 284a 84cd 7c0e 6857  sJ..|.}.(J..|.hW
-00000d90: 4a16 296f 1268 8e75 4a84 cd7c 0e7d 9428  J.)o.h.uJ..|.}.(
-00000da0: 4a83 cd7c 0e68 424a dd76 cb0e 6874 4afa  J..|.hBJ.v..htJ.
-00000db0: 286f 1268 868a 0500 55a8 b200 689d 754a  (o.h....U...h.uJ
-00000dc0: dd76 cb0e 7d94 4a84 cd7c 0e68 5e73 4afa  .v..}.J..|.h^sJ.
-00000dd0: 286f 127d 9428 4a84 cd7c 0e68 6a4a 1629  (o.}.(J..|.hjJ.)
-00000de0: 6f12 6895 754a 1629 6f12 7d94 4afa 286f  o.h.uJ.)o.}.J.(o
-00000df0: 1268 7c73 8a05 0055 a8b2 007d 944a 84cd  .h|s...U...}.J..
-00000e00: 7c0e 684e 7375 8c03 6164 6a94 8c1a 6e65  |.hNsu..adj...ne
-00000e10: 7477 6f72 6b78 2e63 6c61 7373 6573 2e63  tworkx.classes.c
-00000e20: 6f72 6576 6965 7773 948c 124d 756c 7469  oreviews...Multi
-00000e30: 4164 6a61 6365 6e63 7956 6965 7794 9394  AdjacencyView...
-00000e40: 2981 947d 948c 065f 6174 6c61 7394 681b  )..}..._atlas.h.
-00000e50: 7362 8c05 6e6f 6465 7394 8c1c 6e65 7477  sb..nodes...netw
-00000e60: 6f72 6b78 2e63 6c61 7373 6573 2e72 6570  orkx.classes.rep
-00000e70: 6f72 7476 6965 7773 948c 084e 6f64 6556  ortviews...NodeV
-00000e80: 6965 7794 9394 2981 947d 948c 065f 6e6f  iew...)..}..._no
-00000e90: 6465 7394 680f 7362 8c04 7375 6363 9468  des.h.sb..succ.h
-00000ea0: b629 8194 7d94 68b9 681b 7362 8c05 6564  .)..}.h.h.sb..ed
-00000eb0: 6765 7394 68bb 8c10 4f75 744d 756c 7469  ges.h...OutMulti
-00000ec0: 4564 6765 5669 6577 9493 9429 8194 7d94  EdgeView...)..}.
-00000ed0: 288c 065f 6772 6170 6894 6803 8c08 5f61  (.._graph.h..._a
-00000ee0: 646a 6469 6374 9468 1b75 6275 622e       djdict.h.ubub.
+000002e0: 6d65 7472 7994 8c0a 7368 6170 656c 792e  metry...shapely.
+000002f0: 696f 948c 0866 726f 6d5f 776b 6294 9394  io...from_wkb...
+00000300: 4359 0102 0000 0005 0000 00d7 1eac b5e6  CY..............
+00000310: 1931 40c9 e30e 400f 8e49 40aa 9b8b bfed  .1@...@..I@.....
+00000320: 1931 4087 acc9 ae0f 8e49 40b5 e1b0 34f0  .1@......I@...4.
+00000330: 1931 40da d836 d60f 8e49 4091 4028 942a  .1@..6...I@.@(.*
+00000340: 1a31 40af 0562 7e13 8e49 40d5 1cc5 de30  .1@..b~..I@....0
+00000350: 1a31 4073 d30b e313 8e49 4094 8594 5294  .1@s.....I@...R.
+00000360: 7573 4a84 cd7c 0e7d 944b 007d 9428 6820  usJ..|.}.K.}.(h 
+00000370: 4a4d c959 0168 228c 1041 6e64 727a 656a  JM.Y.h"..Andrzej
+00000380: 6120 506f 7465 626e 6994 6824 8c0b 7265  a Potebni.h$..re
+00000390: 7369 6465 6e74 6961 6c94 6826 8c02 3330  sidential.h&..30
+000003a0: 9468 288c 0761 7370 6861 6c74 9468 2189  .h(..asphalt.h!.
+000003b0: 682c 8968 2d68 3068 3643 08dc f97e 6abc  h,.h-h0h6C...~j.
+000003c0: 0065 4094 8694 5294 683c 683f 4399 0102  .e@...R.h<h?C...
+000003d0: 0000 0009 0000 00d7 1eac b5e6 1931 40c9  .............1@.
+000003e0: e30e 400f 8e49 40ef a2f9 ade7 1931 4046  ..@..I@......1@F
+000003f0: 674f b80d 8e49 402a 8d98 d9e7 1931 401d  gO...I@*.....1@.
+00000400: 8c7d 6e0d 8e49 4037 1cf1 bff0 1931 40a1  .}n..I@7.....1@.
+00000410: 3f7e 80ff 8d49 4031 7326 12f1 1931 40ad  ?~...I@1s&...1@.
+00000420: bf25 00ff 8d49 4049 e306 32f1 1931 400d  .%...I@I..2..1@.
+00000430: 9a4c cbfe 8d49 4073 bed8 7bf1 1931 4090  .L...I@s..{..1@.
+00000440: 920d 5afe 8d49 40f7 cec3 6405 1a31 407b  ..Z..I@...d..1@{
+00000450: a41c 27e0 8d49 4015 5800 5306 1a31 40e7  ..'..I@.X.S..1@.
+00000460: 1890 bdde 8d49 4094 8594 5294 7573 754a  .....I@...R.usuJ
+00000470: 84cd 7c0e 7d94 288a 0500 55a8 b200 7d94  ..|.}.(...U...}.
+00000480: 4b00 7d94 2868 205d 9428 4a0d 7175 1e4a  K.}.(h ].(J.qu.J
+00000490: 4dc9 5901 6568 2268 4568 2468 4668 2668  M.Y.eh"hEh$hFh&h
+000004a0: 4768 2868 4868 2189 682c 8968 2d68 3068  Gh(hHh!.h,.h-h0h
+000004b0: 3643 086f 1283 c0ca b16a 4094 8694 5294  6C.o.....j@...R.
+000004c0: 682a 8c03 7965 7394 683c 683f 4379 0102  h*..yes.h<h?Cy..
+000004d0: 0000 0007 0000 0015 5800 5306 1a31 40e7  ........X.S..1@.
+000004e0: 1890 bdde 8d49 40f0 f1ae 1f07 1a31 40d0  .....I@......1@.
+000004f0: 381e 7ddd 8d49 40f9 090c fe23 1a31 40be  8.}..I@....#.1@.
+00000500: 0ba5 40b0 8d49 40b1 e144 4f25 1a31 4041  ..@..I@..DO%.1@A
+00000510: 5d49 97a3 8d49 4082 5da8 5725 1a31 402f  ]I...I@.].W%.1@/
+00000520: c445 49a3 8d49 4040 ca3e 7e25 1a31 40dd  .EI..I@@.>~%.1@.
+00000530: f934 dda1 8d49 402e bb71 9c25 1a31 4072  .4...I@..q.%.1@r
+00000540: 497a bda0 8d49 4094 8594 5294 7573 4a83  Iz...I@...R.usJ.
+00000550: cd7c 0e7d 944b 007d 9428 6820 4a4d c959  .|.}.K.}.(h JM.Y
+00000560: 0168 2268 4568 2468 4668 2668 4768 2868  .h"hEh$hFh&hGh(h
+00000570: 4868 2189 682c 8868 2d68 3068 3643 08db  Hh!.h,.h-h0h6C..
+00000580: f97e 6abc 0065 4094 8694 5294 683c 683f  .~j..e@...R.h<h?
+00000590: 4399 0102 0000 0009 0000 0015 5800 5306  C...........X.S.
+000005a0: 1a31 40e7 1890 bdde 8d49 40f7 cec3 6405  .1@......I@...d.
+000005b0: 1a31 407b a41c 27e0 8d49 4073 bed8 7bf1  .1@{..'..I@s..{.
+000005c0: 1931 4090 920d 5afe 8d49 4049 e306 32f1  .1@...Z..I@I..2.
+000005d0: 1931 400d 9a4c cbfe 8d49 4031 7326 12f1  .1@..L...I@1s&..
+000005e0: 1931 40ad bf25 00ff 8d49 4037 1cf1 bff0  .1@..%...I@7....
+000005f0: 1931 40a1 3f7e 80ff 8d49 402a 8d98 d9e7  .1@.?~...I@*....
+00000600: 1931 401d 8c7d 6e0d 8e49 40ef a2f9 ade7  .1@..}n..I@.....
+00000610: 1931 4046 674f b80d 8e49 40d7 1eac b5e6  .1@FgO...I@.....
+00000620: 1931 40c9 e30e 400f 8e49 4094 8594 5294  .1@...@..I@...R.
+00000630: 7573 4add 76cb 0e7d 944b 007d 9428 6820  usJ.v..}.K.}.(h 
+00000640: 4a4e c959 0168 228c 1150 6965 7277 737a  JN.Y.h"..Pierwsz
+00000650: 656a 2044 7977 697a 6a69 9468 248c 0b72  ej Dywizji.h$..r
+00000660: 6573 6964 656e 7469 616c 9468 268c 0233  esidential.h&..3
+00000670: 3094 6828 8c07 6173 7068 616c 7494 682a  0.h(..asphalt.h*
+00000680: 8c03 7965 7394 6821 8968 2c89 682d 6830  ..yes.h!.h,.h-h0
+00000690: 6836 4308 e27a 14ae 4729 5a40 9486 9452  h6C..z..G)Z@...R
+000006a0: 9468 3c68 3f43 6901 0200 0000 0600 0000  .h<h?Ci.........
+000006b0: 1558 0053 061a 3140 e718 90bd de8d 4940  .X.S..1@......I@
+000006c0: 95f6 6118 0b1a 3140 4cb0 ee0e df8d 4940  ..a...1@L.....I@
+000006d0: 1230 babc 391a 3140 09e3 022b e28d 4940  .0..9.1@...+..I@
+000006e0: d23e b1a9 4e1a 3140 2c85 9be7 e38d 4940  .>..N.1@,.....I@
+000006f0: 0429 67de 601a 3140 0d66 b8a6 e58d 4940  .)g.`.1@.f....I@
+00000700: 91d1 a68f 651a 3140 d261 742f e68d 4940  ....e.1@.at/..I@
+00000710: 9485 9452 9475 734a fa28 6f12 7d94 4b00  ...R.usJ.(o.}.K.
+00000720: 7d94 2868 204a e5a4 ad01 6822 8c11 5069  }.(h J....h"..Pi
+00000730: 6572 7773 7a65 6a20 4479 7769 7a6a 6994  erwszej Dywizji.
+00000740: 6824 8c0d 6c69 7669 6e67 5f73 7472 6565  h$..living_stree
+00000750: 7494 6821 8968 2c89 682d 6830 6836 4308  t.h!.h,.h-h0h6C.
+00000760: 38b4 c876 bea7 5d40 9486 9452 9468 3c68  8..v..]@...R.h<h
+00000770: 3f43 8901 0200 0000 0800 0000 1558 0053  ?C...........X.S
+00000780: 061a 3140 e718 90bd de8d 4940 a5a8 8eb0  ..1@......I@....
+00000790: 031a 3140 6a6d 7594 de8d 4940 6aaa 82ac  ..1@jmu...I@j...
+000007a0: 021a 3140 5f35 8584 de8d 4940 431d 56b8  ..1@_5....I@C.V.
+000007b0: e519 3140 d757 b2be dc8d 4940 c567 fc0c  ..1@.W....I@.g..
+000007c0: b919 3140 f634 1603 da8d 4940 b0e9 9cfa  ..1@.4....I@....
+000007d0: 9b19 3140 44d8 953b d88d 4940 16e3 5707  ..1@D..;..I@..W.
+000007e0: 9b19 3140 cd5f 7c2c d88d 4940 7062 a307  ..1@._|,..I@pb..
+000007f0: 9919 3140 4aaf 720d d88d 4940 9485 9452  ..1@J.r...I@...R
+00000800: 9475 7375 4add 76cb 0e7d 944a 84cd 7c0e  .usuJ.v..}.J..|.
+00000810: 7d94 4b00 7d94 2868 204a 4ec9 5901 6822  }.K.}.(h JN.Y.h"
+00000820: 6864 6824 6865 6826 6866 6828 6867 682a  hdh$heh&hfh(hgh*
+00000830: 6868 6821 8968 2c88 682d 6830 6836 4308  hhh!.h,.h-h0h6C.
+00000840: e17a 14ae 4729 5a40 9486 9452 9468 3c68  .z..G)Z@...R.h<h
+00000850: 3f43 6901 0200 0000 0600 0000 91d1 a68f  ?Ci.............
+00000860: 651a 3140 d261 742f e68d 4940 0429 67de  e.1@.at/..I@.)g.
+00000870: 601a 3140 0d66 b8a6 e58d 4940 d23e b1a9  `.1@.f....I@.>..
+00000880: 4e1a 3140 2c85 9be7 e38d 4940 1230 babc  N.1@,.....I@.0..
+00000890: 391a 3140 09e3 022b e28d 4940 95f6 6118  9.1@...+..I@..a.
+000008a0: 0b1a 3140 4cb0 ee0e df8d 4940 1558 0053  ..1@L.....I@.X.S
+000008b0: 061a 3140 e718 90bd de8d 4940 9485 9452  ..1@......I@...R
+000008c0: 9475 7373 4afa 286f 127d 9428 4a16 296f  .ussJ.(o.}.(J.)o
+000008d0: 127d 944b 007d 9428 6820 4ae2 a4ad 0168  .}.K.}.(h J....h
+000008e0: 228c 1c50 75c5 826b 6f77 6e69 6b61 2046  "..Pu..kownika F
+000008f0: 7261 6e63 6973 7a6b 6120 4e75 6c6c 6194  ranciszka Nulla.
+00000900: 6824 8c0b 7265 7369 6465 6e74 6961 6c94  h$..residential.
+00000910: 6826 8c02 3330 9468 2189 682c 8968 2d68  h&..30.h!.h,.h-h
+00000920: 3068 3643 08ed 51b8 1e85 d364 4094 8694  0h6C..Q....d@...
+00000930: 5294 683c 683f 43a9 0102 0000 000a 0000  R.h<h?C.........
+00000940: 0070 62a3 0799 1931 404a af72 0dd8 8d49  .pb....1@J.r...I
+00000950: 40ee 2763 7c98 1931 4008 0264 e8d8 8d49  @.'c|..1@..d...I
+00000960: 407e 1ccd 9195 1931 4089 44a1 65dd 8d49  @~.....1@.D.e..I
+00000970: 40f5 dc9d 1095 1931 40be e199 2bde 8d49  @......1@...+..I
+00000980: 4043 1ec1 8d94 1931 4046 7ded f4de 8d49  @C.....1@F}....I
+00000990: 401c c2e7 3d84 1931 408d 77ec 0cf8 8d49  @...=..1@.w....I
+000009a0: 404d ae18 6481 1931 40de 077b 6efc 8d49  @M..d..1@..{n..I
+000009b0: 40cd 4301 367b 1931 40f1 dd41 4706 8e49  @.C.6{.1@..AG..I
+000009c0: 40c7 e2ed f77a 1931 4020 ec14 ab06 8e49  @....z.1@ .....I
+000009d0: 4068 c647 307a 1931 404f 6a79 2f08 8e49  @h.G0z.1@Ojy/..I
+000009e0: 4094 8594 5294 7573 4a84 cd7c 0e7d 944b  @...R.usJ..|.}.K
+000009f0: 007d 9428 6820 4ae5 a4ad 0168 2268 7168  .}.(h J....h"hqh
+00000a00: 2468 7268 2189 682c 8868 2d68 3068 3643  $hrh!.h,.h-h0h6C
+00000a10: 0838 b4c8 76be a75d 4094 8694 5294 683c  .8..v..]@...R.h<
+00000a20: 683f 4389 0102 0000 0008 0000 0070 62a3  h?C..........pb.
+00000a30: 0799 1931 404a af72 0dd8 8d49 4016 e357  ...1@J.r...I@..W
+00000a40: 079b 1931 40cd 5f7c 2cd8 8d49 40b0 e99c  ...1@._|,..I@...
+00000a50: fa9b 1931 4044 d895 3bd8 8d49 40c5 67fc  ...1@D..;..I@.g.
+00000a60: 0cb9 1931 40f6 3416 03da 8d49 4043 1d56  ...1@.4....I@C.V
+00000a70: b8e5 1931 40d7 57b2 bedc 8d49 406a aa82  ...1@.W....I@j..
+00000a80: ac02 1a31 405f 3585 84de 8d49 40a5 a88e  ...1@_5....I@...
+00000a90: b003 1a31 406a 6d75 94de 8d49 4015 5800  ...1@jmu...I@.X.
+00000aa0: 5306 1a31 40e7 1890 bdde 8d49 4094 8594  S..1@......I@...
+00000ab0: 5294 7573 754a 1629 6f12 7d94 284a 83cd  R.usuJ.)o.}.(J..
+00000ac0: 7c0e 7d94 4b00 7d94 2868 204a 4cc9 5901  |.}.K.}.(h JL.Y.
+00000ad0: 6821 8868 2268 2368 2468 2568 2668 2768  h!.h"h#h$h%h&h'h
+00000ae0: 2868 2968 2a68 2b68 2c89 682d 6830 6836  (h)h*h+h,.h-h0h6
+00000af0: 4308 9543 8b6c e783 5d40 9486 9452 9468  C..C.l..]@...R.h
+00000b00: 3c68 3f43 4901 0200 0000 0400 0000 68c6  <h?CI.........h.
+00000b10: 4730 7a19 3140 4f6a 792f 088e 4940 ee7d  G0z.1@Ojy/..I@.}
+00000b20: 05c4 7f19 3140 d87b 968c 088e 4940 8738  ....1@.{....I@.8
+00000b30: 317f e019 3140 46d7 e0d8 0e8e 4940 d71e  1...1@F.....I@..
+00000b40: acb5 e619 3140 c9e3 0e40 0f8e 4940 9485  ....1@...@..I@..
+00000b50: 9452 9475 734a fa28 6f12 7d94 4b00 7d94  .R.usJ.(o.}.K.}.
+00000b60: 2868 204a e2a4 ad01 6822 6885 6824 6886  (h J....h"h.h$h.
+00000b70: 6826 6887 6821 8968 2c88 682d 6830 6836  h&h.h!.h,.h-h0h6
+00000b80: 4308 eb51 b81e 85d3 6440 9486 9452 9468  C..Q....d@...R.h
+00000b90: 3c68 3f43 a901 0200 0000 0a00 0000 68c6  <h?C..........h.
+00000ba0: 4730 7a19 3140 4f6a 792f 088e 4940 c7e2  G0z.1@Ojy/..I@..
+00000bb0: edf7 7a19 3140 20ec 14ab 068e 4940 cd43  ..z.1@ .....I@.C
+00000bc0: 0136 7b19 3140 f1dd 4147 068e 4940 4dae  .6{.1@..AG..I@M.
+00000bd0: 1864 8119 3140 de07 7b6e fc8d 4940 1cc2  .d..1@..{n..I@..
+00000be0: e73d 8419 3140 8d77 ec0c f88d 4940 431e  .=..1@.w....I@C.
+00000bf0: c18d 9419 3140 467d edf4 de8d 4940 f5dc  ....1@F}....I@..
+00000c00: 9d10 9519 3140 bee1 992b de8d 4940 7e1c  ....1@...+..I@~.
+00000c10: cd91 9519 3140 8944 a165 dd8d 4940 ee27  ....1@.D.e..I@.'
+00000c20: 637c 9819 3140 0802 64e8 d88d 4940 7062  c|..1@..d...I@pb
+00000c30: a307 9919 3140 4aaf 720d d88d 4940 9485  ....1@J.r...I@..
+00000c40: 9452 9475 7375 8a05 0055 a8b2 007d 944a  .R.usu...U...}.J
+00000c50: 84cd 7c0e 7d94 4b00 7d94 2868 205d 9428  ..|.}.K.}.(h ].(
+00000c60: 4a4d c959 014a 0d71 751e 6568 228c 1041  JM.Y.J.qu.eh"..A
+00000c70: 6e64 727a 656a 6120 506f 7465 626e 6994  ndrzeja Potebni.
+00000c80: 6824 8c0b 7265 7369 6465 6e74 6961 6c94  h$..residential.
+00000c90: 6826 8c02 3330 9468 288c 0761 7370 6861  h&..30.h(..aspha
+00000ca0: 6c74 9468 2a68 5668 2189 682c 8868 2d68  lt.h*hVh!.h,.h-h
+00000cb0: 3068 3643 086e 1283 c0ca b16a 4094 8694  0h6C.n.....j@...
+00000cc0: 5294 683c 683f 4379 0102 0000 0007 0000  R.h<h?Cy........
+00000cd0: 002e bb71 9c25 1a31 4072 497a bda0 8d49  ...q.%.1@rIz...I
+00000ce0: 4040 ca3e 7e25 1a31 40dd f934 dda1 8d49  @@.>~%.1@..4...I
+00000cf0: 4082 5da8 5725 1a31 402f c445 49a3 8d49  @.].W%.1@/.EI..I
+00000d00: 40b1 e144 4f25 1a31 4041 5d49 97a3 8d49  @..DO%.1@A]I...I
+00000d10: 40f9 090c fe23 1a31 40be 0ba5 40b0 8d49  @....#.1@...@..I
+00000d20: 40f0 f1ae 1f07 1a31 40d0 381e 7ddd 8d49  @......1@.8.}..I
+00000d30: 4015 5800 5306 1a31 40e7 1890 bdde 8d49  @.X.S..1@......I
+00000d40: 4094 8594 5294 7573 7375 8c05 5f73 7563  @...R.ussu.._suc
+00000d50: 6394 681b 8c05 5f70 7265 6494 7d94 284a  c.h..._pred.}.(J
+00000d60: 82cd 7c0e 7d94 4a83 cd7c 0e68 1e73 4a83  ..|.}.J..|.h.sJ.
+00000d70: cd7c 0e7d 9428 4a84 cd7c 0e68 5a4a 1629  .|.}.(J..|.hZJ.)
+00000d80: 6f12 6897 754a 84cd 7c0e 7d94 284a 83cd  o.h.uJ..|.}.(J..
+00000d90: 7c0e 6843 4add 76cb 0e68 7a4a fa28 6f12  |.hCJ.v..hzJ.(o.
+00000da0: 688e 8a05 0055 a8b2 0068 a875 4add 76cb  h....U...h.uJ.v.
+00000db0: 0e7d 944a 84cd 7c0e 6862 734a fa28 6f12  .}.J..|.hbsJ.(o.
+00000dc0: 7d94 284a 84cd 7c0e 686f 4a16 296f 1268  }.(J..|.hoJ.)o.h
+00000dd0: 9f75 4a16 296f 127d 944a fa28 6f12 6883  .uJ.)o.}.J.(o.h.
+00000de0: 738a 0500 55a8 b200 7d94 4a84 cd7c 0e68  s...U...}.J..|.h
+00000df0: 5073 758c 0361 646a 948c 1a6e 6574 776f  Psu..adj...netwo
+00000e00: 726b 782e 636c 6173 7365 732e 636f 7265  rkx.classes.core
+00000e10: 7669 6577 7394 8c12 4d75 6c74 6941 646a  views...MultiAdj
+00000e20: 6163 656e 6379 5669 6577 9493 9429 8194  acencyView...)..
+00000e30: 7d94 8c06 5f61 746c 6173 9468 1b73 628c  }..._atlas.h.sb.
+00000e40: 056e 6f64 6573 948c 1c6e 6574 776f 726b  .nodes...network
+00000e50: 782e 636c 6173 7365 732e 7265 706f 7274  x.classes.report
+00000e60: 7669 6577 7394 8c08 4e6f 6465 5669 6577  views...NodeView
+00000e70: 9493 9429 8194 7d94 8c06 5f6e 6f64 6573  ...)..}..._nodes
+00000e80: 9468 0f73 628c 0473 7563 6394 68c2 2981  .h.sb..succ.h.).
+00000e90: 947d 9468 c568 1b73 628c 0565 6467 6573  .}.h.h.sb..edges
+00000ea0: 9468 c78c 104f 7574 4d75 6c74 6945 6467  .h...OutMultiEdg
+00000eb0: 6556 6965 7794 9394 2981 947d 9428 8c06  eView...)..}.(..
+00000ec0: 5f67 7261 7068 9468 038c 085f 6164 6a64  _graph.h..._adjd
+00000ed0: 6963 7494 681b 7562 7562 2e              ict.h.ubub.
```

### Comparing `srai-0.2.0/tests/loaders/osm_way_loader/test_osm_way_loader.py` & `srai-0.3.0/tests/loaders/osm_way_loader/test_osm_way_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for OSMWayLoader."""
-import hashlib
 import pickle as pkl
 from contextlib import nullcontext as does_not_raise
+from functools import partial
 from pathlib import Path
 from typing import Any, Dict, Optional, Sequence, Tuple, Union
 from unittest import TestCase
 
 import geopandas as gpd
 import numpy as np
 import osmnx
@@ -14,15 +14,15 @@
 import shapely.geometry as shpg
 from parametrization import Parametrization as P
 from pytest_check import check
 from pytest_mock import MockerFixture
 
 from srai.constants import GEOMETRY_COLUMN, WGS84_CRS
 from srai.exceptions import LoadedDataIsEmptyException
-from srai.loaders.osm_way_loader import NetworkType, OSMWayLoader
+from srai.loaders import OSMNetworkType, OSMWayLoader
 
 ut = TestCase()
 
 
 @pytest.fixture  # type: ignore
 def empty_area_gdf() -> gpd.GeoDataFrame:
     """Get a gdf with no geometry."""
@@ -83,15 +83,15 @@
     )
 
     gdf = gpd.GeoDataFrame({GEOMETRY_COLUMN: [polygon]}, crs=WGS84_CRS)
     return gdf
 
 
 @pytest.fixture  # type: ignore
-def multiple_polygons_overlaping_area_gdf(
+def multiple_polygons_overlapping_area_gdf(
     first_polygon_area_gdf: gpd.GeoDataFrame, second_polygon_area_gdf: gpd.GeoDataFrame
 ) -> gpd.GeoDataFrame:
     """Get an example area gdf with two polygons."""
     return pd.concat([first_polygon_area_gdf, second_polygon_area_gdf], axis=0)
 
 
 @pytest.fixture  # type: ignore
@@ -122,133 +122,146 @@
 def valid_and_empty_polygons_area_gdf(
     first_polygon_area_gdf: gpd.GeoDataFrame, empty_polygon_area_gdf: gpd.GeoDataFrame
 ) -> gpd.GeoDataFrame:
     """Get an example area gdf with one valid polygon and one without road infrastructure."""
     return pd.concat([first_polygon_area_gdf, empty_polygon_area_gdf], axis=0)
 
 
-@P.parameters("area_gdf_fixture", "expected_result", "loader_params", "expectation")  # type: ignore
+@P.parameters(  # type: ignore
+    "area_gdf_fixture", "expected_result", "loader_params", "file_name", "expectation"
+)
 @P.case(  # type: ignore
-    "Raise when no geometry", "empty_area_gdf", None, None, pytest.raises(ValueError)
+    "Raise when no geometry", "empty_area_gdf", None, None, None, pytest.raises(ValueError)
 )
 @P.case(  # type: ignore
     "Raise when no CRS",
     "no_crs_area_gdf",
     None,
     None,
+    None,
     pytest.raises(ValueError),
 )
 @P.case(  # type: ignore
     "Raise when invalid geometry",
     "bad_geometry_area_gdf",
     None,
     None,
+    "type_error",
     pytest.raises(TypeError),
 )
 @P.case(  # type: ignore
     "Raise when no road infrastructure",
     "empty_polygon_area_gdf",
     None,
     None,
+    "empty_overpass_response",
     pytest.raises(LoadedDataIsEmptyException),
 )
 @P.case(  # type: ignore
     "Return infrastructure when single polygon",
     "first_polygon_area_gdf",
     (7, 6),
     None,
+    "graph_1",
     does_not_raise(),
 )
 @P.case(  # type: ignore
     "Return infrastructure when multiple overlapping polygons",
-    "multiple_polygons_overlaping_area_gdf",
-    (7, 6),
+    "multiple_polygons_overlapping_area_gdf",
+    (7, 7),  # FIXME: should be (7, 6)
     None,
+    "graph_1",
     does_not_raise(),
 )
 @P.case(  # type: ignore
     "Return infrastructure when node without any edges",  # FIXME: shouldn't have a node w/o an edge
-    "multiple_polygons_overlaping_area_gdf",
+    "multiple_polygons_overlapping_area_gdf",
     (9, 7),
-    {"network_type": NetworkType.BIKE, "contain_within_area": True},
+    {"network_type": OSMNetworkType.BIKE, "contain_within_area": True},
+    "graph_2",
     does_not_raise(),
 )
 @P.case(  # type: ignore
     "Return infrastructure when multipolygon",
     "multipolygons_area_gdf",
     (11, 9),
     None,
+    "graph_3",
     does_not_raise(),
 )
 @P.case(  # type: ignore
     "Return infrastructure when correct polygon and polygon with no road infrastructure",
     "valid_and_empty_polygons_area_gdf",
     (7, 6),
     None,
+    "graph_1",
     does_not_raise(),
 )
 @P.case(  # type: ignore
     "Return infrastructure without preprocessing",
     "first_polygon_area_gdf",
     (7, 6),
-    {"network_type": NetworkType.DRIVE, "preprocess": False},
+    {"network_type": OSMNetworkType.DRIVE, "preprocess": False},
+    "graph_1",
     does_not_raise(),
 )
 @P.case(  # type: ignore
     "Return infrastructure in long format",
     "first_polygon_area_gdf",
     (7, 6),
-    {"network_type": NetworkType.DRIVE, "wide": False},
+    {"network_type": OSMNetworkType.DRIVE, "wide": False},
+    "graph_1",
     does_not_raise(),
 )
 @P.case(  # type: ignore
     "Return infrastructure when network_type supplied as a string",
     "first_polygon_area_gdf",
     (7, 6),
     {"network_type": "drive", "wide": False},
+    "graph_4",
     does_not_raise(),
 )
 def test_contract(
     area_gdf_fixture: str,
     expected_result: Optional[Tuple[int, int]],
     loader_params: Optional[Dict[str, Any]],
+    file_name: Optional[str],
     expectation,
     request: pytest.FixtureRequest,
     mocker: MockerFixture,
 ):
     """Test `OSMWayLoader.load`'s contract."""
     if not loader_params:
-        loader_params = {"network_type": NetworkType.DRIVE}
+        loader_params = {"network_type": OSMNetworkType.DRIVE}
 
     loader = OSMWayLoader(**loader_params)
 
     area_gdf = request.getfixturevalue(area_gdf_fixture)
     nodes_expected_len, edges_expected_len = expected_result or (None, None)
 
-    def patched_graph_from_polygon(*args, **kwargs) -> Any:  # type: ignore
-        polygon = args[0]
-
-        name_hashed = hashlib.md5(f"{polygon.wkt}{list(kwargs.values())}".encode()).hexdigest()
-
-        if name_hashed == "785de42ad57bbe33298128212ef9dd71":
+    def patched_graph_from_polygon(f_name: str, *args, **kwargs) -> Any:  # type: ignore
+        if f_name == "type_error":
             raise TypeError
-        elif name_hashed == "de17f3ef99794666b8a16931a9df4e49":
+        elif f_name == "empty_overpass_response":
             raise osmnx._errors.EmptyOverpassResponse
 
-        files_path = Path(__file__).parent / "files"
-        file_name = name_hashed + ".pkl"
+        files_path = Path(__file__).parent / "test_files"
+        file_name = f_name + ".pkl"
         file_path = files_path / file_name
 
         with file_path.open("rb") as f:
             res = pkl.load(f)
 
         return res
 
     with expectation:
-        mocker.patch("osmnx.graph_from_polygon", wraps=patched_graph_from_polygon)
+        mocker.patch(
+            "osmnx.graph_from_polygon",
+            wraps=partial(patched_graph_from_polygon, file_name),
+        )
         nodes, edges = loader.load(area_gdf)
 
         check.equal(len(nodes), nodes_expected_len)
         check.equal(len(edges), edges_expected_len)
         check.is_in(GEOMETRY_COLUMN, nodes.columns)
         check.is_in(GEOMETRY_COLUMN, edges.columns)
 
@@ -402,15 +415,15 @@
         7.5,
     ],
 )  # type: ignore
 def test_preprocessing(
     column_name: str, input: Union[Any, Sequence[Any]], expected: Union[Any, Sequence[Any]]
 ) -> None:
     """Test `OSMWayLoader._sanitize_and_normalize()` preprocessing."""
-    loader = OSMWayLoader(network_type=NetworkType.DRIVE)
+    loader = OSMWayLoader(network_type=OSMNetworkType.DRIVE)
 
     input = list(input) if isinstance(input, Sequence) else [input]
     expected = list(expected) if isinstance(expected, Sequence) else [expected]
 
     if len(expected) == 1:
         expected = expected * len(input)
```

### Comparing `srai-0.2.0/tests/loaders/test_files/example.parquet` & `srai-0.3.0/tests/loaders/test_files/example.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/loaders/test_geoparquet_loader.py` & `srai-0.3.0/tests/loaders/test_geoparquet_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/loaders/test_gtfs_loader.py` & `srai-0.3.0/tests/loaders/test_gtfs_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/miscellaneous/test_optional_dependencies.py` & `srai-0.3.0/tests/miscellaneous/test_optional_dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 from contextlib import nullcontext as does_not_raise
 from typing import Any, List
 
 import geopandas as gpd
 import pytest
 from shapely.geometry import box
 
+from srai._optional import ImportErrorHandle, import_optional_dependency
 from srai.constants import GEOMETRY_COLUMN, REGIONS_INDEX, WGS84_CRS
-from srai.utils._optional import ImportErrorHandle, import_optional_dependency
 
 
 @pytest.fixture  # type: ignore
 def optional_packages() -> List[str]:
     """Get a list with optional packages."""
     return [
         "osmium",
         "osmnx",
         "overpass",
         "pymap3d",
         "haversine",
+        "scipy",
         "spherical_geometry",
         "gtfs_kit",
         "folium",
         "mapclassify",
         "plotly",
         "kaleido",
         "pytorch-lightning",
```

### Comparing `srai-0.2.0/tests/neighbourhoods/h3/test_with_regions.py` & `srai-0.3.0/tests/neighbourhoods/h3/test_with_regions.py`

 * *Files 26% similar despite different names*

```diff
@@ -77,59 +77,97 @@
     indices.remove("862bacc9fffffff")
     indices.remove("862baccd7ffffff")
     indices.remove("862baccdfffffff")
     return gpd.GeoDataFrame(index=indices)
 
 
 @pytest.mark.parametrize(  # type: ignore
-    "regions_gdf_fixture,expected",
+    "regions_gdf_fixture,expected,expected_with_include_center",
     [
         (
             "empty_gdf",
             set(),
+            set(),
         ),
         (
             "single_hex_gdf",
             set(),
+            {"811e3ffffffffff"},
         ),
         (
             "hex_without_one_neighbour_gdf",
             {
                 "811f3ffffffffff",
                 "811fbffffffffff",
                 "811ebffffffffff",
                 "811efffffffffff",
                 "811e7ffffffffff",
             },
+            {
+                "811f3ffffffffff",
+                "811fbffffffffff",
+                "811ebffffffffff",
+                "811efffffffffff",
+                "811e7ffffffffff",
+                "811e3ffffffffff",
+            },
         ),
     ],
 )
 def test_get_neighbours_with_regions_gdf(
-    regions_gdf_fixture: str, expected: Set[str], request: Any
+    regions_gdf_fixture: str,
+    expected: Set[str],
+    expected_with_include_center: Set[str],
+    request: Any,
 ) -> None:
     """Test get_neighbours of H3Neighbourhood with a specified regions GeoDataFrame."""
+    center_region = "811e3ffffffffff"
     regions_gdf = request.getfixturevalue(regions_gdf_fixture)
-    assert H3Neighbourhood(regions_gdf).get_neighbours("811e3ffffffffff") == expected
+
+    neighbourhood = H3Neighbourhood(regions_gdf)
+    assert neighbourhood.get_neighbours(center_region) == expected
+    assert (
+        neighbourhood.get_neighbours(center_region, include_center=True)
+        == expected_with_include_center
+    )
+
+    neighbourhood_with_include_center = H3Neighbourhood(regions_gdf, include_center=True)
+    assert (
+        neighbourhood_with_include_center.get_neighbours(center_region)
+        == expected_with_include_center
+    )
+    assert (
+        neighbourhood_with_include_center.get_neighbours(center_region, include_center=False)
+        == expected
+    )
 
 
 @pytest.mark.parametrize(  # type: ignore
-    "distance,expected",
+    "distance,expected,expected_with_include_center",
     [
         (
             0,
             set(),
+            {"862bac507ffffff"},
         ),
         (
             1,
             {
                 "862bac50fffffff",
                 "862bac517ffffff",
                 "862bac51fffffff",
                 "862bac527ffffff",
             },
+            {
+                "862bac50fffffff",
+                "862bac517ffffff",
+                "862bac51fffffff",
+                "862bac527ffffff",
+                "862bac507ffffff",
+            },
         ),
         (
             2,
             {
                 "862bac50fffffff",
                 "862bac517ffffff",
                 "862bac51fffffff",
@@ -140,60 +178,128 @@
                 "862bac437ffffff",
                 "862bac557ffffff",
                 "862bac577ffffff",
                 "862bac5a7ffffff",
                 "862bac5afffffff",
                 "862bacc8fffffff",
             },
+            {
+                "862bac50fffffff",
+                "862bac517ffffff",
+                "862bac51fffffff",
+                "862bac527ffffff",
+                "862ba124fffffff",
+                "862ba126fffffff",
+                "862bac427ffffff",
+                "862bac437ffffff",
+                "862bac557ffffff",
+                "862bac577ffffff",
+                "862bac5a7ffffff",
+                "862bac5afffffff",
+                "862bacc8fffffff",
+                "862bac507ffffff",
+            },
         ),
     ],
 )
 def test_get_neighbours_up_to_distance_with_regions_gdf(
-    distance: int, expected: Set[str], request: Any
+    distance: int, expected: Set[str], expected_with_include_center: Set[str], request: Any
 ) -> None:
     """Test get_neighbours_up_to_distance of H3Neighbourhood with a specified regions."""
+    center_region = "862bac507ffffff"
     regions_gdf = request.getfixturevalue("two_rings_regions_some_missing")
+
     neighbourhood = H3Neighbourhood(regions_gdf)
-    initial_region_index = "862bac507ffffff"
-    assert neighbourhood.get_neighbours_up_to_distance(initial_region_index, distance) == expected
+    assert neighbourhood.get_neighbours_up_to_distance(center_region, distance) == expected
+    assert (
+        neighbourhood.get_neighbours_up_to_distance(center_region, distance, include_center=True)
+        == expected_with_include_center
+    )
+
+    neighbourhood_with_include_center = H3Neighbourhood(regions_gdf, include_center=True)
+    assert (
+        neighbourhood_with_include_center.get_neighbours_up_to_distance(center_region, distance)
+        == expected_with_include_center
+    )
+    assert (
+        neighbourhood_with_include_center.get_neighbours_up_to_distance(
+            center_region, distance, include_center=False
+        )
+        == expected
+    )
 
 
 @pytest.mark.parametrize(  # type: ignore
-    "distance,expected",
+    "distance,expected,expected_with_include_center",
     [
         (
             0,
             set(),
+            {"862bac507ffffff"},
         ),
         (
             1,
             {
                 "862bac50fffffff",
                 "862bac517ffffff",
                 "862bac51fffffff",
                 "862bac527ffffff",
             },
+            {
+                "862bac50fffffff",
+                "862bac517ffffff",
+                "862bac51fffffff",
+                "862bac527ffffff",
+            },
         ),
         (
             2,
             {
                 "862ba124fffffff",
                 "862ba126fffffff",
                 "862bac427ffffff",
                 "862bac437ffffff",
                 "862bac557ffffff",
                 "862bac577ffffff",
                 "862bac5a7ffffff",
                 "862bac5afffffff",
                 "862bacc8fffffff",
             },
+            {
+                "862ba124fffffff",
+                "862ba126fffffff",
+                "862bac427ffffff",
+                "862bac437ffffff",
+                "862bac557ffffff",
+                "862bac577ffffff",
+                "862bac5a7ffffff",
+                "862bac5afffffff",
+                "862bacc8fffffff",
+            },
         ),
     ],
 )
 def test_get_neighbours_at_distance_with_regions_gdf(
-    distance: int, expected: Set[str], request: Any
+    distance: int, expected: Set[str], expected_with_include_center: Set[str], request: Any
 ) -> None:
     """Test get_neighbours_at_distance of H3Neighbourhood with a specified regions GeoDataFrame."""
+    center_region = "862bac507ffffff"
     regions_gdf = request.getfixturevalue("two_rings_regions_some_missing")
+
     neighbourhood = H3Neighbourhood(regions_gdf)
-    initial_region_index = "862bac507ffffff"
-    assert neighbourhood.get_neighbours_at_distance(initial_region_index, distance) == expected
+    assert neighbourhood.get_neighbours_at_distance(center_region, distance) == expected
+    assert (
+        neighbourhood.get_neighbours_at_distance(center_region, distance, include_center=True)
+        == expected_with_include_center
+    )
+
+    neighbourhood_with_include_center = H3Neighbourhood(regions_gdf, include_center=True)
+    assert (
+        neighbourhood_with_include_center.get_neighbours_at_distance(center_region, distance)
+        == expected_with_include_center
+    )
+    assert (
+        neighbourhood_with_include_center.get_neighbours_at_distance(
+            center_region, distance, include_center=False
+        )
+        == expected
+    )
```

### Comparing `srai-0.2.0/tests/neighbourhoods/test_adjacency_neighbourhood.py` & `srai-0.3.0/tests/neighbourhoods/test_adjacency_neighbourhood.py`

 * *Files 23% similar despite different names*

```diff
@@ -97,30 +97,52 @@
 
 def test_empty_gdf_empty_set(empty_gdf: gpd.GeoDataFrame) -> None:
     """Test checks if empty GeoDataFrames return empty neighbourhoods."""
     neighbourhood = AdjacencyNeighbourhood(empty_gdf)
     assert neighbourhood.get_neighbours(1) == set()
 
 
+def test_empty_gdf_empty_set_include_center(empty_gdf: gpd.GeoDataFrame) -> None:
+    """Test checks if empty GeoDataFrames return empty neighbourhoods."""
+    neighbourhood = AdjacencyNeighbourhood(empty_gdf, include_center=True)
+    assert neighbourhood.get_neighbours(1) == set()
+
+
 def test_lazy_loading_empty_set(squares_regions_fixture: gpd.GeoDataFrame) -> None:
     """Test checks if lookup table is empty after init."""
     neighbourhood = AdjacencyNeighbourhood(squares_regions_fixture)
     assert neighbourhood.lookup == {}
 
 
+def test_lazy_loading_empty_set_include_center(squares_regions_fixture: gpd.GeoDataFrame) -> None:
+    """Test checks if lookup table is empty after init."""
+    neighbourhood = AdjacencyNeighbourhood(squares_regions_fixture, include_center=True)
+    assert neighbourhood.lookup == {}
+
+
 def test_adjacency_lazy_loading(rounded_regions_fixture: gpd.GeoDataFrame) -> None:
     """Test checks if lookup table is lazily populated."""
     neighbourhood = AdjacencyNeighbourhood(rounded_regions_fixture)
     neighbours = neighbourhood.get_neighbours("SW")
     assert neighbours == {"W", "S"}
     assert neighbourhood.lookup == {
         "SW": {"W", "S"},
     }
 
 
+def test_adjacency_lazy_loading_include_center(rounded_regions_fixture: gpd.GeoDataFrame) -> None:
+    """Test checks if lookup table is lazily populated."""
+    neighbourhood = AdjacencyNeighbourhood(rounded_regions_fixture, include_center=True)
+    neighbours = neighbourhood.get_neighbours("SW")
+    assert neighbours == {"W", "S", "SW"}
+    assert neighbourhood.lookup == {
+        "SW": {"W", "S", "SW"},
+    }
+
+
 def test_generate_all_neighbourhoods_rounded_regions(
     rounded_regions_fixture: gpd.GeoDataFrame,
 ) -> None:
     """Test checks `generate_neighbourhoods` function with rounded regions."""
     neighbourhood = AdjacencyNeighbourhood(rounded_regions_fixture)
     neighbourhood.generate_neighbourhoods()
     assert neighbourhood.lookup == {
@@ -152,68 +174,125 @@
         "NW": {"W", "N", "CENTER"},
         "N": {"W", "CENTER", "E", "NW", "NE"},
         "NE": {"E", "N", "CENTER"},
     }
 
 
 @pytest.mark.parametrize(  # type: ignore
-    "index, distance, neighbours_expected",
+    "index,distance,expected,expected_include_center",
     [
-        ("SW", -2, set()),
-        ("SW", -1, set()),
-        ("SW", 0, set()),
-        ("SW", 1, {"S", "W"}),
-        ("SW", 2, {"CENTER", "SE", "NW"}),
-        ("SW", 3, {"N", "E"}),
-        ("SW", 4, {"NE"}),
-        ("SW", 5, set()),
-        ("CENTER", 1, {"N", "E", "S", "W"}),
-        ("CENTER", 2, {"NW", "NE", "SW", "SE"}),
-        ("CENTER", 3, set()),
-        ("N", 1, {"NW", "NE", "CENTER"}),
-        ("N", 2, {"E", "S", "W"}),
-        ("N", 3, {"SE", "SW"}),
-        ("N", 4, set()),
+        ("SW", -2, set(), set()),
+        ("SW", -1, set(), set()),
+        ("SW", 0, set(), {"SW"}),
+        ("SW", 1, {"S", "W"}, {"S", "W"}),
+        ("SW", 2, {"CENTER", "SE", "NW"}, {"CENTER", "SE", "NW"}),
+        ("SW", 3, {"N", "E"}, {"N", "E"}),
+        ("SW", 4, {"NE"}, {"NE"}),
+        ("SW", 5, set(), set()),
+        ("CENTER", 0, set(), {"CENTER"}),
+        ("CENTER", 1, {"N", "E", "S", "W"}, {"N", "E", "S", "W"}),
+        ("CENTER", 2, {"NW", "NE", "SW", "SE"}, {"NW", "NE", "SW", "SE"}),
+        ("CENTER", 3, set(), set()),
+        ("N", 0, set(), {"N"}),
+        ("N", 1, {"NW", "NE", "CENTER"}, {"NW", "NE", "CENTER"}),
+        ("N", 2, {"E", "S", "W"}, {"E", "S", "W"}),
+        ("N", 3, {"SE", "SW"}, {"SE", "SW"}),
+        ("N", 4, set(), set()),
     ],
 )
 def test_adjacency_lazy_loading_at_distance(
     index: str,
     distance: int,
-    neighbours_expected: Set[str],
+    expected: Set[str],
+    expected_include_center: Set[str],
     rounded_regions_fixture: gpd.GeoDataFrame,
 ) -> None:
     """Test checks `get_neighbours_at_distance` function with rounded regions."""
     neighbourhood = AdjacencyNeighbourhood(rounded_regions_fixture)
     neighbours = neighbourhood.get_neighbours_at_distance(index, distance)
-    assert neighbours == neighbours_expected
+    assert neighbours == expected
+    neighbours = neighbourhood.get_neighbours_at_distance(index, distance, include_center=True)
+    assert neighbours == expected_include_center
+
+    neighbourhood = AdjacencyNeighbourhood(rounded_regions_fixture, include_center=True)
+    neighbours = neighbourhood.get_neighbours_at_distance(index, distance)
+    assert neighbours == expected_include_center
+    neighbours = neighbourhood.get_neighbours_at_distance(index, distance, include_center=False)
+    assert neighbours == expected
 
 
 @pytest.mark.parametrize(  # type: ignore
-    "index, distance, neighbours_expected",
+    "index,distance,expected,expected_include_center",
     [
-        ("SW", -2, set()),
-        ("SW", -1, set()),
-        ("SW", 0, set()),
-        ("SW", 1, {"S", "W"}),
-        ("SW", 2, {"S", "W", "CENTER", "SE", "NW"}),
-        ("SW", 3, {"S", "W", "CENTER", "SE", "NW", "N", "E"}),
-        ("SW", 4, {"S", "W", "CENTER", "SE", "NW", "N", "E", "NE"}),
-        ("SW", 5, {"S", "W", "CENTER", "SE", "NW", "N", "E", "NE"}),
-        ("CENTER", 1, {"N", "E", "S", "W"}),
-        ("CENTER", 2, {"N", "E", "S", "W", "NW", "NE", "SW", "SE"}),
-        ("CENTER", 3, {"N", "E", "S", "W", "NW", "NE", "SW", "SE"}),
-        ("N", 1, {"NW", "NE", "CENTER"}),
-        ("N", 2, {"NW", "NE", "CENTER", "E", "S", "W"}),
-        ("N", 3, {"NW", "NE", "CENTER", "E", "S", "W", "SE", "SW"}),
-        ("N", 4, {"NW", "NE", "CENTER", "E", "S", "W", "SE", "SW"}),
+        ("SW", -2, set(), set()),
+        ("SW", -1, set(), set()),
+        ("SW", 0, set(), {"SW"}),
+        ("SW", 1, {"S", "W"}, {"SW", "S", "W"}),
+        ("SW", 2, {"S", "W", "CENTER", "SE", "NW"}, {"SW", "S", "W", "CENTER", "SE", "NW"}),
+        (
+            "SW",
+            3,
+            {"S", "W", "CENTER", "SE", "NW", "N", "E"},
+            {"SW", "S", "W", "CENTER", "SE", "NW", "N", "E"},
+        ),
+        (
+            "SW",
+            4,
+            {"S", "W", "CENTER", "SE", "NW", "N", "E", "NE"},
+            {"SW", "S", "W", "CENTER", "SE", "NW", "N", "E", "NE"},
+        ),
+        (
+            "SW",
+            5,
+            {"S", "W", "CENTER", "SE", "NW", "N", "E", "NE"},
+            {"SW", "S", "W", "CENTER", "SE", "NW", "N", "E", "NE"},
+        ),
+        ("CENTER", 0, set(), {"CENTER"}),
+        ("CENTER", 1, {"N", "E", "S", "W"}, {"CENTER", "N", "E", "S", "W"}),
+        (
+            "CENTER",
+            2,
+            {"N", "E", "S", "W", "NW", "NE", "SW", "SE"},
+            {"CENTER", "N", "E", "S", "W", "NW", "NE", "SW", "SE"},
+        ),
+        (
+            "CENTER",
+            3,
+            {"N", "E", "S", "W", "NW", "NE", "SW", "SE"},
+            {"CENTER", "N", "E", "S", "W", "NW", "NE", "SW", "SE"},
+        ),
+        ("N", 0, set(), {"N"}),
+        ("N", 1, {"NW", "NE", "CENTER"}, {"N", "NW", "NE", "CENTER"}),
+        ("N", 2, {"NW", "NE", "CENTER", "E", "S", "W"}, {"N", "NW", "NE", "CENTER", "E", "S", "W"}),
+        (
+            "N",
+            3,
+            {"NW", "NE", "CENTER", "E", "S", "W", "SE", "SW"},
+            {"N", "NW", "NE", "CENTER", "E", "S", "W", "SE", "SW"},
+        ),
+        (
+            "N",
+            4,
+            {"NW", "NE", "CENTER", "E", "S", "W", "SE", "SW"},
+            {"N", "NW", "NE", "CENTER", "E", "S", "W", "SE", "SW"},
+        ),
     ],
 )
 def test_adjacency_lazy_loading_up_to_distance(
     index: str,
     distance: int,
-    neighbours_expected: Set[str],
+    expected: Set[str],
+    expected_include_center: Set[str],
     rounded_regions_fixture: gpd.GeoDataFrame,
 ) -> None:
     """Test checks `get_neighbours_up_to_distance` function with rounded regions."""
     neighbourhood = AdjacencyNeighbourhood(rounded_regions_fixture)
     neighbours = neighbourhood.get_neighbours_up_to_distance(index, distance)
-    assert neighbours == neighbours_expected
+    assert neighbours == expected
+    neighbours = neighbourhood.get_neighbours_up_to_distance(index, distance, include_center=True)
+    assert neighbours == expected_include_center
+
+    neighbourhood = AdjacencyNeighbourhood(rounded_regions_fixture, include_center=True)
+    neighbours = neighbourhood.get_neighbours_up_to_distance(index, distance)
+    assert neighbours == expected_include_center
+    neighbours = neighbourhood.get_neighbours_up_to_distance(index, distance, include_center=False)
+    assert neighbours == expected
```

### Comparing `srai-0.2.0/tests/regionalizers/conftest.py` & `srai-0.3.0/tests/regionalizers/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-"""Conftest for Regionalizers."""
+"""Fixtures for Regionalizers."""
+
+from typing import List
 
 import geopandas as gpd
 import pytest
 from shapely import geometry
 
 from srai.constants import GEOMETRY_COLUMN, WGS84_CRS
 
@@ -93,27 +95,31 @@
             )
         ],
         crs=WGS84_CRS,
     )
 
 
 @pytest.fixture  # type: ignore
-def gdf_earth_poles() -> gpd.GeoDataFrame:
+def earth_poles() -> List[geometry.Point]:
+    """Get 6 Earth poles."""
+    return [
+        geometry.Point(0, 0),
+        geometry.Point(90, 0),
+        geometry.Point(180, 0),
+        geometry.Point(-90, 0),
+        geometry.Point(0, 90),
+        geometry.Point(0, -90),
+    ]
+
+
+@pytest.fixture  # type: ignore
+def gdf_earth_poles(earth_poles) -> gpd.GeoDataFrame:
     """Get GeoDataFrame with 6 Earth poles."""
     return gpd.GeoDataFrame(
-        {
-            GEOMETRY_COLUMN: [
-                geometry.Point(0, 0),
-                geometry.Point(90, 0),
-                geometry.Point(180, 0),
-                geometry.Point(-90, 0),
-                geometry.Point(0, 90),
-                geometry.Point(0, -90),
-            ]
-        },
+        {GEOMETRY_COLUMN: earth_poles},
         index=[1, 2, 3, 4, 5, 6],
         crs=WGS84_CRS,
     )
 
 
 @pytest.fixture  # type: ignore
 def gdf_poland() -> gpd.GeoDataFrame:
```

### Comparing `srai-0.2.0/tests/regionalizers/test_administrative_boundary_regionalizer.py` & `srai-0.3.0/tests/regionalizers/test_administrative_boundary_regionalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import geopandas as gpd
 import pytest
 from overpass import API
 from pytest_mock import MockerFixture
 from shapely.geometry import Point, box
 
 from srai.constants import GEOMETRY_COLUMN, WGS84_CRS
+from srai.geometry import merge_disjointed_gdf_geometries
 from srai.regionalizers import AdministrativeBoundaryRegionalizer
-from srai.utils import merge_disjointed_gdf_geometries
 
 bbox = box(minx=-180, maxx=180, miny=-90, maxy=90)
 bbox_gdf = gpd.GeoDataFrame({GEOMETRY_COLUMN: [bbox]}, crs=WGS84_CRS)
 
 
 @pytest.mark.parametrize(  # type: ignore
     "admin_level,expectation",
```

### Comparing `srai-0.2.0/tests/regionalizers/test_h3_regionalizer.py` & `srai-0.3.0/tests/regionalizers/test_h3_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/regionalizers/test_s2_regionalizer.py` & `srai-0.3.0/tests/regionalizers/test_s2_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/tests/regionalizers/test_slippy_map_regionalizer.py` & `srai-0.3.0/tests/regionalizers/test_slippy_map_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.2.0/PKG-INFO` & `srai-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srai
-Version: 0.2.0
+Version: 0.3.0
 Summary: A set of python modules for geospatial machine learning and data mining
 Author: Piotr Gramacki, Kacper Leśniara, Kamil Raczycki, Szymon Woźniak
 Author-Email: SRAI Lab <spatialrepresentationsforai@gmail.com>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -28,27 +28,28 @@
 Requires-Dist: geopandas
 Requires-Dist: shapely
 Requires-Dist: h3>=4.0.0b1
 Requires-Dist: numpy
 Requires-Dist: geoparquet
 Requires-Dist: pyfunctional
 Requires-Dist: rtree
-Requires-Dist: scipy
 Requires-Dist: pyarrow
 Requires-Dist: topojson
 Requires-Dist: tqdm
 Requires-Dist: s2
 Requires-Dist: typeguard
 Requires-Dist: requests
+Requires-Dist: h3ronpy>=0.17.4
 Requires-Dist: osmium; extra == "osm"
-Requires-Dist: osmnx<=1.4.0; extra == "osm"
+Requires-Dist: osmnx; extra == "osm"
 Requires-Dist: overpass; extra == "osm"
 Requires-Dist: pillow; extra == "osm"
 Requires-Dist: pymap3d; extra == "voronoi"
 Requires-Dist: haversine; extra == "voronoi"
+Requires-Dist: scipy; extra == "voronoi"
 Requires-Dist: spherical-geometry; extra == "voronoi"
 Requires-Dist: gtfs-kit; extra == "gtfs"
 Requires-Dist: folium; extra == "plotting"
 Requires-Dist: mapclassify; extra == "plotting"
 Requires-Dist: matplotlib; extra == "plotting"
 Requires-Dist: plotly; extra == "plotting"
 Requires-Dist: kaleido<=0.2.1; extra == "plotting"
@@ -158,16 +159,16 @@
 * `OSMOnlineLoader` - downloads data from OpenStreetMap API using [osmnx](https://github.com/gboeing/osmnx) - this is faster for smaller areas or tags counts
 * `OSMPbfLoader` - loads data from automatically downloaded PBF file from [protomaps](https://protomaps.com/) - this is faster for larger areas or tags counts
 
 Example with `OSMOnlineLoader`:
 
 ```python
 from srai.loaders import OSMOnlineLoader
-from srai.utils import geocode_to_region_gdf
 from srai.plotting import plot_regions
+from srai.regionalizers import geocode_to_region_gdf
 
 query = {"leisure": "park"}
 area = geocode_to_region_gdf("Wrocław, Poland")
 loader = OSMOnlineLoader()
 
 parks_gdf = loader.load(area, query)
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0)"], tiles_style="CartoDB positron")
@@ -179,21 +180,20 @@
 </p>
 
 ### Downloading road network
 
 Road network downloading is a special case of OSM data downloading. To download road network for a given area, use `OSMWayLoader` class:
 
 ```python
-from srai.loaders import OSMWayLoader
-from srai.loaders.osm_way_loader import NetworkType
-from srai.utils import geocode_to_region_gdf
+from srai.loaders import OSMNetworkType, OSMWayLoader
 from srai.plotting import plot_regions
+from srai.regionalizers import geocode_to_region_gdf
 
 area = geocode_to_region_gdf("Utrecht, Netherlands")
-loader = OSMWayLoader(NetworkType.BIKE)
+loader = OSMWayLoader(OSMNetworkType.BIKE)
 
 nodes, edges = loader.load(area)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
 edges[["geometry"]].explore(m=folium_map, color="seagreen")
 ```
 
@@ -204,17 +204,17 @@
 ### Downloading GTFS data
 
 To extract features from GTFS use `GTFSLoader`. It will extract trip count and available directions for each stop in 1h time windows.
 
 ```python
 from pathlib import Path
 
-from srai.loaders import GTFSLoader
-from srai.utils import geocode_to_region_gdf, download_file
+from srai.loaders import GTFSLoader, download_file
 from srai.plotting import plot_regions
+from srai.regionalizers import geocode_to_region_gdf
 
 area = geocode_to_region_gdf("Vienna, Austria")
 gtfs_file = Path("vienna_gtfs.zip")
 download_file("https://transitfeeds.com/p/stadt-wien/888/latest/download", gtfs_file.as_posix())
 loader = GTFSLoader()
 
 features = loader.load(gtfs_file)
@@ -235,16 +235,15 @@
 * `S2Regionalizer` - regionalization using [Google's S2 library](https://github.com/google/s2geometry)
 * `VoronoiRegionalizer` - regionalization using Voronoi diagram
 * `AdministativeBoundaryRegionalizer` - regionalization using administrative boundaries
 
 Example:
 
 ```python
-from srai.regionalizers import H3Regionalizer
-from srai.utils import geocode_to_region_gdf
+from srai.regionalizers import H3Regionalizer, geocode_to_region_gdf
 
 area = geocode_to_region_gdf("Berlin, Germany")
 regionalizer = H3Regionalizer(resolution=7)
 
 regions = regionalizer.transform(area)
 
 folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
@@ -268,16 +267,15 @@
 All of those methods share the same API. All of them require results from `Loader` (load features), `Regionalizer` (split area into regions) and `Joiner` (join features to regions) to work. An example using `CountEmbedder`:
 
 ```python
 from srai.embedders import CountEmbedder
 from srai.joiners import IntersectionJoiner
 from srai.loaders import OSMOnlineLoader
 from srai.plotting import plot_regions, plot_numeric_data
-from srai.regionalizers import H3Regionalizer
-from srai.utils import geocode_to_region_gdf
+from srai.regionalizers import H3Regionalizer, geocode_to_region_gdf
 
 loader = OSMOnlineLoader()
 regionalizer = H3Regionalizer(resolution=9)
 joiner = IntersectionJoiner()
 
 query = {"amenity": "bicycle_parking"}
 area = geocode_to_region_gdf("Malmö, Sweden")
@@ -300,16 +298,15 @@
 
 ```python
 from srai.embedders import Hex2VecEmbedder
 from srai.joiners import IntersectionJoiner
 from srai.loaders import OSMPbfLoader
 from srai.loaders.osm_loaders.filters import HEX2VEC_FILTER
 from srai.neighbourhoods.h3_neighbourhood import H3Neighbourhood
-from srai.regionalizers import H3Regionalizer
-from srai.utils import geocode_to_region_gdf
+from srai.regionalizers import H3Regionalizer, geocode_to_region_gdf
 from srai.plotting import plot_regions, plot_numeric_data
 
 loader = OSMPbfLoader()
 regionalizer = H3Regionalizer(resolution=11)
 joiner = IntersectionJoiner()
 
 area = geocode_to_region_gdf("City of London")
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: srai Version: 0.2.0 Summary: A set of python
+Metadata-Version: 2.1 Name: srai Version: 0.3.0 Summary: A set of python
 modules for geospatial machine learning and data mining Author: Piotr Gramacki,
 Kacper LeÅniara, Kamil Raczycki, Szymon WoÅºniak Author-Email: SRAI Lab
 gmail.com> License: Apache-2.0 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: GIS Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
@@ -13,28 +13,29 @@
 Operating System :: Microsoft :: Windows Project-URL: Homepage, https://srai-
 lab.github.io/srai Project-URL: Repository, https://github.com/srai-lab/srai
 Project-URL: Documentation, https://srai-lab.github.io/srai Project-URL:
 Changelog, https://github.com/srai-lab/srai/blob/main/CHANGELOG.md Requires-
 Python: >=3.8 Requires-Dist: pandas Requires-Dist: geopandas Requires-Dist:
 shapely Requires-Dist: h3>=4.0.0b1 Requires-Dist: numpy Requires-Dist:
 geoparquet Requires-Dist: pyfunctional Requires-Dist: rtree Requires-Dist:
-scipy Requires-Dist: pyarrow Requires-Dist: topojson Requires-Dist: tqdm
-Requires-Dist: s2 Requires-Dist: typeguard Requires-Dist: requests Requires-
-Dist: osmium; extra == "osm" Requires-Dist: osmnx<=1.4.0; extra == "osm"
+pyarrow Requires-Dist: topojson Requires-Dist: tqdm Requires-Dist: s2 Requires-
+Dist: typeguard Requires-Dist: requests Requires-Dist: h3ronpy>=0.17.4
+Requires-Dist: osmium; extra == "osm" Requires-Dist: osmnx; extra == "osm"
 Requires-Dist: overpass; extra == "osm" Requires-Dist: pillow; extra == "osm"
 Requires-Dist: pymap3d; extra == "voronoi" Requires-Dist: haversine; extra ==
-"voronoi" Requires-Dist: spherical-geometry; extra == "voronoi" Requires-Dist:
-gtfs-kit; extra == "gtfs" Requires-Dist: folium; extra == "plotting" Requires-
-Dist: mapclassify; extra == "plotting" Requires-Dist: matplotlib; extra ==
-"plotting" Requires-Dist: plotly; extra == "plotting" Requires-Dist:
-kaleido<=0.2.1; extra == "plotting" Requires-Dist: pytorch-lightning; extra ==
-"torch" Requires-Dist: torch; extra == "torch" Requires-Dist: srai
-[gtfs,osm,plotting,torch,voronoi]; extra == "all" Provides-Extra: osm Provides-
-Extra: voronoi Provides-Extra: gtfs Provides-Extra: plotting Provides-Extra:
-torch Provides-Extra: all Description-Content-Type: text/markdown
+"voronoi" Requires-Dist: scipy; extra == "voronoi" Requires-Dist: spherical-
+geometry; extra == "voronoi" Requires-Dist: gtfs-kit; extra == "gtfs" Requires-
+Dist: folium; extra == "plotting" Requires-Dist: mapclassify; extra ==
+"plotting" Requires-Dist: matplotlib; extra == "plotting" Requires-Dist:
+plotly; extra == "plotting" Requires-Dist: kaleido<=0.2.1; extra == "plotting"
+Requires-Dist: pytorch-lightning; extra == "torch" Requires-Dist: torch; extra
+== "torch" Requires-Dist: srai[gtfs,osm,plotting,torch,voronoi]; extra == "all"
+Provides-Extra: osm Provides-Extra: voronoi Provides-Extra: gtfs Provides-
+Extra: plotting Provides-Extra: torch Provides-Extra: all Description-Content-
+Type: text/markdown
  [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/logos/srai-
                              logo-transparent.png]
   [GitHub] [Checks] [GitHub_Workflow_Status_-_DEV] [GitHub_Workflow_Status_-
  PROD] [pre-commit.ci_status] [CodeFactor_Grade] [Codecov] [Package_version]
                 [Supported_Python_versions] [PyPI_-_Downloads]
 # Spatial Representations for Artificial Intelligence
   â ï¸ð§ This library is under HEAVY development. Expect breaking changes
@@ -86,103 +87,103 @@
 17z2OYZG82FZNRK86Kt-eSgbJn9m7meSH?usp=sharing) ### Downloading OSM data To
 download OSM data for a given area, using a set of tags use one of `OSMLoader`
 classes: * `OSMOnlineLoader` - downloads data from OpenStreetMap API using
 [osmnx](https://github.com/gboeing/osmnx) - this is faster for smaller areas or
 tags counts * `OSMPbfLoader` - loads data from automatically downloaded PBF
 file from [protomaps](https://protomaps.com/) - this is faster for larger areas
 or tags counts Example with `OSMOnlineLoader`: ```python from srai.loaders
-import OSMOnlineLoader from srai.utils import geocode_to_region_gdf from
-srai.plotting import plot_regions query = {"leisure": "park"} area =
-geocode_to_region_gdf("WrocÅaw, Poland") loader = OSMOnlineLoader() parks_gdf
-= loader.load(area, query) folium_map = plot_regions(area, colormap=["rgba
-(0,0,0,0)"], tiles_style="CartoDB positron") parks_gdf.explore(m=folium_map,
-color="forestgreen") ```
+import OSMOnlineLoader from srai.plotting import plot_regions from
+srai.regionalizers import geocode_to_region_gdf query = {"leisure": "park"}
+area = geocode_to_region_gdf("WrocÅaw, Poland") loader = OSMOnlineLoader()
+parks_gdf = loader.load(area, query) folium_map = plot_regions(area, colormap=
+["rgba(0,0,0,0)"], tiles_style="CartoDB positron") parks_gdf.explore
+(m=folium_map, color="forestgreen") ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                            downloading_osm_data.jpg]
 ### Downloading road network Road network downloading is a special case of OSM
 data downloading. To download road network for a given area, use `OSMWayLoader`
-class: ```python from srai.loaders import OSMWayLoader from
-srai.loaders.osm_way_loader import NetworkType from srai.utils import
-geocode_to_region_gdf from srai.plotting import plot_regions area =
-geocode_to_region_gdf("Utrecht, Netherlands") loader = OSMWayLoader
-(NetworkType.BIKE) nodes, edges = loader.load(area) folium_map = plot_regions
-(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron") edges[
-["geometry"]].explore(m=folium_map, color="seagreen") ```
+class: ```python from srai.loaders import OSMNetworkType, OSMWayLoader from
+srai.plotting import plot_regions from srai.regionalizers import
+geocode_to_region_gdf area = geocode_to_region_gdf("Utrecht, Netherlands")
+loader = OSMWayLoader(OSMNetworkType.BIKE) nodes, edges = loader.load(area)
+folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"],
+tiles_style="CartoDB positron") edges[["geometry"]].explore(m=folium_map,
+color="seagreen") ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                       downloading_road_network_data.jpg]
 ### Downloading GTFS data To extract features from GTFS use `GTFSLoader`. It
 will extract trip count and available directions for each stop in 1h time
-windows. ```python from pathlib import Path from srai.loaders import GTFSLoader
-from srai.utils import geocode_to_region_gdf, download_file from srai.plotting
-import plot_regions area = geocode_to_region_gdf("Vienna, Austria") gtfs_file =
-Path("vienna_gtfs.zip") download_file("https://transitfeeds.com/p/stadt-wien/
-888/latest/download", gtfs_file.as_posix()) loader = GTFSLoader() features =
-loader.load(gtfs_file) folium_map = plot_regions(area, colormap=["rgba
-(0,0,0,0.1)"], tiles_style="CartoDB positron") features[["trips_at_8",
-"geometry"]].explore("trips_at_8", m=folium_map) ```
+windows. ```python from pathlib import Path from srai.loaders import
+GTFSLoader, download_file from srai.plotting import plot_regions from
+srai.regionalizers import geocode_to_region_gdf area = geocode_to_region_gdf
+("Vienna, Austria") gtfs_file = Path("vienna_gtfs.zip") download_file("https://
+transitfeeds.com/p/stadt-wien/888/latest/download", gtfs_file.as_posix())
+loader = GTFSLoader() features = loader.load(gtfs_file) folium_map =
+plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB
+positron") features[["trips_at_8", "geometry"]].explore("trips_at_8",
+m=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                           downloading_gtfs_data.jpg]
 ### Regionalization Regionalization is a process of dividing a given area into
 smaller regions. This can be done in a variety of ways: * `H3Regionalizer` -
 regionalization using [Uber's H3 library](https://github.com/uber/h3) *
 `S2Regionalizer` - regionalization using [Google's S2 library](https://
 github.com/google/s2geometry) * `VoronoiRegionalizer` - regionalization using
 Voronoi diagram * `AdministativeBoundaryRegionalizer` - regionalization using
 administrative boundaries Example: ```python from srai.regionalizers import
-H3Regionalizer from srai.utils import geocode_to_region_gdf area =
-geocode_to_region_gdf("Berlin, Germany") regionalizer = H3Regionalizer
-(resolution=7) regions = regionalizer.transform(area) folium_map = plot_regions
-(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron")
-plot_regions(regions_gdf=regions, map=folium_map) ```
+H3Regionalizer, geocode_to_region_gdf area = geocode_to_region_gdf("Berlin,
+Germany") regionalizer = H3Regionalizer(resolution=7) regions =
+regionalizer.transform(area) folium_map = plot_regions(area, colormap=["rgba
+(0,0,0,0.1)"], tiles_style="CartoDB positron") plot_regions
+(regions_gdf=regions, map=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                              regionalization.jpg]
 ### Embedding Embedding is a process of mapping regions into a vector space.
 This can be done in a variety of ways: * `Hex2VecEmbedder` - embedding using
 hex2vec[1] algorithm * `GTFS2VecEmbedder` - embedding using GTFS2Vec[2]
 algorithm * `CountEmbedder` - embedding based on features counts *
 `ContextualCountEmbedder` - embedding based on features counts with
 neighbourhood context (proposed in [3]) * `Highway2VecEmbedder` - embedding
 using Highway2Vec[4] algorithm All of those methods share the same API. All of
 them require results from `Loader` (load features), `Regionalizer` (split area
 into regions) and `Joiner` (join features to regions) to work. An example using
 `CountEmbedder`: ```python from srai.embedders import CountEmbedder from
 srai.joiners import IntersectionJoiner from srai.loaders import OSMOnlineLoader
 from srai.plotting import plot_regions, plot_numeric_data from
-srai.regionalizers import H3Regionalizer from srai.utils import
-geocode_to_region_gdf loader = OSMOnlineLoader() regionalizer = H3Regionalizer
-(resolution=9) joiner = IntersectionJoiner() query = {"amenity":
-"bicycle_parking"} area = geocode_to_region_gdf("MalmÃ¶, Sweden") features =
-loader.load(area, query) regions = regionalizer.transform(area) joint =
-joiner.transform(regions, features) embedder = CountEmbedder() embeddings =
-embedder.transform(regions, features, joint) folium_map = plot_regions(area,
-colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB positron") plot_numeric_data
-(regions, embeddings, "amenity_bicycle_parking", map=folium_map) ```
+srai.regionalizers import H3Regionalizer, geocode_to_region_gdf loader =
+OSMOnlineLoader() regionalizer = H3Regionalizer(resolution=9) joiner =
+IntersectionJoiner() query = {"amenity": "bicycle_parking"} area =
+geocode_to_region_gdf("MalmÃ¶, Sweden") features = loader.load(area, query)
+regions = regionalizer.transform(area) joint = joiner.transform(regions,
+features) embedder = CountEmbedder() embeddings = embedder.transform(regions,
+features, joint) folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"],
+tiles_style="CartoDB positron") plot_numeric_data(regions, embeddings,
+"amenity_bicycle_parking", map=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                          embedding_count_embedder.jpg]
 `CountEmbedder` is a simple method, which does not require fitting. Other
 methods, such as `Hex2VecEmbedder` or `GTFS2VecEmbedder` require fitting and
 can be used in a similar way to `scikit-learn` estimators: ```python from
 srai.embedders import Hex2VecEmbedder from srai.joiners import
 IntersectionJoiner from srai.loaders import OSMPbfLoader from
 srai.loaders.osm_loaders.filters import HEX2VEC_FILTER from
 srai.neighbourhoods.h3_neighbourhood import H3Neighbourhood from
-srai.regionalizers import H3Regionalizer from srai.utils import
-geocode_to_region_gdf from srai.plotting import plot_regions, plot_numeric_data
-loader = OSMPbfLoader() regionalizer = H3Regionalizer(resolution=11) joiner =
-IntersectionJoiner() area = geocode_to_region_gdf("City of London") features =
-loader.load(area, HEX2VEC_FILTER) regions = regionalizer.transform(area) joint
-= joiner.transform(regions, features) embedder = Hex2VecEmbedder()
-neighbourhood = H3Neighbourhood(regions_gdf=regions) embedder = Hex2VecEmbedder
-([15, 10, 3]) # Option 1: fit and transform # embedder.fit(regions, features,
-joint, neighbourhood, batch_size=128) # embeddings = embedder.transform
-(regions, features, joint) # Option 2: fit_transform embeddings =
-embedder.fit_transform(regions, features, joint, neighbourhood, batch_size=128)
-folium_map = plot_regions(area, colormap=["rgba(0,0,0,0.1)"],
-tiles_style="CartoDB positron") plot_numeric_data(regions, embeddings, 0,
-map=folium_map) ```
+srai.regionalizers import H3Regionalizer, geocode_to_region_gdf from
+srai.plotting import plot_regions, plot_numeric_data loader = OSMPbfLoader()
+regionalizer = H3Regionalizer(resolution=11) joiner = IntersectionJoiner() area
+= geocode_to_region_gdf("City of London") features = loader.load(area,
+HEX2VEC_FILTER) regions = regionalizer.transform(area) joint = joiner.transform
+(regions, features) embedder = Hex2VecEmbedder() neighbourhood =
+H3Neighbourhood(regions_gdf=regions) embedder = Hex2VecEmbedder([15, 10, 3]) #
+Option 1: fit and transform # embedder.fit(regions, features, joint,
+neighbourhood, batch_size=128) # embeddings = embedder.transform(regions,
+features, joint) # Option 2: fit_transform embeddings = embedder.fit_transform
+(regions, features, joint, neighbourhood, batch_size=128) folium_map =
+plot_regions(area, colormap=["rgba(0,0,0,0.1)"], tiles_style="CartoDB
+positron") plot_numeric_data(regions, embeddings, 0, map=folium_map) ```
    [https://raw.githubusercontent.com/srai-lab/srai/main/docs/assets/images/
                         embedding_hex2vec_embedder.jpg]
 ### Pre-trained models usage We provide pre-trained models for some of the
 embedding methods. To use them, simply download them from [here](https://
 drive.google.com/drive/folders/14sH33-
 kNxA0q1O1abPWTpuix8raR_XbD?usp=drive_link) and load them using `load` method:
 ```python from srai.embedders import Hex2VecEmbedder model_path = "path/to/
```

