# Comparing `tmp/pipestat-0.4.1.tar.gz` & `tmp/pipestat-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipestat-0.4.1.tar", last modified: Wed Jul 26 13:49:14 2023, max compression
+gzip compressed data, was "pipestat-0.5.0.tar", last modified: Tue Aug  8 16:31:37 2023, max compression
```

## Comparing `pipestat-0.4.1.tar` & `pipestat-0.5.0.tar`

### file list

```diff
@@ -1,39 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:14.613767 pipestat-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-26 13:49:05.000000 pipestat-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-26 13:49:05.000000 pipestat-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-26 13:49:14.613767 pipestat-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-26 13:49:05.000000 pipestat-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:14.613767 pipestat-0.4.1/pipestat/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:14.613767 pipestat-0.4.1/pipestat/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/backends/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    26413 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/backends/dbbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/backends/filebackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/parsed_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    21733 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/pipestat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:14.613767 pipestat-0.4.1/pipestat/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/schemas/pipestat_config_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/schemas/status_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/schemas/status_table_schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:14.613767 pipestat-0.4.1/pipestat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-26 13:49:14.000000 pipestat-0.4.1/pipestat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-26 13:49:14.000000 pipestat-0.4.1/pipestat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:49:14.000000 pipestat-0.4.1/pipestat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-26 13:49:14.000000 pipestat-0.4.1/pipestat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-26 13:49:14.000000 pipestat-0.4.1/pipestat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 13:49:14.000000 pipestat-0.4.1/pipestat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 13:49:05.000000 pipestat-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:14.613767 pipestat-0.4.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-26 13:49:05.000000 pipestat-0.4.1/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 13:49:05.000000 pipestat-0.4.1/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-26 13:49:05.000000 pipestat-0.4.1/requirements/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 13:49:05.000000 pipestat-0.4.1/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 13:49:14.613767 pipestat-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-26 13:49:05.000000 pipestat-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:31:37.752212 pipestat-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-08 16:31:27.000000 pipestat-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-08 16:31:27.000000 pipestat-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-08 16:31:37.752212 pipestat-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-08-08 16:31:27.000000 pipestat-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:31:37.748212 pipestat-0.5.0/pipestat/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:31:37.748212 pipestat-0.5.0/pipestat/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/backends/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27849 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/backends/dbbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20531 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/backends/filebackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37348 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/html_reports_pipestat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:31:37.748212 pipestat-0.5.0/pipestat/jinja_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/jinja_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/jinja_templates/footer_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/jinja_templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/jinja_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/jinja_templates/logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/jinja_templates/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/jinja_templates/navbar_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/jinja_templates/navbar_list_parent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/jinja_templates/object.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/jinja_templates/project_object.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/jinja_templates/sample.html
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/jinja_templates/status.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/jinja_templates/status_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/jinja_templates/status_table_no_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/parsed_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22308 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/pipestat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:31:37.752212 pipestat-0.5.0/pipestat/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/schemas/pipestat_config_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/schemas/status_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-08 16:31:27.000000 pipestat-0.5.0/pipestat/schemas/status_table_schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:31:37.748212 pipestat-0.5.0/pipestat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-08 16:31:37.000000 pipestat-0.5.0/pipestat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-08 16:31:37.000000 pipestat-0.5.0/pipestat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 16:31:37.000000 pipestat-0.5.0/pipestat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 16:31:37.000000 pipestat-0.5.0/pipestat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-08 16:31:37.000000 pipestat-0.5.0/pipestat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 16:31:37.000000 pipestat-0.5.0/pipestat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-08 16:31:27.000000 pipestat-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:31:37.752212 pipestat-0.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-08 16:31:27.000000 pipestat-0.5.0/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-08 16:31:27.000000 pipestat-0.5.0/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-08 16:31:27.000000 pipestat-0.5.0/requirements/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-08 16:31:27.000000 pipestat-0.5.0/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 16:31:37.752212 pipestat-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-08-08 16:31:27.000000 pipestat-0.5.0/setup.py
```

### Comparing `pipestat-0.4.1/LICENSE` & `pipestat-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.1/PKG-INFO` & `pipestat-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipestat
-Version: 0.4.1
+Version: 0.5.0
 Summary: A pipeline results reporter
 Home-page: https://github.com/pepkit/pipestat
 Author: Michal Stolarczyk, Nathan Sheffield
 License: BSD2
 Keywords: project,metadata,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pipestat-0.4.1/README.md` & `pipestat-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.1/pipestat/argparser.py` & `pipestat-0.5.0/pipestat/argparser.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 
 REPORT_CMD = "report"
 INSPECT_CMD = "inspect"
 REMOVE_CMD = "remove"
 RETRIEVE_CMD = "retrieve"
 STATUS_CMD = "status"
 INIT_CMD = "init"
+SUMMARIZE_CMD = "summarize"
 SUBPARSER_MESSAGES = {
     REPORT_CMD: "Report a result.",
     INSPECT_CMD: "Inspect a database.",
     REMOVE_CMD: "Remove a result.",
     RETRIEVE_CMD: "Retrieve a result.",
     STATUS_CMD: "Manage pipeline status.",
     INIT_CMD: "Initialize generic config file",
+    SUMMARIZE_CMD: "Generates HTML Report",
 }
 
 STATUS_GET_CMD = "get"
 STATUS_SET_CMD = "set"
 STATUS_SUBPARSER_MESSAGES = {
     STATUS_SET_CMD: "Set status.",
     STATUS_GET_CMD: "Get status.",
@@ -251,8 +253,34 @@
     )
 
     # inspect
     sps[INSPECT_CMD].add_argument(
         "-d", "--data", action="store_true", help="Whether to display the data"
     )
 
+    # Summarize
+    for cmd in [SUMMARIZE_CMD]:
+        sps[cmd].add_argument(
+            "-f",
+            "--results-file",
+            type=str,
+            metavar="F",
+            help=f"Path to the YAML file where the results will be stored. "
+            f"This file will be used as {PKG_NAME} backend and to restore"
+            f" the reported results across sessions",
+        )
+        sps[cmd].add_argument(
+            "-c",
+            "--config",
+            type=str,
+            metavar="C",
+            help=f"Path to the YAML configuration file. {_env_txt('config')}",
+        )
+        sps[cmd].add_argument(
+            "-s",
+            "--schema",
+            type=str,
+            metavar="S",
+            help=f"Path to the schema that defines the results that can be reported. {_env_txt('schema')}",
+        )
+
     return parser
```

### Comparing `pipestat-0.4.1/pipestat/backends/abstract.py` & `pipestat-0.5.0/pipestat/backends/abstract.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,14 +83,21 @@
     def count_records(
         self,
         pipeline_type: Optional[str] = None,
     ):
         _LOGGER.warning("Not implemented yet for this backend")
         pass
 
+    def get_samples(
+        self,
+        pipeline_type: Optional[str] = None,
+    ):
+        _LOGGER.warning("Not implemented yet for this backend")
+        pass
+
     def get_status(self, sample_name: str, pipeline_type: Optional[str] = None) -> Optional[str]:
         _LOGGER.warning("Not implemented yet for this backend")
 
     def clear_status(
         self, sample_name: str = None, flag_names: List[str] = None
     ) -> List[Union[str, None]]:
         _LOGGER.warning("Not implemented yet for this backend")
@@ -133,7 +140,11 @@
     def remove_record(
         self,
         sample_name: Optional[str] = None,
         result_identifier: Optional[str] = None,
         pipeline_type: Optional[str] = None,
     ) -> bool:
         _LOGGER.warning("Not implemented yet for this backend")
+
+    def summarize(self) -> None:
+        _LOGGER.warning("Not implemented yet for this backend")
+        pass
```

### Comparing `pipestat-0.4.1/pipestat/backends/dbbackend.py` & `pipestat-0.5.0/pipestat/backends/dbbackend.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,50 @@
             for mod in models:
                 stmt = sql_select(mod).where(mod.sample_name == rid)
                 record = s.exec(stmt).first()
 
                 if record:
                     return record
 
+    def get_samples(
+        self,
+        pipeline_type: Optional[str] = None,
+    ) -> Optional[list]:
+        """Returns list of sample names and pipeline type as a list of tuples that have been reported, regardless of sample or project level"""
+        all_samples_list = []
+
+        if pipeline_type is not None:
+            table_name = self.get_table_name(pipeline_type)
+            mod = self.get_model(table_name=table_name, strict=True)
+            with self.session as s:
+                sample_list = []
+                stmt = sql_select(mod)
+                records = s.exec(stmt).all()
+                for i in records:
+                    pair = (i.sample_name, pipeline_type)
+                    sample_list.append(pair)
+
+            return sample_list
+        else:
+            pipelines = ["sample", "project"]
+            for i in pipelines:
+                pipeline_type = i
+                table_name = self.get_table_name(pipeline_type)
+                mod = self.get_model(table_name=table_name, strict=True)
+                with self.session as s:
+                    sample_list = []
+                    stmt = sql_select(mod)
+                    records = s.exec(stmt).all()
+                    for i in records:
+                        pair = (i.sample_name, pipeline_type)
+                        sample_list.append(pair)
+
+                all_samples_list += sample_list
+            return all_samples_list
+
     def get_status(self, sample_name: str, pipeline_type: Optional[str] = None) -> Optional[str]:
         """
         Get pipeline status
 
         :param str sample_name: record identifier to set the
             pipeline status for
         :param str pipeline_type: whether status is being set for a project-level pipeline, or sample-level
```

### Comparing `pipestat-0.4.1/pipestat/backends/filebackend.py` & `pipestat-0.5.0/pipestat/backends/filebackend.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,14 +140,37 @@
         elif len(file_list) == 1:
             return file_list[0]
         else:
             _LOGGER.debug("No flag files found")
             return None
         pass
 
+    def get_samples(
+        self,
+        pipeline_type: Optional[str] = None,
+    ) -> Optional[list]:
+        """Returns list of sample names and pipeline type as a list of tuples that have been reported, regardless of sample or project level"""
+        all_samples_list = []
+
+        if pipeline_type is not None:
+            for k in list(self._data.data[self.pipeline_name][pipeline_type].keys()):
+                pair = (k, pipeline_type)
+                all_samples_list.append(pair)
+            return all_samples_list
+
+        else:
+            keys = self._data.data[self.pipeline_name].keys()
+        for k in keys:
+            sample_list = []
+            for i in list(self._data.data[self.pipeline_name][k].keys()):
+                pair = (i, k)
+                sample_list.append(pair)
+            all_samples_list += sample_list
+        return all_samples_list
+
     def get_status(self, sample_name: str, pipeline_type: Optional[str] = None) -> Optional[str]:
         """
         Get the current pipeline status
 
         :param str sample_name: record identifier to set the
             pipeline status for
         :param str pipeline_type: "sample" or "project"
@@ -438,14 +461,31 @@
         with open(flag_path, "w") as f:
             f.write(status_identifier)
         remove_lock(flag_path)
 
         if prev_status:
             _LOGGER.debug(f"Changed status from '{prev_status}' to '{status_identifier}'")
 
+    def summarize(self) -> None:
+        """
+        summarize all reported results by building html report
+        """
+        _LOGGER.debug("Make HTML report here")
+        print("DEBUG SUMMARIZE")
+        self._htmlreportbuilder()
+
+    def _htmlreportbuilder(self):
+        """
+        build html report based on all reported results
+        """
+
+        # build new folder for the report
+        self.reports_dir = os.path.join(self.results_file_path, "reports")
+        _LOGGER.debug(f"Reports dir: {self.reports_dir}")
+
     def _init_results_file(self) -> None:
         """
         Initialize YAML results file if it does not exist.
         Read the data stored in the existing file into the memory otherwise.
 
         :return bool: whether the file has been created
         """
```

### Comparing `pipestat-0.4.1/pipestat/cli.py` & `pipestat-0.5.0/pipestat/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     INSPECT_CMD,
     REMOVE_CMD,
     RETRIEVE_CMD,
     STATUS_CMD,
     STATUS_GET_CMD,
     STATUS_SET_CMD,
     INIT_CMD,
+    SUMMARIZE_CMD,
 )
 from .const import *
 from .exceptions import SchemaNotFoundError, PipestatStartupError
 from .pipestat import PipestatManager
 from .helpers import init_generic_config
 
 _LOGGER = getLogger(PKG_NAME)
@@ -42,14 +43,26 @@
         parser.error("the following arguments are required: -s/--schema")
     if not args.config and not args.results_file:
         msg = (
             "Either a config file or a results file must be provided. Either must be supplied to the object "
             "constructor or via environment variable. \nPlease see: http://pipestat.databio.org/en/dev/cli/"
         )
         raise PipestatStartupError(msg)
+    if args.command == SUMMARIZE_CMD:
+        psm = PipestatManager(
+            schema_path=args.schema,
+            results_file_path=args.results_file,
+            config_file=args.config,
+        )
+        results_path = args.config or args.results_file
+        html_report_path = psm.summarize()
+        _LOGGER.info(f"\nGenerating HTML Report from {results_path} at: {html_report_path}\n")
+
+        sys.exit(0)
+
     psm = PipestatManager(
         schema_path=args.schema,
         results_file_path=args.results_file,
         config_file=args.config,
         database_only=args.database_only,
         flag_file_dir=args.flag_dir,
     )
@@ -101,8 +114,9 @@
         if args.subcommand == STATUS_GET_CMD:
             print(psm.get_status(sample_name=args.sample_name))
         if args.subcommand == STATUS_SET_CMD:
             psm.set_status(
                 status_identifier=args.status_identifier,
                 sample_name=args.sample_name,
             )
+
     sys.exit(0)
```

### Comparing `pipestat-0.4.1/pipestat/exceptions.py` & `pipestat-0.5.0/pipestat/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.1/pipestat/helpers.py` & `pipestat-0.5.0/pipestat/helpers.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.1/pipestat/parsed_schema.py` & `pipestat-0.5.0/pipestat/parsed_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import copy
 import logging
 from pathlib import Path
 from typing import *
 from pydantic import create_model
 
 # from sqlalchemy.dialects.postgresql import ARRAY
-from sqlalchemy import Column
+from sqlalchemy import Column, null
 from sqlalchemy.dialects.postgresql import JSONB
 from sqlmodel import Field, SQLModel
 from .const import *
 from .exceptions import SchemaError
 from .helpers import read_yaml_data
 
 
@@ -87,17 +87,19 @@
         if not self._sample_level_data and not self._project_level_data:
             raise SchemaError("Neither sample-level nor project-level data items are declared.")
 
         # Parse custom status declaration if present.
         self._status_data = _safe_pop_one_mapping(key="status", data=data, info_name="status")
 
         if data:
-            raise SchemaError(
-                f"Extra top-level key(s) in given schema data: {', '.join(data.keys())}"
+            _LOGGER.info(
+                "Top-Level arguments found in output schema. They will be assigned to project-level."
             )
+            extra_project_data = _recursively_replace_custom_types(data)
+            self._project_level_data.update(extra_project_data)
 
         # Check that no reserved keywords were used as data items.
         resv_kwds = {"id", SAMPLE_NAME}
         reserved_keywords_used = set()
         for data in [self.project_level_data, self.sample_level_data, self.status_data]:
             reserved_keywords_used |= set(data.keys()) & resv_kwds
         if reserved_keywords_used:
@@ -108,14 +110,31 @@
         # Check that no data item name overlap exists between project- and sample-level data.
         project_sample_overlap = set(self.project_level_data) & set(self.sample_level_data)
         if project_sample_overlap:
             raise SchemaError(
                 f"Overlap between project- and sample-level keys: {', '.join(project_sample_overlap)}"
             )
 
+    def __str__(self):
+        """
+        Generate string representation of the object
+
+        :return str: string representation of the object
+        """
+        res = f"{self.__class__.__name__} ({self._pipeline_name})"
+        if self._project_level_data is not None:
+            res += f"\n Project Level Data:"
+            for k, v in self._project_level_data.items():
+                res += f"\n -  {k} : {v}"
+        if self._sample_level_data is not None:
+            res += f"\n Sample Level Data:"
+            for k, v in self._sample_level_data.items():
+                res += f"\n -  {k} : {v}"
+        return res
+
     @property
     def pipeline_name(self):
         return self._pipeline_name
 
     @property
     def project_level_data(self):
         return copy.deepcopy(self._project_level_data)
@@ -154,15 +173,15 @@
                 else:
                     data_type = str
             else:
                 data_type = self._get_data_type(typename)
             if data_type == CLASSES_BY_TYPE["object"] or data_type == CLASSES_BY_TYPE["array"]:
                 defs[name] = (
                     data_type,
-                    Field(sa_column=Column(JSONB), default={}),
+                    Field(sa_column=Column(JSONB), default=null()),
                 )
             else:
                 defs[name] = (
                     # Optional[subdata[SCHEMA_TYPE_KEY]],
                     # subdata[SCHEMA_TYPE_KEY],
                     # Optional[str],
                     # CLASSES_BY_TYPE[subdata[SCHEMA_TYPE_KEY]],
@@ -183,14 +202,15 @@
 
     def build_project_model(self):
         """Create the models associated with project-level data."""
         data = self.project_level_data
         field_defs = self._make_field_definitions(data, require_type=True)
         field_defs = self._add_status_field(field_defs)
         field_defs = self._add_sample_name_field(field_defs)
+        field_defs = self._add_project_name_field(field_defs)
         field_defs = self._add_id_field(field_defs)
         if not field_defs:
             return None
         return _create_model(self.project_table_name, **field_defs)
 
     def build_sample_model(self):
         # TODO: include the ability to process the custom types.
```

### Comparing `pipestat-0.4.1/pipestat/pipestat.py` & `pipestat-0.5.0/pipestat/pipestat.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from jsonschema import validate
 
 from yacman import YAMLConfigManager, select_config
 
 from .helpers import *
 from .parsed_schema import ParsedSchema
 
+from .html_reports_pipestat import HTMLReportBuilder, fetch_pipeline_results
+
+
 _LOGGER = getLogger(PKG_NAME)
 
 
 def require_backend(func):
     """Decorator to ensure a backend exists for functions that require one"""
 
     def inner(self, *args, **kwargs):
@@ -434,14 +437,30 @@
         :param str sample_name: record identifier to set the
             pipeline status for
         :param str pipeline_type: "sample" or "project"
         """
         pipeline_type = pipeline_type or self[PIPELINE_TYPE]
         self.backend.set_status(status_identifier, sample_name, pipeline_type)
 
+    @require_backend
+    def summarize(
+        self,
+        amendment: Optional[str] = None,
+    ) -> None:
+        """
+        Builds a browsable html report for reported results.
+        :param Iterable[str] amendment: name indicating amendment to use, optional
+        :return str: report_path
+
+        """
+
+        html_report_builder = HTMLReportBuilder(prj=self)
+        report_path = html_report_builder(pipeline_name=self.pipeline_name, amendment=amendment)
+        return report_path
+
     def _get_attr(self, attr: str) -> Any:
         """
         Safely get the name of the selected attribute of this object
 
         :param str attr: attr to select
         :return:
         """
```

### Comparing `pipestat-0.4.1/pipestat/schemas/pipestat_config_schema.yaml` & `pipestat-0.5.0/pipestat/schemas/pipestat_config_schema.yaml`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.1/pipestat.egg-info/PKG-INFO` & `pipestat-0.5.0/pipestat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipestat
-Version: 0.4.1
+Version: 0.5.0
 Summary: A pipeline results reporter
 Home-page: https://github.com/pepkit/pipestat
 Author: Michal Stolarczyk, Nathan Sheffield
 License: BSD2
 Keywords: project,metadata,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pipestat-0.4.1/setup.py` & `pipestat-0.5.0/setup.py`

 * *Files identical despite different names*

