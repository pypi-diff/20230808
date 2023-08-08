# Comparing `tmp/privateai_client-1.3.0rc1.tar.gz` & `tmp/privateai_client-1.3.1.tar.gz`

## Comparing `privateai_client-1.3.0rc1.tar` & `privateai_client-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/.github/pull-request-template.md
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/.vscode/settings.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/objects.py
--rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/pai_client.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/components/__init__.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/components/pai_requests.py
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/components/pai_responses.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/components/pai_uris.py
--rw-r--r--   0        0        0    24972 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/components/request_objects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/tests/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/tests/test_client.py
--rw-r--r--   0        0        0    41229 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/src/privateai_client/tests/test_request_objects.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/LICENSE
--rw-r--r--   0        0        0    12634 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/README.md
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0    13268 2020-02-02 00:00:00.000000 privateai_client-1.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 privateai_client-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.3.1/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 privateai_client-1.3.1/.github/pull-request-template.md
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 privateai_client-1.3.1/.vscode/settings.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 privateai_client-1.3.1/src/privateai_client/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 privateai_client-1.3.1/src/privateai_client/objects.py
+-rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 privateai_client-1.3.1/src/privateai_client/pai_client.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 privateai_client-1.3.1/src/privateai_client/components/__init__.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 privateai_client-1.3.1/src/privateai_client/components/pai_requests.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 privateai_client-1.3.1/src/privateai_client/components/pai_responses.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 privateai_client-1.3.1/src/privateai_client/components/pai_uris.py
+-rw-r--r--   0        0        0    24972 2020-02-02 00:00:00.000000 privateai_client-1.3.1/src/privateai_client/components/request_objects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.3.1/src/privateai_client/tests/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 privateai_client-1.3.1/src/privateai_client/tests/test_client.py
+-rw-r--r--   0        0        0    41229 2020-02-02 00:00:00.000000 privateai_client-1.3.1/src/privateai_client/tests/test_request_objects.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 privateai_client-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 privateai_client-1.3.1/LICENSE
+-rw-r--r--   0        0        0    12634 2020-02-02 00:00:00.000000 privateai_client-1.3.1/README.md
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 privateai_client-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    13265 2020-02-02 00:00:00.000000 privateai_client-1.3.1/PKG-INFO
```

### Comparing `privateai_client-1.3.0rc1/.pre-commit-config.yaml` & `privateai_client-1.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `privateai_client-1.3.0rc1/src/privateai_client/objects.py` & `privateai_client-1.3.1/src/privateai_client/objects.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.3.0rc1/src/privateai_client/pai_client.py` & `privateai_client-1.3.1/src/privateai_client/pai_client.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.3.0rc1/src/privateai_client/components/pai_requests.py` & `privateai_client-1.3.1/src/privateai_client/components/pai_requests.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.3.0rc1/src/privateai_client/components/pai_responses.py` & `privateai_client-1.3.1/src/privateai_client/components/pai_responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,19 @@
         return self.get_attribute_entries("entities")
 
     @property
     def entities_present(self):
         return self.get_attribute_entries("entities_present")
 
     def get_reidentify_entities(self):
-        return [Entity(attr["processed_text"], attr["text"]) for entity in self.entities for attr in entity]
+        if type(self.body) == dict:
+            entities = [Entity(entity["processed_text"], entity["text"]) for entity in self.entities]
+        else:
+            entities = [Entity(attr["processed_text"], attr["text"]) for entity in self.entities for attr in entity]
+        return entities
 
     def get_reidentify_request(self):
         entities = self.get_reidentify_entities()
         return ReidentifyTextRequest(self.processed_text, entities)
 
 
 class TextResponse(DemiTextResponse):
```

### Comparing `privateai_client-1.3.0rc1/src/privateai_client/components/pai_uris.py` & `privateai_client-1.3.1/src/privateai_client/components/pai_uris.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.3.0rc1/src/privateai_client/components/request_objects.py` & `privateai_client-1.3.1/src/privateai_client/components/request_objects.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.3.0rc1/src/privateai_client/tests/test_request_objects.py` & `privateai_client-1.3.1/src/privateai_client/tests/test_request_objects.py`

 * *Files identical despite different names*

### Comparing `privateai_client-1.3.0rc1/LICENSE` & `privateai_client-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `privateai_client-1.3.0rc1/README.md` & `privateai_client-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `privateai_client-1.3.0rc1/pyproject.toml` & `privateai_client-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "privateai_client"
-version = "1.3.0rc1"
+version = "1.3.1"
 authors = [
   { name="Adam Guiducci", email="adam.guiducci@private-ai.com" },
   { name="Bryan Bell-Smith", email="bryan.bellsmith@private-ai.com" },
 ]
 description = "A thin client for communicating with the Private AI de-identication API."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `privateai_client-1.3.0rc1/PKG-INFO` & `privateai_client-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: privateai_client
-Version: 1.3.0rc1
+Version: 1.3.1
 Summary: A thin client for communicating with the Private AI de-identication API.
 Project-URL: Homepage, https://github.com/privateai/pai-thin-client/
 Project-URL: Bug Tracker, https://github.com/privateai/pai-thin-client/issues
 Author-email: Adam Guiducci <adam.guiducci@private-ai.com>, Bryan Bell-Smith <bryan.bellsmith@private-ai.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

