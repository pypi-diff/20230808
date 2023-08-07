# Comparing `tmp/MicrosoftGraphAPI-0.0.1.tar.gz` & `tmp/MicrosoftGraphAPI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MicrosoftGraphAPI-0.0.1.tar", last modified: Wed May 31 19:33:52 2023, max compression
+gzip compressed data, was "MicrosoftGraphAPI-0.0.2.tar", last modified: Mon Aug  7 23:36:34 2023, max compression
```

## Comparing `MicrosoftGraphAPI-0.0.1.tar` & `MicrosoftGraphAPI-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:33:52.375214 MicrosoftGraphAPI-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-31 19:33:41.000000 MicrosoftGraphAPI-0.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:33:52.375214 MicrosoftGraphAPI-0.0.1/MicrosoftGraphAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-31 19:33:52.000000 MicrosoftGraphAPI-0.0.1/MicrosoftGraphAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-31 19:33:52.000000 MicrosoftGraphAPI-0.0.1/MicrosoftGraphAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:33:52.000000 MicrosoftGraphAPI-0.0.1/MicrosoftGraphAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 19:33:52.000000 MicrosoftGraphAPI-0.0.1/MicrosoftGraphAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 19:33:52.000000 MicrosoftGraphAPI-0.0.1/MicrosoftGraphAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-31 19:33:52.375214 MicrosoftGraphAPI-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-31 19:33:41.000000 MicrosoftGraphAPI-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:33:52.375214 MicrosoftGraphAPI-0.0.1/graphapi/
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-05-31 19:33:41.000000 MicrosoftGraphAPI-0.0.1/graphapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-31 19:33:41.000000 MicrosoftGraphAPI-0.0.1/graphapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:33:52.375214 MicrosoftGraphAPI-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-31 19:33:41.000000 MicrosoftGraphAPI-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:36:34.993106 MicrosoftGraphAPI-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 23:36:21.000000 MicrosoftGraphAPI-0.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:36:34.993106 MicrosoftGraphAPI-0.0.2/MicrosoftGraphAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-08-07 23:36:34.000000 MicrosoftGraphAPI-0.0.2/MicrosoftGraphAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-07 23:36:34.000000 MicrosoftGraphAPI-0.0.2/MicrosoftGraphAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 23:36:34.000000 MicrosoftGraphAPI-0.0.2/MicrosoftGraphAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-07 23:36:34.000000 MicrosoftGraphAPI-0.0.2/MicrosoftGraphAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 23:36:34.000000 MicrosoftGraphAPI-0.0.2/MicrosoftGraphAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-08-07 23:36:34.993106 MicrosoftGraphAPI-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-08-07 23:36:21.000000 MicrosoftGraphAPI-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:36:34.993106 MicrosoftGraphAPI-0.0.2/graphapi/
+-rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-08-07 23:36:21.000000 MicrosoftGraphAPI-0.0.2/graphapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-07 23:36:21.000000 MicrosoftGraphAPI-0.0.2/graphapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 23:36:34.993106 MicrosoftGraphAPI-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-08-07 23:36:21.000000 MicrosoftGraphAPI-0.0.2/setup.py
```

### Comparing `MicrosoftGraphAPI-0.0.1/LICENSE` & `MicrosoftGraphAPI-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MicrosoftGraphAPI-0.0.1/MicrosoftGraphAPI.egg-info/PKG-INFO` & `MicrosoftGraphAPI-0.0.2/MicrosoftGraphAPI.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MicrosoftGraphAPI
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package to interact with the Microsoft Graph API
 Home-page: https://www.adgstudios.co.za
 Author: Ashlin Darius Govindasamy
 Author-email: adg@adgstudios.co.za
 License: MIT
 Description: # GraphAPI
         
@@ -58,19 +58,23 @@
         search_results = api.search_for_file('keyword')
         
         # Delete a file or folder
         api.delete_file('file.txt', '/path/to/folder')
         
         # Generate a share link for a file
         share_link = api.create_share_link('file.txt', '/path/to/folder')
+        
+        # Download Filename from OneDrive
+        download_by_filename('foo.txt')
+        
         ```
         
         ## Contributing
         
-        Contributions are welcome! Please follow the guidelines in the CONTRIBUTING.md file.
+        Contributions are welcome! 
         
         ## License
         
         This project is licensed under the [MIT License](LICENSE).
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MicrosoftGraphAPI-0.0.1/PKG-INFO` & `MicrosoftGraphAPI-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MicrosoftGraphAPI
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package to interact with the Microsoft Graph API
 Home-page: https://www.adgstudios.co.za
 Author: Ashlin Darius Govindasamy
 Author-email: adg@adgstudios.co.za
 License: MIT
 Description: # GraphAPI
         
@@ -58,19 +58,23 @@
         search_results = api.search_for_file('keyword')
         
         # Delete a file or folder
         api.delete_file('file.txt', '/path/to/folder')
         
         # Generate a share link for a file
         share_link = api.create_share_link('file.txt', '/path/to/folder')
+        
+        # Download Filename from OneDrive
+        download_by_filename('foo.txt')
+        
         ```
         
         ## Contributing
         
-        Contributions are welcome! Please follow the guidelines in the CONTRIBUTING.md file.
+        Contributions are welcome! 
         
         ## License
         
         This project is licensed under the [MIT License](LICENSE).
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MicrosoftGraphAPI-0.0.1/README.md` & `MicrosoftGraphAPI-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -50,16 +50,20 @@
 search_results = api.search_for_file('keyword')
 
 # Delete a file or folder
 api.delete_file('file.txt', '/path/to/folder')
 
 # Generate a share link for a file
 share_link = api.create_share_link('file.txt', '/path/to/folder')
+
+# Download Filename from OneDrive
+download_by_filename('foo.txt')
+
 ```
 
 ## Contributing
 
-Contributions are welcome! Please follow the guidelines in the CONTRIBUTING.md file.
+Contributions are welcome! 
 
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
```

### Comparing `MicrosoftGraphAPI-0.0.1/graphapi/__init__.py` & `MicrosoftGraphAPI-0.0.2/graphapi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -262,19 +262,35 @@
         response = requests.get(
             endpoint, headers={'Authorization': 'Bearer ' + self.token})
         if response.status_code == 200:
             return True
         else:
             return False
 
+    def download_by_filename(self, filename):
+        endpoint = f'https://graph.microsoft.com/v1.0/users/{self.userid}/drive/root/search(q=\'{filename}\')'
+        response = requests.get(
+            endpoint, headers={'Authorization': 'Bearer ' + self.token})
+        result = response.json()
+        if 'value' in result:
+            file_id = result['value'][0]['id']
+            download_url = f'https://graph.microsoft.com/v1.0/users/{self.userid}/drive/items/{file_id}/content'
+            file_response = requests.get(download_url, headers={
+                                         'Authorization': 'Bearer ' + self.token})
+            if file_response.status_code == 200:
+                # Here, you can save the file to a location on your local system
+                with open(filename, 'wb') as f:
+                    f.write(file_response.content)
+                return f"File '{filename}' downloaded successfully."
+            else:
+                return f"Error downloading the file. Status code: {file_response.status_code}"
+        else:
+            return f"File '{filename}' not found in OneDrive."
+
 
 # Usage example:
 if __name__ == '__main__':
     appid = ''
     client_secret = ''
     tenant_id = ''
     userid = ''
-
     api = GraphAPI(appid, client_secret, tenant_id, userid)
-    api.get_information()
-    mail = api.get_mail()
-    print(mail)
```

### Comparing `MicrosoftGraphAPI-0.0.1/setup.py` & `MicrosoftGraphAPI-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     # metadata here
     name="MicrosoftGraphAPI",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version="0.0.1",
+    version="0.0.2",
     author="Ashlin Darius Govindasamy",
     author_email="adg@adgstudios.co.za",
     url="https://www.adgstudios.co.za",
     description="A Python package to interact with the Microsoft Graph API",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

