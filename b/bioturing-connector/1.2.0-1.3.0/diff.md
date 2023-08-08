# Comparing `tmp/bioturing-connector-1.2.0.tar.gz` & `tmp/bioturing-connector-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioturing-connector-1.2.0.tar", max compression
+gzip compressed data, was "bioturing-connector-1.3.0.tar", max compression
```

## Comparing `bioturing-connector-1.2.0.tar` & `bioturing-connector-1.3.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     4390 2022-10-11 16:34:14.735244 bioturing-connector-1.2.0/README.md
--rw-r--r--   0        0        0        0 2022-10-11 16:34:14.735376 bioturing-connector-1.2.0/bioturing_connector/__init__.py
--rw-r--r--   0        0        0      383 2023-03-05 03:05:20.458891 bioturing-connector-1.2.0/bioturing_connector/common/__init__.py
--rw-r--r--   0        0        0     4224 2023-04-21 15:38:26.637276 bioturing-connector-1.2.0/bioturing_connector/common/common.py
--rw-r--r--   0        0        0     1449 2023-03-05 03:05:20.460194 bioturing-connector-1.2.0/bioturing_connector/common/https_agent.py
--rw-r--r--   0        0        0    15367 2023-04-21 15:38:26.638203 bioturing-connector-1.2.0/bioturing_connector/connector.py
--rw-r--r--   0        0        0    11963 2023-04-21 15:38:26.638453 bioturing-connector-1.2.0/bioturing_connector/lens_connector.py
--rw-r--r--   0        0        0      347 2023-04-21 15:38:26.639452 bioturing-connector-1.2.0/bioturing_connector/typing/__init__.py
--rw-r--r--   0        0        0      444 2023-04-21 15:38:42.224041 bioturing-connector-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5379 1970-01-01 00:00:00.000000 bioturing-connector-1.2.0/setup.py
--rw-r--r--   0        0        0     5020 1970-01-01 00:00:00.000000 bioturing-connector-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4390 2022-10-11 16:34:14.735244 bioturing-connector-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2022-10-11 16:34:14.735376 bioturing-connector-1.3.0/bioturing_connector/__init__.py
+-rw-r--r--   0        0        0      383 2023-03-05 03:05:20.458891 bioturing-connector-1.3.0/bioturing_connector/common/__init__.py
+-rw-r--r--   0        0        0     4956 2023-08-08 16:05:33.373480 bioturing-connector-1.3.0/bioturing_connector/common/common.py
+-rw-r--r--   0        0        0     1449 2023-03-05 03:05:20.460194 bioturing-connector-1.3.0/bioturing_connector/common/https_agent.py
+-rw-r--r--   0        0        0    19277 2023-08-08 16:05:33.373810 bioturing-connector-1.3.0/bioturing_connector/connector.py
+-rw-r--r--   0        0        0    16868 2023-08-08 16:05:33.374082 bioturing-connector-1.3.0/bioturing_connector/lens_bulk_connector.py
+-rw-r--r--   0        0        0    12748 2023-08-08 16:05:33.374336 bioturing-connector-1.3.0/bioturing_connector/lens_sc_connector.py
+-rw-r--r--   0        0        0      614 2023-08-08 16:05:33.374596 bioturing-connector-1.3.0/bioturing_connector/typing/__init__.py
+-rw-r--r--   0        0        0      409 2023-08-08 16:06:36.447131 bioturing-connector-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5332 1970-01-01 00:00:00.000000 bioturing-connector-1.3.0/setup.py
+-rw-r--r--   0        0        0     4943 1970-01-01 00:00:00.000000 bioturing-connector-1.3.0/PKG-INFO
```

### Comparing `bioturing-connector-1.2.0/README.md` & `bioturing-connector-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bioturing-connector-1.2.0/bioturing_connector/common/common.py` & `bioturing-connector-1.3.0/bioturing_connector/common/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import time
-import requests
 import json
-from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
+import requests
+import pandas as pd
 from tqdm import tqdm
 from scipy import sparse
 from urllib.parse import urljoin
+from requests_toolbelt import MultipartEncoder
+from requests_toolbelt import MultipartEncoderMonitor
 
-from . import decode_base64_array
 from . import get_uuid
+from . import decode_base64_array
 from .https_agent import HttpsAgent
 
+
 def check_result_status(result):
   if not result:
     raise ConnectionError('Connection failed')
 
   if 'status' not in result:
     raise ValueError(result['detail'])
 
@@ -43,15 +46,14 @@
     return None
 
   return submission_status['data']['id']
 
 
 def get_submission_log(group_id: str, task_id: str, https_agent: HttpsAgent, host: str):
   last_status = []
-
   while True:
     submission_log = https_agent.post(
       url=urljoin(host, 'api/v1/get_submission_log'),
       body={'task_id': task_id}
     )
     if not submission_log or 'status' not in submission_log or \
       submission_log['status'] != 200:
@@ -76,24 +78,24 @@
           'group_id': group_id,
           'task_id': task_id
         }
       )
       if not res or 'status' not in res:
         print('Internal server error. Please check server log.')
         break
-
-      if res['status'] != 200:
+      elif res['status'] != 200:
         if 'message' in res:
           print(f"Connection failed. {res['message']}")
         else:
           print('Connection failed.')
         break
-
-      print('Study submitted successfully!')
-      break
+      else:
+        print('Study submitted successfully!')
+        return True
+  return False
 
 
 def parse_query_genes_result(query_genes_result):
   """Parse query genes result
   """
   check_result_status(query_genes_result)
 
@@ -137,8 +139,36 @@
         headers=headers
       ).json()
       if not response:
         raise Exception('Something went wrong')
       if 'status' not in response or response['status'] != 200:
         raise Exception(response)
       output_dir = response['data']
-  return output_dir
+  return output_dir
+
+
+def dataframe2dictionary(df):
+  res = dict()
+  res['barcodes'] = df.index.values
+  for column in df.columns:
+    res[column] = df.loc[:, column].values
+
+  for k in res:
+    try:
+      data = [int(x) for x in res[k]]
+    except:
+      data = [str(x) for x in res[k]]
+    res[k] = data
+  return res
+
+
+def read_csv(path, **kwargs):
+  df = pd.read_csv(filepath_or_buffer = path, sep='\t', **kwargs)
+
+  if 'index_col' in kwargs:
+    if len(df.columns) == 0:
+      return pd.read_csv(filepath_or_buffer = path, sep=',', **kwargs)
+  else:
+    if len(df.columns) < 2:
+      return pd.read_csv(filepath_or_buffer = path, sep=',', **kwargs)
+
+  return df
```

### Comparing `bioturing-connector-1.2.0/bioturing_connector/common/https_agent.py` & `bioturing-connector-1.3.0/bioturing_connector/common/https_agent.py`

 * *Files identical despite different names*

### Comparing `bioturing-connector-1.2.0/bioturing_connector/connector.py` & `bioturing-connector-1.3.0/bioturing_connector/connector.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,55 +20,24 @@
 class BBrowserXConnector:
   """Create a connector object to submit/get data from BBrowserX
   """
   def __init__(self, host: str, token: str, ssl: bool = True):
     """
       Args:
         host:
-          The URL of the BBrowserX server, only supports HTTPS connection
+          The URL of the BBrowserX server, only support HTTPS connection
           Example: https://bbrowserx.bioturing.com
         token:
           The API token to verify authority. Generated in-app.
     """
     self.__host = host
     self.__token = token
     self.__https_agent = HttpsAgent(self.__token, ssl)
 
 
-  def test_connection(self):
-    """Test the connection with the host
-    """
-    url = urljoin(self.__host, 'api/v1/test_connection')
-
-    print(f'Connecting to host at {url}')
-    res = self.__https_agent.post(url=url)
-    if res and 'status' in res and res['status'] == 200:
-      print('Connection successful')
-    else:
-      print('Connection failed')
-
-
-  def get_user_groups(self):
-    """
-      Get all the data sharing groups available for the current token
-      ------------------
-      Returns:
-        [{
-          'group_id': str (uuid),
-          'group_name': str
-        }, ...]
-    """
-    url = urljoin(self.__host, 'api/v1/get_user_groups')
-
-    res = self.__https_agent.post(url=url)
-    if res and 'status' in res and res['status'] == 200:
-      return res['data']
-    raise Exception('''Something went wrong, please contact support@bioturing.com''')
-
-
   def _submit_study(
     self,
     group_id: str,
     study_id: str = None,
     name: str = 'To be detailed',
     authors: List[str] = [],
     abstract: str = '',
@@ -121,58 +90,118 @@
       'normalize': input_matrix_type == InputMatrixType.RAW.value,
       'subsample': -1,
       'skip_dimred': skip_dimred,
       'study_info': study_info,
     }
 
 
+  def test_connection(self):
+    """Test the connection with the host
+    """
+    url = urljoin(self.__host, 'api/v1/test_connection')
+
+    print(f'Connecting to host at {url}')
+    res = self.__https_agent.post(url=url)
+    if res and 'status' in res and res['status'] == 200:
+      print('Connection successful')
+    else:
+      print('Connection failed')
+
+
+  def get_user_groups(self):
+    """
+      Get all the data sharing groups available for the current token
+      ------------------
+      Returns:
+        [{
+          'group_id': str (uuid),
+          'group_name': str
+        }, ...]
+    """
+    url = urljoin(self.__host, 'api/v1/get_user_groups')
+
+    res = self.__https_agent.post(url=url)
+    if res and 'status' in res and res['status'] == 200:
+      return res['data']
+    raise Exception('''Something went wrong, please contact support@bioturing.com''')
+
+
   def submit_study_from_s3(
     self,
     group_id: str,
     batch_info: List[dict] = [],
     study_id: str = None,
-    name: str = 'To be detailed',
+    name: str = 'This is my first study',
     authors: List[str] = [],
     abstract: str = '',
     species: str = Species.HUMAN.value,
     input_matrix_type: str = InputMatrixType.NORMALIZED.value,
     study_type: int = StudyType.H5AD.value,
     min_counts: int = None,
     min_genes: int = None,
     max_counts: int = None,
     max_genes: int = None,
     mt_percentage: Union[int, float] = None,
     skip_dimred: bool = False
   ):
-    """Submit one or multiple scanpy objects.
+    """
+      Submit one or multiple scanpy objects.
+
       Args:
-        group_id: ID of the group to submit the data to.
-        batch_info: File path and batch name information. Exp: [{"name: "normal": "s3_folder/batch1.h5ad"}, {"name": "cancer": "s3_folder/batch2.h5ad"}]
-        study_id: Study ID, if no value is specified, use a random uuidv4 string
-        name: Name of the study.
-        authors: Authors of the study.
-        abstract: Abstract of the study.
-        species: Species of the study.
-        skip_dirmed: Skip BioTuring pipline if set to True (only appliable when input is a scanpy/seurat object).
-        input_matrix_type: If the value of this input is 'normalized',
-          then the software will
-          use slot 'X' from the scanpy object and does not apply normalization.
-          If the value of this input is 'raw',then the software will
-          use slot 'raw.X' from thescanpy object and apply log-normalization.
-        study_type: The format of the study, supports: mtx, h5, h5ad, rds, tsv/csv.
-        min_counts: Minimum number of counts required
-          for a cell to pass filtering.
-        min_genes: Minimum number of genes expressed required
-          for a cell to pass filtering.
-        max_counts: Maximum number of counts required
-          for a cell to pass filtering.
-        max_genes: Maximum number of genes expressed required
-          for a cell to pass filtering.
-        mt_percentage: Maximum number of mitochondria genes percentage
-          required for a cell to pass filtering. Ranging from 0 to 100"""
+        group_id
+          ID of the group to submit the data to.
+        batch_info
+          File path and batch name information, the path should exclude bucket path!
+          Example:
+            For h5ad format:
+              [{
+                'matrix': 's3_path/GSE128223_1.h5ad'
+              }, {...}]
+            For mtx format:
+              [{
+                'matrix': 's3_path/data_1/matrix.mtx',
+                'features': 's3_path/data_1/features.tsv',
+                'barcodes': 's3_path/data_1/barcodes.tsv',
+              }, {...}]
+            For tiledb format:
+              [{
+                'folder': 's3_path/GSE128223_1'
+              }, {...}]
+        study_id
+          If no value is provided, default id will be a random uuidv4 string
+        name
+          Name of the study.
+        authors
+          Authors of the study.
+        abstract
+          Abstract of the study.
+        species
+          Species of the study.
+          Support: human, mouse, primate, others
+        skip_dirmed
+          Skip BioTuring pipline if set to True (only appliable when input is a scanpy/seurat object).
+        input_matrix_type
+          The input matrix is already normalized or not?
+          InputMatrixType.NORMALIZED.value: use slot 'X' from scanpy object and does not apply normalization.
+          InputMatrixType.RAW.value: use slot 'raw.X' from scanpy object and apply log-normalization.
+        study_type
+          The format of the study
+          Support: mtx, h5, h5ad, rds, tsv/csv, tile_db.
+        min_counts
+          Minimum number of counts required for a cell to pass filtering.
+        min_genes
+          Minimum number of genes expressed required for a cell to pass filtering.
+        max_counts
+          Maximum number of counts required for a cell to pass filtering.
+        max_genes
+          Maximum number of genes expressed required for a cell to pass filtering.
+        mt_percentage
+          Maximum number of mitochondria genes percentage required for a cell to pass filtering.
+          Ranging from 0 to 100
+    """
     data = self._submit_study(
       group_id,
       study_id,
       name,
       authors,
       abstract,
       species,
@@ -189,32 +218,35 @@
     if study_type == StudyType.MTX_10X.value:
       for i, o in enumerate(batch_info):
         name = o['matrix'].split('/')
         if len(name) == 1:
           o['name'] = f'Batch {i + 1}'
         else:
           o['name'] = name[-2]
+    elif study_type == StudyType.TILE_DB.value:
+      for i, o in enumerate(batch_info):
+        o['name'] = o['folder'].split('/')[-1]
     else:
       for i, o in enumerate(batch_info):
         o['name'] = o['matrix'].split('/')[-1]
+
     data['batch_info'] = {f'Batch_{i}': o for i, o in enumerate(batch_info)}
 
     submission_status = self.__https_agent.post(
       url=urljoin(self.__host, 'api/v1/submit_study_from_s3'),
       body=data
     )
 
     task_id = common.parse_submission_status(submission_status)
     if task_id is None:
-      return
+      return False
 
-    common.get_submission_log(
+    return common.get_submission_log(
       group_id=group_id, task_id=task_id, https_agent=self.__https_agent, host=self.__host
     )
-    return
 
 
   def submit_study_from_local(
     self,
     group_id: str,
     batch_info: object,
     study_id: str = None,
@@ -229,38 +261,64 @@
     max_counts: int = None,
     max_genes: int = None,
     mt_percentage: Union[int, float] = None,
     skip_dimred: bool = False
   ):
     """Submit one or multiple scanpy objects.
       Args:
-        group_id: ID of the group to submit the data to.
-        batch_info: File path and batch name information. Exp: [{"name: "normal": "local_folder/batch1.h5ad"}, {"name": "cancer": "local_folder/batch2.h5ad"}].
-        study_id: Study ID, if no value is specified, use a random uuidv4 string
-        name: Name of the study.
-        authors: Authors of the study.
-        abstract: Abstract of the study.
-        species: Species of the study.
-        skip_dirmed: Skip BioTuring pipline if set to True (only appliable when input is a scanpy/seurat object).
-        input_matrix_type: If the value of this input is 'normalized',
-          then the software will
-          use slot 'X' from the scanpy object and does not apply normalization.
-          If the value of this input is 'raw',then the software will
-          use slot 'raw.X' from thescanpy object and apply log-normalization.
-        study_type: The format of the study, supports: mtx, h5, h5ad, rds, tsv/csv.
-        min_counts: Minimum number of counts required
-          for a cell to pass filtering.
-        min_genes: Minimum number of genes expressed required
-          for a cell to pass filtering.
-        max_counts: Maximum number of counts required
-          for a cell to pass filtering.
-        max_genes: Maximum number of genes expressed required
-          for a cell to pass filtering.
-        mt_percentage: Maximum number of mitochondria genes percentage
-          required for a cell to pass filtering. Ranging from 0 to 100"""
+        group_id
+          ID of the group to submit the data to.
+        batch_info
+          File path and batch name information, the path should exclude bucket path!
+          Example:
+            For h5ad format:
+              [{
+                'matrix': 'local_path/GSE128223_1.h5ad'
+              }, {...}]
+            For mtx format:
+              [{
+                'name': 'data_1',
+                'matrix': 'local_path/data_1/matrix.mtx',
+                'features': 'local_path/data_1/features.tsv',
+                'barcodes': 'local_path/data_1/barcodes.tsv',
+              }, {...}]
+        study_id
+          If no value is provided, default id will be a random uuidv4 string
+        name
+          Name of the study.
+        authors
+          Authors of the study.
+        abstract
+          Abstract of the study.
+        species
+          Species of the study.
+          Support: human, mouse, primate, others
+        skip_dirmed
+          Skip BioTuring pipline if set to True (only appliable when input is a scanpy/seurat object).
+        input_matrix_type
+          The input matrix is already normalized or not?
+          InputMatrixType.NORMALIZED.value: use slot 'X' from scanpy object and does not apply normalization.
+          InputMatrixType.RAW.value: use slot 'raw.X' from scanpy object and apply log-normalization.
+        study_type
+          The format of the study
+          Support: mtx, h5, h5ad, rds, tsv/csv.
+        min_counts
+          Minimum number of counts required for a cell to pass filtering.
+        min_genes
+          Minimum number of genes expressed required for a cell to pass filtering.
+        max_counts
+          Maximum number of counts required for a cell to pass filtering.
+        max_genes
+          Maximum number of genes expressed required for a cell to pass filtering.
+        mt_percentage
+          Maximum number of mitochondria genes percentage required for a cell to pass filtering.
+          Ranging from 0 to 100
+    """
+    if study_type == StudyType.TILE_DB.value:
+      return 'tile_db submission is only supported through s3 or shared folder'
 
     file_names = []
     files = []
     if study_type == StudyType.MTX_10X.value:
       for o in batch_info:
         file_names.extend([
           f'{o["name"]}matrix.mtx{".gz" if ".gz" in o["matrix"] else ""}',
@@ -305,20 +363,22 @@
     submission_status = self.__https_agent.post(
       url=urljoin(self.__host, 'api/v1/submit_study_from_local'),
       body=data
     )
 
     task_id = common.parse_submission_status(submission_status)
     if task_id is None:
-      return
+      return False
 
-    common.get_submission_log(
-      group_id=group_id, task_id=task_id, https_agent=self.__https_agent, host=self.__host
+    return common.get_submission_log(
+      group_id=group_id,
+      task_id=task_id,
+      https_agent=self.__https_agent,
+      host=self.__host
     )
-    return
 
 
   def query_genes(
     self,
     species: str,
     study_id: str,
     gene_names: List[str],
@@ -516,15 +576,15 @@
   def retrieve_custom_embedding(
     self,
     species: str,
     study_id: str,
     embedding_id: str
   ):
     """
-      List out all custom embeddings in a study
+      Retrive custom embedding array in the study
       -------------
       Args:
         species: str,
           Name of species, 'human' or 'mouse' or 'primate'
         study_id: str,
           Study id (uuid)
         embedding_id: str,
@@ -541,8 +601,108 @@
     result = self.__https_agent.post(
       url=urljoin(self.__host, 'api/v1/retrieve_custom_embedding'),
       body=data
     )
     common.check_result_status(result)
     coord_arr = result['data']['coord_arr']
     coord_shape = result['data']['coord_shape']
-    return decode_base64_array(coord_arr, 'float32', coord_shape)
+    return decode_base64_array(coord_arr, 'float32', coord_shape)
+
+
+  def submit_metadata_from_dataframe(
+    self,
+    species: str,
+    study_id: str,
+    df: pd.DataFrame
+  ):
+    """
+      Submit metadata dataframe directly to platform
+      -------------
+      Args:
+        species: str,
+          Name of species, 'human' or 'mouse' or 'primate'
+        study_id: str,
+          Study id (uuid)
+        df: pandas DataFrame,
+          Barcodes must be in df.index!!!!
+      -------------
+      Returns
+        'Successful' or Error log
+    """
+    metadata_dct = common.dataframe2dictionary(df)
+    data = {
+      'species': species,
+      'study_id': study_id,
+      'metadata_dct': metadata_dct
+    }
+    result = self.__https_agent.post(
+      url=urljoin(self.__host, 'api/v1/submit_metadata_dataframe'),
+      body=data
+    )
+    common.check_result_status(result)
+    return 'Successful'
+
+
+  def submit_metadata_from_local(
+    self,
+    species: str,
+    study_id: str,
+    file_path: str
+  ):
+    """
+      Submit metadata to platform with local path
+      -------------
+      Args:
+        species: str,
+          Name of species, 'human' or 'mouse' or 'primate'
+        study_id: str,
+          Study id (uuid)
+        file_path: local path leading to metadata file,
+          Barcodes must be in the fist column
+          File suffix must be in .tsv/.csv
+      -------------
+      Returns
+        'Successful' or Error log
+    """
+    df = common.read_csv(file_path, index_col=0)
+    return self.submit_metadata_from_dataframe(
+      species,
+      study_id,
+      df
+    )
+
+
+  def submit_metadata_from_s3(
+    self,
+    species: str,
+    study_id: str,
+    file_path: str
+  ):
+    """
+      Submit metadata to platform with s3 path
+      -------------
+      Args:
+        species: str,
+          Name of species, 'human' or 'mouse' or 'primate'
+        study_id: str,
+          Study id (uuid)
+        file_path: path in s3 bucket leading to metadata file,
+          Barcodes must be in the fist column
+          File suffix must be in .tsv/.csv
+          File_path SHOULD NOT contain s3_bucket path configured in the platform
+              E.g. realpath: 's3://bucket/folder/metadata.tsv'
+                  inputpath: 'folder/metadata.tsv'
+      -------------
+      Returns
+        'Successful' or Error log
+    """
+    data = {
+      'species': species,
+      'study_id': study_id,
+      'file_path': file_path
+    }
+    result = self.__https_agent.post(
+      url=urljoin(self.__host, 'api/v1/submit_metadata_s3'),
+      body=data
+    )
+    common.check_result_status(result)
+    return 'Successful'
```

### Comparing `bioturing-connector-1.2.0/bioturing_connector/lens_connector.py` & `bioturing-connector-1.3.0/bioturing_connector/lens_sc_connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-"""Python package for submitting/getting data from BBrowserX"""
+"""Python package for submitting/getting data from Lens SC"""
 
 import pandas as pd
-from pathlib import Path
 
-from urllib.parse import urljoin
 from typing import List
+from pathlib import Path
+from urllib.parse import urljoin
 
 from .common import decode_base64_array
 from .common import get_uuid
 
 from .common.https_agent import HttpsAgent
 from .common import common
 from .typing import Species
 from .typing import StudyType
+from .typing import TechnologyType
 from .typing import UNIT_RAW
 
-class LensBulkConnector:
-  """Create a connector object to submit/get data from BioTuring Lens (Visium/GeoMx DSP)
+
+class LensSCConnector:
+  """
+  	Create a connector object to submit/get data from BioTuring Lens Single-cell
+  	(Xenium/Cosmx/Vizgen/Proteomics)
   """
   def __init__(self, host: str, token: str, ssl: bool = True):
     """
       Args:
         host:
           The URL of the BioTuring Lens server, only supports HTTPS connection
-          Example: https://lens.bioturing.com
+          Example: https://lens_sc.bioturing.com
         token:
           The API token to verify authority. Generated in-app.
     """
     self.__host = host
     self.__token = token
     self.__https_agent = HttpsAgent(self.__token, ssl)
 
@@ -67,15 +71,16 @@
     self,
     group_id: str,
     study_id: str = None,
     name: str = 'To be detailed',
     authors: List[str] = [],
     abstract: str = '',
     species: str = Species.HUMAN.value,
-    study_type: int = StudyType.VISIUM.value,
+    study_type: int = StudyType.XENIUM.value,
+    technology_type: str = TechnologyType.LENS_SC.value
   ):
     if study_id is None:
       study_id = get_uuid()
 
     study_info = {
       'study_hash_id': study_id,
       'name': name,
@@ -89,151 +94,94 @@
       'filter_params': {
         'min_counts': 0,
         'min_genes': 0,
         'max_counts': 1e9,
         'max_genes': 1e9,
         'mt_percentage': 1,
       },
-      'study_type': study_type,
-      'normalize': True,
-      'subsample': -1,
+      'study_type': technology_type,
+      'platform': study_type,
       'study_info': study_info,
     }
 
 
   def submit_study_from_s3(
     self,
     group_id: str,
     batch_info: List[dict] = [],
     study_id: str = None,
     name: str = 'To be detailed',
     authors: List[str] = [],
     abstract: str = '',
     species: str = Species.HUMAN.value,
-    study_type: int = StudyType.DSP.value,
+    study_type: int = StudyType.XENIUM.value,
+    technology_type: str = TechnologyType.LENS_SC.value
   ):
-    """Submit one or multiple scanpy objects.
-      Args:
-        group_id: ID of the group to submit the data to.
-        batch_info: File path and batch name information. Exp: [{"name: "normal", "matrix": "s3_folder/batch1/matrix.xlsx", "image": "s3_folder/batch1/image.ome.tiff"}].
-        study_id: Study ID, if no value is specified, use a random uuidv4 string
-        name: Name of the study.
-        authors: Authors of the study.
-        abstract: Abstract of the study.
-        species: Species of the study.
-        study_type: The format of the study, supports: Visium, GeoMx DSP."""
-    data = self._submit_study(
-      group_id,
-      study_id,
-      name,
-      authors,
-      abstract,
-      species,
-      study_type
-    )
-    for i, o in enumerate(batch_info):
-      name = o['matrix'].split('/')
-      if len(name) == 1:
-        o['name'] = f'Batch {i + 1}'
-      else:
-        o['name'] = name[-2]
-    data['batch_info'] = {f'Batch_{i}': o for i, o in enumerate(batch_info)}
-
-    submission_status = self.__https_agent.post(
-      url=urljoin(self.__host, 'api/v1/submit_study_from_s3'),
-      body=data
-    )
-
-    task_id = common.parse_submission_status(submission_status)
-    if task_id is None:
-      return
-
-    common.get_submission_log(
-      group_id=group_id, task_id=task_id, https_agent=self.__https_agent, host=self.__host
-    )
-    return
-
+    """
+      Submit one (Proteomics) or multiple data (Lens SC) folders.
 
-  def submit_study_from_local(
-    self,
-    group_id: str,
-    batch_info: object,
-    study_id: str = None,
-    name: str = 'To be detailed',
-    authors: List[str] = [],
-    abstract: str = '',
-    species: str = Species.HUMAN.value,
-    study_type: int = StudyType.DSP.value,
-  ):
-    """Submit one or multiple scanpy objects.
       Args:
-        group_id: ID of the group to submit the data to.
-        batch_info: File path and batch name information. Exp: [{"name: "normal", "matrix": "local_folder/batch1/matrix.xlsx", "image": "local_folder/batch1/image.ome.tiff"}].
-        study_id: Study ID, if no value is specified, use a random uuidv4 string
-        name: Name of the study.
-        authors: Authors of the study.
-        abstract: Abstract of the study.
-        species: Species of the study.
-        study_type: The format of the study, supports: Visium, GeoMx DSP."""
-
-    file_names = []
-    files = []
-    if study_type == StudyType.VISIUM.value:
-      for o in batch_info:
-        file_names.extend([
-          f'{o["name"]}matrix.h5',
-          f'{o["name"]}image.{o["image"].split(".")[-1]}',
-          f'{o["name"]}position.{o["position"].split(".")[-1]}',
-          f'{o["name"]}scale.json',
-        ])
-        files.extend([
-          Path(o['matrix']),
-          Path(o['image']),
-          Path(o['position']),
-          Path(o['scale']),
-        ])
-    elif study_type == StudyType.DSP.value:
-      for o in batch_info:
-        file_names.extend([
-          f'{o["name"]}matrix.xlsx',
-          f'{o["name"]}image.tiff',
-        ])
-        files.extend([
-          Path(o['matrix']),
-          Path(o['image']),
-        ])
-
-    output_dir = common.upload_local(
-      file_names, files, group_id, study_type, self.__token, self.__host
-    )
+        group_id
+          ID of the group to submit the data to.
+        batch_info
+          File path and batch name information, the path should exclude bucket path!
+          Example:
+            For LENS_SC format:
+              [{
+                'name': 'study_1',
+                'folder': 's3_path/study_folder',
+              }, {...}]
+            For PROTEOMICS format:
+              [{
+								'name': 'study_1'
+                'image': 's3_path/image.ome.tiff'
+              }, {...}]
+        study_id
+          If no value is provided, default id will be a random uuidv4 string
+        name
+          Name of the study.
+        authors
+          Authors of the study.
+        abstract
+          Abstract of the study.
+        species
+          Species of the study.
+          Support: human, mouse, primate, others
+        study_type:
+          The format of the study
+          Support: Xenium/Vizgen/Cosmx/Proteomics(mass cytometry, akoya, ...).
+        technology_type:
+					Technology type of the study
+          Support:	TechnologyType.LENS_SC.value
+										TechnologyType.PROTEOMICS.value
+      """
     data = self._submit_study(
       group_id,
       study_id,
       name,
       authors,
       abstract,
       species,
       study_type,
+      technology_type
     )
-    data['study_path'] = output_dir
-    data['batch_info'] = [o['name'] for o in batch_info]
+    data['batch_info'] = {o['name']: o for o in batch_info}
 
     submission_status = self.__https_agent.post(
-      url=urljoin(self.__host, 'api/v1/submit_study_from_local'),
+      url=urljoin(self.__host, 'api/v1/submit_study_from_s3'),
       body=data
     )
 
     task_id = common.parse_submission_status(submission_status)
     if task_id is None:
-      return
+      return False
 
-    common.get_submission_log(
+    return common.get_submission_log(
       group_id=group_id, task_id=task_id, https_agent=self.__https_agent, host=self.__host
     )
-    return
 
 
   def query_genes(
     self,
     species: str,
     study_id: str,
     gene_names: List[str],
@@ -431,15 +379,15 @@
   def retrieve_custom_embedding(
     self,
     species: str,
     study_id: str,
     embedding_id: str
   ):
     """
-      List out all custom embeddings in a study
+      Retrive custom embedding array in the study
       -------------
       Args:
         species: str,
           Name of species, 'human' or 'mouse' or 'primate'
         study_id: str,
           Study id (uuid)
         embedding_id: str,
@@ -456,8 +404,108 @@
     result = self.__https_agent.post(
       url=urljoin(self.__host, 'api/v1/retrieve_custom_embedding'),
       body=data
     )
     common.check_result_status(result)
     coord_arr = result['data']['coord_arr']
     coord_shape = result['data']['coord_shape']
-    return decode_base64_array(coord_arr, 'float32', coord_shape)
+    return decode_base64_array(coord_arr, 'float32', coord_shape)
+
+
+  def submit_metadata_from_dataframe(
+    self,
+    species: str,
+    study_id: str,
+    df: pd.DataFrame
+  ):
+    """
+      Submit metadata dataframe directly to platform
+      -------------
+      Args:
+        species: str,
+          Name of species, 'human' or 'mouse' or 'primate'
+        study_id: str,
+          Study id (uuid)
+        df: pandas DataFrame,
+          Barcodes must be in df.index!!!!
+      -------------
+      Returns
+        'Successful' or Error log
+    """
+    metadata_dct = common.dataframe2dictionary(df)
+    data = {
+      'species': species,
+      'study_id': study_id,
+      'metadata_dct': metadata_dct
+    }
+    result = self.__https_agent.post(
+      url=urljoin(self.__host, 'api/v1/submit_metadata_dataframe'),
+      body=data
+    )
+    common.check_result_status(result)
+    return 'Successful'
+
+
+  def submit_metadata_from_local(
+    self,
+    species: str,
+    study_id: str,
+    file_path: str
+  ):
+    """
+      Submit metadata to platform with local path
+      -------------
+      Args:
+        species: str,
+          Name of species, 'human' or 'mouse' or 'primate'
+        study_id: str,
+          Study id (uuid)
+        file_path: local path leading to metadata file,
+          Barcodes must be in the fist column
+          File suffix must be in .tsv/.csv
+      -------------
+      Returns
+        'Successful' or Error log
+    """
+    df = common.read_csv(file_path, index_col=0)
+    return self.submit_metadata_from_dataframe(
+      species,
+      study_id,
+      df
+    )
+
+
+  def submit_metadata_from_s3(
+    self,
+    species: str,
+    study_id: str,
+    file_path: str
+  ):
+    """
+      Submit metadata to platform with s3 path
+      -------------
+      Args:
+        species: str,
+          Name of species, 'human' or 'mouse' or 'primate'
+        study_id: str,
+          Study id (uuid)
+        file_path: path in s3 bucket leading to metadata file,
+          Barcodes must be in the fist column
+          File suffix must be in .tsv/.csv
+          file_path SHOULD NOT contain s3_bucket path configured in the platform
+              E.g.  realpath: 's3://bucket/folder/metadata.tsv'
+                    file_path: 'folder/metadata.tsv'
+      -------------
+      Returns
+        'Successful' or Error log
+    """
+    data = {
+      'species': species,
+      'study_id': study_id,
+      'file_path': file_path
+    }
+    result = self.__https_agent.post(
+      url=urljoin(self.__host, 'api/v1/submit_metadata_s3'),
+      body=data
+    )
+    common.check_result_status(result)
+    return 'Successful'
```

### Comparing `bioturing-connector-1.2.0/setup.py` & `bioturing-connector-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,19 @@
  'bioturing_connector.common',
  'bioturing_connector.typing']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['mypy>=0.982,<0.983', 'pylint>=2.15.3,<3.0.0', 'requests>=2.28.1,<3.0.0']
+['requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'bioturing-connector',
-    'version': '1.2.0',
+    'version': '1.3.0',
     'description': 'A set of python modules for accessing BBrowserX on private server',
     'long_description': '## 1. Installation:\n```\n  pip install bioturing_connector --index-url=https://pypi.bioturing.com\n\n  # Username: bioturing\n  # Password: code@bioturing.com\n```\n\n## 2. Usage:\n**The package only allows data submission via Amazon S3 Bucket. Please configure your S3 Bucket credentials in the `Settings` page.**\n### 2.1. Test the connection:\n```\n# example.py\n\nfrom bioturing_connector.connector import BBrowserXConnector\n\nconnector = BBrowserXConnector(\n  host="https://yourcompany/t2d_index_tool/,\n  token="<input your token here>"\n)\n\nconnector.test_connection()\n```\n\nExample output:\n\n```\nConnecting to host at https://yourcompany/t2d_index_tool/api/v1/test_connection\nConnection successful\n```\n\n### 2.2. Get user groups available for your token:\n```\n# example.py\n\nfrom bioturing_connector.connector import BBrowserXConnector\n\nconnector = BBrowserXConnector(\n  host="https://yourcompany/t2d_index_tool/,\n  token="<input your token here>"\n)\n\nuser_groups = connector.get_user_groups()\nprint(user_groups)\n```\n\nExample output:\n\n```\n[{\'id\': \'all_members\', \'name\': \'All members\'}, {\'id\': \'personal\', \'name\': \'Personal workspace\'}]\n```\n\n### 2.3. Submit h5ad (scanpy object):\n```\n# example.py\nfrom bioturing_connector.connector import BBrowserXConnector\nfrom bioturing_connector.typing import InputMatrixType\nfrom bioturing_connector.typing import Species\n\nconnector = BBrowserXConnector(\n  host="https://yourcompany/t2d_index_tool/,\n  token="<input your token here>"\n)\n\n# Call this function first to get available groups and their id.\nuser_groups = connector.get_user_groups()\n# Example: user_groups is now [{\'id\': \'all_members\', \'name\': \'All members\'}, {\'id\': \'personal\', \'name\': \'Personal workspace\'}]\n\n\n# Submitting the scanpy object:\nconnector.submit_h5ad(\n  group_id=\'personal\',\n  study_s3_keys=[\'GSE128223.h5ad\'],\n  study_id=\'GSE128223\',\n  name=\'This is my first study\',\n  authors=[\'Huy Nguyen\'],\n  species=Species.HUMAN.value,\n  input_matrix_type=InputMatrixType.RAW.value\n)\n\n# Example output:\n> [2022-10-10 01:03] Waiting in queue\n> [2022-10-10 01:03] Downloading GSE128223.h5ad from s3: 262.1 KB / 432.8 MB\n> [2022-10-10 01:03] File downloaded\n> [2022-10-10 01:03] Reading batch: GSE128223.h5ad\n> [2022-10-10 01:03] Preprocessing expression matrix: 19121 cells x 63813 genes\n> [2022-10-10 01:03] Filtered: 19121 cells remain\n> [2022-10-10 01:03] Start processing study\n> [2022-10-10 01:03] Normalizing expression matrix\n> [2022-10-10 01:03] Running PCA\n> [2022-10-10 01:03] Running kNN\n> [2022-10-10 01:03] Running spectral embedding\n> [2022-10-10 01:03] Running venice binarizer\n> [2022-10-10 01:04] Running t-SNE\n> [2022-10-10 01:04] Study was successfully submitted\n> [2022-10-10 01:04] DONE !!!\n> Study submitted successfully!\n```\nAvailable parameters for `submit_h5ad` function:\n```\ngroup_id: str\n  ID of the group to submit the data to.\n\nstudy_s3_keys: List[str]\n  List of the s3 key of the studies.\n\nstudy_id: str, default=None\n  Study ID, if no value is specified, use a random uuidv4 string\n\nname: str, default=\'To be detailed\'\n  Name of the study.\n\nauthors: List[str], default=[]\n  Authors of the study.\n\nabstract: str, default=\'\'\n  Abstract of the study.\n\nspecies: str, default=\'human\'\n  Species of the study. Can be: **bioturing_connector.typing.Species.HUMAN.value** or **bioturing_connector.typing.Species.MOUSE.value** or **bioturing_connector.typing.Species.NON_HUMAN_PRIMATE.value**\n\ninput_matrix_type: str, default=\'raw\'\n  If the value of this input is **bioturing_connector.typing.InputMatrixType.NORMALIZED.value**,\n  then the software will\n  use slot \'X\' from the scanpy object and does not apply normalization.\n  If the value of this input is **bioturing_connector.typing.InputMatrixType.RAW.value**,then the software will\n  use slot \'raw.X\' from thescanpy object and apply log-normalization.\n\nmin_counts: int, default=None\n  Minimum number of counts required\n  for a cell to pass filtering.\n\nmin_genes: int, default=None\n  Minimum number of genes expressed required\n  for a cell to pass filtering.\n\nmax_counts: int, default=None\n  Maximum number of counts required\n  for a cell to pass filtering.\n\nmax_genes: int, default=None\n  Maximum number of genes expressed required\n  for a cell to pass filtering.\n\nmt_percentage: Union[int, float], default=None\n  Maximum number of mitochondria genes percentage\n  required for a cell to pass filtering. Ranging from 0 to 100\n```\n',
     'author': 'BioTuring',
     'author_email': 'support@bioturing.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bioturing-connector-1.2.0/PKG-INFO` & `bioturing-connector-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: bioturing-connector
-Version: 1.2.0
+Version: 1.3.0
 Summary: A set of python modules for accessing BBrowserX on private server
 Author: BioTuring
 Author-email: support@bioturing.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: mypy (>=0.982,<0.983)
-Requires-Dist: pylint (>=2.15.3,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 ## 1. Installation:
 ```
   pip install bioturing_connector --index-url=https://pypi.bioturing.com
```

