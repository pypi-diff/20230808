# Comparing `tmp/glean-cli-0.7.2.tar.gz` & `tmp/glean-cli-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glean-cli-0.7.2.tar", last modified: Thu Aug  3 21:06:05 2023, max compression
+gzip compressed data, was "glean-cli-0.7.3.tar", last modified: Tue Aug  8 18:48:18 2023, max compression
```

## Comparing `glean-cli-0.7.2.tar` & `glean-cli-0.7.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2023-08-03 21:06:05.447640 glean-cli-0.7.2/
--rw-r--r--   0 dse        (501) staff       (20)    11357 2021-08-09 13:38:38.000000 glean-cli-0.7.2/LICENSE
--rw-r--r--   0 dse        (501) staff       (20)     1209 2023-08-03 21:06:05.447709 glean-cli-0.7.2/PKG-INFO
--rw-r--r--   0 dse        (501) staff       (20)      758 2023-08-01 21:35:43.000000 glean-cli-0.7.2/README.md
--rw-r--r--   0 dse        (501) staff       (20)      103 2021-08-09 13:48:34.000000 glean-cli-0.7.2/pyproject.toml
--rw-r--r--   0 dse        (501) staff       (20)      835 2023-08-03 21:06:05.448075 glean-cli-0.7.2/setup.cfg
--rw-r--r--   0 dse        (501) staff       (20)       38 2021-09-03 21:01:45.000000 glean-cli-0.7.2/setup.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2023-08-03 21:06:05.442118 glean-cli-0.7.2/src/
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2023-08-03 21:06:05.444602 glean-cli-0.7.2/src/glean/
--rw-r--r--   0 dse        (501) staff       (20)       18 2023-08-03 21:05:52.000000 glean-cli-0.7.2/src/glean/__init__.py
--rw-r--r--   0 dse        (501) staff       (20)    31696 2023-08-03 21:05:52.000000 glean-cli-0.7.2/src/glean/cli.py
--rw-r--r--   0 dse        (501) staff       (20)      146 2023-08-01 21:35:43.000000 glean-cli-0.7.2/src/glean/constants.py
--rw-r--r--   0 dse        (501) staff       (20)     1598 2022-10-27 21:08:22.000000 glean-cli-0.7.2/src/glean/credentials.py
--rw-r--r--   0 dse        (501) staff       (20)     3904 2023-06-16 13:01:39.000000 glean-cli-0.7.2/src/glean/filesystem.py
--rw-r--r--   0 dse        (501) staff       (20)    17544 2023-08-01 21:35:43.000000 glean-cli-0.7.2/src/glean/glean_api.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2023-08-03 21:06:05.445830 glean-cli-0.7.2/src/glean/utils/
--rw-r--r--   0 dse        (501) staff       (20)        0 2022-10-27 21:08:22.000000 glean-cli-0.7.2/src/glean/utils/__init__.py
--rw-r--r--   0 dse        (501) staff       (20)      509 2022-10-27 21:08:22.000000 glean-cli-0.7.2/src/glean/utils/cli.py
--rw-r--r--   0 dse        (501) staff       (20)     2778 2023-08-03 21:05:52.000000 glean-cli-0.7.2/src/glean/utils/grn.py
--rw-r--r--   0 dse        (501) staff       (20)     1356 2023-06-20 18:52:16.000000 glean-cli-0.7.2/src/glean/utils/resource.py
--rw-r--r--   0 dse        (501) staff       (20)     1089 2023-06-15 15:12:56.000000 glean-cli-0.7.2/src/glean/utils/validate_config.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2023-08-03 21:06:05.446738 glean-cli-0.7.2/src/glean_cli.egg-info/
--rw-r--r--   0 dse        (501) staff       (20)     1209 2023-08-03 21:06:05.000000 glean-cli-0.7.2/src/glean_cli.egg-info/PKG-INFO
--rw-r--r--   0 dse        (501) staff       (20)      639 2023-08-03 21:06:05.000000 glean-cli-0.7.2/src/glean_cli.egg-info/SOURCES.txt
--rw-r--r--   0 dse        (501) staff       (20)        1 2023-08-03 21:06:05.000000 glean-cli-0.7.2/src/glean_cli.egg-info/dependency_links.txt
--rw-r--r--   0 dse        (501) staff       (20)       41 2023-08-03 21:06:05.000000 glean-cli-0.7.2/src/glean_cli.egg-info/entry_points.txt
--rw-r--r--   0 dse        (501) staff       (20)      121 2023-08-03 21:06:05.000000 glean-cli-0.7.2/src/glean_cli.egg-info/requires.txt
--rw-r--r--   0 dse        (501) staff       (20)        6 2023-08-03 21:06:05.000000 glean-cli-0.7.2/src/glean_cli.egg-info/top_level.txt
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2023-08-03 21:06:05.447515 glean-cli-0.7.2/tests/
--rw-r--r--   0 dse        (501) staff       (20)      309 2022-10-27 21:08:22.000000 glean-cli-0.7.2/tests/test_cli.py
--rw-r--r--   0 dse        (501) staff       (20)     1652 2022-10-27 21:08:22.000000 glean-cli-0.7.2/tests/test_credentials.py
--rw-r--r--   0 dse        (501) staff       (20)     4632 2023-06-20 18:52:16.000000 glean-cli-0.7.2/tests/test_filesystem.py
--rw-r--r--   0 dse        (501) staff       (20)      666 2022-10-27 21:08:22.000000 glean-cli-0.7.2/tests/test_glean_api.py
+drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-08-08 18:48:18.207608 glean-cli-0.7.3/
+-rw-r--r--   0 calderhoover   (501) staff       (20)    11357 2023-03-17 14:57:47.000000 glean-cli-0.7.3/LICENSE
+-rw-r--r--   0 calderhoover   (501) staff       (20)     1209 2023-08-08 18:48:18.207663 glean-cli-0.7.3/PKG-INFO
+-rw-r--r--   0 calderhoover   (501) staff       (20)      758 2023-07-26 17:48:44.000000 glean-cli-0.7.3/README.md
+-rw-r--r--   0 calderhoover   (501) staff       (20)      103 2023-03-17 14:57:47.000000 glean-cli-0.7.3/pyproject.toml
+-rw-r--r--   0 calderhoover   (501) staff       (20)      835 2023-08-08 18:48:18.207906 glean-cli-0.7.3/setup.cfg
+-rw-r--r--   0 calderhoover   (501) staff       (20)       38 2023-03-17 14:57:47.000000 glean-cli-0.7.3/setup.py
+drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-08-08 18:48:18.201981 glean-cli-0.7.3/src/
+drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-08-08 18:48:18.204244 glean-cli-0.7.3/src/glean/
+-rw-r--r--   0 calderhoover   (501) staff       (20)       18 2023-08-08 18:48:05.000000 glean-cli-0.7.3/src/glean/__init__.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)    32204 2023-08-08 18:11:17.000000 glean-cli-0.7.3/src/glean/cli.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)      146 2023-07-31 15:36:44.000000 glean-cli-0.7.3/src/glean/constants.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)     1598 2023-03-17 14:57:47.000000 glean-cli-0.7.3/src/glean/credentials.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)     3904 2023-07-11 21:20:42.000000 glean-cli-0.7.3/src/glean/filesystem.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)    17685 2023-08-08 18:11:17.000000 glean-cli-0.7.3/src/glean/glean_api.py
+drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-08-08 18:48:18.205819 glean-cli-0.7.3/src/glean/utils/
+-rw-r--r--   0 calderhoover   (501) staff       (20)        0 2023-03-17 14:57:47.000000 glean-cli-0.7.3/src/glean/utils/__init__.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)      509 2023-07-31 15:36:25.000000 glean-cli-0.7.3/src/glean/utils/cli.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)     2778 2023-08-08 15:09:04.000000 glean-cli-0.7.3/src/glean/utils/grn.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)     1356 2023-07-11 21:20:42.000000 glean-cli-0.7.3/src/glean/utils/resource.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)     1089 2023-07-11 21:20:42.000000 glean-cli-0.7.3/src/glean/utils/validate_config.py
+drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-08-08 18:48:18.206544 glean-cli-0.7.3/src/glean_cli.egg-info/
+-rw-r--r--   0 calderhoover   (501) staff       (20)     1209 2023-08-08 18:48:18.000000 glean-cli-0.7.3/src/glean_cli.egg-info/PKG-INFO
+-rw-r--r--   0 calderhoover   (501) staff       (20)      639 2023-08-08 18:48:18.000000 glean-cli-0.7.3/src/glean_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 calderhoover   (501) staff       (20)        1 2023-08-08 18:48:18.000000 glean-cli-0.7.3/src/glean_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 calderhoover   (501) staff       (20)       41 2023-08-08 18:48:18.000000 glean-cli-0.7.3/src/glean_cli.egg-info/entry_points.txt
+-rw-r--r--   0 calderhoover   (501) staff       (20)      121 2023-08-08 18:48:18.000000 glean-cli-0.7.3/src/glean_cli.egg-info/requires.txt
+-rw-r--r--   0 calderhoover   (501) staff       (20)        6 2023-08-08 18:48:18.000000 glean-cli-0.7.3/src/glean_cli.egg-info/top_level.txt
+drwxr-xr-x   0 calderhoover   (501) staff       (20)        0 2023-08-08 18:48:18.207496 glean-cli-0.7.3/tests/
+-rw-r--r--   0 calderhoover   (501) staff       (20)      309 2023-03-17 14:57:47.000000 glean-cli-0.7.3/tests/test_cli.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)     1652 2023-03-17 14:57:47.000000 glean-cli-0.7.3/tests/test_credentials.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)     4632 2023-07-11 21:20:42.000000 glean-cli-0.7.3/tests/test_filesystem.py
+-rw-r--r--   0 calderhoover   (501) staff       (20)      666 2023-03-17 14:57:47.000000 glean-cli-0.7.3/tests/test_glean_api.py
```

### Comparing `glean-cli-0.7.2/LICENSE` & `glean-cli-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.2/PKG-INFO` & `glean-cli-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-cli
-Version: 0.7.2
+Version: 0.7.3
 Summary: Command-line tools for interacting with Glean
 Home-page: https://glean.io/
 Author: Dan Eisenberg
 Author-email: dse@glean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `glean-cli-0.7.2/README.md` & `glean-cli-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.2/setup.cfg` & `glean-cli-0.7.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.2/src/glean/cli.py` & `glean-cli-0.7.3/src/glean/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,19 +350,26 @@
 @click.argument("grn", required=False, type=str)
 @click.option(
     "--allow-dirty",
     is_flag=True,
     default=False,
     help="Overwrite resources even if the working directory has changes",
 )
+@click.option(
+    "--all",
+    is_flag=True,
+    default=False,
+    help="Pull all project resources, including those not managed by DataOps."
+)
 @click.pass_context
 def pull(
     ctx: click.Context,
     grn: str,
     allow_dirty: bool = False,
+    all: bool = False,
 ):
     """Pull the latest DataOps resource configuration from Glean into the working directory.
 
     GRN is the Glean resource name of the target resource. If the resource has DataOps dependencies, they will also be
     retrieved. If no GRN is specified, all resources for the project are pulled.
     """
     ctx.obj["credentials"] = get_credentials(ctx.obj["credentials_filepath"])
@@ -402,16 +409,24 @@
         try:
             resource_type = RESOURCE_TYPE_FROM_ABBREV[grn_components.resource_type]
         except:
             raise click.ClickException(
                 "Glean pull currently only supports models, saved views, dashboards, and color palettes"
             )
         resource_id = grn_components.gluid
+        # pulling a grn means we ignore the normal dataops-only filter
+        all = True
 
-    SUPPORTED_TYPES = ["dashboard", "saved_view", "model", "color_palette", "homepage_launchpad"]
+    SUPPORTED_TYPES = [
+        "dashboard",
+        "saved_view",
+        "model",
+        "color_palette",
+        "homepage_launchpad",
+    ]
     local_by_path = {
         k: v for k, v in local_resources(Path(".")).items() if v.type in SUPPORTED_TYPES
     }
     click.echo(f"🔎 Found {len(local_by_path)} Glean resources in working directory.")
 
     def get_grn(path: PurePosixPath, resource: Resource) -> GRNComponents:
         RESOURCE_TYPE_TO_ABBREV = {
@@ -468,22 +483,25 @@
     # they should be considered equal.
     local_by_grn = list(
         (get_grn(path, resource), path, resource)
         for (path, resource) in local_by_path.items()
     )
     local_grns = list(local_grn for (local_grn, _, _) in local_by_grn)
 
-    result = pull_resource(s, project_id, resource_type, resource_id)
+    result = pull_resource(s, project_id, resource_type, resource_id, dataops_only=(not all))
     if result.get("errors"):
         _echo_pull_errors_and_exit(result["errors"])
         return
 
     remote: list[Resource] = result["configs"]
+    if len(remote) == 0 and not all:
+        click.echo("No DataOps-managed resources were found. To pull all resources in the project, use `glean pull --all`.")
+        return
 
-    touched_files = [] # either created or modified
+    touched_files = []  # either created or modified
     num_updated = 0
     for resource in remote:
         assert resource.grn is not None
         with suppress(ValueError):
             index = local_grns.index(resource.grn)
             # we've matched the resource to a local file
             (_, path, local_resource) = local_by_grn[index]
```

### Comparing `glean-cli-0.7.2/src/glean/credentials.py` & `glean-cli-0.7.3/src/glean/credentials.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.2/src/glean/filesystem.py` & `glean-cli-0.7.3/src/glean/filesystem.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.2/src/glean/glean_api.py` & `glean-cli-0.7.3/src/glean/glean_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,31 +263,34 @@
 
 
 def pull_resource(
     s: Session,
     project_id: str,
     resource_type: Optional[str],
     resource_id: Optional[str],
+    dataops_only: Optional[bool],
 ) -> PullResourceResponse:
     """Pulls the DataOps config for the given resource, or all resources in the project if none is specified."""
     res = _graphql_query(
         s,
         """
-        query PullResource($projectId: String!, $resourceType: String, $resourceId: String) {
+        query PullResource($projectId: String!, $resourceType: String, $resourceId: String, $dataOpsOnly: Boolean) {
             pullResource(
                 projectId: $projectId,
                 resourceType: $resourceType,
-                resourceId: $resourceId
+                resourceId: $resourceId,
+                dataOpsOnly: $dataOpsOnly
             ) { configs, errors }
         }
         """,
         {
             "projectId": project_id,
             "resourceType": resource_type,
             "resourceId": resource_id,
+            "dataOpsOnly": dataops_only,
         },
     )["data"]["pullResource"]
     res["configs"] = [
         Resource.from_dict(json.loads(string)) for string in res["configs"]
     ]
     return res
```

### Comparing `glean-cli-0.7.2/src/glean/utils/grn.py` & `glean-cli-0.7.3/src/glean/utils/grn.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.2/src/glean/utils/resource.py` & `glean-cli-0.7.3/src/glean/utils/resource.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.2/src/glean/utils/validate_config.py` & `glean-cli-0.7.3/src/glean/utils/validate_config.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.2/src/glean_cli.egg-info/PKG-INFO` & `glean-cli-0.7.3/src/glean_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-cli
-Version: 0.7.2
+Version: 0.7.3
 Summary: Command-line tools for interacting with Glean
 Home-page: https://glean.io/
 Author: Dan Eisenberg
 Author-email: dse@glean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `glean-cli-0.7.2/src/glean_cli.egg-info/SOURCES.txt` & `glean-cli-0.7.3/src/glean_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.2/tests/test_credentials.py` & `glean-cli-0.7.3/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.2/tests/test_filesystem.py` & `glean-cli-0.7.3/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.7.2/tests/test_glean_api.py` & `glean-cli-0.7.3/tests/test_glean_api.py`

 * *Files identical despite different names*

