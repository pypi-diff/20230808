# Comparing `tmp/idun_guardian_client-1.2.0.tar.gz` & `tmp/idun_guardian_client-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idun_guardian_client-1.2.0.tar", max compression
+gzip compressed data, was "idun_guardian_client-1.2.1.tar", max compression
```

## Comparing `idun_guardian_client-1.2.0.tar` & `idun_guardian_client-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3381 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.0/idun_guardian_client/.gitignore
--rw-r--r--   0        0        0      351 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.0/idun_guardian_client/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.0/idun_guardian_client/__main__.py
--rw-r--r--   0        0        0    10327 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.0/idun_guardian_client/client.py
--rw-r--r--   0        0        0     1631 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.0/idun_guardian_client/config.py
--rw-r--r--   0        0        0    16040 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.0/idun_guardian_client/debug_logs.py
--rw-r--r--   0        0        0    25884 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.0/idun_guardian_client/igeb_api.py
--rw-r--r--   0        0        0    34995 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.0/idun_guardian_client/igeb_bluetooth.py
--rw-r--r--   0        0        0     7901 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.0/idun_guardian_client/igeb_utils.py
--rw-r--r--   0        0        0      200 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.0/idun_guardian_client/mock_utils.py
--rw-r--r--   0        0        0     1263 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.0/idun_guardian_client/test_producer_consumer.py
--rw-r--r--   0        0        0      853 2023-07-05 12:04:16.680683 idun_guardian_client-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     8680 2023-06-02 08:49:58.338164 idun_guardian_client-1.2.0/README.md
--rw-r--r--   0        0        0     9175 1970-01-01 00:00:00.000000 idun_guardian_client-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3381 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.1/idun_guardian_client/.gitignore
+-rw-r--r--   0        0        0      351 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.1/idun_guardian_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.1/idun_guardian_client/__main__.py
+-rw-r--r--   0        0        0    10352 2023-08-08 08:05:39.182480 idun_guardian_client-1.2.1/idun_guardian_client/client.py
+-rw-r--r--   0        0        0     1631 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.1/idun_guardian_client/config.py
+-rw-r--r--   0        0        0    16173 2023-08-08 07:34:02.462574 idun_guardian_client-1.2.1/idun_guardian_client/debug_logs.py
+-rw-r--r--   0        0        0    25886 2023-08-08 07:34:02.463574 idun_guardian_client-1.2.1/idun_guardian_client/igeb_api.py
+-rw-r--r--   0        0        0    35000 2023-08-08 07:34:02.464573 idun_guardian_client-1.2.1/idun_guardian_client/igeb_bluetooth.py
+-rw-r--r--   0        0        0     7969 2023-08-08 07:34:02.465574 idun_guardian_client-1.2.1/idun_guardian_client/igeb_utils.py
+-rw-r--r--   0        0        0      200 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.1/idun_guardian_client/mock_utils.py
+-rw-r--r--   0        0        0     1263 2023-07-05 12:04:16.672682 idun_guardian_client-1.2.1/idun_guardian_client/test_producer_consumer.py
+-rw-r--r--   0        0        0      853 2023-08-08 07:34:02.468574 idun_guardian_client-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8680 2023-06-02 08:49:58.338164 idun_guardian_client-1.2.1/README.md
+-rw-r--r--   0        0        0     9175 1970-01-01 00:00:00.000000 idun_guardian_client-1.2.1/PKG-INFO
```

### Comparing `idun_guardian_client-1.2.0/idun_guardian_client/.gitignore` & `idun_guardian_client-1.2.1/idun_guardian_client/.gitignore`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.2.0/idun_guardian_client/client.py` & `idun_guardian_client-1.2.1/idun_guardian_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .igeb_api import GuardianAPI
 from .igeb_utils import check_platform, check_valid_mac, check_valid_uuid
 import uuid
 import gc
 from typing import Union
 from bleak import exc
 from idun_data_models.rest_data_model import RecordingIn, DataStreams, RecordingConfig
+from .debug_logs import *
 
 
 class GuardianClient:
     """
     Class object for the communication between Guardian Earbuds and Cloud API
     """
 
@@ -179,15 +180,15 @@
             )  # the recordingID is a unique ID for each recording
             logging.info("[CLIENT] Recording ID: %s", recording_id)
             # log the experiment name in bold using the logging module
             logging.info("[CLIENT] Experiment description: %s", experiment)
 
             while self.connection_status == 0:  # TRUE FALSE
                 self.connection_status = await self.guardian_ble.connect_to_device()
-                print("Current Device Status=", self.connection_status)
+                log_device_status(self.debug, self.connection_status)
             data_stream = RecordingConfig(
                 data_stream_subscription=DataStreams(bandpass_eeg=True)
             )
 
             self.guardian_api.guardian_rec = RecordingIn(
                 recordingID=recording_id,
                 deviceID=self.guardian_ble.mac_id,
```

### Comparing `idun_guardian_client-1.2.0/idun_guardian_client/config.py` & `idun_guardian_client-1.2.1/idun_guardian_client/config.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.2.0/idun_guardian_client/debug_logs.py` & `idun_guardian_client-1.2.1/idun_guardian_client/debug_logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """
 This module contains the functions that are used to log the debug messages.
 """
 import logging
 import time
 
 
+def log_device_status(debug, connection_status):
+    if debug:
+        logging.info(f"[BLE]: Current Device Status={connection_status}")
+
+
 def log_calling_function_while_retrying(debug, string: str):
     if debug:
         logging.info(string)
 
 
 def log_sending_start_rec_info(debug):
     if debug:
@@ -118,22 +123,21 @@
             "[API]: No Connection has been established, will disconnect and try to reconnect again"
         )
 
 
 def log_exception_unable_to_find_MACaddress(debug, err):
     if debug:
         logging.info(
-            "[BLE]: The following error occurred when trying to find the device mac ID:",
-            err,
+            f"[BLE]: The following error occurred when trying to find the device mac ID:{err}",
         )
 
 
 def log_exception_while_trying_connection(debug, err):
     if debug:
-        logging.info("[BLE]: Exception raised while trying to connect:", err)
+        logging.info(f"[BLE]: Exception raised while trying to connect:{err}")
 
 
 def log_timeout_while_trying_connection(debug):
     if debug:
         logging.info("[API]: Timeout for connection failure, will try to reconnect")
```

### Comparing `idun_guardian_client-1.2.0/idun_guardian_client/igeb_api.py` & `idun_guardian_client-1.2.1/idun_guardian_client/igeb_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .igeb_utils import unpack_from_queue
 from .mock_utils import mock_cloud_package
 from .debug_logs import *
 from .igeb_utils import (
     retry,
     exit_system,
     stop_ongoing_recording,
-    _string_detail_to_log,
+    string_detail_to_log,
 )
 from idun_data_models.rest_data_model import RecordingIn, RecordingStatusOut
 from idun_data_models.serialization import json_pydantic
 
 load_dotenv()
 
 FILTER_PACKAGE = "bp_filter_eeg"
@@ -114,15 +114,15 @@
                 result = session.post(
                     record_url,
                     headers=headers,
                     data=payload,
                     auth=(device_id, self.password),
                 )
                 status = result.status_code
-                status_details = _string_detail_to_log(result.text)
+                status_details = string_detail_to_log(result.text)
 
                 if status == 200 or status == 201:
                     log_successfully_started(self.debug)
                     self.rec_started_time = datetime.datetime.fromtimestamp(time.time())
                 else:
                     self.password = ""
                     log_api_status(self.debug, status)
@@ -456,22 +456,22 @@
             if self.final_message_sent:
                 logging_break(self.debug)
                 break
 
         logging_api_completed(self.debug)
 
     def get_recordings_info_all(
-        self, device_id: str = "mock-device-0", first_to_last=False, password: str = ""
+        self, device_id: str = "mock-device-0", first_to_last=False
     ) -> list:
         recordings_url = f"{settings.REST_API_LOGIN}recordings"
-        if password == "":
-            password = input("\nEnter your new passsword here: ")
+        if self.password == "":
+            self.password = input("\nEnter your new passsword here: ")
         with requests.Session() as session:  # create a session (without auth?) and check the status? if status 200 ok i continue with the normal way
             result = session.get(
-                recordings_url, auth=(device_id, password)
+                recordings_url, auth=(device_id, self.password)
             )  # however ?
             if result.status_code == 200:
                 print("Recording list retrieved successfully")
                 recordings = result.json()
                 recordings.sort(
                     key=lambda x: datetime.datetime.strptime(
                         x["startDeviceTimestamp"], "%Y-%m-%dT%H:%M:%S.%fZ"
@@ -501,22 +501,22 @@
                 print(f"Device {device_id} does not exist")
                 return []
             else:
                 print("Loading recording list failed")
                 return []
 
     def get_recording_info_by_id(
-        self, device_id: str, recording_id: str = "recordingId-0", password: str = ""
+        self, device_id: str, recording_id: str = "recordingId-0"
     ) -> list:
         recordings_url = f"{settings.REST_API_LOGIN}recordings/{recording_id}"
 
-        if password == "":
-            password = input("\nEnter your new passsword here: ")
+        if self.password == "":
+            self.password = input("\nEnter your new passsword here: ")
         with requests.Session() as session:
-            result = session.get(recordings_url, auth=(device_id, password))
+            result = session.get(recordings_url, auth=(device_id, self.password))
             if result.status_code == 200:
                 print("Recording ID file found")
                 print(json.dumps(result.json(), indent=4, sort_keys=True))
                 return result.json()
             elif result.status_code == 401:
                 print(f"Password for {device_id} is incorrect")
                 return []
@@ -540,30 +540,32 @@
             else:
                 print("Recording not found")
                 print(result.status_code)
                 print(result.json())
                 return []
 
     def download_recording_by_id(
-        self, device_id: str, recording_id: str = "recordingId-0", password: str = ""
+        self,
+        device_id: str,
+        recording_id: str = "recordingId-0",
     ) -> None:
         """Download the recording by ID and save it to the recordings folder"""
 
         recordings_folder_name = "recordings"
         recording_subfolder_name = recording_id
 
-        if password == "":
-            password = input("\nEnter your new passsword here: ")
+        if self.password == "":
+            self.password = input("\nEnter your new passsword here: ")
         recording_types = ["eeg", "imu"]
         for data_type in recording_types:
             with requests.Session() as session:
                 record_url_first = f"{settings.REST_API_LOGIN}recordings/"
                 record_url_second = f"{recording_id}/download/{data_type}"
                 record_url = record_url_first + record_url_second
-                result = session.get(record_url, auth=(device_id, password))
+                result = session.get(record_url, auth=(device_id, self.password))
 
                 if result.status_code == 200:
                     print(f"Recording ID file found, downloading {data_type} data")
                     print(result.json())
 
                     # Creating folder for recording
                     folder_path = os.path.join(
```

### Comparing `idun_guardian_client-1.2.0/idun_guardian_client/igeb_bluetooth.py` & `idun_guardian_client-1.2.1/idun_guardian_client/igeb_bluetooth.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
                 pass
             if self.client.is_connected:
                 if self.mac_id == "":
                     try:
                         self.mac_id = await self.get_device_mac(self.client)
 
                     except Exception as err:
-                        log_exception_unable_to_find_MACaddress(self.debug)
+                        log_exception_unable_to_find_MACaddress(self.debug, err)
                         self.initialise_connection = True
                         self.connection_established = False
                         return 0
                 if self.mac_id:
                     self.connection_established = True
                     self.initialise_connection = False
                     logging_connected(self.debug, self.address)
```

### Comparing `idun_guardian_client-1.2.0/idun_guardian_client/igeb_utils.py` & `idun_guardian_client-1.2.1/idun_guardian_client/igeb_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 from .config import settings
 import requests
 from idun_data_models.rest_data_model import RecordingStatusOut
 from idun_data_models.serialization import json_pydantic
 
 
-def _string_detail_to_log(details: str):
+def string_detail_to_log(details: str):
     i1 = details.find("{")
     i2 = details.find("}")
     message = details[i1 + 2 : i2 - 1]
     return message
 
 
 def retry(debug, tries_numb=4, delay=2):
@@ -60,15 +60,15 @@
     """Exit the system."""
     try:
         sys.exit(0)
     except SystemExit:
         os._exit(0)
 
 
-def stop_ongoing_recording(status_details, device_id, passsword):
+def stop_ongoing_recording(status_details, device_id, password):
     start_index = status_details.find("ID:") + 6
     end_index = status_details.find("}")
     # Extract the recording IDs as a string
     recording_ids_str = status_details[start_index:end_index]
     # Split the string by comma to get individual recording IDs
     recording_ids = recording_ids_str.split(", ")
     # Remove the surrounding single quotes from each recording ID
@@ -89,15 +89,15 @@
                 "accept": "application/json",
                 "Content-Type": "application/json",
             }
             result = session.put(
                 record_url,
                 headers=headers,
                 data=json_pydantic(payload),
-                auth=(device_id, passsword),
+                auth=(device_id, password),
             )
             if result.status_code == 200 or result.status_code == 201:
                 log_rec_ongoing_stopped_successfully(debug=True, rec=rec)
                 successfully_stopped = successfully_stopped + 1
 
             else:
                 log_couldnot_stop_ongoing_rec(debug=True, rec=rec)
@@ -108,40 +108,41 @@
     else:
         print(
             f"We could not stop {int(num)-successfully_stopped} recordings, try to stop the resting recordings manually with the given scripts"
         )
     exit_system()
 
 
-def stop_rec(deviceID, recordingID):
-    pssw = input("Type here your password:")
+def stop_rec(device_id, recording_id, password=""):
+    if password == "":
+        password = input("Type here your password:")
     with requests.Session() as session:
         record_url_first = f"{settings.REST_API_LOGIN}"
-        record_url_second = f"devices/{deviceID}/recordings/{recordingID}/status"
+        record_url_second = f"devices/{device_id}/recordings/{recording_id}/status"
         record_url = record_url_first + record_url_second
         payload = RecordingStatusOut(
             stopped=True,
             status="COMPLETED",
             message="Trying to stop the recording",
         )
         headers = {
             "accept": "application/json",
             "Content-Type": "application/json",
         }
         result = session.put(
             record_url,
             headers=headers,
             data=json_pydantic(payload),
-            auth=(device_id, pssw),
+            auth=(device_id, password),
         )
         if result.status_code == 200 or result.status_code == 201:
-            log_rec_ongoing_stopped_successfully(debug=True, rec=rec)
+            log_rec_ongoing_stopped_successfully(debug=True, rec=recording_id)
 
         else:
-            log_couldnot_stop_ongoing_rec(debug=True, rec=rec)
+            log_couldnot_stop_ongoing_rec(debug=True, rec=recording_id)
             print(result.text)
 
 
 def check_platform():
     """
     Check if the script is running on a cross platform
```

### Comparing `idun_guardian_client-1.2.0/idun_guardian_client/test_producer_consumer.py` & `idun_guardian_client-1.2.1/idun_guardian_client/test_producer_consumer.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.2.0/pyproject.toml` & `idun_guardian_client-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idun-guardian-client"
-version = "1.2.0"
+version = "1.2.1"
 description = "Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud"
 authors = ["IDUN Technologies <contact@iduntechnologies.com>"]
 readme = "README.md"
 packages = [{include = "idun_guardian_client"}]
 
 
 [tool.poetry.dependencies]
```

### Comparing `idun_guardian_client-1.2.0/README.md` & `idun_guardian_client-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.2.0/PKG-INFO` & `idun_guardian_client-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idun-guardian-client
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
 Author: IDUN Technologies
 Author-email: contact@iduntechnologies.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

