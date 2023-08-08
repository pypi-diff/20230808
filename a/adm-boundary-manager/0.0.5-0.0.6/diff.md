# Comparing `tmp/adm-boundary-manager-0.0.5.tar.gz` & `tmp/adm-boundary-manager-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adm-boundary-manager-0.0.5.tar", last modified: Tue Aug  1 11:30:50 2023, max compression
+gzip compressed data, was "adm-boundary-manager-0.0.6.tar", last modified: Tue Aug  8 12:34:38 2023, max compression
```

## Comparing `adm-boundary-manager-0.0.5.tar` & `adm-boundary-manager-0.0.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:50.532252 adm-boundary-manager-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20604 2023-08-01 11:30:50.532252 adm-boundary-manager-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:50.528252 adm-boundary-manager-0.0.5/adm_boundary_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20604 2023-08-01 11:30:50.000000 adm-boundary-manager-0.0.5/adm_boundary_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-01 11:30:50.000000 adm-boundary-manager-0.0.5/adm_boundary_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:30:50.000000 adm-boundary-manager-0.0.5/adm_boundary_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-01 11:30:50.000000 adm-boundary-manager-0.0.5/adm_boundary_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:30:50.000000 adm-boundary-manager-0.0.5/adm_boundary_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:50.532252 adm-boundary-manager-0.0.5/adminboundarymanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:50.532252 adm-boundary-manager-0.0.5/adminboundarymanager/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/loaders/cod_abs_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/loaders/gadm_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/loaders/generic_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:50.532252 adm-boundary-manager-0.0.5/adminboundarymanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0004_rename_countries_country_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0005_alter_country_country.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0006_remove_adminboundary_size_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:50.528252 adm-boundary-manager-0.0.5/adminboundarymanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:50.532252 adm-boundary-manager-0.0.5/adminboundarymanager/templates/adminboundarymanager/
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/adminboundarymanager/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 11:30:31.000000 adm-boundary-manager-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 11:30:50.532252 adm-boundary-manager-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:38.044699 adm-boundary-manager-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20604 2023-08-08 12:34:38.044699 adm-boundary-manager-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:38.040699 adm-boundary-manager-0.0.6/adm_boundary_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20604 2023-08-08 12:34:38.000000 adm-boundary-manager-0.0.6/adm_boundary_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-08 12:34:38.000000 adm-boundary-manager-0.0.6/adm_boundary_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:34:38.000000 adm-boundary-manager-0.0.6/adm_boundary_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-08 12:34:38.000000 adm-boundary-manager-0.0.6/adm_boundary_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 12:34:38.000000 adm-boundary-manager-0.0.6/adm_boundary_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:38.040699 adm-boundary-manager-0.0.6/adminboundarymanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:38.044699 adm-boundary-manager-0.0.6/adminboundarymanager/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/loaders/cod_abs_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/loaders/gadm_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/loaders/generic_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:38.044699 adm-boundary-manager-0.0.6/adminboundarymanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/migrations/0004_rename_countries_country_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/migrations/0005_alter_country_country.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/migrations/0006_remove_adminboundary_size_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:38.036699 adm-boundary-manager-0.0.6/adminboundarymanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:34:38.044699 adm-boundary-manager-0.0.6/adminboundarymanager/templates/adminboundarymanager/
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/adminboundarymanager/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-08 12:34:19.000000 adm-boundary-manager-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-08 12:34:38.044699 adm-boundary-manager-0.0.6/setup.cfg
```

### Comparing `adm-boundary-manager-0.0.5/PKG-INFO` & `adm-boundary-manager-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adm-boundary-manager
-Version: 0.0.5
+Version: 0.0.6
 Summary: Load, manage and visualize Administrative Boundaries Data in Wagtail
 Home-page: https://github.com/wmo-raf/adm-boundary-manager
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `adm-boundary-manager-0.0.5/README.md` & `adm-boundary-manager-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adm_boundary_manager.egg-info/PKG-INFO` & `adm-boundary-manager-0.0.6/adm_boundary_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adm-boundary-manager
-Version: 0.0.5
+Version: 0.0.6
 Summary: Load, manage and visualize Administrative Boundaries Data in Wagtail
 Home-page: https://github.com/wmo-raf/adm-boundary-manager
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `adm-boundary-manager-0.0.5/adm_boundary_manager.egg-info/SOURCES.txt` & `adm-boundary-manager-0.0.6/adm_boundary_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/countries.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/countries.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/errors.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/errors.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/forms.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/forms.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/loaders/__init__.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/loaders/cod_abs_loader.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/loaders/cod_abs_loader.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/loaders/gadm_loader.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/loaders/gadm_loader.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/loaders/generic_loader.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/loaders/generic_loader.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0001_initial.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0004_rename_countries_country_and_more.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/migrations/0004_rename_countries_country_and_more.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/migrations/0006_remove_adminboundary_size_and_more.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/migrations/0006_remove_adminboundary_size_and_more.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/models.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,16 +164,18 @@
             })
 
         return countries
 
     @cached_property
     def combined_countries_bounds(self):
         bounds_polygons = self.get_country_bounds_polygons()
-        combined_polygon = unary_union(bounds_polygons)
-        return list(combined_polygon.bounds)
+        if bounds_polygons:
+            combined_polygon = unary_union(bounds_polygons)
+            return list(combined_polygon.bounds)
+        return None
 
     def get_country_bounds_polygons(self):
         bounds_polygons = []
         for country in self.countries_list:
             if country.get("bbox"):
                 bbox = country.get("bbox")
                 polygon = geometry.box(*bbox, ccw=True)
```

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/serializers.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/serializers.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html` & `adm-boundary-manager-0.0.6/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html` & `adm-boundary-manager-0.0.6/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/urls.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/urls.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/utils.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/utils.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/views.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/views.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/adminboundarymanager/wagtail_hooks.py` & `adm-boundary-manager-0.0.6/adminboundarymanager/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.5/setup.cfg` & `adm-boundary-manager-0.0.6/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = adm-boundary-manager
-version = 0.0.5
+version = 0.0.6
 description = Load, manage and visualize Administrative Boundaries Data in Wagtail
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/adm-boundary-manager
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
```

