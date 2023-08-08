# Comparing `tmp/Opti_HPLC_Handler-0.2.4.tar.gz` & `tmp/Opti_HPLC_Handler-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Opti_HPLC_Handler-0.2.4.tar", last modified: Thu Aug  3 06:36:06 2023, max compression
+gzip compressed data, was "Opti_HPLC_Handler-0.2.5.tar", last modified: Tue Aug  8 07:17:29 2023, max compression
```

## Comparing `Opti_HPLC_Handler-0.2.4.tar` & `Opti_HPLC_Handler-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 06:36:06.410286 Opti_HPLC_Handler-0.2.4/
--rw-rw-rw-   0        0        0     1535 2023-08-02 06:32:16.000000 Opti_HPLC_Handler-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     3810 2023-08-03 06:36:06.404765 Opti_HPLC_Handler-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1098 2023-08-02 08:56:46.000000 Opti_HPLC_Handler-0.2.4/README.md
--rw-rw-rw-   0        0        0     1856 2023-08-03 06:35:33.000000 Opti_HPLC_Handler-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-03 06:36:06.411287 Opti_HPLC_Handler-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-03 06:36:06.244480 Opti_HPLC_Handler-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-08-03 06:36:06.322298 Opti_HPLC_Handler-0.2.4/src/OptiHPLCHandler/
--rw-rw-rw-   0        0        0      262 2023-08-03 06:35:15.000000 Opti_HPLC_Handler-0.2.4/src/OptiHPLCHandler/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-07-05 06:16:59.000000 Opti_HPLC_Handler-0.2.4/src/OptiHPLCHandler/data_types.py
--rw-rw-rw-   0        0        0     3392 2023-08-02 08:55:58.000000 Opti_HPLC_Handler-0.2.4/src/OptiHPLCHandler/empower_api_core.py
--rw-rw-rw-   0        0        0     7615 2023-08-02 09:06:05.000000 Opti_HPLC_Handler-0.2.4/src/OptiHPLCHandler/empower_handler.py
-drwxrwxrwx   0        0        0        0 2023-08-03 06:36:06.368995 Opti_HPLC_Handler-0.2.4/src/Opti_HPLC_Handler.egg-info/
--rw-rw-rw-   0        0        0     3810 2023-08-03 06:36:06.000000 Opti_HPLC_Handler-0.2.4/src/Opti_HPLC_Handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      672 2023-08-03 06:36:06.000000 Opti_HPLC_Handler-0.2.4/src/Opti_HPLC_Handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 06:36:06.000000 Opti_HPLC_Handler-0.2.4/src/Opti_HPLC_Handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      167 2023-08-03 06:36:06.000000 Opti_HPLC_Handler-0.2.4/src/Opti_HPLC_Handler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-03 06:36:06.000000 Opti_HPLC_Handler-0.2.4/src/Opti_HPLC_Handler.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 06:36:06.397184 Opti_HPLC_Handler-0.2.4/tests/
--rw-rw-rw-   0        0        0     7088 2023-08-02 10:22:18.000000 Opti_HPLC_Handler-0.2.4/tests/test_core_api.py
--rw-rw-rw-   0        0        0    10886 2023-08-02 09:32:38.000000 Opti_HPLC_Handler-0.2.4/tests/test_proxy_api.py
+drwxrwxrwx   0        0        0        0 2023-08-08 07:17:29.730796 Opti_HPLC_Handler-0.2.5/
+-rw-rw-rw-   0        0        0     1535 2023-08-08 07:06:48.000000 Opti_HPLC_Handler-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     6446 2023-08-08 07:17:29.723147 Opti_HPLC_Handler-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3734 2023-08-08 07:17:19.000000 Opti_HPLC_Handler-0.2.5/README.md
+-rw-rw-rw-   0        0        0     1856 2023-08-08 07:07:28.000000 Opti_HPLC_Handler-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 07:17:29.733788 Opti_HPLC_Handler-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 07:17:29.090678 Opti_HPLC_Handler-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 07:17:29.499993 Opti_HPLC_Handler-0.2.5/src/OptiHPLCHandler/
+-rw-rw-rw-   0        0        0      262 2023-08-08 07:07:35.000000 Opti_HPLC_Handler-0.2.5/src/OptiHPLCHandler/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-08-08 07:06:48.000000 Opti_HPLC_Handler-0.2.5/src/OptiHPLCHandler/data_types.py
+-rw-rw-rw-   0        0        0     3595 2023-08-08 07:06:48.000000 Opti_HPLC_Handler-0.2.5/src/OptiHPLCHandler/empower_api_core.py
+-rw-rw-rw-   0        0        0     7884 2023-08-08 07:06:48.000000 Opti_HPLC_Handler-0.2.5/src/OptiHPLCHandler/empower_handler.py
+drwxrwxrwx   0        0        0        0 2023-08-08 07:17:29.597959 Opti_HPLC_Handler-0.2.5/src/Opti_HPLC_Handler.egg-info/
+-rw-rw-rw-   0        0        0     6446 2023-08-08 07:17:28.000000 Opti_HPLC_Handler-0.2.5/src/Opti_HPLC_Handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-08-08 07:17:29.000000 Opti_HPLC_Handler-0.2.5/src/Opti_HPLC_Handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 07:17:28.000000 Opti_HPLC_Handler-0.2.5/src/Opti_HPLC_Handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2023-08-08 07:17:28.000000 Opti_HPLC_Handler-0.2.5/src/Opti_HPLC_Handler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-08 07:17:28.000000 Opti_HPLC_Handler-0.2.5/src/Opti_HPLC_Handler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 07:17:29.709116 Opti_HPLC_Handler-0.2.5/tests/
+-rw-rw-rw-   0        0        0     9249 2023-08-08 07:06:48.000000 Opti_HPLC_Handler-0.2.5/tests/test_core_api.py
+-rw-rw-rw-   0        0        0    10726 2023-08-08 07:06:48.000000 Opti_HPLC_Handler-0.2.5/tests/test_proxy_api.py
```

### Comparing `Opti_HPLC_Handler-0.2.4/LICENSE` & `Opti_HPLC_Handler-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Opti_HPLC_Handler-0.2.4/pyproject.toml` & `Opti_HPLC_Handler-0.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Opti_HPLC_Handler"
-version = "0.2.4"
+version = "0.2.5"
 description = "Simplified proxy API for interacting with the Waters Empower Web API."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
   { name="Søren Furbo", email="srfu@novonordisk.com" },
 ]
```

### Comparing `Opti_HPLC_Handler-0.2.4/src/OptiHPLCHandler/data_types.py` & `Opti_HPLC_Handler-0.2.5/src/OptiHPLCHandler/data_types.py`

 * *Files identical despite different names*

### Comparing `Opti_HPLC_Handler-0.2.4/src/OptiHPLCHandler/empower_api_core.py` & `Opti_HPLC_Handler-0.2.5/src/OptiHPLCHandler/empower_api_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import getpass
+import warnings
 from typing import Optional
 
 import keyring
 import requests
 from keyring.errors import NoKeyringError
 
 
@@ -86,15 +87,19 @@
                 headers={"Authorization": "Bearer " + self.token},
             )
         return response
 
     @property
     def password(self):
         try:
-            password = keyring.get_password("empower", self.username)
+            password = keyring.get_password("Empower", self.username)
         except (
             NoKeyringError
         ):  # If no keyring is available, ask for password. This is the case in Datalab.
             password = None
         if not password:
-            password = getpass.getpass("Please enter your password: ")
+            if not self.address.startswith("https"):
+                warnings.warn("The password will be sent in plain text.")
+            password = getpass.getpass(
+                f"Please enter the password for user {self.username}: "
+            )
         return password
```

### Comparing `Opti_HPLC_Handler-0.2.4/src/OptiHPLCHandler/empower_handler.py` & `Opti_HPLC_Handler-0.2.5/src/OptiHPLCHandler/empower_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,38 +5,45 @@
 from .empower_api_core import EmpowerConnection
 
 Result = TypeVar("Result")
 
 Setup = TypeVar("Setup")
 
 
-class InstrumentHandler(ABC, Generic[Result, Setup]):
-    def __init__(self, run_automatically: bool):
-        self.run_automatically = run_automatically
+class StatefulInstrumentHandler(ABC, Generic[Result, Setup]):
+    def __init__(self):
+        pass
 
     @property
     @abstractmethod
     def Status(self) -> List[Result]:
         pass
 
     @abstractmethod
-    def Post(experiment: Any) -> Result:
+    def PostExperiment(experiment: Any):
         """
         Post the experiment to the instrument.
+        """
+        pass
+
+    @abstractmethod
+    def RunExperiment(experiment: Any) -> Result:
+        """
+        Run the experiment on the instrument.
 
-        If the InstrumentHandler is set to run automatically, this will also run the experiment.
+        This will run an experiment that already exists .
         """
         pass
 
     @abstractmethod
     def GetSetup() -> List[Setup]:
         pass
 
 
-class EmpowerHandler(InstrumentHandler):
+class EmpowerHandler(StatefulInstrumentHandler[HplcResult, HPLCSetup]):
     def __init__(
         self,
         project: str,
         address: str,
         username: Optional[str] = None,
         service: str = None,
         **kwargs,
@@ -58,92 +65,114 @@
     def username(self) -> str:
         return self.connection.username
 
     def Status(self) -> List[HplcResult]:
         """Get the status of the HPLC."""
         raise NotImplementedError
 
-    def Post(
+    def PostExperiment(
         self,
-        sample_set_name: str,
+        sample_set_method_name: str,
         sample_list: List[Sample],
         plate_list: List[Any],
         audit_trail_message: str,
-        hplc: Optional[str] = None,
-    ) -> List[HplcResult]:
+    ):
         """
-        Post the experiment to the HPLC. Also runs them if the InstrumentHandler is set to run automatically.
+        Post the experiment to the HPLC.
 
 
-        :param sample_set_name: Name of the sample set method. This will be the name of the sample set in Empower.
+        :param sample_set_method_name: Name of the sample set method. This will be the
+            name of the sample set in Empower.
 
-        :param sample_list: List of samples to run. Each sample is a dictionary with the following keys:
+        :param sample_list: List of samples to run. Each sample is a dictionary with
+            the following keys:
             - Method: Name of the method to use for the sample
-            - SamplePos: Position of the sample in the autosampler, including plate and position on the plate
+            - SamplePos: Position of the sample in the autosampler, including plate and
+                position on the plate
             - SampleName: Name of the sample
             - InjectionVolume: Volume of the sample to inject in micro liters
-            - OtherFields: List of other fields to add to the sample. Each field is a dictionary with the
-                following keys:
+            - OtherFields: List of other fields to add to the sample. Each field is a
+                dictionary with the following keys:
                 - name: Name of the field
-                - value: Value of the field. Can be a string, number, or dictionary with the following keys:
+                - value: Value of the field. Can be a string, number, or dictionary
+                    with the following keys:
                     - member: Name of the member to use for the field
                     - value: Value of the member
-            For all fields, the datatype will be autodetermined according the the type of the value. For Boolean
-            values, this will errouneously be set to string. Instead, use `"value": {"member": “No”}` or
-            `"value": {"member": “Yes”}`
+            For all fields, the datatype will be autodetermined according the the type
+                of the value. For Boolean
+            values, this will errouneously be set to string. Instead, use
+                `"value": {"member": “No”}` or `"value": {"member": “Yes”}`
 
-        :param plate_list: List of plates to use. Each plate is a dictionary with the following keys:
+        :param plate_list: List of plates to use. Each plate is a dictionary with the
+            following keys:
             - plateTypeName: Name of the plate type
-            - position: Position of the plate in the autosampler. This is what you reference in
-                the sample value "SamplePos"
-
-        :param audit_trail_message: Message to add to the audit trail of the sample set method
-
-        :param hplc: Name of the HPLC to run the samples on. If not specified, the samples can not be run.
-            If the InstrumentHandler is set to be run automatically, this will raise an error.
-
-        :return:
-
-            - hplc_result_list: List of results of the samples. Each result is a dictionary with the following keys:
-                - StartTime: The (possibly expected) time of the injection
-                - EndTime: The (possibly expected) end time of the analysis
-                - PerformedExperiment: The experiment that was run
-                - Data: A reference to where the raw data of the experiment is stored
+            - position: Position of the plate in the autosampler. This is what you
+                reference in the sample value "SamplePos"
 
+        :param audit_trail_message: Message to add to the audit trail of the sample set
+            method
         """
         sampleset_object = {"plates": plate_list}
         empower_sample_list = []
         for num, sample in enumerate(sample_list):
             field_list = [
                 {"name": "Function", "value": {"member": "Inject Samples"}},
                 {"name": "Processing", "value": {"member": "Normal"}},
                 {"name": "MethodSetOrReportMethod", "value": sample["Method"]},
                 {"name": "Vial", "value": sample["SamplePos"]},
                 {"name": "SampleName", "value": sample["SampleName"]},
                 {"name": "InjVol", "value": sample["InjectionVolume"]},
             ]
             other_fields = sample.get("OtherFields", [])
-            # Getting the other fields to add, or an empty list if no other fields are given.
+            # Getting the other fields to add, or an empty list if no other fields are
+            # given.
             for field in other_fields:
                 field_list.append(field)
             for field in field_list:
-                self.set_data_type(field)
+                self._set_data_type(field)
             empower_sample_list.append(
                 {"components": [], "id": num, "fields": field_list}
             )
         sampleset_object["sampleSetLines"] = empower_sample_list
-        endpoint = f"project/methods/sample-set-method?name={sample_set_name}"
+        endpoint = f"project/methods/sample-set-method?name={sample_set_method_name}"
         if audit_trail_message:
             endpoint += f"&AtComment={audit_trail_message}"
         response = self.connection.post(endpoint=endpoint, body=sampleset_object)
-        if self.run_automatically:
-            if hplc is None:
-                raise ValueError("No HPLC specified.")
-            raise NotImplementedError  # Run the sample set, and find the expected start and end times
-        return response.json()["results"]  # Wrong return type
+        if response.status_code != 201:
+            raise ValueError(
+                f"Could not post sample set method. Response: {response.text}"
+            )
+
+    def RunExperiment(
+        self,
+        sample_set_method: str,
+        node: str,
+        hplc: str = None,
+        sample_set_name: Optional[str] = None,
+    ) -> HplcResult:
+        """Run the experiment on an instrument."""
+        parameters = {
+            "sampleSetMethodName": sample_set_method,
+            "sampleSetName": sample_set_name,
+            "shutDownMethodName": "",
+            "processingPrinter": "",
+            "runMode": "RunOnly",
+            "suitabilityMode": "ContinueOnFault",
+            "waitForUser": False,
+            "reRun": False,
+            "sampleSetId": 0,
+            "fromLine": 0,
+            "nodeName": node,
+            "systemName": hplc,
+        }
+        reply = self.connection.post(
+            endpoint="acquisition/run-sample-set", body=parameters
+        )
+        if reply.status_code != 200:
+            raise ValueError(f"Could not run experiment. Response: {reply.text}")
 
     def AddMethod(
         self,
         template_method: str,
         new_method: str,
         changes: Dict[str, Any],
         audit_trail_message: str,
@@ -167,18 +196,18 @@
         method_name_list = [
             name_dict[0]["value"] for name_dict in method_name_dict_list
         ]
         return method_name_list
 
     def GetSetup(self) -> List[HPLCSetup]:
         """Get the list of HPLC setups"""
-        # This is almost certainly an incredibly naive use of the API. Fill out with correct details when available.
         raise NotImplementedError
 
-    def set_data_type(self, field: Dict[str, Any]) -> Dict[str, Any]:
+    def _set_data_type(self, field: Dict[str, Any]):
+        """Find and set the data type of the field, based on the type of `value"""
         data_type_dict = {
             str: "String",
             int: "Double",
             float: "Double",
             dict: "Enumerator",
         }
         data_type = type(field["value"])
```

### Comparing `Opti_HPLC_Handler-0.2.4/tests/test_core_api.py` & `Opti_HPLC_Handler-0.2.5/tests/test_core_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import unittest
 from unittest.mock import MagicMock, patch
+import warnings
 
 from OptiHPLCHandler import EmpowerConnection
 
 
 class TestEmpowerConnection(unittest.TestCase):
     @patch("OptiHPLCHandler.empower_api_core.getpass.getpass")
     @patch("OptiHPLCHandler.empower_api_core.requests")
@@ -139,7 +140,53 @@
         mock_response.status_code = 401
         mock_requests.post.return_value = mock_response
         mock_requests.get.return_value = mock_response
         mock_getpass.return_value = self.mock_password
 
         with self.assertRaises(IOError):
             self.connection.login()
+
+    @patch("OptiHPLCHandler.empower_api_core.getpass.getpass")
+    @patch("OptiHPLCHandler.empower_api_core.requests")
+    def test_http_warning(self, mock_requests, mock_getpass):
+        # Verify that the handler warns if the connection is not https.
+        mock_response = MagicMock()
+        mock_response.status_code = 200
+        mock_requests.post.return_value = mock_response
+        mock_requests.get.return_value = mock_response
+        mock_getpass.return_value = self.mock_password
+        with self.assertWarns(Warning):
+            self.connection.login()
+
+    @patch("OptiHPLCHandler.empower_api_core.getpass.getpass")
+    @patch("OptiHPLCHandler.empower_api_core.requests")
+    def test_no_warning_https(self, mock_request, mock_getpass):
+        # Verify that the handler does not warn if the connection is https.
+        mock_response = MagicMock()
+        mock_response.status_code = 200
+        mock_request.post.return_value = mock_response
+        mock_request.get.return_value = mock_response
+        mock_getpass.return_value = self.mock_password
+        connection = EmpowerConnection(
+            address="https://test_address/",
+            username="test_username",
+            project="test_project",
+        )
+        with warnings.catch_warnings():
+            warnings.simplefilter("error")
+            connection.login()
+
+    @patch("OptiHPLCHandler.empower_api_core.getpass.getpass")
+    @patch("OptiHPLCHandler.empower_api_core.requests")
+    def test_info_in_login_message(self, mock_request, mock_getpass):
+        # Verify that the handler prints the correct info in the login message.
+        mock_response = MagicMock()
+        mock_response.status_code = 200
+        mock_request.post.return_value = mock_response
+        mock_request.get.return_value = mock_response
+        mock_getpass.return_value = self.mock_password
+        connection = EmpowerConnection(
+            address="https://test_address/",
+            username="test_username",
+            project="test_project",
+        )
+        assert "test_username" in mock_getpass.call_args[0][0]
```

### Comparing `Opti_HPLC_Handler-0.2.4/tests/test_proxy_api.py` & `Opti_HPLC_Handler-0.2.5/tests/test_proxy_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,44 +20,43 @@
         mock_requests.post.return_value = mock_response
         # The connection logs in automatically, so we need to mock that response
 
         mock_password = MagicMock()
         mock_password.return_value = "test_password"
         self.mock_password = mock_password
         mock_getpass.return_value = mock_password
-        # getpass is used to get the password, so we need to mock that response since interactivity is not possible
+        # getpass is used to get the password, so we need to mock that response since
+        # interactivity is not possible for automated testing.
 
         self.handler = EmpowerHandler(
             project="test_project",
             address="http://test_address/",
             username="test_username",
-            run_automatically=True,
         )
 
     def test_empower_handler_initialisation(self):
         assert self.handler.project == "test_project"
         assert self.handler.username == "test_username"
         assert self.handler.address == "http://test_address/"
-        assert self.handler.run_automatically is True
         assert self.handler.connection.address == "http://test_address/"
         assert self.handler.connection.username == "test_username"
         assert self.handler.connection.project == "test_project"
         assert self.handler.connection.service == "test_service"
 
     def test_empower_handler_status(self):
         with self.assertRaises(NotImplementedError):
             self.handler.Status()
 
     @patch("OptiHPLCHandler.empower_api_core.requests")
     def test_empower_handler_post_sample_list(self, mock_requests):
         mock_response = MagicMock()
         mock_response.json.return_value = {"results": "mock_results"}
+        mock_response.status_code = 201
         mock_requests.post.return_value = mock_response
 
-        self.handler.run_automatically = False
         sample_list = [
             {
                 "Method": "test_method_1",
                 "SamplePos": "test_sample_pos_1",
                 "SampleName": "test_sample_name_1",
                 "InjectionVolume": 1,
             },
@@ -68,40 +67,41 @@
                 "InjectionVolume": 2,
                 "OtherFields": [
                     {"name": "test_field_1", "value": "test_value"},
                     {"name": "test_field_2", "value": 2.3},
                 ],
             },
         ]
-        response = self.handler.Post(
-            sample_set_name="test_sampleset_name",
+        self.handler.PostExperiment(
+            sample_set_method_name="test_sampleset_name",
             sample_list=sample_list,
             plate_list=[],
             audit_trail_message="test_audit_trail_message",
         )
-        assert response == "mock_results"
         assert "name=test_sampleset_name" in mock_requests.method_calls[0][1][0]
         # Testing that the name is correct in the request
         assert (
             "AtComment=test_audit_trail_message" in mock_requests.method_calls[0][1][0]
         )
         # Testing that the audit trail message is correct
         sample_set_lines = mock_requests.method_calls[0][2]["json"]["sampleSetLines"]
         first_line_fields = {
             field["name"]: field["value"] for field in sample_set_lines[0]["fields"]
         }
-        # Converting the fields in the first sample set line to a dictionary for easier testing
+        # Converting the fields in the first sample set line to a dictionary for easier
+        # testing
         assert first_line_fields["MethodSetOrReportMethod"] == "test_method_1"
         assert first_line_fields["Vial"] == "test_sample_pos_1"
         assert first_line_fields["SampleName"] == "test_sample_name_1"
         assert first_line_fields["InjVol"] == 1
         second_line_fields = {
             field["name"]: field["value"] for field in sample_set_lines[1]["fields"]
         }
-        # Converting the fields in the second sample set line  to a dictionary for easier testing
+        # Converting the fields in the second sample set line to a dictionary for easier
+        # testing
         assert second_line_fields["MethodSetOrReportMethod"] == "test_method_2"
         assert second_line_fields["Vial"] == "test_sample_pos_2"
         assert second_line_fields["SampleName"] == "test_sample_name_2"
         assert second_line_fields["InjVol"] == 2
         assert second_line_fields["test_field_1"] == "test_value"
         assert second_line_fields["test_field_2"] == 2.3
         int_type_list = [
@@ -130,43 +130,14 @@
             field["dataType"]
             for field in sample_set_lines[0]["fields"]
             if type(field["value"]) == dict
         ]
         assert all([dict_type == "Enumerator" for dict_type in dict_type_list])
         # Testing that all dictionary values are strings
 
-    @patch("OptiHPLCHandler.empower_api_core.requests")
-    def test_empower_handler_run_automatically(self, mock_requests):
-        mock_response = MagicMock()
-        mock_response.json.return_value = {"results": "mock_results"}
-        mock_requests.post.return_value = mock_response
-        sample_list = [
-            {
-                "Method": "test_method_1",
-                "SamplePos": "test_sample_pos_1",
-                "SampleName": "test_sample_name_1",
-                "InjectionVolume": 1,
-            }
-        ]
-        with self.assertRaises(ValueError):
-            self.handler.Post(
-                sample_set_name="test_sampleset_name",
-                sample_list=sample_list,
-                plate_list=[],
-                audit_trail_message="test_audit_trail_message",
-            )
-        with self.assertRaises(NotImplementedError):
-            self.handler.Post(
-                hplc="test_instrument",
-                sample_set_name="test_sampleset_name",
-                sample_list=sample_list,
-                plate_list=[],
-                audit_trail_message="test_audit_trail_message",
-            )
-
     def test_empower_handler_add_method(self):
         with self.assertRaises(NotImplementedError):
             self.handler.AddMethod(
                 template_method="test_template_method",
                 new_method="test_new_method",
                 changes={},
                 audit_trail_message="test_audit_trail_message",
@@ -245,7 +216,34 @@
         mock_requests.get.return_value = mock_response
         with self.assertRaises(ValueError):
             self.handler.GetMethodList()
 
     def test_empower_handler_get_setup(self):
         with self.assertRaises(NotImplementedError):
             self.handler.GetSetup()
+
+    @patch("OptiHPLCHandler.empower_api_core.requests")
+    def test_empower_run_experiment_fails(self, mock_requests):
+        mock_response = MagicMock()
+        mock_response.status_code = 400
+        mock_requests.post.return_value = mock_response
+        with self.assertRaises(ValueError):
+            self.handler.RunExperiment(
+                sample_set_method="test_sample_set_method",
+                node="test_node",
+                hplc="test_hplc",
+            )
+
+    @patch("OptiHPLCHandler.empower_api_core.requests")
+    def test_empower_run_experiment(self, mock_requests):
+        mock_response = MagicMock()
+        mock_response.status_code = 200
+        mock_requests.post.return_value = mock_response
+        self.handler.RunExperiment(
+            sample_set_method="test_sample_set_method",
+            node="test_node",
+            hplc="test_hplc",
+        )
+        assert (
+            mock_requests.post.call_args[0][0]
+            == "http://test_address/acquisition/run-sample-set"
+        )  # Check that the correct URl is used.
```

