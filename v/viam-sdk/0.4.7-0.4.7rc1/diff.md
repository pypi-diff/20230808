# Comparing `tmp/viam_sdk-0.4.7-py3-none-manylinux2014_x86_64.whl.zip` & `tmp/viam_sdk-0.4.7rc1-py3-none-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 10152765 bytes, number of entries: 389
+Zip file size: 10152793 bytes, number of entries: 389
 -rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx     1411 b- defN 80-Jan-01 00:00 viam/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 viam/app/__init__.py
 -rw-r--r--  2.0 unx    28885 b- defN 80-Jan-01 00:00 viam/app/app_client.py
 -rw-r--r--  2.0 unx    27945 b- defN 80-Jan-01 00:00 viam/app/data_client.py
 -rw-r--r--  2.0 unx     2666 b- defN 80-Jan-01 00:00 viam/app/viam_client.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 viam/components/__init__.py
@@ -380,12 +380,12 @@
 -rw-r--r--  2.0 unx     1633 b- defN 80-Jan-01 00:00 viam/services/slam/slam.py
 -rw-r--r--  2.0 unx      426 b- defN 80-Jan-01 00:00 viam/services/vision/__init__.py
 -rw-r--r--  2.0 unx     5176 b- defN 80-Jan-01 00:00 viam/services/vision/client.py
 -rw-r--r--  2.0 unx     5076 b- defN 80-Jan-01 00:00 viam/services/vision/service.py
 -rw-r--r--  2.0 unx     5066 b- defN 80-Jan-01 00:00 viam/services/vision/vision.py
 -rw-r--r--  2.0 unx     5286 b- defN 80-Jan-01 00:00 viam/sessions_client.py
 -rw-r--r--  2.0 unx     8145 b- defN 80-Jan-01 00:00 viam/utils.py
--rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 viam_sdk-0.4.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     8977 b- defN 80-Jan-01 00:00 viam_sdk-0.4.7.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 viam_sdk-0.4.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx    35949 b- defN 16-Jan-01 00:00 viam_sdk-0.4.7.dist-info/RECORD
-389 files, 30926724 bytes uncompressed, 10094869 bytes compressed:  67.4%
+-rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 viam_sdk-0.4.7rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8980 b- defN 80-Jan-01 00:00 viam_sdk-0.4.7rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 viam_sdk-0.4.7rc1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    35961 b- defN 16-Jan-01 00:00 viam_sdk-0.4.7rc1.dist-info/RECORD
+389 files, 30926739 bytes uncompressed, 10094873 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -1149,20 +1149,20 @@
 
 Filename: viam/sessions_client.py
 Comment: 
 
 Filename: viam/utils.py
 Comment: 
 
-Filename: viam_sdk-0.4.7.dist-info/LICENSE
+Filename: viam_sdk-0.4.7rc1.dist-info/LICENSE
 Comment: 
 
-Filename: viam_sdk-0.4.7.dist-info/METADATA
+Filename: viam_sdk-0.4.7rc1.dist-info/METADATA
 Comment: 
 
-Filename: viam_sdk-0.4.7.dist-info/WHEEL
+Filename: viam_sdk-0.4.7rc1.dist-info/WHEEL
 Comment: 
 
-Filename: viam_sdk-0.4.7.dist-info/RECORD
+Filename: viam_sdk-0.4.7rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `viam_sdk-0.4.7.dist-info/LICENSE` & `viam_sdk-0.4.7rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `viam_sdk-0.4.7.dist-info/METADATA` & `viam_sdk-0.4.7rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viam-sdk
-Version: 0.4.7
+Version: 0.4.7rc1
 Summary: Viam Robotics Python SDK
 License: Apache-2.0
 Author: Naveed
 Author-email: naveed@viam.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `viam_sdk-0.4.7.dist-info/RECORD` & `viam_sdk-0.4.7rc1.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -379,11 +379,11 @@
 viam/services/slam/slam.py,sha256=872OV9JvSEvwWRBDiX-P8Zs87fNBp-5mbMx4ruot-gY,1633
 viam/services/vision/__init__.py,sha256=8DPwRKggv0cMb3Z4R5-pAHvbAIIMBfNYWUktuh58gyE,426
 viam/services/vision/client.py,sha256=EHiVW1R2JgS_DzyenmJzcIhQdtiegeUUBy2lYBpKemg,5176
 viam/services/vision/service.py,sha256=ae0zUVBi-QiNYoxfT7KurCUvdy0umdUdFVqMLprF_3c,5076
 viam/services/vision/vision.py,sha256=4JGFJVU8yv5poFnF-LaS_cd2SMRTNHp3XWKlfWWCO4I,5066
 viam/sessions_client.py,sha256=Et7ipPP89RJ6PGjfwfstunDfZzGEmkrfDeldzBZ-Zso,5286
 viam/utils.py,sha256=gJvtsGXG1eWsWbiu52ERNz0UYHc6JmouFXZ68ZlNS3A,8145
-viam_sdk-0.4.7.dist-info/LICENSE,sha256=yVuuHRzgI17MzTVgt3LsHvuX80innw--CmNPDCzO_iw,11358
-viam_sdk-0.4.7.dist-info/METADATA,sha256=ZdKa2PkSmdQbazleUOU1LcERNFdn4QKM1MEHV3zb5zU,8977
-viam_sdk-0.4.7.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-viam_sdk-0.4.7.dist-info/RECORD,,
+viam_sdk-0.4.7rc1.dist-info/LICENSE,sha256=yVuuHRzgI17MzTVgt3LsHvuX80innw--CmNPDCzO_iw,11358
+viam_sdk-0.4.7rc1.dist-info/METADATA,sha256=WkFsA8RJi8pTh3XyBkYH_Pybg94S6Gbo3IEkBAaQVOQ,8980
+viam_sdk-0.4.7rc1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+viam_sdk-0.4.7rc1.dist-info/RECORD,,
```

