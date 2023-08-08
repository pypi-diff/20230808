# Comparing `tmp/tflite_runtime_nightly-2.15.0.dev20230805-cp39-cp39-manylinux_2_34_armv7l.whl.zip` & `tmp/tflite_runtime_nightly-2.15.0.dev20230806-cp39-cp39-manylinux_2_34_armv7l.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 1820880 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       80 b- defN 23-Aug-06 05:05 tflite_runtime/__init__.py
--rwxrwxr-x  2.0 unx  4918140 b- defN 23-Aug-06 05:08 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
--rw-rw-r--  2.0 unx    38775 b- defN 23-Aug-06 05:05 tflite_runtime/interpreter.py
--rw-rw-r--  2.0 unx     1542 b- defN 23-Aug-06 05:05 tflite_runtime/metrics_interface.py
--rw-rw-r--  2.0 unx     2048 b- defN 23-Aug-06 05:05 tflite_runtime/metrics_portable.py
--rw-rw-r--  2.0 unx     1439 b- defN 23-Aug-06 05:08 tflite_runtime_nightly-2.15.0.dev20230805.dist-info/METADATA
--rw-rw-r--  2.0 unx      112 b- defN 23-Aug-06 05:08 tflite_runtime_nightly-2.15.0.dev20230805.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Aug-06 05:08 tflite_runtime_nightly-2.15.0.dev20230805.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 23-Aug-06 05:08 tflite_runtime_nightly-2.15.0.dev20230805.dist-info/RECORD
-9 files, 4963029 bytes uncompressed, 1819334 bytes compressed:  63.3%
+Zip file size: 1820879 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       80 b- defN 23-Aug-07 04:57 tflite_runtime/__init__.py
+-rwxrwxr-x  2.0 unx  4918140 b- defN 23-Aug-07 04:59 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
+-rw-rw-r--  2.0 unx    38775 b- defN 23-Aug-07 04:57 tflite_runtime/interpreter.py
+-rw-rw-r--  2.0 unx     1542 b- defN 23-Aug-07 04:57 tflite_runtime/metrics_interface.py
+-rw-rw-r--  2.0 unx     2048 b- defN 23-Aug-07 04:57 tflite_runtime/metrics_portable.py
+-rw-rw-r--  2.0 unx     1439 b- defN 23-Aug-07 04:59 tflite_runtime_nightly-2.15.0.dev20230806.dist-info/METADATA
+-rw-rw-r--  2.0 unx      112 b- defN 23-Aug-07 04:59 tflite_runtime_nightly-2.15.0.dev20230806.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Aug-07 04:59 tflite_runtime_nightly-2.15.0.dev20230806.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-Aug-07 04:59 tflite_runtime_nightly-2.15.0.dev20230806.dist-info/RECORD
+9 files, 4963029 bytes uncompressed, 1819333 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tflite_runtime/metrics_interface.py
 Comment: 
 
 Filename: tflite_runtime/metrics_portable.py
 Comment: 
 
-Filename: tflite_runtime_nightly-2.15.0.dev20230805.dist-info/METADATA
+Filename: tflite_runtime_nightly-2.15.0.dev20230806.dist-info/METADATA
 Comment: 
 
-Filename: tflite_runtime_nightly-2.15.0.dev20230805.dist-info/WHEEL
+Filename: tflite_runtime_nightly-2.15.0.dev20230806.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_runtime_nightly-2.15.0.dev20230805.dist-info/top_level.txt
+Filename: tflite_runtime_nightly-2.15.0.dev20230806.dist-info/top_level.txt
 Comment: 
 
-Filename: tflite_runtime_nightly-2.15.0.dev20230805.dist-info/RECORD
+Filename: tflite_runtime_nightly-2.15.0.dev20230806.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_runtime/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.15.0dev20230805'
-__git_version__ = '0.6.0-151813-g1710ba1f679'
+__version__ = '2.15.0dev20230806'
+__git_version__ = '0.6.0-151827-g65fbcb0bbe9'
```

## Comparing `tflite_runtime_nightly-2.15.0.dev20230805.dist-info/METADATA` & `tflite_runtime_nightly-2.15.0.dev20230806.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflite-runtime-nightly
-Version: 2.15.0.dev20230805
+Version: 2.15.0.dev20230806
 Summary: TensorFlow Lite is for mobile and embedded devices.
 Home-page: https://www.tensorflow.org/lite/
 Author: Google, LLC
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Keywords: tflite tensorflow tensor machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `tflite_runtime_nightly-2.15.0.dev20230805.dist-info/RECORD` & `tflite_runtime_nightly-2.15.0.dev20230806.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tflite_runtime/__init__.py,sha256=jYrCbMw8uHBKg96-7Hcyr-PWZ01wEmM08j1aBHKBZbQ,80
+tflite_runtime/__init__.py,sha256=dVOWIgm94iK-EHQqVLeojsBFojVKYbwLglf-MnB5z1s,80
 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so,sha256=pVRLZ61Uc0MtXrPsf6NDxPLr0W05E0bXPMuBvyOv3z0,4918140
 tflite_runtime/interpreter.py,sha256=WdMKqxuFdoGPyOKoCsZsHbvsVQXs_81OrG7VUE8p5JU,38775
 tflite_runtime/metrics_interface.py,sha256=dVu6SmbnQUntPgE5o6BxHVMyemwli-7F6tDfVMGrlYI,1542
 tflite_runtime/metrics_portable.py,sha256=YBiMNokP9JtoQaUcCRRY1T_iFSZGeWCjr6L0iUR6eY8,2048
-tflite_runtime_nightly-2.15.0.dev20230805.dist-info/METADATA,sha256=5vPX4vOjSFKpWHsqC_ejDZwoIaVb-Xc1UepvUHo5d-U,1439
-tflite_runtime_nightly-2.15.0.dev20230805.dist-info/WHEEL,sha256=FeylT_K2MLt_X9AUdg-S9Vhuht7KzySHYkJD5kaOSvc,112
-tflite_runtime_nightly-2.15.0.dev20230805.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
-tflite_runtime_nightly-2.15.0.dev20230805.dist-info/RECORD,,
+tflite_runtime_nightly-2.15.0.dev20230806.dist-info/METADATA,sha256=L9dyrHcSgg1qFoG1l-D7uB6fSoUynxEcQssYVVZtDLs,1439
+tflite_runtime_nightly-2.15.0.dev20230806.dist-info/WHEEL,sha256=FeylT_K2MLt_X9AUdg-S9Vhuht7KzySHYkJD5kaOSvc,112
+tflite_runtime_nightly-2.15.0.dev20230806.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
+tflite_runtime_nightly-2.15.0.dev20230806.dist-info/RECORD,,
```

