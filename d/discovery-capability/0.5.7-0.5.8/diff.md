# Comparing `tmp/discovery-capability-0.5.7.tar.gz` & `tmp/discovery-capability-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-capability-0.5.7.tar", last modified: Mon Aug  7 16:58:28 2023, max compression
+gzip compressed data, was "discovery-capability-0.5.8.tar", last modified: Mon Aug  7 22:01:46 2023, max compression
```

## Comparing `discovery-capability-0.5.7.tar` & `discovery-capability-0.5.8.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 16:58:28.114265 discovery-capability-0.5.7/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.5.7/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.5.7/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-07 16:58:28.114505 discovery-capability-0.5.7/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.5.7/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 16:58:27.977900 discovery-capability-0.5.7/discovery_capability.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-07 16:58:27.000000 discovery-capability-0.5.7/discovery_capability.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     2353 2023-08-07 16:58:27.000000 discovery-capability-0.5.7/discovery_capability.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-07 16:58:27.000000 discovery-capability-0.5.7/discovery_capability.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       96 2023-08-07 16:58:27.000000 discovery-capability-0.5.7/discovery_capability.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-08-07 16:58:27.000000 discovery-capability-0.5.7/discovery_capability.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 16:58:27.978307 discovery-capability-0.5.7/ds_capability/
--rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-08-02 15:31:15.000000 discovery-capability-0.5.7/ds_capability/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 16:58:27.981653 discovery-capability-0.5.7/ds_capability/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.5.7/ds_capability/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13783 2023-08-02 15:29:26.000000 discovery-capability-0.5.7/ds_capability/components/abstract_common_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3007 2023-07-27 15:44:19.000000 discovery-capability-0.5.7/ds_capability/components/commons.py
--rw-r--r--   0 doatridge   (503) staff       (20)    20334 2023-08-02 15:29:16.000000 discovery-capability-0.5.7/ds_capability/components/discovery.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7011 2023-08-02 16:48:38.000000 discovery-capability-0.5.7/ds_capability/components/feature_build.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 16:58:27.982039 discovery-capability-0.5.7/ds_capability/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.5.7/ds_capability/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 16:58:27.986068 discovery-capability-0.5.7/ds_capability/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.5.7/ds_capability/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.5.7/ds_capability/intent/abstract_feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.5.7/ds_capability/intent/common_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15964 2023-08-07 16:56:02.000000 discovery-capability-0.5.7/ds_capability/intent/feature_build_correlate_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    68101 2023-07-28 18:34:45.000000 discovery-capability-0.5.7/ds_capability/intent/feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    19736 2023-08-01 23:29:28.000000 discovery-capability-0.5.7/ds_capability/intent/feature_build_model_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 16:58:27.988867 discovery-capability-0.5.7/ds_capability/managers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.5.7/ds_capability/managers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.5.7/ds_capability/managers/controller_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.5.7/ds_capability/managers/feature_build_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.5.7/ds_capability/managers/feature_select_property_manager.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 16:58:28.106886 discovery-capability-0.5.7/ds_capability/sample/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/lookup_complaints.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/lookup_professions.py
--rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/lookup_uk_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/lookup_uk_postcode_district.py
--rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/lookup_us_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/lookup_us_street_names.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/lookup_us_street_suffix.py
--rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/map_companies_fortune1000.py
--rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/map_companies_inc5000.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/map_uk_postcodes_primary.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/map_us_age_salary.py
--rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/map_us_city_area_code.csv
--rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/map_us_city_zipcodes_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/map_us_forename_mf.py
--rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/map_us_forename_unisex.py
--rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/map_us_full_address.py
--rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/map_us_healthcare_organisations.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/map_us_phone_code.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/map_us_profession_detail_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.5.7/ds_capability/sample/map_us_surname_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.5.7/ds_capability/sample/sample_data.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-08-07 16:58:28.115184 discovery-capability-0.5.7/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2271 2023-08-04 20:17:35.000000 discovery-capability-0.5.7/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 16:58:28.107916 discovery-capability-0.5.7/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.5.7/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 16:58:28.109204 discovery-capability-0.5.7/test/component/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.5.7/test/component/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3127 2023-08-01 15:50:17.000000 discovery-capability-0.5.7/test/component/discovery_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.5.7/test/component/synthetic_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 16:58:28.109846 discovery-capability-0.5.7/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.5.7/test/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 16:58:28.113590 discovery-capability-0.5.7/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.5.7/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.5.7/test/intent/fb_analysis_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     4060 2023-08-07 15:57:41.000000 discovery-capability-0.5.7/test/intent/fb_correlate_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.5.7/test/intent/fb_diff_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-29 21:30:04.000000 discovery-capability-0.5.7/test/intent/fb_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.5.7/test/intent/fb_model_intent_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 22:01:46.871146 discovery-capability-0.5.8/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.5.8/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.5.8/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-07 22:01:46.871365 discovery-capability-0.5.8/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.5.8/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 22:01:46.706641 discovery-capability-0.5.8/discovery_capability.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-08-07 22:01:46.000000 discovery-capability-0.5.8/discovery_capability.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     2353 2023-08-07 22:01:46.000000 discovery-capability-0.5.8/discovery_capability.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-07 22:01:46.000000 discovery-capability-0.5.8/discovery_capability.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       96 2023-08-07 22:01:46.000000 discovery-capability-0.5.8/discovery_capability.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-08-07 22:01:46.000000 discovery-capability-0.5.8/discovery_capability.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 22:01:46.707473 discovery-capability-0.5.8/ds_capability/
+-rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-08-07 16:59:33.000000 discovery-capability-0.5.8/ds_capability/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 22:01:46.713105 discovery-capability-0.5.8/ds_capability/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.5.8/ds_capability/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    13783 2023-08-02 15:29:26.000000 discovery-capability-0.5.8/ds_capability/components/abstract_common_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3007 2023-07-27 15:44:19.000000 discovery-capability-0.5.8/ds_capability/components/commons.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    20334 2023-08-02 15:29:16.000000 discovery-capability-0.5.8/ds_capability/components/discovery.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7011 2023-08-02 16:48:38.000000 discovery-capability-0.5.8/ds_capability/components/feature_build.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 22:01:46.714103 discovery-capability-0.5.8/ds_capability/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.5.8/ds_capability/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 22:01:46.719378 discovery-capability-0.5.8/ds_capability/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.5.8/ds_capability/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.5.8/ds_capability/intent/abstract_feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.5.8/ds_capability/intent/common_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    16562 2023-08-07 22:00:19.000000 discovery-capability-0.5.8/ds_capability/intent/feature_build_correlate_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    68101 2023-07-28 18:34:45.000000 discovery-capability-0.5.8/ds_capability/intent/feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    19736 2023-08-01 23:29:28.000000 discovery-capability-0.5.8/ds_capability/intent/feature_build_model_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 22:01:46.722713 discovery-capability-0.5.8/ds_capability/managers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.5.8/ds_capability/managers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.5.8/ds_capability/managers/controller_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.5.8/ds_capability/managers/feature_build_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.5.8/ds_capability/managers/feature_select_property_manager.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 22:01:46.863261 discovery-capability-0.5.8/ds_capability/sample/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/lookup_complaints.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/lookup_professions.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/lookup_uk_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/lookup_uk_postcode_district.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/lookup_us_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/lookup_us_street_names.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/lookup_us_street_suffix.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/map_companies_fortune1000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/map_companies_inc5000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/map_uk_postcodes_primary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/map_us_age_salary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/map_us_city_area_code.csv
+-rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/map_us_city_zipcodes_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/map_us_forename_mf.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/map_us_forename_unisex.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/map_us_full_address.py
+-rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/map_us_healthcare_organisations.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/map_us_phone_code.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/map_us_profession_detail_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.5.8/ds_capability/sample/map_us_surname_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.5.8/ds_capability/sample/sample_data.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-08-07 22:01:46.872221 discovery-capability-0.5.8/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2271 2023-08-04 20:17:35.000000 discovery-capability-0.5.8/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 22:01:46.864252 discovery-capability-0.5.8/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.5.8/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 22:01:46.866157 discovery-capability-0.5.8/test/component/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.5.8/test/component/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3127 2023-08-01 15:50:17.000000 discovery-capability-0.5.8/test/component/discovery_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.5.8/test/component/synthetic_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 22:01:46.866842 discovery-capability-0.5.8/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.5.8/test/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-07 22:01:46.870243 discovery-capability-0.5.8/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.5.8/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.5.8/test/intent/fb_analysis_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5032 2023-08-07 21:53:05.000000 discovery-capability-0.5.8/test/intent/fb_correlate_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.5.8/test/intent/fb_diff_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-29 21:30:04.000000 discovery-capability-0.5.8/test/intent/fb_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.5.8/test/intent/fb_model_intent_test.py
```

### Comparing `discovery-capability-0.5.7/LICENSE.txt` & `discovery-capability-0.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/PKG-INFO` & `discovery-capability-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.5.7
+Version: 0.5.8
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.5.7/README.rst` & `discovery-capability-0.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/discovery_capability.egg-info/PKG-INFO` & `discovery-capability-0.5.8/discovery_capability.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.5.7
+Version: 0.5.8
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.5.7/discovery_capability.egg-info/SOURCES.txt` & `discovery-capability-0.5.8/discovery_capability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/components/abstract_common_component.py` & `discovery-capability-0.5.8/ds_capability/components/abstract_common_component.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/components/commons.py` & `discovery-capability-0.5.8/ds_capability/components/commons.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/components/discovery.py` & `discovery-capability-0.5.8/ds_capability/components/discovery.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/components/feature_build.py` & `discovery-capability-0.5.8/ds_capability/components/feature_build.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/intent/abstract_feature_build_intent.py` & `discovery-capability-0.5.8/ds_capability/intent/abstract_feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/intent/common_intent.py` & `discovery-capability-0.5.8/ds_capability/intent/common_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/intent/feature_build_correlate_intent.py` & `discovery-capability-0.5.8/ds_capability/intent/feature_build_correlate_intent.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,17 +173,17 @@
         rtn_arr = DataDiscovery.to_discrete_intervals(array=canonical.column(header), granularity=granularity,
                                                       lower=lower, upper=upper, categories=categories,
                                                       precision=precision)
         column_name = column_name if isinstance(column_name, str) else next(self.label_gen)
         return pa.table([rtn_arr.dictionary_encode()], names=[column_name])
 
     def correlate_on_condition(self, canonical: pa.Table, header: str, other: str, condition: list,
-                               values: [int, float, str, pa.Array], seed: int=None, save_intent: bool=None,
-                               intent_order: int=None, column_name: [int, str]=None, replace_intent: bool=None,
-                               remove_duplicates: bool=None) -> pa.Table:
+                               value: [int, float, bool, str], default: [int, float, bool, str]=None, seed: int=None,
+                               save_intent: bool=None, intent_order: int=None, column_name: [int, str]=None,
+                               replace_intent: bool=None, remove_duplicates: bool=None) -> pa.Table:
         """ correlates a named header to other header where the condition is met and replaces the header column
         value with a constant or value at the same index of an array. The condition is a list of triple tuples in
         the form: [(comparison, operation, logic)] where comparison is the thing to look for, the operation, what
         to do with it and the logic if you are chaining tuples, the logic to join them. An example might be:
 
                 [(1, 'greater', 'or'), (-1, 'less', None)]
                 [(pa.array(['INACTIVE', 'PENDING']), 'is_in', None)]
@@ -193,15 +193,16 @@
                 operator => 'extract_regex','equal','greater','less','greater_equal','less_equal','not_equal','is_in'
                 logic => 'and','or','xor','and_not'
 
         :param canonical: a pa.Table as the reference table
         :param header: the header for the target values to change
         :param other: the other header to correlate
         :param condition: a tuple or tuples of
-        :param values: the value or array of values
+        :param value: a constant value. If the value is a string starting @ then a header values are taken
+        :param default: (optional) a default constant if not value. A string starting @ then a default name is taken
         :param seed: (optional) the random seed. defaults to current datetime
         :param save_intent: (optional) if the intent contract should be saved to the property manager
         :param column_name: (optional) the column name that groups intent to create a column
         :param intent_order: (optional) the order in which each intent should run.
                     - If None: default's to -1
                     - if -1: added to a level above any current instance of the intent section, level 0 if not found
                     - if int: added to the level specified, overwriting any that already exist
@@ -237,13 +238,21 @@
                 logic = 'and_'
             if logic in ['and', 'or']:
                 logic = logic + '_'
             if logic not in ['xor', 'and_not', 'and_', 'or_']:
                 raise ValueError(f"The logic '{logic}' is not implemented")
             cond_list.append((c_bool, logic))
         # remove column
-        canonical = canonical.drop_columns(header)
+        if column_name == header:
+            canonical = canonical.drop_columns(header)
         final_cond = cond_list[0][0]
         for idx in range(len(cond_list) - 1):
             final_cond = eval(f"pc.{cond_list[idx][1]}(final_cond, cond_list[idx+1][0])", globals(), locals())
-        # replace and add it back to the original table
-        return Commons.table_append(canonical, pa.table([pc.if_else(final_cond, values, h_tbl)], names=[header]))
+        # check the value
+        if isinstance(value, str) and value.startswith('@'):
+            value = canonical.column(value[1:]).combine_chunks()
+        if isinstance(default, str) and default.startswith('@'):
+            default = canonical.column(default[1:]).combine_chunks()
+        elif default is None:
+            default = h_tbl
+            # replace and add it back to the original table
+        return Commons.table_append(canonical, pa.table([pc.if_else(final_cond, value, default)], names=[column_name]))
```

### Comparing `discovery-capability-0.5.7/ds_capability/intent/feature_build_intent.py` & `discovery-capability-0.5.8/ds_capability/intent/feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/intent/feature_build_model_intent.py` & `discovery-capability-0.5.8/ds_capability/intent/feature_build_model_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/managers/controller_property_manager.py` & `discovery-capability-0.5.8/ds_capability/managers/controller_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/managers/feature_build_property_manager.py` & `discovery-capability-0.5.8/ds_capability/managers/feature_build_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/managers/feature_select_property_manager.py` & `discovery-capability-0.5.8/ds_capability/managers/feature_select_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/lookup_complaints.py` & `discovery-capability-0.5.8/ds_capability/sample/lookup_complaints.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/lookup_professions.py` & `discovery-capability-0.5.8/ds_capability/sample/lookup_professions.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/lookup_uk_city.py` & `discovery-capability-0.5.8/ds_capability/sample/lookup_uk_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/lookup_uk_postcode_district.py` & `discovery-capability-0.5.8/ds_capability/sample/lookup_uk_postcode_district.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/lookup_us_city.py` & `discovery-capability-0.5.8/ds_capability/sample/lookup_us_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/lookup_us_street_names.py` & `discovery-capability-0.5.8/ds_capability/sample/lookup_us_street_names.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/lookup_us_street_suffix.py` & `discovery-capability-0.5.8/ds_capability/sample/lookup_us_street_suffix.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/map_companies_fortune1000.py` & `discovery-capability-0.5.8/ds_capability/sample/map_companies_fortune1000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/map_companies_inc5000.py` & `discovery-capability-0.5.8/ds_capability/sample/map_companies_inc5000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/map_uk_postcodes_primary.py` & `discovery-capability-0.5.8/ds_capability/sample/map_uk_postcodes_primary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/map_us_age_salary.py` & `discovery-capability-0.5.8/ds_capability/sample/map_us_age_salary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/map_us_city_area_code.csv` & `discovery-capability-0.5.8/ds_capability/sample/map_us_city_area_code.csv`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/map_us_city_zipcodes_rank.py` & `discovery-capability-0.5.8/ds_capability/sample/map_us_city_zipcodes_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/map_us_forename_mf.py` & `discovery-capability-0.5.8/ds_capability/sample/map_us_forename_mf.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/map_us_forename_unisex.py` & `discovery-capability-0.5.8/ds_capability/sample/map_us_forename_unisex.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/map_us_full_address.py` & `discovery-capability-0.5.8/ds_capability/sample/map_us_full_address.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/map_us_healthcare_organisations.py` & `discovery-capability-0.5.8/ds_capability/sample/map_us_healthcare_organisations.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/map_us_phone_code.py` & `discovery-capability-0.5.8/ds_capability/sample/map_us_phone_code.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/map_us_profession_detail_rank.py` & `discovery-capability-0.5.8/ds_capability/sample/map_us_profession_detail_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/map_us_surname_rank.py` & `discovery-capability-0.5.8/ds_capability/sample/map_us_surname_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/ds_capability/sample/sample_data.py` & `discovery-capability-0.5.8/ds_capability/sample/sample_data.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/setup.py` & `discovery-capability-0.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/test/component/discovery_test.py` & `discovery-capability-0.5.8/test/component/discovery_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/test/component/synthetic_test.py` & `discovery-capability-0.5.8/test/component/synthetic_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/test/intent/fb_analysis_intent_test.py` & `discovery-capability-0.5.8/test/intent/fb_analysis_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/test/intent/fb_correlate_intent_test.py` & `discovery-capability-0.5.8/test/intent/fb_correlate_intent_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -79,20 +79,30 @@
         fb = FeatureBuild.from_memory()
         tools: FeatureBuildIntentModel = fb.tools
         tbl = tools.get_synthetic_data_types(10, seed=101)
         # check no zeros
         self.assertEqual(0, pc.count(pc.index_in(tbl.column('int').combine_chunks(), pa.array([0])).drop_null()).as_py())
         # check three zeros
         result = tools.correlate_on_condition(tbl, header='int', other='num',
-                                              condition=[(1, 'greater', 'or'), (-1, 'less', None)], values=0)
+                                              condition=[(1, 'greater', 'or'), (-1, 'less', None)], value=0, column_name='int')
         self.assertEqual(3, pc.count(pc.index_in(result.column('int').combine_chunks(), pa.array([0])).drop_null()).as_py())
         # check string
         result = tools.correlate_on_condition(tbl, header='cat', other='cat',
-                                              condition=[(pa.array(['INACTIVE', "SUSPENDED"]), 'is_in', None)], values='N/A')
-        print(result.column('cat').combine_chunks())
+                                              condition=[(pa.array(['INACTIVE', "SUSPENDED"]), 'is_in', None)], value='N/A', column_name='target')
+        self.assertEqual(4, pc.count(pc.index_in(result.column('target').combine_chunks(), pa.array(['N/A'])).drop_null()).as_py())
+        # check headers
+        result = tools.correlate_on_condition(tbl, header='int', other='num',
+                                              condition=[(1, 'greater', 'or'), (-1, 'less', None)],
+                                              value=0, default=1, column_name='target')
+        self.assertEqual(7, pc.sum(result.column('target')).as_py())
+        result = tools.correlate_on_condition(tbl, header='int', other='num',
+                                              condition=[(1, 'greater', 'or'), (-1, 'less', None)],
+                                              value=0, default="@num", column_name='target')
+        self.assertEqual(result.column('target').slice(2, 4), result.column('num').slice(2, 4))
+        self.assertEqual(3, pc.count(pc.index_in(result.column('target').combine_chunks(), pa.array([0])).drop_null()).as_py())
 
     def test_raise(self):
         with self.assertRaises(KeyError) as context:
             env = os.environ['NoEnvValueTest']
         self.assertTrue("'NoEnvValueTest'" in str(context.exception))
```

### Comparing `discovery-capability-0.5.7/test/intent/fb_diff_intent_test.py` & `discovery-capability-0.5.8/test/intent/fb_diff_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/test/intent/fb_intent_test.py` & `discovery-capability-0.5.8/test/intent/fb_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.7/test/intent/fb_model_intent_test.py` & `discovery-capability-0.5.8/test/intent/fb_model_intent_test.py`

 * *Files identical despite different names*

