# Comparing `tmp/olca_schema-0.0.8.tar.gz` & `tmp/olca_schema-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olca_schema-0.0.8.tar", last modified: Mon Nov  7 16:37:17 2022, max compression
+gzip compressed data, was "olca_schema-0.0.9.tar", last modified: Fri Nov 25 11:06:06 2022, max compression
```

## Comparing `olca_schema-0.0.8.tar` & `olca_schema-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-11-07 16:37:17.359595 olca_schema-0.0.8/
--rw-rw-rw-   0        0        0       37 2022-09-19 11:29:38.000000 olca_schema-0.0.8/.gitignore
--rw-rw-rw-   0        0        0     2058 2022-11-07 16:37:17.358598 olca_schema-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1320 2022-09-22 10:18:10.000000 olca_schema-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-11-07 16:37:17.334661 olca_schema-0.0.8/olca_schema/
--rw-rw-rw-   0        0        0    10975 2022-11-07 15:56:55.000000 olca_schema-0.0.8/olca_schema/__init__.py
--rw-rw-rw-   0        0        0     8118 2022-11-07 16:24:31.000000 olca_schema-0.0.8/olca_schema/results.py
--rw-rw-rw-   0        0        0   115260 2022-11-07 16:24:31.000000 olca_schema-0.0.8/olca_schema/schema.py
-drwxrwxrwx   0        0        0        0 2022-11-07 16:37:17.348887 olca_schema-0.0.8/olca_schema/units/
--rw-rw-rw-   0        0        0     1886 2022-09-22 09:08:02.000000 olca_schema-0.0.8/olca_schema/units/__init__.py
--rw-rw-rw-   0        0        0    40186 2020-08-14 08:19:50.000000 olca_schema-0.0.8/olca_schema/units/units.csv
--rw-rw-rw-   0        0        0     4883 2022-09-19 11:29:38.000000 olca_schema-0.0.8/olca_schema/zipio.py
-drwxrwxrwx   0        0        0        0 2022-11-07 16:37:17.346628 olca_schema-0.0.8/olca_schema.egg-info/
--rw-rw-rw-   0        0        0     2058 2022-11-07 16:37:17.000000 olca_schema-0.0.8/olca_schema.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2022-11-07 16:37:17.000000 olca_schema-0.0.8/olca_schema.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-07 16:37:17.000000 olca_schema-0.0.8/olca_schema.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-11-07 16:37:17.000000 olca_schema-0.0.8/olca_schema.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      925 2022-11-07 16:30:13.000000 olca_schema-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-07 16:37:17.359595 olca_schema-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-11-07 16:37:17.357600 olca_schema-0.0.8/tests/
--rw-rw-rw-   0        0        0      707 2022-10-21 08:56:42.000000 olca_schema-0.0.8/tests/example.py
--rw-rw-rw-   0        0        0      684 2022-11-07 16:33:16.000000 olca_schema-0.0.8/tests/test_bools.py
--rw-rw-rw-   0        0        0     1288 2022-09-22 10:39:06.000000 olca_schema-0.0.8/tests/test_enum_conv.py
--rw-rw-rw-   0        0        0     2837 2022-09-22 10:30:09.000000 olca_schema-0.0.8/tests/test_factory.py
--rw-rw-rw-   0        0        0     1518 2022-09-22 10:40:52.000000 olca_schema-0.0.8/tests/test_json.py
--rw-rw-rw-   0        0        0      621 2022-09-22 09:08:16.000000 olca_schema-0.0.8/tests/test_ref_conv.py
--rw-rw-rw-   0        0        0     1093 2022-10-21 09:08:28.000000 olca_schema-0.0.8/tests/test_result_types.py
--rw-rw-rw-   0        0        0     1245 2022-09-19 11:29:38.000000 olca_schema-0.0.8/tests/test_root_fns.py
--rw-rw-rw-   0        0        0      803 2022-09-22 10:43:17.000000 olca_schema-0.0.8/tests/test_units.py
--rw-rw-rw-   0        0        0     2191 2022-09-22 09:08:16.000000 olca_schema-0.0.8/tests/test_zipio.py
+drwxrwxrwx   0        0        0        0 2022-11-25 11:06:06.755633 olca_schema-0.0.9/
+-rw-rw-rw-   0        0        0       37 2022-09-19 11:29:38.000000 olca_schema-0.0.9/.gitignore
+-rw-rw-rw-   0        0        0     2058 2022-11-25 11:06:06.755633 olca_schema-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1320 2022-09-22 10:18:10.000000 olca_schema-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-11-25 11:06:06.726711 olca_schema-0.0.9/olca_schema/
+-rw-rw-rw-   0        0        0    10975 2022-11-07 15:56:55.000000 olca_schema-0.0.9/olca_schema/__init__.py
+-rw-rw-rw-   0        0        0     8118 2022-11-07 16:24:31.000000 olca_schema-0.0.9/olca_schema/results.py
+-rw-rw-rw-   0        0        0   115260 2022-11-07 16:24:31.000000 olca_schema-0.0.9/olca_schema/schema.py
+drwxrwxrwx   0        0        0        0 2022-11-25 11:06:06.743666 olca_schema-0.0.9/olca_schema/units/
+-rw-rw-rw-   0        0        0     1886 2022-09-22 09:08:02.000000 olca_schema-0.0.9/olca_schema/units/__init__.py
+-rw-rw-rw-   0        0        0    40186 2020-08-14 08:19:50.000000 olca_schema-0.0.9/olca_schema/units/units.csv
+-rw-rw-rw-   0        0        0     5700 2022-11-25 11:04:37.000000 olca_schema-0.0.9/olca_schema/zipio.py
+drwxrwxrwx   0        0        0        0 2022-11-25 11:06:06.741701 olca_schema-0.0.9/olca_schema.egg-info/
+-rw-rw-rw-   0        0        0     2058 2022-11-25 11:06:06.000000 olca_schema-0.0.9/olca_schema.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2022-11-25 11:06:06.000000 olca_schema-0.0.9/olca_schema.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-25 11:06:06.000000 olca_schema-0.0.9/olca_schema.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2022-11-25 11:06:06.000000 olca_schema-0.0.9/olca_schema.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      925 2022-11-25 11:05:16.000000 olca_schema-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-11-25 11:06:06.755633 olca_schema-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-11-25 11:06:06.754636 olca_schema-0.0.9/tests/
+-rw-rw-rw-   0        0        0      707 2022-10-21 08:56:42.000000 olca_schema-0.0.9/tests/example.py
+-rw-rw-rw-   0        0        0      684 2022-11-07 16:33:16.000000 olca_schema-0.0.9/tests/test_bools.py
+-rw-rw-rw-   0        0        0     1288 2022-09-22 10:39:06.000000 olca_schema-0.0.9/tests/test_enum_conv.py
+-rw-rw-rw-   0        0        0     2837 2022-11-25 09:37:42.000000 olca_schema-0.0.9/tests/test_factory.py
+-rw-rw-rw-   0        0        0     1518 2022-09-22 10:40:52.000000 olca_schema-0.0.9/tests/test_json.py
+-rw-rw-rw-   0        0        0      621 2022-09-22 09:08:16.000000 olca_schema-0.0.9/tests/test_ref_conv.py
+-rw-rw-rw-   0        0        0     1093 2022-10-21 09:08:28.000000 olca_schema-0.0.9/tests/test_result_types.py
+-rw-rw-rw-   0        0        0     1245 2022-09-19 11:29:38.000000 olca_schema-0.0.9/tests/test_root_fns.py
+-rw-rw-rw-   0        0        0      803 2022-09-22 10:43:17.000000 olca_schema-0.0.9/tests/test_units.py
+-rw-rw-rw-   0        0        0     2771 2022-11-25 11:00:39.000000 olca_schema-0.0.9/tests/test_zipio.py
```

### Comparing `olca_schema-0.0.8/PKG-INFO` & `olca_schema-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olca_schema
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for reading and writing data sets in the openLCA schema format.
 Project-URL: Homepage, https://github.com/GreenDelta/olca-schema
 Project-URL: Bug Tracker, https://github.com/GreenDelta/olca-schema/issues
 Keywords: openLCA,life cycle assessment,LCA
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
```

### Comparing `olca_schema-0.0.8/README.md` & `olca_schema-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `olca_schema-0.0.8/olca_schema/__init__.py` & `olca_schema-0.0.9/olca_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `olca_schema-0.0.8/olca_schema/results.py` & `olca_schema-0.0.9/olca_schema/results.py`

 * *Files identical despite different names*

### Comparing `olca_schema-0.0.8/olca_schema/schema.py` & `olca_schema-0.0.9/olca_schema/schema.py`

 * *Files identical despite different names*

### Comparing `olca_schema-0.0.8/olca_schema/units/__init__.py` & `olca_schema-0.0.9/olca_schema/units/__init__.py`

 * *Files identical despite different names*

### Comparing `olca_schema-0.0.8/olca_schema/units/units.csv` & `olca_schema-0.0.9/olca_schema/units/units.csv`

 * *Files identical despite different names*

### Comparing `olca_schema-0.0.8/olca_schema/zipio.py` & `olca_schema-0.0.9/olca_schema/zipio.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,59 @@
+import os
 import zipfile
 
+from typing import Iterator, List, Optional, Type, TypeVar, Union
+
 import olca_schema as schema
 
-from typing import Optional, Type
 
+_E = TypeVar("_E", bound=schema.RootEntity)
 
-class ZipWriter:
 
-    def __init__(self, file_name: str):
+class ZipWriter:
+    def __init__(self, path: Union[str, os.PathLike]):
         self.__zip = zipfile.ZipFile(
-            file_name, mode='a', compression=zipfile.ZIP_DEFLATED)
-        if 'olca-schema.json' not in self.__zip.namelist():
-            self.__zip.writestr('olca-schema.json', '{"version": 2}')
+            path, mode="a", compression=zipfile.ZIP_DEFLATED
+        )
+        if "olca-schema.json" not in self.__zip.namelist():
+            self.__zip.writestr("olca-schema.json", '{"version": 2}')
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
         self.close()
 
     def close(self):
         self.__zip.close()
 
     def write(self, entity: schema.RootEntity):
-        if entity.id is None or entity.id == '':
-            raise ValueError('entity must have an ID')
+        if entity.id is None or entity.id == "":
+            raise ValueError("entity must have an ID")
         folder = _folder_of_entity(entity)
-        path = f'{folder}/{entity.id}.json'
+        path = f"{folder}/{entity.id}.json"
         self.__zip.writestr(path, entity.to_json())
 
 
 class ZipReader:
-
-    def __init__(self, file_name: str):
-        self.__zip = zipfile.ZipFile(file_name, mode='r')
+    def __init__(self, path: Union[str, os.PathLike]):
+        self.__zip = zipfile.ZipFile(path, mode="r")
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
         self.close()
 
     def close(self):
         self.__zip.close()
 
-    def read(self, class_type: Type[schema.RootEntity],
-             uid: str) -> Optional[schema.RootEntity]:
+    def read(self, class_type: Type[_E], uid: str) -> Optional[_E]:
         folder = _folder_of_class(class_type)
-        path = f'{folder}/{uid}.json'
+        path = f"{folder}/{uid}.json"
         if path not in self.__zip.namelist():
             return None
         data = self.__zip.read(path)
         return class_type.from_json(data)
 
     def read_actor(self, uid: str) -> Optional[schema.Actor]:
         return self.read(schema.Actor, uid)
@@ -91,60 +93,84 @@
 
     def read_project(self, uid: str) -> Optional[schema.Project]:
         return self.read(schema.Project, uid)
 
     def read_result(self, uid: str) -> Optional[schema.Result]:
         return self.read(schema.Result, uid)
 
-    def read_social_indicator(self, uid: str) -> Optional[
-        schema.SocialIndicator]:
+    def read_social_indicator(
+        self, uid: str
+    ) -> Optional[schema.SocialIndicator]:
         return self.read(schema.SocialIndicator, uid)
 
     def read_source(self, uid: str) -> Optional[schema.Source]:
         return self.read(schema.Source, uid)
 
     def read_unit_group(self, uid: str) -> Optional[schema.UnitGroup]:
         return self.read(schema.UnitGroup, uid)
 
+    def read_each(self, type_: Type[_E]) -> Iterator[_E]:
+        for uid in self.ids_of(type_):
+            e = self.read(type_, uid)
+            if e is not None:
+                yield e
+
+    def ids_of(self, type_: Type[_E]) -> List[str]:
+        folder = _folder_of_class(type_)
+        ids = []
+        for info in self.__zip.filelist:
+            if info.is_dir():
+                continue
+            name = info.filename
+            if not name.endswith(".json"):
+                continue
+            parts = name.split("/")
+            if len(parts) < 2:
+                continue
+            if parts[-2] != folder:
+                continue
+            ids.append(parts[-1][0:-5])
+        return ids
+
 
 def _folder_of_entity(entity: schema.RootEntity) -> str:
     if entity is None:
         raise ValueError("unknown root entity type")
     return _folder_of_class(type(entity))
 
 
-def _folder_of_class(t: type) -> str:
+def _folder_of_class(t: Type[_E]) -> str:
     if t == schema.Actor:
-        return 'actors'
+        return "actors"
     if t == schema.Currency:
-        return 'currencies'
+        return "currencies"
     if t == schema.DQSystem:
-        return 'dq_systems'
+        return "dq_systems"
     if t == schema.Epd:
-        return 'epds'
+        return "epds"
     if t == schema.Flow:
-        return 'flows'
+        return "flows"
     if t == schema.FlowProperty:
-        return 'flow_properties'
+        return "flow_properties"
     if t == schema.ImpactCategory:
-        return 'lcia_categories'
+        return "lcia_categories"
     if t == schema.ImpactMethod:
-        return 'lcia_methods'
+        return "lcia_methods"
     if t == schema.Location:
-        return 'locations'
+        return "locations"
     if t == schema.Parameter:
-        return 'parameters'
+        return "parameters"
     if t == schema.Process:
-        return 'processes'
+        return "processes"
     if t == schema.ProductSystem:
-        return 'product_systems'
+        return "product_systems"
     if t == schema.Project:
-        return 'projects'
+        return "projects"
     if t == schema.Result:
-        return 'results'
+        return "results"
     if t == schema.SocialIndicator:
-        return 'social_indicators'
+        return "social_indicators"
     if t == schema.Source:
-        return 'sources'
+        return "sources"
     if t == schema.UnitGroup:
-        return 'unit_groups'
-    raise ValueError(f'not a known root entity type: {t}')
+        return "unit_groups"
+    raise ValueError(f"not a known root entity type: {t}")
```

### Comparing `olca_schema-0.0.8/olca_schema.egg-info/PKG-INFO` & `olca_schema-0.0.9/olca_schema.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olca-schema
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for reading and writing data sets in the openLCA schema format.
 Project-URL: Homepage, https://github.com/GreenDelta/olca-schema
 Project-URL: Bug Tracker, https://github.com/GreenDelta/olca-schema/issues
 Keywords: openLCA,life cycle assessment,LCA
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
```

### Comparing `olca_schema-0.0.8/olca_schema.egg-info/SOURCES.txt` & `olca_schema-0.0.9/olca_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `olca_schema-0.0.8/pyproject.toml` & `olca_schema-0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "olca_schema"
-version = "0.0.8"
+version = "0.0.9"
 description = "A package for reading and writing data sets in the openLCA schema format."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords=["openLCA", "life cycle assessment", "LCA"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3",
```

### Comparing `olca_schema-0.0.8/tests/example.py` & `olca_schema-0.0.9/tests/example.py`

 * *Files identical despite different names*

### Comparing `olca_schema-0.0.8/tests/test_bools.py` & `olca_schema-0.0.9/tests/test_bools.py`

 * *Files identical despite different names*

### Comparing `olca_schema-0.0.8/tests/test_enum_conv.py` & `olca_schema-0.0.9/tests/test_enum_conv.py`

 * *Files identical despite different names*

### Comparing `olca_schema-0.0.8/tests/test_factory.py` & `olca_schema-0.0.9/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `olca_schema-0.0.8/tests/test_json.py` & `olca_schema-0.0.9/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `olca_schema-0.0.8/tests/test_ref_conv.py` & `olca_schema-0.0.9/tests/test_ref_conv.py`

 * *Files identical despite different names*

### Comparing `olca_schema-0.0.8/tests/test_result_types.py` & `olca_schema-0.0.9/tests/test_result_types.py`

 * *Files identical despite different names*

### Comparing `olca_schema-0.0.8/tests/test_root_fns.py` & `olca_schema-0.0.9/tests/test_root_fns.py`

 * *Files identical despite different names*

### Comparing `olca_schema-0.0.8/tests/test_units.py` & `olca_schema-0.0.9/tests/test_units.py`

 * *Files identical despite different names*

