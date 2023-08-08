# Comparing `tmp/cirq-1.3.0.dev20230807212704-py3-none-any.whl.zip` & `tmp/cirq-1.3.0.dev20230807214542-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 8394 bytes, number of entries: 6
--rw-r--r--  2.0 unx      292 b- defN 23-Aug-07 21:27 cirq-1.3.0.dev20230807212704.dist-info/AUTHORS
--rw-r--r--  2.0 unx    11357 b- defN 23-Aug-07 21:27 cirq-1.3.0.dev20230807212704.dist-info/LICENSE
--rw-r--r--  2.0 unx     7874 b- defN 23-Aug-07 21:27 cirq-1.3.0.dev20230807212704.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 21:27 cirq-1.3.0.dev20230807212704.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Aug-07 21:27 cirq-1.3.0.dev20230807212704.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      563 b- defN 23-Aug-07 21:27 cirq-1.3.0.dev20230807212704.dist-info/RECORD
-6 files, 20179 bytes uncompressed, 7356 bytes compressed:  63.5%
+Zip file size: 8395 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      292 b- defN 23-Aug-07 21:45 cirq-1.3.0.dev20230807214542.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    11357 b- defN 23-Aug-07 21:45 cirq-1.3.0.dev20230807214542.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7874 b- defN 23-Aug-07 21:45 cirq-1.3.0.dev20230807214542.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 21:45 cirq-1.3.0.dev20230807214542.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-07 21:45 cirq-1.3.0.dev20230807214542.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      563 b- defN 23-Aug-07 21:45 cirq-1.3.0.dev20230807214542.dist-info/RECORD
+6 files, 20179 bytes uncompressed, 7357 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: cirq-1.3.0.dev20230807212704.dist-info/AUTHORS
+Filename: cirq-1.3.0.dev20230807214542.dist-info/AUTHORS
 Comment: 
 
-Filename: cirq-1.3.0.dev20230807212704.dist-info/LICENSE
+Filename: cirq-1.3.0.dev20230807214542.dist-info/LICENSE
 Comment: 
 
-Filename: cirq-1.3.0.dev20230807212704.dist-info/METADATA
+Filename: cirq-1.3.0.dev20230807214542.dist-info/METADATA
 Comment: 
 
-Filename: cirq-1.3.0.dev20230807212704.dist-info/WHEEL
+Filename: cirq-1.3.0.dev20230807214542.dist-info/WHEEL
 Comment: 
 
-Filename: cirq-1.3.0.dev20230807212704.dist-info/top_level.txt
+Filename: cirq-1.3.0.dev20230807214542.dist-info/top_level.txt
 Comment: 
 
-Filename: cirq-1.3.0.dev20230807212704.dist-info/RECORD
+Filename: cirq-1.3.0.dev20230807214542.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cirq-1.3.0.dev20230807212704.dist-info/LICENSE` & `cirq-1.3.0.dev20230807214542.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cirq-1.3.0.dev20230807212704.dist-info/METADATA` & `cirq-1.3.0.dev20230807214542.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: cirq
-Version: 1.3.0.dev20230807212704
+Version: 1.3.0.dev20230807214542
 Summary: A framework for creating, editing, and invoking Noisy Intermediate Scale Quantum (NISQ) circuits.
 Home-page: http://github.com/quantumlib/cirq
 Author: The Cirq Developers
 Author-email: cirq-dev@googlegroups.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.9.0
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: cirq-aqt ==1.3.0.dev20230807212704
-Requires-Dist: cirq-core ==1.3.0.dev20230807212704
-Requires-Dist: cirq-ft ==1.3.0.dev20230807212704
-Requires-Dist: cirq-google ==1.3.0.dev20230807212704
-Requires-Dist: cirq-ionq ==1.3.0.dev20230807212704
-Requires-Dist: cirq-pasqal ==1.3.0.dev20230807212704
-Requires-Dist: cirq-rigetti ==1.3.0.dev20230807212704
-Requires-Dist: cirq-web ==1.3.0.dev20230807212704
+Requires-Dist: cirq-aqt ==1.3.0.dev20230807214542
+Requires-Dist: cirq-core ==1.3.0.dev20230807214542
+Requires-Dist: cirq-ft ==1.3.0.dev20230807214542
+Requires-Dist: cirq-google ==1.3.0.dev20230807214542
+Requires-Dist: cirq-ionq ==1.3.0.dev20230807214542
+Requires-Dist: cirq-pasqal ==1.3.0.dev20230807214542
+Requires-Dist: cirq-rigetti ==1.3.0.dev20230807214542
+Requires-Dist: cirq-web ==1.3.0.dev20230807214542
 Provides-Extra: dev_env
 Requires-Dist: mypy ==1.2.0 ; extra == 'dev_env'
 Requires-Dist: types-backports ==0.1.3 ; extra == 'dev_env'
 Requires-Dist: types-cachetools ; extra == 'dev_env'
 Requires-Dist: types-protobuf ~=3.20 ; extra == 'dev_env'
 Requires-Dist: types-requests ==2.28.1 ; extra == 'dev_env'
 Requires-Dist: types-setuptools ==62.6.1 ; extra == 'dev_env'
```

