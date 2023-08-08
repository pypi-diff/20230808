# Comparing `tmp/esd_services_api_client-0.8.0.tar.gz` & `tmp/esd_services_api_client-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esd_services_api_client-0.8.0.tar", max compression
+gzip compressed data, was "esd_services_api_client-0.8.1.tar", max compression
```

## Comparing `esd_services_api_client-0.8.0.tar` & `esd_services_api_client-0.8.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    10693 2023-06-20 13:22:24.363952 esd_services_api_client-0.8.0/LICENSE
--rw-r--r--   0        0        0      111 2023-06-20 13:22:24.363952 esd_services_api_client-0.8.0/README.md
--rw-r--r--   0        0        0      598 2023-06-20 13:22:24.363952 esd_services_api_client-0.8.0/esd_services_api_client/__init__.py
--rw-r--r--   0        0        0       22 2023-06-20 13:22:39.136227 esd_services_api_client-0.8.0/esd_services_api_client/_version.py
--rw-r--r--   0        0        0      743 2023-06-20 13:22:24.363952 esd_services_api_client-0.8.0/esd_services_api_client/beast/__init__.py
--rw-r--r--   0        0        0     2666 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/beast/_auth.py
--rw-r--r--   0        0        0    10369 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/beast/_connector.py
--rw-r--r--   0        0        0     9442 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/beast/_models.py
--rw-r--r--   0        0        0     2221 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/boxer/README.md
--rw-r--r--   0        0        0      780 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/boxer/__init__.py
--rw-r--r--   0        0        0     5214 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/boxer/_auth.py
--rw-r--r--   0        0        0      976 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/boxer/_base.py
--rw-r--r--   0        0        0     8272 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/boxer/_connector.py
--rw-r--r--   0        0        0     1736 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/boxer/_helpers.py
--rw-r--r--   0        0        0     3105 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/boxer/_models.py
--rw-r--r--   0        0        0      598 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/common/__init__.py
--rw-r--r--   0        0        0      787 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/crystal/__init__.py
--rw-r--r--   0        0        0      832 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/crystal/_api_versions.py
--rw-r--r--   0        0        0    12015 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/crystal/_connector.py
--rw-r--r--   0        0        0     4025 2023-06-20 13:22:24.367952 esd_services_api_client-0.8.0/esd_services_api_client/crystal/_models.py
--rw-r--r--   0        0        0      949 2023-06-20 13:22:39.136227 esd_services_api_client-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 esd_services_api_client-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    10693 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/LICENSE
+-rw-r--r--   0        0        0      111 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/README.md
+-rw-r--r--   0        0        0      598 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-08 08:56:11.740412 esd_services_api_client-0.8.1/esd_services_api_client/_version.py
+-rw-r--r--   0        0        0      743 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/beast/__init__.py
+-rw-r--r--   0        0        0     2666 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/beast/_auth.py
+-rw-r--r--   0        0        0    10505 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/beast/_connector.py
+-rw-r--r--   0        0        0     9438 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/beast/_models.py
+-rw-r--r--   0        0        0     2221 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/boxer/README.md
+-rw-r--r--   0        0        0      780 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/boxer/__init__.py
+-rw-r--r--   0        0        0     5214 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/boxer/_auth.py
+-rw-r--r--   0        0        0      976 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/boxer/_base.py
+-rw-r--r--   0        0        0     8272 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/boxer/_connector.py
+-rw-r--r--   0        0        0     1736 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/boxer/_helpers.py
+-rw-r--r--   0        0        0     3105 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/boxer/_models.py
+-rw-r--r--   0        0        0      598 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/common/__init__.py
+-rw-r--r--   0        0        0      787 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/crystal/__init__.py
+-rw-r--r--   0        0        0      832 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/crystal/_api_versions.py
+-rw-r--r--   0        0        0    12015 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/crystal/_connector.py
+-rw-r--r--   0        0        0     4025 2023-08-08 08:55:55.136190 esd_services_api_client-0.8.1/esd_services_api_client/crystal/_models.py
+-rw-r--r--   0        0        0      949 2023-08-08 08:56:11.740412 esd_services_api_client-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 esd_services_api_client-0.8.1/PKG-INFO
```

### Comparing `esd_services_api_client-0.8.0/LICENSE` & `esd_services_api_client-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/__init__.py` & `esd_services_api_client-0.8.1/esd_services_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/beast/__init__.py` & `esd_services_api_client-0.8.1/esd_services_api_client/beast/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/beast/_auth.py` & `esd_services_api_client-0.8.1/esd_services_api_client/beast/_auth.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/beast/_connector.py` & `esd_services_api_client-0.8.1/esd_services_api_client/beast/_connector.py`

 * *Files 10% similar despite different names*

```diff
@@ -181,14 +181,15 @@
                 flexible_driver=job_params.flexible_driver,
                 max_runtime_hours=job_params.max_runtime_hours,
                 additional_driver_node_tolerations=job_params.additional_driver_node_tolerations,
                 execution_group=job_params.execution_group,
                 debug_mode=job_params.debug_mode,
                 expected_parallelism=job_params.expected_parallelism,
                 submission_mode=job_params.submission_mode,
+                extended_code_mount=job_params.extended_code_mount,
             )
 
             (request_id, request_lifecycle) = self._submit(submit_request)
 
         while (
             request_lifecycle not in self.success_stages
             and request_lifecycle not in self.failed_stages
@@ -267,12 +268,13 @@
                 flexible_driver=job_params.flexible_driver,
                 max_runtime_hours=job_params.max_runtime_hours,
                 additional_driver_node_tolerations=job_params.additional_driver_node_tolerations,
                 execution_group=job_params.execution_group,
                 debug_mode=job_params.debug_mode,
                 expected_parallelism=job_params.expected_parallelism,
                 submission_mode=job_params.submission_mode,
+                extended_code_mount=job_params.extended_code_mount,
             )
 
             request_id, _ = self._submit(submit_request)
 
         return request_id
```

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/beast/_models.py` & `esd_services_api_client-0.8.1/esd_services_api_client/beast/_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,36 +92,31 @@
     """
     Job size hints for Beast.
 
     TINY - jobs running DDL or hive imports or any tiny workload. Should receive minimum allowed resources (1 core, 1g ram per executor)
     SMALL - small workloads, one or 30% pod cores, 30% pod memory per executor
     MEDIUM - medium workloads, one or 30% pod cores, 50% pod memory per executor
     LARGE - large workloads, one or 30% pod cores, all available executor memory
-    XLARGE - extra large workload, two or 60% pod cores, all available executor memory
-    XXLARGE - x-extra large workloads, all available cores, all available memory
     """
 
     TINY = "TINY"
     SMALL = "SMALL"
     MEDIUM = "MEDIUM"
     LARGE = "LARGE"
-    XLARGE = "XLARGE"
-    XXLARGE = "XXLARGE"
 
 
 class SubmissionMode(Enum):
     """
     Submission modes supported by Beast.
 
     SWARM - submit a job to a shared cluster.
     K8S - submit a job directly to k8s.
     STREAM - submit a job directly to a shared cluster bypassing application limit constraints.
     """
 
-    SWARM = "SWARM"
     K8S = "K8S"
     STREAM = "STREAM"
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass
 class JobRequest(DataClassJsonMixin):
@@ -148,14 +143,15 @@
     debug_mode: Optional[RequestDebugMode]
     expected_parallelism: Optional[int]
     submission_mode: Optional[SubmissionMode] = field(
         metadata=config(
             encoder=lambda v: v.value if v else None, decoder=SubmissionMode
         )
     )
+    extended_code_mount: Optional[bool]
 
 
 class ArgumentValue:
     """
     Wrapper around job argument value. Supports fernet encryption.
     """
 
@@ -299,7 +295,13 @@
     )
     additional_driver_node_tolerations: Optional[Dict[str, str]] = field(
         metadata={
             "description": "Additional taints allowed for application driver nodes."
         },
         default=None,
     )
+    extended_code_mount: Optional[bool] = field(
+        metadata={
+            "description": "Whether extended code mounting config should be used."
+        },
+        default=None,
+    )
```

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/boxer/README.md` & `esd_services_api_client-0.8.1/esd_services_api_client/boxer/README.md`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/boxer/__init__.py` & `esd_services_api_client-0.8.1/esd_services_api_client/boxer/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/boxer/_auth.py` & `esd_services_api_client-0.8.1/esd_services_api_client/boxer/_auth.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/boxer/_base.py` & `esd_services_api_client-0.8.1/esd_services_api_client/boxer/_base.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/boxer/_connector.py` & `esd_services_api_client-0.8.1/esd_services_api_client/boxer/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/boxer/_helpers.py` & `esd_services_api_client-0.8.1/esd_services_api_client/boxer/_helpers.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/boxer/_models.py` & `esd_services_api_client-0.8.1/esd_services_api_client/boxer/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/common/__init__.py` & `esd_services_api_client-0.8.1/esd_services_api_client/common/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/crystal/__init__.py` & `esd_services_api_client-0.8.1/esd_services_api_client/crystal/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/crystal/_api_versions.py` & `esd_services_api_client-0.8.1/esd_services_api_client/crystal/_api_versions.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/crystal/_connector.py` & `esd_services_api_client-0.8.1/esd_services_api_client/crystal/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.8.0/esd_services_api_client/crystal/_models.py` & `esd_services_api_client-0.8.1/esd_services_api_client/crystal/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.8.0/pyproject.toml` & `esd_services_api_client-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esd-services-api-client"
-version = "0.8.0"
+version = "0.8.1"
 description = "Python clients for ESD services"
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>', 'VISA <visa@ecco.com>']
 readme = "README.md"
 license = 'Apache 2.0'
 repository = 'https://github.com/SneaksAndData/esd-services-api-client'
```

### Comparing `esd_services_api_client-0.8.0/PKG-INFO` & `esd_services_api_client-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esd-services-api-client
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python clients for ESD services
 Home-page: https://github.com/SneaksAndData/esd-services-api-client
 License: Apache 2.0
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
```

