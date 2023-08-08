# Comparing `tmp/yente-3.6.0.tar.gz` & `tmp/yente-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yente-3.6.0.tar", last modified: Mon Jul 24 07:45:56 2023, max compression
+gzip compressed data, was "yente-3.6.1.tar", last modified: Tue Aug  8 13:49:03 2023, max compression
```

## Comparing `yente-3.6.0.tar` & `yente-3.6.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:45:56.321580 yente-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-24 07:44:08.000000 yente-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-24 07:44:08.000000 yente-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-24 07:45:56.321580 yente-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-24 07:44:08.000000 yente-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 07:45:56.321580 yente-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-24 07:44:08.000000 yente-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:45:56.317580 yente-3.6.0/yente/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:44:08.000000 yente-3.6.0/yente/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-24 07:44:08.000000 yente-3.6.0/yente/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-24 07:44:08.000000 yente-3.6.0/yente/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:45:56.317580 yente-3.6.0/yente/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-24 07:44:08.000000 yente-3.6.0/yente/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-24 07:44:08.000000 yente-3.6.0/yente/data/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-24 07:44:08.000000 yente-3.6.0/yente/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-24 07:44:08.000000 yente-3.6.0/yente/data/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-24 07:44:08.000000 yente-3.6.0/yente/data/freebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-24 07:44:08.000000 yente-3.6.0/yente/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-24 07:44:08.000000 yente-3.6.0/yente/data/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-24 07:44:08.000000 yente-3.6.0/yente/data/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-24 07:44:08.000000 yente-3.6.0/yente/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 07:44:08.000000 yente-3.6.0/yente/reindex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:45:56.317580 yente-3.6.0/yente/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-24 07:44:08.000000 yente-3.6.0/yente/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:45:56.321580 yente-3.6.0/yente/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:44:08.000000 yente-3.6.0/yente/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-24 07:44:08.000000 yente-3.6.0/yente/routers/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-24 07:44:08.000000 yente-3.6.0/yente/routers/match.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-24 07:44:08.000000 yente-3.6.0/yente/routers/reconcile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-24 07:44:08.000000 yente-3.6.0/yente/routers/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-24 07:44:08.000000 yente-3.6.0/yente/routers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-24 07:44:08.000000 yente-3.6.0/yente/scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:45:56.321580 yente-3.6.0/yente/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:44:08.000000 yente-3.6.0/yente/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-24 07:44:08.000000 yente-3.6.0/yente/search/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-07-24 07:44:08.000000 yente-3.6.0/yente/search/indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-24 07:44:08.000000 yente-3.6.0/yente/search/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-24 07:44:08.000000 yente-3.6.0/yente/search/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-07-24 07:44:08.000000 yente-3.6.0/yente/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-24 07:44:08.000000 yente-3.6.0/yente/search/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-24 07:44:08.000000 yente-3.6.0/yente/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-24 07:44:08.000000 yente-3.6.0/yente/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-24 07:44:08.000000 yente-3.6.0/yente/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:45:56.317580 yente-3.6.0/yente.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-24 07:45:56.000000 yente-3.6.0/yente.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-24 07:45:56.000000 yente-3.6.0/yente.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:45:56.000000 yente-3.6.0/yente.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 07:45:56.000000 yente-3.6.0/yente.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:45:56.000000 yente-3.6.0/yente.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:44:23.000000 yente-3.6.0/yente.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 07:45:56.000000 yente-3.6.0/yente.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 07:45:56.000000 yente-3.6.0/yente.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:49:03.120693 yente-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-08 13:46:50.000000 yente-3.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-08 13:46:50.000000 yente-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-08-08 13:49:03.116693 yente-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-08 13:46:50.000000 yente-3.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 13:49:03.120693 yente-3.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-08 13:46:50.000000 yente-3.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:49:03.112693 yente-3.6.1/yente/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:46:50.000000 yente-3.6.1/yente/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-08-08 13:46:50.000000 yente-3.6.1/yente/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-08 13:46:50.000000 yente-3.6.1/yente/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:49:03.116693 yente-3.6.1/yente/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-08 13:46:50.000000 yente-3.6.1/yente/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-08-08 13:46:50.000000 yente-3.6.1/yente/data/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-08-08 13:46:50.000000 yente-3.6.1/yente/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-08 13:46:50.000000 yente-3.6.1/yente/data/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-08-08 13:46:50.000000 yente-3.6.1/yente/data/freebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-08-08 13:46:50.000000 yente-3.6.1/yente/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-08-08 13:46:50.000000 yente-3.6.1/yente/data/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-08-08 13:46:50.000000 yente-3.6.1/yente/data/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-08-08 13:46:50.000000 yente-3.6.1/yente/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-08 13:46:50.000000 yente-3.6.1/yente/reindex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:49:03.116693 yente-3.6.1/yente/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-08-08 13:46:50.000000 yente-3.6.1/yente/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:49:03.116693 yente-3.6.1/yente/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:46:50.000000 yente-3.6.1/yente/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-08-08 13:46:50.000000 yente-3.6.1/yente/routers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-08-08 13:46:50.000000 yente-3.6.1/yente/routers/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-08-08 13:46:50.000000 yente-3.6.1/yente/routers/reconcile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-08-08 13:46:50.000000 yente-3.6.1/yente/routers/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-08 13:46:50.000000 yente-3.6.1/yente/routers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-08 13:46:50.000000 yente-3.6.1/yente/scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:49:03.116693 yente-3.6.1/yente/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:46:50.000000 yente-3.6.1/yente/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-08-08 13:46:50.000000 yente-3.6.1/yente/search/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-08-08 13:46:50.000000 yente-3.6.1/yente/search/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-08-08 13:46:50.000000 yente-3.6.1/yente/search/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-08-08 13:46:50.000000 yente-3.6.1/yente/search/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-08-08 13:46:50.000000 yente-3.6.1/yente/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-08-08 13:46:50.000000 yente-3.6.1/yente/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-08 13:46:50.000000 yente-3.6.1/yente/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-08-08 13:46:50.000000 yente-3.6.1/yente/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-08 13:46:50.000000 yente-3.6.1/yente/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:49:03.116693 yente-3.6.1/yente.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-08-08 13:49:02.000000 yente-3.6.1/yente.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-08 13:49:03.000000 yente-3.6.1/yente.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:49:02.000000 yente-3.6.1/yente.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-08 13:49:02.000000 yente-3.6.1/yente.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:49:02.000000 yente-3.6.1/yente.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:47:08.000000 yente-3.6.1/yente.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-08 13:49:02.000000 yente-3.6.1/yente.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 13:49:02.000000 yente-3.6.1/yente.egg-info/top_level.txt
```

### Comparing `yente-3.6.0/LICENSE` & `yente-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/PKG-INFO` & `yente-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.6.0
+Version: 3.6.1
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `yente-3.6.0/README.md` & `yente-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/setup.py` & `yente-3.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,46 +2,46 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="yente",
-    version="3.6.0",
+    version="3.6.1",
     url="https://opensanctions.org/docs/api/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     author="OpenSanctions",
     author_email="info@opensanctions.org",
     packages=find_packages(exclude=["examples", "tests"]),
     namespace_packages=[],
     install_requires=[
         "followthemoney==3.5.1",
-        "nomenklatura==3.3.4",
+        "nomenklatura==3.3.8",
         "asyncstdlib==3.10.8",
         "aiocron==1.8",
         "aiocsv==1.2.4",
         "aiofiles==23.1.0",
         "types-aiofiles>=23.1.0.4,<23.2",
         "aiohttp[speedups]==3.8.5",
-        "elasticsearch[async]==8.8.2",
-        "fastapi==0.100.0",
-        "uvicorn[standard]==0.23.1",
+        "elasticsearch[async]==8.9.0",
+        "fastapi==0.101.0",
+        "uvicorn[standard]==0.23.2",
         "python-multipart==0.0.6",
         "email-validator==2.0.0.post2",
         "structlog==23.1.0",
         "pyicu==2.11",
         "jellyfish==1.0.0",
-        "orjson==3.9.2",
+        "orjson==3.9.4",
         "text-unidecode==1.3",
         "click==8.1.6",
         "normality==2.4.0",
         "languagecodes==1.1.1",
-        "countrynames==1.15.1",
+        "countrynames==1.15.2",
         "fingerprints==1.1.0",
         "pantomime==0.6.1",
     ],
     extras_require={
         "dev": [
             "pip>=10.0.0",
             "bump2version",
```

### Comparing `yente-3.6.0/yente/app.py` & `yente-3.6.1/yente/app.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/cli.py` & `yente-3.6.1/yente/cli.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/data/__init__.py` & `yente-3.6.1/yente/data/__init__.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/data/common.py` & `yente-3.6.1/yente/data/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     id: str = Field(..., examples=["NK-A7z...."])
     caption: str = Field(..., examples=["John Doe"])
     schema_: str = Field(..., examples=["LegalEntity"], alias="schema")
     properties: EntityProperties = Field(..., examples=[{"name": ["John Doe"]}])
     datasets: List[str] = Field([], examples=[["us_ofac_sdn"]])
     referents: List[str] = Field([], examples=[["ofac-1234"]])
     target: bool = Field(False)
-    first_seen: Optional[datetime] = Field(..., examples=[datetime.utcnow()])
-    last_seen: Optional[datetime] = Field(..., examples=[datetime.utcnow()])
-    last_change: Optional[datetime] = Field(..., examples=[datetime.utcnow()])
+    first_seen: Optional[datetime] = Field(None, examples=[datetime.utcnow()])
+    last_seen: Optional[datetime] = Field(None, examples=[datetime.utcnow()])
+    last_change: Optional[datetime] = Field(None, examples=[datetime.utcnow()])
 
     @classmethod
     def from_entity(cls, entity: Entity) -> "EntityResponse":
         return cls.model_validate(entity.to_dict())
 
 
 EntityResponse.model_rebuild()
```

### Comparing `yente-3.6.0/yente/data/dataset.py` & `yente-3.6.1/yente/data/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 class Dataset(NKDataset):
     def __init__(self, catalog: DataCatalog["Dataset"], data: Dict[str, Any]):
         name = data["name"]
         norm_name = slugify(name, sep="_")
         if name != norm_name:
             raise ValueError("Invalid dataset name %r (try: %r)" % (name, norm_name))
         super().__init__(catalog, data)
-        self._children.update(data.get("scopes", []))
 
         if self.version is None:
             ts = data.get("last_export", BOOT_TIME)
             self.version = iso_to_version(ts) or "static"
 
         self.load = as_bool(data.get("load"), True)
         self.entities_url = self._get_entities_url(data)
```

### Comparing `yente-3.6.0/yente/data/freebase.py` & `yente-3.6.1/yente/data/freebase.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/data/loader.py` & `yente-3.6.1/yente/data/loader.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/data/manifest.py` & `yente-3.6.1/yente/data/manifest.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/data/util.py` & `yente-3.6.1/yente/data/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/logs.py` & `yente-3.6.1/yente/logs.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/resources/favicon.ico` & `yente-3.6.1/yente/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/routers/admin.py` & `yente-3.6.1/yente/routers/admin.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/routers/match.py` & `yente-3.6.1/yente/routers/match.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import asyncio
-from typing import Dict
+from typing import Dict, List
 from fastapi import APIRouter, Query, Response, HTTPException
+from nomenklatura.matching import ALGORITHMS, get_algorithm
 
 from yente import settings
 from yente.logs import get_logger
 from yente.data.common import ErrorResponse
 from yente.data.common import EntityMatchQuery, EntityMatchResponse, EntityExample
 from yente.data.common import EntityMatches
 from yente.search.queries import entity_query
 from yente.search.search import search_entities, result_entities, result_total
 from yente.data.entity import Entity
 from yente.util import limit_window
 from yente.scoring import score_results
-from nomenklatura.matching import ALGORITHMS, get_algorithm
 from yente.routers.util import get_dataset
 from yente.routers.util import PATH_DATASET
 
 log = get_logger(__name__)
 router = APIRouter()
 
 ALGO_LIST = ", ".join([a.NAME for a in ALGORITHMS])
@@ -49,14 +49,20 @@
         settings.SCORE_CUTOFF,
         title="Lower bound of score for results to be returned at all",
     ),
     algorithm: str = Query(
         settings.DEFAULT_ALGORITHM,
         title=f"Scoring algorithm to use, options: {ALGO_LIST}",
     ),
+    exclude_schema: List[str] = Query(
+        [], title="Remove the given types of entities from results"
+    ),
+    exclude_dataset: List[str] = Query(
+        [], title="Remove the given datasets from results"
+    ),
     fuzzy: bool = Query(
         settings.MATCH_FUZZY,
         title="Use slow matching for candidate generation, does not affect scores",
     ),
 ) -> EntityMatchResponse:
     """Match entities based on a complex set of criteria, like name, date of birth
     and nationality of a person. This works by submitting a batch of entities, each
@@ -124,22 +130,32 @@
     queries = []
     entities = []
     responses: Dict[str, EntityMatches] = {}
 
     for name, example in match.queries.items():
         try:
             entity = Entity.from_example(example)
-            query = entity_query(ds, entity, fuzzy=fuzzy)
+            query = entity_query(
+                ds,
+                entity,
+                fuzzy=fuzzy,
+                exclude_schema=exclude_schema,
+                exclude_dataset=exclude_dataset,
+            )
         except Exception as exc:
             log.info("Cannot parse example entity: %s" % str(exc))
             raise HTTPException(
                 status_code=400,
                 detail=f"Cannot parse example entity: {exc}",
             )
-        queries.append(search_entities(query, limit=limit * 10))
+        # We're using a higher limit for candidate generation, because we want to
+        # get a broad range of candidates to score against. This is a trade-off
+        # between speed and accuracy.
+        candidates = limit * settings.MATCH_CANDIDATES
+        queries.append(search_entities(query, limit=candidates))
         entities.append((name, entity))
     if not len(queries) and not len(responses):
         raise HTTPException(400, detail="No queries provided.")
     results = await asyncio.gather(*queries)
 
     for (name, entity), resp in zip(entities, results):
         ents = result_entities(resp)
```

### Comparing `yente-3.6.0/yente/routers/reconcile.py` & `yente-3.6.1/yente/routers/reconcile.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/routers/search.py` & `yente-3.6.1/yente/routers/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,17 @@
     dataset: str = PATH_DATASET,
     schema: str = Query(
         settings.BASE_SCHEMA, title="Types of entities that can match the search"
     ),
     exclude_schema: List[str] = Query(
         [], title="Remove the given types of entities from results"
     ),
+    exclude_dataset: List[str] = Query(
+        [], title="Remove the given datasets from results"
+    ),
     countries: List[str] = Query([], title="Filter by country codes"),
     topics: List[str] = Query(
         [], title="Filter by entity topics (e.g. sanction, role.pep)"
     ),
     datasets: List[str] = Query([], title="Filter by data sources"),
     limit: int = Query(10, title="Number of results to return", le=settings.MAX_PAGE),
     offset: int = Query(
@@ -80,14 +83,15 @@
         ds,
         schema_obj,
         q,
         filters=filters,
         fuzzy=fuzzy,
         simple=simple,
         exclude_schema=exclude_schema,
+        exclude_dataset=exclude_dataset,
     )
     aggregations = facet_aggregations([f for f in filters.keys()])
     resp = await search_entities(
         query,
         limit=limit,
         offset=offset,
         aggregations=aggregations,
```

### Comparing `yente-3.6.0/yente/routers/util.py` & `yente-3.6.1/yente/routers/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/scoring.py` & `yente-3.6.1/yente/scoring.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/search/base.py` & `yente-3.6.1/yente/search/base.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/search/indexer.py` & `yente-3.6.1/yente/search/indexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         "Indexing entities",
         dataset=dataset.name,
         url=dataset.entities_url,
         version=version,
     )
     dataset_prefix = f"{settings.ENTITY_INDEX}-{dataset.name}"
     next_index = f"{dataset_prefix}-{version}"
-    exists = await es.indices.exists(index=next_index)
+    exists = await es.indices.exists_alias(name=settings.ENTITY_INDEX, index=next_index)
     if exists.body and not force:
         log.info("Index is up to date.", index=next_index)
         return False
 
     # await es.indices.delete(index=next_index)
     log.info("Create index", index=next_index)
     try:
```

### Comparing `yente-3.6.0/yente/search/mapping.py` & `yente-3.6.1/yente/search/mapping.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/search/nested.py` & `yente-3.6.1/yente/search/nested.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/search/queries.py` & `yente-3.6.1/yente/search/queries.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 
 def filter_query(
     shoulds: List[Clause],
     dataset: Optional[Dataset] = None,
     schema: Optional[Schema] = None,
     filters: FilterDict = {},
     exclude_schema: List[str] = [],
+    exclude_dataset: List[str] = [],
 ) -> Clause:
     filterqs: List[Clause] = []
     if dataset is not None:
-        filterqs.append({"terms": {"datasets": dataset.dataset_names}})
+        ds = [d for d in dataset.dataset_names if d not in exclude_dataset]
+        filterqs.append({"terms": {"datasets": ds}})
     if schema is not None:
         schemata = schema.matchable_schemata
         schemata.add(schema)
         if not schema.matchable:
             schemata.update(schema.descendants)
         names = [s.name for s in schemata]
         filterqs.append({"terms": {"schema": names}})
@@ -69,39 +71,52 @@
     for token in name_words(names):
         shoulds.append({"term": {NAME_PART_FIELD: {"value": token}}})
     for phoneme in soundex_names(names):
         shoulds.append({"term": {SOUNDEX_FIELD: {"value": phoneme}}})
     return shoulds
 
 
-def entity_query(dataset: Dataset, entity: EntityProxy, fuzzy: bool = True) -> Clause:
+def entity_query(
+    dataset: Dataset,
+    entity: EntityProxy,
+    fuzzy: bool = True,
+    exclude_schema: List[str] = [],
+    exclude_dataset: List[str] = [],
+) -> Clause:
     shoulds: List[Clause] = []
     for prop, value in entity.itervalues():
         if prop.type == registry.name or not prop.matchable:
             continue
         if prop.type == registry.address:
             query = {"match": {prop.type.group: value}}
             shoulds.append(query)
         elif prop.type.group is not None:
             shoulds.append({"term": {prop.type.group: value}})
         elif fuzzy:
             shoulds.append({"match": {"text": value}})
 
     shoulds.extend(names_query(entity, fuzzy=fuzzy))
-    return filter_query(shoulds, dataset=dataset, schema=entity.schema)
+    return filter_query(
+        shoulds,
+        dataset=dataset,
+        schema=entity.schema,
+        exclude_schema=exclude_schema,
+        exclude_dataset=exclude_dataset,
+    )
 
 
 def text_query(
     dataset: Dataset,
     schema: Schema,
     query: str,
     filters: FilterDict = {},
     fuzzy: bool = False,
     simple: bool = False,
     exclude_schema: List[str] = [],
+    exclude_dataset: List[str] = [],
 ) -> Clause:
     if not len(query.strip()):
         should: Clause = {"match_all": {}}
     elif simple:
         should = {
             "simple_query_string": {
                 "query": query,
@@ -125,14 +140,15 @@
         # log.info("Query", should=should)
     return filter_query(
         [should],
         dataset=dataset,
         schema=schema,
         filters=filters,
         exclude_schema=exclude_schema,
+        exclude_dataset=exclude_dataset,
     )
 
 
 def prefix_query(
     dataset: Dataset,
     prefix: str,
 ) -> Clause:
```

### Comparing `yente-3.6.0/yente/search/search.py` & `yente-3.6.1/yente/search/search.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente/settings.py` & `yente-3.6.1/yente/settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def env_str(name: str, default: Optional[str] = None) -> Optional[str]:
     """Ensure the env returns a string even on Windows (#100)."""
     value = stringify(env.get(name))
     return default if value is None else value
 
 
-VERSION = "3.6.0"
+VERSION = "3.6.1"
 AUTHOR = "OpenSanctions"
 HOME_PAGE = "https://www.opensanctions.org"
 EMAIL = "info@opensanctions.org"
 CONTACT = {"name": AUTHOR, "url": HOME_PAGE, "email": EMAIL}
 
 TITLE = env_str("YENTE_TITLE") or "yente"
 DESCRIPTION = """
@@ -103,36 +103,56 @@
 BASE_SCHEMA = "Thing"
 PORT = int(env_str("YENTE_PORT") or env_str("PORT") or "8000")
 UPDATE_TOKEN = env_str("YENTE_UPDATE_TOKEN", "unsafe-default")
 CACHE_HEADERS = {
     "Cache-Control": "public; max-age=3600",
     "X-Robots-Tag": "none",
 }
+# How many results to return per page of search results max:
 MAX_PAGE = 500
+
+# How many entities to accept in a /match batch at most:
 MAX_BATCH = int(env_str("YENTE_MAX_BATCH") or "100")
 MAX_RESULTS = 9999
 MAX_OFFSET = MAX_RESULTS - MAX_PAGE
-MAX_MATCHES = 10
+
+# How many results to return per /match query by default:
 MATCH_PAGE = int(env_str("YENTE_MATCH_PAGE") or "5")
+
+# How many results to return per /match query at most:
+MAX_MATCHES = int(env_str("YENTE_MAX_MATCHES") or "10")
+
+# How many candidates to retrieve as a multiplier of the /match limit:
+MATCH_CANDIDATES = int(env_str("YENTE_MATCH_CANDIDATES") or "10")
+
+# Whether to run expensive levenshtein queries inside ElasticSearch:
 MATCH_FUZZY = as_bool(env_str("YENTE_MATCH_FUZZY") or "true")
+
+# How many match and search queries to run against ES in parallel:
 QUERY_CONCURRENCY = int(env_str("YENTE_QUERY_CONCURRENCY") or "10")
+
+# How many index operations to run against ES in parallel:
 INDEX_CONCURRENCY = int(env_str("YENTE_INDEX_CONCURRENCY") or "5")
 
+# Default scoring threshold for /match results:
 SCORE_THRESHOLD = 0.70
+
+# Default cutoff for scores that should not be returned as /match results:
 SCORE_CUTOFF = 0.10
 
 # ElasticSearch settings:
 ES_URL = env_str("YENTE_ELASTICSEARCH_URL", "http://localhost:9200")
 ES_USERNAME = env_str("YENTE_ELASTICSEARCH_USERNAME")
 ES_PASSWORD = env_str("YENTE_ELASTICSEARCH_PASSWORD")
 ES_CLOUD_ID = env_str("YENTE_ELASTICSEARCH_CLOUD_ID")
 ES_SNIFF = as_bool(env_str("YENTE_ELASTICSEARCH_SNIFF") or "false")
 ES_INDEX = env_str("YENTE_ELASTICSEARCH_INDEX", "yente")
 ES_SHARDS = int(env_str("YENTE_ELASTICSEARCH_SHARDS") or "1")
 ENTITY_INDEX = f"{ES_INDEX}-entities"
 INDEX_VERSION = env_str("YENTE_INDEX_VERSION", "005")
 
+# Log output can be formatted as JSON:
 LOG_JSON = as_bool(env_str("YENTE_LOG_JSON", "false"))
 LOG_LEVEL = logging.DEBUG if DEBUG else logging.INFO
 
 # Used to pad out first_seen, last_seen on static collections
 RUN_TIME = datetime.utcnow().isoformat()[:19]
```

### Comparing `yente-3.6.0/yente/util.py` & `yente-3.6.1/yente/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente.egg-info/PKG-INFO` & `yente-3.6.1/yente.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.6.0
+Version: 3.6.1
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `yente-3.6.0/yente.egg-info/SOURCES.txt` & `yente-3.6.1/yente.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yente-3.6.0/yente.egg-info/requires.txt` & `yente-3.6.1/yente.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 followthemoney==3.5.1
-nomenklatura==3.3.4
+nomenklatura==3.3.8
 asyncstdlib==3.10.8
 aiocron==1.8
 aiocsv==1.2.4
 aiofiles==23.1.0
 types-aiofiles<23.2,>=23.1.0.4
 aiohttp[speedups]==3.8.5
-elasticsearch[async]==8.8.2
-fastapi==0.100.0
-uvicorn[standard]==0.23.1
+elasticsearch[async]==8.9.0
+fastapi==0.101.0
+uvicorn[standard]==0.23.2
 python-multipart==0.0.6
 email-validator==2.0.0.post2
 structlog==23.1.0
 pyicu==2.11
 jellyfish==1.0.0
-orjson==3.9.2
+orjson==3.9.4
 text-unidecode==1.3
 click==8.1.6
 normality==2.4.0
 languagecodes==1.1.1
-countrynames==1.15.1
+countrynames==1.15.2
 fingerprints==1.1.0
 pantomime==0.6.1
 
 [dev]
 pip>=10.0.0
 bump2version
 wheel>=0.29.0
```

