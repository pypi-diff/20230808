# Comparing `tmp/ssb_klass_python-0.0.4.tar.gz` & `tmp/ssb_klass_python-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_klass_python-0.0.4.tar", max compression
+gzip compressed data, was "ssb_klass_python-0.0.5.tar", max compression
```

## Comparing `ssb_klass_python-0.0.4.tar` & `ssb_klass_python-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1076 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/LICENSE.md
--rw-r--r--   0        0        0     1722 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/README.md
--rw-r--r--   0        0        0     1488 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/klass/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/classes/__init__.py
--rw-r--r--   0        0        0     3913 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/klass/classes/classification.py
--rw-r--r--   0        0        0     4459 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/klass/classes/codes.py
--rw-r--r--   0        0        0     3423 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/klass/classes/correspondance.py
--rw-r--r--   0        0        0      704 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/classes/family.py
--rw-r--r--   0        0        0     3810 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/classes/search.py
--rw-r--r--   0        0        0     2631 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/klass/classes/variant.py
--rw-r--r--   0        0        0     1831 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/classes/version.py
--rw-r--r--   0        0        0      520 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/klass/klass_config.py
--rw-r--r--   0        0        0        0 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/requests/__init__.py
--rw-r--r--   0        0        0    10886 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/klass/requests/klass_requests.py
--rw-r--r--   0        0        0      530 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/requests/sections.py
--rw-r--r--   0        0        0     3199 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/klass/requests/validate.py
--rw-r--r--   0        0        0      180 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/utility/classification.py
--rw-r--r--   0        0        0      244 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/utility/codes.py
--rw-r--r--   0        0        0        0 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/widgets/__init__.py
--rw-r--r--   0        0        0     3078 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/widgets/search_ipywidget.py
--rw-r--r--   0        0        0     1156 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 ssb_klass_python-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/LICENSE.md
+-rw-r--r--   0        0        0     2728 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/README.md
+-rw-r--r--   0        0        0     1494 2023-08-08 12:16:56.248541 ssb_klass_python-0.0.5/klass/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/classes/__init__.py
+-rw-r--r--   0        0        0    15026 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/classes/classification.py
+-rw-r--r--   0        0        0     9449 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/classes/codes.py
+-rw-r--r--   0        0        0     8141 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/classes/correspondance.py
+-rw-r--r--   0        0        0     2276 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/classes/family.py
+-rw-r--r--   0        0        0     9111 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/classes/search.py
+-rw-r--r--   0        0        0     9983 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/classes/variant.py
+-rw-r--r--   0        0        0     8660 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/classes/version.py
+-rw-r--r--   0        0        0      520 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/klass_config.py
+-rw-r--r--   0        0        0        0 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/requests/__init__.py
+-rw-r--r--   0        0        0    10886 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/requests/klass_requests.py
+-rw-r--r--   0        0        0      530 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/requests/sections.py
+-rw-r--r--   0        0        0     3199 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/requests/validate.py
+-rw-r--r--   0        0        0      180 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/utility/classification.py
+-rw-r--r--   0        0        0      244 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/utility/codes.py
+-rw-r--r--   0        0        0        0 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/widgets/__init__.py
+-rw-r--r--   0        0        0     3078 2023-08-08 12:16:35.040450 ssb_klass_python-0.0.5/klass/widgets/search_ipywidget.py
+-rw-r--r--   0        0        0     1157 2023-08-08 12:16:56.248541 ssb_klass_python-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 ssb_klass_python-0.0.5/PKG-INFO
```

### Comparing `ssb_klass_python-0.0.4/LICENSE.md` & `ssb_klass_python-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.4/README.md` & `ssb_klass_python-0.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 # ssb-klass-python
 
 A Python package built on top of Statistics Norway's code- and classification-system "KLASS". \
 The package aims to make Klass's API for retrieving data easier to use by re-representing Klass's internal hierarchy as python-classes. Containing methods for easier traversal down, search classes and widgets, reasonable defaults to parameters etc.
 Where data is possible to fit into pandas DataFrames, this will be preferred, but hirerachical data will be kept as json / dict structure.
 
 
+## Installing
+The package is available on Pypi, and can be installed by for example poetry like this:
+```bash
+poetry add ssb-klass-python
+```
+
+
 ## Example usages
 
 
 ### Getting started
 ```python
 from klass import search_classification
 # Opens a ipywidget in notebooks for searching for classifications and copying code, to get started
 search_classification(no_dupes=True)
 ```
+![The GUI available through the search_classification function](GUI.png)
+
+
 
 ### Getting a classification directly
 ```python
 from klass import get_classification # Import the utility-function
 nus = get_classification(36)
 ```
 
@@ -31,14 +41,39 @@
 ```python
 codes = nus.get_codes() # codes from current date
 print(codes)
 codes.data  # Pandas dataframe available under the .data attribute
 ```
 
 
+From searching through "families", down to a specific codelist
+```python
+from klass import KlassSearchFamilies
+search = KlassSearchFamilies(360)
+print(search)
+>>> "Family ID: 20 - Utdanning - Number of classifications: 5"
+utdanning = search.get_family(20)
+print(utdanning)
+>>> "The Klass Family "Utdanning" has id 20."
+>>> "And contains the following classifications:"
+>>>  "36: Standard for utdanningsgruppering (NUS)"
+nus = utdanning.get_classification(36)
+print(nus)
+>>> "Classification 36: Standard for utdanningsgruppering (NUS)..."
+nus_codes = nus.get_codes("2023-01-01")
+print(nus_codes)
+>>> "Codelist for classification: 36"
+>>> " From date: 2023-01-01"
+nus_codes.data  # A pandas dataframe
+```
+
+
+For more examples check out the demo-notebooks in the demo/ folder in the repo.
+
+
 
 ## Technical notes
 Documentation for the [endpoints we are using can be found on Statistics Norways pages.](https://data.ssb.no/api/klass/v1/api-guide.html)
 
 Technical architecture of the API we are interacting with is detailed in [Statistics Norway's **internal** wiki](https://wiki.ssb.no/display/KP/Teknisk+arkitektur#Tekniskarkitektur-GSIM).
```

### Comparing `ssb_klass_python-0.0.4/klass/__init__.py` & `ssb_klass_python-0.0.5/klass/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib import import_module
 
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 __all__ = []
 
 # Everything we want to be directly importable from under "klass"-package
 local_imports = {
     "requests.klass_requests": [
         "classifications",
         "classification_search",
@@ -25,15 +25,15 @@
     ],
     "classes.codes": ["KlassCodes"],
     "classes.correspondance": ["KlassCorrespondance"],
     "classes.classification": ["KlassClassification"],
     "classes.family": ["KlassFamily"],
     "classes.search": ["KlassSearchClassifications", "KlassSearchFamilies"],
     "requests.sections": ["sections_list", "sections_dict"],
-    "classes.variant": ["KlassVariant", "KlassVariantSearch"],
+    "classes.variant": ["KlassVariant", "KlassVariantSearchByName"],
     "classes.version": ["KlassVersion"],
     "utility.codes": ["get_codes"],
     "utility.classification": ["get_classification"],
     "widgets.search_ipywidget": ["search_classification"],
     "klass_config": ["KlassConfig"],
 }
```

### Comparing `ssb_klass_python-0.0.4/klass/klass_config.py` & `ssb_klass_python-0.0.5/klass/klass_config.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.4/klass/requests/klass_requests.py` & `ssb_klass_python-0.0.5/klass/requests/klass_requests.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.4/klass/requests/sections.py` & `ssb_klass_python-0.0.5/klass/requests/sections.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.4/klass/requests/validate.py` & `ssb_klass_python-0.0.5/klass/requests/validate.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.4/klass/widgets/search_ipywidget.py` & `ssb_klass_python-0.0.5/klass/widgets/search_ipywidget.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.4/pyproject.toml` & `ssb_klass_python-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "ssb-klass-python"
-version = "0.0.4"
+version = "0.0.5"
 description = "A Python package built on top of KLASS's API for retrieving classifications, codes, correspondances etc."
 authors = ["Carl Corneil <cfc@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "klass"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 dapla-toolbelt = "^1.3.2"
 python-dateutil = "^2.8.2"
 toml = "^0.10.2"
 ipywidgets = "^8.0.6"
-pandas = "1.5.3"
+pandas = "^1.5.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 ipykernel = "^6.15.3"
 pre-commit = "^2.20.0"
 autoflake = "^1.7.6"
 pep8-naming = "^0.13.2"
```

### Comparing `ssb_klass_python-0.0.4/PKG-INFO` & `ssb_klass_python-0.0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 Metadata-Version: 2.1
 Name: ssb-klass-python
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package built on top of KLASS's API for retrieving classifications, codes, correspondances etc.
 License: MIT
 Author: Carl Corneil
 Author-email: cfc@ssb.no
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: dapla-toolbelt (>=1.3.2,<2.0.0)
 Requires-Dist: ipywidgets (>=8.0.6,<9.0.0)
-Requires-Dist: pandas (==1.5.3)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # ssb-klass-python
 
 A Python package built on top of Statistics Norway's code- and classification-system "KLASS". \
 The package aims to make Klass's API for retrieving data easier to use by re-representing Klass's internal hierarchy as python-classes. Containing methods for easier traversal down, search classes and widgets, reasonable defaults to parameters etc.
 Where data is possible to fit into pandas DataFrames, this will be preferred, but hirerachical data will be kept as json / dict structure.
 
 
+## Installing
+The package is available on Pypi, and can be installed by for example poetry like this:
+```bash
+poetry add ssb-klass-python
+```
+
+
 ## Example usages
 
 
 ### Getting started
 ```python
 from klass import search_classification
 # Opens a ipywidget in notebooks for searching for classifications and copying code, to get started
 search_classification(no_dupes=True)
 ```
+![The GUI available through the search_classification function](GUI.png)
+
+
 
 ### Getting a classification directly
 ```python
 from klass import get_classification # Import the utility-function
 nus = get_classification(36)
 ```
 
@@ -49,14 +59,39 @@
 ```python
 codes = nus.get_codes() # codes from current date
 print(codes)
 codes.data  # Pandas dataframe available under the .data attribute
 ```
 
 
+From searching through "families", down to a specific codelist
+```python
+from klass import KlassSearchFamilies
+search = KlassSearchFamilies(360)
+print(search)
+>>> "Family ID: 20 - Utdanning - Number of classifications: 5"
+utdanning = search.get_family(20)
+print(utdanning)
+>>> "The Klass Family "Utdanning" has id 20."
+>>> "And contains the following classifications:"
+>>>  "36: Standard for utdanningsgruppering (NUS)"
+nus = utdanning.get_classification(36)
+print(nus)
+>>> "Classification 36: Standard for utdanningsgruppering (NUS)..."
+nus_codes = nus.get_codes("2023-01-01")
+print(nus_codes)
+>>> "Codelist for classification: 36"
+>>> " From date: 2023-01-01"
+nus_codes.data  # A pandas dataframe
+```
+
+
+For more examples check out the demo-notebooks in the demo/ folder in the repo.
+
+
 
 ## Technical notes
 Documentation for the [endpoints we are using can be found on Statistics Norways pages.](https://data.ssb.no/api/klass/v1/api-guide.html)
 
 Technical architecture of the API we are interacting with is detailed in [Statistics Norway's **internal** wiki](https://wiki.ssb.no/display/KP/Teknisk+arkitektur#Tekniskarkitektur-GSIM).
```

