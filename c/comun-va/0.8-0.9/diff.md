# Comparing `tmp/comun_va-0.8.tar.gz` & `tmp/comun_va-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comun_va-0.8.tar", last modified: Tue Jul 25 08:53:48 2023, max compression
+gzip compressed data, was "comun_va-0.9.tar", last modified: Tue Aug  8 07:39:40 2023, max compression
```

## Comparing `comun_va-0.8.tar` & `comun_va-0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 08:53:48.015993 comun_va-0.8/
--rw-rw-rw-   0        0        0       53 2023-07-25 08:53:48.015993 comun_va-0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-25 08:53:48.014984 comun_va-0.8/comun_va.egg-info/
--rw-rw-rw-   0        0        0       53 2023-07-25 08:53:47.000000 comun_va-0.8/comun_va.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-07-25 08:53:47.000000 comun_va-0.8/comun_va.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 08:53:47.000000 comun_va-0.8/comun_va.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-25 08:53:47.000000 comun_va-0.8/comun_va.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-25 08:53:47.000000 comun_va-0.8/comun_va.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5104 2023-07-25 08:53:16.000000 comun_va-0.8/comun_va.py
--rw-rw-rw-   0        0        0       42 2023-07-25 08:53:48.015993 comun_va-0.8/setup.cfg
--rw-rw-rw-   0        0        0      192 2023-07-25 08:53:16.000000 comun_va-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 07:39:40.071595 comun_va-0.9/
+-rw-rw-rw-   0        0        0       53 2023-08-08 07:39:40.070186 comun_va-0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-08 07:39:40.069185 comun_va-0.9/comun_va.egg-info/
+-rw-rw-rw-   0        0        0       53 2023-08-08 07:39:39.000000 comun_va-0.9/comun_va.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-08-08 07:39:39.000000 comun_va-0.9/comun_va.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 07:39:39.000000 comun_va-0.9/comun_va.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-08-08 07:39:39.000000 comun_va-0.9/comun_va.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-08 07:39:39.000000 comun_va-0.9/comun_va.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5090 2023-08-08 07:39:37.000000 comun_va-0.9/comun_va.py
+-rw-rw-rw-   0        0        0       42 2023-08-08 07:39:40.071595 comun_va-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      192 2023-08-08 07:39:37.000000 comun_va-0.9/setup.py
```

### Comparing `comun_va-0.8/comun_va.py` & `comun_va-0.9/comun_va.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,32 +25,32 @@
                 Date: {self.date_time},
                 Endpoint name: {self.endpoint_name},
                 Endpoint received data: {self.endpoint_data_received},
                 Result: {self.result},
                 Prediction: {self.prediction}         
                 """
 
-    def save_log(self, mssql_srv: str, database: str, user: str, passwd: str, rescale_size: tuple = None):
+    def save_log(self, mssql_srv: str, database: str, user: str, passwd: str, resize=False):
         """
         Save the image in local path and the data into the DB
         :param mssql_srv: IP of the MSsql server
         :param database: Name of the database
         :param user: User of the database
         :param passwd: Password of the user
-        :param rescale_size: A tuple with the HxW (in px) to rescale the image, example: (500, 500)
+        :param resize: Boolean argument, by defect is False, if True will save the image resized to 500x500
         :return: doesn't return anything
         """
         # SAVE IMAGE:
         if self.img_frame is not None:
             if self.img_name is None:
                 self.img_name = f'{self.date_time.strftime("%Y_%m_%d_%H_%M_%S")}.jpg'
             if self.img_path is None:
                 self.img_path = f'img_save/{self.img_name}'
-            if rescale_size:
-                self.img_frame = cv2.resize(self.img_frame, rescale_size)
+            if resize:
+                self.img_frame = cv2.resize(self.img_frame, (500, 500))
             cv2.imwrite(self.img_path, self.img_frame)
 
         # SAVE LOG IN DB:
         mssql = comun_sqlsrv.Sql(mssql_srv, database, user, passwd)
         query = f"""
                 INSERT INTO T_VA_API_LOG
                 (FECHA_HORA, ENDPOINT, RESULTADO, DATO_RECIBIDO, PREDICCION_VA, NOMBRE_IMAGEN, COD_BAR, ERROR)
```

