# Comparing `tmp/animage-data_sorter-1.1.4.tar.gz` & `tmp/animage-data_sorter-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\animage-data_sorter-1.1.4.tar", last modified: Mon Jul 10 02:16:36 2023, max compression
+gzip compressed data, was "dist\animage-data_sorter-1.1.5.tar", last modified: Tue Aug  8 07:31:17 2023, max compression
```

## Comparing `animage-data_sorter-1.1.4.tar` & `animage-data_sorter-1.1.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/
--rw-rw-rw-   0        0        0     1363 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      976 2023-05-11 05:19:09.000000 animage-data_sorter-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/animage_data_sorter.egg-info/
--rw-rw-rw-   0        0        0     1363 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/animage_data_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1347 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/animage_data_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/animage_data_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/animage_data_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/data_sorter/
--rw-rw-rw-   0        0        0      630 2023-05-31 06:58:45.000000 animage-data_sorter-1.1.4/data_sorter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/data_sorter/old/
--rw-rw-rw-   0        0        0    23325 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageASLUtility.py
--rw-rw-rw-   0        0        0     7768 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDCMUtility.py
--rw-rw-rw-   0        0        0    26840 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorter.py
--rw-rw-rw-   0        0        0     9852 2023-02-08 06:54:39.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterGEeASL7.py
--rw-rw-rw-   0        0        0     9373 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterGEpCASL13.py
--rw-rw-rw-   0        0        0     4348 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterMISC.py
--rw-rw-rw-   0        0        0     5901 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterPhilips13.py
--rw-rw-rw-   0        0        0    13115 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterSiemens4.py
--rw-rw-rw-   0        0        0    12711 2022-11-17 03:53:33.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterSiemens5.py
--rw-rw-rw-   0        0        0    12032 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterSiemensPASL.py
--rw-rw-rw-   0        0        0    21838 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterSiemens_UCLA.py
--rw-rw-rw-   0        0        0    11395 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterUtility.py
--rw-rw-rw-   0        0        0        0 2023-05-31 06:57:47.000000 animage-data_sorter-1.1.4/data_sorter/old/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/data_sorter/restructure/
--rw-rw-rw-   0        0        0     5204 2023-05-16 02:45:03.000000 animage-data_sorter-1.1.4/data_sorter/restructure/__init__.py
--rw-rw-rw-   0        0        0    37172 2023-07-04 08:05:20.000000 animage-data_sorter-1.1.4/data_sorter/restructure/_dicom.py
--rw-rw-rw-   0        0        0    12556 2023-06-26 04:37:14.000000 animage-data_sorter-1.1.4/data_sorter/restructure/_dicom_util.py
--rw-rw-rw-   0        0        0     4367 2023-06-29 08:41:50.000000 animage-data_sorter-1.1.4/data_sorter/restructure/_type.py
--rw-rw-rw-   0        0        0     4279 2023-06-20 03:26:13.000000 animage-data_sorter-1.1.4/data_sorter/restructure/data_sorter_base.py
--rw-rw-rw-   0        0        0     7621 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.4/data_sorter/restructure/dcm2nifti.py
--rw-rw-rw-   0        0        0     3678 2023-06-30 04:16:40.000000 animage-data_sorter-1.1.4/data_sorter/restructure/errors.py
--rw-rw-rw-   0        0        0     5737 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.4/data_sorter/restructure/ge_3d_pcasl.py
--rw-rw-rw-   0        0        0     8516 2023-07-10 02:11:42.000000 animage-data_sorter-1.1.4/data_sorter/restructure/ge_easl.py
--rw-rw-rw-   0        0        0    12056 2023-07-03 03:36:19.000000 animage-data_sorter-1.1.4/data_sorter/restructure/noASL_MRI.py
--rw-rw-rw-   0        0        0     4431 2023-06-07 08:39:25.000000 animage-data_sorter-1.1.4/data_sorter/restructure/philips_3d_pcasl.py
--rw-rw-rw-   0        0        0     6769 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.4/data_sorter/restructure/siemens_3d_pasl.py
--rw-rw-rw-   0        0        0     7951 2023-05-31 02:53:56.000000 animage-data_sorter-1.1.4/data_sorter/restructure/siemens_3d_pcasl.py
--rw-rw-rw-   0        0        0     8366 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.4/data_sorter/restructure/siemens_3d_pcasl_old.py
--rw-rw-rw-   0        0        0     5735 2023-07-04 08:23:37.000000 animage-data_sorter-1.1.4/data_sorter/restructure/uih_3d_pasl.py
--rw-rw-rw-   0        0        0       42 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      602 2023-07-10 02:15:17.000000 animage-data_sorter-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 07:31:17.000000 animage-data_sorter-1.1.5/
+-rw-rw-rw-   0        0        0     1363 2023-08-08 07:31:17.000000 animage-data_sorter-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      976 2023-05-11 05:19:09.000000 animage-data_sorter-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 07:31:17.000000 animage-data_sorter-1.1.5/animage_data_sorter.egg-info/
+-rw-rw-rw-   0        0        0     1363 2023-08-08 07:31:17.000000 animage-data_sorter-1.1.5/animage_data_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1347 2023-08-08 07:31:17.000000 animage-data_sorter-1.1.5/animage_data_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 07:31:17.000000 animage-data_sorter-1.1.5/animage_data_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-08 07:31:17.000000 animage-data_sorter-1.1.5/animage_data_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 07:31:17.000000 animage-data_sorter-1.1.5/data_sorter/
+-rw-rw-rw-   0        0        0      630 2023-05-31 06:58:45.000000 animage-data_sorter-1.1.5/data_sorter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 07:31:17.000000 animage-data_sorter-1.1.5/data_sorter/old/
+-rw-rw-rw-   0        0        0    23325 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.5/data_sorter/old/AnImageASLUtility.py
+-rw-rw-rw-   0        0        0     7768 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.5/data_sorter/old/AnImageDCMUtility.py
+-rw-rw-rw-   0        0        0    26840 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorter.py
+-rw-rw-rw-   0        0        0     9852 2023-02-08 06:54:39.000000 animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterGEeASL7.py
+-rw-rw-rw-   0        0        0     9373 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterGEpCASL13.py
+-rw-rw-rw-   0        0        0     4348 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterMISC.py
+-rw-rw-rw-   0        0        0     5901 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterPhilips13.py
+-rw-rw-rw-   0        0        0    13115 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterSiemens4.py
+-rw-rw-rw-   0        0        0    12711 2022-11-17 03:53:33.000000 animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterSiemens5.py
+-rw-rw-rw-   0        0        0    12032 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterSiemensPASL.py
+-rw-rw-rw-   0        0        0    21838 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterSiemens_UCLA.py
+-rw-rw-rw-   0        0        0    11395 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterUtility.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 06:57:47.000000 animage-data_sorter-1.1.5/data_sorter/old/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 07:31:17.000000 animage-data_sorter-1.1.5/data_sorter/restructure/
+-rw-rw-rw-   0        0        0     5716 2023-07-24 02:23:24.000000 animage-data_sorter-1.1.5/data_sorter/restructure/__init__.py
+-rw-rw-rw-   0        0        0    37172 2023-07-04 08:05:20.000000 animage-data_sorter-1.1.5/data_sorter/restructure/_dicom.py
+-rw-rw-rw-   0        0        0    12556 2023-07-11 04:25:57.000000 animage-data_sorter-1.1.5/data_sorter/restructure/_dicom_util.py
+-rw-rw-rw-   0        0        0     4367 2023-06-29 08:41:50.000000 animage-data_sorter-1.1.5/data_sorter/restructure/_type.py
+-rw-rw-rw-   0        0        0     4279 2023-06-20 03:26:13.000000 animage-data_sorter-1.1.5/data_sorter/restructure/data_sorter_base.py
+-rw-rw-rw-   0        0        0     7621 2023-08-08 07:24:29.000000 animage-data_sorter-1.1.5/data_sorter/restructure/dcm2nifti.py
+-rw-rw-rw-   0        0        0     3678 2023-06-30 04:16:40.000000 animage-data_sorter-1.1.5/data_sorter/restructure/errors.py
+-rw-rw-rw-   0        0        0     5737 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.5/data_sorter/restructure/ge_3d_pcasl.py
+-rw-rw-rw-   0        0        0     8516 2023-08-08 07:24:36.000000 animage-data_sorter-1.1.5/data_sorter/restructure/ge_easl.py
+-rw-rw-rw-   0        0        0    11877 2023-08-03 06:08:17.000000 animage-data_sorter-1.1.5/data_sorter/restructure/noASL_MRI.py
+-rw-rw-rw-   0        0        0     4431 2023-06-07 08:39:25.000000 animage-data_sorter-1.1.5/data_sorter/restructure/philips_3d_pcasl.py
+-rw-rw-rw-   0        0        0     6769 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.5/data_sorter/restructure/siemens_3d_pasl.py
+-rw-rw-rw-   0        0        0     8166 2023-08-07 08:15:56.000000 animage-data_sorter-1.1.5/data_sorter/restructure/siemens_3d_pcasl.py
+-rw-rw-rw-   0        0        0     8366 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.5/data_sorter/restructure/siemens_3d_pcasl_old.py
+-rw-rw-rw-   0        0        0     6243 2023-08-02 08:09:23.000000 animage-data_sorter-1.1.5/data_sorter/restructure/uih_3d_pasl.py
+-rw-rw-rw-   0        0        0       42 2023-08-08 07:31:17.000000 animage-data_sorter-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      602 2023-08-08 07:30:10.000000 animage-data_sorter-1.1.5/setup.py
```

### Comparing `animage-data_sorter-1.1.4/PKG-INFO` & `animage-data_sorter-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animage-data_sorter
-Version: 1.1.4
+Version: 1.1.5
 Summary: dicom sort
 Home-page: https://gitee.com/AnImage-Beijing/data_sorter
 Author: zhaomy
 Author-email: zhaomy@an-image.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `animage-data_sorter-1.1.4/README.md` & `animage-data_sorter-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/animage_data_sorter.egg-info/PKG-INFO` & `animage-data_sorter-1.1.5/animage_data_sorter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animage-data-sorter
-Version: 1.1.4
+Version: 1.1.5
 Summary: dicom sort
 Home-page: https://gitee.com/AnImage-Beijing/data_sorter
 Author: zhaomy
 Author-email: zhaomy@an-image.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `animage-data_sorter-1.1.4/animage_data_sorter.egg-info/SOURCES.txt` & `animage-data_sorter-1.1.5/animage_data_sorter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/__init__.py` & `animage-data_sorter-1.1.5/data_sorter/__init__.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/old/AnImageASLUtility.py` & `animage-data_sorter-1.1.5/data_sorter/old/AnImageASLUtility.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/old/AnImageDCMUtility.py` & `animage-data_sorter-1.1.5/data_sorter/old/AnImageDCMUtility.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorter.py` & `animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorter.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterGEeASL7.py` & `animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterGEeASL7.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterGEpCASL13.py` & `animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterGEpCASL13.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterMISC.py` & `animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterMISC.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterPhilips13.py` & `animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterPhilips13.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterSiemens4.py` & `animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterSiemens4.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterSiemens5.py` & `animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterSiemens5.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterSiemensPASL.py` & `animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterSiemensPASL.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterSiemens_UCLA.py` & `animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterSiemens_UCLA.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterUtility.py` & `animage-data_sorter-1.1.5/data_sorter/old/AnImageDataSorterUtility.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/restructure/__init__.py` & `animage-data_sorter-1.1.5/data_sorter/restructure/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,23 @@
         if len(delay_time) == 0:
             delay_time = default_value_lambda(data_type, 0)
         if len(label_dur) == 0:
             label_dur = default_value_lambda(data_type, 1)
         if len(delay_rep) == 0:
             delay_rep = default_value_lambda(data_type, 2)
     except Exception as e:
-        logger.warning(f'{data_type} 获取ASL参数失败 => {str(e)}')
+        if data_type in [MRI_Type.MRI_TYPE_3D_PASL_SIEMENS,
+                         MRI_Type.MRI_TYPE_5Delay_3D_PCASL_SIEMENS,
+                         MRI_Type.MRI_TYPE_1Delay_3D_PCASL_SIEMENS,
+                         MRI_Type.MRI_TYPE_4Delay_3D_PCASL_SIEMENS_Old,
+                         MRI_Type.MRI_TYPE_3D_PCASL_PHILIPS,
+                         MRI_Type.MRI_TYPE_3D_PCASL_GE,
+                         MRI_Type.MRI_TYPE_eASL_PCASL_GE,
+                         MRI_Type.MRI_TYPE_3D_PASL_UIH]:
+            logger.warning(f'{data_type} 获取ASL参数失败 => {str(e)}')
     if data_type == MRI_Type.MRI_TYPE_3D_PASL_SIEMENS:
         return DataSorterSiemensPASL(data_type, output_root, delay_time, delay_rep, label_dur, series_list, extra_factor, calc_c_cbf)
     elif data_type in [MRI_Type.MRI_TYPE_5Delay_3D_PCASL_SIEMENS, MRI_Type.MRI_TYPE_1Delay_3D_PCASL_SIEMENS]:
         return DataSorterSiemensPCASL(data_type, output_root, delay_time, delay_rep, label_dur, series_list, calc_c_cbf)
     elif data_type == MRI_Type.MRI_TYPE_4Delay_3D_PCASL_SIEMENS_Old:
         return DataSorterSiemensPCASL_old(data_type, output_root, delay_time, delay_rep, label_dur, series_list, calc_c_cbf)
     elif data_type == MRI_Type.MRI_TYPE_3D_PCASL_PHILIPS:
```

### Comparing `animage-data_sorter-1.1.4/data_sorter/restructure/_dicom.py` & `animage-data_sorter-1.1.5/data_sorter/restructure/_dicom.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/restructure/_dicom_util.py` & `animage-data_sorter-1.1.5/data_sorter/restructure/_dicom_util.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/restructure/_type.py` & `animage-data_sorter-1.1.5/data_sorter/restructure/_type.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/restructure/data_sorter_base.py` & `animage-data_sorter-1.1.5/data_sorter/restructure/data_sorter_base.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/restructure/dcm2nifti.py` & `animage-data_sorter-1.1.5/data_sorter/restructure/dcm2nifti.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/restructure/errors.py` & `animage-data_sorter-1.1.5/data_sorter/restructure/errors.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/restructure/ge_3d_pcasl.py` & `animage-data_sorter-1.1.5/data_sorter/restructure/ge_3d_pcasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/restructure/ge_easl.py` & `animage-data_sorter-1.1.5/data_sorter/restructure/ge_easl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/restructure/noASL_MRI.py` & `animage-data_sorter-1.1.5/data_sorter/restructure/noASL_MRI.py`

 * *Files 10% similar despite different names*

```diff
@@ -126,27 +126,33 @@
                 self.DWI = dwi
                 self.is_find_multi_volume = True
                 break
 
         # 多B值不在同一个序列，必须要求DWI_list大于1
         if (not self.is_find_multi_volume):
             if len(self.DWI_list) < 2:
-                raise NeedTwoBValueDWIError()
+                self.DWI = self.DWI_list[0]
+                # 当DWI不足报个警告，不再抛异常；当需要计算ADC的时候，再判断是否抛异常
+                logger.warning('DWI序列缺少两个不同B值的Series')
+                # raise NeedTwoBValueDWIError()
             else:
-                first_dwi = self.DWI_list[0]
-                second_dwi = self.DWI_list[1]
-                self.DWI = first_dwi
-                if first_dwi.SliceNumber != second_dwi.SliceNumber:
-                    raise SpaceIsDifferentError('DWI', 'ADC')
-
+                self.DWI = self.DWI_list[0]
+                # 判断层数是否一致
+                if len(set([i.SliceNumber for i in self.DWI_list])) != 1:
+                    raise SpaceIsDifferentError('DWI')
 
         # ADC序列验证，允许不存在。
         if len(self.ADC_list) < 1:
             logger.info(f'未发现ADC序列')
             self.ADC = None
+
+            # DWI不足无法计算ADC
+            if (not self.is_find_multi_volume) and len(self.DWI_list) < 2:
+                raise NeedTwoBValueDWIError()
+
         else:
             logger.debug(f'发现{len(self.ADC_list)}组ADC数据')
             self.ADC = self.ADC_list[0]
 
         if self.ADC is not None and self.DWI.SliceNumber != self.ADC.SliceNumber:
             raise SpaceIsDifferentError('DWI', 'ADC')
 
@@ -154,83 +160,73 @@
     @staticmethod
     def get_tag(dcm_obj: Union[DicomRequiredTags, pydicom.Dataset], key, default=None):
         if isinstance(dcm_obj, DicomRequiredTags):
             return dcm_obj.get_tag(key, default=default)
         else:
             return DicomRequiredTags.get_key(key, dcm_obj, default)
 
-    def find_two_instance(self):
+    def find_multi_instance(self):
+        multi_instances = []
+
         # 多B值不在同一个序列, 找到第二个Volume的位置
         if self.is_find_multi_volume:
-            second_slice_number = 1 if self.DWI.is_second_arrangement_mode else self.DWI.SliceNumber
-            # 3D dicom的B值在PerFrameFunctionalGroupsSequence中
-            if self.DWI.dicom_image_type == DICOM_IMAGE_TYPE.DICOM_IMAGE_TYPE_3D:
-                first_instance = self.get_tag(self.DWI.PerFrameFunctionalGroupsSequence[0], (0x0018, 0x9117))[0]
-                second_instance = \
-                    self.get_tag(self.DWI.PerFrameFunctionalGroupsSequence[second_slice_number], (0x0018, 0x9117))[0]
-            else:
-                first_instance = self.DWI[0]
-                second_instance = self.DWI[second_slice_number]
+            multi_slice_number = [i for i in range(self.DWI.Repetition)] if self.DWI.is_second_arrangement_mode \
+                else [i * self.DWI.SliceNumber for i in range(self.DWI.Repetition)]
 
+            # 3D dicom的B值在PerFrameFunctionalGroupsSequence中
+            for i in multi_slice_number:
+                if self.DWI.dicom_image_type == DICOM_IMAGE_TYPE.DICOM_IMAGE_TYPE_3D:
+                    multi_instances.append(self.get_tag(self.DWI.PerFrameFunctionalGroupsSequence[i], (0x0018, 0x9117))[0])
+                else:
+                    multi_instances.append(self.DWI[i])
             DWI_image = self.DWI.load()
-            return (first_instance, DWI_image[...,0]), (second_instance, DWI_image[...,1])
+            return multi_instances, DWI_image
         else:
-            first_dwi = self.DWI_list[0]
-            second_dwi = self.DWI_list[1]
-            if first_dwi.dicom_image_type == DICOM_IMAGE_TYPE.DICOM_IMAGE_TYPE_3D:
-                first_instance = self.get_tag(first_dwi.PerFrameFunctionalGroupsSequence[0], (0x0018, 0x9117))[0]
-                second_instance = \
-                    self.get_tag(second_dwi.PerFrameFunctionalGroupsSequence[0], (0x0018, 0x9117))[0]
-            else:
-                first_instance = first_dwi[0]
-                second_instance = second_dwi[0]
-            return (first_instance, first_dwi.load()), (second_instance, second_dwi.load())
+            for dwi in self.DWI_list:
+                if self.DWI.dicom_image_type == DICOM_IMAGE_TYPE.DICOM_IMAGE_TYPE_3D:
+                    multi_instances.append(self.get_tag(dwi.PerFrameFunctionalGroupsSequence[0], (0x0018, 0x9117))[0])
+                else:
+                    multi_instances.append(dwi[0])
+            return multi_instances, np.concatenate([i.load() for i in self.DWI_list], axis=-1)
+
+
 
     def Sorter(self):
         super(DataSorterDWI, self).Sorter()
         self.validate_series()
-        (first_instance, first_volume), (second_instance, second_volume) = self.find_two_instance()
+        multi_instances, DWI_volume = self.find_multi_instance()
 
-        # DWI需要包含B0与B1000
-        # 标准dicom中的B值(弥散系数)标签信息
-        first_b_value = self.get_tag(first_instance, (0x0018, 0x9087), 0)
-        second_b_value = self.get_tag(second_instance, (0x0018, 0x9087), 0)
-        if self.DWI.Manufacturer == MANUFACTURER.kMANUFACTURER_GE:
-            first_b_value = first_b_value if first_b_value != 0 else \
-                self.get_tag(first_instance, (0x0043, 0x1039), [0])[0]
-            second_b_value = second_b_value if second_b_value != 0 else \
-                self.get_tag(second_instance, (0x0043, 0x1039), [0])[0]
-
-        elif self.DWI.Manufacturer == MANUFACTURER.kMANUFACTURER_SIEMENS:
-            first_b_value = first_b_value if first_b_value != 0 else \
-                self.get_tag(first_instance, (0x0019, 0x100C), 0)
-            second_b_value = second_b_value if second_b_value != 0 else \
-                self.get_tag(second_instance, (0x0019, 0x100C), 0)
+        b_value_list = []
+        # 读取每组的B值
+        for instance in multi_instances:
+            # 标准dicom中的B值(弥散系数)标签信息
+            b_value = self.get_tag(instance, (0x0018, 0x9087), 0)
+            if self.DWI.Manufacturer == MANUFACTURER.kMANUFACTURER_GE:
+                b_value = b_value if b_value != 0 else \
+                    self.get_tag(instance, (0x0043, 0x1039), [0])[0]
+
+            elif self.DWI.Manufacturer == MANUFACTURER.kMANUFACTURER_SIEMENS:
+                b_value = b_value if b_value != 0 else \
+                    self.get_tag(instance, (0x0019, 0x100C), 0)
 
-        elif self.DWI.Manufacturer in [MANUFACTURER.kMANUFACTURER_PHILIPS, MANUFACTURER.kMANUFACTURER_UIH]:
-            pass
-
-        else:
-            raise UnSupportDataTypeError(self.DWI.Manufacturer)
+            elif self.DWI.Manufacturer in [MANUFACTURER.kMANUFACTURER_PHILIPS, MANUFACTURER.kMANUFACTURER_UIH]:
+                pass
+            else:
+                raise UnSupportDataTypeError(self.DWI.Manufacturer)
+            b_value_list.append(b_value)
+        b_value_list = [int(i) for i in b_value_list]
+        logger.info(f'DWI发现的B值：{b_value_list}')
 
-        first_b_value = int(first_b_value)
-        second_b_value = int(second_b_value)
-        logger.info(f'DWI使用的两个B值：{first_b_value}, {second_b_value}')
-        if first_b_value == 0 and second_b_value == 0:
-            raise DiffusionBValueMissingError()
 
         cur_series_number = SeriesNumberStartWith.DWI
+        for b_value, slice in zip(b_value_list, range(DWI_volume.shape[-1])):
+            write_dicom_series(DWI_volume[..., slice], self.DWI, f'dwi-b{b_value}', cur_series_number,
+                               os.path.join(self.output_root, 'dwi', f'b{b_value}'))
+            cur_series_number += 1
 
-        write_dicom_series(first_volume, self.DWI, f'dwi-b{first_b_value}', cur_series_number,
-                           os.path.join(self.output_root, 'dwi', f'b{first_b_value}'))
-        cur_series_number += 1
-        write_dicom_series(second_volume, self.DWI, f'dwi-b{second_b_value}', cur_series_number,
-                               os.path.join(self.output_root, 'dwi', f'b{second_b_value}'))
-
-        cur_series_number += 1
         rescale_type = '10^-6 mm^2/s'
         if self.ADC is not None:
             # ADC， 确定单位
             rescale_type_1 = self.ADC.get_tag((0x0028, 0x1054), '')
             rescale_type_2 = self.ADC.get_tag((0x2005, 0x140B), '')
             if rescale_type_1 != '':
                 rescale_type = rescale_type_1
@@ -238,21 +234,27 @@
                 rescale_type = rescale_type_2
 
             rescale = 1000 if rescale_type == '10^-3 mm^2/s' else 1
             ADC_img = self.ADC.load(rescale)[...,0]
             write_dicom_series(ADC_img, self.DWI, 'dwi-adc', cur_series_number,
                                os.path.join(self.output_root, 'dwi', 'adc'))
 
-        else:
+        else: # 需要计算ADC
+            # 验证B值是否符合要求
+            first_b_value, first_volume = b_value_list[0], DWI_volume[...,0]
+            second_b_value, second_volume = b_value_list[1], DWI_volume[...,1]
+            logger.info(f'DWI使用的两个B值：{first_b_value}, {second_b_value}')
+            if first_b_value == 0 and second_b_value == 0:
+                raise DiffusionBValueMissingError()
+
             logger.debug(f'开始计算ADC')
             # 使second_b_value等于较大B值的那个图像
             if first_b_value > second_b_value:
                 first_b_value, second_b_value = second_b_value, first_b_value
                 first_volume, second_volume = second_volume, first_volume
             ADC_img = np.log(first_volume / second_volume) / (second_b_value - first_b_value)
-            # ADC_img = -1000 * np.log(np.divide(second_volume, first_volume))
             ADC_img[np.isinf(ADC_img) | np.isnan(ADC_img)] = 0
             ADC_img *= 10**6
             ADC_img[ADC_img < 0] = -256
 
             write_dicom_series(ADC_img, self.DWI, 'dwi-adc', cur_series_number,
                                os.path.join(self.output_root, 'dwi', 'adc'))
```

### Comparing `animage-data_sorter-1.1.4/data_sorter/restructure/philips_3d_pcasl.py` & `animage-data_sorter-1.1.5/data_sorter/restructure/philips_3d_pcasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/restructure/siemens_3d_pasl.py` & `animage-data_sorter-1.1.5/data_sorter/restructure/siemens_3d_pasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/restructure/siemens_3d_pcasl.py` & `animage-data_sorter-1.1.5/data_sorter/restructure/siemens_3d_pcasl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,497 +1,511 @@
 00000000: 0d0a 696d 706f 7274 206a 736f 6e0d 0a69  ..import json..i
-00000010: 6d70 6f72 7420 7368 7574 696c 0d0a 696d  mport shutil..im
-00000020: 706f 7274 2073 7562 7072 6f63 6573 730d  port subprocess.
-00000030: 0a0d 0a69 6d70 6f72 7420 6d61 7470 6c6f  ...import matplo
-00000040: 746c 6962 0d0a 696d 706f 7274 206d 6174  tlib..import mat
-00000050: 706c 6f74 6c69 622e 7079 706c 6f74 2061  plotlib.pyplot a
-00000060: 7320 706c 740d 0a69 6d70 6f72 7420 6e75  s plt..import nu
-00000070: 6d70 7920 6173 206e 700d 0a0d 0a66 726f  mpy as np....fro
-00000080: 6d20 2e5f 6469 636f 6d20 696d 706f 7274  m ._dicom import
-00000090: 202a 0d0a 6672 6f6d 202e 5f64 6963 6f6d   *..from ._dicom
-000000a0: 5f75 7469 6c20 696d 706f 7274 2077 7269  _util import wri
-000000b0: 7465 5f64 6963 6f6d 5f73 6572 6965 730d  te_dicom_series.
-000000c0: 0a66 726f 6d20 2e64 6174 615f 736f 7274  .from .data_sort
-000000d0: 6572 5f62 6173 6520 696d 706f 7274 2044  er_base import D
-000000e0: 6174 6153 6f72 7465 7241 534c 4261 7365  ataSorterASLBase
-000000f0: 0d0a 0d0a 0d0a 636c 6173 7320 4461 7461  ......class Data
-00000100: 536f 7274 6572 5369 656d 656e 7350 4341  SorterSiemensPCA
-00000110: 534c 2844 6174 6153 6f72 7465 7241 534c  SL(DataSorterASL
-00000120: 4261 7365 293a 0d0a 2020 2020 6465 6620  Base):..    def 
-00000130: 5f5f 696e 6974 5f5f 2873 656c 662c 2064  __init__(self, d
-00000140: 6174 615f 7479 7065 2c20 6f75 7470 7574  ata_type, output
-00000150: 5f72 6f6f 742c 2064 656c 6179 5f74 696d  _root, delay_tim
-00000160: 652c 2064 656c 6179 5f72 6570 2c20 6c61  e, delay_rep, la
-00000170: 6265 6c5f 6475 722c 2073 6572 6965 735f  bel_dur, series_
-00000180: 6c69 7374 2c20 6361 6c63 5f63 5f63 6266  list, calc_c_cbf
-00000190: 293a 0d0a 2020 2020 2020 2020 4461 7461  ):..        Data
-000001a0: 536f 7274 6572 4153 4c42 6173 652e 5f5f  SorterASLBase.__
-000001b0: 696e 6974 5f5f 2873 656c 662c 2064 6174  init__(self, dat
-000001c0: 615f 7479 7065 2c20 6f75 7470 7574 5f72  a_type, output_r
-000001d0: 6f6f 742c 2064 656c 6179 5f74 696d 652c  oot, delay_time,
-000001e0: 2064 656c 6179 5f72 6570 2c20 6c61 6265   delay_rep, labe
-000001f0: 6c5f 6475 722c 2073 6572 6965 735f 6c69  l_dur, series_li
-00000200: 7374 2c20 6361 6c63 5f63 5f63 6266 290d  st, calc_c_cbf).
-00000210: 0a0d 0a20 2020 2020 2020 2064 656c 6179  ...        delay
-00000220: 5f6e 756d 203d 206c 656e 2873 656c 662e  _num = len(self.
-00000230: 6465 6c61 795f 7469 6d65 290d 0a20 2020  delay_time)..   
-00000240: 2020 2020 2072 6570 5f6e 756d 203d 206c       rep_num = l
-00000250: 656e 2873 656c 662e 6465 6c61 795f 7265  en(self.delay_re
-00000260: 7029 0d0a 2020 2020 2020 2020 6966 2064  p)..        if d
-00000270: 656c 6179 5f6e 756d 2021 3d20 7265 705f  elay_num != rep_
-00000280: 6e75 6d3a 0d0a 2020 2020 2020 2020 2020  num:..          
-00000290: 2020 7261 6973 6520 4465 6c61 794e 6f74    raise DelayNot
-000002a0: 4571 7561 6c52 6570 6574 6974 696f 6e45  EqualRepetitionE
-000002b0: 7272 6f72 2864 656c 6179 5f6e 756d 2c20  rror(delay_num, 
-000002c0: 7265 705f 6e75 6d29 0d0a 0d0a 2020 2020  rep_num)....    
-000002d0: 2020 2020 6966 2073 656c 662e 6461 7461      if self.data
-000002e0: 5f74 7970 6520 3d3d 204d 5249 5f54 7970  _type == MRI_Typ
-000002f0: 652e 4d52 495f 5459 5045 5f35 4465 6c61  e.MRI_TYPE_5Dela
-00000300: 795f 3344 5f50 4341 534c 5f53 4945 4d45  y_3D_PCASL_SIEME
-00000310: 4e53 2061 6e64 2064 656c 6179 5f6e 756d  NS and delay_num
-00000320: 2021 3d20 353a 0d0a 2020 2020 2020 2020   != 5:..        
-00000330: 2020 2020 7261 6973 6520 4465 6c61 794e      raise DelayN
-00000340: 6f74 4571 7561 6c53 6572 6965 734e 756d  otEqualSeriesNum
-00000350: 6265 7245 7272 6f72 2864 656c 6179 5f6e  berError(delay_n
-00000360: 756d 2c20 3529 0d0a 2020 2020 2020 2020  um, 5)..        
-00000370: 6966 2073 656c 662e 6461 7461 5f74 7970  if self.data_typ
-00000380: 6520 3d3d 204d 5249 5f54 7970 652e 4d52  e == MRI_Type.MR
-00000390: 495f 5459 5045 5f31 4465 6c61 795f 3344  I_TYPE_1Delay_3D
-000003a0: 5f50 4341 534c 5f53 4945 4d45 4e53 2061  _PCASL_SIEMENS a
-000003b0: 6e64 2064 656c 6179 5f6e 756d 2021 3d20  nd delay_num != 
-000003c0: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
-000003d0: 7261 6973 6520 4465 6c61 794e 6f74 4571  raise DelayNotEq
-000003e0: 7561 6c53 6572 6965 734e 756d 6265 7245  ualSeriesNumberE
-000003f0: 7272 6f72 2864 656c 6179 5f6e 756d 2c20  rror(delay_num, 
-00000400: 3129 0d0a 0d0a 0d0a 2020 2020 2020 2020  1)......        
-00000410: 2320 5057 49e5 9bbe e5a6 82e6 9e9c e8a2  # PWI...........
-00000420: abe5 8c85 e590 abe8 bf9b e69d a5ef bc8c  ................
-00000430: e68e 92e9 99a4 e68e 890d 0a20 2020 2020  ...........     
-00000440: 2020 2073 656c 662e 7261 775f 7365 7269     self.raw_seri
-00000450: 6573 203d 2073 6f72 7465 6428 7365 7269  es = sorted(seri
-00000460: 6573 5f6c 6973 742c 206b 6579 3d6c 616d  es_list, key=lam
-00000470: 6264 6120 783a 206c 656e 2878 292c 2072  bda x: len(x), r
-00000480: 6576 6572 7365 3d54 7275 6529 5b30 5d0d  everse=True)[0].
-00000490: 0a0d 0a20 2020 2064 6566 2053 6f72 7465  ...    def Sorte
-000004a0: 7228 7365 6c66 293a 0d0a 2020 2020 2020  r(self):..      
-000004b0: 2020 7375 7065 7228 4461 7461 536f 7274    super(DataSort
-000004c0: 6572 5369 656d 656e 7350 4341 534c 2c20  erSiemensPCASL, 
-000004d0: 7365 6c66 292e 536f 7274 6572 2829 0d0a  self).Sorter()..
-000004e0: 0d0a 2020 2020 2020 2020 2320 e58d 95e5  ..        # ....
-000004f0: bbb6 e8bf 9f50 4341 534c e987 8de6 96b0  .....PCASL......
-00000500: e8ae a1e7 ae97 e987 8de5 a48d e6ac a1e6  ................
-00000510: 95b0 0d0a 2020 2020 2020 2020 6966 2073  ....        if s
-00000520: 656c 662e 6461 7461 5f74 7970 6520 3d3d  elf.data_type ==
-00000530: 204d 5249 5f54 7970 652e 4d52 495f 5459   MRI_Type.MRI_TY
-00000540: 5045 5f31 4465 6c61 795f 3344 5f50 4341  PE_1Delay_3D_PCA
-00000550: 534c 5f53 4945 4d45 4e53 3a0d 0a20 2020  SL_SIEMENS:..   
-00000560: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-00000570: 6c61 795f 7265 7020 3d20 5b73 656c 662e  lay_rep = [self.
-00000580: 7261 775f 7365 7269 6573 2e6c 6f61 6428  raw_series.load(
-00000590: 292e 7368 6170 655b 2d31 5d20 2f2f 2032  ).shape[-1] // 2
-000005a0: 202d 2031 5d0d 0a0d 0a20 2020 2020 2020   - 1]....       
-000005b0: 206a 6176 615f 7465 6d70 203d 206f 732e   java_temp = os.
-000005c0: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e6f  path.join(self.o
-000005d0: 7574 7075 745f 726f 6f74 2c20 276a 6176  utput_root, 'jav
-000005e0: 615f 7465 6d70 2729 0d0a 2020 2020 2020  a_temp')..      
-000005f0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00000600: 2020 2020 7265 636f 6e73 7472 7563 7465      reconstructe
-00000610: 645f 6469 7220 3d20 7365 6c66 2e67 656e  d_dir = self.gen
-00000620: 6572 6174 655f 6672 6f6d 5f72 6177 5f66  erate_from_raw_f
-00000630: 6f6c 6465 7228 6a61 7661 5f74 656d 7029  older(java_temp)
-00000640: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00000650: 6c66 2e5f 7361 7665 5f68 6561 645f 6d6f  lf._save_head_mo
-00000660: 7469 6f6e 5f67 7261 7068 2829 0d0a 0d0a  tion_graph()....
-00000670: 2020 2020 2020 2020 2020 2020 2320 e8ae              # ..
-00000680: a1e7 ae97 e5ae 8ce5 908e efbc 8ce5 be97  ................
-00000690: e588 b0e7 9a84 3244 e5a2 9ee5 bcba 4469  ......2D......Di
-000006a0: 636f 6de6 9687 e4bb b6ef bc8c e5b0 86e5  com.............
-000006b0: 85b6 e987 8de6 95b4 e4b8 ba32 4420 4469  ...........2D Di
-000006c0: 636f 6def bc9b e987 8de5 8699 e696 b9e5  com.............
-000006d0: 9091 efbc 8ce4 bd8d e7bd aee6 a087 e7ad  ................
-000006e0: be0d 0a20 2020 2020 2020 2020 2020 2064  ...            d
-000006f0: 6566 206c 616d 6264 615f 6c6f 6164 5f64  ef lambda_load_d
-00000700: 6963 6f6d 286e 616d 6529 3a0d 0a20 2020  icom(name):..   
-00000710: 2020 2020 2020 2020 2020 2020 206d 6174               mat
-00000720: 203d 2070 7964 6963 6f6d 2e72 6561 645f   = pydicom.read_
-00000730: 6669 6c65 286f 732e 7061 7468 2e6a 6f69  file(os.path.joi
-00000740: 6e28 7265 636f 6e73 7472 7563 7465 645f  n(reconstructed_
-00000750: 6469 722c 206e 616d 652b 272e 6463 6d27  dir, name+'.dcm'
-00000760: 2929 2e70 6978 656c 5f61 7272 6179 0d0a  )).pixel_array..
-00000770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000780: 6d61 7420 3d20 6d61 742e 7377 6170 6178  mat = mat.swapax
-00000790: 6573 2830 2c20 3229 0d0a 2020 2020 2020  es(0, 2)..      
-000007a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000007b0: 206d 6174 2e73 7761 7061 7865 7328 302c   mat.swapaxes(0,
-000007c0: 2031 290d 0a0d 0a20 2020 2020 2020 2020   1)....         
-000007d0: 2020 2063 7572 5f73 6572 6965 735f 6e75     cur_series_nu
-000007e0: 6d62 6572 203d 2053 6572 6965 734e 756d  mber = SeriesNum
-000007f0: 6265 7253 7461 7274 5769 7468 2e41 534c  berStartWith.ASL
-00000800: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00000810: 206c 656e 2873 656c 662e 6465 6c61 795f   len(self.delay_
-00000820: 7469 6d65 2920 3d3d 2035 3a0d 0a20 2020  time) == 5:..   
-00000830: 2020 2020 2020 2020 2020 2020 2070 6172               par
-00000840: 616d 5f61 7272 6179 203d 204e 6f6e 650d  am_array = None.
-00000850: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00000860: 2020 2066 696c 655f 6c69 7374 203d 205b     file_list = [
-00000870: 226d 3022 2c20 226d 6362 6622 2c20 2261  "m0", "mcbf", "a
-00000880: 7474 222c 2022 6163 6276 222c 2022 6362  tt", "acbv", "cb
-00000890: 6631 222c 2022 6362 6632 222c 2022 6362  f1", "cbf2", "cb
-000008a0: 6633 222c 2022 6362 6634 222c 2022 6362  f3", "cbf4", "cb
-000008b0: 6635 225d 0d0a 2020 2020 2020 2020 2020  f5"]..          
-000008c0: 2020 2020 2020 7363 616c 696e 675f 6c69        scaling_li
-000008d0: 7374 203d 205b 312c 2030 2e31 2c20 302e  st = [1, 0.1, 0.
-000008e0: 3031 2c20 302e 3030 312c 2030 2e31 2c20  01, 0.001, 0.1, 
-000008f0: 302e 312c 2030 2e31 2c20 302e 312c 2030  0.1, 0.1, 0.1, 0
-00000900: 2e31 5d0d 0a20 2020 2020 2020 2020 2020  .1]..           
-00000910: 2020 2020 2066 6f72 2066 2c20 732c 2069       for f, s, i
-00000920: 6478 2069 6e20 7a69 7028 6669 6c65 5f6c  dx in zip(file_l
-00000930: 6973 742c 2073 6361 6c69 6e67 5f6c 6973  ist, scaling_lis
-00000940: 742c 2072 616e 6765 286c 656e 2866 696c  t, range(len(fil
-00000950: 655f 6c69 7374 2929 293a 0d0a 2020 2020  e_list))):..    
-00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000970: 696d 6167 6520 3d20 6c61 6d62 6461 5f6c  image = lambda_l
-00000980: 6f61 645f 6469 636f 6d28 662e 7570 7065  oad_dicom(f.uppe
-00000990: 7228 2929 0d0a 2020 2020 2020 2020 2020  r())..          
-000009a0: 2020 2020 2020 2020 2020 7772 6974 655f            write_
-000009b0: 6469 636f 6d5f 7365 7269 6573 2869 6d61  dicom_series(ima
-000009c0: 6765 2c20 7365 6c66 2e72 6177 5f73 6572  ge, self.raw_ser
-000009d0: 6965 732c 2066 2761 736c 2d7b 667d 272c  ies, f'asl-{f}',
-000009e0: 2063 7572 5f73 6572 6965 735f 6e75 6d62   cur_series_numb
-000009f0: 6572 2c0d 0a20 2020 2020 2020 2020 2020  er,..           
-00000a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a10: 2020 2020 2020 2020 2020 2020 6f73 2e70              os.p
-00000a20: 6174 682e 6a6f 696e 2873 656c 662e 6f75  ath.join(self.ou
-00000a30: 7470 7574 5f72 6f6f 742c 2027 6173 6c27  tput_root, 'asl'
-00000a40: 2c20 6629 2c20 736c 6f70 653d 7329 0d0a  , f), slope=s)..
-00000a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a60: 2020 2020 6375 725f 7365 7269 6573 5f6e      cur_series_n
-00000a70: 756d 6265 7220 2b3d 2031 0d0a 0d0a 2020  umber += 1....  
-00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a90: 2020 6966 2070 6172 616d 5f61 7272 6179    if param_array
-00000aa0: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00000ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ac0: 2020 2070 6172 616d 5f61 7272 6179 203d     param_array =
-00000ad0: 206e 702e 7a65 726f 7328 6c69 7374 2869   np.zeros(list(i
-00000ae0: 6d61 6765 2e73 6861 7065 2920 2b20 5b39  mage.shape) + [9
-00000af0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00000b00: 2020 2020 2020 2020 7061 7261 6d5f 6172          param_ar
-00000b10: 7261 795b 2e2e 2e2c 2069 6478 5d20 3d20  ray[..., idx] = 
-00000b20: 696d 6167 650d 0a0d 0a20 2020 2020 2020  image....       
-00000b30: 2020 2020 2020 2020 2023 20e5 908e 35e4           # ...5.
-00000b40: b8aa e698 af43 4246 312d 35ef bc8c e7ac  .....CBF1-5.....
-00000b50: ac33 e4b8 aae6 98af 4154 540d 0a20 2020  .3......ATT..   
-00000b60: 2020 2020 2020 2020 2020 2020 2073 7570               sup
-00000b70: 6572 2829 2e63 616c 635f 636f 7272 6563  er().calc_correc
-00000b80: 745f 4342 4628 7061 7261 6d5f 6172 7261  t_CBF(param_arra
-00000b90: 795b 2e2e 2e2c 2d35 3a5d 202a 2030 2e31  y[...,-5:] * 0.1
-00000ba0: 2c20 7365 6c66 2e72 6177 5f73 6572 6965  , self.raw_serie
-00000bb0: 732c 2063 7572 5f73 6572 6965 735f 6e75  s, cur_series_nu
-00000bc0: 6d62 6572 290d 0a0d 0a20 2020 2020 2020  mber)....       
-00000bd0: 2020 2020 2065 6c69 6620 6c65 6e28 7365       elif len(se
-00000be0: 6c66 2e64 656c 6179 5f74 696d 6529 203d  lf.delay_time) =
-00000bf0: 3d20 313a 0d0a 2020 2020 2020 2020 2020  = 1:..          
-00000c00: 2020 2020 2020 696d 6167 6520 3d20 6c61        image = la
-00000c10: 6d62 6461 5f6c 6f61 645f 6469 636f 6d28  mbda_load_dicom(
-00000c20: 274d 3027 290d 0a20 2020 2020 2020 2020  'M0')..         
-00000c30: 2020 2020 2020 2077 7269 7465 5f64 6963         write_dic
-00000c40: 6f6d 5f73 6572 6965 7328 696d 6167 652c  om_series(image,
-00000c50: 2073 656c 662e 7261 775f 7365 7269 6573   self.raw_series
-00000c60: 2c20 6627 6173 6c2d 6d30 272c 2063 7572  , f'asl-m0', cur
-00000c70: 5f73 6572 6965 735f 6e75 6d62 6572 2c0d  _series_number,.
-00000c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ca0: 2020 2020 6f73 2e70 6174 682e 6a6f 696e      os.path.join
-00000cb0: 2873 656c 662e 6f75 7470 7574 5f72 6f6f  (self.output_roo
-00000cc0: 742c 2027 6173 6c27 2c20 276d 3027 292c  t, 'asl', 'm0'),
-00000cd0: 2073 6c6f 7065 3d31 290d 0a20 2020 2020   slope=1)..     
-00000ce0: 2020 2020 2020 2020 2020 2063 7572 5f73             cur_s
-00000cf0: 6572 6965 735f 6e75 6d62 6572 202b 3d20  eries_number += 
-00000d00: 310d 0a0d 0a20 2020 2020 2020 2020 2020  1....           
-00000d10: 2020 2020 2069 6d61 6765 203d 206c 616d       image = lam
-00000d20: 6264 615f 6c6f 6164 5f64 6963 6f6d 2827  bda_load_dicom('
-00000d30: 4342 4627 290d 0a20 2020 2020 2020 2020  CBF')..         
-00000d40: 2020 2020 2020 2077 7269 7465 5f64 6963         write_dic
-00000d50: 6f6d 5f73 6572 6965 7328 696d 6167 652c  om_series(image,
-00000d60: 2073 656c 662e 7261 775f 7365 7269 6573   self.raw_series
-00000d70: 2c20 6627 6173 6c2d 6362 6631 272c 2063  , f'asl-cbf1', c
-00000d80: 7572 5f73 6572 6965 735f 6e75 6d62 6572  ur_series_number
-00000d90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000db0: 2020 2020 2020 6f73 2e70 6174 682e 6a6f        os.path.jo
-00000dc0: 696e 2873 656c 662e 6f75 7470 7574 5f72  in(self.output_r
-00000dd0: 6f6f 742c 2027 6173 6c27 2c20 2763 6266  oot, 'asl', 'cbf
-00000de0: 3127 292c 2073 6c6f 7065 3d30 2e31 290d  1'), slope=0.1).
-00000df0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00000e00: 2020 2073 7570 6572 2829 2e63 616c 635f     super().calc_
-00000e10: 636f 7272 6563 745f 4342 4628 696d 6167  correct_CBF(imag
-00000e20: 6520 2a20 302e 312c 2073 656c 662e 7261  e * 0.1, self.ra
-00000e30: 775f 7365 7269 6573 2c20 6375 725f 7365  w_series, cur_se
-00000e40: 7269 6573 5f6e 756d 6265 7220 2b20 3129  ries_number + 1)
-00000e50: 0d0a 0d0a 2020 2020 2020 2020 6578 6365  ....        exce
-00000e60: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00000e70: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00000e80: 6c6f 6767 6572 2e65 7272 6f72 2865 290d  logger.error(e).
-00000e90: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00000ea0: 7365 2065 0d0a 2020 2020 2020 2020 6669  se e..        fi
-00000eb0: 6e61 6c6c 793a 0d0a 2020 2020 2020 2020  nally:..        
-00000ec0: 2020 2020 7368 7574 696c 2e72 6d74 7265      shutil.rmtre
-00000ed0: 6528 6a61 7661 5f74 656d 7029 0d0a 0d0a  e(java_temp)....
-00000ee0: 2020 2020 6465 6620 6765 6e65 7261 7465      def generate
-00000ef0: 5f66 726f 6d5f 7261 775f 666f 6c64 6572  _from_raw_folder
-00000f00: 2873 656c 662c 2074 656d 705f 6469 7229  (self, temp_dir)
-00000f10: 3a0d 0a20 2020 2020 2020 2023 2070 7269  :..        # pri
-00000f20: 6e74 2822 e5b1 82e6 95b0 203d 207b 3a64  nt("...... = {:d
-00000f30: 7d22 2e66 6f72 6d61 7428 7365 6c66 2e73  }".format(self.s
-00000f40: 6c69 6365 5f6e 756d 2929 0d0a 2020 2020  lice_num))..    
-00000f50: 2020 2020 6f73 2e6d 616b 6564 6972 7328      os.makedirs(
-00000f60: 6f73 2e70 6174 682e 6a6f 696e 2874 656d  os.path.join(tem
-00000f70: 705f 6469 722c 2022 7265 6f72 6465 7265  p_dir, "reordere
-00000f80: 6422 292c 2065 7869 7374 5f6f 6b3d 5472  d"), exist_ok=Tr
-00000f90: 7565 290d 0a20 2020 2020 2020 206f 732e  ue)..        os.
-00000fa0: 6d61 6b65 6469 7273 286f 732e 7061 7468  makedirs(os.path
-00000fb0: 2e6a 6f69 6e28 7465 6d70 5f64 6972 2c20  .join(temp_dir, 
-00000fc0: 2272 6563 6f6e 7374 7275 6374 6564 2229  "reconstructed")
-00000fd0: 2c20 6578 6973 745f 6f6b 3d54 7275 6529  , exist_ok=True)
-00000fe0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00000ff0: 6d61 6b65 5f6a 736f 6e28 290d 0a0d 0a20  make_json().... 
-00001000: 2020 2020 2020 2066 6f72 2069 2c20 696e         for i, in
-00001010: 7374 616e 6365 2069 6e20 656e 756d 6572  stance in enumer
-00001020: 6174 6528 7365 6c66 2e72 6177 5f73 6572  ate(self.raw_ser
-00001030: 6965 7329 3a0d 0a20 2020 2020 2020 2020  ies):..         
-00001040: 2020 2069 6e73 7461 6e63 652e 7361 7665     instance.save
-00001050: 5f61 7328 6f73 2e70 6174 682e 6a6f 696e  _as(os.path.join
-00001060: 2874 656d 705f 6469 722c 2022 7265 6f72  (temp_dir, "reor
-00001070: 6465 7265 6422 2c20 2274 656d 705f 6463  dered", "temp_dc
-00001080: 6d5f 7b3a 3034 647d 2e64 636d 222e 666f  m_{:04d}.dcm".fo
-00001090: 726d 6174 2869 2929 290d 0a20 2020 2020  rmat(i)))..     
-000010a0: 2020 206a 6172 5f66 6f6c 6465 7220 3d20     jar_folder = 
-000010b0: 6f73 2e70 6174 682e 6a6f 696e 286f 732e  os.path.join(os.
-000010c0: 6765 7463 7764 2829 2c20 2255 434c 415f  getcwd(), "UCLA_
-000010d0: 6a61 7661 5f6a 6172 2229 0d0a 0d0a 2020  java_jar")....  
-000010e0: 2020 2020 2020 7072 696e 7428 6a61 725f        print(jar_
-000010f0: 666f 6c64 6572 290d 0a20 2020 2020 2020  folder)..       
-00001100: 2072 6573 706f 6e73 6520 3d20 7375 6270   response = subp
-00001110: 726f 6365 7373 2e72 756e 280d 0a20 2020  rocess.run(..   
-00001120: 2020 2020 2020 2020 205b 0d0a 2020 2020           [..    
-00001130: 2020 2020 2020 2020 2020 2020 226a 6176              "jav
-00001140: 6122 2c20 222d 6a61 7222 2c0d 0a20 2020  a", "-jar",..   
-00001150: 2020 2020 2020 2020 2020 2020 2022 2d44               "-D
-00001160: 6a61 7661 2e6c 6962 7261 7279 2e70 6174  java.library.pat
-00001170: 683d 7b7d 222e 666f 726d 6174 286f 732e  h={}".format(os.
-00001180: 7061 7468 2e6a 6f69 6e28 6a61 725f 666f  path.join(jar_fo
-00001190: 6c64 6572 2c20 226c 6962 2229 292c 0d0a  lder, "lib")),..
-000011a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011b0: 6f73 2e70 6174 682e 6a6f 696e 286a 6172  os.path.join(jar
-000011c0: 5f66 6f6c 6465 722c 2022 4153 4c5f 7961  _folder, "ASL_ya
-000011d0: 6f5f 4a41 5641 2d6d 6173 7465 722e 6a61  o_JAVA-master.ja
-000011e0: 7222 292c 0d0a 2020 2020 2020 2020 2020  r"),..          
-000011f0: 2020 2020 2020 6f73 2e70 6174 682e 6a6f        os.path.jo
-00001200: 696e 2874 656d 705f 6469 722c 2022 7061  in(temp_dir, "pa
-00001210: 7261 6d2e 6a73 6f6e 2229 0d0a 2020 2020  ram.json")..    
-00001220: 2020 2020 2020 2020 5d0d 0a20 2020 2020          ]..     
-00001230: 2020 2029 0d0a 2020 2020 2020 2020 6966     )..        if
-00001240: 2072 6573 706f 6e73 652e 7265 7475 726e   response.return
-00001250: 636f 6465 2021 3d20 303a 0d0a 2020 2020  code != 0:..    
-00001260: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
-00001270: 6365 7074 696f 6e28 224a 6176 61e7 a88b  ception("Java...
-00001280: e5ba 8fe8 bf90 e8a1 8ce5 a4b1 e8b4 a5ef  ................
-00001290: bc8c e7bc 96e5 8fb7 3a20 7b3a 647d 222e  ........: {:d}".
-000012a0: 666f 726d 6174 2872 6573 706f 6e73 652e  format(response.
-000012b0: 7265 7475 726e 636f 6465 2929 0d0a 0d0a  returncode))....
-000012c0: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
-000012d0: 7468 2e69 7366 696c 6528 6f73 2e70 6174  th.isfile(os.pat
-000012e0: 682e 6a6f 696e 2873 656c 662e 6f75 7470  h.join(self.outp
-000012f0: 7574 5f72 6f6f 742c 2022 6a61 7661 5f74  ut_root, "java_t
-00001300: 656d 7022 2c20 2272 6563 6f6e 7374 7275  emp", "reconstru
-00001310: 6374 6564 222c 2022 6669 6e69 7368 6564  cted", "finished
-00001320: 2e74 7874 2229 293a 0d0a 2020 2020 2020  .txt")):..      
-00001330: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00001340: 7567 2822 e5ae 8ce6 8890 e794 a84a 6176  ug(".........Jav
-00001350: 61e7 9a84 e59b bee5 838f e987 8de5 bbba  a...............
-00001360: efbc 8ce5 bc80 e5a7 8be7 94a8 5079 7468  ............Pyth
-00001370: 6f6e e69d a5e8 b083 e695 b4e6 a087 e7ad  on..............
-00001380: be22 290d 0a0d 0a20 2020 2020 2020 2072  .")....        r
-00001390: 6574 7572 6e20 6f73 2e70 6174 682e 6a6f  eturn os.path.jo
-000013a0: 696e 2874 656d 705f 6469 722c 2022 7265  in(temp_dir, "re
-000013b0: 636f 6e73 7472 7563 7465 6422 290d 0a0d  constructed")...
-000013c0: 0a20 2020 2064 6566 205f 7361 7665 5f68  .    def _save_h
-000013d0: 6561 645f 6d6f 7469 6f6e 5f67 7261 7068  ead_motion_graph
-000013e0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-000013f0: 2066 696c 655f 7061 7468 203d 206f 732e   file_path = os.
-00001400: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e6f  path.join(self.o
-00001410: 7574 7075 745f 726f 6f74 2c20 226a 6176  utput_root, "jav
-00001420: 615f 7465 6d70 222c 2022 7265 636f 6e73  a_temp", "recons
-00001430: 7472 7563 7465 6422 2c20 2268 6561 644d  tructed", "headM
-00001440: 6f74 696f 6e2e 6a73 6f6e 2229 0d0a 2020  otion.json")..  
-00001450: 2020 2020 2020 7361 7665 5f70 6174 6820        save_path 
-00001460: 3d20 6f73 2e70 6174 682e 6a6f 696e 2873  = os.path.join(s
-00001470: 656c 662e 6f75 7470 7574 5f72 6f6f 742c  elf.output_root,
-00001480: 2022 6865 6164 4d6f 7469 6f6e 2e70 6e67   "headMotion.png
-00001490: 2229 0d0a 2020 2020 2020 2020 7769 7468  ")..        with
-000014a0: 206f 7065 6e28 6669 6c65 5f70 6174 682c   open(file_path,
-000014b0: 2027 7227 2920 6173 2066 3a0d 0a20 2020   'r') as f:..   
-000014c0: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-000014d0: 6a73 6f6e 2e6c 6f61 6428 6629 0d0a 2020  json.load(f)..  
-000014e0: 2020 2020 2020 2320 7072 696e 7428 6461        # print(da
-000014f0: 7461 290d 0a20 2020 2020 2020 2066 6967  ta)..        fig
-00001500: 203d 2070 6c74 2e66 6967 7572 6528 290d   = plt.figure().
-00001510: 0a20 2020 2020 2020 206d 6174 706c 6f74  .        matplot
-00001520: 6c69 622e 7263 5061 7261 6d73 5b27 666f  lib.rcParams['fo
-00001530: 6e74 2e66 616d 696c 7927 5d20 3d20 2273  nt.family'] = "s
-00001540: 696d 7375 6e22 0d0a 2020 2020 2020 2020  imsun"..        
-00001550: 6669 672e 7365 745f 7369 7a65 5f69 6e63  fig.set_size_inc
-00001560: 6865 7328 362c 2032 290d 0a20 2020 2020  hes(6, 2)..     
-00001570: 2020 2078 6461 7461 203d 206e 702e 6c69     xdata = np.li
-00001580: 6e73 7061 6365 2831 2c20 6c65 6e28 6461  nspace(1, len(da
-00001590: 7461 5b22 636f 6e74 726f 6c46 4422 5d29  ta["controlFD"])
-000015a0: 2c20 6c65 6e28 6461 7461 5b22 636f 6e74  , len(data["cont
-000015b0: 726f 6c46 4422 5d29 290d 0a20 2020 2020  rolFD"]))..     
-000015c0: 2020 2070 6c74 2e70 6c6f 7428 7864 6174     plt.plot(xdat
-000015d0: 612c 2064 6174 615b 2263 6f6e 7472 6f6c  a, data["control
-000015e0: 4644 225d 2c20 2762 6f2d 272c 206c 6162  FD"], 'bo-', lab
-000015f0: 656c 3d27 e697 a0e6 a087 e8ae b0e5 838f  el='............
-00001600: 2729 0d0a 2020 2020 2020 2020 706c 742e  ')..        plt.
-00001610: 706c 6f74 2878 6461 7461 2c20 6461 7461  plot(xdata, data
-00001620: 5b22 6c61 6265 6c46 4422 5d2c 2027 726f  ["labelFD"], 'ro
-00001630: 2d27 2c20 6c61 6265 6c3d 27e6 a087 e8ae  -', label='.....
-00001640: b0e5 838f 2729 0d0a 2020 2020 2020 2020  ....')..        
-00001650: 706c 742e 7874 6963 6b73 2878 6461 7461  plt.xticks(xdata
-00001660: 290d 0a20 2020 2020 2020 2070 6c74 2e78  )..        plt.x
-00001670: 6c61 6265 6c28 22e5 9bbe e789 87e5 ba8f  label(".........
-00001680: e58f b722 290d 0a20 2020 2020 2020 2070  ...")..        p
-00001690: 6c74 2e79 6c61 6265 6c28 22e5 a4b4 e58a  lt.ylabel(".....
-000016a0: a828 6d6d 2922 290d 0a20 2020 2020 2020  .(mm)")..       
-000016b0: 2070 6c74 2e6c 6567 656e 6428 290d 0a20   plt.legend().. 
-000016c0: 2020 2020 2020 2070 6c74 2e74 6967 6874         plt.tight
-000016d0: 5f6c 6179 6f75 7428 290d 0a20 2020 2020  _layout()..     
-000016e0: 2020 2070 6c74 2e73 6176 6566 6967 2873     plt.savefig(s
-000016f0: 6176 655f 7061 7468 2c20 6470 693d 3230  ave_path, dpi=20
-00001700: 3029 0d0a 2020 2020 2020 2020 706c 742e  0)..        plt.
-00001710: 6669 6775 7265 2829 2e63 6c65 6172 2829  figure().clear()
-00001720: 0d0a 2020 2020 2020 2020 706c 742e 636c  ..        plt.cl
-00001730: 6f73 6528 290d 0a20 2020 2020 2020 2070  ose()..        p
-00001740: 6c74 2e63 6c61 2829 0d0a 2020 2020 2020  lt.cla()..      
-00001750: 2020 706c 742e 636c 6628 290d 0a0d 0a20    plt.clf().... 
-00001760: 2020 2064 6566 205f 6d61 6b65 5f6a 736f     def _make_jso
-00001770: 6e28 7365 6c66 293a 0d0a 2020 2020 2020  n(self):..      
-00001780: 2020 7365 6c66 2e72 6177 5f73 6572 6965    self.raw_serie
-00001790: 733a 2053 6572 6965 734d 6f64 656c 0d0a  s: SeriesModel..
-000017a0: 2020 2020 2020 2020 6465 6c61 795f 6e75          delay_nu
-000017b0: 6d20 3d20 6c65 6e28 7365 6c66 2e64 656c  m = len(self.del
-000017c0: 6179 5f74 696d 6529 0d0a 2020 2020 2020  ay_time)..      
-000017d0: 2020 6966 2064 656c 6179 5f6e 756d 203d    if delay_num =
-000017e0: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
-000017f0: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
-00001800: 6e28 2764 656c 6179 5f74 696d 6520 6973  n('delay_time is
-00001810: 206e 756c 6c27 290d 0a20 2020 2020 2020   null')..       
-00001820: 2069 6620 6465 6c61 795f 6e75 6d20 213d   if delay_num !=
-00001830: 206c 656e 2873 656c 662e 6465 6c61 795f   len(self.delay_
-00001840: 7265 7029 3a0d 0a20 2020 2020 2020 2020  rep):..         
-00001850: 2020 2072 6169 7365 2044 656c 6179 4e6f     raise DelayNo
-00001860: 7445 7175 616c 5265 7065 7469 7469 6f6e  tEqualRepetition
-00001870: 4572 726f 7228 6465 6c61 795f 6e75 6d2c  Error(delay_num,
-00001880: 206c 656e 2873 656c 662e 6465 6c61 795f   len(self.delay_
-00001890: 7265 7029 290d 0a0d 0a20 2020 2020 2020  rep))....       
-000018a0: 2070 6172 616d 5f6a 736f 6e5f 6469 6374   param_json_dict
-000018b0: 203d 207b 0d0a 2020 2020 2020 2020 2020   = {..          
-000018c0: 2020 2264 6174 615f 7479 7065 223a 2027    "data_type": '
-000018d0: 3564 656c 6179 5f6d 6f73 6169 6327 2069  5delay_mosaic' i
-000018e0: 6620 7365 6c66 2e64 6174 615f 7479 7065  f self.data_type
-000018f0: 2069 6e20 5b4d 5249 5f54 7970 652e 4d52   in [MRI_Type.MR
-00001900: 495f 5459 5045 5f35 4465 6c61 795f 3344  I_TYPE_5Delay_3D
-00001910: 5f50 4341 534c 5f53 4945 4d45 4e53 2c0d  _PCASL_SIEMENS,.
-00001920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001960: 4d52 495f 5479 7065 2e4d 5249 5f54 5950  MRI_Type.MRI_TYP
-00001970: 455f 3144 656c 6179 5f33 445f 5043 4153  E_1Delay_3D_PCAS
-00001980: 4c5f 5349 454d 454e 535d 2065 6c73 6520  L_SIEMENS] else 
-00001990: 2734 6465 6c61 795f 3364 272c 0d0a 2020  '4delay_3d',..  
-000019a0: 2020 2020 2020 2020 2020 2273 6c69 6365            "slice
-000019b0: 5f6f 7264 6572 223a 2027 6173 6365 6e64  _order": 'ascend
-000019c0: 696e 6727 2c20 2320 e6ad a4e5 8f82 e695  ing', # ........
-000019d0: b0e5 b7b2 e4b8 8de9 878d e8a6 810d 0a20  ............... 
-000019e0: 2020 2020 2020 2020 2020 2022 736c 6963             "slic
-000019f0: 655f 6e75 6d22 3a20 7365 6c66 2e72 6177  e_num": self.raw
-00001a00: 5f73 6572 6965 732e 536c 6963 654e 756d  _series.SliceNum
-00001a10: 6265 722c 0d0a 2020 2020 2020 2020 2020  ber,..          
-00001a20: 2020 2269 6e69 745f 6465 6c61 7922 3a20    "init_delay": 
-00001a30: 7365 6c66 2e64 656c 6179 5f74 696d 655b  self.delay_time[
-00001a40: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
-00001a50: 2022 6465 6c61 795f 6e75 6d22 3a20 6465   "delay_num": de
-00001a60: 6c61 795f 6e75 6d2c 0d0a 2020 2020 2020  lay_num,..      
-00001a70: 2020 2020 2020 2269 6e74 6572 7661 6c22        "interval"
-00001a80: 3a20 7365 6c66 2e64 656c 6179 5f74 696d  : self.delay_tim
-00001a90: 655b 315d 202d 2073 656c 662e 6465 6c61  e[1] - self.dela
-00001aa0: 795f 7469 6d65 5b30 5d20 6966 2064 656c  y_time[0] if del
-00001ab0: 6179 5f6e 756d 203e 3d20 3220 656c 7365  ay_num >= 2 else
-00001ac0: 2030 2e30 2c0d 0a20 2020 2020 2020 2020   0.0,..         
-00001ad0: 2020 2022 6465 6c61 795f 7265 7022 3a20     "delay_rep": 
-00001ae0: 7365 6c66 2e64 656c 6179 5f72 6570 2c0d  self.delay_rep,.
-00001af0: 0a20 2020 2020 2020 2020 2020 2022 6c6f  .            "lo
-00001b00: 6164 5f70 6174 6822 3a20 6f73 2e70 6174  ad_path": os.pat
-00001b10: 682e 6a6f 696e 2873 656c 662e 6f75 7470  h.join(self.outp
-00001b20: 7574 5f72 6f6f 742c 2022 6a61 7661 5f74  ut_root, "java_t
-00001b30: 656d 7022 2c20 2272 656f 7264 6572 6564  emp", "reordered
-00001b40: 2229 2c0d 0a20 2020 2020 2020 2020 2020  "),..           
-00001b50: 2022 7361 7665 5f70 6174 6822 3a20 6f73   "save_path": os
-00001b60: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
-00001b70: 6f75 7470 7574 5f72 6f6f 742c 2022 6a61  output_root, "ja
-00001b80: 7661 5f74 656d 7022 2c20 2272 6563 6f6e  va_temp", "recon
-00001b90: 7374 7275 6374 6564 2229 7d0d 0a0d 0a20  structed")}.... 
-00001ba0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-00001bb0: 286f 732e 7061 7468 2e6a 6f69 6e28 7365  (os.path.join(se
-00001bc0: 6c66 2e6f 7574 7075 745f 726f 6f74 2c20  lf.output_root, 
-00001bd0: 226a 6176 615f 7465 6d70 222c 2022 7061  "java_temp", "pa
-00001be0: 7261 6d2e 6a73 6f6e 2229 2c20 2277 2229  ram.json"), "w")
-00001bf0: 2061 7320 6670 3a0d 0a20 2020 2020 2020   as fp:..       
-00001c00: 2020 2020 206a 736f 6e2e 6475 6d70 2870       json.dump(p
-00001c10: 6172 616d 5f6a 736f 6e5f 6469 6374 2c20  aram_json_dict, 
-00001c20: 6670 2c20 696e 6465 6e74 3d34 290d 0a20  fp, indent=4).. 
-00001c30: 2020 2020 2020 2070 7269 6e74 2822 6a73         print("js
-00001c40: 6f6e e696 87e4 bbb6 e4bf 9de5 ad98 2229  on............")
-00001c50: 0d0a 0d0a 2020 2020 4073 7461 7469 636d  ....    @staticm
-00001c60: 6574 686f 640d 0a20 2020 2064 6566 205f  ethod..    def _
-00001c70: 3344 5f74 6f5f 6d6f 7361 6963 2861 7272  3D_to_mosaic(arr
-00001c80: 6179 3a20 6e70 2e6e 6461 7272 6179 293a  ay: np.ndarray):
-00001c90: 0d0a 2020 2020 2020 2020 7769 6474 6820  ..        width 
-00001ca0: 3d20 6865 6967 6874 203d 2069 6e74 286e  = height = int(n
-00001cb0: 702e 6365 696c 2861 7272 6179 2e73 6861  p.ceil(array.sha
-00001cc0: 7065 5b32 5d29 290d 0a20 2020 2020 2020  pe[2]))..       
-00001cd0: 2064 6566 2067 6574 5f73 6c69 6365 2861   def get_slice(a
-00001ce0: 7272 6179 3a20 6e70 2e6e 6461 7272 6179  rray: np.ndarray
-00001cf0: 2c20 736c 6963 653a 2069 6e74 293a 0d0a  , slice: int):..
-00001d00: 2020 2020 2020 2020 2020 2020 2320 e8b6              # ..
-00001d10: 85e5 87ba e88c 83e5 9bb4 e794 a820 30e5  ............. 0.
-00001d20: 80bc e5a1 abe5 8585 0d0a 2020 2020 2020  ..........      
-00001d30: 2020 2020 2020 6966 2061 7272 6179 2e73        if array.s
-00001d40: 6861 7065 5b32 5d20 3e20 736c 6963 653a  hape[2] > slice:
-00001d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001d60: 2020 7265 7475 726e 2061 7272 6179 5b3a    return array[:
-00001d70: 2c20 3a2c 2073 6c69 6365 5d0d 0a20 2020  , :, slice]..   
-00001d80: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001da0: 7265 7475 726e 206e 702e 7a65 726f 7328  return np.zeros(
-00001db0: 6172 7261 795b 3a2c 203a 2c20 305d 2e73  array[:, :, 0].s
-00001dc0: 6861 7065 2c20 6474 7970 653d 6172 7261  hape, dtype=arra
-00001dd0: 792e 6474 7970 6529 0d0a 0d0a 2020 2020  y.dtype)....    
-00001de0: 2020 2020 726f 775f 696d 675f 7665 6374      row_img_vect
-00001df0: 6f72 203d 205b 5d0d 0a20 2020 2020 2020  or = []..       
-00001e00: 2066 6f72 206f 6666 7365 7420 696e 2072   for offset in r
-00001e10: 616e 6765 2877 6964 7468 293a 0d0a 2020  ange(width):..  
-00001e20: 2020 2020 2020 2020 2020 636f 6c5f 696e            col_in
-00001e30: 6465 7820 3d20 7475 706c 6528 5b69 202a  dex = tuple([i *
-00001e40: 2077 6964 7468 202b 206f 6666 7365 7420   width + offset 
-00001e50: 666f 7220 6920 696e 2072 616e 6765 2868  for i in range(h
-00001e60: 6569 6768 7429 5d29 0d0a 2020 2020 2020  eight)])..      
-00001e70: 2020 2020 2020 636f 6c5f 696d 6720 3d20        col_img = 
-00001e80: 6e70 2e76 7374 6163 6b28 5b67 6574 5f73  np.vstack([get_s
-00001e90: 6c69 6365 2861 7272 6179 2c20 6329 2066  lice(array, c) f
-00001ea0: 6f72 2063 2069 6e20 636f 6c5f 696e 6465  or c in col_inde
-00001eb0: 785d 290d 0a20 2020 2020 2020 2020 2020  x])..           
-00001ec0: 2072 6f77 5f69 6d67 5f76 6563 746f 722e   row_img_vector.
-00001ed0: 6170 7065 6e64 2863 6f6c 5f69 6d67 290d  append(col_img).
-00001ee0: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-00001ef0: 6e20 6e70 2e68 7374 6163 6b28 726f 775f  n np.hstack(row_
-00001f00: 696d 675f 7665 6374 6f72 290d 0a0d 0a    img_vector)....
+00000010: 6d70 6f72 7420 7375 6270 726f 6365 7373  mport subprocess
+00000020: 0d0a 0d0a 696d 706f 7274 206d 6174 706c  ....import matpl
+00000030: 6f74 6c69 620d 0a69 6d70 6f72 7420 6d61  otlib..import ma
+00000040: 7470 6c6f 746c 6962 2e70 7970 6c6f 7420  tplotlib.pyplot 
+00000050: 6173 2070 6c74 0d0a 0d0a 6672 6f6d 202e  as plt....from .
+00000060: 5f64 6963 6f6d 2069 6d70 6f72 7420 2a0d  _dicom import *.
+00000070: 0a66 726f 6d20 2e5f 6469 636f 6d5f 7574  .from ._dicom_ut
+00000080: 696c 2069 6d70 6f72 7420 7772 6974 655f  il import write_
+00000090: 6469 636f 6d5f 7365 7269 6573 0d0a 6672  dicom_series..fr
+000000a0: 6f6d 202e 6461 7461 5f73 6f72 7465 725f  om .data_sorter_
+000000b0: 6261 7365 2069 6d70 6f72 7420 4461 7461  base import Data
+000000c0: 536f 7274 6572 4153 4c42 6173 650d 0a0d  SorterASLBase...
+000000d0: 0a0d 0a63 6c61 7373 2044 6174 6153 6f72  ...class DataSor
+000000e0: 7465 7253 6965 6d65 6e73 5043 4153 4c28  terSiemensPCASL(
+000000f0: 4461 7461 536f 7274 6572 4153 4c42 6173  DataSorterASLBas
+00000100: 6529 3a0d 0a20 2020 2064 6566 205f 5f69  e):..    def __i
+00000110: 6e69 745f 5f28 7365 6c66 2c20 6461 7461  nit__(self, data
+00000120: 5f74 7970 652c 206f 7574 7075 745f 726f  _type, output_ro
+00000130: 6f74 2c20 6465 6c61 795f 7469 6d65 2c20  ot, delay_time, 
+00000140: 6465 6c61 795f 7265 702c 206c 6162 656c  delay_rep, label
+00000150: 5f64 7572 2c20 7365 7269 6573 5f6c 6973  _dur, series_lis
+00000160: 742c 2063 616c 635f 635f 6362 6629 3a0d  t, calc_c_cbf):.
+00000170: 0a20 2020 2020 2020 2044 6174 6153 6f72  .        DataSor
+00000180: 7465 7241 534c 4261 7365 2e5f 5f69 6e69  terASLBase.__ini
+00000190: 745f 5f28 7365 6c66 2c20 6461 7461 5f74  t__(self, data_t
+000001a0: 7970 652c 206f 7574 7075 745f 726f 6f74  ype, output_root
+000001b0: 2c20 6465 6c61 795f 7469 6d65 2c20 6465  , delay_time, de
+000001c0: 6c61 795f 7265 702c 206c 6162 656c 5f64  lay_rep, label_d
+000001d0: 7572 2c20 7365 7269 6573 5f6c 6973 742c  ur, series_list,
+000001e0: 2063 616c 635f 635f 6362 6629 0d0a 0d0a   calc_c_cbf)....
+000001f0: 2020 2020 2020 2020 6465 6c61 795f 6e75          delay_nu
+00000200: 6d20 3d20 6c65 6e28 7365 6c66 2e64 656c  m = len(self.del
+00000210: 6179 5f74 696d 6529 0d0a 2020 2020 2020  ay_time)..      
+00000220: 2020 7265 705f 6e75 6d20 3d20 6c65 6e28    rep_num = len(
+00000230: 7365 6c66 2e64 656c 6179 5f72 6570 290d  self.delay_rep).
+00000240: 0a20 2020 2020 2020 2069 6620 6465 6c61  .        if dela
+00000250: 795f 6e75 6d20 213d 2072 6570 5f6e 756d  y_num != rep_num
+00000260: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00000270: 6169 7365 2044 656c 6179 4e6f 7445 7175  aise DelayNotEqu
+00000280: 616c 5265 7065 7469 7469 6f6e 4572 726f  alRepetitionErro
+00000290: 7228 6465 6c61 795f 6e75 6d2c 2072 6570  r(delay_num, rep
+000002a0: 5f6e 756d 290d 0a0d 0a20 2020 2020 2020  _num)....       
+000002b0: 2069 6620 7365 6c66 2e64 6174 615f 7479   if self.data_ty
+000002c0: 7065 203d 3d20 4d52 495f 5479 7065 2e4d  pe == MRI_Type.M
+000002d0: 5249 5f54 5950 455f 3544 656c 6179 5f33  RI_TYPE_5Delay_3
+000002e0: 445f 5043 4153 4c5f 5349 454d 454e 5320  D_PCASL_SIEMENS 
+000002f0: 616e 6420 6465 6c61 795f 6e75 6d20 213d  and delay_num !=
+00000300: 2035 3a0d 0a20 2020 2020 2020 2020 2020   5:..           
+00000310: 2072 6169 7365 2044 656c 6179 4e6f 7445   raise DelayNotE
+00000320: 7175 616c 5365 7269 6573 4e75 6d62 6572  qualSeriesNumber
+00000330: 4572 726f 7228 6465 6c61 795f 6e75 6d2c  Error(delay_num,
+00000340: 2035 290d 0a20 2020 2020 2020 2069 6620   5)..        if 
+00000350: 7365 6c66 2e64 6174 615f 7479 7065 203d  self.data_type =
+00000360: 3d20 4d52 495f 5479 7065 2e4d 5249 5f54  = MRI_Type.MRI_T
+00000370: 5950 455f 3144 656c 6179 5f33 445f 5043  YPE_1Delay_3D_PC
+00000380: 4153 4c5f 5349 454d 454e 5320 616e 6420  ASL_SIEMENS and 
+00000390: 6465 6c61 795f 6e75 6d20 213d 2031 3a0d  delay_num != 1:.
+000003a0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+000003b0: 7365 2044 656c 6179 4e6f 7445 7175 616c  se DelayNotEqual
+000003c0: 5365 7269 6573 4e75 6d62 6572 4572 726f  SeriesNumberErro
+000003d0: 7228 6465 6c61 795f 6e75 6d2c 2031 290d  r(delay_num, 1).
+000003e0: 0a0d 0a0d 0a20 2020 2020 2020 2023 2050  .....        # P
+000003f0: 5749 e59b bee5 a682 e69e 9ce8 a2ab e58c  WI..............
+00000400: 85e5 90ab e8bf 9be6 9da5 efbc 8ce6 8e92  ................
+00000410: e999 a4e6 8e89 0d0a 2020 2020 2020 2020  ........        
+00000420: 7365 6c66 2e72 6177 5f73 6572 6965 7320  self.raw_series 
+00000430: 3d20 736f 7274 6564 2873 6572 6965 735f  = sorted(series_
+00000440: 6c69 7374 2c20 6b65 793d 6c61 6d62 6461  list, key=lambda
+00000450: 2078 3a20 6c65 6e28 7829 2c20 7265 7665   x: len(x), reve
+00000460: 7273 653d 5472 7565 295b 305d 0d0a 0d0a  rse=True)[0]....
+00000470: 2020 2020 6465 6620 536f 7274 6572 2873      def Sorter(s
+00000480: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
+00000490: 7570 6572 2844 6174 6153 6f72 7465 7253  uper(DataSorterS
+000004a0: 6965 6d65 6e73 5043 4153 4c2c 2073 656c  iemensPCASL, sel
+000004b0: 6629 2e53 6f72 7465 7228 290d 0a0d 0a20  f).Sorter().... 
+000004c0: 2020 2020 2020 2023 20e5 8d95 e5bb b6e8         # .......
+000004d0: bf9f 5043 4153 4ce9 878d e696 b0e8 aea1  ..PCASL.........
+000004e0: e7ae 97e9 878d e5a4 8de6 aca1 e695 b00d  ................
+000004f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00000500: 2e64 6174 615f 7479 7065 203d 3d20 4d52  .data_type == MR
+00000510: 495f 5479 7065 2e4d 5249 5f54 5950 455f  I_Type.MRI_TYPE_
+00000520: 3144 656c 6179 5f33 445f 5043 4153 4c5f  1Delay_3D_PCASL_
+00000530: 5349 454d 454e 533a 0d0a 2020 2020 2020  SIEMENS:..      
+00000540: 2020 2020 2020 7365 6c66 2e64 656c 6179        self.delay
+00000550: 5f72 6570 203d 205b 7365 6c66 2e72 6177  _rep = [self.raw
+00000560: 5f73 6572 6965 732e 6c6f 6164 2829 2e73  _series.load().s
+00000570: 6861 7065 5b2d 315d 202f 2f20 3220 2d20  hape[-1] // 2 - 
+00000580: 315d 0d0a 0d0a 2020 2020 2020 2020 6a61  1]....        ja
+00000590: 7661 5f74 656d 7020 3d20 6f73 2e70 6174  va_temp = os.pat
+000005a0: 682e 6a6f 696e 2873 656c 662e 6f75 7470  h.join(self.outp
+000005b0: 7574 5f72 6f6f 742c 2027 6a61 7661 5f74  ut_root, 'java_t
+000005c0: 656d 7027 290d 0a20 2020 2020 2020 2074  emp')..        t
+000005d0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+000005e0: 2072 6563 6f6e 7374 7275 6374 6564 5f64   reconstructed_d
+000005f0: 6972 203d 2073 656c 662e 6765 6e65 7261  ir = self.genera
+00000600: 7465 5f66 726f 6d5f 7261 775f 666f 6c64  te_from_raw_fold
+00000610: 6572 286a 6176 615f 7465 6d70 290d 0a20  er(java_temp).. 
+00000620: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00000630: 5f73 6176 655f 6865 6164 5f6d 6f74 696f  _save_head_motio
+00000640: 6e5f 6772 6170 6828 290d 0a0d 0a20 2020  n_graph()....   
+00000650: 2020 2020 2020 2020 2023 20e8 aea1 e7ae           # .....
+00000660: 97e5 ae8c e590 8eef bc8c e5be 97e5 88b0  ................
+00000670: e79a 8432 44e5 a29e e5bc ba44 6963 6f6d  ...2D......Dicom
+00000680: e696 87e4 bbb6 efbc 8ce5 b086 e585 b6e9  ................
+00000690: 878d e695 b4e4 b8ba 3244 2044 6963 6f6d  ........2D Dicom
+000006a0: efbc 9be9 878d e586 99e6 96b9 e590 91ef  ................
+000006b0: bc8c e4bd 8de7 bdae e6a0 87e7 adbe 0d0a  ................
+000006c0: 2020 2020 2020 2020 2020 2020 6465 6620              def 
+000006d0: 6c61 6d62 6461 5f6c 6f61 645f 6469 636f  lambda_load_dico
+000006e0: 6d28 6e61 6d65 293a 0d0a 2020 2020 2020  m(name):..      
+000006f0: 2020 2020 2020 2020 2020 6d61 7420 3d20            mat = 
+00000700: 7079 6469 636f 6d2e 7265 6164 5f66 696c  pydicom.read_fil
+00000710: 6528 6f73 2e70 6174 682e 6a6f 696e 2872  e(os.path.join(r
+00000720: 6563 6f6e 7374 7275 6374 6564 5f64 6972  econstructed_dir
+00000730: 2c20 6e61 6d65 2b27 2e64 636d 2729 292e  , name+'.dcm')).
+00000740: 7069 7865 6c5f 6172 7261 790d 0a20 2020  pixel_array..   
+00000750: 2020 2020 2020 2020 2020 2020 206d 6174               mat
+00000760: 203d 206d 6174 2e73 7761 7061 7865 7328   = mat.swapaxes(
+00000770: 302c 2032 290d 0a20 2020 2020 2020 2020  0, 2)..         
+00000780: 2020 2020 2020 2072 6574 7572 6e20 6d61         return ma
+00000790: 742e 7377 6170 6178 6573 2830 2c20 3129  t.swapaxes(0, 1)
+000007a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000007b0: 6375 725f 7365 7269 6573 5f6e 756d 6265  cur_series_numbe
+000007c0: 7220 3d20 5365 7269 6573 4e75 6d62 6572  r = SeriesNumber
+000007d0: 5374 6172 7457 6974 682e 4153 4c0d 0a20  StartWith.ASL.. 
+000007e0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+000007f0: 6e28 7365 6c66 2e64 656c 6179 5f74 696d  n(self.delay_tim
+00000800: 6529 203d 3d20 353a 0d0a 2020 2020 2020  e) == 5:..      
+00000810: 2020 2020 2020 2020 2020 7061 7261 6d5f            param_
+00000820: 6172 7261 7920 3d20 4e6f 6e65 0d0a 0d0a  array = None....
+00000830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000840: 6669 6c65 5f6c 6973 7420 3d20 5b22 6d30  file_list = ["m0
+00000850: 222c 2022 6d63 6266 222c 2022 6174 7422  ", "mcbf", "att"
+00000860: 2c20 2261 6362 7622 2c20 2263 6266 3122  , "acbv", "cbf1"
+00000870: 2c20 2263 6266 3222 2c20 2263 6266 3322  , "cbf2", "cbf3"
+00000880: 2c20 2263 6266 3422 2c20 2263 6266 3522  , "cbf4", "cbf5"
+00000890: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000008a0: 2020 2073 6361 6c69 6e67 5f6c 6973 7420     scaling_list 
+000008b0: 3d20 5b31 2c20 302e 312c 2030 2e30 312c  = [1, 0.1, 0.01,
+000008c0: 2030 2e30 3031 2c20 302e 312c 2030 2e31   0.001, 0.1, 0.1
+000008d0: 2c20 302e 312c 2030 2e31 2c20 302e 315d  , 0.1, 0.1, 0.1]
+000008e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000008f0: 2020 666f 7220 662c 2073 2c20 6964 7820    for f, s, idx 
+00000900: 696e 207a 6970 2866 696c 655f 6c69 7374  in zip(file_list
+00000910: 2c20 7363 616c 696e 675f 6c69 7374 2c20  , scaling_list, 
+00000920: 7261 6e67 6528 6c65 6e28 6669 6c65 5f6c  range(len(file_l
+00000930: 6973 7429 2929 3a0d 0a20 2020 2020 2020  ist))):..       
+00000940: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
+00000950: 6765 203d 206c 616d 6264 615f 6c6f 6164  ge = lambda_load
+00000960: 5f64 6963 6f6d 2866 2e75 7070 6572 2829  _dicom(f.upper()
+00000970: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00000980: 2020 2020 2020 2077 7269 7465 5f64 6963         write_dic
+00000990: 6f6d 5f73 6572 6965 7328 696d 6167 652c  om_series(image,
+000009a0: 2073 656c 662e 7261 775f 7365 7269 6573   self.raw_series
+000009b0: 2c20 6627 6173 6c2d 7b66 7d27 2c20 6375  , f'asl-{f}', cu
+000009c0: 725f 7365 7269 6573 5f6e 756d 6265 722c  r_series_number,
+000009d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009f0: 2020 2020 2020 2020 206f 732e 7061 7468           os.path
+00000a00: 2e6a 6f69 6e28 7365 6c66 2e6f 7574 7075  .join(self.outpu
+00000a10: 745f 726f 6f74 2c20 2761 736c 272c 2066  t_root, 'asl', f
+00000a20: 292c 2073 6c6f 7065 3d73 290d 0a20 2020  ), slope=s)..   
+00000a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a40: 2063 7572 5f73 6572 6965 735f 6e75 6d62   cur_series_numb
+00000a50: 6572 202b 3d20 310d 0a0d 0a20 2020 2020  er += 1....     
+00000a60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00000a70: 6620 7061 7261 6d5f 6172 7261 7920 6973  f param_array is
+00000a80: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 7061 7261 6d5f 6172 7261 7920 3d20 6e70  param_array = np
+00000ab0: 2e7a 6572 6f73 286c 6973 7428 696d 6167  .zeros(list(imag
+00000ac0: 652e 7368 6170 6529 202b 205b 395d 290d  e.shape) + [9]).
+00000ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ae0: 2020 2020 2070 6172 616d 5f61 7272 6179       param_array
+00000af0: 5b2e 2e2e 2c20 6964 785d 203d 2069 6d61  [..., idx] = ima
+00000b00: 6765 0d0a 0d0a 2020 2020 2020 2020 2020  ge....          
+00000b10: 2020 2020 2020 2320 e590 8e35 e4b8 aae6        # ...5....
+00000b20: 98af 4342 4631 2d35 efbc 8ce7 acac 33e4  ..CBF1-5......3.
+00000b30: b8aa e698 af41 5454 0d0a 2020 2020 2020  .....ATT..      
+00000b40: 2020 2020 2020 2020 2020 7375 7065 7228            super(
+00000b50: 292e 6361 6c63 5f63 6f72 7265 6374 5f43  ).calc_correct_C
+00000b60: 4246 2870 6172 616d 5f61 7272 6179 5b2e  BF(param_array[.
+00000b70: 2e2e 2c2d 353a 5d20 2a20 302e 312c 2073  ..,-5:] * 0.1, s
+00000b80: 656c 662e 7261 775f 7365 7269 6573 2c20  elf.raw_series, 
+00000b90: 6375 725f 7365 7269 6573 5f6e 756d 6265  cur_series_numbe
+00000ba0: 7229 0d0a 0d0a 2020 2020 2020 2020 2020  r)....          
+00000bb0: 2020 656c 6966 206c 656e 2873 656c 662e    elif len(self.
+00000bc0: 6465 6c61 795f 7469 6d65 2920 3d3d 2031  delay_time) == 1
+00000bd0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000be0: 2020 2069 6d61 6765 203d 206c 616d 6264     image = lambd
+00000bf0: 615f 6c6f 6164 5f64 6963 6f6d 2827 4d30  a_load_dicom('M0
+00000c00: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+00000c10: 2020 2020 7772 6974 655f 6469 636f 6d5f      write_dicom_
+00000c20: 7365 7269 6573 2869 6d61 6765 2c20 7365  series(image, se
+00000c30: 6c66 2e72 6177 5f73 6572 6965 732c 2066  lf.raw_series, f
+00000c40: 2761 736c 2d6d 3027 2c20 6375 725f 7365  'asl-m0', cur_se
+00000c50: 7269 6573 5f6e 756d 6265 722c 0d0a 2020  ries_number,..  
+00000c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c80: 206f 732e 7061 7468 2e6a 6f69 6e28 7365   os.path.join(se
+00000c90: 6c66 2e6f 7574 7075 745f 726f 6f74 2c20  lf.output_root, 
+00000ca0: 2761 736c 272c 2027 6d30 2729 2c20 736c  'asl', 'm0'), sl
+00000cb0: 6f70 653d 3129 0d0a 2020 2020 2020 2020  ope=1)..        
+00000cc0: 2020 2020 2020 2020 6375 725f 7365 7269          cur_seri
+00000cd0: 6573 5f6e 756d 6265 7220 2b3d 2031 0d0a  es_number += 1..
+00000ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000cf0: 2020 696d 6167 6520 3d20 6c61 6d62 6461    image = lambda
+00000d00: 5f6c 6f61 645f 6469 636f 6d28 2743 4246  _load_dicom('CBF
+00000d10: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+00000d20: 2020 2020 7772 6974 655f 6469 636f 6d5f      write_dicom_
+00000d30: 7365 7269 6573 2869 6d61 6765 2c20 7365  series(image, se
+00000d40: 6c66 2e72 6177 5f73 6572 6965 732c 2066  lf.raw_series, f
+00000d50: 2761 736c 2d63 6266 3127 2c20 6375 725f  'asl-cbf1', cur_
+00000d60: 7365 7269 6573 5f6e 756d 6265 722c 0d0a  series_number,..
+00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d90: 2020 206f 732e 7061 7468 2e6a 6f69 6e28     os.path.join(
+00000da0: 7365 6c66 2e6f 7574 7075 745f 726f 6f74  self.output_root
+00000db0: 2c20 2761 736c 272c 2027 6362 6631 2729  , 'asl', 'cbf1')
+00000dc0: 2c20 736c 6f70 653d 302e 3129 0d0a 0d0a  , slope=0.1)....
+00000dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000de0: 7375 7065 7228 292e 6361 6c63 5f63 6f72  super().calc_cor
+00000df0: 7265 6374 5f43 4246 2869 6d61 6765 202a  rect_CBF(image *
+00000e00: 2030 2e31 2c20 7365 6c66 2e72 6177 5f73   0.1, self.raw_s
+00000e10: 6572 6965 732c 2063 7572 5f73 6572 6965  eries, cur_serie
+00000e20: 735f 6e75 6d62 6572 202b 2031 290d 0a0d  s_number + 1)...
+00000e30: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+00000e40: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
+00000e50: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00000e60: 6765 722e 6572 726f 7228 6529 0d0a 2020  ger.error(e)..  
+00000e70: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00000e80: 650d 0a20 2020 2020 2020 2066 696e 616c  e..        final
+00000e90: 6c79 3a0d 0a20 2020 2020 2020 2020 2020  ly:..           
+00000ea0: 2070 6173 730d 0a20 2020 2020 2020 2020   pass..         
+00000eb0: 2020 2023 2073 6875 7469 6c2e 726d 7472     # shutil.rmtr
+00000ec0: 6565 286a 6176 615f 7465 6d70 290d 0a0d  ee(java_temp)...
+00000ed0: 0a20 2020 2064 6566 2067 656e 6572 6174  .    def generat
+00000ee0: 655f 6672 6f6d 5f72 6177 5f66 6f6c 6465  e_from_raw_folde
+00000ef0: 7228 7365 6c66 2c20 7465 6d70 5f64 6972  r(self, temp_dir
+00000f00: 293a 0d0a 2020 2020 2020 2020 6966 206e  ):..        if n
+00000f10: 6f74 206f 732e 7061 7468 2e65 7869 7374  ot os.path.exist
+00000f20: 7328 7465 6d70 5f64 6972 293a 0d0a 2020  s(temp_dir):..  
+00000f30: 2020 2020 2020 2020 2020 2320 7072 696e            # prin
+00000f40: 7428 22e5 b182 e695 b020 3d20 7b3a 647d  t("...... = {:d}
+00000f50: 222e 666f 726d 6174 2873 656c 662e 736c  ".format(self.sl
+00000f60: 6963 655f 6e75 6d29 290d 0a20 2020 2020  ice_num))..     
+00000f70: 2020 2020 2020 206f 732e 6d61 6b65 6469         os.makedi
+00000f80: 7273 286f 732e 7061 7468 2e6a 6f69 6e28  rs(os.path.join(
+00000f90: 7465 6d70 5f64 6972 2c20 2272 656f 7264  temp_dir, "reord
+00000fa0: 6572 6564 2229 2c20 6578 6973 745f 6f6b  ered"), exist_ok
+00000fb0: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00000fc0: 2020 2020 6f73 2e6d 616b 6564 6972 7328      os.makedirs(
+00000fd0: 6f73 2e70 6174 682e 6a6f 696e 2874 656d  os.path.join(tem
+00000fe0: 705f 6469 722c 2022 7265 636f 6e73 7472  p_dir, "reconstr
+00000ff0: 7563 7465 6422 292c 2065 7869 7374 5f6f  ucted"), exist_o
+00001000: 6b3d 5472 7565 290d 0a20 2020 2020 2020  k=True)..       
+00001010: 2020 2020 2073 656c 662e 5f6d 616b 655f       self._make_
+00001020: 6a73 6f6e 2829 0d0a 0d0a 2020 2020 2020  json()....      
+00001030: 2020 2020 2020 666f 7220 692c 2069 6e73        for i, ins
+00001040: 7461 6e63 6520 696e 2065 6e75 6d65 7261  tance in enumera
+00001050: 7465 2873 656c 662e 7261 775f 7365 7269  te(self.raw_seri
+00001060: 6573 293a 0d0a 2020 2020 2020 2020 2020  es):..          
+00001070: 2020 2020 2020 696e 7374 616e 6365 2e73        instance.s
+00001080: 6176 655f 6173 286f 732e 7061 7468 2e6a  ave_as(os.path.j
+00001090: 6f69 6e28 7465 6d70 5f64 6972 2c20 2272  oin(temp_dir, "r
+000010a0: 656f 7264 6572 6564 222c 2022 7465 6d70  eordered", "temp
+000010b0: 5f64 636d 5f7b 3a30 3464 7d2e 6463 6d22  _dcm_{:04d}.dcm"
+000010c0: 2e66 6f72 6d61 7428 6929 2929 0d0a 2020  .format(i)))..  
+000010d0: 2020 2020 2020 2020 2020 6a61 725f 666f            jar_fo
+000010e0: 6c64 6572 203d 206f 732e 7061 7468 2e6a  lder = os.path.j
+000010f0: 6f69 6e28 6f73 2e67 6574 6377 6428 292c  oin(os.getcwd(),
+00001100: 2022 5543 4c41 5f6a 6176 615f 6a61 7222   "UCLA_java_jar"
+00001110: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00001120: 2070 7269 6e74 286a 6172 5f66 6f6c 6465   print(jar_folde
+00001130: 7229 0d0a 2020 2020 2020 2020 2020 2020  r)..            
+00001140: 7265 7370 6f6e 7365 203d 2073 7562 7072  response = subpr
+00001150: 6f63 6573 732e 7275 6e28 0d0a 2020 2020  ocess.run(..    
+00001160: 2020 2020 2020 2020 2020 2020 5b0d 0a20              [.. 
+00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001180: 2020 2022 6a61 7661 222c 2022 2d6a 6172     "java", "-jar
+00001190: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000011a0: 2020 2020 2020 2020 222d 446a 6176 612e          "-Djava.
+000011b0: 6c69 6272 6172 792e 7061 7468 3d7b 7d22  library.path={}"
+000011c0: 2e66 6f72 6d61 7428 6f73 2e70 6174 682e  .format(os.path.
+000011d0: 6a6f 696e 286a 6172 5f66 6f6c 6465 722c  join(jar_folder,
+000011e0: 2022 6c69 6222 2929 2c0d 0a20 2020 2020   "lib")),..     
+000011f0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00001200: 732e 7061 7468 2e6a 6f69 6e28 6a61 725f  s.path.join(jar_
+00001210: 666f 6c64 6572 2c20 2241 534c 5f79 616f  folder, "ASL_yao
+00001220: 5f4a 4156 412d 6d61 7374 6572 2e6a 6172  _JAVA-master.jar
+00001230: 2229 2c0d 0a20 2020 2020 2020 2020 2020  "),..           
+00001240: 2020 2020 2020 2020 206f 732e 7061 7468           os.path
+00001250: 2e6a 6f69 6e28 7465 6d70 5f64 6972 2c20  .join(temp_dir, 
+00001260: 2270 6172 616d 2e6a 736f 6e22 290d 0a20  "param.json").. 
+00001270: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00001280: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001290: 2020 2073 6865 6c6c 3d54 7275 650d 0a20     shell=True.. 
+000012a0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+000012b0: 2020 2020 2020 2020 2020 6966 2072 6573            if res
+000012c0: 706f 6e73 652e 7265 7475 726e 636f 6465  ponse.returncode
+000012d0: 2021 3d20 303a 0d0a 2020 2020 2020 2020   != 0:..        
+000012e0: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
+000012f0: 6365 7074 696f 6e28 224a 6176 61e7 a88b  ception("Java...
+00001300: e5ba 8fe8 bf90 e8a1 8ce5 a4b1 e8b4 a5ef  ................
+00001310: bc8c e7bc 96e5 8fb7 3a20 7b3a 647d 222e  ........: {:d}".
+00001320: 666f 726d 6174 2872 6573 706f 6e73 652e  format(response.
+00001330: 7265 7475 726e 636f 6465 2929 0d0a 0d0a  returncode))....
+00001340: 2020 2020 2020 2020 2020 2020 6966 206f              if o
+00001350: 732e 7061 7468 2e69 7366 696c 6528 6f73  s.path.isfile(os
+00001360: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
+00001370: 6f75 7470 7574 5f72 6f6f 742c 2022 6a61  output_root, "ja
+00001380: 7661 5f74 656d 7022 2c20 2272 6563 6f6e  va_temp", "recon
+00001390: 7374 7275 6374 6564 222c 2022 6669 6e69  structed", "fini
+000013a0: 7368 6564 2e74 7874 2229 293a 0d0a 2020  shed.txt")):..  
+000013b0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+000013c0: 6767 6572 2e64 6562 7567 2822 e5ae 8ce6  gger.debug("....
+000013d0: 8890 e794 a84a 6176 61e7 9a84 e59b bee5  .....Java.......
+000013e0: 838f e987 8de5 bbba efbc 8ce5 bc80 e5a7  ................
+000013f0: 8be7 94a8 5079 7468 6f6e e69d a5e8 b083  ....Python......
+00001400: e695 b4e6 a087 e7ad be22 290d 0a20 2020  .........")..   
+00001410: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00001420: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00001430: 6562 7567 2827 e4bd bfe7 94a8 e5b7 b2e5  ebug('..........
+00001440: ad98 e59c a8e7 9a84 4a61 7661 e4b8 b4e6  ........Java....
+00001450: 97b6 e79b aee5 bd95 2729 0d0a 0d0a 2020  ........')....  
+00001460: 2020 2020 2020 7265 7475 726e 206f 732e        return os.
+00001470: 7061 7468 2e6a 6f69 6e28 7465 6d70 5f64  path.join(temp_d
+00001480: 6972 2c20 2272 6563 6f6e 7374 7275 6374  ir, "reconstruct
+00001490: 6564 2229 0d0a 0d0a 2020 2020 6465 6620  ed")....    def 
+000014a0: 5f73 6176 655f 6865 6164 5f6d 6f74 696f  _save_head_motio
+000014b0: 6e5f 6772 6170 6828 7365 6c66 293a 0d0a  n_graph(self):..
+000014c0: 2020 2020 2020 2020 6669 6c65 5f70 6174          file_pat
+000014d0: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
+000014e0: 2873 656c 662e 6f75 7470 7574 5f72 6f6f  (self.output_roo
+000014f0: 742c 2022 6a61 7661 5f74 656d 7022 2c20  t, "java_temp", 
+00001500: 2272 6563 6f6e 7374 7275 6374 6564 222c  "reconstructed",
+00001510: 2022 6865 6164 4d6f 7469 6f6e 2e6a 736f   "headMotion.jso
+00001520: 6e22 290d 0a20 2020 2020 2020 2073 6176  n")..        sav
+00001530: 655f 7061 7468 203d 206f 732e 7061 7468  e_path = os.path
+00001540: 2e6a 6f69 6e28 7365 6c66 2e6f 7574 7075  .join(self.outpu
+00001550: 745f 726f 6f74 2c20 2268 6561 644d 6f74  t_root, "headMot
+00001560: 696f 6e2e 706e 6722 290d 0a20 2020 2020  ion.png")..     
+00001570: 2020 2077 6974 6820 6f70 656e 2866 696c     with open(fil
+00001580: 655f 7061 7468 2c20 2772 2729 2061 7320  e_path, 'r') as 
+00001590: 663a 0d0a 2020 2020 2020 2020 2020 2020  f:..            
+000015a0: 6461 7461 203d 206a 736f 6e2e 6c6f 6164  data = json.load
+000015b0: 2866 290d 0a20 2020 2020 2020 2023 2070  (f)..        # p
+000015c0: 7269 6e74 2864 6174 6129 0d0a 2020 2020  rint(data)..    
+000015d0: 2020 2020 6669 6720 3d20 706c 742e 6669      fig = plt.fi
+000015e0: 6775 7265 2829 0d0a 2020 2020 2020 2020  gure()..        
+000015f0: 6d61 7470 6c6f 746c 6962 2e72 6350 6172  matplotlib.rcPar
+00001600: 616d 735b 2766 6f6e 742e 6661 6d69 6c79  ams['font.family
+00001610: 275d 203d 2022 7369 6d73 756e 220d 0a20  '] = "simsun".. 
+00001620: 2020 2020 2020 2066 6967 2e73 6574 5f73         fig.set_s
+00001630: 697a 655f 696e 6368 6573 2836 2c20 3229  ize_inches(6, 2)
+00001640: 0d0a 2020 2020 2020 2020 7864 6174 6120  ..        xdata 
+00001650: 3d20 6e70 2e6c 696e 7370 6163 6528 312c  = np.linspace(1,
+00001660: 206c 656e 2864 6174 615b 2263 6f6e 7472   len(data["contr
+00001670: 6f6c 4644 225d 292c 206c 656e 2864 6174  olFD"]), len(dat
+00001680: 615b 2263 6f6e 7472 6f6c 4644 225d 2929  a["controlFD"]))
+00001690: 0d0a 2020 2020 2020 2020 706c 742e 706c  ..        plt.pl
+000016a0: 6f74 2878 6461 7461 2c20 6461 7461 5b22  ot(xdata, data["
+000016b0: 636f 6e74 726f 6c46 4422 5d2c 2027 626f  controlFD"], 'bo
+000016c0: 2d27 2c20 6c61 6265 6c3d 27e6 97a0 e6a0  -', label='.....
+000016d0: 87e8 aeb0 e583 8f27 290d 0a20 2020 2020  .......')..     
+000016e0: 2020 2070 6c74 2e70 6c6f 7428 7864 6174     plt.plot(xdat
+000016f0: 612c 2064 6174 615b 226c 6162 656c 4644  a, data["labelFD
+00001700: 225d 2c20 2772 6f2d 272c 206c 6162 656c  "], 'ro-', label
+00001710: 3d27 e6a0 87e8 aeb0 e583 8f27 290d 0a20  ='.........').. 
+00001720: 2020 2020 2020 2070 6c74 2e78 7469 636b         plt.xtick
+00001730: 7328 7864 6174 6129 0d0a 2020 2020 2020  s(xdata)..      
+00001740: 2020 706c 742e 786c 6162 656c 2822 e59b    plt.xlabel("..
+00001750: bee7 8987 e5ba 8fe5 8fb7 2229 0d0a 2020  ..........")..  
+00001760: 2020 2020 2020 706c 742e 796c 6162 656c        plt.ylabel
+00001770: 2822 e5a4 b4e5 8aa8 286d 6d29 2229 0d0a  ("......(mm)")..
+00001780: 2020 2020 2020 2020 706c 742e 6c65 6765          plt.lege
+00001790: 6e64 2829 0d0a 2020 2020 2020 2020 706c  nd()..        pl
+000017a0: 742e 7469 6768 745f 6c61 796f 7574 2829  t.tight_layout()
+000017b0: 0d0a 2020 2020 2020 2020 706c 742e 7361  ..        plt.sa
+000017c0: 7665 6669 6728 7361 7665 5f70 6174 682c  vefig(save_path,
+000017d0: 2064 7069 3d32 3030 290d 0a20 2020 2020   dpi=200)..     
+000017e0: 2020 2070 6c74 2e66 6967 7572 6528 292e     plt.figure().
+000017f0: 636c 6561 7228 290d 0a20 2020 2020 2020  clear()..       
+00001800: 2070 6c74 2e63 6c6f 7365 2829 0d0a 2020   plt.close()..  
+00001810: 2020 2020 2020 706c 742e 636c 6128 290d        plt.cla().
+00001820: 0a20 2020 2020 2020 2070 6c74 2e63 6c66  .        plt.clf
+00001830: 2829 0d0a 0d0a 2020 2020 6465 6620 5f6d  ()....    def _m
+00001840: 616b 655f 6a73 6f6e 2873 656c 6629 3a0d  ake_json(self):.
+00001850: 0a20 2020 2020 2020 2073 656c 662e 7261  .        self.ra
+00001860: 775f 7365 7269 6573 3a20 5365 7269 6573  w_series: Series
+00001870: 4d6f 6465 6c0d 0a20 2020 2020 2020 2064  Model..        d
+00001880: 656c 6179 5f6e 756d 203d 206c 656e 2873  elay_num = len(s
+00001890: 656c 662e 6465 6c61 795f 7469 6d65 290d  elf.delay_time).
+000018a0: 0a20 2020 2020 2020 2069 6620 6465 6c61  .        if dela
+000018b0: 795f 6e75 6d20 3d3d 2030 3a0d 0a20 2020  y_num == 0:..   
+000018c0: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+000018d0: 7863 6570 7469 6f6e 2827 6465 6c61 795f  xception('delay_
+000018e0: 7469 6d65 2069 7320 6e75 6c6c 2729 0d0a  time is null')..
+000018f0: 2020 2020 2020 2020 6966 2064 656c 6179          if delay
+00001900: 5f6e 756d 2021 3d20 6c65 6e28 7365 6c66  _num != len(self
+00001910: 2e64 656c 6179 5f72 6570 293a 0d0a 2020  .delay_rep):..  
+00001920: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00001930: 4465 6c61 794e 6f74 4571 7561 6c52 6570  DelayNotEqualRep
+00001940: 6574 6974 696f 6e45 7272 6f72 2864 656c  etitionError(del
+00001950: 6179 5f6e 756d 2c20 6c65 6e28 7365 6c66  ay_num, len(self
+00001960: 2e64 656c 6179 5f72 6570 2929 0d0a 0d0a  .delay_rep))....
+00001970: 2020 2020 2020 2020 7061 7261 6d5f 6a73          param_js
+00001980: 6f6e 5f64 6963 7420 3d20 7b0d 0a20 2020  on_dict = {..   
+00001990: 2020 2020 2020 2020 2022 6461 7461 5f74           "data_t
+000019a0: 7970 6522 3a20 2735 6465 6c61 795f 6d6f  ype": '5delay_mo
+000019b0: 7361 6963 2720 6966 2073 656c 662e 6461  saic' if self.da
+000019c0: 7461 5f74 7970 6520 696e 205b 4d52 495f  ta_type in [MRI_
+000019d0: 5479 7065 2e4d 5249 5f54 5950 455f 3544  Type.MRI_TYPE_5D
+000019e0: 656c 6179 5f33 445f 5043 4153 4c5f 5349  elay_3D_PCASL_SI
+000019f0: 454d 454e 532c 0d0a 2020 2020 2020 2020  EMENS,..        
+00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a30: 2020 2020 2020 204d 5249 5f54 7970 652e         MRI_Type.
+00001a40: 4d52 495f 5459 5045 5f31 4465 6c61 795f  MRI_TYPE_1Delay_
+00001a50: 3344 5f50 4341 534c 5f53 4945 4d45 4e53  3D_PCASL_SIEMENS
+00001a60: 5d20 656c 7365 2027 3464 656c 6179 5f33  ] else '4delay_3
+00001a70: 6427 2c0d 0a20 2020 2020 2020 2020 2020  d',..           
+00001a80: 2022 736c 6963 655f 6f72 6465 7222 3a20   "slice_order": 
+00001a90: 2761 7363 656e 6469 6e67 272c 2023 20e6  'ascending', # .
+00001aa0: ada4 e58f 82e6 95b0 e5b7 b2e4 b88d e987  ................
+00001ab0: 8de8 a681 0d0a 2020 2020 2020 2020 2020  ......          
+00001ac0: 2020 2273 6c69 6365 5f6e 756d 223a 2073    "slice_num": s
+00001ad0: 656c 662e 7261 775f 7365 7269 6573 2e53  elf.raw_series.S
+00001ae0: 6c69 6365 4e75 6d62 6572 2c0d 0a20 2020  liceNumber,..   
+00001af0: 2020 2020 2020 2020 2022 696e 6974 5f64           "init_d
+00001b00: 656c 6179 223a 2073 656c 662e 6465 6c61  elay": self.dela
+00001b10: 795f 7469 6d65 5b30 5d2c 0d0a 2020 2020  y_time[0],..    
+00001b20: 2020 2020 2020 2020 2264 656c 6179 5f6e          "delay_n
+00001b30: 756d 223a 2064 656c 6179 5f6e 756d 2c0d  um": delay_num,.
+00001b40: 0a20 2020 2020 2020 2020 2020 2022 696e  .            "in
+00001b50: 7465 7276 616c 223a 2073 656c 662e 6465  terval": self.de
+00001b60: 6c61 795f 7469 6d65 5b31 5d20 2d20 7365  lay_time[1] - se
+00001b70: 6c66 2e64 656c 6179 5f74 696d 655b 305d  lf.delay_time[0]
+00001b80: 2069 6620 6465 6c61 795f 6e75 6d20 3e3d   if delay_num >=
+00001b90: 2032 2065 6c73 6520 302e 302c 0d0a 2020   2 else 0.0,..  
+00001ba0: 2020 2020 2020 2020 2020 2264 656c 6179            "delay
+00001bb0: 5f72 6570 223a 2073 656c 662e 6465 6c61  _rep": self.dela
+00001bc0: 795f 7265 702c 0d0a 2020 2020 2020 2020  y_rep,..        
+00001bd0: 2020 2020 226c 6f61 645f 7061 7468 223a      "load_path":
+00001be0: 206f 732e 7061 7468 2e6a 6f69 6e28 7365   os.path.join(se
+00001bf0: 6c66 2e6f 7574 7075 745f 726f 6f74 2c20  lf.output_root, 
+00001c00: 226a 6176 615f 7465 6d70 222c 2022 7265  "java_temp", "re
+00001c10: 6f72 6465 7265 6422 292c 0d0a 2020 2020  ordered"),..    
+00001c20: 2020 2020 2020 2020 2273 6176 655f 7061          "save_pa
+00001c30: 7468 223a 206f 732e 7061 7468 2e6a 6f69  th": os.path.joi
+00001c40: 6e28 7365 6c66 2e6f 7574 7075 745f 726f  n(self.output_ro
+00001c50: 6f74 2c20 226a 6176 615f 7465 6d70 222c  ot, "java_temp",
+00001c60: 2022 7265 636f 6e73 7472 7563 7465 6422   "reconstructed"
+00001c70: 297d 0d0a 0d0a 2020 2020 2020 2020 7769  )}....        wi
+00001c80: 7468 206f 7065 6e28 6f73 2e70 6174 682e  th open(os.path.
+00001c90: 6a6f 696e 2873 656c 662e 6f75 7470 7574  join(self.output
+00001ca0: 5f72 6f6f 742c 2022 6a61 7661 5f74 656d  _root, "java_tem
+00001cb0: 7022 2c20 2270 6172 616d 2e6a 736f 6e22  p", "param.json"
+00001cc0: 292c 2022 7722 2920 6173 2066 703a 0d0a  ), "w") as fp:..
+00001cd0: 2020 2020 2020 2020 2020 2020 6a73 6f6e              json
+00001ce0: 2e64 756d 7028 7061 7261 6d5f 6a73 6f6e  .dump(param_json
+00001cf0: 5f64 6963 742c 2066 702c 2069 6e64 656e  _dict, fp, inden
+00001d00: 743d 3429 0d0a 2020 2020 2020 2020 7072  t=4)..        pr
+00001d10: 696e 7428 226a 736f 6ee6 9687 e4bb b6e4  int("json.......
+00001d20: bf9d e5ad 9822 290d 0a0d 0a20 2020 2040  .....")....    @
+00001d30: 7374 6174 6963 6d65 7468 6f64 0d0a 2020  staticmethod..  
+00001d40: 2020 6465 6620 5f33 445f 746f 5f6d 6f73    def _3D_to_mos
+00001d50: 6169 6328 6172 7261 793a 206e 702e 6e64  aic(array: np.nd
+00001d60: 6172 7261 7929 3a0d 0a20 2020 2020 2020  array):..       
+00001d70: 2077 6964 7468 203d 2068 6569 6768 7420   width = height 
+00001d80: 3d20 696e 7428 6e70 2e63 6569 6c28 6172  = int(np.ceil(ar
+00001d90: 7261 792e 7368 6170 655b 325d 2929 0d0a  ray.shape[2]))..
+00001da0: 2020 2020 2020 2020 6465 6620 6765 745f          def get_
+00001db0: 736c 6963 6528 6172 7261 793a 206e 702e  slice(array: np.
+00001dc0: 6e64 6172 7261 792c 2073 6c69 6365 3a20  ndarray, slice: 
+00001dd0: 696e 7429 3a0d 0a20 2020 2020 2020 2020  int):..         
+00001de0: 2020 2023 20e8 b685 e587 bae8 8c83 e59b     # ...........
+00001df0: b4e7 94a8 2030 e580 bce5 a1ab e585 850d  .... 0..........
+00001e00: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00001e10: 6172 7261 792e 7368 6170 655b 325d 203e  array.shape[2] >
+00001e20: 2073 6c69 6365 3a0d 0a20 2020 2020 2020   slice:..       
+00001e30: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001e40: 6172 7261 795b 3a2c 203a 2c20 736c 6963  array[:, :, slic
+00001e50: 655d 0d0a 2020 2020 2020 2020 2020 2020  e]..            
+00001e60: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00001e70: 2020 2020 2020 2072 6574 7572 6e20 6e70         return np
+00001e80: 2e7a 6572 6f73 2861 7272 6179 5b3a 2c20  .zeros(array[:, 
+00001e90: 3a2c 2030 5d2e 7368 6170 652c 2064 7479  :, 0].shape, dty
+00001ea0: 7065 3d61 7272 6179 2e64 7479 7065 290d  pe=array.dtype).
+00001eb0: 0a0d 0a20 2020 2020 2020 2072 6f77 5f69  ...        row_i
+00001ec0: 6d67 5f76 6563 746f 7220 3d20 5b5d 0d0a  mg_vector = []..
+00001ed0: 2020 2020 2020 2020 666f 7220 6f66 6673          for offs
+00001ee0: 6574 2069 6e20 7261 6e67 6528 7769 6474  et in range(widt
+00001ef0: 6829 3a0d 0a20 2020 2020 2020 2020 2020  h):..           
+00001f00: 2063 6f6c 5f69 6e64 6578 203d 2074 7570   col_index = tup
+00001f10: 6c65 285b 6920 2a20 7769 6474 6820 2b20  le([i * width + 
+00001f20: 6f66 6673 6574 2066 6f72 2069 2069 6e20  offset for i in 
+00001f30: 7261 6e67 6528 6865 6967 6874 295d 290d  range(height)]).
+00001f40: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
+00001f50: 5f69 6d67 203d 206e 702e 7673 7461 636b  _img = np.vstack
+00001f60: 285b 6765 745f 736c 6963 6528 6172 7261  ([get_slice(arra
+00001f70: 792c 2063 2920 666f 7220 6320 696e 2063  y, c) for c in c
+00001f80: 6f6c 5f69 6e64 6578 5d29 0d0a 2020 2020  ol_index])..    
+00001f90: 2020 2020 2020 2020 726f 775f 696d 675f          row_img_
+00001fa0: 7665 6374 6f72 2e61 7070 656e 6428 636f  vector.append(co
+00001fb0: 6c5f 696d 6729 0d0a 0d0a 2020 2020 2020  l_img)....      
+00001fc0: 2020 7265 7475 726e 206e 702e 6873 7461    return np.hsta
+00001fd0: 636b 2872 6f77 5f69 6d67 5f76 6563 746f  ck(row_img_vecto
+00001fe0: 7229 0d0a 0d0a                           r)....
```

### Comparing `animage-data_sorter-1.1.4/data_sorter/restructure/siemens_3d_pcasl_old.py` & `animage-data_sorter-1.1.5/data_sorter/restructure/siemens_3d_pcasl_old.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.4/data_sorter/restructure/uih_3d_pasl.py` & `animage-data_sorter-1.1.5/data_sorter/restructure/uih_3d_pasl.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,38 +70,47 @@
         # 多张M0只有第一张有效
         m0_image = m0_image[..., 0]
         write_dicom_series(m0_image, self.M0, 'asl-m0', 1001, os.path.join(self.output_root, 'asl', 'm0'))
 
         cbf_image = self.CBF[0].load()[..., 0]
         write_dicom_series(cbf_image * 10, self.M0, 'asl-cbf', 1002, os.path.join(self.output_root, 'asl', 'cbf'), slope=0.1)
 
+        # UIH的ATT 单位为ms，不再乘以1000
         att_image = self.ATT.load()[..., 0]
-        write_dicom_series(att_image * 1000, self.M0, 'asl-att', 1003, os.path.join(self.output_root, 'asl', 'att'), slope=0.001)
+        write_dicom_series(att_image, self.M0, 'asl-att', 1003, os.path.join(self.output_root, 'asl', 'att'), slope=0.001)
 
         acbv_image = self.ACBV.load()[..., 0]
         write_dicom_series(acbv_image * 1000, self.M0, 'asl-acbv', 1004, os.path.join(self.output_root, 'asl', 'acbv'), slope=0.001)
 
     def generate_cbf_3d_pasl(self):
         self.M0: SeriesModel = self.M0[0]
         m0_image = self.M0.load()
         # 多张M0只有第一张有效
         m0_image = m0_image[...,0]
         m0_nii = write_dicom_series(m0_image, self.M0, 'asl-m0', 1001, os.path.join(self.output_root, 'asl', 'm0'))
 
-        for i, cbf in enumerate(self.CBF):
-            cbf_image = cbf.load()[...,0]
-            cbf_nii = write_dicom_series(cbf_image * 10, cbf, f'asl-cbf{i+1}', 1002 + i,
+        # 加载全部的CBF，空间如不一致抛异常
+        cbf_mat_list = []
+        space_resolution = None
+        for i in self.CBF:
+            mat = i.load()[..., 0]
+            if space_resolution is None:
+                space_resolution = mat.shape
+            elif space_resolution != mat.shape:
+                raise Exception(f'多个PLD图像分辨率不一致{mat.shape} 与 {space_resolution}')
+            cbf_mat_list.append(mat)
+
+        for i, (cbf_mat, cbf_series) in enumerate(zip(cbf_mat_list, self.CBF)):
+            cbf_nii = write_dicom_series(cbf_mat * 10, cbf_series, f'asl-cbf{i+1}', 1002 + i,
                                os.path.join(self.output_root, 'asl', f'cbf{i+1}'), slope=0.1)
 
-            convert(cbf_nii, cbf_nii, m0_nii)
+            # convert(cbf_nii, cbf_nii, m0_nii)
 
         super().calc_correct_CBF(np.concatenate([i.load() for i in self.CBF], axis=3), self.CBF[0], 1002+len(self.CBF))
 
-
-
     def generate_calc_cbf_3d_pasl(self):
         self.M0: SeriesModel
         m0_image = self.M0.load()
         # 多张M0只有第一张有效
         m0_image = m0_image[:,:,:,0]
         write_dicom_series(m0_image, self.M0, 'asl-m0', 1001, os.path.join(self.output_root, 'asl', 'm0'))
```

### Comparing `animage-data_sorter-1.1.4/setup.py` & `animage-data_sorter-1.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="animage-data_sorter",
-  version="1.1.4",
+  version="1.1.5",
   author="zhaomy",
   author_email="zhaomy@an-image.cn",
   description="dicom sort",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://gitee.com/AnImage-Beijing/data_sorter",
   packages=setuptools.find_packages(),
```

