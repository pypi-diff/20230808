# Comparing `tmp/yastas-data-0.3.6.tar.gz` & `tmp/yastas-data-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yastas-data-0.3.6.tar", last modified: Tue Jul 18 19:43:42 2023, max compression
+gzip compressed data, was "yastas-data-0.3.7.tar", last modified: Mon Aug  7 22:10:17 2023, max compression
```

## Comparing `yastas-data-0.3.6.tar` & `yastas-data-0.3.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 19:43:42.706694 yastas-data-0.3.6/
--rw-rw-rw-   0        0        0      607 2023-07-18 19:43:42.693255 yastas-data-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      181 2023-07-17 22:01:49.000000 yastas-data-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 19:43:42.421548 yastas-data-0.3.6/data_code/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:24:11.000000 yastas-data-0.3.6/data_code/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 19:43:42.462983 yastas-data-0.3.6/data_code/beam/
--rw-rw-rw-   0        0        0        0 2023-07-10 19:17:14.000000 yastas-data-0.3.6/data_code/beam/__init__.py
--rw-rw-rw-   0        0        0     2384 2023-07-18 19:42:13.000000 yastas-data-0.3.6/data_code/beam/database.py
--rw-rw-rw-   0        0        0      919 2023-07-18 19:39:49.000000 yastas-data-0.3.6/data_code/beam/processing.py
-drwxrwxrwx   0        0        0        0 2023-07-18 19:43:42.564856 yastas-data-0.3.6/data_code/gcp/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:34:31.000000 yastas-data-0.3.6/data_code/gcp/__init__.py
--rw-rw-rw-   0        0        0     1684 2023-07-07 18:59:37.000000 yastas-data-0.3.6/data_code/gcp/bq.py
--rw-rw-rw-   0        0        0      416 2023-06-26 22:44:12.000000 yastas-data-0.3.6/data_code/gcp/secrets.py
--rw-rw-rw-   0        0        0        0 2023-06-23 22:17:23.000000 yastas-data-0.3.6/data_code/gcp/service_account.py
--rw-rw-rw-   0        0        0     2394 2023-07-18 19:42:35.000000 yastas-data-0.3.6/data_code/gcp/sql.py
--rw-rw-rw-   0        0        0       43 2023-06-21 19:52:01.000000 yastas-data-0.3.6/data_code/gcp/storage.py
-drwxrwxrwx   0        0        0        0 2023-07-18 19:43:42.616246 yastas-data-0.3.6/data_code/parquets/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:30:05.000000 yastas-data-0.3.6/data_code/parquets/__init__.py
--rw-rw-rw-   0        0        0      490 2023-06-27 22:57:11.000000 yastas-data-0.3.6/data_code/parquets/get_schema.py
--rw-rw-rw-   0        0        0      637 2023-07-17 21:57:17.000000 yastas-data-0.3.6/data_code/parquets/parquet2csv.py
--rw-rw-rw-   0        0        0       42 2023-07-18 19:43:42.707699 yastas-data-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      700 2023-07-18 19:43:24.000000 yastas-data-0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 19:43:42.681097 yastas-data-0.3.6/yastas_data.egg-info/
--rw-rw-rw-   0        0        0      607 2023-07-18 19:43:41.000000 yastas-data-0.3.6/yastas_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2023-07-18 19:43:42.000000 yastas-data-0.3.6/yastas_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 19:43:41.000000 yastas-data-0.3.6/yastas_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-18 19:43:41.000000 yastas-data-0.3.6/yastas_data.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 22:10:17.026888 yastas-data-0.3.7/
+-rw-rw-rw-   0        0        0      607 2023-08-07 22:10:17.013921 yastas-data-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2023-07-17 22:01:49.000000 yastas-data-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 22:10:16.756760 yastas-data-0.3.7/data_code/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:24:11.000000 yastas-data-0.3.7/data_code/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 22:10:16.803002 yastas-data-0.3.7/data_code/beam/
+-rw-rw-rw-   0        0        0        0 2023-07-10 19:17:14.000000 yastas-data-0.3.7/data_code/beam/__init__.py
+-rw-rw-rw-   0        0        0     2384 2023-07-18 19:42:13.000000 yastas-data-0.3.7/data_code/beam/database.py
+-rw-rw-rw-   0        0        0      919 2023-07-18 19:39:49.000000 yastas-data-0.3.7/data_code/beam/processing.py
+drwxrwxrwx   0        0        0        0 2023-08-07 22:10:16.889931 yastas-data-0.3.7/data_code/gcp/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:34:31.000000 yastas-data-0.3.7/data_code/gcp/__init__.py
+-rw-rw-rw-   0        0        0     2439 2023-08-07 22:06:19.000000 yastas-data-0.3.7/data_code/gcp/bq.py
+-rw-rw-rw-   0        0        0      416 2023-06-26 22:44:12.000000 yastas-data-0.3.7/data_code/gcp/secrets.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 22:17:23.000000 yastas-data-0.3.7/data_code/gcp/service_account.py
+-rw-rw-rw-   0        0        0     2394 2023-07-18 19:42:35.000000 yastas-data-0.3.7/data_code/gcp/sql.py
+-rw-rw-rw-   0        0        0      486 2023-08-03 22:46:20.000000 yastas-data-0.3.7/data_code/gcp/storage.py
+drwxrwxrwx   0        0        0        0 2023-08-07 22:10:16.940882 yastas-data-0.3.7/data_code/parquets/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:30:05.000000 yastas-data-0.3.7/data_code/parquets/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-06-27 22:57:11.000000 yastas-data-0.3.7/data_code/parquets/get_schema.py
+-rw-rw-rw-   0        0        0      637 2023-07-17 21:57:17.000000 yastas-data-0.3.7/data_code/parquets/parquet2csv.py
+-rw-rw-rw-   0        0        0       42 2023-08-07 22:10:17.027919 yastas-data-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-08-07 22:10:08.000000 yastas-data-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 22:10:17.004000 yastas-data-0.3.7/yastas_data.egg-info/
+-rw-rw-rw-   0        0        0      607 2023-08-07 22:10:16.000000 yastas-data-0.3.7/yastas_data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2023-08-07 22:10:16.000000 yastas-data-0.3.7/yastas_data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 22:10:16.000000 yastas-data-0.3.7/yastas_data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-07 22:10:16.000000 yastas-data-0.3.7/yastas_data.egg-info/top_level.txt
```

### Comparing `yastas-data-0.3.6/PKG-INFO` & `yastas-data-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: yastas-data
-Version: 0.3.6
+Version: 0.3.7
 Summary: Paquete distribuible en repositorio de funciones locales
 Home-page: https://bitbucket.org/gentera-insumos/data-code
 Author: Data - Aaron
 Author-email: e-ajuareza@minsait.com
 License: MIT
 Description: # InstalaciÃ³n
```

### Comparing `yastas-data-0.3.6/data_code/beam/database.py` & `yastas-data-0.3.7/data_code/beam/database.py`

 * *Files identical despite different names*

### Comparing `yastas-data-0.3.6/data_code/beam/processing.py` & `yastas-data-0.3.7/data_code/beam/processing.py`

 * *Files identical despite different names*

### Comparing `yastas-data-0.3.6/data_code/gcp/bq.py` & `yastas-data-0.3.7/data_code/gcp/bq.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,52 @@
 from google.cloud import bigquery
 from google.cloud.exceptions import NotFound
 import ast
 import subprocess
 
-def create_or_evaluate_bq_table(table_id:str,raw_parquet:str)->dict:
-    """Verifica si existe la tabla y extrae los metadatos; en caso de que no exista la crea con base en el parquet de raw.
+def create_or_evaluate_bq_table(table_id:str,trn_parquet:str, delete_columns:str)->dict:
+        """Verifica si existe la tabla y extrae los metadatos; en caso de que no exista la crea con base en el parquet de raw.
 
-    Args:
-        table (str): Nombre de la tabla.
-        raw_parquet (str): Ruta del parquet.
-
-    Returns:
-        dict: Diccionario con la metadata de la tabla.
-    """
-    try:
-        client = bigquery.Client()
-        client.get_table(table_id.replace(':','.'))  # Make an API request.
-        print(f"Table: {table_id} already exists.")
-        metadata_table_bq = get_metadata(table_id)
-        return metadata_table_bq
-    except NotFound:
-        print(f"Table: {table_id} not found. \nCreating it with parquet: {raw_parquet}")
-        #TODO: bq load --autodetect --source_format=PARQUET <project_id>:<dataset>.<table_name> gs://<bucket_name>/<path_to_parquet_file>
-        subprocess.run(["bq","load","--autodetect", "--source_format=PARQUET", table_id, raw_parquet], capture_output=True, shell=True).stdout
-        print(f'{table_id} was created succesfully')
-        metadata_table_bq = get_metadata(table_id)
-        return metadata_table_bq
+        Args:
+            table (str): Nombre de la tabla.
+            raw_parquet (str): Ruta del parquet.
+
+        Returns:
+            dict: Diccionario con la metadata de la tabla.
+        """
+        try:
+            client = bigquery.Client()
+            client.get_table(table_id.replace(':','.'))  # Make an API request.
+            print(f"Table: {table_id} already exists.")
+            metadata_table_bq = get_metadata(table_id)
+            return metadata_table_bq
+        except NotFound:
+            print(f"Table: {table_id} not found. \nCreating it with parquet: {trn_parquet}")
+            subprocess.run(["bq","load","--autodetect", "--source_format=PARQUET", table_id, trn_parquet], capture_output=True, shell=True).stdout
+            print(f'{table_id} was created succesfully')
+            metadata_table_bq = get_metadata(table_id)
+            if delete_columns != "[]":
+                print("Erasing columns")
+                delete_columns_processed = ast.literal_eval(delete_columns.replace('"',''))   
+                delete_columns_table(table_id,delete_columns_processed)
+                print(f"Columns: {delete_columns} erased.")
+            return metadata_table_bq
+        
+def delete_columns_table(table_id:str,delete_columns:str):
+    client = bigquery.Client()
+
+    table_id = table_id.replace(":",".")
+    for column in delete_columns:
+        delete_columns_query = f'''
+                                ALTER TABLE {table_id}
+                                DROP COLUMN {column}
+                                '''
+        print(delete_columns_query)
+        query_job = client.query(delete_columns_query)
+        query_job.result()
 
 def get_metadata(table_id:str)->dict:
     """_summary_
 
     Args:
         table_id (str): _description_
```

### Comparing `yastas-data-0.3.6/data_code/gcp/sql.py` & `yastas-data-0.3.7/data_code/gcp/sql.py`

 * *Files identical despite different names*

### Comparing `yastas-data-0.3.6/data_code/parquets/parquet2csv.py` & `yastas-data-0.3.7/data_code/parquets/parquet2csv.py`

 * *Files identical despite different names*

### Comparing `yastas-data-0.3.6/setup.py` & `yastas-data-0.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open('requirements.txt') as file:
         return file.read().splitlines()
     
 readme = open("./README.md", "r")
 
 setup(
     name='yastas-data',
-    version='0.3.6',
+    version='0.3.7',
     author='Data - Aaron',
     author_email="e-ajuareza@minsait.com",
     description='Paquete distribuible en repositorio de funciones locales',
     long_description=readme.read(),
     packages=find_packages(),
     url="https://bitbucket.org/gentera-insumos/data-code",
     keywords=['data', 'big_data', 'data_analytics', 'data_engineer', 'data_science'],
```

### Comparing `yastas-data-0.3.6/yastas_data.egg-info/PKG-INFO` & `yastas-data-0.3.7/yastas_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: yastas-data
-Version: 0.3.6
+Version: 0.3.7
 Summary: Paquete distribuible en repositorio de funciones locales
 Home-page: https://bitbucket.org/gentera-insumos/data-code
 Author: Data - Aaron
 Author-email: e-ajuareza@minsait.com
 License: MIT
 Description: # InstalaciÃ³n
```

