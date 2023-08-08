# Comparing `tmp/odoo13-addon-photovoltaic_api-13.0.1.1.5.tar.gz` & `tmp/odoo13-addon-photovoltaic_api-13.0.1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo13-addon-photovoltaic_api-13.0.1.1.5.tar", last modified: Wed Jul  5 08:05:46 2023, max compression
+gzip compressed data, was "odoo13-addon-photovoltaic_api-13.0.1.1.6.tar", last modified: Tue Aug  8 09:44:38 2023, max compression
```

## Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5.tar` & `odoo13-addon-photovoltaic_api-13.0.1.1.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:05:46.819830 odoo13-addon-photovoltaic_api-13.0.1.1.5/
--rw-r--r--   0 root         (0) root         (0)      448 2023-07-05 08:05:46.819830 odoo13-addon-photovoltaic_api-13.0.1.1.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:05:46.811830 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:05:46.811830 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:05:46.814830 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/
--rw-rw-rw-   0 root         (0) root         (0)     1275 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      954 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:05:46.814830 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/controllers/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/controllers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/controllers/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:05:46.814830 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/data/
--rw-rw-rw-   0 root         (0) root         (0)     3883 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/data/data.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:05:46.815830 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/models/
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/models/auth_jwt_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:05:46.816830 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/pydantic_models/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/pydantic_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/pydantic_models/allocation.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/pydantic_models/bank_account.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/pydantic_models/contract.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/pydantic_models/info.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/pydantic_models/list_response.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/pydantic_models/power_station.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/pydantic_models/power_station_production.py
--rw-rw-rw-   0 root         (0) root         (0)     1991 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/pydantic_models/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:05:46.816830 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/security/
--rw-rw-rw-   0 root         (0) root         (0)     2578 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/security/ir.model.access.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:05:46.817830 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/services/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4683 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/services/account.py
--rw-rw-rw-   0 root         (0) root         (0)     4970 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/services/allocations.py
--rw-rw-rw-   0 root         (0) root         (0)     3533 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/services/bank_account.py
--rw-rw-rw-   0 root         (0) root         (0)     5989 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/services/contracts.py
--rw-rw-rw-   0 root         (0) root         (0)     2057 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/services/info.py
--rw-rw-rw-   0 root         (0) root         (0)     3290 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/services/powerstation.py
--rw-rw-rw-   0 root         (0) root         (0)     5410 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/services/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:05:46.818830 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/tests/
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1640 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/tests/common.py
--rw-rw-rw-   0 root         (0) root         (0)     6052 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/tests/test_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:05:46.819830 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo13_addon_photovoltaic_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      448 2023-07-05 08:05:46.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo13_addon_photovoltaic_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1850 2023-07-05 08:05:46.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:05:46.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo13_addon_photovoltaic_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:05:46.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo13_addon_photovoltaic_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      212 2023-07-05 08:05:46.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo13_addon_photovoltaic_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-05 08:05:46.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo13_addon_photovoltaic_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 08:05:46.819830 odoo13-addon-photovoltaic_api-13.0.1.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-07-05 08:05:30.000000 odoo13-addon-photovoltaic_api-13.0.1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:44:38.237425 odoo13-addon-photovoltaic_api-13.0.1.1.6/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-08-08 09:44:38.237425 odoo13-addon-photovoltaic_api-13.0.1.1.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:44:38.227425 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:44:38.227425 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:44:38.229425 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:44:38.230425 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/controllers/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/controllers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/controllers/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:44:38.230425 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/data/
+-rw-rw-rw-   0 root         (0) root         (0)     3883 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/data/data.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:44:38.230425 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/models/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/models/auth_jwt_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:44:38.232425 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/pydantic_models/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/pydantic_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/pydantic_models/allocation.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/pydantic_models/bank_account.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/pydantic_models/contract.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/pydantic_models/info.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/pydantic_models/list_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/pydantic_models/power_station.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/pydantic_models/power_station_production.py
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/pydantic_models/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:44:38.232425 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/security/
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/security/ir.model.access.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:44:38.234425 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/services/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4683 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/services/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     4970 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/services/allocations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3533 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/services/bank_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     5989 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/services/contracts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2057 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/services/info.py
+-rw-rw-rw-   0 root         (0) root         (0)     4925 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/services/powerstation.py
+-rw-rw-rw-   0 root         (0) root         (0)     5410 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/services/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:44:38.235425 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/tests/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     6052 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/tests/test_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:44:38.236425 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo13_addon_photovoltaic_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-08-08 09:44:38.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo13_addon_photovoltaic_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-08-08 09:44:38.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 09:44:38.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo13_addon_photovoltaic_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 09:44:38.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo13_addon_photovoltaic_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      212 2023-08-08 09:44:38.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo13_addon_photovoltaic_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-08 09:44:38.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo13_addon_photovoltaic_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 09:44:38.237425 odoo13-addon-photovoltaic_api-13.0.1.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-08-08 09:44:19.000000 odoo13-addon-photovoltaic_api-13.0.1.1.6/setup.py
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/CHANGELOG.md` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 All notable changes to this project will be documented in this file. (from version 13.0.1.1.0 onwards)
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [13.0.1.1.6] - 08-08-2023
+
+### Added
+- New endpoint to retrieve powerstations open for investment
+
 ## [13.0.1.1.5] - 05-06-2023
 
 ### Added 
 - New endpoint to allow synchronization with mailchimp via mailchimp webhooks
 
 
 ## [13.0.1.1.4] - 29-06-2023
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/__manifest__.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/__manifest__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': 'Photovoltaic API',
-    'version': '13.0.1.1.5',
+    'version': '13.0.1.1.6',
     'depends': [
         'base_rest',
         'auth_api_key',
         'auth_jwt',
         'base_rest_pydantic',
         'pydantic',
         'photovoltaic_mgmt',
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/data/data.xml` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/data/data.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/pydantic_models/__init__.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/pydantic_models/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/pydantic_models/contract.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/pydantic_models/contract.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/pydantic_models/power_station.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/pydantic_models/power_station.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,13 +28,30 @@
     tn_co2_avoided: float
     reservation: float
     contracts_count: int
     eq_family_consumption: float
     production: List[PowerStationProduction]
     allocations_by_year: List[AllocationByYear]
 
+class PowerStationPublic(OrmModel):
+    id: int
+    name: str
+    display_name: Optional[str]
+    image: Optional[str] 
+    province: str
+    city: str
+    link_google_maps: str
+    peak_power: str
+    rated_power: str
+    start_date: date
+    energy_generated: float
+    tn_co2_avoided: float
+    reservation: float
+    contracts_count: int
+    eq_family_consumption: float
+
 class PowerStationShort(BaseModel):
     id: int
     name: str
     display_name: Optional[str]
     province: str
     city: str
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/pydantic_models/user.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/pydantic_models/user.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/security/ir.model.access.csv` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/security/ir.model.access.csv`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/services/account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/services/account.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/services/allocations.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/services/allocations.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/services/bank_account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/services/bank_account.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/services/contracts.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/services/contracts.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/services/info.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/services/info.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/services/user.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/services/user.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/tests/common.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/tests/common.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo/addons/photovoltaic_api/tests/test_account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo/addons/photovoltaic_api/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.5/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt` & `odoo13-addon-photovoltaic_api-13.0.1.1.6/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

