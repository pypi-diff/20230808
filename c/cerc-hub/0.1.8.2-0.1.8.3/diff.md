# Comparing `tmp/cerc-hub-0.1.8.2.tar.gz` & `tmp/cerc-hub-0.1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerc-hub-0.1.8.2.tar", last modified: Thu Aug  3 16:24:52 2023, max compression
+gzip compressed data, was "cerc-hub-0.1.8.3.tar", last modified: Tue Aug  8 16:52:46 2023, max compression
```

## Comparing `cerc-hub-0.1.8.2.tar` & `cerc-hub-0.1.8.3.tar`

### file list

```diff
@@ -1,377 +1,344 @@
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.036953 cerc-hub-0.1.8.2/
--rw-r--r--   0 jenkins    (109) jenkins    (117)      828 2023-08-03 16:24:52.036953 cerc-hub-0.1.8.2/PKG-INFO
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.004953 cerc-hub-0.1.8.2/cerc_hub.egg-info/
--rw-r--r--   0 jenkins    (109) jenkins    (117)       32 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/cerc_hub.egg-info/.gitignore
--rw-r--r--   0 jenkins    (109) jenkins    (117)      828 2023-08-03 16:24:51.000000 cerc-hub-0.1.8.2/cerc_hub.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (117)    14403 2023-08-03 16:24:51.000000 cerc-hub-0.1.8.2/cerc_hub.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)        1 2023-08-03 16:24:51.000000 cerc-hub-0.1.8.2/cerc_hub.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)      263 2023-08-03 16:24:51.000000 cerc-hub-0.1.8.2/cerc_hub.egg-info/requires.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)        4 2023-08-03 16:24:51.000000 cerc-hub-0.1.8.2/cerc_hub.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.004953 cerc-hub-0.1.8.2/hub/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.004953 cerc-hub-0.1.8.2/hub/catalog_factories/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      870 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/catalog.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.004953 cerc-hub-0.1.8.2/hub/catalog_factories/construction/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/construction/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1701 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/construction/construction_helper.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10136 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/construction/eilat_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10217 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/construction/nrcan_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10304 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/construction/nrel_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1507 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/construction_catalog_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.004953 cerc-hub-0.1.8.2/hub/catalog_factories/cost/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/cost/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     8566 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/cost/montreal_custom_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1044 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/costs_catalog_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.004953 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.004953 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/construction/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/construction/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4634 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/construction/archetype.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2057 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/construction/construction.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1370 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/construction/content.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1298 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/construction/layer.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3187 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/construction/material.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1728 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/construction/window.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.004953 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3180 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/archetype.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1801 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/capital_cost.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1320 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/chapter.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      951 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/content.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1938 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/fuel.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2185 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/income.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2612 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/item_description.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2132 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/operational_cost.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.004953 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/energy_systems/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/energy_systems/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1269 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/energy_systems/archetype.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1624 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/energy_systems/content.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2701 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/energy_systems/distribution_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1389 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/energy_systems/emission_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3804 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/energy_systems/generation_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2942 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/energy_systems/system.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.004953 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/greenery/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/greenery/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1164 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/greenery/content.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2912 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/greenery/plant.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1494 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/greenery/plant_percentage.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3584 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/greenery/soil.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5825 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/greenery/vegetation.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.008953 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2071 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/appliances.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      873 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/content.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1879 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/domestic_hot_water.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2053 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/lighting.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2547 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/occupancy.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2225 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/schedule.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3578 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/thermal_control.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4088 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/usage.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.008953 cerc-hub-0.1.8.2/hub/catalog_factories/energy_systems/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/energy_systems/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    11133 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/energy_systems/montreal_custom_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1201 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/energy_systems_catalog_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.008953 cerc-hub-0.1.8.2/hub/catalog_factories/greenery/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/greenery/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.008953 cerc-hub-0.1.8.2/hub/catalog_factories/greenery/ecore_greenery/
--rw-r--r--   0 jenkins    (109) jenkins    (117)    19314 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.ecore
--rw-r--r--   0 jenkins    (109) jenkins    (117)    12388 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    18684 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog_no_quantities.ecore
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4564 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/greenery/greenery_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1107 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/greenery_catalog_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.008953 cerc-hub-0.1.8.2/hub/catalog_factories/usage/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/usage/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10095 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/usage/comnet_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10017 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/usage/eilat_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10380 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/usage/nrcan_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4425 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/usage/usage_helper.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1516 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/catalog_factories/usage_catalog_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.008953 cerc-hub-0.1.8.2/hub/city_model_structure/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.008953 cerc-hub-0.1.8.2/hub/city_model_structure/attributes/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/attributes/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      935 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/attributes/edge.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1194 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/attributes/node.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1929 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/attributes/plane.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      843 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/attributes/point.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    13218 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/attributes/polygon.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     6590 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/attributes/polyhedron.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      763 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/attributes/record.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2922 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/attributes/schedule.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      770 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/attributes/time_series.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    26423 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.012953 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2359 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/appliances.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2052 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/domestic_hot_water.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      650 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/household.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3009 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/internal_gain.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2895 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/internal_zone.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1259 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/layer.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2349 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/lighting.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4070 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/material.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2865 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/occupancy.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3090 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/storey.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    11228 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/surface.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     9018 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/thermal_boundary.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4622 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/thermal_control.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5277 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/thermal_opening.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    24514 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/thermal_zone.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     7848 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/usage.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      957 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/buildings_cluster.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1385 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/bus_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    16886 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/city.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     8101 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/city_object.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1638 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/city_objects_cluster.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1613 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/energy_system.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.012953 cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3237 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/air_source_hp.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      570 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/control_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      918 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/distribution_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      841 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/emission_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3526 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/energy_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2693 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/generation_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2665 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/generic_distribution_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      775 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/generic_emission_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2577 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/generic_energy_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3996 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/generic_generation_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1508 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/heat_pump.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1115 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/hvac_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      709 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/hvac_terminal_unit.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3093 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/water_to_water_hp.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.012953 cerc-hub-0.1.8.2/hub/city_model_structure/greenery/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/greenery/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2304 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/greenery/plant.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3288 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/greenery/soil.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1630 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/greenery/vegetation.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.012953 cerc-hub-0.1.8.2/hub/city_model_structure/iot/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/iot/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1503 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/iot/sensor.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      867 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/iot/sensor_measure.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      462 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/iot/sensor_type.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      943 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/iot/station.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2502 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/level_of_detail.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1195 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/network.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      974 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/parts_consisting_building.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.016953 cerc-hub-0.1.8.2/hub/city_model_structure/transport/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2403 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/bus.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      880 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/bus_depot.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1045 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/bus_edge.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      970 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/bus_network.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1154 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/bus_node.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1494 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/bus_stop.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2616 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/connection.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1775 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/crossing.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      821 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/join.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3285 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/lane.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1251 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/origin_destination_edge.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1141 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/origin_destination_network.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2159 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/origin_destination_node.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3173 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/phase.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3542 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/traffic_edge.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1877 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/traffic_light.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1080 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/traffic_network.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2186 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/traffic_node.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      965 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/city_model_structure/transport/walkway_node.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.016953 cerc-hub-0.1.8.2/hub/config/
--rw-r--r--   0 jenkins    (109) jenkins    (117)      629 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/config/configuration.ini
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.000954 cerc-hub-0.1.8.2/hub/data/
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.016953 cerc-hub-0.1.8.2/hub/data/construction/
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3280 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/construction/eilat_archetypes.json
--rw-r--r--   0 jenkins    (109) jenkins    (117)    73899 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/construction/eilat_constructions.json
--rw-r--r--   0 jenkins    (109) jenkins    (117)  1894214 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/construction/nrcan_archetypes.json
--rw-r--r--   0 jenkins    (109) jenkins    (117)   274471 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/construction/nrcan_constructions.json
--rw-r--r--   0 jenkins    (109) jenkins    (117)    44638 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/construction/us_archetypes.xml
--rw-r--r--   0 jenkins    (109) jenkins    (117)    32891 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/construction/us_constructions.xml
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.016953 cerc-hub-0.1.8.2/hub/data/costs/
--rw-r--r--   0 jenkins    (109) jenkins    (117)    11017 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/costs/montreal_costs.xml
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.016953 cerc-hub-0.1.8.2/hub/data/customized_imports/
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3228 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/customized_imports/ashrae_archetypes.xml
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.016953 cerc-hub-0.1.8.2/hub/data/energy_systems/
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.016953 cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/
--rw-r--r--   0 jenkins    (109) jenkins    (117)   105875 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/air_source.xlsx
--rw-r--r--   0 jenkins    (109) jenkins    (117)    11051 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/as_parallel.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10802 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/as_series.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)      446 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/constants.yaml
--rw-r--r--   0 jenkins    (109) jenkins    (117)  1040664 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/demand.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10820 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/w2w_parallel.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10411 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/w2w_series.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)    73906 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/water_to_water.xlsx
--rw-r--r--   0 jenkins    (109) jenkins    (117)   257760 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/wt_hourly3.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)    18850 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/energy_systems/montreal_custom_systems.xml
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.020953 cerc-hub-0.1.8.2/hub/data/geolocation/
--rw-r--r--   0 jenkins    (109) jenkins    (117)  2219196 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/geolocation/admin2Codes.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)  6284352 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/geolocation/cities15000.txt
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.024953 cerc-hub-0.1.8.2/hub/data/greenery/
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5044 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/greenery/ecore_greenery_catalog.xml
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.024953 cerc-hub-0.1.8.2/hub/data/usage/
--rw-r--r--   0 jenkins    (109) jenkins    (117)   299386 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/usage/comnet_archetypes.xlsx
--rw-r--r--   0 jenkins    (109) jenkins    (117)   348793 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/usage/comnet_schedules_archetypes.xlsx
--rw-r--r--   0 jenkins    (109) jenkins    (117)    15170 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/usage/eilat_archetypes.xlsx
--rw-r--r--   0 jenkins    (109) jenkins    (117)    78312 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/usage/eilat_schedules_archetypes.xlsx
--rw-r--r--   0 jenkins    (109) jenkins    (117)      398 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/usage/nrcan.xml
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.000954 cerc-hub-0.1.8.2/hub/data/weather/
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.024953 cerc-hub-0.1.8.2/hub/data/weather/epw/
--rw-r--r--   0 jenkins    (109) jenkins    (117)  1588401 2023-08-03 16:23:25.000000 cerc-hub-0.1.8.2/hub/data/weather/epw/CAN_PQ_Montreal.Intl.AP.716270_CWEC.epw
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.024953 cerc-hub-0.1.8.2/hub/exports/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.024953 cerc-hub-0.1.8.2/hub/exports/building_energy/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/building_energy/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    17060 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/building_energy/energy_ade.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    35617 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/building_energy/idf.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.028953 cerc-hub-0.1.8.2/hub/exports/building_energy/idf_files/
--rw-r--r--   0 jenkins    (109) jenkins    (117)  4241609 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/building_energy/idf_files/Energy+.idd
--rw-r--r--   0 jenkins    (109) jenkins    (117)     7428 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/building_energy/idf_files/Minimal.idf
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.028953 cerc-hub-0.1.8.2/hub/exports/building_energy/insel/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/building_energy/insel/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    13413 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/building_energy/insel/insel_monthly_energy_balance.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2814 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/energy_building_exports_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.028953 cerc-hub-0.1.8.2/hub/exports/energy_systems/
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2379 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/energy_systems/air_source_hp_export.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    12750 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/energy_systems/heat_pump_export.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2228 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/energy_systems/water_to_water_hp_export.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2238 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/energy_systems_factory.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1918 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/exports_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.028953 cerc-hub-0.1.8.2/hub/exports/formats/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/formats/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1737 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/formats/obj.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4828 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/formats/simplified_radiosity_algorithm.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      398 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/formats/stl.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1069 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/exports/formats/triangular.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.028953 cerc-hub-0.1.8.2/hub/helpers/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      766 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/auth.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4765 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/configuration_helper.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     6128 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/constants.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.032953 cerc-hub-0.1.8.2/hub/helpers/data/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     9183 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/alkis_function_to_hub_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      694 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/eilat_function_to_hub_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1039 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/hft_function_to_hub_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      710 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/hub_function_to_eilat_construction_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3266 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/hub_function_to_montreal_custom_costs_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2980 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/hub_function_to_nrcan_construction_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3006 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/hub_function_to_nrel_construction_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3213 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/hub_usage_to_comnet_usage.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      630 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/hub_usage_to_eilat_usage.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3178 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/hub_usage_to_hft_usage.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3228 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/hub_usage_to_nrcan_usage.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      635 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/montreal_custom_fuel_to_hub_fuel.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      813 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/montreal_demand_type_to_hub_energy_demand_type.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    31279 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/montreal_function_to_hub_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2155 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/montreal_system_to_hub_energy_generation_system.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     6408 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/data/pluto_function_to_hub_function.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5351 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/dictionaries.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    12422 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/geometry_helper.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      729 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/location.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1632 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/monthly_values.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.032953 cerc-hub-0.1.8.2/hub/helpers/peak_calculation/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/peak_calculation/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     6723 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/peak_calculation/loads_calculation.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4985 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/peak_loads.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      883 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/helpers/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.032953 cerc-hub-0.1.8.2/hub/imports/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.032953 cerc-hub-0.1.8.2/hub/imports/construction/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/construction/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    11083 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/construction/eilat_physics_parameters.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.032953 cerc-hub-0.1.8.2/hub/imports/construction/helpers/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/construction/helpers/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2425 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/construction/helpers/construction_helper.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     7447 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/construction/helpers/storeys_generation.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10727 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/construction/nrcan_physics_parameters.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     9906 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/construction/nrel_physics_parameters.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1916 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/construction_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.032953 cerc-hub-0.1.8.2/hub/imports/energy_systems/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/energy_systems/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5582 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/energy_systems/air_source_hp_parameters.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.032953 cerc-hub-0.1.8.2/hub/imports/energy_systems/helpers/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/energy_systems/helpers/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      679 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/energy_systems/helpers/energy_systems_helper.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     7609 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/energy_systems/montreal_custom_energy_system_parameters.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     6552 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/energy_systems/water_to_water_hp_parameters.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2217 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/energy_systems_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.032953 cerc-hub-0.1.8.2/hub/imports/geometry/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/geometry/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     7933 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/geometry/citygml.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.032953 cerc-hub-0.1.8.2/hub/imports/geometry/citygml_classes/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/geometry/citygml_classes/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      792 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/geometry/citygml_classes/citygml_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2358 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/geometry/citygml_classes/citygml_lod1.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3409 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/geometry/citygml_classes/citygml_lod2.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    14539 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/geometry/geojson.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3944 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/geometry/gpandas.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.032953 cerc-hub-0.1.8.2/hub/imports/geometry/helpers/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/geometry/helpers/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3258 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/geometry/helpers/geometry_helper.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2936 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/geometry/obj.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2676 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/geometry_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.036953 cerc-hub-0.1.8.2/hub/imports/results/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/results/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1432 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/results/insel_heatpump_energy_demand.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5454 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/results/insel_monthly_energry_balance.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3874 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/results/simplified_radiosity_algorithm.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2129 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/results_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.036953 cerc-hub-0.1.8.2/hub/imports/usage/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/usage/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10941 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/usage/comnet_usage_parameters.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    10929 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/usage/eilat_usage_parameters.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     9313 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/usage/nrcan_usage_parameters.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1894 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/usage_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.036953 cerc-hub-0.1.8.2/hub/imports/weather/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/weather/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     9545 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/weather/epw_weather_parameters.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.036953 cerc-hub-0.1.8.2/hub/imports/weather/helpers/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/weather/helpers/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5749 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/weather/helpers/weather.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1204 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/imports/weather_factory.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.036953 cerc-hub-0.1.8.2/hub/persistence/
--rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1941 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/configuration.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     9486 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/db_control.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2942 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/db_setup.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.036953 cerc-hub-0.1.8.2/hub/persistence/models/
--rw-r--r--   0 jenkins    (109) jenkins    (117)      203 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/models/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1039 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/models/application.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1235 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/models/city.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2811 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/models/city_object.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1177 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/models/simulation_results.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1129 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/models/user.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.036953 cerc-hub-0.1.8.2/hub/persistence/repositories/
--rw-r--r--   0 jenkins    (109) jenkins    (117)       29 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/repositories/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3574 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/repositories/application.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4545 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/repositories/city.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4837 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/repositories/city_object.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     6022 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/repositories/simulation_results.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5087 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/repositories/user.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      772 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/persistence/repository.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)       51 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/hub/version.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      164 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/pyproject.toml
--rw-r--r--   0 jenkins    (109) jenkins    (117)      251 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/requirements.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)       38 2023-08-03 16:24:52.036953 cerc-hub-0.1.8.2/setup.cfg
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5290 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/setup.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 16:24:52.036953 cerc-hub-0.1.8.2/tests/
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5014 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_city_merge.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2734 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_construction_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    17918 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_construction_factory.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      938 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_costs_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     7637 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_custom_insel_block.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    13088 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_db_factory.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4109 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_db_retrieve.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2684 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_energy_systems_air_source_hp.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     2497 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_energy_systems_water_to_water_hp.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     7368 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_enrichement.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4942 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_exports.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     9903 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_geometry_factory.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1339 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_greenery_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3225 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_greenery_in_idf.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3007 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_heat_pump_results.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     7571 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_insel_exports.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     4434 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_results_import.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1471 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_systems_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     5817 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_systems_factory.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      819 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_usage_catalog.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)    11500 2023-08-03 16:23:26.000000 cerc-hub-0.1.8.2/tests/test_usage_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.662922 cerc-hub-0.1.8.3/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      828 2023-08-08 16:52:46.662922 cerc-hub-0.1.8.3/PKG-INFO
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.626922 cerc-hub-0.1.8.3/cerc_hub.egg-info/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)       32 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/cerc_hub.egg-info/.gitignore
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      828 2023-08-08 16:52:46.000000 cerc-hub-0.1.8.3/cerc_hub.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    12879 2023-08-08 16:52:46.000000 cerc-hub-0.1.8.3/cerc_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        1 2023-08-08 16:52:46.000000 cerc-hub-0.1.8.3/cerc_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      263 2023-08-08 16:52:46.000000 cerc-hub-0.1.8.3/cerc_hub.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        4 2023-08-08 16:52:46.000000 cerc-hub-0.1.8.3/cerc_hub.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.630922 cerc-hub-0.1.8.3/hub/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.630922 cerc-hub-0.1.8.3/hub/catalog_factories/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      870 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/catalog.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.630922 cerc-hub-0.1.8.3/hub/catalog_factories/construction/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/construction/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1701 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/construction/construction_helper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10216 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/construction/eilat_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10333 2023-08-08 16:47:52.000000 cerc-hub-0.1.8.3/hub/catalog_factories/construction/nrcan_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10384 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/construction/nrel_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1507 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/construction_catalog_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.630922 cerc-hub-0.1.8.3/hub/catalog_factories/cost/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/cost/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     8566 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/cost/montreal_custom_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1044 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/costs_catalog_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.630922 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.630922 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/construction/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/construction/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4634 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/construction/archetype.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2057 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/construction/construction.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1370 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/construction/content.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1298 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/construction/layer.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3187 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/construction/material.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1728 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/construction/window.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.630922 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3180 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/archetype.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1801 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/capital_cost.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1320 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/chapter.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      951 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/content.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1926 2023-08-08 16:47:52.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/fuel.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2189 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/income.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2612 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/item_description.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2132 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/operational_cost.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.630922 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/energy_systems/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/energy_systems/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1269 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/energy_systems/archetype.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1624 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/energy_systems/content.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2585 2023-08-08 16:47:52.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/energy_systems/distribution_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1389 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/energy_systems/emission_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3804 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/energy_systems/generation_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2942 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/energy_systems/system.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.630922 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/greenery/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/greenery/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1164 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/greenery/content.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2912 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/greenery/plant.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1494 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/greenery/plant_percentage.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3584 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/greenery/soil.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5825 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/greenery/vegetation.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.634922 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2063 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/appliances.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      873 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/content.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1879 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/domestic_hot_water.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2053 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/lighting.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2547 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/occupancy.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2225 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/schedule.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3578 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/thermal_control.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4090 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/usage.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.634922 cerc-hub-0.1.8.3/hub/catalog_factories/energy_systems/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/energy_systems/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    11133 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/energy_systems/montreal_custom_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1201 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/energy_systems_catalog_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.634922 cerc-hub-0.1.8.3/hub/catalog_factories/greenery/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/greenery/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.634922 cerc-hub-0.1.8.3/hub/catalog_factories/greenery/ecore_greenery/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    19314 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.ecore
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    12388 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    18684 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog_no_quantities.ecore
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4564 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/greenery/greenery_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1107 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/greenery_catalog_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.634922 cerc-hub-0.1.8.3/hub/catalog_factories/usage/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/usage/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10095 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/usage/comnet_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10017 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/usage/eilat_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10409 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/usage/nrcan_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4425 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/usage/usage_helper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1516 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/catalog_factories/usage_catalog_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.634922 cerc-hub-0.1.8.3/hub/city_model_structure/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.634922 cerc-hub-0.1.8.3/hub/city_model_structure/attributes/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/attributes/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      935 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/attributes/edge.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1194 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/attributes/node.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1929 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/attributes/plane.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      843 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/attributes/point.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    13218 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/attributes/polygon.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     6590 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/attributes/polyhedron.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      763 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/attributes/record.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2922 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/attributes/schedule.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      770 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/attributes/time_series.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    26678 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.638922 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2359 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/appliances.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2677 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/construction.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2052 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/domestic_hot_water.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      650 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/household.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3009 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/internal_gain.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4090 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/internal_zone.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4439 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/layer.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2349 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/lighting.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2865 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/occupancy.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3178 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/storey.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    11190 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/surface.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3502 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/thermal_archetype.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10729 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/thermal_boundary.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4622 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/thermal_control.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5277 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/thermal_opening.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    25615 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/thermal_zone.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     7852 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/usage.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      957 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/buildings_cluster.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    16458 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/city.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     8085 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/city_object.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1638 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/city_objects_cluster.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.638922 cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      570 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/control_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      918 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/distribution_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      841 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/emission_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3526 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/energy_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2693 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/generation_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2661 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/generic_distribution_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      775 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/generic_emission_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2577 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/generic_energy_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3996 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/generic_generation_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1508 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/heat_pump.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      709 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/hvac_terminal_unit.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.638922 cerc-hub-0.1.8.3/hub/city_model_structure/greenery/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/greenery/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2304 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/greenery/plant.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3288 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/greenery/soil.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1630 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/greenery/vegetation.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.638922 cerc-hub-0.1.8.3/hub/city_model_structure/iot/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/iot/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1503 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/iot/sensor.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      867 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/iot/sensor_measure.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      462 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/iot/sensor_type.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      943 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/iot/station.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2502 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/level_of_detail.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1195 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/network.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      974 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/city_model_structure/parts_consisting_building.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.638922 cerc-hub-0.1.8.3/hub/config/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      629 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/config/configuration.ini
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.626922 cerc-hub-0.1.8.3/hub/data/
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.638922 cerc-hub-0.1.8.3/hub/data/construction/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3280 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/construction/eilat_archetypes.json
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    73899 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/construction/eilat_constructions.json
+-rw-r--r--   0 jenkins    (109) jenkins    (117)  1894214 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/construction/nrcan_archetypes.json
+-rw-r--r--   0 jenkins    (109) jenkins    (117)   274471 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/construction/nrcan_constructions.json
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    44638 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/construction/us_archetypes.xml
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    32891 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/construction/us_constructions.xml
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.638922 cerc-hub-0.1.8.3/hub/data/costs/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    11017 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/costs/montreal_costs.xml
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.638922 cerc-hub-0.1.8.3/hub/data/customized_imports/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3228 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/customized_imports/ashrae_archetypes.xml
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.642922 cerc-hub-0.1.8.3/hub/data/energy_systems/
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.642922 cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)   105875 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/air_source.xlsx
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    11051 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/as_parallel.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10802 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/as_series.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      446 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/constants.yaml
+-rw-r--r--   0 jenkins    (109) jenkins    (117)  1040664 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/demand.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10820 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/w2w_parallel.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10411 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/w2w_series.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    73906 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/water_to_water.xlsx
+-rw-r--r--   0 jenkins    (109) jenkins    (117)   257760 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/wt_hourly3.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    18850 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/energy_systems/montreal_custom_systems.xml
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.642922 cerc-hub-0.1.8.3/hub/data/geolocation/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)  2219196 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/geolocation/admin2Codes.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)  6284352 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/geolocation/cities15000.txt
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.646922 cerc-hub-0.1.8.3/hub/data/greenery/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5044 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/greenery/ecore_greenery_catalog.xml
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.646922 cerc-hub-0.1.8.3/hub/data/usage/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)   299386 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/usage/comnet_archetypes.xlsx
+-rw-r--r--   0 jenkins    (109) jenkins    (117)   348793 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/usage/comnet_schedules_archetypes.xlsx
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    15170 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/usage/eilat_archetypes.xlsx
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    78312 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/usage/eilat_schedules_archetypes.xlsx
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      398 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/usage/nrcan.xml
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.626922 cerc-hub-0.1.8.3/hub/data/weather/
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.650922 cerc-hub-0.1.8.3/hub/data/weather/epw/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)  1574165 2023-08-08 16:08:33.000000 cerc-hub-0.1.8.3/hub/data/weather/epw/CAN_BC_Summerland.717680_CWEC.epw
+-rw-r--r--   0 jenkins    (109) jenkins    (117)  1588401 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/data/weather/epw/CAN_PQ_Montreal.Intl.AP.716270_CWEC.epw
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.650922 cerc-hub-0.1.8.3/hub/exports/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.650922 cerc-hub-0.1.8.3/hub/exports/building_energy/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/building_energy/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    17080 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/building_energy/energy_ade.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    35872 2023-08-08 16:47:52.000000 cerc-hub-0.1.8.3/hub/exports/building_energy/idf.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.654922 cerc-hub-0.1.8.3/hub/exports/building_energy/idf_files/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)  4241609 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/building_energy/idf_files/Energy+.idd
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     7428 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/building_energy/idf_files/Minimal.idf
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.654922 cerc-hub-0.1.8.3/hub/exports/building_energy/insel/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/building_energy/insel/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    13259 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/building_energy/insel/insel_monthly_energy_balance.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2814 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/energy_building_exports_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.654922 cerc-hub-0.1.8.3/hub/exports/energy_systems/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2379 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/energy_systems/air_source_hp_export.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    12750 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/energy_systems/heat_pump_export.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2228 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/energy_systems/water_to_water_hp_export.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2238 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/energy_systems_factory.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1918 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/exports_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.654922 cerc-hub-0.1.8.3/hub/exports/formats/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/formats/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1737 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/formats/obj.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4897 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/formats/simplified_radiosity_algorithm.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      398 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/formats/stl.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1069 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/exports/formats/triangular.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.654922 cerc-hub-0.1.8.3/hub/helpers/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      766 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/auth.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4765 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/configuration_helper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     6598 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/constants.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.654922 cerc-hub-0.1.8.3/hub/helpers/data/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/data/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     9183 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/data/alkis_function_to_hub_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      694 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/data/eilat_function_to_hub_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1039 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/data/hft_function_to_hub_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      710 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/data/hub_function_to_eilat_construction_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3266 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/data/hub_function_to_montreal_custom_costs_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2980 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/data/hub_function_to_nrcan_construction_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3006 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/data/hub_function_to_nrel_construction_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3213 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/data/hub_usage_to_comnet_usage.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      630 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/data/hub_usage_to_eilat_usage.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3178 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/data/hub_usage_to_hft_usage.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3228 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/data/hub_usage_to_nrcan_usage.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      635 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/data/montreal_custom_fuel_to_hub_fuel.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      813 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/data/montreal_demand_type_to_hub_energy_demand_type.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    30726 2023-08-08 16:47:52.000000 cerc-hub-0.1.8.3/hub/helpers/data/montreal_function_to_hub_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2155 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/data/montreal_system_to_hub_energy_generation_system.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     6408 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/data/pluto_function_to_hub_function.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5351 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/dictionaries.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    12422 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/geometry_helper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      729 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/location.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1238 2023-08-08 16:47:52.000000 cerc-hub-0.1.8.3/hub/helpers/monthly_values.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.654922 cerc-hub-0.1.8.3/hub/helpers/peak_calculation/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/peak_calculation/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     6701 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/peak_calculation/loads_calculation.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5039 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/peak_loads.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1674 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/helpers/thermal_zones_creation.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      916 2023-08-08 16:47:52.000000 cerc-hub-0.1.8.3/hub/helpers/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.658922 cerc-hub-0.1.8.3/hub/imports/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.658922 cerc-hub-0.1.8.3/hub/imports/construction/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/construction/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5730 2023-08-08 16:47:52.000000 cerc-hub-0.1.8.3/hub/imports/construction/eilat_physics_parameters.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.658922 cerc-hub-0.1.8.3/hub/imports/construction/helpers/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/construction/helpers/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2470 2023-08-08 16:47:52.000000 cerc-hub-0.1.8.3/hub/imports/construction/helpers/construction_helper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     7447 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/construction/helpers/storeys_generation.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5371 2023-08-08 16:47:52.000000 cerc-hub-0.1.8.3/hub/imports/construction/nrcan_physics_parameters.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5644 2023-08-08 16:47:52.000000 cerc-hub-0.1.8.3/hub/imports/construction/nrel_physics_parameters.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1916 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/construction_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.658922 cerc-hub-0.1.8.3/hub/imports/energy_systems/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/energy_systems/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     7520 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/energy_systems/montreal_custom_energy_system_parameters.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1385 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/energy_systems_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.658922 cerc-hub-0.1.8.3/hub/imports/geometry/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/geometry/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     7933 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/geometry/citygml.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.658922 cerc-hub-0.1.8.3/hub/imports/geometry/citygml_classes/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/geometry/citygml_classes/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      792 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/geometry/citygml_classes/citygml_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2358 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/geometry/citygml_classes/citygml_lod1.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3409 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/geometry/citygml_classes/citygml_lod2.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    14539 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/geometry/geojson.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.658922 cerc-hub-0.1.8.3/hub/imports/geometry/helpers/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/geometry/helpers/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3259 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/geometry/helpers/geometry_helper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2936 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/geometry/obj.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2335 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/geometry_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.658922 cerc-hub-0.1.8.3/hub/imports/results/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/results/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4689 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/results/insel_monthly_energry_balance.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1828 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/results/simplified_radiosity_algorithm.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1824 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/results_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.658922 cerc-hub-0.1.8.3/hub/imports/usage/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/usage/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10879 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/usage/comnet_usage_parameters.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    10867 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/usage/eilat_usage_parameters.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     9287 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/usage/nrcan_usage_parameters.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1894 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/usage_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.658922 cerc-hub-0.1.8.3/hub/imports/weather/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/weather/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     9033 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/weather/epw_weather_parameters.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.658922 cerc-hub-0.1.8.3/hub/imports/weather/helpers/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/weather/helpers/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4250 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/weather/helpers/weather.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1179 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/imports/weather_factory.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.658922 cerc-hub-0.1.8.3/hub/persistence/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1941 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/configuration.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     9486 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/db_control.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2942 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/db_setup.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.658922 cerc-hub-0.1.8.3/hub/persistence/models/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      203 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/models/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1039 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/models/application.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1235 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/models/city.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2831 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/models/city_object.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1177 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/models/simulation_results.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1129 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/models/user.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.662922 cerc-hub-0.1.8.3/hub/persistence/repositories/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)       29 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/repositories/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3574 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/repositories/application.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4545 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/repositories/city.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4837 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/repositories/city_object.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     6022 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/repositories/simulation_results.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5087 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/repositories/user.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      772 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/persistence/repository.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)       51 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/hub/version.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      164 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/pyproject.toml
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      251 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/requirements.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)       38 2023-08-08 16:52:46.662922 cerc-hub-0.1.8.3/setup.cfg
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5190 2023-08-08 16:51:35.000000 cerc-hub-0.1.8.3/setup.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 16:52:46.662922 cerc-hub-0.1.8.3/tests/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4910 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_city_merge.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     2734 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_construction_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    16963 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_construction_factory.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      938 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_costs_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     7097 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_custom_insel_block.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    13035 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_db_factory.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4109 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_db_retrieve.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     7488 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_enrichement.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4852 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_exports.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     9910 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_geometry_factory.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1339 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_greenery_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3225 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_greenery_in_idf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     6967 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_insel_exports.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     4288 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_results_import.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1471 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_systems_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     5818 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_systems_factory.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      819 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_usage_catalog.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)    11500 2023-08-08 16:06:10.000000 cerc-hub-0.1.8.3/tests/test_usage_factory.py
```

### Comparing `cerc-hub-0.1.8.2/PKG-INFO` & `cerc-hub-0.1.8.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-hub
-Version: 0.1.8.2
+Version: 0.1.8.3
 Summary: CERC Hub consist in a set of classes (Central data model), importers and exporters to help researchers to create better and sustainable cities
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 
 CERC Hub consist in a set of classes (Central data model), importers and exporters to help researchers to create better and sustainable cities.
```

### Comparing `cerc-hub-0.1.8.2/cerc_hub.egg-info/PKG-INFO` & `cerc-hub-0.1.8.3/cerc_hub.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-hub
-Version: 0.1.8.2
+Version: 0.1.8.3
 Summary: CERC Hub consist in a set of classes (Central data model), importers and exporters to help researchers to create better and sustainable cities
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 
 CERC Hub consist in a set of classes (Central data model), importers and exporters to help researchers to create better and sustainable cities.
```

### Comparing `cerc-hub-0.1.8.2/cerc_hub.egg-info/SOURCES.txt` & `cerc-hub-0.1.8.3/cerc_hub.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -73,19 +73,17 @@
 hub/catalog_factories/usage/comnet_catalog.py
 hub/catalog_factories/usage/eilat_catalog.py
 hub/catalog_factories/usage/nrcan_catalog.py
 hub/catalog_factories/usage/usage_helper.py
 hub/city_model_structure/__init__.py
 hub/city_model_structure/building.py
 hub/city_model_structure/buildings_cluster.py
-hub/city_model_structure/bus_system.py
 hub/city_model_structure/city.py
 hub/city_model_structure/city_object.py
 hub/city_model_structure/city_objects_cluster.py
-hub/city_model_structure/energy_system.py
 hub/city_model_structure/level_of_detail.py
 hub/city_model_structure/network.py
 hub/city_model_structure/parts_consisting_building.py
 hub/city_model_structure/attributes/__init__.py
 hub/city_model_structure/attributes/edge.py
 hub/city_model_structure/attributes/node.py
 hub/city_model_structure/attributes/plane.py
@@ -93,73 +91,51 @@
 hub/city_model_structure/attributes/polygon.py
 hub/city_model_structure/attributes/polyhedron.py
 hub/city_model_structure/attributes/record.py
 hub/city_model_structure/attributes/schedule.py
 hub/city_model_structure/attributes/time_series.py
 hub/city_model_structure/building_demand/__init__.py
 hub/city_model_structure/building_demand/appliances.py
+hub/city_model_structure/building_demand/construction.py
 hub/city_model_structure/building_demand/domestic_hot_water.py
 hub/city_model_structure/building_demand/household.py
 hub/city_model_structure/building_demand/internal_gain.py
 hub/city_model_structure/building_demand/internal_zone.py
 hub/city_model_structure/building_demand/layer.py
 hub/city_model_structure/building_demand/lighting.py
-hub/city_model_structure/building_demand/material.py
 hub/city_model_structure/building_demand/occupancy.py
 hub/city_model_structure/building_demand/storey.py
 hub/city_model_structure/building_demand/surface.py
+hub/city_model_structure/building_demand/thermal_archetype.py
 hub/city_model_structure/building_demand/thermal_boundary.py
 hub/city_model_structure/building_demand/thermal_control.py
 hub/city_model_structure/building_demand/thermal_opening.py
 hub/city_model_structure/building_demand/thermal_zone.py
 hub/city_model_structure/building_demand/usage.py
 hub/city_model_structure/energy_systems/__init__.py
-hub/city_model_structure/energy_systems/air_source_hp.py
 hub/city_model_structure/energy_systems/control_system.py
 hub/city_model_structure/energy_systems/distribution_system.py
 hub/city_model_structure/energy_systems/emission_system.py
 hub/city_model_structure/energy_systems/energy_system.py
 hub/city_model_structure/energy_systems/generation_system.py
 hub/city_model_structure/energy_systems/generic_distribution_system.py
 hub/city_model_structure/energy_systems/generic_emission_system.py
 hub/city_model_structure/energy_systems/generic_energy_system.py
 hub/city_model_structure/energy_systems/generic_generation_system.py
 hub/city_model_structure/energy_systems/heat_pump.py
-hub/city_model_structure/energy_systems/hvac_system.py
 hub/city_model_structure/energy_systems/hvac_terminal_unit.py
-hub/city_model_structure/energy_systems/water_to_water_hp.py
 hub/city_model_structure/greenery/__init__.py
 hub/city_model_structure/greenery/plant.py
 hub/city_model_structure/greenery/soil.py
 hub/city_model_structure/greenery/vegetation.py
 hub/city_model_structure/iot/__init__.py
 hub/city_model_structure/iot/sensor.py
 hub/city_model_structure/iot/sensor_measure.py
 hub/city_model_structure/iot/sensor_type.py
 hub/city_model_structure/iot/station.py
-hub/city_model_structure/transport/__init__.py
-hub/city_model_structure/transport/bus.py
-hub/city_model_structure/transport/bus_depot.py
-hub/city_model_structure/transport/bus_edge.py
-hub/city_model_structure/transport/bus_network.py
-hub/city_model_structure/transport/bus_node.py
-hub/city_model_structure/transport/bus_stop.py
-hub/city_model_structure/transport/connection.py
-hub/city_model_structure/transport/crossing.py
-hub/city_model_structure/transport/join.py
-hub/city_model_structure/transport/lane.py
-hub/city_model_structure/transport/origin_destination_edge.py
-hub/city_model_structure/transport/origin_destination_network.py
-hub/city_model_structure/transport/origin_destination_node.py
-hub/city_model_structure/transport/phase.py
-hub/city_model_structure/transport/traffic_edge.py
-hub/city_model_structure/transport/traffic_light.py
-hub/city_model_structure/transport/traffic_network.py
-hub/city_model_structure/transport/traffic_node.py
-hub/city_model_structure/transport/walkway_node.py
 hub/config/configuration.ini
 hub/data/construction/eilat_archetypes.json
 hub/data/construction/eilat_constructions.json
 hub/data/construction/nrcan_archetypes.json
 hub/data/construction/nrcan_constructions.json
 hub/data/construction/us_archetypes.xml
 hub/data/construction/us_constructions.xml
@@ -179,14 +155,15 @@
 hub/data/geolocation/cities15000.txt
 hub/data/greenery/ecore_greenery_catalog.xml
 hub/data/usage/comnet_archetypes.xlsx
 hub/data/usage/comnet_schedules_archetypes.xlsx
 hub/data/usage/eilat_archetypes.xlsx
 hub/data/usage/eilat_schedules_archetypes.xlsx
 hub/data/usage/nrcan.xml
+hub/data/weather/epw/CAN_BC_Summerland.717680_CWEC.epw
 hub/data/weather/epw/CAN_PQ_Montreal.Intl.AP.716270_CWEC.epw
 hub/exports/__init__.py
 hub/exports/energy_building_exports_factory.py
 hub/exports/energy_systems_factory.py
 hub/exports/exports_factory.py
 hub/exports/building_energy/__init__.py
 hub/exports/building_energy/energy_ade.py
@@ -208,14 +185,15 @@
 hub/helpers/configuration_helper.py
 hub/helpers/constants.py
 hub/helpers/dictionaries.py
 hub/helpers/geometry_helper.py
 hub/helpers/location.py
 hub/helpers/monthly_values.py
 hub/helpers/peak_loads.py
+hub/helpers/thermal_zones_creation.py
 hub/helpers/utils.py
 hub/helpers/data/__init__.py
 hub/helpers/data/alkis_function_to_hub_function.py
 hub/helpers/data/eilat_function_to_hub_function.py
 hub/helpers/data/hft_function_to_hub_function.py
 hub/helpers/data/hub_function_to_eilat_construction_function.py
 hub/helpers/data/hub_function_to_montreal_custom_costs_function.py
@@ -243,32 +221,26 @@
 hub/imports/construction/eilat_physics_parameters.py
 hub/imports/construction/nrcan_physics_parameters.py
 hub/imports/construction/nrel_physics_parameters.py
 hub/imports/construction/helpers/__init__.py
 hub/imports/construction/helpers/construction_helper.py
 hub/imports/construction/helpers/storeys_generation.py
 hub/imports/energy_systems/__init__.py
-hub/imports/energy_systems/air_source_hp_parameters.py
 hub/imports/energy_systems/montreal_custom_energy_system_parameters.py
-hub/imports/energy_systems/water_to_water_hp_parameters.py
-hub/imports/energy_systems/helpers/__init__.py
-hub/imports/energy_systems/helpers/energy_systems_helper.py
 hub/imports/geometry/__init__.py
 hub/imports/geometry/citygml.py
 hub/imports/geometry/geojson.py
-hub/imports/geometry/gpandas.py
 hub/imports/geometry/obj.py
 hub/imports/geometry/citygml_classes/__init__.py
 hub/imports/geometry/citygml_classes/citygml_base.py
 hub/imports/geometry/citygml_classes/citygml_lod1.py
 hub/imports/geometry/citygml_classes/citygml_lod2.py
 hub/imports/geometry/helpers/__init__.py
 hub/imports/geometry/helpers/geometry_helper.py
 hub/imports/results/__init__.py
-hub/imports/results/insel_heatpump_energy_demand.py
 hub/imports/results/insel_monthly_energry_balance.py
 hub/imports/results/simplified_radiosity_algorithm.py
 hub/imports/usage/__init__.py
 hub/imports/usage/comnet_usage_parameters.py
 hub/imports/usage/eilat_usage_parameters.py
 hub/imports/usage/nrcan_usage_parameters.py
 hub/imports/weather/__init__.py
@@ -295,21 +267,18 @@
 tests/test_city_merge.py
 tests/test_construction_catalog.py
 tests/test_construction_factory.py
 tests/test_costs_catalog.py
 tests/test_custom_insel_block.py
 tests/test_db_factory.py
 tests/test_db_retrieve.py
-tests/test_energy_systems_air_source_hp.py
-tests/test_energy_systems_water_to_water_hp.py
 tests/test_enrichement.py
 tests/test_exports.py
 tests/test_geometry_factory.py
 tests/test_greenery_catalog.py
 tests/test_greenery_in_idf.py
-tests/test_heat_pump_results.py
 tests/test_insel_exports.py
 tests/test_results_import.py
 tests/test_systems_catalog.py
 tests/test_systems_factory.py
 tests/test_usage_catalog.py
 tests/test_usage_factory.py
```

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/catalog.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/construction/construction_helper.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/construction/construction_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/construction/eilat_catalog.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/construction/eilat_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from hub.catalog_factories.data_models.construction.content import Content
 from hub.catalog_factories.construction.construction_helper import ConstructionHelper
 from hub.catalog_factories.data_models.construction.construction import Construction
 from hub.catalog_factories.data_models.construction.archetype import Archetype
 from hub.catalog_factories.data_models.construction.window import Window
 from hub.catalog_factories.data_models.construction.material import Material
 from hub.catalog_factories.data_models.construction.layer import Layer
+import hub.helpers.constants as cte
 
 
 class EilatCatalog(Catalog):
   """
   Eilat catalog class
   """
   def __init__(self, path):
@@ -116,16 +117,16 @@
       archetype_id = f'{archetype["function"]}_{archetype["period_of_construction"]}_{archetype["climate_zone"]}'
       function = archetype['function']
       name = archetype_id
       climate_zone = archetype['climate_zone']
       construction_period = archetype['period_of_construction']
       average_storey_height = archetype['average_storey_height']
       extra_loses_due_to_thermal_bridges = archetype['extra_loses_due_thermal_bridges']
-      infiltration_rate_for_ventilation_system_off = archetype['infiltration_rate_for_ventilation_system_off']
-      infiltration_rate_for_ventilation_system_on = archetype['infiltration_rate_for_ventilation_system_on']
+      infiltration_rate_for_ventilation_system_off = archetype['infiltration_rate_for_ventilation_system_off'] / cte.HOUR_TO_SECONDS
+      infiltration_rate_for_ventilation_system_on = archetype['infiltration_rate_for_ventilation_system_on'] / cte.HOUR_TO_SECONDS
 
       archetype_constructions = []
       for archetype_construction in archetype['constructions']:
         archetype_construction_type = ConstructionHelper().nrcan_surfaces_types_to_hub_types[archetype_construction]
         archetype_construction_name = archetype['constructions'][archetype_construction]['opaque_surface_name']
         for construction in self._catalog_constructions:
           if archetype_construction_type == construction.type and construction.name == archetype_construction_name:
```

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/construction/nrcan_catalog.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/construction/nrcan_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from hub.catalog_factories.data_models.construction.content import Content
 from hub.catalog_factories.construction.construction_helper import ConstructionHelper
 from hub.catalog_factories.data_models.construction.construction import Construction
 from hub.catalog_factories.data_models.construction.archetype import Archetype
 from hub.catalog_factories.data_models.construction.window import Window
 from hub.catalog_factories.data_models.construction.material import Material
 from hub.catalog_factories.data_models.construction.layer import Layer
+import hub.helpers.constants as cte
 
 
 class NrcanCatalog(Catalog):
   """
   Nrcan catalog class
   """
   def __init__(self, path):
@@ -117,16 +118,20 @@
       function = archetype['function']
       name = archetype_id
       climate_zone = archetype['climate_zone']
       construction_period = archetype['period_of_construction']
       average_storey_height = archetype['average_storey_height']
       thermal_capacity = float(archetype['thermal_capacity']) * 1000
       extra_loses_due_to_thermal_bridges = archetype['extra_loses_due_thermal_bridges']
-      infiltration_rate_for_ventilation_system_off = archetype['infiltration_rate_for_ventilation_system_off']
-      infiltration_rate_for_ventilation_system_on = archetype['infiltration_rate_for_ventilation_system_on']
+      infiltration_rate_for_ventilation_system_off = (
+        archetype['infiltration_rate_for_ventilation_system_off'] / cte.HOUR_TO_SECONDS
+      )
+      infiltration_rate_for_ventilation_system_on = (
+        archetype['infiltration_rate_for_ventilation_system_on'] / cte.HOUR_TO_SECONDS
+      )
 
       archetype_constructions = []
       for archetype_construction in archetype['constructions']:
         archetype_construction_type = ConstructionHelper().nrcan_surfaces_types_to_hub_types[archetype_construction]
         archetype_construction_name = archetype['constructions'][archetype_construction]['opaque_surface_name']
         for construction in self._catalog_constructions:
           if archetype_construction_type == construction.type and construction.name == archetype_construction_name:
```

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/construction/nrel_catalog.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/construction/nrel_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from hub.catalog_factories.data_models.construction.window import Window
 from hub.catalog_factories.data_models.construction.material import Material
 from hub.catalog_factories.data_models.construction.layer import Layer
 from hub.catalog_factories.data_models.construction.construction import Construction
 from hub.catalog_factories.data_models.construction.content import Content
 from hub.catalog_factories.data_models.construction.archetype import Archetype
 from hub.catalog_factories.construction.construction_helper import ConstructionHelper
+import hub.helpers.constants as cte
 
 
 class NrelCatalog(Catalog):
   """
   Nrel catalog class
   """
   def __init__(self, path):
@@ -120,18 +121,18 @@
       ]
       average_storey_height = float(archetype['average_storey_height']['#text'])
       thermal_capacity = float(archetype['thermal_capacity']['#text']) * 1000
       extra_loses_due_to_thermal_bridges = float(archetype['extra_loses_due_to_thermal_bridges']['#text'])
       indirect_heated_ratio = float(archetype['indirect_heated_ratio']['#text'])
       infiltration_rate_for_ventilation_system_off = float(
         archetype['infiltration_rate_for_ventilation_system_off']['#text']
-      )
+      ) / cte.HOUR_TO_SECONDS
       infiltration_rate_for_ventilation_system_on = float(
         archetype['infiltration_rate_for_ventilation_system_on']['#text']
-      )
+      ) / cte.HOUR_TO_SECONDS
 
       archetype_constructions = []
       for archetype_construction in archetype['constructions']['construction']:
         for construction in self._catalog_constructions:
           if construction.id == archetype_construction['@id']:
             window_ratio = float(archetype_construction['window_ratio']['#text'])
             window_id = archetype_construction['window']
```

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/construction_catalog_factory.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/construction_catalog_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/cost/montreal_custom_catalog.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/cost/montreal_custom_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/costs_catalog_factory.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/costs_catalog_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/construction/archetype.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/construction/archetype.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,23 +116,23 @@
     :return: float
     """
     return self._indirect_heated_ratio
 
   @property
   def infiltration_rate_for_ventilation_system_off(self):
     """
-    Get archetype infiltration rate for ventilation system off in ACH
+    Get archetype infiltration rate for ventilation system off in 1/s
     :return: float
     """
     return self._infiltration_rate_for_ventilation_system_off
 
   @property
   def infiltration_rate_for_ventilation_system_on(self):
     """
-    Get archetype infiltration rate for ventilation system on in ACH
+    Get archetype infiltration rate for ventilation system on in 1/s
     :return: float
     """
     return self._infiltration_rate_for_ventilation_system_on
 
   def to_dictionary(self):
     """Class content to dictionary"""
     _constructions = []
@@ -143,13 +143,13 @@
                              'function': self.function,
                              'climate zone': self.climate_zone,
                              'period of construction': self.construction_period,
                              'average storey height [m]': self.average_storey_height,
                              'thermal capacity [J/m3K]': self.thermal_capacity,
                              'extra loses due to thermal bridges [W/m2K]': self.extra_loses_due_to_thermal_bridges,
                              'indirect heated ratio': self.indirect_heated_ratio,
-                             'infiltration rate for ventilation off [ACH]': self.infiltration_rate_for_ventilation_system_off,
-                             'infiltration rate for ventilation on [ACH]': self.infiltration_rate_for_ventilation_system_on,
+                             'infiltration rate for ventilation off [1/s]': self.infiltration_rate_for_ventilation_system_off,
+                             'infiltration rate for ventilation on [1/s]': self.infiltration_rate_for_ventilation_system_on,
                              'constructions': _constructions
                              }
                }
     return content
```

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/construction/construction.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/construction/construction.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/construction/content.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/construction/content.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/construction/layer.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/construction/layer.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/construction/material.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/construction/material.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/construction/window.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/construction/window.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/archetype.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/archetype.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/capital_cost.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/capital_cost.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/chapter.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/chapter.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/content.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/content.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/fuel.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/fuel.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,16 +44,15 @@
   def fixed_power(self) -> Union[None, float]:
     """
     Get fixed operational costs depending on the peak power consumed in currency per month per W
     :return: None or float
     """
     if self._fixed_power is not None:
       return self._fixed_power/1000
-    else:
-      return None
+    return None
 
   @property
   def variable(self) -> Union[tuple[None, None], tuple[float, str]]:
     """
     Get variable costs in given units
     :return: None, None or float, str
     """
```

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/income.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/income.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,23 +23,23 @@
     self._photovoltaic_subsidy = photovoltaic_subsidy
     self._electricity_export = electricity_export
     self._reductions_tax = reductions_tax
 
   @property
   def construction_subsidy(self) -> Union[None, float]:
     """
-    Get subsidy for construction in percentage
+    Get subsidy for construction in percentage %
     :return: None or float
     """
     return self._construction_subsidy
 
   @property
   def hvac_subsidy(self) -> Union[None, float]:
     """
-    Get subsidy for HVAC system in percentage
+    Get subsidy for HVAC system in percentage %
     :return: None or float
     """
     return self._hvac_subsidy
 
   @property
   def photovoltaic_subsidy(self) -> Union[None, float]:
     """
```

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/item_description.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/item_description.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/cost/operational_cost.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/cost/operational_cost.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/energy_systems/archetype.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/energy_systems/archetype.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/energy_systems/content.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/energy_systems/content.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/energy_systems/distribution_system.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/energy_systems/distribution_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 """
 
 
 class DistributionSystem:
   """
   Distribution system class
   """
+
   def __init__(self, system_id, name, system_type, supply_temperature, distribution_consumption_fix_flow,
                distribution_consumption_variable_flow, heat_losses):
-
     self._system_id = system_id
     self._name = name
     self._type = system_type
     self._supply_temperature = supply_temperature
     self._distribution_consumption_fix_flow = distribution_consumption_fix_flow
     self._distribution_consumption_variable_flow = distribution_consumption_variable_flow
     self._heat_losses = heat_losses
@@ -76,17 +76,19 @@
     Get heat_losses in ratio over energy produced in J/J
     :return: float
     """
     return self._heat_losses
 
   def to_dictionary(self):
     """Class content to dictionary"""
-    content = {'Layer': {'id': self.id,
-                         'name': self.name,
-                         'type': self.type,
-                         'supply temperature [Celsius]': self.supply_temperature,
-                         'distribution consumption if fix flow over peak power [W/W]': self.distribution_consumption_fix_flow,
-                         'distribution consumption if variable flow over peak power [J/J]': self.distribution_consumption_variable_flow,
-                         'heat losses per energy produced [J/J]': self.heat_losses
-                         }
-               }
+    content = {
+      'Layer': {
+        'id': self.id,
+        'name': self.name,
+        'type': self.type,
+        'supply temperature [Celsius]': self.supply_temperature,
+        'distribution consumption if fix flow over peak power [W/W]': self.distribution_consumption_fix_flow,
+        'distribution consumption if variable flow over peak power [J/J]': self.distribution_consumption_variable_flow,
+        'heat losses per energy produced [J/J]': self.heat_losses
+      }
+    }
     return content
```

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/energy_systems/emission_system.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/energy_systems/emission_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/energy_systems/generation_system.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/energy_systems/generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/energy_systems/system.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/energy_systems/system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/greenery/content.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/greenery/content.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/greenery/plant.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/greenery/plant.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/greenery/plant_percentage.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/greenery/plant_percentage.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/greenery/soil.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/greenery/soil.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/greenery/vegetation.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/greenery/vegetation.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/appliances.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/appliances.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     self._radiative_fraction = radiative_fraction
     self._latent_fraction = latent_fraction
     self._schedules = schedules
 
   @property
   def density(self) -> Union[None, float]:
     """
-    Get appliances density in Watts per m2
+    Get appliances density in W/m2
     :return: None or float
     """
     return self._density
 
   @property
   def convective_fraction(self) -> Union[None, float]:
     """
```

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/content.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/content.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/domestic_hot_water.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/domestic_hot_water.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/lighting.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/lighting.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/occupancy.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/occupancy.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/schedule.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/schedule.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/thermal_control.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/thermal_control.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/data_models/usages/usage.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/data_models/usages/usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     :return: None or float
     """
     return self._days_year
 
   @property
   def mechanical_air_change(self) -> Union[None, float]:
     """
-    Get usage zone mechanical air change in air change per hour (ACH)
+    Get usage zone mechanical air change in air change per second (1/s)
     :return: None or float
     """
     return self._mechanical_air_change
 
   @property
   def ventilation_rate(self) -> Union[None, float]:
     """
```

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/energy_systems/montreal_custom_catalog.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/energy_systems/montreal_custom_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/energy_systems_catalog_factory.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/energy_systems_catalog_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.ecore` & `cerc-hub-0.1.8.3/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.ecore`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog_no_quantities.ecore` & `cerc-hub-0.1.8.3/hub/catalog_factories/greenery/ecore_greenery/greenerycatalog_no_quantities.ecore`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/greenery/greenery_catalog.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/greenery/greenery_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/greenery_catalog_factory.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/greenery_catalog_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/usage/comnet_catalog.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/usage/comnet_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/usage/eilat_catalog.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/usage/eilat_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/usage/nrcan_catalog.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/usage/nrcan_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,16 +130,16 @@
       lighting_schedule = self._get_schedules(lighting_schedule_name)
       appliance_schedule = self._get_schedules(appliance_schedule_name)
       heating_schedule = self._get_schedules(heating_setpoint_schedule_name)
       cooling_schedule = self._get_schedules(cooling_setpoint_schedule_name)
       hvac_availability = self._get_schedules(hvac_schedule_name)
       domestic_hot_water_load_schedule = self._get_schedules(domestic_hot_water_schedule_name)
 
-      # ACH
-      mechanical_air_change = space_type['ventilation_air_changes']
+      # ACH -> 1/s
+      mechanical_air_change = space_type['ventilation_air_changes'] / cte.HOUR_TO_SECONDS
       # cfm/ft2 to m3/m2.s
       ventilation_rate = space_type['ventilation_per_area'] / (cte.METERS_TO_FEET * cte.MINUTES_TO_SECONDS)
       # cfm/person to m3/m2.s
       ventilation_rate += space_type['ventilation_per_person'] / (
           pow(cte.METERS_TO_FEET, 3) * cte.MINUTES_TO_SECONDS
       ) * occupancy_density
```

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/usage/usage_helper.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/usage/usage_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/catalog_factories/usage_catalog_factory.py` & `cerc-hub-0.1.8.3/hub/catalog_factories/usage_catalog_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/attributes/edge.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/attributes/edge.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/attributes/node.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/attributes/node.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/attributes/plane.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/attributes/plane.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/attributes/point.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/attributes/point.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/attributes/polygon.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/attributes/polygon.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/attributes/polyhedron.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/attributes/polyhedron.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/attributes/record.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/attributes/record.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/attributes/schedule.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/attributes/schedule.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/attributes/time_series.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/attributes/time_series.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/building.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/building.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     self._year_of_construction = year_of_construction
     self._function = function
     self._average_storey_height = None
     self._storeys_above_ground = None
     self._floor_area = None
     self._roof_type = None
     self._internal_zones = None
-    self._thermal_zones = None
+    self._thermal_zones_from_internal_zones = None
     self._shell = None
     self._aliases = []
     self._type = 'building'
     self._cold_water_temperature = {}
     self._heating_demand = {}
     self._cooling_demand = {}
     self._lighting_electrical_demand = {}
@@ -110,34 +110,31 @@
     """
     Get building internal zones
     For Lod up to 3, there is only one internal zone which corresponds to the building shell.
     In LoD 4 there can be more than one. In this case the definition of surfaces and floor area must be redefined.
     :return: [InternalZone]
     """
     if self._internal_zones is None:
-      self._internal_zones = [InternalZone(self.surfaces, self.floor_area)]
+      self._internal_zones = [InternalZone(self.surfaces, self.floor_area, self.volume)]
     return self._internal_zones
 
   @property
-  def thermal_zones(self) -> Union[None, List[ThermalZone]]:
+  def thermal_zones_from_internal_zones(self) -> Union[None, List[ThermalZone]]:
     """
     Get building thermal zones
-    For Lod up to 3, there can be more than one thermal zone per internal zone.
-    In LoD 4, there can be more than one internal zone, and therefore, only one thermal zone per internal zone
     :return: [ThermalZone]
     """
-    if self._thermal_zones is None:
-      self._thermal_zones = []
+    if self._thermal_zones_from_internal_zones is None:
+      self._thermal_zones_from_internal_zones = []
       for internal_zone in self.internal_zones:
-        if internal_zone.thermal_zones is None:
-          self._thermal_zones = None
-          return self._thermal_zones
-        for thermal_zone in internal_zone.thermal_zones:
-          self._thermal_zones.append(thermal_zone)
-    return self._thermal_zones
+        if internal_zone.thermal_zones_from_internal_zones is None:
+          self._thermal_zones_from_internal_zones = None
+          return self._thermal_zones_from_internal_zones
+        self._thermal_zones_from_internal_zones.append(internal_zone.thermal_zones_from_internal_zones[0])
+    return self._thermal_zones_from_internal_zones
 
   @property
   def grounds(self) -> List[Surface]:
     """
     Get building ground surfaces
     :return: [Surface]
     """
@@ -257,14 +254,23 @@
 
   @property
   def average_storey_height(self) -> Union[None, float]:
     """
     Get building average storey height in meters
     :return: None or float
     """
+    if len(self.internal_zones) > 1:
+      self._average_storey_height = 0
+      for internal_zone in self.internal_zones:
+        self._average_storey_height += internal_zone.mean_height / len(self.internal_zones)
+    else:
+      if self.internal_zones[0].thermal_archetype is None:
+        self._average_storey_height = None
+      else:
+        self._average_storey_height = self.internal_zones[0].thermal_archetype.average_storey_height
     return self._average_storey_height
 
   @average_storey_height.setter
   def average_storey_height(self, value):
     """
     Set building average storey height in meters
     :param value: float
@@ -292,115 +298,116 @@
     if value is not None:
       self._storeys_above_ground = int(value)
 
   @property
   def cold_water_temperature(self) -> {float}:
     """
     Get cold water temperature in degrees Celsius
-    :return: dict{DataFrame(float)}
+    :return: dict{[float]}
     """
     return self._cold_water_temperature
 
   @cold_water_temperature.setter
   def cold_water_temperature(self, value):
     """
     Set cold water temperature in degrees Celsius
-    :param value: dict{DataFrame(float)}
+    :param value: dict{[float]}
     """
     self._cold_water_temperature = value
 
   @property
   def heating_demand(self) -> dict:
     """
-    Get heating demand in Wh
-    :return: dict{DataFrame(float)}
+    Get heating demand in J
+    :return: dict{[float]}
     """
     return self._heating_demand
 
   @heating_demand.setter
   def heating_demand(self, value):
     """
-    Set heating demand in Wh
-    :param value: dict{DataFrame(float)}
+    Set heating demand in J
+    :param value: dict{[float]}
     """
     self._heating_demand = value
 
   @property
   def cooling_demand(self) -> dict:
     """
-    Get cooling demand in Wh
-    :return: dict{DataFrame(float)}
+    Get cooling demand in J
+    :return: dict{[float]}
     """
     return self._cooling_demand
 
   @cooling_demand.setter
   def cooling_demand(self, value):
     """
-    Set cooling demand in Wh
-    :param value: dict{DataFrame(float)}
+    Set cooling demand in J
+    :param value: dict{[float]}
     """
     self._cooling_demand = value
 
   @property
   def lighting_electrical_demand(self) -> dict:
     """
-    Get lighting electrical demand in Wh
-    :return: dict{DataFrame(float)}
+    Get lighting electrical demand in J
+    :return: dict{[float]}
     """
     return self._lighting_electrical_demand
 
   @lighting_electrical_demand.setter
   def lighting_electrical_demand(self, value):
     """
-    Set lighting electrical demand in Wh
-    :param value: dict{DataFrame(float)}
+    Set lighting electrical demand in J
+    :param value: dict{[float]}
     """
     self._lighting_electrical_demand = value
 
   @property
   def appliances_electrical_demand(self) -> dict:
     """
-    Get appliances electrical demand in Wh
-    :return: dict{DataFrame(float)}
+    Get appliances electrical demand in J
+    :return: dict{[float]}
     """
     return self._appliances_electrical_demand
 
   @appliances_electrical_demand.setter
   def appliances_electrical_demand(self, value):
     """
-    Set appliances electrical demand in Wh
-    :param value: dict{DataFrame(float)}
+    Set appliances electrical demand in J
+    :param value: dict{[float]}
     """
     self._appliances_electrical_demand = value
 
   @property
   def domestic_hot_water_heat_demand(self) -> dict:
     """
-    Get domestic hot water heat demand in Wh
-    :return: dict{DataFrame(float)}
+    Get domestic hot water heat demand in J
+    :return: dict{[float]}
     """
     return self._domestic_hot_water_heat_demand
 
   @domestic_hot_water_heat_demand.setter
   def domestic_hot_water_heat_demand(self, value):
     """
-    Set domestic hot water heat demand in Wh
-    :param value: dict{DataFrame(float)}
+    Set domestic hot water heat demand in J
+    :param value: dict{[float]}
     """
     self._domestic_hot_water_heat_demand = value
 
   @property
   def lighting_peak_load(self) -> Union[None, dict]:
     """
     Get lighting peak load in W
     :return: dict{[float]}
     """
     results = {}
     peak_lighting = 0
-    for thermal_zone in self.thermal_zones:
+    peak = 0
+    for thermal_zone in self.thermal_zones_from_internal_zones:
       lighting = thermal_zone.lighting
       for schedule in lighting.schedules:
         peak = max(schedule.values) * lighting.density * thermal_zone.total_floor_area
         if peak > peak_lighting:
           peak_lighting = peak
     results[cte.MONTH] = [peak for _ in range(0, 12)]
     results[cte.YEAR] = [peak]
@@ -410,56 +417,57 @@
   def appliances_peak_load(self) -> Union[None, dict]:
     """
     Get appliances peak load in W
     :return: dict{[float]}
     """
     results = {}
     peak_appliances = 0
-    for thermal_zone in self.thermal_zones:
+    peak = 0
+    for thermal_zone in self.thermal_zones_from_internal_zones:
       appliances = thermal_zone.appliances
       for schedule in appliances.schedules:
         peak = max(schedule.values) * appliances.density * thermal_zone.total_floor_area
         if peak > peak_appliances:
           peak_appliances = peak
     results[cte.MONTH] = [peak for _ in range(0, 12)]
     results[cte.YEAR] = [peak]
     return results
 
   @property
   def heating_peak_load(self) -> Union[None, dict]:
     """
     Get heating peak load in W
-    :return: dict{DataFrame(float)}
+    :return: dict{[float]}
     """
     results = {}
     if cte.HOUR in self.heating_demand:
       monthly_values = PeakLoads().\
-        peak_loads_from_hourly(self.heating_demand[cte.HOUR][next(iter(self.heating_demand[cte.HOUR]))])
+        peak_loads_from_hourly(self.heating_demand[cte.HOUR])
     else:
       monthly_values = PeakLoads(self).heating_peak_loads_from_methodology
     if monthly_values is None:
       return None
-    results[cte.MONTH] = monthly_values
+    results[cte.MONTH] = [x * cte.WATTS_HOUR_TO_JULES for x in monthly_values]
     results[cte.YEAR] = [max(monthly_values)]
     return results
 
   @property
   def cooling_peak_load(self) -> Union[None, dict]:
     """
     Get cooling peak load in W
-    :return: dict{DataFrame(float)}
+    :return: dict{[float]}
     """
     results = {}
     if cte.HOUR in self.cooling_demand:
-      monthly_values = PeakLoads().peak_loads_from_hourly(self.cooling_demand[cte.HOUR][next(iter(self.cooling_demand[cte.HOUR]))])
+      monthly_values = PeakLoads().peak_loads_from_hourly(self.cooling_demand[cte.HOUR])
     else:
       monthly_values = PeakLoads(self).cooling_peak_loads_from_methodology
     if monthly_values is None:
       return None
-    results[cte.MONTH] = monthly_values
+    results[cte.MONTH] = [x * cte.WATTS_HOUR_TO_JULES for x in monthly_values]
     results[cte.YEAR] = [max(monthly_values)]
     return results
 
   @property
   def eave_height(self):
     """
     Get building eave height in meters
@@ -605,63 +613,63 @@
     :param value: str
     """
     self._systems_archetype_name = value
 
   @property
   def heating_consumption(self):
     """
-    Get energy consumption for heating according to the heating system installed in Wh
+    Get energy consumption for heating according to the heating system installed in J
     return: dict
     """
     if len(self._heating_consumption) == 0:
       for heating_demand_key in self.heating_demand:
-        demand = self.heating_demand[heating_demand_key][cte.INSEL_MEB]
+        demand = self.heating_demand[heating_demand_key]
         consumption_type = cte.HEATING
         final_energy_consumed = self._calculate_consumption(consumption_type, demand)
         if final_energy_consumed is None:
           continue
         self._heating_consumption[heating_demand_key] = final_energy_consumed
     return self._heating_consumption
 
   @property
   def cooling_consumption(self):
     """
-    Get energy consumption for cooling according to the cooling system installed in Wh
+    Get energy consumption for cooling according to the cooling system installed in J
     return: dict
     """
     if len(self._cooling_consumption) == 0:
       for cooling_demand_key in self.cooling_demand:
-        demand = self.cooling_demand[cooling_demand_key][cte.INSEL_MEB]
+        demand = self.cooling_demand[cooling_demand_key]
         consumption_type = cte.COOLING
         final_energy_consumed = self._calculate_consumption(consumption_type, demand)
         if final_energy_consumed is None:
           continue
         self._cooling_consumption[cooling_demand_key] = final_energy_consumed
     return self._cooling_consumption
 
   @property
   def domestic_hot_water_consumption(self):
     """
-    Get energy consumption for domestic according to the domestic hot water system installed in Wh
+    Get energy consumption for domestic according to the domestic hot water system installed in J
     return: dict
     """
     if len(self._domestic_hot_water_consumption) == 0:
       for domestic_hot_water_demand_key in self.domestic_hot_water_heat_demand:
-        demand = self.domestic_hot_water_heat_demand[domestic_hot_water_demand_key][cte.INSEL_MEB]
+        demand = self.domestic_hot_water_heat_demand[domestic_hot_water_demand_key]
         consumption_type = cte.DOMESTIC_HOT_WATER
         final_energy_consumed = self._calculate_consumption(consumption_type, demand)
         if final_energy_consumed is None:
           continue
         self._domestic_hot_water_consumption[domestic_hot_water_demand_key] = final_energy_consumed
     return self._domestic_hot_water_consumption
 
   def _calculate_working_hours(self):
     _working_hours = {}
     for internal_zone in self.internal_zones:
-      for thermal_zone in internal_zone.thermal_zones:
+      for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
         _working_hours_per_thermal_zone = {}
         for schedule in thermal_zone.thermal_control.hvac_availability_schedules:
           _working_hours_per_schedule = [0] * len(schedule.values)
           for i, value in enumerate(schedule.values):
             if value > 0:
               _working_hours_per_schedule[i] = 1
           for day_type in schedule.day_types:
@@ -673,21 +681,21 @@
             saved_values = _working_hours_per_thermal_zone[key]
             for i, value in enumerate(item):
               _working_hours[key][i] = max(_working_hours[key][i], saved_values[i])
 
     _total_hours = 0
     for key in _working_hours:
       hours = sum(_working_hours[key])
-      _total_hours += hours * cte.DAYS_A_YEAR[key]
+      _total_hours += hours * cte.WEEK_DAYS_A_YEAR[key]
     return _total_hours
 
   @property
   def distribution_systems_electrical_consumption(self):
     """
-    Get total electricity consumption for distribution and emission systems in Wh
+    Get total electricity consumption for distribution and emission systems in J
     return: dict
     """
     if len(self._distribution_systems_electrical_consumption) != 0:
       return self._distribution_systems_electrical_consumption
     _peak_load = self.heating_peak_load[cte.YEAR][0]
     _peak_load_type = cte.HEATING
     if _peak_load < self.cooling_peak_load[cte.YEAR][0]:
@@ -706,25 +714,25 @@
       distribution_system = energy_system.distribution_system.generic_distribution_system
       consumption_variable_flow = distribution_system.distribution_consumption_variable_flow
       for demand_type in energy_system.demand_types:
         if demand_type.lower() == cte.HEATING.lower():
           if _peak_load_type == cte.HEATING.lower():
             _consumption_fix_flow = distribution_system.distribution_consumption_fix_flow
           for heating_demand_key in self.heating_demand:
-            _consumption = [0]*len(self.heating_demand[heating_demand_key][cte.INSEL_MEB])
-            _demand = self.heating_demand[heating_demand_key][cte.INSEL_MEB]
+            _consumption = [0]*len(self.heating_demand[heating_demand_key])
+            _demand = self.heating_demand[heating_demand_key]
             for i, _ in enumerate(_consumption):
               _consumption[i] += (parasitic_energy_consumption + consumption_variable_flow) * _demand[i]
             self._distribution_systems_electrical_consumption[heating_demand_key] = _consumption
         if demand_type.lower() == cte.COOLING.lower():
           if _peak_load_type == cte.COOLING.lower():
             _consumption_fix_flow = distribution_system.distribution_consumption_fix_flow
           for demand_key in self.cooling_demand:
             _consumption = self._distribution_systems_electrical_consumption[demand_key]
-            _demand = self.cooling_demand[demand_key][cte.INSEL_MEB]
+            _demand = self.cooling_demand[demand_key]
             for i, _ in enumerate(_consumption):
               _consumption[i] += (parasitic_energy_consumption + consumption_variable_flow) * _demand[i]
             self._distribution_systems_electrical_consumption[demand_key] = _consumption
 
       for key, item in self._distribution_systems_electrical_consumption.items():
         for i in range(0, len(item)):
           self._distribution_systems_electrical_consumption[key][i] += _peak_load * _consumption_fix_flow \
@@ -754,38 +762,38 @@
       for demand_value in demand:
         final_energy_consumed.append(demand_value / coefficient_of_performance)
     return final_energy_consumed
 
   @property
   def onsite_electrical_production(self):
     """
-    Get total electricity produced onsite in Wh
+    Get total electricity produced onsite in J
     return: dict
     """
-
-    # Add other systems whenever new ones appear
     orientation_losses_factor = {cte.MONTH: {'north': [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
                                              'east': [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
                                              'south': [2.137931, 1.645503, 1.320946, 1.107817, 0.993213, 0.945175,
                                                        0.967949, 1.065534, 1.24183, 1.486486, 1.918033, 2.210526],
                                              'west': [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]},
                                  cte.YEAR: {'north': [0],
                                             'east': [0],
                                             'south': [1.212544],
                                             'west': [0]}
                                  }
+
+    # Add other systems whenever new ones appear
     if self.energy_systems is None:
       return self._onsite_electrical_production
     for energy_system in self.energy_systems:
       if energy_system.generation_system.generic_generation_system.type == cte.PHOTOVOLTAIC:
         _efficiency = energy_system.generation_system.generic_generation_system.electricity_efficiency
         self._onsite_electrical_production = {}
         for _key in self.roofs[0].global_irradiance.keys():
-          _results = [0 for _ in range(0, len(self.roofs[0].global_irradiance[_key][cte.SRA]))]
+          _results = [0 for _ in range(0, len(self.roofs[0].global_irradiance[_key]))]
           for surface in self.roofs:
             if _key in orientation_losses_factor:
               _results = [x + y * _efficiency * surface.perimeter_area
                           * surface.solar_collectors_area_reduction_factor * z
-                          for x, y, z in zip(_results, surface.global_irradiance[_key][cte.SRA],
+                          for x, y, z in zip(_results, surface.global_irradiance[_key],
                                              orientation_losses_factor[_key]['south'])]
           self._onsite_electrical_production[_key] = _results
     return self._onsite_electrical_production
```

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/appliances.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/appliances.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/domestic_hot_water.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/domestic_hot_water.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/household.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/household.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/internal_gain.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/internal_gain.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/layer.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/iot/sensor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,79 @@
 """
-Layers module
+Sensor module
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2022 Concordia CERC group
 Project Coder Guille Gutierrez guillermo.gutierrezmorote@concordia.ca
 """
-import uuid
-from typing import Union
-from hub.city_model_structure.building_demand.material import Material
 
+from hub.helpers.location import Location
+from hub.city_model_structure.iot.sensor_measure import SensorMeasure
+from hub.city_model_structure.iot.sensor_type import SensorType
 
-class Layer:
+
+class Sensor:
   """
-  Layer class
+  Sensor abstract class
   """
   def __init__(self):
-    self._material = None
-    self._thickness = None
-    self._id = None
+    self._name = None
+    self._type = None
+    self._units = None
+    self._location = None
 
   @property
-  def id(self):
+  def name(self):
     """
-    Get layer id, a universally unique identifier randomly generated
+    Get sensor name
     :return: str
     """
-    if self._id is None:
-      self._id = uuid.uuid4()
-    return self._id
+    if self._name is None:
+      raise ValueError('Undefined sensor name')
+    return self._name
+
+  @name.setter
+  def name(self, value):
+    """
+    Set sensor name
+    :param value: str
+    """
+    if value is not None:
+      self._name = str(value)
 
   @property
-  def material(self) -> Material:
+  def type(self) -> SensorType:
     """
-    Get layer material
-    :return: Material
+    Get sensor type
+    :return: str
     """
-    return self._material
+    return self._type
 
-  @material.setter
-  def material(self, value):
+  @property
+  def units(self):
     """
-    Set layer material
-    :param value: Material
+    Get sensor units
+    :return: str
     """
-    self._material = value
+    return self._units
 
   @property
-  def thickness(self) -> Union[None, float]:
+  def location(self) -> Location:
     """
-    Get layer thickness in meters
-    :return: None or float
+    Get sensor location
+    :return: Location
     """
-    return self._thickness
+    return self._location
 
-  @thickness.setter
-  def thickness(self, value):
+  @location.setter
+  def location(self, value):
     """
-    Get layer thickness in meters
-    :param value: float
+    Set sensor location
+    :param value: Location
     """
-    if value is not None:
-      self._thickness = float(value)
+    self._location = value
+
+  @property
+  def measures(self) -> [SensorMeasure]:
+    """
+    Raises not implemented error
+    """
+    raise NotImplementedError
```

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/lighting.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/lighting.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/material.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/layer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,61 @@
 """
-Material module
+Layers module
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2022 Concordia CERC group
 Project Coder Guille Gutierrez guillermo.gutierrezmorote@concordia.ca
 """
 
+import uuid
 from typing import Union
 
 
-class Material:
+class Layer:
   """
-  Material class
+  Layer class
   """
   def __init__(self):
+    self._thickness = None
     self._id = None
     self._name = None
     self._conductivity = None
     self._specific_heat = None
     self._density = None
     self._solar_absorptance = None
     self._thermal_absorptance = None
     self._visible_absorptance = None
     self._no_mass = False
     self._thermal_resistance = None
 
   @property
   def id(self):
     """
-    Get material id
+    Get layer id, a universally unique identifier randomly generated
     :return: str
     """
+    if self._id is None:
+      self._id = uuid.uuid4()
     return self._id
 
-  @id.setter
-  def id(self, value):
+  @property
+  def thickness(self) -> Union[None, float]:
+    """
+    Get layer thickness in meters
+    :return: None or float
+    """
+    return self._thickness
+
+  @thickness.setter
+  def thickness(self, value):
     """
-    Set material id
-    :param value: str
+    Get layer thickness in meters
+    :param value: float
     """
-    self._id = value
+    if value is not None:
+      self._thickness = float(value)
 
   @property
   def name(self):
     """
     Get material name
     :return: str
     """
```

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/occupancy.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/occupancy.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/storey.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/storey.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,17 @@
   @property
   def thermal_zone(self) -> ThermalZone:
     """
     Get the thermal zone inside the storey
     :return: ThermalZone
     """
     if self._thermal_zone is None:
-      self._thermal_zone = ThermalZone(self.thermal_boundaries, self._internal_zone, self.volume, self.floor_area)
+      _number_of_storeys = 1
+      self._thermal_zone = ThermalZone(self.thermal_boundaries, self._internal_zone,
+                                       self.volume, self.floor_area, _number_of_storeys)
     return self._thermal_zone
 
   @property
   def volume(self):
     """
     Get storey's volume in cubic meters
     :return: float
```

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/surface.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/surface.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,24 +174,24 @@
       else:
         self._type = 'Roof'
     return self._type
 
   @property
   def global_irradiance(self) -> dict:
     """
-    Get global irradiance on surface in Wh/m2
-    :return: dict{DataFrame(float)}
+    Get global irradiance on surface in J/m2
+    :return: dict
     """
     return self._global_irradiance
 
   @global_irradiance.setter
   def global_irradiance(self, value):
     """
-    Set global irradiance on surface in Wh/m2
-    :param value: dict{DataFrame(float)}
+    Set global irradiance on surface in J/m2
+    :param value: dict
     """
     self._global_irradiance = value
 
   @property
   def perimeter_polygon(self) -> Polygon:
     """
     Get a polygon surface defined by the perimeter, merging solid and holes
```

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/thermal_boundary.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/thermal_boundary.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2022 Concordia CERC group
 Project Coder Guille Gutierrez guillermo.gutierrezmorote@concordia.ca
 Code contributors: Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
 """
 
 import uuid
+import math
 from typing import List, Union, TypeVar
+import logging
 from hub.helpers.configuration_helper import ConfigurationHelper as ch
 import hub.helpers.constants as cte
 from hub.city_model_structure.building_demand.layer import Layer
 from hub.city_model_structure.building_demand.thermal_opening import ThermalOpening
 from hub.city_model_structure.building_demand.thermal_zone import ThermalZone
 
 Surface = TypeVar('Surface')
@@ -31,15 +33,16 @@
     self._layers = None
     self._he = ch().convective_heat_transfer_coefficient_exterior
     self._hi = ch().convective_heat_transfer_coefficient_interior
     self._u_value = None
     self._construction_name = None
     self._thickness = None
     self._internal_surface = None
-    self._window_ratio = None
+    self._external_surface = None
+    self._window_ratio = 0
     self._window_ratio_to_be_calculated = False
     if self._windows_areas is not None:
       self._window_ratio_to_be_calculated = True
 
   @property
   def id(self):
     """
@@ -49,15 +52,15 @@
     if self._id is None:
       self._id = uuid.uuid4()
     return self._id
 
   @property
   def parent_surface(self) -> Surface:
     """
-    Get the surface that belongs to the thermal boundary
+    Get the surface that belongs to the thermal boundary, considered the external surface of that boundary
     :return: Surface
     """
     return self._parent_surface
 
   @property
   def thermal_zones(self) -> List[ThermalZone]:
     """
@@ -88,15 +91,15 @@
     Get the thermal boundary thickness in meters
     :return: float
     """
     if self._thickness is None:
       self._thickness = 0.0
       if self.layers is not None:
         for layer in self.layers:
-          if not layer.material.no_mass:
+          if not layer.no_mass:
             self._thickness += layer.thickness
     return self._thickness
 
   @property
   def thermal_openings(self) -> Union[None, List[ThermalOpening]]:
     """
     Get thermal boundary thermal openings
@@ -144,49 +147,43 @@
           else:
             for _thermal_opening in self._thermal_openings:
               if self.window_ratio == 1:
                 _area = self.opaque_area
               else:
                 _area = self.opaque_area * self.window_ratio / (1-self.window_ratio)
               _thermal_opening.area = _area
+              self._thermal_openings = [_thermal_opening]
+    for thermal_opening in self._thermal_openings:
+      thermal_opening.g_value = self._construction_archetype.window_g_value
+      thermal_opening.overall_u_value = self._construction_archetype.window_overall_u_value
+      thermal_opening.frame_ratio = self._construction_archetype.window_frame_ratio
+      thermal_opening.construction_name = self._construction_archetype.window_type
     return self._thermal_openings
 
   @property
-  def construction_name(self) -> Union[None, str]:
-    """
-    Get construction name
-    :return: None or str
-    """
-    return self._construction_name
-
-  @construction_name.setter
-  def construction_name(self, value):
-    """
-    Set construction name
-    :param value: str
-    """
-    if value is not None:
-      self._construction_name = str(value)
+  def _construction_archetype(self):
+    construction_archetypes = self.thermal_zones[0].parent_internal_zone.thermal_archetype.constructions
+    for construction_archetype in construction_archetypes:
+      if str(self.type) == str(construction_archetype.type):
+        return construction_archetype
+    return None
 
   @property
   def layers(self) -> List[Layer]:
     """
     Get thermal boundary layers
     :return: [Layers]
     """
+    if self._construction_archetype is not None:
+      self._layers = self._construction_archetype.layers
+    else:
+      logging.error('Layers not defined\n')
+      raise ValueError('Layers not defined')
     return self._layers
 
-  @layers.setter
-  def layers(self, value):
-    """
-    Set thermal boundary layers
-    :param value: [Layer]
-    """
-    self._layers = value
-
   @property
   def type(self):
     """
     Get thermal boundary surface type
     :return: str
     """
     return self.parent_surface.type
@@ -205,26 +202,31 @@
       if len(self.windows_areas) == 0:
         self._window_ratio = 0
       else:
         total_window_area = 0
         for window_area in self.windows_areas:
           total_window_area += window_area
         self._window_ratio = total_window_area / (self.opaque_area + total_window_area)
+    else:
+      if self.type in (cte.WALL, cte.ROOF):
+        if -math.sqrt(2) / 2 < math.sin(self.parent_surface.azimuth) < math.sqrt(2) / 2:
+          if 0 < math.cos(self.parent_surface.azimuth):
+            self._window_ratio = \
+              float(self._construction_archetype.window_ratio['north']) / 100
+          else:
+            self._window_ratio = \
+              float(self._construction_archetype.window_ratio['south']) / 100
+        elif math.sqrt(2) / 2 <= math.sin(self._parent_surface.azimuth):
+          self._window_ratio = \
+            float(self._construction_archetype.window_ratio['east']) / 100
+        else:
+          self._window_ratio = \
+            float(self._construction_archetype.window_ratio['west']) / 100
     return self._window_ratio
 
-  @window_ratio.setter
-  def window_ratio(self, value):
-    """
-    Set thermal boundary window ratio
-    :param value: str
-    """
-    if self._window_ratio_to_be_calculated:
-      raise ValueError('Window ratio cannot be assigned when the windows are defined in the geometry.')
-    self._window_ratio = float(value)
-
   @property
   def windows_areas(self) -> [float]:
     """
     Get windows areas
     :return: [float]
     """
     return self._windows_areas
@@ -241,18 +243,18 @@
       h_e = self.he
       if self.type == cte.GROUND:
         r_value = 1.0 / h_i + ch().soil_thickness / ch().soil_conductivity
       else:
         r_value = 1.0/h_i + 1.0/h_e
       try:
         for layer in self.layers:
-          if layer.material.no_mass:
-            r_value += float(layer.material.thermal_resistance)
+          if layer.no_mass:
+            r_value += float(layer.thermal_resistance)
           else:
-            r_value += float(layer.thickness) / float(layer.material.conductivity)
+            r_value += float(layer.thickness) / float(layer.conductivity)
         self._u_value = 1.0/r_value
       except TypeError:
         raise TypeError('Constructions layers are not initialized') from TypeError
     return self._u_value
 
   @u_value.setter
   def u_value(self, value):
@@ -301,8 +303,22 @@
   def internal_surface(self) -> Surface:
     """
     Get the internal surface of the thermal boundary
     :return: Surface
     """
     if self._internal_surface is None:
       self._internal_surface = self.parent_surface.inverse
+      # The agreement is that the layers are defined from outside to inside
+      internal_layer = self.layers[len(self.layers) - 1]
+      self._internal_surface.short_wave_reflectance = 1 - internal_layer.solar_absorptance
+      self._internal_surface.long_wave_emittance = 1 - internal_layer.solar_absorptance
+
     return self._internal_surface
+
+  @property
+  def external_surface(self) -> Surface:
+    if self._external_surface is None:
+      # The agreement is that the layers are defined from outside to inside
+      self._external_surface = self.parent_surface
+      self._external_surface.short_wave_reflectance = 1 - self.layers[0].solar_absorptance
+      self._external_surface.long_wave_emittance = 1 - self.layers[0].solar_absorptance
+    return self._external_surface
```

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/thermal_control.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/thermal_control.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/thermal_opening.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/thermal_opening.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/thermal_zone.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/thermal_zone.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,28 +25,34 @@
 
 
 class ThermalZone:
   """
   ThermalZone class
   """
 
-  def __init__(self, thermal_boundaries, parent_internal_zone, volume, footprint_area, usage_name=None):
+  def __init__(self, thermal_boundaries,
+               parent_internal_zone,
+               volume,
+               footprint_area,
+               number_of_storeys,
+               usage_name=None):
     self._id = None
     self._parent_internal_zone = parent_internal_zone
     self._footprint_area = footprint_area
     self._thermal_boundaries = thermal_boundaries
     self._additional_thermal_bridge_u_value = None
     self._effective_thermal_capacity = None
     self._indirectly_heated_area_ratio = None
     self._infiltration_rate_system_on = None
     self._infiltration_rate_system_off = None
     self._volume = volume
     self._ordinate_number = None
     self._view_factors_matrix = None
     self._total_floor_area = None
+    self._number_of_storeys = number_of_storeys
     self._usage_name = usage_name
     self._usage_from_parent = False
     if usage_name is None:
       self._usage_from_parent = True
     self._hours_day = None
     self._days_year = None
     self._mechanical_air_change = None
@@ -55,14 +61,22 @@
     self._appliances = None
     self._internal_gains = None
     self._thermal_control = None
     self._domestic_hot_water = None
     self._usages = None
 
   @property
+  def parent_internal_zone(self) -> InternalZone:
+    """
+    Get the internal zone to which this thermal zone belongs
+    :return: InternalZone
+    """
+    return self._parent_internal_zone
+
+  @property
   def usages(self):
     """
     Get the thermal zone usages including percentage with the format [percentage]-usage_[percentage]-usage...
     Eg: 70-office_30-residential
     :return: str
     """
     if self._usage_from_parent:
@@ -109,91 +123,53 @@
 
   @property
   def additional_thermal_bridge_u_value(self) -> Union[None, float]:
     """
     Get thermal zone additional thermal bridge u value per footprint area W/m2K
     :return: None or float
     """
+    self._additional_thermal_bridge_u_value = self.parent_internal_zone.thermal_archetype.extra_loses_due_to_thermal_bridges
     return self._additional_thermal_bridge_u_value
 
-  @additional_thermal_bridge_u_value.setter
-  def additional_thermal_bridge_u_value(self, value):
-    """
-    Set thermal zone additional thermal bridge u value per footprint area W/m2K
-    :param value: float
-    """
-    if value is not None:
-      self._additional_thermal_bridge_u_value = float(value)
-
   @property
   def effective_thermal_capacity(self) -> Union[None, float]:
     """
     Get thermal zone effective thermal capacity in J/m3K
     :return: None or float
     """
+    self._effective_thermal_capacity = self._parent_internal_zone.thermal_archetype.thermal_capacity
     return self._effective_thermal_capacity
 
-  @effective_thermal_capacity.setter
-  def effective_thermal_capacity(self, value):
-    """
-    Set thermal zone effective thermal capacity in J/m3K
-    :param value: float
-    """
-    if value is not None:
-      self._effective_thermal_capacity = float(value)
-
   @property
   def indirectly_heated_area_ratio(self) -> Union[None, float]:
     """
     Get thermal zone indirectly heated area ratio
     :return: None or float
     """
+    self._indirectly_heated_area_ratio = self._parent_internal_zone.thermal_archetype.indirect_heated_ratio
     return self._indirectly_heated_area_ratio
 
-  @indirectly_heated_area_ratio.setter
-  def indirectly_heated_area_ratio(self, value):
-    """
-    Set thermal zone indirectly heated area ratio
-    :param value: float
-    """
-    if value is not None:
-      self._indirectly_heated_area_ratio = float(value)
-
   @property
   def infiltration_rate_system_on(self):
     """
-    Get thermal zone infiltration rate system on in air changes per hour (ACH)
+    Get thermal zone infiltration rate system on in air changes per second (1/s)
     :return: None or float
     """
+    self._infiltration_rate_system_on = self._parent_internal_zone.thermal_archetype.infiltration_rate_for_ventilation_system_on
     return self._infiltration_rate_system_on
 
-  @infiltration_rate_system_on.setter
-  def infiltration_rate_system_on(self, value):
-    """
-    Set thermal zone infiltration rate system on in air changes per hour (ACH)
-    :param value: float
-    """
-    self._infiltration_rate_system_on = value
-
   @property
   def infiltration_rate_system_off(self):
     """
-    Get thermal zone infiltration rate system off in air changes per hour (ACH)
+    Get thermal zone infiltration rate system off in air changes per second (1/s)
     :return: None or float
     """
+    self._infiltration_rate_system_off = self._parent_internal_zone.thermal_archetype.infiltration_rate_for_ventilation_system_off
     return self._infiltration_rate_system_off
 
-  @infiltration_rate_system_off.setter
-  def infiltration_rate_system_off(self, value):
-    """
-    Set thermal zone infiltration rate system on in air changes per hour (ACH)
-    :param value: float
-    """
-    self._infiltration_rate_system_off = value
-
   @property
   def volume(self):
     """
     Get thermal zone volume
     :return: float
     """
     return self._volume
@@ -217,24 +193,52 @@
 
   @property
   def view_factors_matrix(self):
     """
     Get thermal zone view factors matrix
     :return: [[float]]
     """
+    # todo: review method if windows not in window_ratio but in geometry
+    if self._view_factors_matrix is None:
+      total_area = 0
+      for thermal_boundary in self.thermal_boundaries:
+        total_area += thermal_boundary.opaque_area
+        for thermal_opening in thermal_boundary.thermal_openings:
+          total_area += thermal_opening.area
+
+      view_factors_matrix = []
+      for thermal_boundary_1 in self.thermal_boundaries:
+        values = []
+        for thermal_boundary_2 in self.thermal_boundaries:
+          value = 0
+          if thermal_boundary_1.id != thermal_boundary_2.id:
+            value = thermal_boundary_2.opaque_area / (total_area - thermal_boundary_1.opaque_area)
+          values.append(value)
+        for thermal_boundary in self.thermal_boundaries:
+          for thermal_opening in thermal_boundary.thermal_openings:
+            value = thermal_opening.area / (total_area - thermal_boundary_1.opaque_area)
+            values.append(value)
+        view_factors_matrix.append(values)
+
+      for thermal_boundary_1 in self.thermal_boundaries:
+        values = []
+        for thermal_opening_1 in thermal_boundary_1.thermal_openings:
+          for thermal_boundary_2 in self.thermal_boundaries:
+            value = thermal_boundary_2.opaque_area / (total_area - thermal_opening_1.area)
+            values.append(value)
+          for thermal_boundary in self.thermal_boundaries:
+            for thermal_opening_2 in thermal_boundary.thermal_openings:
+              value = 0
+              if thermal_opening_1.id != thermal_opening_2.id:
+                value = thermal_opening_2.area / (total_area - thermal_opening_1.area)
+              values.append(value)
+          view_factors_matrix.append(values)
+      self._view_factors_matrix = view_factors_matrix
     return self._view_factors_matrix
 
-  @view_factors_matrix.setter
-  def view_factors_matrix(self, value):
-    """
-    Set thermal zone view factors matrix
-    :param value: [[float]]
-    """
-    self._view_factors_matrix = value
-
   @property
   def usage_name(self) -> Union[None, str]:
     """
     Get thermal zone usage name
     :return: None or str
     """
     if self._usage_from_parent:
@@ -281,15 +285,15 @@
       for usage in self.usages:
         self._days_year += usage.percentage * usage.days_year
     return self._days_year
 
   @property
   def mechanical_air_change(self) -> Union[None, float]:
     """
-    Get thermal zone mechanical air change in air change per hour (ACH)
+    Get thermal zone mechanical air change in air change per second (1/s)
     :return: None or float
     """
     if self.usages is None:
       return None
     if self._mechanical_air_change is None:
       self._mechanical_air_change = 0
       for usage in self.usages:
@@ -649,19 +653,12 @@
       self._domestic_hot_water.schedules = _schedules
 
     return self._domestic_hot_water
 
   @property
   def total_floor_area(self):
     """
-    Get the total floor area of this thermal zone
+    Get the total floor area of this thermal zone in m2
     :return: float
     """
+    self._total_floor_area = self.footprint_area * self._number_of_storeys
     return self._total_floor_area
-
-  @total_floor_area.setter
-  def total_floor_area(self, value):
-    """
-    Set the total floor area of this thermal zone
-    :param value: float
-    """
-    self._total_floor_area = value
```

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/building_demand/usage.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,23 +169,23 @@
     """
     if value is not None:
       self._days_year = float(value)
 
   @property
   def mechanical_air_change(self) -> Union[None, float]:
     """
-    Get usage zone mechanical air change in air change per hour (ACH)
+    Get usage zone mechanical air change in air change per second (1/s)
     :return: None or float
     """
     return self._mechanical_air_change
 
   @mechanical_air_change.setter
   def mechanical_air_change(self, value):
     """
-    Set usage zone mechanical air change in air change per hour (ACH)
+    Set usage zone mechanical air change in air change per second (1/s)
     :param value: float
     """
     if value is not None:
       self._mechanical_air_change = float(value)
 
   @property
   def occupancy(self) -> Union[None, Occupancy]:
```

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/buildings_cluster.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/buildings_cluster.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/city.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/city.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from pandas import DataFrame
 from pyproj import Transformer
 
 from hub.city_model_structure.building import Building
 from hub.city_model_structure.buildings_cluster import BuildingsCluster
 from hub.city_model_structure.city_object import CityObject
 from hub.city_model_structure.city_objects_cluster import CityObjectsCluster
-from hub.city_model_structure.energy_system import EnergySystem
 from hub.city_model_structure.iot.station import Station
 from hub.city_model_structure.level_of_detail import LevelOfDetail
 from hub.city_model_structure.parts_consisting_building import PartsConsistingBuilding
 from hub.helpers.geometry_helper import GeometryHelper
 from hub.helpers.location import Location
 import hub.helpers.constants as cte
 
@@ -159,17 +158,14 @@
       if self.city_objects_clusters is None:
         self._city_objects = []
       else:
         self._city_objects = self.city_objects_clusters
       if self.buildings is not None:
         for building in self.buildings:
           self._city_objects.append(building)
-      if self.energy_systems is not None:
-        for energy_system in self.energy_systems:
-          self._city_objects.append(energy_system)
     return self._city_objects
 
   @property
   def buildings(self) -> Union[List[Building], None]:
     """
     Get the buildings belonging to the city
     :return: None or [Building]
@@ -406,22 +402,14 @@
     """
     Get parts consisting buildings belonging to the city
     :return: None or [PartsConsistingBuilding]
     """
     return self._parts_consisting_buildings
 
   @property
-  def energy_systems(self) -> Union[List[EnergySystem], None]:
-    """
-    Get energy systems belonging to the city
-    :return: None or [EnergySystem]
-    """
-    return self._energy_systems
-
-  @property
   def stations(self) -> [Station]:
     """
     Get the sensors stations belonging to the city
     :return: [Station]
     """
     return self._stations
 
@@ -474,20 +462,20 @@
         # building is new so added to the city
         merged_city.add_city_object(copy.deepcopy(building))
       else:
         # keep the one with less radiation
         parameter_city_building_total_radiation = 0
         for surface in building.surfaces:
           if surface.global_irradiance:
-            parameter_city_building_total_radiation += surface.global_irradiance[cte.YEAR].iloc[0, 0]
+            parameter_city_building_total_radiation += surface.global_irradiance[cte.YEAR][0]
 
         merged_city_building_total_radiation = 0
         for surface in merged_city.city_object(building.name).surfaces:
           if surface.global_irradiance:
-            merged_city_building_total_radiation += surface.global_irradiance[cte.YEAR].iloc[0, 0]
+            merged_city_building_total_radiation += surface.global_irradiance[cte.YEAR][0]
 
         if merged_city_building_total_radiation == 0:
           merged_city.remove_city_object(merged_city.city_object(building.name))
           merged_city.add_city_object(building)
         elif merged_city_building_total_radiation > parameter_city_building_total_radiation > 0:
           merged_city.remove_city_object(merged_city.city_object(building.name))
           merged_city.add_city_object(building)
```

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/city_object.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/city_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,14 +77,18 @@
     """
     if self._volume is None:
       self._volume = self.simplified_polyhedron.volume
     return self._volume
 
   @volume.setter
   def volume(self, value):
+    """
+    Set city object volume in cubic meters
+    :param value: float
+    """
     self._volume = value
 
   @property
   def detailed_polyhedron(self) -> Polyhedron:
     """
     Get city object polyhedron including details such as holes
     :return: Polyhedron
@@ -168,27 +172,26 @@
     """
     return self.simplified_polyhedron.max_z
 
   @property
   def external_temperature(self) -> {float}:
     """
     Get external temperature surrounding the city object in Celsius
-    :return: dict{DataFrame(float)}
+    :return: dict{dict{[float]}}
     """
     return self._external_temperature
 
   @external_temperature.setter
   def external_temperature(self, value):
     """
     Set external temperature surrounding the city object in Celsius
-    :param value: dict{DataFrame(float)}
+    :param value: dict{dict{[float]}}
     """
     self._external_temperature = value
 
-  # todo: this is the new format we will use to get rid of the data frames
   @property
   def ground_temperature(self) -> dict:
     """
     Get ground temperature under the city object in Celsius at different depths in meters for different time steps
     example of use: {month: {0.5: [10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10, 10]}}
     :return: dict{dict{[float]}}
     """
@@ -201,56 +204,56 @@
     :param value: dict{dict{[float]}}
     """
     self._ground_temperature = value
 
   @property
   def global_horizontal(self) -> dict:
     """
-    Get global horizontal radiation surrounding the city object in W/m2
-    :return: dict{DataFrame(float)}
+    Get global horizontal radiation surrounding the city object in J/m2
+    :return: dict{dict{[float]}}
     """
     return self._global_horizontal
 
   @global_horizontal.setter
   def global_horizontal(self, value):
     """
-    Set global horizontal radiation surrounding the city object in W/m2
-    :param value: dict{DataFrame(float)}
+    Set global horizontal radiation surrounding the city object in J/m2
+    :param value: dict{dict{[float]}}
     """
     self._global_horizontal = value
 
   @property
   def diffuse(self) -> dict:
     """
-    Get diffuse radiation surrounding the city object in W/m2
-    :return: dict{DataFrame(float)}
+    Get diffuse radiation surrounding the city object in J/m2
+    :return: dict{dict{[float]}}
     """
     return self._diffuse
 
   @diffuse.setter
   def diffuse(self, value):
     """
-    Set diffuse radiation surrounding the city object in W/m2
-    :param value: dict{DataFrame(float)}
+    Set diffuse radiation surrounding the city object in J/m2
+    :param value: dict{dict{[float]}}
     """
     self._diffuse = value
 
   @property
   def beam(self) -> dict:
     """
-    Get beam radiation surrounding the city object in W/m2
-    :return: dict{DataFrame(float)}
+    Get beam radiation surrounding the city object in J/m2
+    :return: dict{dict{[float]}}
     """
     return self._beam
 
   @beam.setter
   def beam(self, value):
     """
-    Set beam radiation surrounding the city object in W/m2
-    :param value: dict{DataFrame(float)}
+    Set beam radiation surrounding the city object in J/m2
+    :param value: dict{dict{[float]}}
     """
     self._beam = value
 
   @property
   def lower_corner(self):
     """
     Get city object lower corner coordinates [x, y, z]
```

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/city_objects_cluster.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/city_objects_cluster.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/control_system.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/control_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/distribution_system.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/distribution_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/emission_system.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/emission_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/energy_system.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/energy_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/generation_system.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/generic_distribution_system.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/generic_distribution_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,24 +65,24 @@
     """
     self._distribution_consumption_fix_flow = value
 
   @property
   def distribution_consumption_variable_flow(self):
     """
     Get distribution_consumption if the pump or fan work at variable mass or volume flow in ratio
-    over energy produced (Wh/Wh)
+    over energy produced (J/J)
     :return: float
     """
     return self._distribution_consumption_variable_flow
 
   @distribution_consumption_variable_flow.setter
   def distribution_consumption_variable_flow(self, value):
     """
     Set distribution_consumption if the pump or fan work at variable mass or volume flow in ratio
-    over energy produced (Wh/Wh)
+    over energy produced (J/J)
     :return: float
     """
     self._distribution_consumption_variable_flow = value
 
   @property
   def heat_losses(self):
     """
```

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/generic_emission_system.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/generic_emission_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/generic_energy_system.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/generic_energy_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/generic_generation_system.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/generic_generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/heat_pump.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/heat_pump.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/energy_systems/hvac_terminal_unit.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/energy_systems/hvac_terminal_unit.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/greenery/plant.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/greenery/plant.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/greenery/soil.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/greenery/soil.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/greenery/vegetation.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/greenery/vegetation.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/iot/sensor_measure.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/iot/sensor_measure.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/iot/station.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/iot/station.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/level_of_detail.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/level_of_detail.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/network.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/network.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/parts_consisting_building.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/parts_consisting_building.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/transport/connection.py` & `cerc-hub-0.1.8.3/hub/city_model_structure/building_demand/construction.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,125 +1,134 @@
 """
-Connection module
+Construction thermal parameters
 SPDX - License - Identifier: LGPL - 3.0 - or -later
-Copyright © 2022 Concordia CERC group
+Copyright © 2023 Concordia CERC group
 Project Coder Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
-Code contributors: Guille guille.gutierrezmorote@concordia.ca
 """
 
-import ast
-from typing import Union
+from hub.city_model_structure.building_demand.layer import Layer
 
-from hub.city_model_structure.attributes.edge import Edge
-from hub.city_model_structure.transport.lane import Lane
 
-
-class Connection:
+class Construction:
   """
-  Connection class
+  Construction class
   """
-
   def __init__(self):
-    self._from_edge = None
-    self._to_edge = None
-    self._from_lane = None
-    self._to_lane = None
-    self._pass = None
-    self._keep_clear = None
+    self._type = None
+    self._layers = None
+    self._window_ratio = None
+    self._window_frame_ratio = None
+    self._window_g_value = None
+    self._window_overall_u_value = None
+    self._window_type = None
+
+  @property
+  def type(self):
+    """
+    Get construction type
+    :return: str
+    """
+    return self._type
+
+  @type.setter
+  def type(self, value):
+    """
+    Set construction type
+    :param value: str
+    """
+    self._type = value
 
   @property
-  def from_edge(self) -> Edge:
+  def layers(self) -> [Layer]:
     """
-    Get "from" edge
-    :return: Edge
+    Get layers
+    :return: [layer]
     """
-    return self._from_edge
+    return self._layers
 
-  @from_edge.setter
-  def from_edge(self, value):
+  @layers.setter
+  def layers(self, value):
     """
-    Set "from" edge
-    :param value: Edge
+    Set layers
+    :param value: [layer]
     """
-    self._from_edge = value
+    self._layers = value
 
   @property
-  def to_edge(self) -> Edge:
+  def window_ratio(self):
     """
-    Get "to" edge
-    :return: Edge
+    Get window ratio
+    :return: dict
     """
-    return self._to_edge
+    return self._window_ratio
 
-  @to_edge.setter
-  def to_edge(self, value):
+  @window_ratio.setter
+  def window_ratio(self, value):
     """
-    Set "to" edge
-    :param value: Edge
+    Set window ratio
+    :param value: dict
     """
-    self._to_edge = value
+    self._window_ratio = value
 
   @property
-  def from_lane(self) -> Lane:
+  def window_frame_ratio(self):
     """
-    Get "from" lane
-    :return: Lane
+    Get window frame ratio
+    :return: float
     """
-    return self._to_lane
+    return self._window_frame_ratio
 
-  @from_lane.setter
-  def from_lane(self, value):
+  @window_frame_ratio.setter
+  def window_frame_ratio(self, value):
     """
-    Set "from" lane
-    :param value: Lane
+    Set window frame ratio
+    :param value: float
     """
-    self._from_lane = value
+    self._window_frame_ratio = value
 
   @property
-  def to_lane(self) -> Lane:
+  def window_g_value(self):
     """
-    Get "to" lane
-    :return: Lane
+    Get transparent surface g-value
+    :return: float
     """
-    return self._to_lane
+    return self._window_g_value
 
-  @to_lane.setter
-  def to_lane(self, value):
+  @window_g_value.setter
+  def window_g_value(self, value):
     """
-    Set "to" lane
-    :param value: Lane
+    Set transparent surface g-value
+    :param value: float
     """
-    self._to_lane = value
+    self._window_g_value = value
 
   @property
-  def pass_not_wait(self) -> Union[None, bool]:
+  def window_overall_u_value(self):
     """
-    Get if the vehicles which pass this (lane to lane) connection will not wait
-    :return: None or Boolean
+    Get transparent surface overall U-value in W/m2K
+    :return: float
     """
-    return self._pass
+    return self._window_overall_u_value
 
-  @pass_not_wait.setter
-  def pass_not_wait(self, value):
+  @window_overall_u_value.setter
+  def window_overall_u_value(self, value):
     """
-    Set if the vehicles which pass this (lane to lane) connection will not wait
-    :param value: Boolean
+    Set transparent surface overall U-value in W/m2K
+    :param value: float
     """
-    if value is not None:
-      self._pass = ast.literal_eval(value)
+    self._window_overall_u_value = value
 
   @property
-  def keep_clear(self) -> Union[None, bool]:
+  def window_type(self):
     """
-    Get if vehicles which pass this (lane to lane) connection should keep the intersection clear
-    :return: None or Boolean
+    Get transparent surface type, 'window' or 'skylight'
+    :return: str
     """
-    return self._keep_clear
+    return self._window_type
 
-  @keep_clear.setter
-  def keep_clear(self, value):
+  @window_type.setter
+  def window_type(self, value):
     """
-    Set if vehicles which pass this (lane to lane) connection should keep the intersection clear
-    :param value: Boolean
+    Set transparent surface type, 'window' or 'skylight'
+    :return: str
     """
-    if value is not None:
-      self._keep_clear = ast.literal_eval(value)
+    self._window_type = value
```

### Comparing `cerc-hub-0.1.8.2/hub/city_model_structure/transport/origin_destination_node.py` & `cerc-hub-0.1.8.3/hub/exports/exports_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,73 @@
 """
-Origin-Destination node module
+ExportsFactory export a city into several formats
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2022 Concordia CERC group
-Project Coder Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
+Project Coder Guille Gutierrez guillermo.gutierrezmorote@concordia.ca
 """
-from typing import List, TypeVar
 
-from hub.city_model_structure.attributes.node import Node
-from hub.city_model_structure.attributes.point import Point
-from hub.city_model_structure.attributes.polygon import Polygon
-from hub.city_model_structure.city_object import CityObject
+from pathlib import Path
 
-OriginDestinationEdge = TypeVar('OriginDestinationEdge')
+from hub.exports.formats.obj import Obj
+from hub.exports.formats.simplified_radiosity_algorithm import SimplifiedRadiosityAlgorithm
+from hub.exports.formats.stl import Stl
+from hub.helpers.utils import validate_import_export_type
 
 
-class OriginDestinationNode(Node):
+class ExportsFactory:
   """
-  OriginDestinationNode class
+  Exports factory class
   """
-
-  def __init__(self, name, coordinates, node_type='OriginDestinationNode', edges=None, polygon=None):
-    super().__init__(name, edges)
-    self._coordinates = coordinates
-    self._node_type = node_type
-    self._polygon = polygon
-    self._land_use_types = None
-    self._city_objects = None
+  def __init__(self, handler, city, path, target_buildings=None, adjacent_buildings=None):
+    self._city = city
+    self._handler = '_' + handler.lower()
+    validate_import_export_type(ExportsFactory, handler)
+    if isinstance(path, str):
+      path = Path(path)
+    self._path = path
+    self._target_buildings = target_buildings
+    self._adjacent_buildings = adjacent_buildings
 
   @property
-  def node_type(self):
+  def _citygml(self):
     """
-    Get node type
-    :return: str
+    Export to citygml
+    :return: None
     """
-    return self._node_type
+    raise NotImplementedError
 
   @property
-  def coordinates(self) -> Point:
-    """
-    Get node coordinates
-    :return: Point
-    """
-    return self._coordinates
-
-  @coordinates.setter
-  def coordinates(self, value):
-    """
-    Set node coordinates
-    :param value: Point
-    """
-    self._coordinates = value
+  def _collada(self):
+    raise NotImplementedError
 
   @property
-  def edges(self) -> List[OriginDestinationEdge]:
+  def _stl(self):
     """
-    get edges delimited by the node
-    :return: [OriginDestinationEdge]
+    Export the city geometry to stl
+    :return: None
     """
-    return self._edges
+    return Stl(self._city, self._path)
 
   @property
-  def polygon(self) -> Polygon:
+  def _obj(self):
     """
-    Get node polygon that defines the zone represented by the node
-    :return: Polygon
+    Export the city geometry to obj
+    :return: None
     """
-    return self._polygon
+    return Obj(self._city, self._path)
 
   @property
-  def land_use_types(self) -> dict:
+  def _sra(self):
     """
-    Get land use types inside the node polygon. It returns a dictionary with the types of land use together with the
-    percentage of the land that corresponds to each type
-    :return: {string : float}
+    Export the city to Simplified Radiosity Algorithm xml format
+    :return: None
     """
-    return self._land_use_types
+    return SimplifiedRadiosityAlgorithm(self._city,
+                                        (self._path / f'{self._city.name}_sra.xml'),
+                                        target_buildings=self._target_buildings)
 
-  @property
-  def city_objects(self) -> List[CityObject]:
+  def export(self):
     """
-    Get the list of city objects place inside the zone
-    :return: List[CityObject]
+    Export the city given to the class using the given export type handler
+    :return: None
     """
-    return self._city_objects
+    return getattr(self, self._handler, lambda: None)
```

### Comparing `cerc-hub-0.1.8.2/hub/config/configuration.ini` & `cerc-hub-0.1.8.3/hub/config/configuration.ini`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/construction/eilat_archetypes.json` & `cerc-hub-0.1.8.3/hub/data/construction/eilat_archetypes.json`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/construction/eilat_constructions.json` & `cerc-hub-0.1.8.3/hub/data/construction/eilat_constructions.json`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/construction/nrcan_archetypes.json` & `cerc-hub-0.1.8.3/hub/data/construction/nrcan_archetypes.json`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/construction/nrcan_constructions.json` & `cerc-hub-0.1.8.3/hub/data/construction/nrcan_constructions.json`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/construction/us_archetypes.xml` & `cerc-hub-0.1.8.3/hub/data/construction/us_archetypes.xml`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/construction/us_constructions.xml` & `cerc-hub-0.1.8.3/hub/data/construction/us_constructions.xml`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/costs/montreal_costs.xml` & `cerc-hub-0.1.8.3/hub/data/costs/montreal_costs.xml`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/customized_imports/ashrae_archetypes.xml` & `cerc-hub-0.1.8.3/hub/data/customized_imports/ashrae_archetypes.xml`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/air_source.xlsx` & `cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/air_source.xlsx`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/as_parallel.txt` & `cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/as_parallel.txt`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/as_series.txt` & `cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/as_series.txt`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/demand.txt` & `cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/demand.txt`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/w2w_parallel.txt` & `cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/w2w_parallel.txt`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/w2w_series.txt` & `cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/w2w_series.txt`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/water_to_water.xlsx` & `cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/water_to_water.xlsx`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/energy_systems/heat_pumps/wt_hourly3.txt` & `cerc-hub-0.1.8.3/hub/data/energy_systems/heat_pumps/wt_hourly3.txt`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/energy_systems/montreal_custom_systems.xml` & `cerc-hub-0.1.8.3/hub/data/energy_systems/montreal_custom_systems.xml`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/geolocation/admin2Codes.txt` & `cerc-hub-0.1.8.3/hub/data/geolocation/admin2Codes.txt`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/geolocation/cities15000.txt` & `cerc-hub-0.1.8.3/hub/data/geolocation/cities15000.txt`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/greenery/ecore_greenery_catalog.xml` & `cerc-hub-0.1.8.3/hub/data/greenery/ecore_greenery_catalog.xml`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/usage/comnet_archetypes.xlsx` & `cerc-hub-0.1.8.3/hub/data/usage/comnet_archetypes.xlsx`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/usage/comnet_schedules_archetypes.xlsx` & `cerc-hub-0.1.8.3/hub/data/usage/comnet_schedules_archetypes.xlsx`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/usage/eilat_archetypes.xlsx` & `cerc-hub-0.1.8.3/hub/data/usage/eilat_archetypes.xlsx`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/usage/eilat_schedules_archetypes.xlsx` & `cerc-hub-0.1.8.3/hub/data/usage/eilat_schedules_archetypes.xlsx`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/data/weather/epw/CAN_PQ_Montreal.Intl.AP.716270_CWEC.epw` & `cerc-hub-0.1.8.3/hub/data/weather/epw/CAN_PQ_Montreal.Intl.AP.716270_CWEC.epw`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/exports/building_energy/energy_ade.py` & `cerc-hub-0.1.8.3/hub/exports/building_energy/energy_ade.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,15 @@
 
     building_dic['bldg:Building']['gml:boundedBy'] = boundaries
     return building_dic
 
   def _thermal_zones(self, building, city):
     thermal_zones = []
     for internal_zone in building.internal_zones:
-      for index, thermal_zone in enumerate(internal_zone.thermal_zones):
+      for index, thermal_zone in enumerate(internal_zone.thermal_zones_from_internal_zones):
         usages = []
         for usage in internal_zone.usages:
           usages.append({'@xlink:href': f'#GML_{usage.id}'})
         thermal_zone_dic = {
           'energy:ThermalZone': {
             '@gml:id': f'GML_{thermal_zone.id}',
             'gml:name': f'Thermal zone {index} in {building.name} building',
```

### Comparing `cerc-hub-0.1.8.2/hub/exports/building_energy/idf.py` & `cerc-hub-0.1.8.3/hub/exports/building_energy/idf.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,15 +391,17 @@
                            Heating_Availability_Schedule_Name=f'HVAC AVAIL SCHEDULES {thermal_zone.usage_name}',
                            Cooling_Availability_Schedule_Name=f'HVAC AVAIL SCHEDULES {thermal_zone.usage_name}',
                            Template_Thermostat_Name=thermostat.Name)
 
   def _add_occupancy(self, thermal_zone, zone_name):
     number_of_people = thermal_zone.occupancy.occupancy_density * thermal_zone.total_floor_area
     fraction_radiant = 0
-    total_sensible = thermal_zone.occupancy.sensible_radiative_internal_gain + thermal_zone.occupancy.sensible_convective_internal_gain
+    total_sensible = (
+      thermal_zone.occupancy.sensible_radiative_internal_gain + thermal_zone.occupancy.sensible_convective_internal_gain
+    )
     if total_sensible != 0:
       fraction_radiant = thermal_zone.occupancy.sensible_radiative_internal_gain / total_sensible
 
     self._idf.newidfobject(self._PEOPLE,
                            Name=f'{zone_name}_occupancy',
                            Zone_or_ZoneList_Name=zone_name,
                            Number_of_People_Schedule_Name=f'Occupancy schedules {thermal_zone.usage_name}',
@@ -444,30 +446,32 @@
                            Fraction_Latent=fraction_latent,
                            Fraction_Radiant=fraction_radiant,
                            EndUse_Subcategory=subcategory
                            )
 
   def _add_infiltration(self, thermal_zone, zone_name):
     schedule = f'Infiltration schedules {thermal_zone.usage_name}'
+    _infiltration = thermal_zone.infiltration_rate_system_off * cte.HOUR_TO_SECONDS
     self._idf.newidfobject(self._INFILTRATION,
                            Name=f'{zone_name}_infiltration',
                            Zone_or_ZoneList_Name=zone_name,
                            Schedule_Name=schedule,
                            Design_Flow_Rate_Calculation_Method='AirChanges/Hour',
-                           Air_Changes_per_Hour=thermal_zone.infiltration_rate_system_off
+                           Air_Changes_per_Hour=_infiltration
                            )
 
   def _add_ventilation(self, thermal_zone, zone_name):
     schedule = f'Ventilation schedules {thermal_zone.usage_name}'
+    _air_change = thermal_zone.mechanical_air_change * cte.HOUR_TO_SECONDS
     self._idf.newidfobject(self._VENTILATION,
                            Name=f'{zone_name}_ventilation',
                            Zone_or_ZoneList_Name=zone_name,
                            Schedule_Name=schedule,
                            Design_Flow_Rate_Calculation_Method='AirChanges/Hour',
-                           Air_Changes_per_Hour=thermal_zone.mechanical_air_change
+                           Air_Changes_per_Hour=_air_change
                            )
 
   def _add_dhw(self, thermal_zone, zone_name):
     peak_flow_rate = thermal_zone.domestic_hot_water.peak_flow * thermal_zone.total_floor_area
     self._idf.newidfobject(self._DHW,
                            Name=f'DHW {zone_name}',
                            Peak_Flow_Rate=peak_flow_rate,
@@ -506,17 +510,17 @@
     self._remove_location()
     self._remove_sizing_periods()
     self._rename_building(self._city.name)
     self._lod = self._city.level_of_detail.geometry
     for building in self._city.buildings:
       print('building name', building.name)
       for internal_zone in building.internal_zones:
-        if internal_zone.thermal_zones is None:
+        if internal_zone.thermal_zones_from_internal_zones is None:
           continue
-        for thermal_zone in internal_zone.thermal_zones:
+        for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
           for thermal_boundary in thermal_zone.thermal_boundaries:
             self._add_construction(thermal_boundary)
             if thermal_boundary.parent_surface.vegetation is not None:
               self._add_vegetation_material(thermal_boundary.parent_surface.vegetation)
             for thermal_opening in thermal_boundary.thermal_openings:
               self._add_window_construction_and_material(thermal_opening)
           usage = thermal_zone.usage_name
@@ -529,15 +533,15 @@
             self._add_schedules(usage, 'HVAC AVAIL', thermal_zone.thermal_control.hvac_availability_schedules)
             self._add_schedules(usage, 'Heating thermostat', thermal_zone.thermal_control.heating_set_point_schedules)
             self._add_schedules(usage, 'Cooling thermostat', thermal_zone.thermal_control.cooling_set_point_schedules)
             self._add_schedules(usage, 'Lighting', thermal_zone.lighting.schedules)
             self._add_schedules(usage, 'Appliance', thermal_zone.appliances.schedules)
             self._add_schedules(usage, 'DHW_prof', thermal_zone.domestic_hot_water.schedules)
             _new_schedules = self._create_yearly_values_schedules('cold_temp',
-                                                                  building.cold_water_temperature[cte.HOUR]['epw'])
+                                                                  building.cold_water_temperature[cte.HOUR])
             self._add_schedules(building.name, 'cold_temp', _new_schedules)
             value = thermal_zone.domestic_hot_water.service_temperature
             _new_schedules = self._create_constant_value_schedules('DHW_temp', value)
             self._add_schedules(usage, 'DHW_temp', _new_schedules)
             _occ = thermal_zone.occupancy
             if _occ.occupancy_density == 0:
               _total_heat = 0
@@ -552,15 +556,15 @@
             self._add_ventilation(thermal_zone, building.name)
             self._add_occupancy(thermal_zone, building.name)
             self._add_lighting(thermal_zone, building.name)
             self._add_appliances(thermal_zone, building.name)
             self._add_dhw(thermal_zone, building.name)
       if self._export_type == "Surfaces":
         if building.name in self._target_buildings or building.name in self._adjacent_buildings:
-          if building.internal_zones[0].thermal_zones is not None:
+          if building.internal_zones[0].thermal_zones_from_internal_zones is not None:
             self._add_surfaces(building, building.name)
           else:
             self._add_pure_geometry(building, building.name)
         else:
           self._add_shading(building)
       else:
         self._add_block(building)
@@ -607,15 +611,15 @@
 
   def _add_block(self, building):
     _points = self._matrix_to_2d_list(building.foot_print.coordinates)
     self._idf.add_block(name=building.name, coordinates=_points, height=building.max_height,
                         num_stories=int(building.storeys_above_ground))
 
     for surface in self._idf.idfobjects[self._SURFACE]:
-      for thermal_zone in building.thermal_zones:
+      for thermal_zone in building.thermal_zones_from_internal_zones:
         for boundary in thermal_zone.thermal_boundaries:
           if surface.Type == self.idf_surfaces[boundary.surface.type]:
             surface.Construction_Name = boundary.construction_name
             break
         for usage in thermal_zone.usages:
           surface.Zone_Name = usage.id
           break
@@ -660,25 +664,25 @@
       idf_surface = self._idf.newidfobject(self._SURFACE, **_kwargs)
 
       coordinates = self._matrix_to_list(surface.solid_polygon.coordinates,
                                          self._city.lower_corner)
       idf_surface.setcoords(coordinates)
     if self._lod >= 3:
       for internal_zone in building.internal_zones:
-        for thermal_zone in internal_zone.thermal_zones:
+        for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
           for boundary in thermal_zone.thermal_boundaries:
             self._add_windows_by_vertices(boundary)
     else:
       # idf only allows setting wwr for external walls
       wwr = 0
       self._idf.set_wwr(wwr)
 
   def _add_surfaces(self, building, zone_name):
     for internal_zone in building.internal_zones:
-      for thermal_zone in internal_zone.thermal_zones:
+      for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
         for boundary in thermal_zone.thermal_boundaries:
           idf_surface_type = self.idf_surfaces[boundary.parent_surface.type]
           outside_boundary_condition = 'Outdoors'
           sun_exposure = 'SunExposed'
           wind_exposure = 'WindExposed'
           _kwargs = {'Name': f'{boundary.parent_surface.name}',
                      'Surface_Type': idf_surface_type,
@@ -707,15 +711,15 @@
 
           coordinates = self._matrix_to_list(boundary.parent_surface.solid_polygon.coordinates,
                                              self._city.lower_corner)
           surface.setcoords(coordinates)
 
     if self._lod >= 3:
       for internal_zone in building.internal_zones:
-        for thermal_zone in internal_zone.thermal_zones:
+        for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
           for boundary in thermal_zone.thermal_boundaries:
             self._add_windows_by_vertices(boundary)
     else:
       # idf only allows setting wwr for external walls
       wwr = 0
       for surface in building.surfaces:
         if surface.type == cte.WALL:
```

### Comparing `cerc-hub-0.1.8.2/hub/exports/building_energy/idf_files/Energy+.idd` & `cerc-hub-0.1.8.3/hub/exports/building_energy/idf_files/Energy+.idd`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/exports/building_energy/idf_files/Minimal.idf` & `cerc-hub-0.1.8.3/hub/exports/building_energy/idf_files/Minimal.idf`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/exports/building_energy/insel/insel_monthly_energy_balance.py` & `cerc-hub-0.1.8.3/hub/exports/building_energy/insel/insel_monthly_energy_balance.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,33 +26,31 @@
 _NUMBER_DAYS_PER_MONTH = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
 
 
 class InselMonthlyEnergyBalance:
   """
   Insel monthly energy balance class
   """
-  def __init__(self, city, path, custom_insel_block, radiation_calculation_method='sra', weather_format='epw'):
+  def __init__(self, city, path, custom_insel_block):
     self._city = city
     self._path = path
     self._custom_insel_block = custom_insel_block
     self._results = None
-    self._radiation_calculation_method = radiation_calculation_method
-    self._weather_format = weather_format
     self._contents = []
     self._insel_files_paths = []
     self._sanity_check()
     for building in city.buildings:
       self._insel_files_paths.append(building.name + '.insel')
       file_name_out = building.name + '.out'
       output_path = Path(self._path / file_name_out).resolve()
-      if building.thermal_zones is None:
+      if building.thermal_zones_from_internal_zones is None:
         logging.warning('Building %s has missing values. Monthly Energy Balance cannot be processed', building.name)
 
       self._contents.append(
-        self._generate_meb_template(building, output_path, self._radiation_calculation_method, self._weather_format, self._custom_insel_block)
+        self._generate_meb_template(building, output_path, self._custom_insel_block)
       )
     self._export()
 
   @staticmethod
   def _add_block(file, block_number, block_type, inputs=None, parameters=None):
     file += "S " + str(block_number) + " " + block_type + "\n"
     if inputs is not None:
@@ -92,15 +90,15 @@
     if levels_of_detail.surface_radiation is None:
       raise AttributeError('Level of detail of surface radiation not assigned')
     if levels_of_detail.surface_radiation < 1:
       raise AttributeError(f'Level of detail of surface radiation = {levels_of_detail.surface_radiation}. '
                            f'Required minimum level 1')
 
   @staticmethod
-  def _generate_meb_template(building, insel_outputs_path, radiation_calculation_method, weather_format, custom_insel_block):
+  def _generate_meb_template(building, insel_outputs_path, custom_insel_block):
     file = ""
     i_block = 1
     parameters = ["1", "12", "1"]
     file = InselMonthlyEnergyBalance._add_block(file, i_block, 'DO', parameters=parameters)
 
     i_block = 4
     inputs = ["1.1", "20.1", "21.1"]
@@ -122,37 +120,37 @@
                   f'{number_of_storeys} % BP(3) Number of storeys above ground',
                   f'{attic_heated} % BP(4) Attic heating type (0=no room, 1=unheated, 2=heated)',
                   f'{basement_heated} % BP(5) Cellar heating type (0=no room, 1=unheated, 2=heated, '
                   f'99=invalid)']
 
     # todo: this method and the insel model have to be reviewed for more than one internal zone
     internal_zone = building.internal_zones[0]
-    thermal_zone = internal_zone.thermal_zones[0]
+    thermal_zone = internal_zone.thermal_zones_from_internal_zones[0]
     parameters.append(f'{thermal_zone.indirectly_heated_area_ratio} % BP(6) Indirectly heated area ratio')
     parameters.append(f'{thermal_zone.effective_thermal_capacity / 3600 / building.average_storey_height}'
                       f' % BP(7) Effective heat capacity (Wh/m2K)')
     parameters.append(f'{thermal_zone.additional_thermal_bridge_u_value} '
                       f'% BP(8) Additional U-value for heat bridge (W/m2K)')
     parameters.append('1 % BP(9) Usage type (0=standard, 1=IWU)')
 
     # ZONES AND SURFACES
     parameters.append(f'{len(internal_zone.usages)} %  BP(10) Number of zones')
 
     for i, usage in enumerate(internal_zone.usages):
       percentage_usage = usage.percentage
-      parameters.append(f'{internal_zone.thermal_zones[0].total_floor_area * percentage_usage} '
+      parameters.append(f'{internal_zone.thermal_zones_from_internal_zones[0].total_floor_area * percentage_usage} '
                         f'% BP(11) #1 Area of zone {i + 1} (m2)')
       total_internal_gain = 0
       for i_gain in usage.internal_gains:
         internal_gain = i_gain.average_internal_gain * (i_gain.convective_fraction + i_gain.radiative_fraction)
         for schedule in i_gain.schedules:
           total_values = sum(schedule.values)
           total_hours = 0
           for day_type in schedule.day_types:
-            total_hours += cte.DAYS_A_YEAR[day_type] / 365 / 24
+            total_hours += cte.WEEK_DAYS_A_YEAR[day_type] / 365 / 24
           total_values *= total_hours
           total_internal_gain += internal_gain * total_values
 
       parameters.append(f'{total_internal_gain} % BP(12) #2 Internal gains of zone {i + 1}')
       parameters.append(f'{usage.thermal_control.mean_heating_set_point} % BP(13) #3 Heating setpoint temperature '
                         f'zone {i + 1} (degree Celsius)')
       parameters.append(f'{usage.thermal_control.heating_set_back} % BP(14) #4 Heating setback temperature '
@@ -165,28 +163,28 @@
       ventilation = 0
       infiltration = 0
       for schedule in usage.thermal_control.hvac_availability_schedules:
         ventilation_day = 0
         infiltration_day = 0
         for value in schedule.values:
           if value == 0:
-            infiltration_day += internal_zone.thermal_zones[0].infiltration_rate_system_off / 24
+            infiltration_day += internal_zone.thermal_zones_from_internal_zones[0].infiltration_rate_system_off / 24 * cte.HOUR_TO_SECONDS
             ventilation_day += 0
           else:
-            ventilation_value = usage.mechanical_air_change * value
-            infiltration_value = internal_zone.thermal_zones[0].infiltration_rate_system_off * value
+            ventilation_value = usage.mechanical_air_change * value * cte.HOUR_TO_SECONDS
+            infiltration_value = internal_zone.thermal_zones_from_internal_zones[0].infiltration_rate_system_off * value * cte.HOUR_TO_SECONDS
             if ventilation_value >= infiltration_value:
               ventilation_day += ventilation_value / 24
               infiltration_day += 0
             else:
               ventilation_day += 0
               infiltration_day += infiltration_value / 24
         for day_type in schedule.day_types:
-          infiltration += infiltration_day * cte.DAYS_A_YEAR[day_type] / 365
-          ventilation += ventilation_day * cte.DAYS_A_YEAR[day_type] / 365
+          infiltration += infiltration_day * cte.WEEK_DAYS_A_YEAR[day_type] / 365
+          ventilation += ventilation_day * cte.WEEK_DAYS_A_YEAR[day_type] / 365
 
       ventilation_infiltration = ventilation + infiltration
       parameters.append(f'{ventilation_infiltration} % BP(18) #8 Minimum air change rate zone {i + 1} (ACH)')
 
     parameters.append(f'{len(thermal_zone.thermal_boundaries)}  % Number of surfaces = BP(11+8z) \n'
                       f'% 1. Surface type (1=wall, 2=ground 3=roof, 4=flat roof)\n'
                       f'% 2. Areas above ground (m2)\n'
@@ -223,54 +221,52 @@
         parameters.append(0.0)
       else:
         thermal_opening = thermal_boundary.thermal_openings[0]
         parameters.append(thermal_opening.frame_ratio)
         parameters.append(thermal_opening.overall_u_value)
         parameters.append(thermal_opening.g_value)
       if thermal_boundary.type is not cte.GROUND:
-        parameters.append(thermal_boundary.parent_surface.short_wave_reflectance)
+        parameters.append(thermal_boundary.external_surface.short_wave_reflectance)
       else:
         parameters.append(0.0)
-
     file = InselMonthlyEnergyBalance._add_block(file, i_block, custom_insel_block, inputs=inputs, parameters=parameters)
 
     i_block = 20
     inputs = ['1']
     parameters = ['12 % Monthly ambient temperature (degree Celsius)']
 
     external_temperature = building.external_temperature[cte.MONTH]
-
     for i in range(0, len(external_temperature)):
-      parameters.append(f'{i + 1} {external_temperature.at[i, weather_format]}')
+      parameters.append(f'{i + 1} {external_temperature[i]}')
 
     file = InselMonthlyEnergyBalance._add_block(file, i_block, 'polyg', inputs=inputs, parameters=parameters)
 
     i_block = 21
     inputs = ['1']
     parameters = ['12 % Monthly sky temperature']
 
-    sky_temperature = Weather.sky_temperature(external_temperature[[weather_format]].to_numpy().T[0])
+    sky_temperature = Weather.sky_temperature(external_temperature)
     for i, temperature in enumerate(sky_temperature):
       parameters.append(f'{i + 1} {temperature}')
 
     file = InselMonthlyEnergyBalance._add_block(file, i_block, 'polyg', inputs=inputs, parameters=parameters)
-
     for i, surface in enumerate(surfaces):
       i_block = 101 + i
       inputs = ['1 % Monthly surface radiation (W/m2)']
       parameters = [f'12 % Azimuth {np.rad2deg(surface.azimuth)}, '
                     f'inclination {np.rad2deg(surface.inclination)} (degrees)']
 
       if surface.type != 'Ground':
         if cte.MONTH not in surface.global_irradiance:
           raise ValueError(f'surface: {surface.name} from building {building.name} has no global irradiance!')
+
         global_irradiance = surface.global_irradiance[cte.MONTH]
         for j in range(0, len(global_irradiance)):
           parameters.append(f'{j + 1} '
-                            f'{global_irradiance.at[j, radiation_calculation_method] / 24 / _NUMBER_DAYS_PER_MONTH[j]}')
+                            f'{global_irradiance[j] * cte.WATTS_HOUR_TO_JULES / 24 / _NUMBER_DAYS_PER_MONTH[j]}')
       else:
         for j in range(0, 12):
           parameters.append(f'{j + 1} 0.0')
 
       file = InselMonthlyEnergyBalance._add_block(file, i_block, 'polyg', inputs=inputs, parameters=parameters)
 
     i_block = 300 + len(surfaces)
@@ -286,9 +282,8 @@
     i_block = 310 + len(surfaces)
     inputs = ['4.1', '4.2']
     parameters = ['1 % Mode',
                   '0 % Suppress FNQ inputs',
                   f"'{str(insel_outputs_path)}' % File name",
                   "'*' % Fortran format"]
     file = InselMonthlyEnergyBalance._add_block(file, i_block, 'WRITE', inputs=inputs, parameters=parameters)
-
     return file
```

### Comparing `cerc-hub-0.1.8.2/hub/exports/energy_building_exports_factory.py` & `cerc-hub-0.1.8.3/hub/exports/energy_building_exports_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/exports/energy_systems/air_source_hp_export.py` & `cerc-hub-0.1.8.3/hub/exports/energy_systems/air_source_hp_export.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/exports/energy_systems/heat_pump_export.py` & `cerc-hub-0.1.8.3/hub/exports/energy_systems/heat_pump_export.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/exports/energy_systems/water_to_water_hp_export.py` & `cerc-hub-0.1.8.3/hub/exports/energy_systems/water_to_water_hp_export.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/exports/energy_systems_factory.py` & `cerc-hub-0.1.8.3/hub/exports/energy_systems_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/exports/formats/obj.py` & `cerc-hub-0.1.8.3/hub/exports/formats/obj.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/exports/formats/simplified_radiosity_algorithm.py` & `cerc-hub-0.1.8.3/hub/exports/formats/simplified_radiosity_algorithm.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,16 +62,17 @@
       for day in range(1, days_in_month[month - 1] + 1):
         for hour in range(1, 25):
           if month == 1:
             i = 24 * (day - 1) + hour - 1
           else:
             i = (total_days + day - 1) * 24 + hour - 1
           representative_building = self._city.buildings[0]
-          content += f'{day}  {month}  {hour}  {representative_building.global_horizontal[cte.HOUR].epw[i]}  ' \
-                     f'{representative_building.beam[cte.HOUR].epw[i]}\n'
+          _global = representative_building.global_horizontal[cte.HOUR][i] * cte.WATTS_HOUR_TO_JULES
+          _beam = representative_building.beam[cte.HOUR][i] * cte.WATTS_HOUR_TO_JULES
+          content += f'{day}  {month}  {hour}  {_global}  {_beam}\n'
     with open(file, 'w', encoding='utf-8') as file:
       file.write(content)
 
   def _export_sra_xml(self):
     buildings = []
     for building_index, building in enumerate(self._city.buildings):
       if self._target_buildings is None:
```

### Comparing `cerc-hub-0.1.8.2/hub/exports/formats/triangular.py` & `cerc-hub-0.1.8.3/hub/exports/formats/triangular.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/auth.py` & `cerc-hub-0.1.8.3/hub/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/configuration_helper.py` & `cerc-hub-0.1.8.3/hub/helpers/configuration_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/constants.py` & `cerc-hub-0.1.8.3/hub/helpers/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # converters
 HOUR_TO_MINUTES = 60
 MINUTES_TO_SECONDS = 60
 HOUR_TO_SECONDS = 3600
 METERS_TO_FEET = 3.28084
 BTU_H_TO_WATTS = 0.29307107
 KILO_WATTS_HOUR_TO_JULES = 3600000
+WATTS_HOUR_TO_JULES = 3600
 GALLONS_TO_QUBIC_METERS = 0.0037854117954011185
 
 # time
 SECOND = 'second'
 MINUTE = 'minute'
 HOUR = 'hour'
 DAY = 'day'
@@ -44,31 +45,44 @@
 HOLIDAY = 'holiday'
 WINTER_DESIGN_DAY = 'winter_design_day'
 SUMMER_DESIGN_DAY = 'summer_design_day'
 WEEK_DAYS = 'Weekdays'
 WEEK_ENDS = 'Weekends'
 ALL_DAYS = 'Alldays'
 
-DAYS_A_MONTH = {'monday': [5, 4, 4, 5, 4, 4, 5, 4, 4, 5, 4, 5],
-                'tuesday': [5, 4, 4, 4, 5, 4, 5, 4, 4, 5, 4, 4],
-                'wednesday': [5, 4, 4, 4, 5, 4, 4, 5, 4, 5, 4, 4],
-                'thursday': [4, 4, 5, 4, 5, 4, 4, 5, 4, 4, 5, 4],
-                'friday': [4, 4, 5, 4, 4, 5, 4, 5, 4, 4, 5, 4],
-                'saturday': [4, 4, 5, 4, 4, 5, 4, 4, 5, 4, 4, 5],
-                'sunday': [4, 4, 4, 5, 4, 4, 5, 4, 5, 4, 4, 5],
-                'holiday': [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]}
-
-DAYS_A_YEAR = {'monday': 51,
-               'tuesday': 50,
-               'wednesday': 50,
-               'thursday': 50,
-               'friday': 50,
-               'saturday': 52,
-               'sunday': 52,
-               'holiday': 10}
+WEEK_DAYS_A_MONTH = {'monday': [5, 4, 4, 5, 4, 4, 5, 4, 4, 5, 4, 5],
+                     'tuesday': [5, 4, 4, 4, 5, 4, 5, 4, 4, 5, 4, 4],
+                     'wednesday': [5, 4, 4, 4, 5, 4, 4, 5, 4, 5, 4, 4],
+                     'thursday': [4, 4, 5, 4, 5, 4, 4, 5, 4, 4, 5, 4],
+                     'friday': [4, 4, 5, 4, 4, 5, 4, 5, 4, 4, 5, 4],
+                     'saturday': [4, 4, 5, 4, 4, 5, 4, 4, 5, 4, 4, 5],
+                     'sunday': [4, 4, 4, 5, 4, 4, 5, 4, 5, 4, 4, 5],
+                     'holiday': [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]}
+
+WEEK_DAYS_A_YEAR = {'monday': 51,
+                    'tuesday': 50,
+                    'wednesday': 50,
+                    'thursday': 50,
+                    'friday': 50,
+                    'saturday': 52,
+                    'sunday': 52,
+                    'holiday': 10}
+
+DAYS_A_MONTH = {'January': 31,
+                'February': 28,
+                'March': 31,
+                'April': 30,
+                'May': 31,
+                'June': 30,
+                'July': 31,
+                'August': 31,
+                'September': 30,
+                'October': 31,
+                'November': 30,
+                'December': 31}
 
 # data types
 ANY_NUMBER = 'any_number'
 FRACTION = 'fraction'
 ON_OFF = 'on_off'
 TEMPERATURE = 'temperature'
 HUMIDITY = 'humidity'
```

### Comparing `cerc-hub-0.1.8.2/hub/helpers/data/alkis_function_to_hub_function.py` & `cerc-hub-0.1.8.3/hub/helpers/data/alkis_function_to_hub_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/data/eilat_function_to_hub_function.py` & `cerc-hub-0.1.8.3/hub/helpers/data/eilat_function_to_hub_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/data/hft_function_to_hub_function.py` & `cerc-hub-0.1.8.3/hub/helpers/data/hft_function_to_hub_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/data/hub_function_to_eilat_construction_function.py` & `cerc-hub-0.1.8.3/hub/helpers/data/hub_function_to_eilat_construction_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/data/hub_function_to_montreal_custom_costs_function.py` & `cerc-hub-0.1.8.3/hub/helpers/data/hub_function_to_montreal_custom_costs_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/data/hub_function_to_nrcan_construction_function.py` & `cerc-hub-0.1.8.3/hub/helpers/data/hub_function_to_nrcan_construction_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/data/hub_function_to_nrel_construction_function.py` & `cerc-hub-0.1.8.3/hub/helpers/data/hub_function_to_nrel_construction_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/data/hub_usage_to_comnet_usage.py` & `cerc-hub-0.1.8.3/hub/helpers/data/hub_usage_to_comnet_usage.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/data/hub_usage_to_eilat_usage.py` & `cerc-hub-0.1.8.3/hub/helpers/data/hub_usage_to_eilat_usage.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/data/hub_usage_to_hft_usage.py` & `cerc-hub-0.1.8.3/hub/helpers/data/hub_usage_to_hft_usage.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/data/hub_usage_to_nrcan_usage.py` & `cerc-hub-0.1.8.3/hub/helpers/data/hub_usage_to_nrcan_usage.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/data/montreal_custom_fuel_to_hub_fuel.py` & `cerc-hub-0.1.8.3/hub/helpers/data/montreal_custom_fuel_to_hub_fuel.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/data/montreal_demand_type_to_hub_energy_demand_type.py` & `cerc-hub-0.1.8.3/hub/helpers/data/montreal_demand_type_to_hub_energy_demand_type.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/data/montreal_system_to_hub_energy_generation_system.py` & `cerc-hub-0.1.8.3/hub/helpers/data/montreal_system_to_hub_energy_generation_system.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/data/pluto_function_to_hub_function.py` & `cerc-hub-0.1.8.3/hub/helpers/data/pluto_function_to_hub_function.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/dictionaries.py` & `cerc-hub-0.1.8.3/hub/helpers/dictionaries.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/geometry_helper.py` & `cerc-hub-0.1.8.3/hub/helpers/geometry_helper.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/location.py` & `cerc-hub-0.1.8.3/hub/helpers/location.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/helpers/peak_calculation/loads_calculation.py` & `cerc-hub-0.1.8.3/hub/helpers/peak_calculation/loads_calculation.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,108 +42,107 @@
     return load_transmitted
 
   @staticmethod
   def _get_load_ventilation(thermal_zone, internal_temperature, ambient_temperature):
     load_renovation_sensible = 0
     for usage in thermal_zone.usages:
       load_renovation_sensible += cte.AIR_DENSITY * cte.AIR_HEAT_CAPACITY * usage.mechanical_air_change \
-                                  * thermal_zone.volume / cte.HOUR_TO_MINUTES / cte.MINUTES_TO_SECONDS \
-                                  * (internal_temperature - ambient_temperature)
+                                  * thermal_zone.volume * (internal_temperature - ambient_temperature)
 
     load_infiltration_sensible = (
-        cte.AIR_DENSITY * cte.AIR_HEAT_CAPACITY * thermal_zone.infiltration_rate_system_off * thermal_zone.volume /
-        cte.HOUR_TO_MINUTES / cte.MINUTES_TO_SECONDS * (internal_temperature - ambient_temperature)
+        cte.AIR_DENSITY * cte.AIR_HEAT_CAPACITY * thermal_zone.infiltration_rate_system_off * thermal_zone.volume
+        * (internal_temperature - ambient_temperature)
     )
 
     load_ventilation = load_renovation_sensible + load_infiltration_sensible
 
     return load_ventilation
 
   def get_heating_transmitted_load(self, ambient_temperature, ground_temperature):
     """
     Calculates the heating transmitted load
     :return: int
     """
     heating_load_transmitted = 0
     for internal_zone in self._building.internal_zones:
-      for thermal_zone in internal_zone.thermal_zones:
+      for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
         internal_temperature = thermal_zone.thermal_control.mean_heating_set_point
         heating_load_transmitted += self._get_load_transmitted(thermal_zone, internal_temperature, ambient_temperature,
                                                                ground_temperature)
     return heating_load_transmitted
 
   def get_cooling_transmitted_load(self, ambient_temperature, ground_temperature):
     """
     Calculates the cooling transmitted load
     :return: int
     """
     cooling_load_transmitted = 0
     for internal_zone in self._building.internal_zones:
-      for thermal_zone in internal_zone.thermal_zones:
+      for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
         internal_temperature = thermal_zone.thermal_control.mean_cooling_set_point
         cooling_load_transmitted += self._get_load_transmitted(thermal_zone, internal_temperature, ambient_temperature,
                                                                ground_temperature)
     return cooling_load_transmitted
 
   def get_heating_ventilation_load_sensible(self, ambient_temperature):
     """
     Calculates the heating ventilation load sensible
     :return: int
     """
     heating_ventilation_load = 0
     for internal_zone in self._building.internal_zones:
-      for thermal_zone in internal_zone.thermal_zones:
+      for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
         internal_temperature = thermal_zone.thermal_control.mean_heating_set_point
         heating_ventilation_load += self._get_load_ventilation(thermal_zone, internal_temperature, ambient_temperature)
     return heating_ventilation_load
 
   def get_cooling_ventilation_load_sensible(self, ambient_temperature):
     """
     Calculates the cooling ventilation load sensible
     :return: int
     """
     cooling_ventilation_load = 0
     for internal_zone in self._building.internal_zones:
-      for thermal_zone in internal_zone.thermal_zones:
+      for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
         internal_temperature = thermal_zone.thermal_control.mean_cooling_set_point
         cooling_ventilation_load += self._get_load_ventilation(thermal_zone, internal_temperature, ambient_temperature)
     return cooling_ventilation_load
 
   def get_internal_load_sensible(self):
     """
     Calculates the internal load sensible
     :return: int
     """
     cooling_load_occupancy_sensible = 0
     cooling_load_lighting = 0
     cooling_load_equipment_sensible = 0
     for internal_zone in self._building.internal_zones:
-      for thermal_zone in internal_zone.thermal_zones:
+      for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
         cooling_load_occupancy_sensible += (thermal_zone.occupancy.sensible_convective_internal_gain
                                             + thermal_zone.occupancy.sensible_radiative_internal_gain) \
                                            * thermal_zone.footprint_area
         cooling_load_lighting += (
             thermal_zone.lighting.density * thermal_zone.lighting.convective_fraction + thermal_zone.lighting.density *
             thermal_zone.lighting.radiative_fraction
         ) * thermal_zone.footprint_area
         cooling_load_equipment_sensible += (
             thermal_zone.appliances.density * thermal_zone.appliances.convective_fraction +
             thermal_zone.appliances.density * thermal_zone.appliances.radiative_fraction
         ) * thermal_zone.footprint_area
     internal_load = cooling_load_occupancy_sensible + cooling_load_lighting + cooling_load_equipment_sensible
     return internal_load
 
-  def get_radiation_load(self, irradiance_format, hour):
+  def get_radiation_load(self, hour):
     """
     Calculates the radiation load
     :return: int
     """
     cooling_load_radiation = 0
     for internal_zone in self._building.internal_zones:
-      for thermal_zone in internal_zone.thermal_zones:
+      for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
         for thermal_boundary in thermal_zone.thermal_boundaries:
           for thermal_opening in thermal_boundary.thermal_openings:
-            radiation = thermal_boundary.parent_surface.global_irradiance[cte.HOUR][irradiance_format][hour]
+            radiation = thermal_boundary.parent_surface.global_irradiance[cte.HOUR][hour] * cte.WATTS_HOUR_TO_JULES
             cooling_load_radiation += (
                 thermal_opening.area * (1 - thermal_opening.frame_ratio) * thermal_opening.g_value * radiation
             )
     return cooling_load_radiation
```

### Comparing `cerc-hub-0.1.8.2/hub/helpers/peak_loads.py` & `cerc-hub-0.1.8.3/hub/helpers/peak_loads.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,31 +50,33 @@
   def peak_loads_from_hourly(hourly_values):
     """
     Get peak loads from hourly
     :return: [int]
     """
     month = 1
     peaks = [0 for _ in range(12)]
-    for i, value in enumerate(hourly_values):
+    print('hv', hourly_values)
+    for i in range(0, len(hourly_values)):
       if _MONTH_STARTING_HOUR[month] <= i:
         month += 1
-      if value > peaks[month-1]:
-        peaks[month-1] = value
+      if hourly_values[i] > peaks[month-1]:
+        peaks[month-1] = hourly_values[i]
+    print('peak', peaks)
     return peaks
 
   @property
   def heating_peak_loads_from_methodology(self):
     """
     Get heating peak loads by calculate
     :return: [int]
     """
     if not self._can_be_calculated():
       return None
     monthly_heating_loads = []
-    ambient_temperature = self._building.external_temperature[cte.HOUR]['epw']
+    ambient_temperature = self._building.external_temperature[cte.HOUR]
     for month in range(0, 12):
       ground_temperature = self._building.ground_temperature[cte.MONTH]['2'][month]
       heating_ambient_temperature = 100
       start_hour = _MONTH_STARTING_HOUR[month]
       end_hour = 8760
       if month < 11:
         end_hour = _MONTH_STARTING_HOUR[month + 1]
@@ -96,15 +98,15 @@
     """
     Get cooling peak loads by calculate
     :return: [int]
     """
     if not self._can_be_calculated():
       return None
     monthly_cooling_loads = []
-    ambient_temperature = self._building.external_temperature[cte.HOUR]['epw']
+    ambient_temperature = self._building.external_temperature[cte.HOUR]
     for month in range(0, 12):
       ground_temperature = self._building.ground_temperature[cte.MONTH]['2'][month]
       cooling_ambient_temperature = -100
       cooling_calculation_hour = -1
       start_hour = _MONTH_STARTING_HOUR[month]
       end_hour = 8760
       if month < 11:
@@ -114,15 +116,15 @@
         if temperature > cooling_ambient_temperature:
           cooling_ambient_temperature = temperature
           cooling_calculation_hour = hour
       loads = LoadsCalculation(self._building)
       cooling_load_transmitted = loads.get_cooling_transmitted_load(cooling_ambient_temperature, ground_temperature)
       cooling_load_renovation_sensible = loads.get_cooling_ventilation_load_sensible(cooling_ambient_temperature)
       cooling_load_internal_gains_sensible = loads.get_internal_load_sensible()
-      cooling_load_radiation = loads.get_radiation_load('sra', cooling_calculation_hour)
+      cooling_load_radiation = loads.get_radiation_load(cooling_calculation_hour)
       cooling_load_sensible = cooling_load_transmitted + cooling_load_renovation_sensible - cooling_load_radiation \
                               - cooling_load_internal_gains_sensible
 
       cooling_load_latent = 0
       cooling_load = cooling_load_sensible + cooling_load_latent
       cooling_load = min(cooling_load, 0)
       monthly_cooling_loads.append(abs(cooling_load))
```

### Comparing `cerc-hub-0.1.8.2/hub/imports/construction/helpers/construction_helper.py` & `cerc-hub-0.1.8.3/hub/imports/construction/helpers/construction_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 Construction helper
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2022 Concordia CERC group
 Project Coder Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
 """
 
-from hub.helpers import constants as cte
-
 
 class ConstructionHelper:
   """
   Construction helper
   """
   # NREL
 
@@ -36,15 +34,19 @@
   _reference_city_to_nrcan_climate_zone = {
     'Montreal': '6',
     'Repentigny': '6',
     "Montreal Int'l": '6',
     'Levis': '7A',
     'Quebec City': '7A',
     'Kelowna': '5',
-    'Park Slope': '4'
+    'Park Slope': '4',
+    'Varennes': '6',
+    'Laval': '6',
+    'Longueuil': '6',
+    'Saint-Leonard': '6'
   }
 
   _reference_city_to_israel_climate_zone = {
     'Eilat': 'BWh'
   }
 
   @staticmethod
```

### Comparing `cerc-hub-0.1.8.2/hub/imports/construction/helpers/storeys_generation.py` & `cerc-hub-0.1.8.3/hub/imports/construction/helpers/storeys_generation.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/imports/construction_factory.py` & `cerc-hub-0.1.8.3/hub/imports/construction_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/imports/energy_systems/montreal_custom_energy_system_parameters.py` & `cerc-hub-0.1.8.3/hub/imports/energy_systems/montreal_custom_energy_system_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from hub.city_model_structure.energy_systems.generic_energy_system import GenericEnergySystem
 from hub.city_model_structure.energy_systems.generic_generation_system import GenericGenerationSystem
 from hub.city_model_structure.energy_systems.energy_system import EnergySystem
 from hub.city_model_structure.energy_systems.generation_system import GenerationSystem
 from hub.city_model_structure.energy_systems.distribution_system import DistributionSystem
 from hub.city_model_structure.energy_systems.emission_system import EmissionSystem
 from hub.helpers.dictionaries import Dictionaries
-from hub.imports.energy_systems.helpers.energy_systems_helper import EnergySystemsHelper
 
 
 class MontrealCustomEnergySystemParameters:
   """
   MontrealCustomEnergySystemParameters class
   """
```

### Comparing `cerc-hub-0.1.8.2/hub/imports/energy_systems_factory.py` & `cerc-hub-0.1.8.3/hub/imports/energy_systems_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 Copyright © 2022 Concordia CERC group
 Project Coder Pilar Monsalvete pilar.monsalvete@concordi.
 Code contributors: Peter Yefi peteryefi@gmail.com
 """
 from pathlib import Path
 
 from hub.helpers.utils import validate_import_export_type
-from hub.imports.energy_systems.air_source_hp_parameters import AirSourceHeatPumpParameters
 from hub.imports.energy_systems.montreal_custom_energy_system_parameters import MontrealCustomEnergySystemParameters
-from hub.imports.energy_systems.water_to_water_hp_parameters import WaterToWaterHPParameters
 
 
 class EnergySystemsFactory:
   """
   EnergySystemsFactory class
   """
 
@@ -22,32 +20,14 @@
     if base_path is None:
       base_path = Path(Path(__file__).parent.parent / 'data/energy_systems')
     self._handler = '_' + handler.lower()
     validate_import_export_type(EnergySystemsFactory, handler)
     self._city = city
     self._base_path = base_path
 
-  def _air_source_hp(self):
-    """
-    Enrich the city by using xlsx heat pump information
-    """
-    AirSourceHeatPumpParameters(self._city, self._base_path).enrich_city()
-    self._city.level_of_detail.energy_systems = 0
-    for building in self._city.buildings:
-      building.level_of_detail.energy_systems = 0
-
-  def _water_to_water_hp(self):
-    """
-    Enrich the city by using water to water heat pump information
-    """
-    WaterToWaterHPParameters(self._city, self._base_path).enrich_city()
-    self._city.level_of_detail.energy_systems = 0
-    for building in self._city.buildings:
-      building.level_of_detail.energy_systems = 0
-
   def _montreal_custom(self):
     """
     Enrich the city by using montreal custom energy systems catalog information
     """
     MontrealCustomEnergySystemParameters(self._city).enrich_buildings()
     self._city.level_of_detail.energy_systems = 1
     for building in self._city.buildings:
```

### Comparing `cerc-hub-0.1.8.2/hub/imports/geometry/citygml.py` & `cerc-hub-0.1.8.3/hub/imports/geometry/citygml.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/imports/geometry/citygml_classes/citygml_base.py` & `cerc-hub-0.1.8.3/hub/imports/geometry/citygml_classes/citygml_base.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/imports/geometry/citygml_classes/citygml_lod1.py` & `cerc-hub-0.1.8.3/hub/imports/geometry/citygml_classes/citygml_lod1.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/imports/geometry/citygml_classes/citygml_lod2.py` & `cerc-hub-0.1.8.3/hub/imports/geometry/citygml_classes/citygml_lod2.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/imports/geometry/geojson.py` & `cerc-hub-0.1.8.3/hub/imports/geometry/geojson.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/imports/geometry/helpers/geometry_helper.py` & `cerc-hub-0.1.8.3/hub/imports/geometry/helpers/geometry_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 import math
 import sys
 
 import numpy as np
 from numpy import ndarray
 
+
 class GeometryHelper:
   """
   Geometry helper
   """
   @staticmethod
   def to_points_matrix(points):
     """
```

### Comparing `cerc-hub-0.1.8.2/hub/imports/geometry/obj.py` & `cerc-hub-0.1.8.3/hub/imports/geometry/obj.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/imports/geometry_factory.py` & `cerc-hub-0.1.8.3/hub/imports/geometry_factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """
 GeometryFactory retrieve the specific geometric module to load the given format
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2022 Concordia CERC group
 Project Coder Guille Gutierrez guillermo.gutierrezmorote@concordia.ca
 """
-import geopandas
 
 from hub.city_model_structure.city import City
 from hub.helpers.utils import validate_import_export_type
 from hub.imports.geometry.citygml import CityGml
 from hub.imports.geometry.geojson import Geojson
-from hub.imports.geometry.gpandas import GPandas
 from hub.imports.geometry.obj import Obj
 
 
 class GeometryFactory:
   """
   GeometryFactory class
   """
@@ -53,24 +51,14 @@
     """
     Enrich the city by using OBJ information as data source
     :return: City
     """
     return Obj(self._path).city
 
   @property
-  def _gpandas(self) -> City:
-    """
-    Enrich the city by using GeoPandas information as data source
-    :return: City
-    """
-    if self._data_frame is None:
-      self._data_frame = geopandas.read_file(self._path)
-    return GPandas(self._data_frame).city
-
-  @property
   def _geojson(self) -> City:
     """
     Enrich the city by using Geojson information as data source
     :return: City
     """
     return Geojson(self._path,
                    self._aliases_field,
```

### Comparing `cerc-hub-0.1.8.2/hub/imports/results/insel_monthly_energry_balance.py` & `cerc-hub-0.1.8.3/hub/imports/results/insel_monthly_energry_balance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Insel monthly energy balance
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2022 Concordia CERC group
 Project Coder Guillermo.GutierrezMorote@concordia.ca
 """
+
 from pathlib import Path
 import csv
-import pandas as pd
 
 import hub.helpers.constants as cte
 
 
 class InselMonthlyEnergyBalance:
   """
   Import insel monthly energy balance results
@@ -26,37 +26,35 @@
     cooling = []
     with open(Path(insel_output_file_path).resolve(), 'r', encoding='utf8') as csv_file:
       csv_reader = csv.reader(csv_file)
       for line in csv_reader:
         demand = str(line).replace("['", '').replace("']", '').split()
         for i in range(0, 2):
           if demand[i] != 'NaN':
-            aux = float(demand[i]) * 1000  # kWh to Wh
+            aux = float(demand[i]) * cte.WATTS_HOUR_TO_JULES * 1000  # kWh to J
             demand[i] = str(aux)
           else:
             demand[i] = '0'
-        heating.append(demand[0])
-        cooling.append(demand[1])
-    monthly_heating = pd.DataFrame(heating, columns=[cte.INSEL_MEB]).astype(float)
-    monthly_cooling = pd.DataFrame(cooling, columns=[cte.INSEL_MEB]).astype(float)
-    return monthly_heating, monthly_cooling
+        heating.append(float(demand[0]))
+        cooling.append(float(demand[1]))
+    return heating, cooling
 
   def _dhw_and_electric_demand(self):
     for building in self._city.buildings:
       domestic_hot_water_demand = []
       lighting_demand = []
       appliances_demand = []
-      if building.internal_zones[0].thermal_zones is None:
+      if building.internal_zones[0].thermal_zones_from_internal_zones is None:
         domestic_hot_water_demand = [0] * 12
         lighting_demand = [0] * 12
         appliances_demand = [0] * 12
       else:
-        thermal_zone = building.internal_zones[0].thermal_zones[0]
+        thermal_zone = building.internal_zones[0].thermal_zones_from_internal_zones[0]
         area = thermal_zone.total_floor_area
-        cold_water = building.cold_water_temperature[cte.MONTH]['epw']
+        cold_water = building.cold_water_temperature[cte.MONTH]
         peak_flow = thermal_zone.domestic_hot_water.peak_flow
         service_temperature = thermal_zone.domestic_hot_water.service_temperature
         lighting_density = thermal_zone.lighting.density
         appliances_density = thermal_zone.appliances.density
 
         for month in range(0, 12):
           total_dhw_demand = 0
@@ -64,64 +62,53 @@
           total_appliances = 0
 
           for schedule in thermal_zone.lighting.schedules:
             total_day = 0
             for value in schedule.values:
               total_day += value
             for day_type in schedule.day_types:
-              total_lighting += total_day * cte.DAYS_A_MONTH[day_type][month] * lighting_density
+              total_lighting += total_day * cte.WEEK_DAYS_A_MONTH[day_type][month] \
+                                * lighting_density / cte.WATTS_HOUR_TO_JULES
           lighting_demand.append(total_lighting * area)
 
           for schedule in thermal_zone.appliances.schedules:
             total_day = 0
             for value in schedule.values:
               total_day += value
             for day_type in schedule.day_types:
-              total_appliances += total_day * cte.DAYS_A_MONTH[day_type][month] * appliances_density
+              total_appliances += total_day * cte.WEEK_DAYS_A_MONTH[day_type][month] \
+                                  * appliances_density / cte.WATTS_HOUR_TO_JULES
           appliances_demand.append(total_appliances * area)
 
           for schedule in thermal_zone.domestic_hot_water.schedules:
             total_day = 0
             for value in schedule.values:
               total_day += value
             for day_type in schedule.day_types:
               demand = (
-                  peak_flow * cte.WATER_DENSITY * cte.WATER_HEAT_CAPACITY * (service_temperature - cold_water[month])
+                  peak_flow * cte.WATER_DENSITY * cte.WATER_HEAT_CAPACITY
+                  * (service_temperature - cold_water[month]) / cte.WATTS_HOUR_TO_JULES
               )
-              total_dhw_demand += total_day * cte.DAYS_A_MONTH[day_type][month] * demand
+              total_dhw_demand += total_day * cte.WEEK_DAYS_A_MONTH[day_type][month] * demand
           domestic_hot_water_demand.append(total_dhw_demand * area)
 
-      building.domestic_hot_water_heat_demand[cte.MONTH] = pd.DataFrame(domestic_hot_water_demand,
-                                                                        columns=[cte.INSEL_MEB])
-      yearly_domestic_hot_water_demand = [sum(domestic_hot_water_demand)]
-      building.domestic_hot_water_heat_demand[cte.YEAR] = pd.DataFrame(yearly_domestic_hot_water_demand,
-                                                                       columns=[cte.INSEL_MEB])
-      building.lighting_electrical_demand[cte.MONTH] = pd.DataFrame(lighting_demand, columns=[cte.INSEL_MEB])
-      yearly_lighting_electrical_demand = [sum(lighting_demand)]
-      building.lighting_electrical_demand[cte.YEAR] = pd.DataFrame(
-        yearly_lighting_electrical_demand,
-        columns=[cte.INSEL_MEB]
-      )
-      building.appliances_electrical_demand[cte.MONTH] = pd.DataFrame(appliances_demand, columns=[cte.INSEL_MEB])
-      yearly_appliances_electrical_demand = [sum(appliances_demand)]
-      building.appliances_electrical_demand[cte.YEAR] = pd.DataFrame(
-        yearly_appliances_electrical_demand,
-        columns=[cte.INSEL_MEB]
-      )
+      building.domestic_hot_water_heat_demand[cte.MONTH] = domestic_hot_water_demand
+      building.domestic_hot_water_heat_demand[cte.YEAR] = [sum(domestic_hot_water_demand)]
+      building.lighting_electrical_demand[cte.MONTH] = lighting_demand
+      building.lighting_electrical_demand[cte.YEAR] = [sum(lighting_demand)]
+      building.appliances_electrical_demand[cte.MONTH] = appliances_demand
+      building.appliances_electrical_demand[cte.YEAR] = [sum(appliances_demand)]
 
   def enrich(self):
     """
-    Enrich the city by using the insel monthly energy balance output files
+    Enrich the city by using the insel monthly energy balance output files (J)
     :return: None
     """
     for building in self._city.buildings:
       file_name = building.name + '.out'
       insel_output_file_path = Path(self._base_path / file_name).resolve()
       if insel_output_file_path.is_file():
-        building.heating_demand[cte.MONTH], building.cooling_demand[cte.MONTH] = self._conditioning_demand(insel_output_file_path)
-        building.heating_demand[cte.YEAR] = pd.DataFrame(
-          [building.heating_demand[cte.MONTH][cte.INSEL_MEB].astype(float).sum()], columns=[cte.INSEL_MEB]
-        )
-        building.cooling_demand[cte.YEAR] = pd.DataFrame(
-          [building.cooling_demand[cte.MONTH][cte.INSEL_MEB].astype(float).sum()], columns=[cte.INSEL_MEB]
-        )
+        building.heating_demand[cte.MONTH], building.cooling_demand[cte.MONTH] \
+          = self._conditioning_demand(insel_output_file_path)
+        building.heating_demand[cte.YEAR] = [sum(building.heating_demand[cte.MONTH])]
+        building.cooling_demand[cte.YEAR] = [sum(building.cooling_demand[cte.MONTH])]
     self._dhw_and_electric_demand()
```

### Comparing `cerc-hub-0.1.8.2/hub/imports/results_factory.py` & `cerc-hub-0.1.8.3/hub/imports/results_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 Copyright © 2022 Concordia CERC group
 Project Coder Guille Gutierrez guillermo.gutierrezmorote@concordia.ca
 Code contributors: Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
 """
 from pathlib import Path
 
 from hub.helpers.utils import validate_import_export_type
-from hub.imports.results.insel_heatpump_energy_demand import InselHeatPumpEnergyDemand
 from hub.imports.results.insel_monthly_energry_balance import InselMonthlyEnergyBalance
 from hub.imports.results.simplified_radiosity_algorithm import SimplifiedRadiosityAlgorithm
 
 
 class ResultFactory:
   """
   ResultFactory class
@@ -37,21 +36,14 @@
 
   def _sra(self):
     """
     Enrich the city with Simplified Radiosity Algorithm results
     """
     SimplifiedRadiosityAlgorithm(self._city, self._base_path).enrich()
 
-  def _heat_pump(self):
-    """
-    Enrich the city (energy system specifically) with heat pump insel simulation
-    results
-    """
-    InselHeatPumpEnergyDemand(self._city, self._base_path, self._hp_model).enrich()
-
   def _insel_monthly_energy_balance(self):
     """
     Enrich the city with insel monthly energy balance results
     """
     InselMonthlyEnergyBalance(self._city, self._base_path).enrich()
 
   def enrich(self):
```

### Comparing `cerc-hub-0.1.8.2/hub/imports/usage/comnet_usage_parameters.py` & `cerc-hub-0.1.8.3/hub/imports/usage/comnet_usage_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,16 +67,15 @@
     raise KeyError('archetype not found')
 
   @staticmethod
   def _assign_values(usage, archetype, volume_per_area, cold_water_temperature):
     # Due to the fact that python is not a typed language, the wrong object type is assigned to
     # usage.occupancy when writing usage.occupancy = archetype.occupancy.
     # Same happens for lighting and appliances. Therefore, this walk around has been done.
-    usage.mechanical_air_change = archetype.ventilation_rate / volume_per_area \
-                                  * cte.HOUR_TO_SECONDS
+    usage.mechanical_air_change = archetype.ventilation_rate / volume_per_area
     _occupancy = Occupancy()
     _occupancy.occupancy_density = archetype.occupancy.occupancy_density
     _occupancy.sensible_radiative_internal_gain = archetype.occupancy.sensible_radiative_internal_gain
     _occupancy.latent_internal_gain = archetype.occupancy.latent_internal_gain
     _occupancy.sensible_convective_internal_gain = archetype.occupancy.sensible_convective_internal_gain
     _occupancy.occupancy_schedules = archetype.occupancy.schedules
     usage.occupancy = _occupancy
@@ -100,15 +99,15 @@
     _control.hvac_availability_schedules = archetype.thermal_control.hvac_availability_schedules
     usage.thermal_control = _control
     _domestic_hot_water = DomesticHotWater()
     _domestic_hot_water.density = archetype.domestic_hot_water.density
     _domestic_hot_water.service_temperature = archetype.domestic_hot_water.service_temperature
     peak_flow = None
     if len(cold_water_temperature) > 0:
-      cold_temperature = cold_water_temperature[cte.YEAR]['epw']
+      cold_temperature = cold_water_temperature[cte.YEAR][0]
       peak_flow = 0
       if (archetype.domestic_hot_water.service_temperature - cold_temperature) > 0:
         peak_flow = archetype.domestic_hot_water.density / cte.WATER_DENSITY / cte.WATER_HEAT_CAPACITY \
                     / (archetype.domestic_hot_water.service_temperature - cold_temperature)
     _domestic_hot_water.peak_flow = peak_flow
     _domestic_hot_water.schedules = archetype.domestic_hot_water.schedules
     usage.domestic_hot_water = _domestic_hot_water
```

### Comparing `cerc-hub-0.1.8.2/hub/imports/usage/eilat_usage_parameters.py` & `cerc-hub-0.1.8.3/hub/imports/usage/eilat_usage_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,16 +67,15 @@
     raise KeyError('archetype not found')
 
   @staticmethod
   def _assign_values(usage, archetype, volume_per_area, cold_water_temperature):
     # Due to the fact that python is not a typed language, the wrong object type is assigned to
     # usage.occupancy when writing usage.occupancy = archetype.occupancy.
     # Same happens for lighting and appliances. Therefore, this walk around has been done.
-    usage.mechanical_air_change = archetype.ventilation_rate / volume_per_area \
-                                  * cte.HOUR_TO_SECONDS
+    usage.mechanical_air_change = archetype.ventilation_rate / volume_per_area
     _occupancy = Occupancy()
     _occupancy.occupancy_density = archetype.occupancy.occupancy_density
     _occupancy.sensible_radiative_internal_gain = archetype.occupancy.sensible_radiative_internal_gain
     _occupancy.latent_internal_gain = archetype.occupancy.latent_internal_gain
     _occupancy.sensible_convective_internal_gain = archetype.occupancy.sensible_convective_internal_gain
     _occupancy.occupancy_schedules = archetype.occupancy.schedules
     usage.occupancy = _occupancy
@@ -100,15 +99,15 @@
     _control.hvac_availability_schedules = archetype.thermal_control.hvac_availability_schedules
     usage.thermal_control = _control
     _domestic_hot_water = DomesticHotWater()
     _domestic_hot_water.density = archetype.domestic_hot_water.density
     _domestic_hot_water.service_temperature = archetype.domestic_hot_water.service_temperature
     peak_flow = None
     if len(cold_water_temperature) > 0:
-      cold_temperature = cold_water_temperature[cte.YEAR]['epw']
+      cold_temperature = cold_water_temperature[cte.YEAR][0]
       peak_flow = 0
       if (archetype.domestic_hot_water.service_temperature - cold_temperature) > 0:
         peak_flow = archetype.domestic_hot_water.density / cte.WATER_DENSITY / cte.WATER_HEAT_CAPACITY \
                     / (archetype.domestic_hot_water.service_temperature - cold_temperature)
     _domestic_hot_water.peak_flow = peak_flow
     _domestic_hot_water.schedules = archetype.domestic_hot_water.schedules
     usage.domestic_hot_water = _domestic_hot_water
```

### Comparing `cerc-hub-0.1.8.2/hub/imports/usage/nrcan_usage_parameters.py` & `cerc-hub-0.1.8.3/hub/imports/usage/nrcan_usage_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,19 +88,19 @@
       if str(usage_name) == str(building_archetype.name):
         return building_archetype
     raise KeyError('archetype not found')
 
   @staticmethod
   def _assign_values(usage, archetype, volume_per_area, cold_water_temperature):
     if archetype.mechanical_air_change > 0:
-      # ACH
+      # 1/s
       usage.mechanical_air_change = archetype.mechanical_air_change
     elif archetype.ventilation_rate > 0:
-      # m3/m2.s to ACH
-      usage.mechanical_air_change = archetype.ventilation_rate / volume_per_area * cte.HOUR_TO_SECONDS
+      # m3/m2.s to 1/s
+      usage.mechanical_air_change = archetype.ventilation_rate / volume_per_area
     else:
       usage.mechanical_air_change = 0
     _occupancy = Occupancy()
     _occupancy.occupancy_density = archetype.occupancy.occupancy_density
     _occupancy.sensible_radiative_internal_gain = archetype.occupancy.sensible_radiative_internal_gain
     _occupancy.latent_internal_gain = archetype.occupancy.latent_internal_gain
     _occupancy.sensible_convective_internal_gain = archetype.occupancy.sensible_convective_internal_gain
@@ -126,15 +126,15 @@
     _control.hvac_availability_schedules = archetype.thermal_control.hvac_availability_schedules
     usage.thermal_control = _control
     _domestic_hot_water = DomesticHotWater()
     _domestic_hot_water.peak_flow = archetype.domestic_hot_water.peak_flow
     _domestic_hot_water.service_temperature = archetype.domestic_hot_water.service_temperature
     density = None
     if len(cold_water_temperature) > 0:
-      cold_temperature = cold_water_temperature[cte.YEAR]['epw']
+      cold_temperature = cold_water_temperature[cte.YEAR][0]
       density = (
           archetype.domestic_hot_water.peak_flow * cte.WATER_DENSITY * cte.WATER_HEAT_CAPACITY *
           (archetype.domestic_hot_water.service_temperature - cold_temperature)
       )
     _domestic_hot_water.density = density
     _domestic_hot_water.schedules = archetype.domestic_hot_water.schedules
     usage.domestic_hot_water = _domestic_hot_water
```

### Comparing `cerc-hub-0.1.8.2/hub/imports/usage_factory.py` & `cerc-hub-0.1.8.3/hub/imports/usage_factory.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/imports/weather/epw_weather_parameters.py` & `cerc-hub-0.1.8.3/hub/imports/weather/epw_weather_parameters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 EpwWeatherParameters class to extract weather parameters from a defined region in .epw format (EnergyPlus Weather)
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2022 Concordia CERC group
 Project Coder Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
 """
+
 import logging
 import sys
 from pathlib import Path
-
-import pandas as pd
 import requests
+import pandas as pd
 
 import hub.helpers.constants as cte
+from hub.helpers.monthly_values import MonthlyValues
 from hub.city_model_structure.city import City
 from hub.imports.weather.helpers.weather import Weather as wh
 
 
 class EpwWeatherParameters:
   """
   EpwWeatherParameters class
@@ -71,87 +72,68 @@
                                                 'opaque_sky_cover', 'visibility_km',
                                                 'ceiling_heigh_m_s', 'present_weather_observation',
                                                 'present_weather_codes',
                                                 'precipitable_water_mm', 'aerosol_optical_depth_10_3_ths',
                                                 'snow_depth_cm',
                                                 'days_since_last_snowfall', 'albedo', 'liquid_precipitation_depth_mm',
                                                 'liquid_precipitation_quality_hr'])
+      number_invalid_records = self._weather_values[
+        self._weather_values.dry_bulb_temperature_c == 99.9].count().dry_bulb_temperature_c
+      if number_invalid_records > 0:
+        sys.stderr.write(f'Warning: {self._path} invalid records (value of 99.9) in dry bulb temperature\n')
+      number_invalid_records = self._weather_values[
+        self._weather_values.global_horizontal_radiation_wh_m2 == 9999].count().global_horizontal_radiation_wh_m2
+      if number_invalid_records > 0:
+        sys.stderr.write(f'Warning: {self._path} invalid records (value of 9999) in global horizontal radiation\n')
+      number_invalid_records = self._weather_values[
+        self._weather_values.diffuse_horizontal_radiation_wh_m2 == 9999].count().diffuse_horizontal_radiation_wh_m2
+      if number_invalid_records > 0:
+        sys.stderr.write(f'Warning: {self._path} invalid records (value of 9999) in diffuse horizontal radiation\n')
+      number_invalid_records = self._weather_values[
+        self._weather_values.direct_normal_radiation_wh_m2 == 9999].count().direct_normal_radiation_wh_m2
+      if number_invalid_records > 0:
+        sys.stderr.write(f'Warning: {self._path} invalid records (value of 9999) in direct horizontal radiation\n')
+
+      self._weather_values = self._weather_values.to_dict(orient='list')
+
     except SystemExit:
       sys.stderr.write(f'Error: wrong formatting of weather file {self._path}\n')
       sys.exit()
     for building in self._city.buildings:
       building.ground_temperature[cte.MONTH] = ground_temperature_from_file
       ground_temperature = {}
       for ground_temperature_set in building.ground_temperature[cte.MONTH]:
-        temperature = 0
-        for value in building.ground_temperature[cte.MONTH][ground_temperature_set]:
-          temperature += value / 12
+        temperature = sum(building.ground_temperature[cte.MONTH][ground_temperature_set]) / 12
         ground_temperature[ground_temperature_set] = [temperature]
       building.ground_temperature[cte.YEAR] = ground_temperature
       if cte.HOUR in building.external_temperature:
         del building.external_temperature[cte.HOUR]
-      new_value = pd.DataFrame(self._weather_values[['dry_bulb_temperature_c']].to_numpy(), columns=['epw'])
-      number_invalid_records = new_value[new_value.epw == 99.9].count().epw
-      if number_invalid_records > 0:
-        sys.stderr.write(f'Warning: {self._path} invalid records (value of 99.9) in dry bulb temperature\n')
-      if cte.HOUR not in building.external_temperature:
-        building.external_temperature[cte.HOUR] = new_value
-      else:
-        pd.concat([building.external_temperature[cte.HOUR], new_value], axis=1)
-
-      new_value = pd.DataFrame(self._weather_values[['global_horizontal_radiation_wh_m2']].to_numpy(), columns=['epw'])
-      number_invalid_records = new_value[new_value.epw == 9999].count().epw
-      if number_invalid_records > 0:
-        sys.stderr.write(f'Warning: {self._path} invalid records (value of 9999) in global horizontal radiation\n')
-      if cte.HOUR not in building.global_horizontal:
-        building.global_horizontal[cte.HOUR] = new_value
-      else:
-        pd.concat([building.global_horizontal[cte.HOUR], new_value], axis=1)
-
-      new_value = pd.DataFrame(self._weather_values[['diffuse_horizontal_radiation_wh_m2']].to_numpy(), columns=['epw'])
-      number_invalid_records = new_value[new_value.epw == 9999].count().epw
-      if number_invalid_records > 0:
-        sys.stderr.write(f'Warning: {self._path} invalid records (value of 9999) in diffuse horizontal radiation\n')
-      if cte.HOUR not in building.diffuse:
-        building.diffuse[cte.HOUR] = new_value
-      else:
-        pd.concat([building.diffuse[cte.HOUR], new_value], axis=1)
+#      new_value = pd.DataFrame(self._weather_values[['dry_bulb_temperature_c']].to_numpy(), columns=['epw'])
+#      number_invalid_records = new_value[new_value.epw == 99.9].count().epw
+      building.external_temperature[cte.HOUR] = self._weather_values['dry_bulb_temperature_c']
+      building.global_horizontal[cte.HOUR] = [x / cte.WATTS_HOUR_TO_JULES
+                                              for x in self._weather_values['global_horizontal_radiation_wh_m2']]
+      building.diffuse[cte.HOUR] = [x / cte.WATTS_HOUR_TO_JULES
+                                    for x in self._weather_values['diffuse_horizontal_radiation_wh_m2']]
+      building.beam[cte.HOUR] = [x / cte.WATTS_HOUR_TO_JULES
+                                 for x in self._weather_values['direct_normal_radiation_wh_m2']]
+      building.cold_water_temperature[cte.HOUR] = wh().cold_water_temperature(building.external_temperature[cte.HOUR])
 
-      new_value = pd.DataFrame(self._weather_values[['direct_normal_radiation_wh_m2']].to_numpy(), columns=['epw'])
-      number_invalid_records = new_value[new_value.epw == 9999].count().epw
-      if number_invalid_records > 0:
-        sys.stderr.write(f'Warning: {self._path} invalid records (value of 9999) in direct horizontal radiation\n')
-      if cte.HOUR not in building.beam:
-        building.beam[cte.HOUR] = new_value
-      else:
-        pd.concat([building.beam[cte.HOUR], new_value], axis=1)
-
-      new_value = wh().cold_water_temperature(building.external_temperature[cte.HOUR]['epw'])
-      if cte.HOUR not in building.cold_water_temperature:
-        building.cold_water_temperature[cte.HOUR] = new_value
-      else:
-        pd.concat([building.cold_water_temperature[cte.HOUR], new_value], axis=1)
     # create the monthly and yearly values out of the hourly
     for building in self._city.buildings:
-      if cte.MONTH not in building.external_temperature:
-        building.external_temperature[cte.MONTH] = \
-          wh().get_monthly_mean_values(building.external_temperature[cte.HOUR][['epw']])
-      if cte.YEAR not in building.external_temperature:
-        building.external_temperature[cte.YEAR] = \
-          wh(). get_yearly_mean_values(building.external_temperature[cte.HOUR][['epw']])
-      if cte.MONTH not in building.cold_water_temperature:
-        building.cold_water_temperature[cte.MONTH] = wh().get_monthly_mean_values(
-          building.cold_water_temperature[cte.HOUR][['epw']])
-      if cte.YEAR not in building.cold_water_temperature:
-        building.cold_water_temperature[cte.YEAR] = wh().get_yearly_mean_values(
-          building.cold_water_temperature[cte.HOUR][['epw']])
+      building.external_temperature[cte.MONTH] = \
+        MonthlyValues().get_mean_values(building.external_temperature[cte.HOUR])
+      building.external_temperature[cte.YEAR] = [sum(building.external_temperature[cte.HOUR]) / 9870]
+      building.cold_water_temperature[cte.MONTH] = \
+        MonthlyValues().get_mean_values(building.cold_water_temperature[cte.HOUR])
+      building.cold_water_temperature[cte.YEAR] = [sum(building.cold_water_temperature[cte.HOUR]) / 9870]
 
       # If the usage has already being imported, the domestic hot water missing values must be calculated here that
       # the cold water temperature is finally known
-      cold_temperature = building.cold_water_temperature[cte.YEAR]['epw']
+      cold_temperature = building.cold_water_temperature[cte.YEAR][0]
       for internal_zone in building.internal_zones:
         if internal_zone.usages is not None:
           for usage in internal_zone.usages:
             if usage.domestic_hot_water.peak_flow is None:
               if usage.domestic_hot_water.density is None:
                 continue
               peak_flow = 0
```

### Comparing `cerc-hub-0.1.8.2/hub/imports/weather_factory.py` & `cerc-hub-0.1.8.3/hub/imports/weather_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 WeatherFactory retrieve the specific weather module for the given source format
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2022 Concordia CERC group
 Project Coder Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
 """
-from pathlib import Path
 
 from hub.city_model_structure.city import City
 from hub.helpers.utils import validate_import_export_type
 from hub.imports.weather.epw_weather_parameters import EpwWeatherParameters
 
 
 class WeatherFactory:
```

### Comparing `cerc-hub-0.1.8.2/hub/persistence/configuration.py` & `cerc-hub-0.1.8.3/hub/persistence/configuration.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/persistence/db_control.py` & `cerc-hub-0.1.8.3/hub/persistence/db_control.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/persistence/db_setup.py` & `cerc-hub-0.1.8.3/hub/persistence/db_setup.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/persistence/models/application.py` & `cerc-hub-0.1.8.3/hub/persistence/models/application.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/persistence/models/city.py` & `cerc-hub-0.1.8.3/hub/persistence/models/city.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/persistence/models/city_object.py` & `cerc-hub-0.1.8.3/hub/persistence/models/city_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     self.total_heating_area = building.floor_area * storeys
     wall_area = 0
     for wall in building.walls:
       wall_area += wall.solid_polygon.area
     self.wall_area = wall_area
     window_ratio = 0
     for internal_zone in building.internal_zones:
-      for thermal_zone in internal_zone.thermal_zones:
+      for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
         for thermal_boundary in thermal_zone.thermal_boundaries:
           window_ratio = thermal_boundary.window_ratio
           break
     self.windows_area = wall_area * window_ratio
     system_name = building.energy_systems_archetype_name
     if system_name is None:
       system_name = ''
```

### Comparing `cerc-hub-0.1.8.2/hub/persistence/models/simulation_results.py` & `cerc-hub-0.1.8.3/hub/persistence/models/simulation_results.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/persistence/models/user.py` & `cerc-hub-0.1.8.3/hub/persistence/models/user.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/persistence/repositories/application.py` & `cerc-hub-0.1.8.3/hub/persistence/repositories/application.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/persistence/repositories/city.py` & `cerc-hub-0.1.8.3/hub/persistence/repositories/city.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/persistence/repositories/city_object.py` & `cerc-hub-0.1.8.3/hub/persistence/repositories/city_object.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/persistence/repositories/simulation_results.py` & `cerc-hub-0.1.8.3/hub/persistence/repositories/simulation_results.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/persistence/repositories/user.py` & `cerc-hub-0.1.8.3/hub/persistence/repositories/user.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/hub/persistence/repository.py` & `cerc-hub-0.1.8.3/hub/persistence/repository.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/setup.py` & `cerc-hub-0.1.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
             'hub.catalog_factories.usage',
             'hub.city_model_structure',
             'hub.city_model_structure.attributes',
             'hub.city_model_structure.building_demand',
             'hub.city_model_structure.energy_systems',
             'hub.city_model_structure.greenery',
             'hub.city_model_structure.iot',
-            'hub.city_model_structure.transport',
             'hub.config',
             'hub.data',
             'hub.exports',
             'hub.exports.building_energy',
             'hub.exports.building_energy.idf_files',
             'hub.exports.building_energy.insel',
             'hub.exports.energy_systems',
@@ -68,15 +67,14 @@
             'hub.helpers',
             'hub.helpers.peak_calculation',
             'hub.helpers.data',
             'hub.imports',
             'hub.imports.construction',
             'hub.imports.construction.helpers',
             'hub.imports.energy_systems',
-            'hub.imports.energy_systems.helpers',
             'hub.imports.geometry',
             'hub.imports.geometry.citygml_classes',
             'hub.imports.geometry.helpers',
             'hub.imports.results',
             'hub.imports.usage',
             'hub.imports.weather',
             'hub.imports.weather.helpers',
```

### Comparing `cerc-hub-0.1.8.2/tests/test_city_merge.py` & `cerc-hub-0.1.8.3/tests/test_city_merge.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 TestCityMerge test and validate the merge of several cities into one
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2022 Concordia CERC group
 Project Coder Guille Gutierrez Guillermo.GutierrezMorote@concordia.ca
 """
+
 import copy
 import distutils.spawn
 import subprocess
 from pathlib import Path
 from unittest import TestCase
 
-import pandas as pd
-
 from hub.city_model_structure.city import City
 from hub.imports.geometry_factory import GeometryFactory
 from hub.imports.results_factory import ResultFactory
 from hub.exports.exports_factory import ExportsFactory
 import hub.helpers.constants as cte
 
 
@@ -68,42 +67,42 @@
     self.assertEqual(17, len(full_city.buildings), 'Wrong number of buildings')
     merged_city = full_city.merge(even_city)
 
     full_city_building_total_radiation = 0
     for building in merged_city.buildings:
       for surface in building.surfaces:
         if surface.global_irradiance:
-          full_city_building_total_radiation += surface.global_irradiance[cte.YEAR].iloc[0, 0]
+          full_city_building_total_radiation += surface.global_irradiance[cte.YEAR][0]
 
     merged_city_building_total_radiation = 0
     for building in merged_city.buildings:
       for surface in building.surfaces:
         if surface.global_irradiance:
-          merged_city_building_total_radiation += surface.global_irradiance[cte.YEAR].iloc[0, 0]
+          merged_city_building_total_radiation += surface.global_irradiance[cte.YEAR][0]
     self.assertEqual(full_city_building_total_radiation, merged_city_building_total_radiation)
 
     merged_city = even_city.merge(full_city)
     merged_city_building_total_radiation = 0
     for building in merged_city.buildings:
       for surface in building.surfaces:
         if surface.global_irradiance:
-          merged_city_building_total_radiation += surface.global_irradiance[cte.YEAR].iloc[0, 0]
+          merged_city_building_total_radiation += surface.global_irradiance[cte.YEAR][0]
     self.assertEqual(full_city_building_total_radiation, merged_city_building_total_radiation)
 
     for building in even_city.buildings:
       for surface in building.surfaces:
-        surface.global_irradiance[cte.YEAR] = pd.DataFrame([3], columns=['sra_mockup_value'])
+        surface.global_irradiance[cte.YEAR] = [3]
 
     merged_city = full_city.merge(even_city)
     first_merged_city_building_total_radiation = 0
     for building in merged_city.buildings:
       for surface in building.surfaces:
         if surface.global_irradiance:
-          first_merged_city_building_total_radiation += surface.global_irradiance[cte.YEAR].iloc[0, 0]
+          first_merged_city_building_total_radiation += surface.global_irradiance[cte.YEAR][0]
     merged_city = even_city.merge(full_city)
     second_merged_city_building_total_radiation = 0
     for building in merged_city.buildings:
       for surface in building.surfaces:
         if surface.global_irradiance:
-          second_merged_city_building_total_radiation += surface.global_irradiance[cte.YEAR].iloc[0, 0]
+          second_merged_city_building_total_radiation += surface.global_irradiance[cte.YEAR][0]
     self.assertEqual(first_merged_city_building_total_radiation, second_merged_city_building_total_radiation)
```

### Comparing `cerc-hub-0.1.8.2/tests/test_construction_catalog.py` & `cerc-hub-0.1.8.3/tests/test_construction_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/tests/test_construction_factory.py` & `cerc-hub-0.1.8.3/tests/test_construction_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
       self.assertIsNotNone(building.roof_type, 'building roof type is none')
       self.assertIsNotNone(building.floor_area, 'building floor_area is none')
       self.assertIsNone(building.households, 'building households is not none')
       self.assertFalse(building.is_conditioned, 'building is conditioned')
       self.assertIsNotNone(building.shell, 'building shell is none')
 
   def _check_thermal_zones(self, internal_zone):
-    for thermal_zone in internal_zone.thermal_zones:
+    for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
       self.assertIsNotNone(thermal_zone.id, 'thermal_zone id is none')
       self.assertIsNotNone(thermal_zone.footprint_area, 'thermal_zone floor area is none')
       self.assertTrue(len(thermal_zone.thermal_boundaries) > 0, 'thermal_zone thermal_boundaries not defined')
       self.assertIsNotNone(thermal_zone.additional_thermal_bridge_u_value, 'additional_thermal_bridge_u_value is none')
       self.assertIsNotNone(thermal_zone.effective_thermal_capacity, 'thermal_zone effective_thermal_capacity is none')
       self.assertIsNotNone(thermal_zone.infiltration_rate_system_off,
                            'thermal_zone infiltration_rate_system_off is none')
@@ -134,37 +134,34 @@
         self.assertIsNotNone(thermal_boundary.id, 'thermal_boundary id is none')
         self.assertIsNotNone(thermal_boundary.parent_surface, 'thermal_boundary surface is none')
         self.assertIsNotNone(thermal_boundary.thermal_zones, 'thermal_boundary delimits no thermal zone')
         self.assertIsNotNone(thermal_boundary.opaque_area, 'thermal_boundary area is none')
         self.assertIsNotNone(thermal_boundary.thickness, 'thermal_boundary thickness is none')
         self.assertIsNotNone(thermal_boundary.type, 'thermal_boundary type is none')
         self.assertIsNotNone(thermal_boundary.thermal_openings, 'thermal_openings is none')
-        self.assertIsNotNone(thermal_boundary.construction_name, 'construction_name is none')
         self.assertIsNotNone(thermal_boundary.window_ratio, 'window_ratio is none')
         self.assertIsNone(thermal_boundary.windows_areas, 'windows_areas is not none')
         self.assertIsNotNone(thermal_boundary.u_value, 'u_value is none')
         self.assertIsNotNone(thermal_boundary.hi, 'hi is none')
         self.assertIsNotNone(thermal_boundary.he, 'he is none')
         self.assertIsNotNone(thermal_boundary.internal_surface, 'virtual_internal_surface is none')
         self.assertIsNotNone(thermal_boundary.layers, 'layers is not none')
 
   def _check_thermal_openings(self, thermal_boundary):
     for thermal_opening in thermal_boundary.thermal_openings:
       self.assertIsNotNone(thermal_opening.id, 'thermal opening id is not none')
-      self.assertIsNotNone(thermal_opening.construction_name, 'thermal opening construction is none')
       self.assertIsNotNone(thermal_opening.area, 'thermal opening area is not none')
       self.assertIsNotNone(thermal_opening.frame_ratio, 'thermal opening frame_ratio is none')
       self.assertIsNotNone(thermal_opening.g_value, 'thermal opening g_value is none')
       self.assertIsNotNone(thermal_opening.overall_u_value, 'thermal opening overall_u_value is none')
       self.assertIsNotNone(thermal_opening.hi, 'thermal opening hi is none')
       self.assertIsNotNone(thermal_opening.he, 'thermal opening he is none')
-      self.assertIsNotNone(thermal_opening.construction_name, 'thermal opening construction_name is none')
 
   def _check_surfaces(self, thermal_boundary):
-    external_surface = thermal_boundary.parent_surface
+    external_surface = thermal_boundary.external_surface
     internal_surface = thermal_boundary.internal_surface
     self.assertIsNotNone(external_surface.short_wave_reflectance,
                          'external surface short_wave_reflectance id is not none')
     self.assertIsNotNone(external_surface.long_wave_emittance, 'external surface long_wave_emittance id is not none')
     self.assertIsNotNone(internal_surface.short_wave_reflectance,
                          'external surface short_wave_reflectance id is not none')
     self.assertIsNotNone(internal_surface.long_wave_emittance, 'external surface long_wave_emittance id is not none')
@@ -180,15 +177,15 @@
       building.function = self._internal_function('hft', building.function)
     ConstructionFactory('nrcan', city).enrich()
 
     self._check_buildings(city)
     for building in city.buildings:
       for internal_zone in building.internal_zones:
         self._check_thermal_zones(internal_zone)
-        for thermal_zone in internal_zone.thermal_zones:
+        for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
           self._check_thermal_boundaries(thermal_zone)
           for thermal_boundary in thermal_zone.thermal_boundaries:
             self.assertIsNotNone(thermal_boundary.layers, 'layers is none')
             self._check_thermal_openings(thermal_boundary)
             self._check_surfaces(thermal_boundary)
 
     file = 'pluto_building.gml'
@@ -198,33 +195,15 @@
       building.function = self._internal_function('pluto', building.function)
     ConstructionFactory('nrcan', city).enrich()
 
     self._check_buildings(city)
     for building in city.buildings:
       for internal_zone in building.internal_zones:
         self._check_thermal_zones(internal_zone)
-        for thermal_zone in internal_zone.thermal_zones:
-          self._check_thermal_boundaries(thermal_zone)
-          for thermal_boundary in thermal_zone.thermal_boundaries:
-            self.assertIsNotNone(thermal_boundary.layers, 'layers is none')
-            self._check_thermal_openings(thermal_boundary)
-            self._check_surfaces(thermal_boundary)
-
-    file = 'one_building_in_kelowna.gml'
-    city = self._get_citygml(file)
-    for building in city.buildings:
-      building.year_of_construction = 2006
-      building.function = self._internal_function('hft', building.function)
-    ConstructionFactory('nrel', city).enrich()
-
-    self._check_buildings(city)
-    for building in city.buildings:
-      for internal_zone in building.internal_zones:
-        self._check_thermal_zones(internal_zone)
-        for thermal_zone in internal_zone.thermal_zones:
+        for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
           self._check_thermal_boundaries(thermal_zone)
           for thermal_boundary in thermal_zone.thermal_boundaries:
             self.assertIsNotNone(thermal_boundary.layers, 'layers is none')
             self._check_thermal_openings(thermal_boundary)
             self._check_surfaces(thermal_boundary)
 
     file = 'pluto_building.gml'
@@ -234,15 +213,15 @@
       building.function = self._internal_function('pluto', building.function)
     ConstructionFactory('nrel', city).enrich()
 
     self._check_buildings(city)
     for building in city.buildings:
       for internal_zone in building.internal_zones:
         self._check_thermal_zones(internal_zone)
-        for thermal_zone in internal_zone.thermal_zones:
+        for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
           self._check_thermal_boundaries(thermal_zone)
           for thermal_boundary in thermal_zone.thermal_boundaries:
             self.assertIsNotNone(thermal_boundary.layers, 'layers is none')
             self._check_thermal_openings(thermal_boundary)
             self._check_surfaces(thermal_boundary)
 
     file = 'one_building_in_kelowna.gml'
@@ -252,15 +231,15 @@
       building.function = self._internal_function('hft', building.function)
     ConstructionFactory('nrcan', city).enrich()
 
     self._check_buildings(city)
     for building in city.buildings:
       for internal_zone in building.internal_zones:
         self._check_thermal_zones(internal_zone)
-        for thermal_zone in internal_zone.thermal_zones:
+        for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
           self._check_thermal_boundaries(thermal_zone)
           for thermal_boundary in thermal_zone.thermal_boundaries:
             self.assertIsNotNone(thermal_boundary.layers, 'layers is none')
             self._check_thermal_openings(thermal_boundary)
             self._check_surfaces(thermal_boundary)
 
     file_path = (self._example_path / 'test.geojson').resolve()
@@ -273,15 +252,15 @@
 
     ConstructionFactory('nrcan', city).enrich()
 
     self._check_buildings(city)
     for building in city.buildings:
       for internal_zone in building.internal_zones:
         self._check_thermal_zones(internal_zone)
-        for thermal_zone in internal_zone.thermal_zones:
+        for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
           self._check_thermal_boundaries(thermal_zone)
           for thermal_boundary in thermal_zone.thermal_boundaries:
             self.assertIsNotNone(thermal_boundary.layers, 'layers is none')
             self._check_thermal_openings(thermal_boundary)
             self._check_surfaces(thermal_boundary)
 
   def test_nrcan_construction_factory(self):
@@ -295,15 +274,15 @@
                            function_to_hub=Dictionaries().montreal_function_to_hub_function).city
     ConstructionFactory('nrcan', city).enrich()
 
     self._check_buildings(city)
     for building in city.buildings:
       for internal_zone in building.internal_zones:
         self._check_thermal_zones(internal_zone)
-        for thermal_zone in internal_zone.thermal_zones:
+        for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
           self._check_thermal_boundaries(thermal_zone)
           for thermal_boundary in thermal_zone.thermal_boundaries:
             self.assertIsNotNone(thermal_boundary.layers, 'layers is none')
             self._check_thermal_openings(thermal_boundary)
             self._check_surfaces(thermal_boundary)
 
   def test_eilat_construction_factory(self):
@@ -317,13 +296,13 @@
                            function_to_hub=Dictionaries().eilat_function_to_hub_function).city
     ConstructionFactory('eilat', city).enrich()
 
     self._check_buildings(city)
     for building in city.buildings:
       for internal_zone in building.internal_zones:
         self._check_thermal_zones(internal_zone)
-        for thermal_zone in internal_zone.thermal_zones:
+        for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
           self._check_thermal_boundaries(thermal_zone)
           for thermal_boundary in thermal_zone.thermal_boundaries:
             self.assertIsNotNone(thermal_boundary.layers, 'layers is none')
             self._check_thermal_openings(thermal_boundary)
             self._check_surfaces(thermal_boundary)
```

### Comparing `cerc-hub-0.1.8.2/tests/test_costs_catalog.py` & `cerc-hub-0.1.8.3/tests/test_costs_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/tests/test_custom_insel_block.py` & `cerc-hub-0.1.8.3/tests/test_insel_exports.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 TestInselExports test
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2022 Concordia CERC group
 Project Coder Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
 """
-import logging
+
 from pathlib import Path
 from unittest import TestCase
 import pandas as pd
 import hub.helpers.constants as cte
 from hub.helpers.monthly_values import MonthlyValues
 from hub.imports.geometry_factory import GeometryFactory
 from hub.imports.construction_factory import ConstructionFactory
@@ -33,64 +33,49 @@
 
   def _get_citygml(self, file):
     file_path = (self._example_path / file).resolve()
     self._city = GeometryFactory('citygml', path=file_path).city
     self.assertIsNotNone(self._city, 'city is none')
     return self._city
 
-  @property
-  def _read_sra_file(self) -> []:
-    path = (self._example_path / "one_building_in_kelowna_sra_SW.out").resolve()
-    _results = pd.read_csv(path, sep='\s+', header=0)
-    id_building = ''
-    header_building = []
-    _radiation = []
-    for column in _results.columns.values:
-      if id_building != column.split(':')[1]:
-        id_building = column.split(':')[1]
-        if len(header_building) > 0:
-          _radiation.append(pd.concat([MonthlyValues().month_hour, _results[header_building]], axis=1))
-        header_building = [column]
-      else:
-        header_building.append(column)
-    _radiation.append(pd.concat([MonthlyValues().month_hour, _results[header_building]], axis=1))
-    return _radiation
-
   def _set_irradiance_surfaces(self, city):
     """
     saves in building surfaces the correspondent irradiance at different time-scales depending on the mode
     if building is None, it saves all buildings' surfaces in file, if building is specified, it saves only that
     specific building values
     :parameter city: city
     :return: none
     """
     city.level_of_detail.surface_radiation = 2
-    for radiation in self._read_sra_file:
-      city_object_name = radiation.columns.values.tolist()[1].split(':')[1]
-      building = city.city_object(city_object_name)
-      for column in radiation.columns.values:
-        if column == cte.MONTH:
-          continue
-        header_id = column
-        surface_id = header_id.split(':')[2]
-        surface = building.surface_by_id(surface_id)
-        new_value = pd.DataFrame(radiation[[header_id]].to_numpy(), columns=['sra'])
-        surface.global_irradiance[cte.HOUR] = new_value
-        month_new_value = MonthlyValues().get_mean_values(new_value)
-        surface.global_irradiance[cte.MONTH] = month_new_value
+    path = (self._example_path / "one_building_in_kelowna_sra_SW.out").resolve()
+    self._results = pd.read_csv(path, sep='\s+', header=0).to_dict(orient='list')
+    _irradiance = {}
+    for key in self._results:
+      header_name = key.split(':')
+      result = [x / cte.WATTS_HOUR_TO_JULES for x in self._results[key]]
+      city_object_name = header_name[1]
+      building = self._city.city_object(city_object_name)
+      surface_id = header_name[2]
+      surface = building.surface_by_id(surface_id)
+      monthly_result = MonthlyValues.get_total_month(result)
+      yearly_result = [sum(result)]
+      _irradiance[cte.YEAR] = yearly_result
+      _irradiance[cte.MONTH] = monthly_result
+      _irradiance[cte.HOUR] = result
+      surface.global_irradiance = _irradiance
 
   def test_insel_monthly_energy_balance_export(self):
     """
     export to Insel MonthlyEnergyBalance
     """
     city = self._get_citygml('one_building_in_kelowna.gml')
     WeatherFactory('epw', city).enrich()
     for building in city.buildings:
       building.external_temperature[cte.MONTH] = MonthlyValues().\
-        get_mean_values(building.external_temperature[cte.HOUR][['epw']])
+        get_mean_values(building.external_temperature[cte.HOUR])
     self._set_irradiance_surfaces(city)
 
     for building in city.buildings:
       self.assertIsNotNone(building.external_temperature[cte.MONTH], f'building {building.name} '
                                                                      f'external_temperature is none')
       for surface in building.surfaces:
         if surface.type != 'Ground':
@@ -111,15 +96,15 @@
       self.assertIsNotNone(building.volume, f'building {building.name} volume is none')
       self.assertIsNotNone(building.average_storey_height, f'building {building.name} average_storey_height is none')
       self.assertIsNotNone(building.storeys_above_ground, f'building {building.name} storeys_above_ground is none')
       self.assertIsNotNone(building.attic_heated, f'building {building.name} attic_heated is none')
       self.assertIsNotNone(building.basement_heated, f'building {building.name} basement_heated is none')
       for internal_zone in building.internal_zones:
         self.assertIsNotNone(internal_zone.area, f'internal zone {internal_zone.id} area is none')
-        for thermal_zone in internal_zone.thermal_zones:
+        for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
           self.assertIsNotNone(thermal_zone.indirectly_heated_area_ratio, f'thermal zone {thermal_zone.id} '
                                                                           f'indirectly_heated_area_ratio is none')
           self.assertIsNotNone(thermal_zone.effective_thermal_capacity, f'thermal zone {thermal_zone.id} '
                                                                         f'effective_thermal_capacity is none')
           self.assertIsNotNone(thermal_zone.additional_thermal_bridge_u_value, f'thermal zone {thermal_zone.id} '
                                                                                f'additional_thermal_bridge_u_value '
                                                                                f'is none')
@@ -128,25 +113,24 @@
           for thermal_boundary in thermal_zone.thermal_boundaries:
             self.assertIsNotNone(thermal_boundary.type)
             self.assertIsNotNone(thermal_boundary.opaque_area)
             self.assertIsNotNone(thermal_boundary.window_ratio)
             self.assertIsNotNone(thermal_boundary.u_value)
             self.assertIsNotNone(thermal_boundary.thermal_openings)
             if thermal_boundary.type is not cte.GROUND:
-              self.assertIsNotNone(thermal_boundary.parent_surface.short_wave_reflectance)
+              self.assertIsNotNone(thermal_boundary.external_surface.short_wave_reflectance)
 
         for usage in internal_zone.usages:
           self.assertIsNotNone(usage.percentage, f'usage zone {usage.name} percentage is none')
           self.assertIsNotNone(usage.internal_gains, f'usage zone {usage.name} internal_gains is none')
           self.assertIsNotNone(usage.thermal_control, f'usage zone {usage.name} thermal_control is none')
           self.assertIsNotNone(usage.hours_day, f'usage zone {usage.name} hours_day is none')
           self.assertIsNotNone(usage.days_year, f'usage zone {usage.name} days_year is none')
           self.assertIsNotNone(
             usage.mechanical_air_change,
             f'usage zone {usage.name} mechanical_air_change is none'
           )
     # export files
     try:
-      EnergyBuildingsExportsFactory('insel_monthly_energy_balance', city, self._output_path, 'MEB_Montreal').export()
-    except Exception as err:
-      logging.exception(err)
+      EnergyBuildingsExportsFactory('insel_monthly_energy_balance', city, self._output_path).export()
+    except Exception:
       self.fail("Insel MonthlyEnergyBalance ExportsFactory raised ExceptionType unexpectedly!")
```

### Comparing `cerc-hub-0.1.8.2/tests/test_db_factory.py` & `cerc-hub-0.1.8.3/tests/test_db_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     self._application_id = self._database.persist_application(
       'City_layers',
       'City layers test user',
       self.application_uuid
     )
     self._user_id = self._database.create_user('city_layers', self._application_id, 'city_layers', UserRoles.Admin)
 
-    self._pickle_path = 'tests_data/pickle_path.bz2'
+    self._pickle_path = Path('tests_data/pickle_path.bz2').resolve()
 
   @property
   def database(self):
     return self._database
 
   @property
   def application_uuid(self):
@@ -179,15 +179,14 @@
     city_id = control.database.persist_city(
       control.city,
       control.pickle_path,
       control.city.name,
       control.application_id,
       control.user_id)
     control.database.delete_city(city_id)
-    os.unlink(control.pickle_path)
 
   @unittest.skipIf(control.skip_test, control.skip_reason)
   def test_get_update_city(self):
     city_id = control.database.persist_city(control.city,
                                             control.pickle_path,
                                             control.city.name,
                                             control.application_id,
@@ -221,55 +220,57 @@
       yearly_cooling_peak_load = building.cooling_peak_load[cte.YEAR]
       monthly_heating_peak_load = building.heating_peak_load[cte.MONTH]
       yearly_heating_peak_load = building.heating_peak_load[cte.YEAR]
       monthly_lighting_peak_load = building.lighting_peak_load[cte.MONTH]
       yearly_lighting_peak_load = building.lighting_peak_load[cte.YEAR]
       monthly_appliances_peak_load = building.appliances_peak_load[cte.MONTH]
       yearly_appliances_peak_load = building.appliances_peak_load[cte.YEAR]
-      monthly_cooling_demand = building.cooling_demand[cte.MONTH][cte.INSEL_MEB]
-      yearly_cooling_demand = building.cooling_demand[cte.YEAR][cte.INSEL_MEB]
-      monthly_heating_demand = building.heating_demand[cte.MONTH][cte.INSEL_MEB]
-      yearly_heating_demand = building.heating_demand[cte.YEAR][cte.INSEL_MEB]
-      monthly_lighting_electrical_demand = building.lighting_electrical_demand[cte.MONTH][cte.INSEL_MEB]
-      yearly_lighting_electrical_demand = building.lighting_electrical_demand[cte.YEAR][cte.INSEL_MEB]
-      monthly_appliances_electrical_demand = building.appliances_electrical_demand[cte.MONTH][cte.INSEL_MEB]
-      yearly_appliances_electrical_demand = building.appliances_electrical_demand[cte.YEAR][cte.INSEL_MEB]
-      monthly_domestic_hot_water_heat_demand = building.domestic_hot_water_heat_demand[cte.MONTH][cte.INSEL_MEB]
-      yearly_domestic_hot_water_heat_demand = building.domestic_hot_water_heat_demand[cte.YEAR][cte.INSEL_MEB]
+      monthly_cooling_demand = building.cooling_demand[cte.MONTH]
+      yearly_cooling_demand = building.cooling_demand[cte.YEAR]
+      monthly_heating_demand = building.heating_demand[cte.MONTH]
+      yearly_heating_demand = building.heating_demand[cte.YEAR]
+      monthly_lighting_electrical_demand = building.lighting_electrical_demand[cte.MONTH]
+      yearly_lighting_electrical_demand = building.lighting_electrical_demand[cte.YEAR]
+      monthly_appliances_electrical_demand = building.appliances_electrical_demand[cte.MONTH]
+      yearly_appliances_electrical_demand = building.appliances_electrical_demand[cte.YEAR]
+      monthly_domestic_hot_water_heat_demand = building.domestic_hot_water_heat_demand[cte.MONTH]
+      yearly_domestic_hot_water_heat_demand = building.domestic_hot_water_heat_demand[cte.YEAR]
       monthly_heating_consumption = building.heating_consumption[cte.MONTH]
       yearly_heating_consumption = building.heating_consumption[cte.YEAR]
       monthly_cooling_consumption = building.cooling_consumption[cte.MONTH]
       yearly_cooling_consumption = building.cooling_consumption[cte.YEAR]
       monthly_domestic_hot_water_consumption = building.domestic_hot_water_consumption[cte.MONTH]
       yearly_domestic_hot_water_consumption = building._domestic_hot_water_consumption[cte.YEAR]
       monthly_distribution_systems_electrical_consumption = building.distribution_systems_electrical_consumption[
         cte.MONTH]
       yearly_distribution_systems_electrical_consumption = building.distribution_systems_electrical_consumption[
         cte.YEAR]
-      monthly_on_site_electrical_production = building.onsite_electrical_production[cte.MONTH]
-      yearly_on_site_electrical_production = building.onsite_electrical_production[cte.YEAR]
+      monthly_on_site_electrical_production = [x * cte.WATTS_HOUR_TO_JULES
+                                               for x in building.onsite_electrical_production[cte.MONTH]]
+      yearly_on_site_electrical_production = [x * cte.WATTS_HOUR_TO_JULES
+                                              for x in building.onsite_electrical_production[cte.YEAR]]
       results = json.dumps({cte.INSEL_MEB: [
         {'monthly_cooling_peak_load': monthly_cooling_peak_load},
         {'yearly_cooling_peak_load': yearly_cooling_peak_load},
         {'monthly_heating_peak_load': monthly_heating_peak_load},
         {'yearly_heating_peak_load': yearly_heating_peak_load},
         {'monthly_lighting_peak_load': monthly_lighting_peak_load},
         {'yearly_lighting_peak_load': yearly_lighting_peak_load},
         {'monthly_appliances_peak_load': monthly_appliances_peak_load},
         {'yearly_appliances_peak_load': yearly_appliances_peak_load},
-        {'monthly_cooling_demand': monthly_cooling_demand.tolist()},
-        {'yearly_cooling_demand': yearly_cooling_demand.tolist()},
-        {'monthly_heating_demand': monthly_heating_demand.tolist()},
-        {'yearly_heating_demand': yearly_heating_demand.tolist()},
-        {'monthly_lighting_electrical_demand': monthly_lighting_electrical_demand.tolist()},
-        {'yearly_lighting_electrical_demand': yearly_lighting_electrical_demand.tolist()},
-        {'monthly_appliances_electrical_demand': monthly_appliances_electrical_demand.tolist()},
-        {'yearly_appliances_electrical_demand': yearly_appliances_electrical_demand.tolist()},
-        {'monthly_domestic_hot_water_heat_demand': monthly_domestic_hot_water_heat_demand.tolist()},
-        {'yearly_domestic_hot_water_heat_demand': yearly_domestic_hot_water_heat_demand.tolist()},
+        {'monthly_cooling_demand': monthly_cooling_demand},
+        {'yearly_cooling_demand': yearly_cooling_demand},
+        {'monthly_heating_demand': monthly_heating_demand},
+        {'yearly_heating_demand': yearly_heating_demand},
+        {'monthly_lighting_electrical_demand': monthly_lighting_electrical_demand},
+        {'yearly_lighting_electrical_demand': yearly_lighting_electrical_demand},
+        {'monthly_appliances_electrical_demand': monthly_appliances_electrical_demand},
+        {'yearly_appliances_electrical_demand': yearly_appliances_electrical_demand},
+        {'monthly_domestic_hot_water_heat_demand': monthly_domestic_hot_water_heat_demand},
+        {'yearly_domestic_hot_water_heat_demand': yearly_domestic_hot_water_heat_demand},
         {'monthly_heating_consumption': monthly_heating_consumption},
         {'yearly_heating_consumption': yearly_heating_consumption},
         {'monthly_cooling_consumption': monthly_cooling_consumption},
         {'yearly_cooling_consumption': yearly_cooling_consumption},
         {'monthly_domestic_hot_water_consumption': monthly_domestic_hot_water_consumption},
         {'yearly_domestic_hot_water_consumption': yearly_domestic_hot_water_consumption},
         {'monthly_distribution_systems_electrical_consumption': monthly_distribution_systems_electrical_consumption},
@@ -290,7 +291,8 @@
     control.database.delete_city(city_id)
 
   @classmethod
   @unittest.skipIf(control.skip_test, control.skip_reason)
   def tearDownClass(cls):
     control.database.delete_application(control.application_uuid)
     control.database.delete_user(control.user_id)
+    os.unlink(control.pickle_path)
```

### Comparing `cerc-hub-0.1.8.2/tests/test_db_retrieve.py` & `cerc-hub-0.1.8.3/tests/test_db_retrieve.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/tests/test_enrichement.py` & `cerc-hub-0.1.8.3/tests/test_enrichement.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,23 +34,23 @@
   def _check_result(self, city):
     self._check_buildings(city)
     for building in city.buildings:
       for internal_zone in building.internal_zones:
         self.assertIsNot(len(internal_zone.usages), 0, 'no building usages defined')
         for usage in internal_zone.usages:
           self.assertIsNotNone(usage.id, 'usage id is none')
-        for thermal_zone in internal_zone.thermal_zones:
+        for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
           self._check_thermal_zone(thermal_zone)
 
   def _check_buildings(self, city):
     for building in city.buildings:
       self.assertIsNotNone(building.internal_zones, 'no internal zones created')
       for internal_zone in building.internal_zones:
         self.assertIsNotNone(internal_zone.usages, 'usage zones are not defined')
-        self.assertIsNotNone(internal_zone.thermal_zones, 'thermal zones are not defined')
+        self.assertIsNotNone(internal_zone.thermal_zones_from_internal_zones, 'thermal zones are not defined')
       self.assertIsNone(building.basement_heated, 'building basement_heated is not none')
       self.assertIsNone(building.attic_heated, 'building attic_heated is not none')
       self.assertIsNotNone(building.average_storey_height, 'building average_storey_height is none')
       self.assertIsNotNone(building.storeys_above_ground, 'building storeys_above_ground is none')
       self.assertTrue(building.is_conditioned, 'building is_conditioned is not conditioned')
 
   def _check_thermal_zone(self, thermal_zone):
@@ -101,27 +101,27 @@
           building.year_of_construction = 2006
         self.assertTrue(len(city.buildings) > 0)
         self._prepare_case_construction_first(city, 'hft', construction_key, usage_key)
         self._check_result(city)
         if usage_key == 'comnet':
           for building in city.buildings:
             for internal_zone in building.internal_zones:
-              for thermal_zone in internal_zone.thermal_zones:
+              for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
                 self._check_extra_thermal_zone(thermal_zone)
         # usage factory called first
         city = self._get_citygml(file)
         for building in city.buildings:
           building.year_of_construction = 2006
         self.assertTrue(len(city.buildings) > 0)
         self._prepare_case_usage_first(city, 'hft', construction_key, usage_key)
         self._check_result(city)
         if usage_key == 'comnet':
           for building in city.buildings:
             for internal_zone in building.internal_zones:
-              for thermal_zone in internal_zone.thermal_zones:
+              for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
                 self._check_extra_thermal_zone(thermal_zone)
 
   def _test_pluto(self, file):
     _construction_keys = ['nrel']
     _usage_keys = ['comnet', 'nrcan']
     for construction_key in _construction_keys:
       for usage_key in _usage_keys:
@@ -131,27 +131,27 @@
           building.year_of_construction = 2006
         self.assertTrue(len(city.buildings) > 0)
         self._prepare_case_construction_first(city, 'pluto', construction_key, usage_key)
         self._check_result(city)
         if usage_key == 'comnet':
           for building in city.buildings:
             for internal_zone in building.internal_zones:
-              for thermal_zone in internal_zone.thermal_zones:
+              for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
                 self._check_extra_thermal_zone(thermal_zone)
         # usage factory called first
         city = self._get_citygml(file)
         for building in city.buildings:
           building.year_of_construction = 2006
         self.assertTrue(len(city.buildings) > 0)
         self._prepare_case_usage_first(city, 'pluto', construction_key, usage_key)
         self._check_result(city)
         if usage_key == 'comnet':
           for building in city.buildings:
             for internal_zone in building.internal_zones:
-              for thermal_zone in internal_zone.thermal_zones:
+              for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
                 self._check_extra_thermal_zone(thermal_zone)
 
   def test_enrichment(self):
     """
     Test enrichment of the city with different orders
     :return: None
     """
```

### Comparing `cerc-hub-0.1.8.2/tests/test_exports.py` & `cerc-hub-0.1.8.3/tests/test_exports.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 TestExports test and validate the city export formats
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2022 Concordia CERC group
 Project Coder Guille Gutierrez guillermo.gutierrezmorote@concordia.ca
 Code contributors: Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
 """
+
 import logging.handlers
 from pathlib import Path
 from unittest import TestCase
-import pandas as pd
 from hub.imports.geometry_factory import GeometryFactory
 from hub.helpers.dictionaries import Dictionaries
 from hub.imports.construction_factory import ConstructionFactory
 from hub.imports.usage_factory import UsageFactory
 from hub.imports.weather_factory import WeatherFactory
 from hub.exports.exports_factory import ExportsFactory
 from hub.exports.energy_building_exports_factory import EnergyBuildingsExportsFactory
@@ -54,18 +54,18 @@
         ConstructionFactory('nrel', self._complete_city).enrich()
         UsageFactory('nrcan', self._complete_city).enrich()
         cli = (self._example_path / 'weather' / 'inseldb_Summerland.cli').resolve()
         self._complete_city.climate_file = Path(cli)
         self._complete_city.climate_reference_city = 'Summerland'
         dummy_measures = [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
         for building in self._complete_city.buildings:
-          building.heating_demand[cte.MONTH] = pd.DataFrame({'INSEL': dummy_measures})
-          building.cooling_demand[cte.MONTH] = pd.DataFrame({'INSEL': dummy_measures})
-          building.heating_demand[cte.YEAR] = pd.DataFrame({'INSEL': [0.0]})
-          building.cooling_demand[cte.YEAR] = pd.DataFrame({'INSEL': [0.0]})
+          building.heating_demand[cte.MONTH] = dummy_measures
+          building.cooling_demand[cte.MONTH] = dummy_measures
+          building.heating_demand[cte.YEAR] = [0.0]
+          building.cooling_demand[cte.YEAR] = [0.0]
     return self._complete_city
 
   def _export(self, export_type, from_pickle=False):
     self._complete_city = self._get_complete_city(from_pickle)
     try:
       ExportsFactory(export_type, self._complete_city, self._output_path).export()
     except ValueError as err:
@@ -116,12 +116,13 @@
 
     self.assertIsNotNone(city, 'city is none')
     EnergyBuildingsExportsFactory('idf', city, self._output_path).export()
     ConstructionFactory('nrcan', city).enrich()
     EnergyBuildingsExportsFactory('idf', city, self._output_path).export()
     UsageFactory('nrcan', city).enrich()
     WeatherFactory('epw', city).enrich()
+    print(self._output_path)
     try:
       EnergyBuildingsExportsFactory('idf', city, self._output_path).export()
     except Exception:
       self.fail("Idf ExportsFactory raised ExceptionType unexpectedly!")
```

### Comparing `cerc-hub-0.1.8.2/tests/test_geometry_factory.py` & `cerc-hub-0.1.8.3/tests/test_geometry_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
       self.assertIsNotNone(building.internal_zones, 'no internal zones created')
       self.assertIsNotNone(building.grounds, 'building grounds is none')
       self.assertIsNotNone(building.walls, 'building walls is none')
       self.assertIsNotNone(building.roofs, 'building roofs is none')
       self.assertIsNotNone(building.internal_zones, 'building internal zones is none')
       for internal_zone in building.internal_zones:
         self.assertIsNone(internal_zone.usages, 'usage zones are defined')
-        self.assertIsNone(internal_zone.thermal_zones, 'thermal zones are defined')
+        self.assertIsNone(internal_zone.thermal_archetype, 'thermal archetype is defined')
       self.assertIsNone(building.basement_heated, 'building basement_heated is not none')
       self.assertIsNone(building.attic_heated, 'building attic_heated is not none')
       self.assertIsNone(building.terrains, 'building terrains is not none')
       self.assertIsNone(building.average_storey_height, 'building average_storey_height is not none')
       self.assertIsNone(building.storeys_above_ground, 'building storeys_above_ground is not none')
       self.assertEqual(len(building.heating_demand), 0, 'building heating is not none')
       self.assertEqual(len(building.cooling_demand), 0, 'building cooling is not none')
```

### Comparing `cerc-hub-0.1.8.2/tests/test_greenery_catalog.py` & `cerc-hub-0.1.8.3/tests/test_greenery_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/tests/test_greenery_in_idf.py` & `cerc-hub-0.1.8.3/tests/test_greenery_in_idf.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/tests/test_insel_exports.py` & `cerc-hub-0.1.8.3/tests/test_custom_insel_block.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 TestInselExports test
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2022 Concordia CERC group
 Project Coder Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
 """
-
+import logging
 from pathlib import Path
 from unittest import TestCase
 import pandas as pd
 import hub.helpers.constants as cte
 from hub.helpers.monthly_values import MonthlyValues
 from hub.imports.geometry_factory import GeometryFactory
 from hub.imports.construction_factory import ConstructionFactory
@@ -33,64 +33,49 @@
 
   def _get_citygml(self, file):
     file_path = (self._example_path / file).resolve()
     self._city = GeometryFactory('citygml', path=file_path).city
     self.assertIsNotNone(self._city, 'city is none')
     return self._city
 
-  @property
-  def _read_sra_file(self) -> []:
-    path = (self._example_path / "one_building_in_kelowna_sra_SW.out").resolve()
-    _results = pd.read_csv(path, sep='\s+', header=0)
-    id_building = ''
-    header_building = []
-    _radiation = []
-    for column in _results.columns.values:
-      if id_building != column.split(':')[1]:
-        id_building = column.split(':')[1]
-        if len(header_building) > 0:
-          _radiation.append(pd.concat([MonthlyValues().month_hour, _results[header_building]], axis=1))
-        header_building = [column]
-      else:
-        header_building.append(column)
-    _radiation.append(pd.concat([MonthlyValues().month_hour, _results[header_building]], axis=1))
-    return _radiation
-
   def _set_irradiance_surfaces(self, city):
     """
     saves in building surfaces the correspondent irradiance at different time-scales depending on the mode
     if building is None, it saves all buildings' surfaces in file, if building is specified, it saves only that
     specific building values
     :parameter city: city
     :return: none
     """
     city.level_of_detail.surface_radiation = 2
-    for radiation in self._read_sra_file:
-      city_object_name = radiation.columns.values.tolist()[1].split(':')[1]
-      building = city.city_object(city_object_name)
-      for column in radiation.columns.values:
-        if column == cte.MONTH:
-          continue
-        header_id = column
-        surface_id = header_id.split(':')[2]
-        surface = building.surface_by_id(surface_id)
-        new_value = pd.DataFrame(radiation[[header_id]].to_numpy(), columns=['sra'])
-        surface.global_irradiance[cte.HOUR] = new_value
-        month_new_value = MonthlyValues().get_mean_values(new_value)
-        surface.global_irradiance[cte.MONTH] = month_new_value
+    path = (self._example_path / "one_building_in_kelowna_sra_SW.out").resolve()
+    self._results = pd.read_csv(path, sep='\s+', header=0).to_dict(orient='list')
+    _irradiance = {}
+    for key in self._results:
+      header_name = key.split(':')
+      result = [x / cte.WATTS_HOUR_TO_JULES for x in self._results[key]]
+      city_object_name = header_name[1]
+      building = self._city.city_object(city_object_name)
+      surface_id = header_name[2]
+      surface = building.surface_by_id(surface_id)
+      monthly_result = MonthlyValues.get_total_month(result)
+      yearly_result = [sum(result)]
+      _irradiance[cte.YEAR] = yearly_result
+      _irradiance[cte.MONTH] = monthly_result
+      _irradiance[cte.HOUR] = result
+      surface.global_irradiance = _irradiance
 
   def test_insel_monthly_energy_balance_export(self):
     """
     export to Insel MonthlyEnergyBalance
     """
     city = self._get_citygml('one_building_in_kelowna.gml')
     WeatherFactory('epw', city).enrich()
     for building in city.buildings:
       building.external_temperature[cte.MONTH] = MonthlyValues().\
-        get_mean_values(building.external_temperature[cte.HOUR][['epw']])
+        get_mean_values(building.external_temperature[cte.HOUR])
     self._set_irradiance_surfaces(city)
 
     for building in city.buildings:
       self.assertIsNotNone(building.external_temperature[cte.MONTH], f'building {building.name} '
                                                                      f'external_temperature is none')
       for surface in building.surfaces:
         if surface.type != 'Ground':
@@ -111,41 +96,43 @@
       self.assertIsNotNone(building.volume, f'building {building.name} volume is none')
       self.assertIsNotNone(building.average_storey_height, f'building {building.name} average_storey_height is none')
       self.assertIsNotNone(building.storeys_above_ground, f'building {building.name} storeys_above_ground is none')
       self.assertIsNotNone(building.attic_heated, f'building {building.name} attic_heated is none')
       self.assertIsNotNone(building.basement_heated, f'building {building.name} basement_heated is none')
       for internal_zone in building.internal_zones:
         self.assertIsNotNone(internal_zone.area, f'internal zone {internal_zone.id} area is none')
-        for thermal_zone in internal_zone.thermal_zones:
+        for thermal_zone in internal_zone.thermal_zones_from_internal_zones:
           self.assertIsNotNone(thermal_zone.indirectly_heated_area_ratio, f'thermal zone {thermal_zone.id} '
                                                                           f'indirectly_heated_area_ratio is none')
           self.assertIsNotNone(thermal_zone.effective_thermal_capacity, f'thermal zone {thermal_zone.id} '
                                                                         f'effective_thermal_capacity is none')
           self.assertIsNotNone(thermal_zone.additional_thermal_bridge_u_value, f'thermal zone {thermal_zone.id} '
                                                                                f'additional_thermal_bridge_u_value '
                                                                                f'is none')
           self.assertIsNotNone(thermal_zone.total_floor_area, f'thermal zone {thermal_zone.id} '
                                                               f'total_floor_area is none')
           for thermal_boundary in thermal_zone.thermal_boundaries:
             self.assertIsNotNone(thermal_boundary.type)
             self.assertIsNotNone(thermal_boundary.opaque_area)
-            self.assertIsNotNone(thermal_boundary.window_ratio)
+            if thermal_boundary.type in (cte.WALL, cte.ROOF):
+              self.assertIsNotNone(thermal_boundary.window_ratio)
             self.assertIsNotNone(thermal_boundary.u_value)
             self.assertIsNotNone(thermal_boundary.thermal_openings)
             if thermal_boundary.type is not cte.GROUND:
-              self.assertIsNotNone(thermal_boundary.parent_surface.short_wave_reflectance)
+              self.assertIsNotNone(thermal_boundary.external_surface.short_wave_reflectance)
 
         for usage in internal_zone.usages:
           self.assertIsNotNone(usage.percentage, f'usage zone {usage.name} percentage is none')
           self.assertIsNotNone(usage.internal_gains, f'usage zone {usage.name} internal_gains is none')
           self.assertIsNotNone(usage.thermal_control, f'usage zone {usage.name} thermal_control is none')
           self.assertIsNotNone(usage.hours_day, f'usage zone {usage.name} hours_day is none')
           self.assertIsNotNone(usage.days_year, f'usage zone {usage.name} days_year is none')
           self.assertIsNotNone(
             usage.mechanical_air_change,
             f'usage zone {usage.name} mechanical_air_change is none'
           )
     # export files
     try:
-      EnergyBuildingsExportsFactory('insel_monthly_energy_balance', city, self._output_path).export()
-    except Exception:
+      EnergyBuildingsExportsFactory('insel_monthly_energy_balance', city, self._output_path, 'MEB_Montreal').export()
+    except Exception as err:
+      logging.exception(err)
       self.fail("Insel MonthlyEnergyBalance ExportsFactory raised ExceptionType unexpectedly!")
```

### Comparing `cerc-hub-0.1.8.2/tests/test_results_import.py` & `cerc-hub-0.1.8.3/tests/test_results_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 TestExports test and validate the city export formats
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2022 Concordia CERC group
 Project Coder Guille Gutierrez guillermo.gutierrezmorote@concordia.ca
 """
+
 import subprocess
 from pathlib import Path
 from unittest import TestCase
 
-import pandas as pd
-
 import hub.helpers.constants as cte
 from hub.exports.energy_building_exports_factory import EnergyBuildingsExportsFactory
 from hub.exports.exports_factory import ExportsFactory
 from hub.helpers.dictionaries import Dictionaries
 from hub.imports.construction_factory import ConstructionFactory
 from hub.imports.geometry_factory import GeometryFactory
 from hub.imports.results_factory import ResultFactory
@@ -61,18 +60,18 @@
     EnergyBuildingsExportsFactory('insel_monthly_energy_balance', self._city, self._output_path).export()
     for building in self._city.buildings:
       insel_path = (self._output_path / f'{building.name}.insel')
       subprocess.run(['insel', str(insel_path)])
     ResultFactory('insel_monthly_energy_balance', self._city, self._output_path).enrich()
     # Check that all the buildings have heating and cooling values
     for building in self._city.buildings:
-      self.assertIsNotNone(building.heating_demand[cte.MONTH][cte.INSEL_MEB])
-      self.assertIsNotNone(building.cooling_demand[cte.MONTH][cte.INSEL_MEB])
-      self.assertIsNotNone(building.heating_demand[cte.YEAR][cte.INSEL_MEB])
-      self.assertIsNotNone(building.cooling_demand[cte.YEAR][cte.INSEL_MEB])
+      self.assertIsNotNone(building.heating_demand[cte.MONTH])
+      self.assertIsNotNone(building.cooling_demand[cte.MONTH])
+      self.assertIsNotNone(building.heating_demand[cte.YEAR])
+      self.assertIsNotNone(building.cooling_demand[cte.YEAR])
       self.assertIsNotNone(building.lighting_peak_load[cte.MONTH])
       self.assertIsNotNone(building.lighting_peak_load[cte.YEAR])
       self.assertIsNotNone(building.appliances_peak_load[cte.MONTH])
       self.assertIsNotNone(building.appliances_peak_load[cte.YEAR])
 
   def test_peak_loads(self):
     # todo: this is not technically a import
@@ -85,11 +84,11 @@
       self.assertIsNotNone(building.cooling_peak_load)
 
     values = [0 for _ in range(8760)]
     values[0] = 1000
     expected_monthly_list = [0 for _ in range(12)]
     expected_monthly_list[0] = 1000
     for building in self._city.buildings:
-      building.heating_demand[cte.HOUR] = pd.DataFrame(values, columns=['dummy'])
-      building.cooling_demand[cte.HOUR] = pd.DataFrame(values, columns=['dummy'])
+      building.heating_demand[cte.HOUR] = values
+      building.cooling_demand[cte.HOUR] = values
       self.assertIsNotNone(building.heating_peak_load)
       self.assertIsNotNone(building.cooling_peak_load)
```

### Comparing `cerc-hub-0.1.8.2/tests/test_systems_catalog.py` & `cerc-hub-0.1.8.3/tests/test_systems_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/tests/test_systems_factory.py` & `cerc-hub-0.1.8.3/tests/test_systems_factory.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -111,8 +111,8 @@
           _building_energy_systems.append(_building_energy_equipment)
       building.energy_systems = _building_energy_systems
 
     for building in self._city.buildings:
       self.assertLess(0, building.heating_consumption[cte.YEAR][0])
       self.assertLess(0, building.cooling_consumption[cte.YEAR][0])
       self.assertLess(0, building.domestic_hot_water_consumption[cte.YEAR][0])
-      self.assertLess(0, building.onsite_electrical_production[cte.YEAR][0])
+      self.assertLess(0, building.onsite_electrical_production[cte.YEAR][0])
```

### Comparing `cerc-hub-0.1.8.2/tests/test_usage_catalog.py` & `cerc-hub-0.1.8.3/tests/test_usage_catalog.py`

 * *Files identical despite different names*

### Comparing `cerc-hub-0.1.8.2/tests/test_usage_factory.py` & `cerc-hub-0.1.8.3/tests/test_usage_factory.py`

 * *Files identical despite different names*

