# Comparing `tmp/datarefiner_client-0.0.2.tar.gz` & `tmp/datarefiner_client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarefiner_client-0.0.2.tar", max compression
+gzip compressed data, was "datarefiner_client-0.0.3.tar", max compression
```

## Comparing `datarefiner_client-0.0.2.tar` & `datarefiner_client-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      907 2023-07-27 12:11:45.113217 datarefiner_client-0.0.2/README.md
--rw-r--r--   0        0        0      112 2023-07-27 12:42:30.245165 datarefiner_client-0.0.2/datarefiner_client/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 11:21:29.796050 datarefiner_client-0.0.2/datarefiner_client/api/__init__.py
--rw-r--r--   0        0        0      808 2023-07-19 14:18:24.527446 datarefiner_client-0.0.2/datarefiner_client/api/entities.py
--rw-r--r--   0        0        0     3296 2023-07-21 14:18:21.973807 datarefiner_client-0.0.2/datarefiner_client/api/supervised_labels.py
--rw-r--r--   0        0        0     1543 2023-07-24 11:53:38.465589 datarefiner_client-0.0.2/datarefiner_client/api/uploads.py
--rw-r--r--   0        0        0     4403 2023-07-25 13:16:50.415403 datarefiner_client-0.0.2/datarefiner_client/client.py
--rw-r--r--   0        0        0     1277 2023-07-24 11:25:22.677009 datarefiner_client-0.0.2/datarefiner_client/dataframe_uploader.py
--rw-r--r--   0        0        0      387 2023-07-24 11:05:07.712720 datarefiner_client-0.0.2/datarefiner_client/exceptions.py
--rw-r--r--   0        0        0      287 2023-07-25 13:15:37.886662 datarefiner_client-0.0.2/datarefiner_client/settings.py
--rw-r--r--   0        0        0      981 2023-07-27 12:42:22.593016 datarefiner_client-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1535 1970-01-01 00:00:00.000000 datarefiner_client-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      870 2023-08-07 19:19:47.149132 datarefiner_client-0.0.3/README.md
+-rw-r--r--   0        0        0      112 2023-08-08 21:18:05.761740 datarefiner_client-0.0.3/datarefiner_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 19:19:24.801470 datarefiner_client-0.0.3/datarefiner_client/api/__init__.py
+-rw-r--r--   0        0        0      808 2023-08-07 19:19:24.801470 datarefiner_client-0.0.3/datarefiner_client/api/entities.py
+-rw-r--r--   0        0        0     3644 2023-08-08 21:06:21.063031 datarefiner_client-0.0.3/datarefiner_client/api/supervised_labels.py
+-rw-r--r--   0        0        0     1543 2023-08-07 19:19:47.149132 datarefiner_client-0.0.3/datarefiner_client/api/uploads.py
+-rw-r--r--   0        0        0     4847 2023-08-08 21:06:21.063031 datarefiner_client-0.0.3/datarefiner_client/client.py
+-rw-r--r--   0        0        0     1277 2023-08-07 19:19:47.149132 datarefiner_client-0.0.3/datarefiner_client/dataframe_uploader.py
+-rw-r--r--   0        0        0      513 2023-08-08 21:06:21.063031 datarefiner_client-0.0.3/datarefiner_client/exceptions.py
+-rw-r--r--   0        0        0      287 2023-08-07 19:19:47.149132 datarefiner_client-0.0.3/datarefiner_client/settings.py
+-rw-r--r--   0        0        0      981 2023-08-08 21:18:19.301692 datarefiner_client-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 datarefiner_client-0.0.3/PKG-INFO
```

### Comparing `datarefiner_client-0.0.2/README.md` & `datarefiner_client-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 * Login using API key
 * Perform Supervised labelling (predict cluster labels and groups from trained toplogical project)
 
 ### Usage example: 
 ###
 
 ```
-    import pandas as pd
-    from datarefiner_client import DataRefinerClient
+import pandas as pd
+from datarefiner_client import DataRefinerClient
 
-	# Login using API key
-    client = DataRefinerClient(token='datarefiner_token',
-							   base_url='https://app.datarefiner.com')
-    client.me()
+# Login using API key
+client = DataRefinerClient(
+    token='datarefiner_token',
+    base_url='https://app.datarefiner.com',
+)
+client.me()
 
-	# Loading new data from CSV file
-    project_id = 2698269341
-    df = pd.read_csv("./data.csv")
-    
-    # Performig prediction for new data
-    clusters_df, groups_df = client.supervised_labeling(project_id=project_id, df=df)
+# Loading new data from CSV file
+project_id = 2698269341
+df = pd.read_csv("./data.csv")
+
+# Performig prediction for new data
+clusters_df, groups_df = client.supervised_labeling(project_id=project_id, df=df)
 ```
```

### Comparing `datarefiner_client-0.0.2/datarefiner_client/api/entities.py` & `datarefiner_client-0.0.3/datarefiner_client/api/entities.py`

 * *Files identical despite different names*

### Comparing `datarefiner_client-0.0.2/datarefiner_client/api/supervised_labels.py` & `datarefiner_client-0.0.3/datarefiner_client/api/supervised_labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,21 @@
         with self.session.post(
             url=self._supervised_labels_url.format(project_id=project_id), json={"upload_id": upload_id}
         ) as resp:
             if not resp.ok:
                 raise DatarefinerClientError(response=resp)
             return SupervisedLabel(**dict(resp.json(), upload_id=upload_id))
 
+    def supervised_labels_delete(self, project_id: int, supervised_label_id: int) -> None:
+        with self.session.delete(
+            url=urljoin(f"{self._supervised_labels_url.format(project_id=project_id)}/", str(supervised_label_id))
+        ) as resp:
+            if not resp.ok:
+                raise DatarefinerClientError(response=resp)
+
     def supervised_labels_check(self, project_id: int, supervised_label_id: int) -> None:
         with self.session.get(
             url=urljoin(f"{self._supervised_labels_url.format(project_id=project_id)}/", f"{supervised_label_id}/check")
         ) as resp:
             if not resp.ok:
                 raise DatarefinerClientError(response=resp)
```

### Comparing `datarefiner_client-0.0.2/datarefiner_client/api/uploads.py` & `datarefiner_client-0.0.3/datarefiner_client/api/uploads.py`

 * *Files identical despite different names*

### Comparing `datarefiner_client-0.0.2/datarefiner_client/client.py` & `datarefiner_client-0.0.3/datarefiner_client/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 import pandas as pd
 from progressbar import AnimatedMarker, ProgressBar
 from requests import Session
 
 from datarefiner_client.api.entities import SupervisedLabelStatus
 from datarefiner_client.api.supervised_labels import SupervisedLabelsEntrypoints
 from datarefiner_client.api.uploads import UploadsEntrypoints
-from datarefiner_client.exceptions import DatarefinerClientAuthError, DatarefinerClientError
+from datarefiner_client.exceptions import (
+    DatarefinerClientAuthError,
+    DatarefinerClientError,
+    DatarefinerSupervisedLabelingError,
+)
 from datarefiner_client.settings import API_BASE_URL, API_TOKEN
 
 
 def default_session_factory() -> Session:
     return Session()
 
 
@@ -74,16 +78,19 @@
             return resp.json()
 
     def supervised_labeling(self, project_id: int, df: pd.DataFrame) -> pd.DataFrame:
         upload = self.upload(df)
         pbar = ProgressBar(widgets=["Check dataframe: ", AnimatedMarker()]).start()
         supervised_label = self.supervised_labels_get_by_upload_id(project_id=project_id, upload_id=upload.id)
         pbar.update(pbar.currval + 1)
-        if not supervised_label:
+        if not supervised_label or supervised_label.status == SupervisedLabelStatus.ERROR:
             pbar.update(pbar.currval + 1)
+            if supervised_label:
+                self.supervised_labels_delete(project_id=project_id, supervised_label_id=supervised_label.id)
+                pbar.update(pbar.currval + 1)
             supervised_label = self.supervised_labels_create(project_id=project_id, upload_id=upload.id)
             pbar.update(pbar.currval + 1)
         if supervised_label.status == SupervisedLabelStatus.CHECKING:
             pbar.update(pbar.currval + 1)
             self.supervised_labels_check(project_id=project_id, supervised_label_id=supervised_label.id)
             pbar.update(pbar.currval + 1)
         pbar.finish()
@@ -92,14 +99,16 @@
             supervised_label := self.supervised_labels_get(
                 project_id=project_id, supervised_label_id=supervised_label.id
             )
         ).status not in (SupervisedLabelStatus.COMPLETE, SupervisedLabelStatus.ERROR):
             pbar.update(pbar.currval + 1)
             sleep(1)
         pbar.finish()
+        if supervised_label.status == SupervisedLabelStatus.ERROR:
+            raise DatarefinerSupervisedLabelingError(supervised_label.error)
         clusters_df: pd.DataFrame = pd.read_csv(
             BytesIO(self.supervised_labels_clusters(project_id=project_id, supervised_label_id=supervised_label.id))
         )
         groups_df: Optional[pd.DataFrame] = None
         if supervised_label.has_groups:
             groups_df = pd.read_csv(
                 BytesIO(self.supervised_labels_groups(project_id=project_id, supervised_label_id=supervised_label.id))
```

### Comparing `datarefiner_client-0.0.2/datarefiner_client/dataframe_uploader.py` & `datarefiner_client-0.0.3/datarefiner_client/dataframe_uploader.py`

 * *Files identical despite different names*

### Comparing `datarefiner_client-0.0.2/pyproject.toml` & `datarefiner_client-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datarefiner-client"
-version = "0.0.2"
+version = "0.0.3"
 description = "API client for Datarefiner"
 authors = ["Datarefiner <admin@datarefiner.com>"]
 readme = "README.md"
 packages = [{include = "datarefiner_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `datarefiner_client-0.0.2/PKG-INFO` & `datarefiner_client-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarefiner-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: API client for Datarefiner
 Author: Datarefiner
 Author-email: admin@datarefiner.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,23 +27,25 @@
 * Login using API key
 * Perform Supervised labelling (predict cluster labels and groups from trained toplogical project)
 
 ### Usage example: 
 ###
 
 ```
-    import pandas as pd
-    from datarefiner_client import DataRefinerClient
+import pandas as pd
+from datarefiner_client import DataRefinerClient
 
-	# Login using API key
-    client = DataRefinerClient(token='datarefiner_token',
-							   base_url='https://app.datarefiner.com')
-    client.me()
-
-	# Loading new data from CSV file
-    project_id = 2698269341
-    df = pd.read_csv("./data.csv")
-    
-    # Performig prediction for new data
-    clusters_df, groups_df = client.supervised_labeling(project_id=project_id, df=df)
+# Login using API key
+client = DataRefinerClient(
+    token='datarefiner_token',
+    base_url='https://app.datarefiner.com',
+)
+client.me()
+
+# Loading new data from CSV file
+project_id = 2698269341
+df = pd.read_csv("./data.csv")
+
+# Performig prediction for new data
+clusters_df, groups_df = client.supervised_labeling(project_id=project_id, df=df)
 ```
```

