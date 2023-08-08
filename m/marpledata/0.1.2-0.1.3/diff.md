# Comparing `tmp/marpledata-0.1.2.tar.gz` & `tmp/marpledata-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marpledata-0.1.2.tar", last modified: Fri Mar 17 17:08:44 2023, max compression
+gzip compressed data, was "marpledata-0.1.3.tar", last modified: Tue Aug  8 20:22:50 2023, max compression
```

## Comparing `marpledata-0.1.2.tar` & `marpledata-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 17:08:44.896932 marpledata-0.1.2/
--rw-rw-rw-   0        0        0        0 2022-07-22 12:48:55.000000 marpledata-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2536 2023-03-17 17:08:44.896932 marpledata-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2110 2023-03-17 16:34:19.000000 marpledata-0.1.2/README.md
--rw-rw-rw-   0        0        0      575 2023-03-17 16:38:07.000000 marpledata-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-17 17:08:44.896932 marpledata-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-17 17:08:44.872176 marpledata-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-17 17:08:44.886331 marpledata-0.1.2/src/marple/
--rw-rw-rw-   0        0        0     4852 2022-12-06 11:02:07.000000 marpledata-0.1.2/src/marple/__init__.py
--rw-rw-rw-   0        0        0     5543 2022-11-29 14:01:19.000000 marpledata-0.1.2/src/marple/__init___BACKUP_1366.py
--rw-rw-rw-   0        0        0     3757 2022-11-29 14:05:08.000000 marpledata-0.1.2/src/marple/__init___BASE_1366.py
--rw-rw-rw-   0        0        0     4352 2022-11-29 14:05:08.000000 marpledata-0.1.2/src/marple/__init___LOCAL_1366.py
--rw-rw-rw-   0        0        0     4407 2022-11-29 14:05:09.000000 marpledata-0.1.2/src/marple/__init___REMOTE_1366.py
-drwxrwxrwx   0        0        0        0 2023-03-17 17:08:44.893372 marpledata-0.1.2/src/marpledata.egg-info/
--rw-rw-rw-   0        0        0     2536 2023-03-17 17:08:44.000000 marpledata-0.1.2/src/marpledata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-03-17 17:08:44.000000 marpledata-0.1.2/src/marpledata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 17:08:44.000000 marpledata-0.1.2/src/marpledata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-03-17 17:08:44.000000 marpledata-0.1.2/src/marpledata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-17 17:08:44.895380 marpledata-0.1.2/tests/
--rw-rw-rw-   0        0        0     2294 2022-12-06 11:06:07.000000 marpledata-0.1.2/tests/test_SDK.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:22:50.482379 marpledata-0.1.3/
+-rw-rw-rw-   0        0        0        0 2022-07-22 12:48:55.000000 marpledata-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2700 2023-08-08 20:22:50.481378 marpledata-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2276 2023-08-08 20:21:25.000000 marpledata-0.1.3/README.md
+-rw-rw-rw-   0        0        0      570 2023-08-08 20:21:25.000000 marpledata-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 20:22:50.482379 marpledata-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 20:22:50.460598 marpledata-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 20:22:50.473339 marpledata-0.1.3/src/marple/
+-rw-rw-rw-   0        0        0     5171 2023-08-07 15:42:32.000000 marpledata-0.1.3/src/marple/__init__.py
+-rw-rw-rw-   0        0        0     5543 2022-11-29 14:01:19.000000 marpledata-0.1.3/src/marple/__init___BACKUP_1366.py
+-rw-rw-rw-   0        0        0     3757 2022-11-29 14:05:08.000000 marpledata-0.1.3/src/marple/__init___BASE_1366.py
+-rw-rw-rw-   0        0        0     4352 2022-11-29 14:05:08.000000 marpledata-0.1.3/src/marple/__init___LOCAL_1366.py
+-rw-rw-rw-   0        0        0     4407 2022-11-29 14:05:09.000000 marpledata-0.1.3/src/marple/__init___REMOTE_1366.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:22:50.479363 marpledata-0.1.3/src/marpledata.egg-info/
+-rw-rw-rw-   0        0        0     2700 2023-08-08 20:22:50.000000 marpledata-0.1.3/src/marpledata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-08-08 20:22:50.000000 marpledata-0.1.3/src/marpledata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 20:22:50.000000 marpledata-0.1.3/src/marpledata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-08 20:22:50.000000 marpledata-0.1.3/src/marpledata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 20:22:50.480371 marpledata-0.1.3/tests/
+-rw-rw-rw-   0        0        0     2294 2022-12-06 11:06:07.000000 marpledata-0.1.3/tests/test_SDK.py
```

### Comparing `marpledata-0.1.2/PKG-INFO` & `marpledata-0.1.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,81 +1,84 @@
-Metadata-Version: 2.1
-Name: marpledata
-Version: 0.1.2
-Summary: Marple SDK
-Author-email: Matthias Baert <support@marpledata.com>
-Project-URL: Homepage, https://www.marpledata.com/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Marple SDK
 
 A simple SDK to upload data to Marple
 
 ## Installation
+
 Install the Marple SDK using:
 
 `pip install marpledata`
 
 Import the package using:
 
 `import marple`
 
 ## Usage
+
 ### Setup
+
 Create a Marple connection using:
 
 ```python
 from marple import Marple
 m = Marple(ACCESS_TOKEN)
 ```
 
-You can find your personal access token in your account settings.
+You can generate access tokens in the app, under _Settings->Tokens_.
 
 If you are using Marple on-premise, you can add the custom URL:
 
 `m = Marple(ACCESS_TOKEN, api_url='https://marple.company.com/api/v1')`
 
 To check your connection, use:
 
 `m.check_connection()`
 
+### Calling endpoints
+
+Call endpoints by their METHOD:
+
+```python
+m.get('/version')
+m.post('/sources/info', json={'id': 98})
+```
+
 ### Upload data files
+
 If your data is already in a file format, use this function to upload the data to Marple.
 
-`source_id = m.upload_data_file(file_path, marple_folder, metadata={})`
+`source_id = m.upload_data_file(file_path, marple_folder='/', metadata={})`
 
 - `file_path`: the file_path of your data set
 - `marple_folder`: in what folder you would like to upload the data
 - `metadata`: dictionary with metadata. Example: `{'Pilot': 'John Doe'}'` Note that the metadata fields need to be added to your workspace before you will see them.
 
 ### Upload a dataframe
+
 If your data is in a pandas dataframe, use this function to upload the data to Marple.
 
-`source_id = m.upload_dataframe(dataframe, target_name, marple_folder, metadata={})`
+`source_id = m.upload_dataframe(dataframe, target_name, marple_folder='/', metadata={})`
 
 - `target_name`: the target name for the dataset, this is how it will appear in Marple.
 
 ### Add and send data
+
 You can also use the Marple SDK to add data piece by piece and send it to Marple.
 First use:
 
 `m.add_data(data_dict)`
 
 - `data_dict` = dictionary with signal, value pairs in it.
   Example: `{'time': 2, 'signal 1': 0, 'signal 2': 5}`
 
 Once all the data has been added, use:
 
 `source_id = m.send_data(target_name, marple_folder, metadata={})`
 
 ### Get a link to the data
+
 You can generate a link to Marple that opens the data and a project immediately. This can be very useful to see the results of a simulation directly.
 
 `link = m.get_link(source_id, project_name)`
 
 - `source_id`: identifier for the data set, is returned by all above functions.
 - `project_name`: name of the project that you want to open the data in.
```

### Comparing `marpledata-0.1.2/src/marple/__init__.py` & `marpledata-0.1.3/src/marple/__init___REMOTE_1366.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,20 @@
 class Marple:
 
     plugin_map = {
         'csv': 'csv_plugin',
         'txt': 'csv_plugin',
         'mat': 'mat_plugin',
         'h5': 'hdf5_plugin',
-        'zip': 'csv_zip_plugin',
+        'zip': 'hdf5_plugin',
         'bag': 'rosbag_plugin',
         'ulg': 'ulog_plugin'
     }
 
     def __init__(self, access_token, api_url=SAAS_URL):
-        if access_token == '':
-            raise Exception('Invalid access token')
         bearer_token = f"Bearer {access_token}"
         self.session = requests.Session()
         self.session.headers.update({"Authorization": bearer_token})
         self.api_url = api_url
         self.data = {}
 
     # User functions #
@@ -47,36 +45,30 @@
                 raise Exception(msg_fail_auth)
 
         except ConnectionError:
             raise Exception(msg_fail_connect)
 
         return True
 
-    def upload_data_file(self, file_path, marple_folder, plugin=None, metadata={}, config=DEFAULT_IMPORT_CONFIG):
+    def upload_data_file(self, file_path, marple_folder, metadata={}, config=DEFAULT_IMPORT_CONFIG):
         file = open(file_path, 'rb')
         r = self.session.post('{}/library/file/upload'.format(self.api_url),
                               params={'path': marple_folder},
                               files={'file': file})
-        if r.status_code != 200:
-            r.raise_for_status()
         source_id, path = r.json()['message']['source_id'], r.json()['message']['path']
 
         # convert to name, value structure
         if metadata:
+            metadata_marple = [{'name': key, 'value': value} for key, value in metadata.items()]
             r = self.session.post('{}/library/metadata'.format(self.api_url),
-                                  json={'source_id': source_id, 'metadata': metadata})
-            if r.status_code != 200:
-                r.raise_for_status()
+                                  json={'source_id': source_id, 'metadata': metadata_marple})
 
-        if plugin is None:
-            plugin = self._guess_plugin(file_path)
+        plugin = self._guess_plugin(file_path)
         body = {'path': path, 'plugin': plugin, 'config': config}
         self.session.post('{}/library/file/import'.format(self.api_url), json=body)
-        if r.status_code != 200:
-            r.raise_for_status()
         return source_id
 
     def upload_dataframe(self, dataframe, name, marple_folder, metadata={}):
         file_name = f'{name}.csv'
         dataframe.to_csv(file_name, sep=',', index=False)
         source_id = self.upload_data_file(file_name, marple_folder, metadata=metadata)
         os.remove(file_name)
@@ -97,34 +89,28 @@
     def send_data(self, name, marple_folder, metadata={}):
         df = pd.DataFrame.from_dict(self.data)
         self.clear_data()
         return self.upload_dataframe(df, name, marple_folder, metadata={})
 
     def check_import_status(self, source_id):
         r = self.session.get('{}/sources/status'.format(self.api_url), params={'id': source_id})
-        if r.status_code != 200:
-            r.raise_for_status()
         return r.json()['message'][0]['status']
 
     def get_link(self, source_id, project_name, open_link=True):
         # make new share link
         body = {'workbook_name': project_name, 'source_ids': [source_id]}
         r = self.session.post('{}/library/share/new'.format(self.api_url), json=body)
-        if r.status_code != 200:
-            r.raise_for_status()
         share_id = r.json()['message']
 
         # Generate clickable link in terminal
         r = self.session.get('{}/library/share/{}/link'.format(self.api_url, share_id))
-        if r.status_code != 200:
-            r.raise_for_status()
         link = r.json()['message']
         print('View your data: {}'.format(link))
         return link
 
     # Internal functions #
 
     def _guess_plugin(self, file_path):
-        extension = file_path.split('.')[-1].lower()
+        extension = file_path.split('.')[0].lower()
         if extension in self.plugin_map:
             return self.plugin_map[extension]
         return 'csv_plugin'
```

### Comparing `marpledata-0.1.2/src/marple/__init___BACKUP_1366.py` & `marpledata-0.1.3/src/marple/__init___BACKUP_1366.py`

 * *Files identical despite different names*

### Comparing `marpledata-0.1.2/src/marple/__init___BASE_1366.py` & `marpledata-0.1.3/src/marple/__init___BASE_1366.py`

 * *Files identical despite different names*

### Comparing `marpledata-0.1.2/src/marple/__init___LOCAL_1366.py` & `marpledata-0.1.3/src/marple/__init___LOCAL_1366.py`

 * *Files identical despite different names*

### Comparing `marpledata-0.1.2/src/marple/__init___REMOTE_1366.py` & `marpledata-0.1.3/src/marple/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,116 +1,143 @@
+import os
+import webbrowser
+
+import pandas as pd
 import requests
 import requests.auth
+from requests import Response
 from requests.exceptions import ConnectionError
-import os
-import pandas as pd
 
-SAAS_URL = 'https://app.marpledata.com/api/v1'
-DEFAULT_IMPORT_CONFIG = {'common':  [], 'signals_groups': []}
+SAAS_URL = "https://app.marpledata.com/api/v1"
+DEFAULT_IMPORT_CONFIG = {"common": [], "signals_groups": []}
 
 
 class Marple:
-
     plugin_map = {
-        'csv': 'csv_plugin',
-        'txt': 'csv_plugin',
-        'mat': 'mat_plugin',
-        'h5': 'hdf5_plugin',
-        'zip': 'hdf5_plugin',
-        'bag': 'rosbag_plugin',
-        'ulg': 'ulog_plugin'
+        "csv": "csv_plugin",
+        "txt": "csv_plugin",
+        "mat": "mat_plugin",
+        "h5": "hdf5_plugin",
+        "zip": "csv_zip_plugin",
+        "bag": "rosbag_plugin",
+        "ulg": "ulog_plugin",
     }
 
     def __init__(self, access_token, api_url=SAAS_URL):
+        if access_token == "":
+            raise Exception("Invalid access token")
         bearer_token = f"Bearer {access_token}"
         self.session = requests.Session()
         self.session.headers.update({"Authorization": bearer_token})
-        self.api_url = api_url
-        self.data = {}
+        self._api_url = api_url
+        self._data = {}
 
     # User functions #
 
+    def get(self, url: str, *args, **kwargs) -> Response:
+        return self.session.get(f"{self._api_url}{url}", *args, **kwargs)
+
+    def post(self, url: str, *args, **kwargs) -> Response:
+        return self.session.post(f"{self._api_url}{url}", *args, **kwargs)
+
+    def patch(self, url: str, *args, **kwargs) -> Response:
+        return self.session.patch(f"{self._api_url}{url}", *args, **kwargs)
+
+    def delete(self, url: str, *args, **kwargs) -> Response:
+        return self.session.delete(f"{self._api_url}{url}", *args, **kwargs)
+
     def check_connection(self):
-        msg_fail_connect = 'Could not connect to server at {}'.format(self.api_url)
-        msg_fail_auth = 'Could not authenticate with token'
+        msg_fail_connect = "Could not connect to server at {}".format(self._api_url)
+        msg_fail_auth = "Could not authenticate with token"
 
         try:
             # unauthenticated endpoints
-            r = self.session.get('{}/version'.format(self.api_url))
+            r = self.get("/version")
             if r.status_code != 200:
                 raise Exception(msg_fail_connect)
 
             # authenticated endpoint
-            r = self.session.get('{}/user/info'.format(self.api_url))
+            r = self.get("/")
             if r.status_code != 200:
                 raise Exception(msg_fail_auth)
 
         except ConnectionError:
             raise Exception(msg_fail_connect)
 
         return True
 
-    def upload_data_file(self, file_path, marple_folder, metadata={}, config=DEFAULT_IMPORT_CONFIG):
-        file = open(file_path, 'rb')
-        r = self.session.post('{}/library/file/upload'.format(self.api_url),
-                              params={'path': marple_folder},
-                              files={'file': file})
-        source_id, path = r.json()['message']['source_id'], r.json()['message']['path']
+    def upload_data_file(self, file_path, marple_folder='/', plugin=None, metadata={}, config=DEFAULT_IMPORT_CONFIG):
+        file = open(file_path, "rb")
+        r = self.post("/library/file/upload", params={"path": marple_folder}, files={"file": file})
+        if r.status_code != 200:
+            r.raise_for_status()
+        source_id, path = r.json()["message"]["source_id"], r.json()["message"]["path"]
 
         # convert to name, value structure
         if metadata:
-            metadata_marple = [{'name': key, 'value': value} for key, value in metadata.items()]
-            r = self.session.post('{}/library/metadata'.format(self.api_url),
-                                  json={'source_id': source_id, 'metadata': metadata_marple})
-
-        plugin = self._guess_plugin(file_path)
-        body = {'path': path, 'plugin': plugin, 'config': config}
-        self.session.post('{}/library/file/import'.format(self.api_url), json=body)
+            r = self.post("/library/metadata", json={"source_id": source_id, "metadata": metadata})
+            if r.status_code != 200:
+                r.raise_for_status()
+
+        if plugin is None:
+            plugin = self._guess_plugin(file_path)
+        body = {"path": path, "plugin": plugin, "config": config}
+        self.post("/library/file/import", json=body)
+        if r.status_code != 200:
+            r.raise_for_status()
         return source_id
 
-    def upload_dataframe(self, dataframe, name, marple_folder, metadata={}):
-        file_name = f'{name}.csv'
-        dataframe.to_csv(file_name, sep=',', index=False)
+    def upload_dataframe(self, dataframe, name, marple_folder='/', metadata={}):
+        file_name = f"{name}.csv"
+        dataframe.to_csv(file_name, sep=",", index=False)
         source_id = self.upload_data_file(file_name, marple_folder, metadata=metadata)
         os.remove(file_name)
         return source_id
 
     def add_data(self, data_dict):
-        if self.data == {}:
-            self.data = {s: [v] for s, v in data_dict.items()}
+        if self._data == {}:
+            self._data = {s: [v] for s, v in data_dict.items()}
         else:
             for key in data_dict:
-                if key not in self.data:
-                    raise Exception(f'Key {key} not known in data.')
-                self.data[key].append(data_dict[key])
+                if key not in self._data:
+                    raise Exception(f"Key {key} not known in data.")
+                self._data[key].append(data_dict[key])
 
     def clear_data(self):
-        self.data = {}
+        self._data = {}
 
-    def send_data(self, name, marple_folder, metadata={}):
-        df = pd.DataFrame.from_dict(self.data)
+    def send_data(self, name, marple_folder='/', metadata={}):
+        df = pd.DataFrame.from_dict(self._data)
         self.clear_data()
-        return self.upload_dataframe(df, name, marple_folder, metadata={})
+        return self.upload_dataframe(df, name, marple_folder, metadata)
 
     def check_import_status(self, source_id):
-        r = self.session.get('{}/sources/status'.format(self.api_url), params={'id': source_id})
-        return r.json()['message'][0]['status']
+        r = self.get("/sources/status", params={"id": source_id})
+        if r.status_code != 200:
+            r.raise_for_status()
+        return r.json()["message"][0]["status"]
 
     def get_link(self, source_id, project_name, open_link=True):
         # make new share link
-        body = {'workbook_name': project_name, 'source_ids': [source_id]}
-        r = self.session.post('{}/library/share/new'.format(self.api_url), json=body)
-        share_id = r.json()['message']
+        body = {"workbook_name": project_name, "source_ids": [source_id]}
+        r = self.post("/library/share/new", json=body)
+        if r.status_code != 200:
+            r.raise_for_status()
+        share_id = r.json()["message"]
 
         # Generate clickable link in terminal
-        r = self.session.get('{}/library/share/{}/link'.format(self.api_url, share_id))
-        link = r.json()['message']
-        print('View your data: {}'.format(link))
+        r = self.get(f"/library/share/{share_id}/link")
+        if r.status_code != 200:
+            r.raise_for_status()
+        link = r.json()["message"]
+        if open_link:
+            webbrowser.open(link)
+        print(f"View your data: {link}")
         return link
 
     # Internal functions #
 
     def _guess_plugin(self, file_path):
-        extension = file_path.split('.')[0].lower()
+        extension = file_path.split(".")[-1].lower()
         if extension in self.plugin_map:
             return self.plugin_map[extension]
-        return 'csv_plugin'
+        return "csv_plugin"
```

### Comparing `marpledata-0.1.2/src/marpledata.egg-info/PKG-INFO` & `marpledata-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marpledata
-Version: 0.1.2
+Version: 0.1.3
 Summary: Marple SDK
 Author-email: Matthias Baert <support@marpledata.com>
 Project-URL: Homepage, https://www.marpledata.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -12,70 +12,86 @@
 License-File: LICENSE
 
 # Marple SDK
 
 A simple SDK to upload data to Marple
 
 ## Installation
+
 Install the Marple SDK using:
 
 `pip install marpledata`
 
 Import the package using:
 
 `import marple`
 
 ## Usage
+
 ### Setup
+
 Create a Marple connection using:
 
 ```python
 from marple import Marple
 m = Marple(ACCESS_TOKEN)
 ```
 
-You can find your personal access token in your account settings.
+You can generate access tokens in the app, under _Settings->Tokens_.
 
 If you are using Marple on-premise, you can add the custom URL:
 
 `m = Marple(ACCESS_TOKEN, api_url='https://marple.company.com/api/v1')`
 
 To check your connection, use:
 
 `m.check_connection()`
 
+### Calling endpoints
+
+Call endpoints by their METHOD:
+
+```python
+m.get('/version')
+m.post('/sources/info', json={'id': 98})
+```
+
 ### Upload data files
+
 If your data is already in a file format, use this function to upload the data to Marple.
 
-`source_id = m.upload_data_file(file_path, marple_folder, metadata={})`
+`source_id = m.upload_data_file(file_path, marple_folder='/', metadata={})`
 
 - `file_path`: the file_path of your data set
 - `marple_folder`: in what folder you would like to upload the data
 - `metadata`: dictionary with metadata. Example: `{'Pilot': 'John Doe'}'` Note that the metadata fields need to be added to your workspace before you will see them.
 
 ### Upload a dataframe
+
 If your data is in a pandas dataframe, use this function to upload the data to Marple.
 
-`source_id = m.upload_dataframe(dataframe, target_name, marple_folder, metadata={})`
+`source_id = m.upload_dataframe(dataframe, target_name, marple_folder='/', metadata={})`
 
 - `target_name`: the target name for the dataset, this is how it will appear in Marple.
 
 ### Add and send data
+
 You can also use the Marple SDK to add data piece by piece and send it to Marple.
 First use:
 
 `m.add_data(data_dict)`
 
 - `data_dict` = dictionary with signal, value pairs in it.
   Example: `{'time': 2, 'signal 1': 0, 'signal 2': 5}`
 
 Once all the data has been added, use:
 
 `source_id = m.send_data(target_name, marple_folder, metadata={})`
 
 ### Get a link to the data
+
 You can generate a link to Marple that opens the data and a project immediately. This can be very useful to see the results of a simulation directly.
 
 `link = m.get_link(source_id, project_name)`
 
 - `source_id`: identifier for the data set, is returned by all above functions.
 - `project_name`: name of the project that you want to open the data in.
```

### Comparing `marpledata-0.1.2/tests/test_SDK.py` & `marpledata-0.1.3/tests/test_SDK.py`

 * *Files identical despite different names*

