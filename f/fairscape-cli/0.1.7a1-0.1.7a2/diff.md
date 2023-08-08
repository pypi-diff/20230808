# Comparing `tmp/fairscape_cli-0.1.7a1.tar.gz` & `tmp/fairscape_cli-0.1.7a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairscape_cli-0.1.7a1.tar", max compression
+gzip compressed data, was "fairscape_cli-0.1.7a2.tar", max compression
```

## Comparing `fairscape_cli-0.1.7a1.tar` & `fairscape_cli-0.1.7a2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1066 2023-01-06 17:27:00.899279 fairscape_cli-0.1.7a1/LICENSE
--rw-r--r--   0        0        0      201 2023-08-03 18:18:58.025686 fairscape_cli-0.1.7a1/README.md
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.7a1/fairscape_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.7a1/fairscape_cli/apps/__init__.py
--rw-r--r--   0        0        0      274 2023-03-27 17:08:49.098247 fairscape_cli-0.1.7a1/fairscape_cli/apps/cache.py
--rw-r--r--   0        0        0      510 2023-03-27 17:08:49.098247 fairscape_cli-0.1.7a1/fairscape_cli/apps/describe.py
--rw-r--r--   0        0        0      764 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a1/fairscape_cli/apps/fairscape.py
--rw-r--r--   0        0        0       89 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a1/fairscape_cli/apps/list.py
--rw-r--r--   0        0        0      173 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a1/fairscape_cli/apps/models/__init__.py
--rw-r--r--   0        0        0      340 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a1/fairscape_cli/apps/models/computation.py
--rw-r--r--   0        0        0     2559 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a1/fairscape_cli/apps/models/dataset.py
--rw-r--r--   0        0        0     1890 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a1/fairscape_cli/apps/models/software.py
--rw-r--r--   0        0        0     8135 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a1/fairscape_cli/apps/objects.py
--rw-r--r--   0        0        0     3369 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a1/fairscape_cli/apps/rocrate.py
--rw-r--r--   0        0        0     2276 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a1/fairscape_cli/apps/utils.py
--rw-r--r--   0        0        0     2677 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a1/fairscape_cli/apps/validator.py
--rw-r--r--   0        0        0      397 2023-05-30 16:31:53.800262 fairscape_cli-0.1.7a1/fairscape_cli/main.py
--rw-r--r--   0        0        0      397 2023-08-03 18:18:58.025686 fairscape_cli-0.1.7a1/fairscape_cli/models/__init__.py
--rw-r--r--   0        0        0     8833 2023-08-03 18:20:59.115662 fairscape_cli-0.1.7a1/fairscape_cli/models/bagit.py
--rw-r--r--   0        0        0     1022 2023-08-03 18:21:00.805662 fairscape_cli-0.1.7a1/fairscape_cli/models/base.py
--rw-r--r--   0        0        0      761 2023-08-03 18:18:58.025686 fairscape_cli-0.1.7a1/fairscape_cli/models/computation.py
--rw-r--r--   0        0        0     1371 2023-08-03 18:21:00.175662 fairscape_cli-0.1.7a1/fairscape_cli/models/dataset.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a1/fairscape_cli/models/models.py
--rw-r--r--   0        0        0     8473 2023-08-03 18:20:59.645662 fairscape_cli-0.1.7a1/fairscape_cli/models/rocrate.py
--rw-r--r--   0        0        0    13054 2023-08-02 16:41:43.014515 fairscape_cli-0.1.7a1/fairscape_cli/models/schema.py
--rw-r--r--   0        0        0      710 2023-08-03 18:20:58.235663 fairscape_cli-0.1.7a1/fairscape_cli/models/software.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a1/fairscape_cli/rocrate/__init__.py
--rw-r--r--   0        0        0    25851 2023-08-03 18:18:58.025686 fairscape_cli-0.1.7a1/fairscape_cli/rocrate/rocrate.py
--rw-r--r--   0        0        0     1326 2023-05-30 16:31:53.800262 fairscape_cli-0.1.7a1/fairscape_cli/rocrate/utils.py
--rw-r--r--   0        0        0        0 2023-05-30 16:31:53.800262 fairscape_cli-0.1.7a1/fairscape_cli/schema/__init__.py
--rw-r--r--   0        0        0      338 2023-05-30 16:31:53.800262 fairscape_cli-0.1.7a1/fairscape_cli/schema/schema.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a1/fairscape_cli/validate/__init__.py
--rw-r--r--   0        0        0     1422 2023-08-03 18:18:58.025686 fairscape_cli-0.1.7a1/fairscape_cli/validate/validate_json.py
--rw-r--r--   0        0        0     1541 2023-08-03 18:21:20.975658 fairscape_cli-0.1.7a1/pyproject.toml
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 fairscape_cli-0.1.7a1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-01-06 17:27:00.899279 fairscape_cli-0.1.7a2/LICENSE
+-rw-r--r--   0        0        0      201 2023-08-03 18:18:58.025686 fairscape_cli-0.1.7a2/README.md
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.7a2/fairscape_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.7a2/fairscape_cli/apps/__init__.py
+-rw-r--r--   0        0        0      274 2023-03-27 17:08:49.098247 fairscape_cli-0.1.7a2/fairscape_cli/apps/cache.py
+-rw-r--r--   0        0        0      510 2023-03-27 17:08:49.098247 fairscape_cli-0.1.7a2/fairscape_cli/apps/describe.py
+-rw-r--r--   0        0        0      764 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a2/fairscape_cli/apps/fairscape.py
+-rw-r--r--   0        0        0       89 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a2/fairscape_cli/apps/list.py
+-rw-r--r--   0        0        0      173 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a2/fairscape_cli/apps/models/__init__.py
+-rw-r--r--   0        0        0      340 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a2/fairscape_cli/apps/models/computation.py
+-rw-r--r--   0        0        0     2559 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a2/fairscape_cli/apps/models/dataset.py
+-rw-r--r--   0        0        0     1890 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a2/fairscape_cli/apps/models/software.py
+-rw-r--r--   0        0        0     8135 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a2/fairscape_cli/apps/objects.py
+-rw-r--r--   0        0        0     3369 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a2/fairscape_cli/apps/rocrate.py
+-rw-r--r--   0        0        0     2276 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a2/fairscape_cli/apps/utils.py
+-rw-r--r--   0        0        0     2677 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a2/fairscape_cli/apps/validator.py
+-rw-r--r--   0        0        0      397 2023-05-30 16:31:53.800262 fairscape_cli-0.1.7a2/fairscape_cli/main.py
+-rw-r--r--   0        0        0      397 2023-08-03 18:18:58.025686 fairscape_cli-0.1.7a2/fairscape_cli/models/__init__.py
+-rw-r--r--   0        0        0     8833 2023-08-03 18:20:59.115662 fairscape_cli-0.1.7a2/fairscape_cli/models/bagit.py
+-rw-r--r--   0        0        0     1063 2023-08-08 15:16:38.488994 fairscape_cli-0.1.7a2/fairscape_cli/models/base.py
+-rw-r--r--   0        0        0      812 2023-08-08 16:00:14.248334 fairscape_cli-0.1.7a2/fairscape_cli/models/computation.py
+-rw-r--r--   0        0        0     1371 2023-08-03 18:21:00.175662 fairscape_cli-0.1.7a2/fairscape_cli/models/dataset.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a2/fairscape_cli/models/models.py
+-rw-r--r--   0        0        0     8473 2023-08-03 18:20:59.645662 fairscape_cli-0.1.7a2/fairscape_cli/models/rocrate.py
+-rw-r--r--   0        0        0    13054 2023-08-02 16:41:43.014515 fairscape_cli-0.1.7a2/fairscape_cli/models/schema.py
+-rw-r--r--   0        0        0      695 2023-08-08 15:16:39.878993 fairscape_cli-0.1.7a2/fairscape_cli/models/software.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a2/fairscape_cli/rocrate/__init__.py
+-rw-r--r--   0        0        0    25970 2023-08-08 15:27:23.168830 fairscape_cli-0.1.7a2/fairscape_cli/rocrate/rocrate.py
+-rw-r--r--   0        0        0     1326 2023-05-30 16:31:53.800262 fairscape_cli-0.1.7a2/fairscape_cli/rocrate/utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 16:31:53.800262 fairscape_cli-0.1.7a2/fairscape_cli/schema/__init__.py
+-rw-r--r--   0        0        0      338 2023-05-30 16:31:53.800262 fairscape_cli-0.1.7a2/fairscape_cli/schema/schema.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.7a2/fairscape_cli/validate/__init__.py
+-rw-r--r--   0        0        0     1422 2023-08-03 18:18:58.025686 fairscape_cli-0.1.7a2/fairscape_cli/validate/validate_json.py
+-rw-r--r--   0        0        0     1541 2023-08-08 14:59:44.059248 fairscape_cli-0.1.7a2/pyproject.toml
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 fairscape_cli-0.1.7a2/PKG-INFO
```

### Comparing `fairscape_cli-0.1.7a1/LICENSE` & `fairscape_cli-0.1.7a2/LICENSE`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.7a1/fairscape_cli/apps/fairscape.py` & `fairscape_cli-0.1.7a2/fairscape_cli/apps/fairscape.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.7a1/fairscape_cli/apps/models/dataset.py` & `fairscape_cli-0.1.7a2/fairscape_cli/apps/models/dataset.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.7a1/fairscape_cli/apps/models/software.py` & `fairscape_cli-0.1.7a2/fairscape_cli/apps/models/software.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.7a1/fairscape_cli/apps/objects.py` & `fairscape_cli-0.1.7a2/fairscape_cli/apps/objects.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.7a1/fairscape_cli/apps/rocrate.py` & `fairscape_cli-0.1.7a2/fairscape_cli/apps/rocrate.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.7a1/fairscape_cli/apps/utils.py` & `fairscape_cli-0.1.7a2/fairscape_cli/apps/utils.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.7a1/fairscape_cli/apps/validator.py` & `fairscape_cli-0.1.7a2/fairscape_cli/apps/validator.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.7a1/fairscape_cli/models/bagit.py` & `fairscape_cli-0.1.7a2/fairscape_cli/models/bagit.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.7a1/fairscape_cli/models/base.py` & `fairscape_cli-0.1.7a2/fairscape_cli/models/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,11 +45,12 @@
         title="context",
         alias="@context"
     )
     metadataType: str = Field(
         title="metadataType",
         alias="@type"
     )
-    url: Optional[AnyUrl] = Field(default=None)
-    name: str = Field(max_length=64)
+    url: Optional[str] = Field(default=None)
+    name: str = Field(max_length=200)
     keywords: List[str] = Field(default=[])
+    description: str = Field(min_length=5)
```

### Comparing `fairscape_cli-0.1.7a1/fairscape_cli/models/dataset.py` & `fairscape_cli-0.1.7a2/fairscape_cli/models/dataset.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.7a1/fairscape_cli/models/rocrate.py` & `fairscape_cli-0.1.7a2/fairscape_cli/models/rocrate.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.7a1/fairscape_cli/models/schema.py` & `fairscape_cli-0.1.7a2/fairscape_cli/models/schema.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.7a1/fairscape_cli/models/software.py` & `fairscape_cli-0.1.7a2/fairscape_cli/models/software.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,13 @@
 
 class Software(FairscapeBaseModel): 
     metadataType: str = "https://w3id.org/EVI#Software"
     author: str = Field(min_length=4, max_length=64)
     dateModified: str
     version: str
     description: str =  Field(min_length=10)
-    keywords: List[str] = Field(...)
     associatedPublication: Optional[str]
     additionalDocumentation: Optional[str]
     fileFormat: str = Field(title="fileFormat", alias="format")
     usedByComputation: Optional[List[str]]
-    contentUrl: Optional[str]
+    contentUrl: Optional[str] = Field(default=None)
```

### Comparing `fairscape_cli-0.1.7a1/fairscape_cli/rocrate/rocrate.py` & `fairscape_cli-0.1.7a2/fairscape_cli/rocrate/rocrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 @click.option('--guid', required=False, type=str, default="", show_default=False)
 @click.option('--name',    required=True, prompt = "Software Name")
 @click.option('--author',  required=True, prompt = "Author Name")
 @click.option('--version', required=True, prompt = "Software Version")
 @click.option('--description', required = True, prompt = "Software Description")
 @click.option('--keywords', required=True, multiple=True)
 @click.option('--file-format', required = True, prompt = "File Format of Software")
-@click.option('--url',     required = False)
+@click.option('--url', required = False)
 @click.option('--date-modified', required=False)
 @click.option('--filepath', required=False)
 @click.option('--used-by-computation', required=False, multiple=True)
 @click.option('--associated-publication', required=False)
 @click.option('--additional-documentation', required=False)
 def registerSoftware(
     rocrate_path: pathlib.Path,
@@ -170,24 +170,25 @@
     filepath,
     used_by_computation,
     associated_publication,
     additional_documentation
     ):
     
     metadata_path = rocrate_path / "ro-crate-metadata.json"
+    #click.echo(f"METADATA PATH: {str(metadata_path)}")
 
     # check if you are in the rocrate path
     # ro-crate-metadata.json should be a local file
     if metadata_path.exists() != True:
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
         click.Abort()
 
     crate = ROCrate.model_construct(
         _fields_set={"path"}, 
-        **{"path":"metadata_path"}
+        **{"path": metadata_path}
     ) 
 
 
     software_metadata = {
             "@id": guid,
             "@type": "https://w3id.org/EVI#Software",
             "url": url,
@@ -202,19 +203,21 @@
             "format": file_format,
             # sanitize new line characters for multiple inputs
             "usedByComputation": [
                 computation.strip("\n") for computation in used_by_computation
             ],
         }
 
-    if filepath != "" and filepath is not None:
+    if filepath is not None:
+        if type(filepath) == str:
             # TODO if URL just set
             software_metadata["contentUrl"] = filepath 
-
+        if type(filepath) == pathlib.Path:
             # TODO if pathlike object
+            pass
 
     try:
         software_model = Software(**software_metadata)
         crate.registerSoftware(software_model)
 
     except ValidationError as e:
         click.echo("Software Validation Error")
@@ -266,15 +269,15 @@
     # ro-crate-metadata.json should be a local file
     if metadata_path.exists() != True:
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
         click.Abort()
 
     crate = ROCrate.model_construct(
         _fields_set={"path"}, 
-        **{"path":"metadata_path"}
+        **{"path": metadata_path}
     ) 
 
     dataset_metadata = {
             "@id": guid,
             "@type": "https://w3id.org/EVI#Dataset",
             "url": url,
             "author": author,
@@ -345,15 +348,15 @@
     metadata_path = rocrate_path / "ro-crate-metadata.json"
     if metadata_path.exists() != True:
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
         click.Abort()
 
     crate = ROCrate.model_construct(
         _fields_set={"path"}, 
-        **{"path":"metadata_path"}
+        **{"path": metadata_path}
     ) 
 
     if guid == "":
         guid = generate_id(metadata_path, name, "Computation")
 
     # initilize the model with the required properties
     try:
@@ -423,15 +426,15 @@
     metadata_path = rocrate_path / "ro-crate-metadata.json"
     if metadata_path.exists() != True:
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
         click.Abort()
 
     crate = ROCrate.model_construct(
         _fields_set={"path"}, 
-        **{"path":"metadata_path"}
+        **{"path": metadata_path}
     ) 
 
     if guid == "":
         guid = generate_id(metadata_path, name, "Dataset")
 
     # validate the provided metadata
     try: 
@@ -474,15 +477,15 @@
     metadata_path = rocrate_path / "ro-crate-metadata.json"
     if metadata_path.exists() != True:
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
         click.Abort()
 
     crate = ROCrate.model_construct(
         _fields_set={"path"}, 
-        **{"path":"metadata_path"}
+        **{"path": metadata_path}
     ) 
 
     # TODO check that dataset container is guid
 
     # TODO check that dataset guid is guid
 
     try:
@@ -505,15 +508,15 @@
     metadata_path = rocrate_path / "ro-crate-metadata.json"
     if metadata_path.exists() != True:
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
         click.Abort()
 
     crate = ROCrate.model_construct(
         _fields_set={"path"}, 
-        **{"path":"metadata_path"}
+        **{"path": metadata_path}
     ) 
 
     # TODO check that dataset container is guid
 
     # TODO check that dataset guid is guid
 
     try:
@@ -677,15 +680,15 @@
 
     if guid == "":
         guid = generate_id(metadata_path, name, "Dataset")
 
 
     crate = ROCrate.model_construct(
         _fields_set={"path"}, 
-        **{"path":"metadata_path"}
+        **{"path": metadata_path}
     ) 
     
     try:
         dataset_model = Dataset(   
             **{
             "@id": guid,
             "@type": "https://w3id.org/EVI#Dataset",
```

### Comparing `fairscape_cli-0.1.7a1/fairscape_cli/rocrate/utils.py` & `fairscape_cli-0.1.7a2/fairscape_cli/rocrate/utils.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.7a1/fairscape_cli/validate/validate_json.py` & `fairscape_cli-0.1.7a2/fairscape_cli/validate/validate_json.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.7a1/pyproject.toml` & `fairscape_cli-0.1.7a2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 [project.urls]
 Homepage = "https://github.com/fairscape/fairscape-cli"
 
 
 [tool.poetry]
 name = "fairscape-cli"
-version = "0.1.7a1"
+version = "0.1.7a2"
 description = "A cli for validating metadata, packaging ROCrates, and interacting with the FAIRSCAPE API"
 authors = [
         "Max Levinson",
         "Sadnan Al Manir", 
         "Tim Clark"
 ]
 license = "LICENSE"
```

### Comparing `fairscape_cli-0.1.7a1/PKG-INFO` & `fairscape_cli-0.1.7a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairscape-cli
-Version: 0.1.7a1
+Version: 0.1.7a2
 Summary: A cli for validating metadata, packaging ROCrates, and interacting with the FAIRSCAPE API
 License: LICENSE
 Author: Max Levinson
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

