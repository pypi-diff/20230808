# Comparing `tmp/foursight-3.6.1.1b3.tar.gz` & `tmp/foursight-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight-3.6.1.1b3.tar", max compression
+gzip compressed data, was "foursight-3.6.2.tar", max compression
```

## Comparing `foursight-3.6.1.1b3.tar` & `foursight-3.6.2.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     1083 2022-09-07 10:59:14.705392 foursight-3.6.1.1b3/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-01-19 14:12:17.947754 foursight-3.6.1.1b3/chalicelib_fourfront/__init__.py
--rw-r--r--   0        0        0     1088 2023-07-16 15:38:27.409196 foursight-3.6.1.1b3/chalicelib_fourfront/app_utils.py
--rw-r--r--   0        0        0     5405 2023-01-19 14:12:17.952115 foursight-3.6.1.1b3/chalicelib_fourfront/check_schedules.py
--rw-r--r--   0        0        0    54860 2023-07-07 22:27:54.136755 foursight-3.6.1.1b3/chalicelib_fourfront/check_setup.json
--rw-r--r--   0        0        0      249 2023-01-19 14:12:17.956201 foursight-3.6.1.1b3/chalicelib_fourfront/checks/__init__.py
--rw-r--r--   0        0        0    62768 2023-07-07 22:27:54.137645 foursight-3.6.1.1b3/chalicelib_fourfront/checks/audit_checks.py
--rw-r--r--   0        0        0    37729 2023-07-27 22:59:26.969695 foursight-3.6.1.1b3/chalicelib_fourfront/checks/badge_checks.py
--rw-r--r--   0        0        0    11548 2023-01-19 14:12:17.965655 foursight-3.6.1.1b3/chalicelib_fourfront/checks/deployment_checks.py
--rw-r--r--   0        0        0     2939 2023-01-25 11:36:46.617974 foursight-3.6.1.1b3/chalicelib_fourfront/checks/ecs_checks.py
--rw-r--r--   0        0        0     3914 2023-01-19 14:12:17.970674 foursight-3.6.1.1b3/chalicelib_fourfront/checks/es_checks.py
--rw-r--r--   0        0        0    15663 2023-06-09 17:46:33.623749 foursight-3.6.1.1b3/chalicelib_fourfront/checks/header_checks.py
--rw-r--r--   0        0        0      262 2023-01-19 14:12:17.974848 foursight-3.6.1.1b3/chalicelib_fourfront/checks/helpers/confchecks.py
--rw-r--r--   0        0        0    44428 2023-01-19 14:12:17.975418 foursight-3.6.1.1b3/chalicelib_fourfront/checks/helpers/google_utils.py
--rw-r--r--   0        0        0    95229 2023-01-19 14:12:17.978748 foursight-3.6.1.1b3/chalicelib_fourfront/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0    17372 2023-01-19 14:12:17.979325 foursight-3.6.1.1b3/chalicelib_fourfront/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     3686 2023-01-19 14:12:17.979607 foursight-3.6.1.1b3/chalicelib_fourfront/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0    97361 2023-01-19 14:12:17.983575 foursight-3.6.1.1b3/chalicelib_fourfront/checks/higlass_checks.py
--rw-r--r--   0        0        0    32926 2023-01-19 14:12:17.989004 foursight-3.6.1.1b3/chalicelib_fourfront/checks/release_updates_checks.py
--rw-r--r--   0        0        0    45209 2023-04-27 02:48:56.047051 foursight-3.6.1.1b3/chalicelib_fourfront/checks/system_checks.py
--rw-r--r--   0        0        0   128320 2023-07-16 13:30:55.184666 foursight-3.6.1.1b3/chalicelib_fourfront/checks/wfr_checks.py
--rw-r--r--   0        0        0    43470 2023-01-19 14:12:18.009971 foursight-3.6.1.1b3/chalicelib_fourfront/checks/wfr_encode_checks.py
--rw-r--r--   0        0        0   137844 2023-07-16 15:38:27.410509 foursight-3.6.1.1b3/chalicelib_fourfront/checks/wrangler_checks.py
--rw-r--r--   0        0        0      621 2023-03-29 20:27:15.171432 foursight-3.6.1.1b3/chalicelib_fourfront/package.py
--rw-r--r--   0        0        0      240 2023-07-27 22:59:23.665948 foursight-3.6.1.1b3/chalicelib_fourfront/scripts/local_check_execution.py
--rw-r--r--   0        0        0      316 2023-03-29 19:16:47.518681 foursight-3.6.1.1b3/chalicelib_fourfront/vars.py
--rw-r--r--   0        0        0     1245 2023-07-28 04:00:27.647155 foursight-3.6.1.1b3/pyproject.toml
--rw-r--r--   0        0        0     1494 1970-01-01 00:00:00.000000 foursight-3.6.1.1b3/setup.py
--rw-r--r--   0        0        0     1132 1970-01-01 00:00:00.000000 foursight-3.6.1.1b3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2017-11-21 15:12:01.000000 foursight-3.6.2/LICENSE.txt
+-rw-r--r--   0        0        0        0 2022-11-16 16:53:13.403096 foursight-3.6.2/chalicelib_fourfront/__init__.py
+-rw-r--r--   0        0        0     1088 2023-07-19 18:36:43.842986 foursight-3.6.2/chalicelib_fourfront/app_utils.py
+-rw-r--r--   0        0        0     5405 2022-11-16 16:53:13.404868 foursight-3.6.2/chalicelib_fourfront/check_schedules.py
+-rw-r--r--   0        0        0    54860 2023-06-21 14:22:50.333640 foursight-3.6.2/chalicelib_fourfront/check_setup.json
+-rw-r--r--   0        0        0      249 2022-11-16 16:53:13.406545 foursight-3.6.2/chalicelib_fourfront/checks/__init__.py
+-rw-r--r--   0        0        0    62768 2023-06-21 14:22:50.335968 foursight-3.6.2/chalicelib_fourfront/checks/audit_checks.py
+-rw-r--r--   0        0        0    37729 2023-07-20 15:47:44.788397 foursight-3.6.2/chalicelib_fourfront/checks/badge_checks.py
+-rw-r--r--   0        0        0    11548 2023-01-19 17:19:39.272753 foursight-3.6.2/chalicelib_fourfront/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2939 2023-04-19 19:52:24.091358 foursight-3.6.2/chalicelib_fourfront/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3914 2023-01-19 17:19:39.273550 foursight-3.6.2/chalicelib_fourfront/checks/es_checks.py
+-rw-r--r--   0        0        0    15663 2023-06-09 22:12:58.101520 foursight-3.6.2/chalicelib_fourfront/checks/header_checks.py
+-rw-r--r--   0        0        0      262 2022-11-16 16:53:13.426279 foursight-3.6.2/chalicelib_fourfront/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0    44428 2022-11-16 16:53:13.427051 foursight-3.6.2/chalicelib_fourfront/checks/helpers/google_utils.py
+-rw-r--r--   0        0        0    95229 2023-01-19 17:19:30.850214 foursight-3.6.2/chalicelib_fourfront/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0    17372 2022-11-16 16:53:13.428402 foursight-3.6.2/chalicelib_fourfront/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     3686 2022-11-16 16:53:13.428930 foursight-3.6.2/chalicelib_fourfront/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0    97361 2023-01-19 17:19:39.276361 foursight-3.6.2/chalicelib_fourfront/checks/higlass_checks.py
+-rw-r--r--   0        0        0    32926 2023-01-19 17:19:39.279026 foursight-3.6.2/chalicelib_fourfront/checks/release_updates_checks.py
+-rw-r--r--   0        0        0    45209 2023-04-19 19:52:24.091978 foursight-3.6.2/chalicelib_fourfront/checks/system_checks.py
+-rw-r--r--   0        0        0   128352 2023-08-07 20:31:26.074887 foursight-3.6.2/chalicelib_fourfront/checks/wfr_checks.py
+-rw-r--r--   0        0        0    43470 2023-01-19 17:19:39.282546 foursight-3.6.2/chalicelib_fourfront/checks/wfr_encode_checks.py
+-rw-r--r--   0        0        0   137844 2023-07-19 18:36:43.844611 foursight-3.6.2/chalicelib_fourfront/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      621 2022-11-16 16:53:13.457648 foursight-3.6.2/chalicelib_fourfront/package.py
+-rw-r--r--   0        0        0      316 2022-11-16 16:53:13.457903 foursight-3.6.2/chalicelib_fourfront/vars.py
+-rw-r--r--   0        0        0     1283 2023-08-07 20:31:26.075830 foursight-3.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1535 1970-01-01 00:00:00.000000 foursight-3.6.2/setup.py
+-rw-r--r--   0        0        0     1076 1970-01-01 00:00:00.000000 foursight-3.6.2/PKG-INFO
```

### Comparing `foursight-3.6.1.1b3/LICENSE.txt` & `foursight-3.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/app_utils.py` & `foursight-3.6.2/chalicelib_fourfront/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/check_schedules.py` & `foursight-3.6.2/chalicelib_fourfront/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/check_setup.json` & `foursight-3.6.2/chalicelib_fourfront/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/checks/audit_checks.py` & `foursight-3.6.2/chalicelib_fourfront/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/checks/badge_checks.py` & `foursight-3.6.2/chalicelib_fourfront/checks/badge_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/checks/deployment_checks.py` & `foursight-3.6.2/chalicelib_fourfront/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/checks/ecs_checks.py` & `foursight-3.6.2/chalicelib_fourfront/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/checks/es_checks.py` & `foursight-3.6.2/chalicelib_fourfront/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/checks/header_checks.py` & `foursight-3.6.2/chalicelib_fourfront/checks/header_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/checks/helpers/google_utils.py` & `foursight-3.6.2/chalicelib_fourfront/checks/helpers/google_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/checks/helpers/wfr_utils.py` & `foursight-3.6.2/chalicelib_fourfront/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/checks/helpers/wfrset_utils.py` & `foursight-3.6.2/chalicelib_fourfront/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/checks/helpers/wrangler_utils.py` & `foursight-3.6.2/chalicelib_fourfront/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/checks/higlass_checks.py` & `foursight-3.6.2/chalicelib_fourfront/checks/higlass_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/checks/release_updates_checks.py` & `foursight-3.6.2/chalicelib_fourfront/checks/release_updates_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/checks/system_checks.py` & `foursight-3.6.2/chalicelib_fourfront/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/checks/wfr_checks.py` & `foursight-3.6.2/chalicelib_fourfront/checks/wfr_checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1813,21 +1813,21 @@
     if skip:
         return check
     # Get Fastq files from RNA-seq that are missing beta-actin counts
     files = ff_utils.search_metadata(
         '/search/?type=FileFastq&file_format.file_format=fastq&track_and_facet_info.experiment_type=RNA-seq'
         + '&experiments.biosample.biosource.organism.name!=No+value'
         + '&beta_actin_sense_count=No+value&beta_actin_antisense_count=No+value'
-        + '&status=pre-release&status=released&status=released to project',
+        + '&status=uploaded&status=pre-release&status=released&status=released to project',
         key=my_auth)
     # Get RNA-seq sets that are tagged with skip_processing
     expsets_to_skip = ff_utils.search_metadata(
         '/search/?type=ExperimentSetReplicate&experiments_in_set.experiment_type.display_title=RNA-seq'
         + '&experiments_in_set.biosample.biosource.organism.name!=No+value'
-        + '&status=pre-release&status=released&status=released to project'
+        + '&status=uploaded&status=pre-release&status=released&status=released to project'
         + '&tags=skip_processing&field=accession',
         key=my_auth)
     expsets_acc_to_skip = [expset['accession'] for expset in expsets_to_skip]
 
     targets = []
     for a_file in files:
         replicate_expsets = [es['accession'] for es in a_file['experiments'][0]['experiment_sets'] if es['experimentset_type'] == 'replicate']
```

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/checks/wfr_encode_checks.py` & `foursight-3.6.2/chalicelib_fourfront/checks/wfr_encode_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/checks/wrangler_checks.py` & `foursight-3.6.2/chalicelib_fourfront/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/chalicelib_fourfront/package.py` & `foursight-3.6.2/chalicelib_fourfront/package.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.1.1b3/pyproject.toml` & `foursight-3.6.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 [tool.poetry]
 name = "foursight"
-version = "3.6.1.1b3"  # TODO: To become 3.6.2
+version = "3.6.2"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_fourfront" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.10"
+#dcicutils = "^7.5.1"
+dcicutils = "7.6.0.1b4"
 click = "^7.1.2"
-dcicutils = "^7.5.2"
+PyJWT = "^2.5.0"
+Jinja2 = "2.10.1"
+MarkupSafe = "1.1.1"
+google-api-python-client = "^1.7.4"
+geocoder = "1.38.1"
 elasticsearch = "^7.13.4"
 elasticsearch-dsl = "^7.0.0"
+gitpython = "^3.1.2"
+pytz = "^2020.1"
+tibanna_ff = ">=0.22.5"
 ## adding foursight-core
 # use below for deployment
+foursight-core = "4.4.0"
 # use below for tests but not for deployment
 # foursight-core = { git = "https://github.com/4dn-dcic/foursight-core.git", branch="master" }
-foursight-core = "4.4.0.1b2"
-geocoder = "1.38.1"
-gitpython = "^3.1.2"
-google-api-python-client = "^1.7.4"
-google-auth = "^2.22.0"
+pytest = "5.1.2"
 gspread = ">=3.6.0"
-Jinja2 = "2.10.1"
-MarkupSafe = "1.1.1"
 oauth2client = ">=4.1.3"
 pandas = ">=1.1.4"
-PyJWT = "^2.5.0"
-pytest = "5.1.2"
-tibanna_ff = ">=0.22.5"
-pytz = "^2020.1"
 
 [tool.poetry.dev-dependencies]
 chalice = "^1.26.0"
-flaky = "3.6.1"
 pytest-cov = "2.7.1"
+flaky = "3.6.1"
 
 [tool.poetry.scripts]
-local-check-execution = "chalicelib_fourfront.scripts.local_check_execution:main"
+encrypt-accounts-file = "foursight_core.scripts.encrypt_accounts_file:main"
+decrypt-accounts-file = "foursight_core.scripts.decrypt_accounts_file:main"
 publish-to-pypi = "dcicutils.scripts.publish_to_pypi:main"
 
 [build-system]
-build-backend = "poetry.masonry.api"
 requires = ["poetry>=0.12"]
+build-backend = "poetry.masonry.api"
```

### Comparing `foursight-3.6.1.1b3/PKG-INFO` & `foursight-3.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: foursight
-Version: 3.6.1.1b3
+Version: 3.6.2
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (==2.10.1)
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
-Requires-Dist: dcicutils (>=7.5.2,<8.0.0)
+Requires-Dist: dcicutils (==7.6.0.1b4)
 Requires-Dist: elasticsearch (>=7.13.4,<8.0.0)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
-Requires-Dist: foursight-core (==4.4.0.1b2)
+Requires-Dist: foursight-core (==4.4.0)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.7.4,<2.0.0)
-Requires-Dist: google-auth (>=2.22.0,<3.0.0)
 Requires-Dist: gspread (>=3.6.0)
 Requires-Dist: oauth2client (>=4.1.3)
 Requires-Dist: pandas (>=1.1.4)
 Requires-Dist: pytest (==5.1.2)
 Requires-Dist: pytz (>=2020.1,<2021.0)
 Requires-Dist: tibanna_ff (>=0.22.5)
```

