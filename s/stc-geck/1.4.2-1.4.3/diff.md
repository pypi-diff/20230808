# Comparing `tmp/stc-geck-1.4.2.tar.gz` & `tmp/stc-geck-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-geck-1.4.2.tar", last modified: Tue Aug  8 07:59:46 2023, max compression
+gzip compressed data, was "stc-geck-1.4.3.tar", last modified: Tue Aug  8 11:57:02 2023, max compression
```

## Comparing `stc-geck-1.4.2.tar` & `stc-geck-1.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 07:59:46.771823 stc-geck-1.4.2/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.4.2/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-08 07:59:46.771568 stc-geck-1.4.2/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)     6985 2023-07-23 19:18:57.000000 stc-geck-1.4.2/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      600 2023-08-08 07:59:37.000000 stc-geck-1.4.2/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      171 2023-08-08 07:37:57.000000 stc-geck-1.4.2/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-08 07:59:46.771901 stc-geck-1.4.2/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 07:59:46.768734 stc-geck-1.4.2/stc_geck/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-19 19:56:31.000000 stc-geck-1.4.2/stc_geck/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     1464 2023-08-07 18:24:50.000000 stc-geck-1.4.2/stc_geck/advices.py
--rw-r--r--   0 pasha      (501) staff       (20)     7261 2023-08-07 19:06:08.000000 stc-geck-1.4.2/stc_geck/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     7405 2023-08-08 07:48:12.000000 stc-geck-1.4.2/stc_geck/client.py
--rw-r--r--   0 pasha      (501) staff       (20)    10455 2023-08-08 07:37:57.000000 stc-geck-1.4.2/stc_geck/query_processor.py
--rw-r--r--   0 pasha      (501) staff       (20)     3254 2023-08-07 18:22:54.000000 stc-geck-1.4.2/stc_geck/utils.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 07:59:46.771052 stc-geck-1.4.2/stc_geck.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-08 07:59:46.000000 stc-geck-1.4.2/stc_geck.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      369 2023-08-08 07:59:46.000000 stc-geck-1.4.2/stc_geck.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-08 07:59:46.000000 stc-geck-1.4.2/stc_geck.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-08 07:59:46.000000 stc-geck-1.4.2/stc_geck.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      172 2023-08-08 07:59:46.000000 stc-geck-1.4.2/stc_geck.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        9 2023-08-08 07:59:46.000000 stc-geck-1.4.2/stc_geck.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 11:57:02.781215 stc-geck-1.4.3/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.4.3/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-08 11:57:02.779883 stc-geck-1.4.3/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)     6985 2023-07-23 19:18:57.000000 stc-geck-1.4.3/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      600 2023-08-08 11:56:07.000000 stc-geck-1.4.3/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      171 2023-08-08 07:37:57.000000 stc-geck-1.4.3/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-08 11:57:02.781839 stc-geck-1.4.3/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 11:57:02.766764 stc-geck-1.4.3/stc_geck/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-19 19:56:31.000000 stc-geck-1.4.3/stc_geck/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1464 2023-08-07 18:24:50.000000 stc-geck-1.4.3/stc_geck/advices.py
+-rw-r--r--   0 pasha      (501) staff       (20)     7261 2023-08-07 19:06:08.000000 stc-geck-1.4.3/stc_geck/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     7405 2023-08-08 07:48:12.000000 stc-geck-1.4.3/stc_geck/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)    10545 2023-08-08 11:56:01.000000 stc-geck-1.4.3/stc_geck/query_processor.py
+-rw-r--r--   0 pasha      (501) staff       (20)     3254 2023-08-07 18:22:54.000000 stc-geck-1.4.3/stc_geck/utils.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 11:57:02.777516 stc-geck-1.4.3/stc_geck.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-08 11:57:02.000000 stc-geck-1.4.3/stc_geck.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      369 2023-08-08 11:57:02.000000 stc-geck-1.4.3/stc_geck.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-08 11:57:02.000000 stc-geck-1.4.3/stc_geck.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-08 11:57:02.000000 stc-geck-1.4.3/stc_geck.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      172 2023-08-08 11:57:02.000000 stc-geck-1.4.3/stc_geck.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        9 2023-08-08 11:57:02.000000 stc-geck-1.4.3/stc_geck.egg-info/top_level.txt
```

### Comparing `stc-geck-1.4.2/PKG-INFO` & `stc-geck-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stc-geck
-Version: 1.4.2
+Version: 1.4.3
 Summary: GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `stc-geck-1.4.2/README.md` & `stc-geck-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `stc-geck-1.4.2/pyproject.toml` & `stc-geck-1.4.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-geck"
-version = "1.4.2"
+version = "1.4.3"
 authors = [{ name = "Interdimensional Walker" }]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-geck-1.4.2/stc_geck/advices.py` & `stc-geck-1.4.3/stc_geck/advices.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.4.2/stc_geck/cli.py` & `stc-geck-1.4.3/stc_geck/cli.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.4.2/stc_geck/client.py` & `stc-geck-1.4.3/stc_geck/client.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.4.2/stc_geck/query_processor.py` & `stc-geck-1.4.3/stc_geck/query_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,14 +146,16 @@
         extra_filter: Optional[Dict] = None,
         fields: Optional[Union[List[str], Dict[str, List[str]]]] = None,
         skip_doi_isbn_term_field_mapper: bool = False,
         query_language: str = 'en',
     ):
         queries = []
         query = self.process_filters(escape(query, quote=False))
+        if not index_aliases:
+            index_aliases = ["nexus_free", "nexus_science"]
         if isinstance(fields, List):
             new_fields = {}
             for index_alias in index_aliases:
                 new_fields[index_alias] = fields
             fields = new_fields
         for index_alias in index_aliases:
             queries.append(self.query_builders[index_alias].build(
```

### Comparing `stc-geck-1.4.2/stc_geck/utils.py` & `stc-geck-1.4.3/stc_geck/utils.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.4.2/stc_geck.egg-info/PKG-INFO` & `stc-geck-1.4.3/stc_geck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stc-geck
-Version: 1.4.2
+Version: 1.4.3
 Summary: GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

