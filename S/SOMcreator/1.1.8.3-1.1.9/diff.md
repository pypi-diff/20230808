# Comparing `tmp/SOMcreator-1.1.8.3.tar.gz` & `tmp/SOMcreator-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SOMcreator-1.1.8.3.tar", last modified: Fri Aug  4 09:33:15 2023, max compression
+gzip compressed data, was "SOMcreator-1.1.9.tar", last modified: Tue Aug  8 06:50:45 2023, max compression
```

## Comparing `SOMcreator-1.1.8.3.tar` & `SOMcreator-1.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 09:33:15.664758 SOMcreator-1.1.8.3/
--rw-rw-rw-   0        0        0     1095 2022-10-28 12:14:14.000000 SOMcreator-1.1.8.3/LICENSE
--rw-rw-rw-   0        0        0       81 2022-11-01 07:22:32.000000 SOMcreator-1.1.8.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1556 2023-08-04 09:33:15.663717 SOMcreator-1.1.8.3/PKG-INFO
--rw-rw-rw-   0        0        0        9 2022-10-28 11:24:11.000000 SOMcreator-1.1.8.3/README.md
--rw-rw-rw-   0        0        0      876 2023-03-20 13:30:05.000000 SOMcreator-1.1.8.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-04 09:33:15.665258 SOMcreator-1.1.8.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-04 09:33:15.441687 SOMcreator-1.1.8.3/src/
-drwxrwxrwx   0        0        0        0 2023-08-04 09:33:15.476686 SOMcreator-1.1.8.3/src/SOMcreator/
-drwxrwxrwx   0        0        0        0 2023-08-04 09:33:15.555880 SOMcreator-1.1.8.3/src/SOMcreator/Template/
--rw-rw-rw-   0        0        0      375 2023-05-16 05:28:24.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 09:33:15.567367 SOMcreator-1.1.8.3/src/SOMcreator/Template/__pyinstaller/
--rw-rw-rw-   0        0        0       71 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0      202 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
--rw-rw-rw-   0        0        0      331 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/bookmark_template.txt
--rw-rw-rw-   0        0        0    25168 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/ifc.json
-drwxrwxrwx   0        0        0        0 2023-08-04 09:33:15.605855 SOMcreator-1.1.8.3/src/SOMcreator/Template/js_templates/
--rw-rw-rw-   0        0        0     1001 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/js_templates/end_ungetestet.js
--rw-rw-rw-   0        0        0     7071 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/js_templates/start_check_start.js
--rw-rw-rw-   0        0        0      598 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/js_templates/start_koordinaten.js
--rw-rw-rw-   0        0        0     2938 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/mapping_template.txt
--rw-rw-rw-   0        0        0     3121 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/template.txt
--rw-rw-rw-   0        0        0      156 2023-08-04 09:32:50.000000 SOMcreator-1.1.8.3/src/SOMcreator/__init__.py
--rw-rw-rw-   0        0        0    25149 2023-08-04 09:32:50.000000 SOMcreator-1.1.8.3/src/SOMcreator/classes.py
--rw-rw-rw-   0        0        0     1898 2023-05-04 10:57:17.000000 SOMcreator-1.1.8.3/src/SOMcreator/constants.py
-drwxrwxrwx   0        0        0        0 2023-08-04 09:33:15.662713 SOMcreator-1.1.8.3/src/SOMcreator/external_software/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/external_software/__init__.py
--rw-rw-rw-   0        0        0     4311 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/external_software/allplan.py
--rw-rw-rw-   0        0        0     1365 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/external_software/card1.py
--rw-rw-rw-   0        0        0    22074 2023-08-04 09:32:50.000000 SOMcreator-1.1.8.3/src/SOMcreator/external_software/desite.py
--rw-rw-rw-   0        0        0    21951 2023-06-28 13:16:14.000000 SOMcreator-1.1.8.3/src/SOMcreator/external_software/excel.py
--rw-rw-rw-   0        0        0     3326 2023-05-04 10:57:17.000000 SOMcreator-1.1.8.3/src/SOMcreator/external_software/revit.py
--rw-rw-rw-   0        0        0     3227 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/external_software/vestra.py
--rw-rw-rw-   0        0        0     9397 2023-08-01 15:25:56.000000 SOMcreator-1.1.8.3/src/SOMcreator/filehandling.py
--rw-rw-rw-   0        0        0      970 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/quality_check.py
-drwxrwxrwx   0        0        0        0 2023-08-04 09:33:15.513005 SOMcreator-1.1.8.3/src/SOMcreator.egg-info/
--rw-rw-rw-   0        0        0     1556 2023-08-04 09:33:15.000000 SOMcreator-1.1.8.3/src/SOMcreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2023-08-04 09:33:15.000000 SOMcreator-1.1.8.3/src/SOMcreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 09:33:15.000000 SOMcreator-1.1.8.3/src/SOMcreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-08-04 09:33:15.000000 SOMcreator-1.1.8.3/src/SOMcreator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-08-04 09:33:15.000000 SOMcreator-1.1.8.3/src/SOMcreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-04 09:33:15.000000 SOMcreator-1.1.8.3/src/SOMcreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 06:50:45.837276 SOMcreator-1.1.9/
+-rw-rw-rw-   0        0        0     1095 2022-10-28 12:14:14.000000 SOMcreator-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0       81 2022-11-01 07:22:32.000000 SOMcreator-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1554 2023-08-08 06:50:45.837276 SOMcreator-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2022-10-28 11:24:11.000000 SOMcreator-1.1.9/README.md
+-rw-rw-rw-   0        0        0      876 2023-03-20 13:30:05.000000 SOMcreator-1.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 06:50:45.837276 SOMcreator-1.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 06:50:45.622191 SOMcreator-1.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 06:50:45.655194 SOMcreator-1.1.9/src/SOMcreator/
+drwxrwxrwx   0        0        0        0 2023-08-08 06:50:45.723620 SOMcreator-1.1.9/src/SOMcreator/Template/
+-rw-rw-rw-   0        0        0      375 2023-05-16 05:28:24.000000 SOMcreator-1.1.9/src/SOMcreator/Template/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:50:45.739839 SOMcreator-1.1.9/src/SOMcreator/Template/__pyinstaller/
+-rw-rw-rw-   0        0        0       71 2023-04-06 10:29:25.000000 SOMcreator-1.1.9/src/SOMcreator/Template/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0      202 2023-04-06 10:29:25.000000 SOMcreator-1.1.9/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
+-rw-rw-rw-   0        0        0      331 2023-04-06 10:29:25.000000 SOMcreator-1.1.9/src/SOMcreator/Template/bookmark_template.txt
+-rw-rw-rw-   0        0        0    25168 2023-04-06 10:29:25.000000 SOMcreator-1.1.9/src/SOMcreator/Template/ifc.json
+drwxrwxrwx   0        0        0        0 2023-08-08 06:50:45.780408 SOMcreator-1.1.9/src/SOMcreator/Template/js_templates/
+-rw-rw-rw-   0        0        0     1001 2023-04-06 10:29:25.000000 SOMcreator-1.1.9/src/SOMcreator/Template/js_templates/end_ungetestet.js
+-rw-rw-rw-   0        0        0     7071 2023-04-06 10:29:25.000000 SOMcreator-1.1.9/src/SOMcreator/Template/js_templates/start_check_start.js
+-rw-rw-rw-   0        0        0      598 2023-04-06 10:29:25.000000 SOMcreator-1.1.9/src/SOMcreator/Template/js_templates/start_koordinaten.js
+-rw-rw-rw-   0        0        0     2938 2023-04-06 10:29:25.000000 SOMcreator-1.1.9/src/SOMcreator/Template/mapping_template.txt
+-rw-rw-rw-   0        0        0     3121 2023-04-06 10:29:25.000000 SOMcreator-1.1.9/src/SOMcreator/Template/template.txt
+-rw-rw-rw-   0        0        0      154 2023-08-08 06:50:28.000000 SOMcreator-1.1.9/src/SOMcreator/__init__.py
+-rw-rw-rw-   0        0        0    25397 2023-08-08 06:40:48.000000 SOMcreator-1.1.9/src/SOMcreator/classes.py
+-rw-rw-rw-   0        0        0     1898 2023-05-04 10:57:17.000000 SOMcreator-1.1.9/src/SOMcreator/constants.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:50:45.836276 SOMcreator-1.1.9/src/SOMcreator/external_software/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:29:25.000000 SOMcreator-1.1.9/src/SOMcreator/external_software/__init__.py
+-rw-rw-rw-   0        0        0     4311 2023-04-06 10:29:25.000000 SOMcreator-1.1.9/src/SOMcreator/external_software/allplan.py
+-rw-rw-rw-   0        0        0     1365 2023-04-06 10:29:25.000000 SOMcreator-1.1.9/src/SOMcreator/external_software/card1.py
+-rw-rw-rw-   0        0        0    22074 2023-08-04 09:32:50.000000 SOMcreator-1.1.9/src/SOMcreator/external_software/desite.py
+-rw-rw-rw-   0        0        0    21951 2023-06-28 13:16:14.000000 SOMcreator-1.1.9/src/SOMcreator/external_software/excel.py
+-rw-rw-rw-   0        0        0     3326 2023-05-04 10:57:17.000000 SOMcreator-1.1.9/src/SOMcreator/external_software/revit.py
+-rw-rw-rw-   0        0        0     3227 2023-04-06 10:29:25.000000 SOMcreator-1.1.9/src/SOMcreator/external_software/vestra.py
+-rw-rw-rw-   0        0        0    10188 2023-08-08 06:48:56.000000 SOMcreator-1.1.9/src/SOMcreator/filehandling.py
+-rw-rw-rw-   0        0        0      970 2023-04-06 10:29:25.000000 SOMcreator-1.1.9/src/SOMcreator/quality_check.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:50:45.679427 SOMcreator-1.1.9/src/SOMcreator.egg-info/
+-rw-rw-rw-   0        0        0     1554 2023-08-08 06:50:45.000000 SOMcreator-1.1.9/src/SOMcreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2023-08-08 06:50:45.000000 SOMcreator-1.1.9/src/SOMcreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 06:50:45.000000 SOMcreator-1.1.9/src/SOMcreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-08-08 06:50:45.000000 SOMcreator-1.1.9/src/SOMcreator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-08-08 06:50:45.000000 SOMcreator-1.1.9/src/SOMcreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-08 06:50:45.000000 SOMcreator-1.1.9/src/SOMcreator.egg-info/top_level.txt
```

### Comparing `SOMcreator-1.1.8.3/LICENSE` & `SOMcreator-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.3/PKG-INFO` & `SOMcreator-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.1.8.3
+Version: 1.1.9
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.1.8.3/pyproject.toml` & `SOMcreator-1.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator/Template/ifc.json` & `SOMcreator-1.1.9/src/SOMcreator/Template/ifc.json`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator/Template/js_templates/end_ungetestet.js` & `SOMcreator-1.1.9/src/SOMcreator/Template/js_templates/end_ungetestet.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator/Template/js_templates/start_check_start.js` & `SOMcreator-1.1.9/src/SOMcreator/Template/js_templates/start_check_start.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator/Template/js_templates/start_koordinaten.js` & `SOMcreator-1.1.9/src/SOMcreator/Template/js_templates/start_koordinaten.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator/Template/mapping_template.txt` & `SOMcreator-1.1.9/src/SOMcreator/Template/mapping_template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator/Template/template.txt` & `SOMcreator-1.1.9/src/SOMcreator/Template/template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator/classes.py` & `SOMcreator-1.1.9/src/SOMcreator/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,19 +211,19 @@
     def name(self, value: str):
         self._name = value
         for child in self.children:
             child.name = value
         self.changed = True
 
     @property
-    def parent(self) -> Hirarchy:
+    def parent(self) -> PropertySet | Object | Attribute | Aggregation:
         return self._parent
 
     @parent.setter
-    def parent(self, parent: Hirarchy) -> None:
+    def parent(self, parent: PropertySet | Object | Attribute | Aggregation) -> None:
         if self.parent is not None:
             self.parent._children.remove(self)
         self._parent = parent
         if parent is not None:
             self._parent._children.add(self)
         self.changed = True
 
@@ -238,23 +238,23 @@
     def is_child(self) -> bool:
         if self.parent is not None:
             return True
         else:
             return False
 
     @property
-    def children(self) -> set[Hirarchy]:
+    def children(self) -> set[PropertySet | Object | Attribute | Aggregation]:
         return self._children
 
-    def add_child(self, child: Hirarchy) -> None:
+    def add_child(self, child: PropertySet | Object | Attribute | Aggregation) -> None:
         self.children.add(child)
         child.parent = self
         self.changed = True
 
-    def remove_child(self, child: Hirarchy) -> None:
+    def remove_child(self, child: PropertySet | Object | Attribute | Aggregation) -> None:
         self.children.remove(child)
         child.delete()
 
     def delete(self) -> None:
         if self in self._registry:
             self._registry.remove(self)
 
@@ -754,14 +754,16 @@
         if not self.is_root:
             self.parent.children.remove(self)
         for child in self.children:
             child.parent = None
 
     @property
     def parent_connection(self):
+        if self.parent is None:
+            return None
         return self._parent_connection
 
     @parent_connection.setter
     def parent_connection(self, value):
         self._parent_connection = value
 
     @property
```

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator/constants.py` & `SOMcreator-1.1.9/src/SOMcreator/constants.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator/external_software/allplan.py` & `SOMcreator-1.1.9/src/SOMcreator/external_software/allplan.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator/external_software/card1.py` & `SOMcreator-1.1.9/src/SOMcreator/external_software/card1.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator/external_software/desite.py` & `SOMcreator-1.1.9/src/SOMcreator/external_software/desite.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator/external_software/excel.py` & `SOMcreator-1.1.9/src/SOMcreator/external_software/excel.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator/external_software/revit.py` & `SOMcreator-1.1.9/src/SOMcreator/external_software/revit.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator/external_software/vestra.py` & `SOMcreator-1.1.9/src/SOMcreator/external_software/vestra.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator/filehandling.py` & `SOMcreator-1.1.9/src/SOMcreator/filehandling.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,19 @@
     code = template.render(attribute_dict=attrib_dict, pset_name=pset_name)
     with open(path, "w") as file:
         file.write(code)
     pass
 
 
 def export_json(project: classes.Project, path: str) -> dict:
+    def create_project(project_dict:dict) -> None:
+        project_dict[constants.NAME] = project.name
+        project_dict[constants.AUTHOR] = project.author
+        project_dict[constants.VERSION] = project.version
+
     def filL_basics(entity_dict, entity):
         entity_dict[constants.NAME] = entity.name
         entity_dict[constants.OPTIONAL] = entity.optional
         if entity.parent is not None:
             parent = entity.parent.uuid
         else:
             parent = None
@@ -106,14 +111,17 @@
             aggregation_dict[constants.PARENT] = aggregation.parent.uuid
         else:
             aggregation_dict[constants.PARENT] = aggregation.parent
         aggregation_dict[constants.CONNECTION] = aggregation.parent_connection
         aggregations_dict[aggregation.uuid] = aggregation_dict
 
     main_dict = dict()
+    main_dict[constants.PROJECT] = dict()
+    create_project(main_dict[constants.PROJECT])
+
     predef_pset_dict = dict()
     predefined_psets = project.get_predefined_psets()
     for entity in sorted(predefined_psets, key=lambda x: x.uuid):
         create_pset_entry(predef_pset_dict, entity)
     main_dict[constants.PREDEFINED_PSETS] = predef_pset_dict
 
     objects_dict = dict()
@@ -136,14 +144,18 @@
     if not os.path.isfile(path):
         return
     parent_dict = {}
     aggregation_parent_dict: dict[classes.Aggregation, (str, int)] = dict()
 
     with open(path, "r") as file:
         main_dict: dict = json.load(file)
+    def load_project_data(project_dict:dict):
+        project.name = project_dict.get(constants.NAME)
+        project.author = project_dict.get(constants.AUTHOR)
+        project.version = project_dict.get(constants.VERSION)
 
     def load_basics(element_dict: dict) -> (str, str, str):
         name = element_dict[constants.NAME]
         description = element_dict[constants.DESCRIPTION]
         optional = element_dict[constants.OPTIONAL]
         parent = element_dict[constants.PARENT]
         return name, description, optional, parent
@@ -207,14 +219,20 @@
 
     def build_aggregation_structure():
         for aggregation, (uuid, connection_type) in aggregation_parent_dict.items():
             parent = project.get_element_by_uuid(uuid)
             if parent is not None:
                 parent.add_child(aggregation,connection_type)
 
+    project_dict = main_dict.get(constants.PROJECT)
+    if project_dict is None:
+        logging.warning(f"{constants.PROJECT}-dict doesn't exist unable to load Author, Name and Version")
+    else:
+        load_project_data(project_dict)
+
     predefined_psets_dict = load_dict(constants.PREDEFINED_PSETS)
 
     for ident, pset_dict in predefined_psets_dict.items():
         load_pset(pset_dict, ident, None)
 
     objects_dict = load_dict(constants.OBJECTS)
     for ident, object_dict in objects_dict.items():
```

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator/quality_check.py` & `SOMcreator-1.1.9/src/SOMcreator/quality_check.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator.egg-info/PKG-INFO` & `SOMcreator-1.1.9/src/SOMcreator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.1.8.3
+Version: 1.1.9
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.1.8.3/src/SOMcreator.egg-info/SOURCES.txt` & `SOMcreator-1.1.9/src/SOMcreator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

