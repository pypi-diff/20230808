# Comparing `tmp/vital-1.4.4.tar.gz` & `tmp/vital-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-1.4.4.tar", max compression
+gzip compressed data, was "vital-1.4.6.tar", max compression
```

## Comparing `vital-1.4.4.tar` & `vital-1.4.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      388 2023-08-03 18:40:14.650615 vital-1.4.4/README.md
--rw-r--r--   0        0        0     1123 2023-08-03 18:40:14.650615 vital-1.4.4/pyproject.toml
--rw-r--r--   0        0        0      107 2023-08-03 18:40:14.650615 vital-1.4.4/vital/__init__.py
--rw-r--r--   0        0        0      702 2023-08-03 18:40:14.650615 vital-1.4.4/vital/api/__init__.py
--rw-r--r--   0        0        0     1531 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/activity.py
--rw-r--r--   0        0        0      142 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/api.py
--rw-r--r--   0        0        0     2904 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/athome_phlebotomy.py
--rw-r--r--   0        0        0     1515 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/body.py
--rw-r--r--   0        0        0      598 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/devices.py
--rw-r--r--   0        0        0     3870 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/labtests.py
--rw-r--r--   0        0        0     3093 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/link.py
--rw-r--r--   0        0        0      823 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/meals.py
--rw-r--r--   0        0        0      820 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/profile.py
--rw-r--r--   0        0        0        0 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/schema/__init__.py
--rw-r--r--   0        0        0     1719 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/schema/athome_phlebotomy.py
--rw-r--r--   0        0        0     2259 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/sleep.py
--rw-r--r--   0        0        0     2287 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/user.py
--rw-r--r--   0        0        0     3866 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/vitals.py
--rw-r--r--   0        0        0      632 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/webhooks.py
--rw-r--r--   0        0        0     1318 2023-08-03 18:40:14.654615 vital-1.4.4/vital/api/workouts.py
--rw-r--r--   0        0        0     5888 2023-08-03 18:40:14.654615 vital-1.4.4/vital/client.py
--rw-r--r--   0        0        0     3118 2023-08-03 18:40:14.654615 vital-1.4.4/vital/errors.py
--rw-r--r--   0        0        0        0 2023-08-03 18:40:14.654615 vital-1.4.4/vital/internal/__init__.py
--rw-r--r--   0        0        0     2363 2023-08-03 18:40:14.654615 vital-1.4.4/vital/internal/requester.py
--rw-r--r--   0        0        0       80 2023-08-03 18:40:14.654615 vital-1.4.4/vital/internal/utils.py
--rw-r--r--   0        0        0     2762 2023-08-03 18:40:14.654615 vital-1.4.4/vital/internal/webhook.py
--rw-r--r--   0        0        0      359 2023-08-03 18:40:14.654615 vital-1.4.4/vital/types.py
--rw-r--r--   0        0        0      239 2023-08-03 18:40:14.654615 vital-1.4.4/vital/version.py
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 vital-1.4.4/setup.py
--rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 vital-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0      388 2023-08-08 13:36:07.004325 vital-1.4.6/README.md
+-rw-r--r--   0        0        0     1123 2023-08-08 13:36:07.004325 vital-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-08-08 13:36:07.004325 vital-1.4.6/vital/__init__.py
+-rw-r--r--   0        0        0      702 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/__init__.py
+-rw-r--r--   0        0        0     1531 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/activity.py
+-rw-r--r--   0        0        0      142 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/api.py
+-rw-r--r--   0        0        0     2904 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/athome_phlebotomy.py
+-rw-r--r--   0        0        0     1515 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/body.py
+-rw-r--r--   0        0        0      598 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/devices.py
+-rw-r--r--   0        0        0     5148 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/labtests.py
+-rw-r--r--   0        0        0     3093 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/link.py
+-rw-r--r--   0        0        0      823 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/meals.py
+-rw-r--r--   0        0        0      820 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/profile.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/schema/__init__.py
+-rw-r--r--   0        0        0     1719 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/schema/athome_phlebotomy.py
+-rw-r--r--   0        0        0     2259 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/sleep.py
+-rw-r--r--   0        0        0     2287 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/user.py
+-rw-r--r--   0        0        0     3866 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/vitals.py
+-rw-r--r--   0        0        0      632 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/webhooks.py
+-rw-r--r--   0        0        0     1318 2023-08-08 13:36:07.004325 vital-1.4.6/vital/api/workouts.py
+-rw-r--r--   0        0        0     5888 2023-08-08 13:36:07.004325 vital-1.4.6/vital/client.py
+-rw-r--r--   0        0        0     3118 2023-08-08 13:36:07.004325 vital-1.4.6/vital/errors.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:07.004325 vital-1.4.6/vital/internal/__init__.py
+-rw-r--r--   0        0        0     2363 2023-08-08 13:36:07.004325 vital-1.4.6/vital/internal/requester.py
+-rw-r--r--   0        0        0       80 2023-08-08 13:36:07.004325 vital-1.4.6/vital/internal/utils.py
+-rw-r--r--   0        0        0     2762 2023-08-08 13:36:07.004325 vital-1.4.6/vital/internal/webhook.py
+-rw-r--r--   0        0        0      359 2023-08-08 13:36:07.004325 vital-1.4.6/vital/types.py
+-rw-r--r--   0        0        0      239 2023-08-08 13:36:07.004325 vital-1.4.6/vital/version.py
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 vital-1.4.6/setup.py
+-rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 vital-1.4.6/PKG-INFO
```

### Comparing `vital-1.4.4/pyproject.toml` & `vital-1.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vital"
-version = "1.4.4"
+version = "1.4.6"
 description = ""
 authors = ["maitham <maitham@tryvital.io>"]
 license = "GNU"
 readme = "README.md"
 homepage = "https://github.com/adeptlabs/vital-python"
 repository = "https://github.com/adeptlabs/vital-python"
 keywords = ["vital", "tryvital", "python"]
```

### Comparing `vital-1.4.4/vital/api/__init__.py` & `vital-1.4.6/vital/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/api/activity.py` & `vital-1.4.6/vital/api/activity.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/api/athome_phlebotomy.py` & `vital-1.4.6/vital/api/athome_phlebotomy.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/api/body.py` & `vital-1.4.6/vital/api/body.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/api/devices.py` & `vital-1.4.6/vital/api/devices.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/api/labtests.py` & `vital-1.4.6/vital/api/labtests.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,86 @@
-from typing import Dict, Mapping, Optional
+from typing import Dict, List, Mapping, Optional
 
 from vital.api.api import API
 
 
 class LabTests(API):
     """V3 endpoints for managing testkit orders."""
 
+    def register_testkit_order(
+        self,
+        user_id: str,
+        sample_id: str,
+        patient_details: dict,
+        patient_address: dict,
+        physician: Optional[dict] = None,
+        consents: Optional[List[dict]] = None,
+    ) -> Mapping[str, str]:
+        """ Register a testkit """
+        params = {
+            "user_id": user_id,
+            "sample_id": sample_id,
+            "patient_details": patient_details,
+            "patient_address": patient_address,
+        }
+        if physician:
+            params["physician"] = physician
+        if consents:
+            params["consents"] = consents
+
+        return self.client.post("/order/testkit/register", params, api_version="v3")
+
+    def create_unregistered_testkit_order(
+        self,
+        user_id: str,
+        lab_test_id: str,
+        shipping_details: dict,
+    ) -> Mapping[str, str]:
+        """ Order an unregistered testkit """
+        params = {
+            "user_id": user_id,
+            "lab_test_id": lab_test_id,
+            "shipping_details": shipping_details,
+        }
+
+        return self.client.post("/order/testkit", params, api_version="v3")
+
     def create_order(
         self,
         user_id: str,
         patient_details: Dict,
         patient_address: Dict,
         lab_test_id: str,
-        physician: Optional[Dict],
+        physician: Optional[Dict] = None,
         health_insurance: Optional[Dict] = None,
         priority: Optional[bool] = None,
+        consents: Optional[List[dict]] = None,
     ) -> Mapping[str, str]:
         """Create new order"""
         params = {
             "user_id": user_id,
             "patient_details": patient_details,
             "patient_address": patient_address,
             "lab_test_id": lab_test_id,
             "physician": physician,
         }
         if health_insurance:
             params["health_insurance"] = health_insurance
         if priority:
             params["priority"] = priority
+        if consents:
+            params["consents"] = consents
 
         return self.client.post("/order", params, api_version="v3")
     
     def create_test(
         self,
         name: str,
         description: str,
-        markers: list[str],
+        markers: List[str],
         lab_id: int,
         method: str,
         sample_type: str,
     ) -> Mapping[str, str]:
         """Create new lab test"""
         params = {
             "name": name,
```

### Comparing `vital-1.4.4/vital/api/link.py` & `vital-1.4.6/vital/api/link.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/api/meals.py` & `vital-1.4.6/vital/api/meals.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/api/profile.py` & `vital-1.4.6/vital/api/profile.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/api/schema/athome_phlebotomy.py` & `vital-1.4.6/vital/api/schema/athome_phlebotomy.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/api/sleep.py` & `vital-1.4.6/vital/api/sleep.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/api/user.py` & `vital-1.4.6/vital/api/user.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/api/vitals.py` & `vital-1.4.6/vital/api/vitals.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/api/webhooks.py` & `vital-1.4.6/vital/api/webhooks.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/api/workouts.py` & `vital-1.4.6/vital/api/workouts.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/client.py` & `vital-1.4.6/vital/client.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/errors.py` & `vital-1.4.6/vital/errors.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/internal/requester.py` & `vital-1.4.6/vital/internal/requester.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/vital/internal/webhook.py` & `vital-1.4.6/vital/internal/webhook.py`

 * *Files identical despite different names*

### Comparing `vital-1.4.4/setup.py` & `vital-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pydantic>=1.10.7,<2.0.0',
  'requests',
  'svix>=0.41.2,<0.42.0',
  'typed-ast>=1.5.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'vital',
-    'version': '1.4.4',
+    'version': '1.4.6',
     'description': '',
     'long_description': "# vital-python\n\nThe official Python Library for [Vital API](https://docs.tryvital.io)\n\n# Install\n\n```\npip install vital\n```\n\n# Installing locally\n\n```\npoetry build --format sdist\ntar -xvf dist/*-`poetry version -s`.tar.gz -O '*/setup.py' > setup.py\n```\n\n## Documentation\n\nPlease refer to the official [Vital docs](https://docs.tryvital.io) provide a full reference on using this library.\n",
     'author': 'maitham',
     'author_email': 'maitham@tryvital.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/adeptlabs/vital-python',
```

### Comparing `vital-1.4.4/PKG-INFO` & `vital-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vital
-Version: 1.4.4
+Version: 1.4.6
 Summary: 
 Home-page: https://github.com/adeptlabs/vital-python
 License: GNU
 Keywords: vital,tryvital,python
 Author: maitham
 Author-email: maitham@tryvital.io
 Requires-Python: >=3.8,<4.0
```

