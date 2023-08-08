# Comparing `tmp/cntracer-0.4.0-cp39-cp39-win_amd64.whl.zip` & `tmp/cntracer-0.6.1-cp39-cp39-musllinux_1_1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,12 @@
-Zip file size: 79266 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   175616 b- defN 23-Aug-03 09:00 cntracer.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2182 b- defN 23-Aug-03 09:00 cntracer-0.4.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      233 b- defN 23-Aug-03 09:00 cntracer-0.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-03 09:00 cntracer-0.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Aug-03 09:00 cntracer-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      476 b- defN 23-Aug-03 09:00 cntracer-0.4.0.dist-info/RECORD
-6 files, 178616 bytes uncompressed, 78406 bytes compressed:  56.1%
+Zip file size: 639139 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 02:06 cntracer-0.6.1.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 02:06 cntracer.libs/
+-rwxr-xr-x  2.0 unx   283785 b- defN 23-Aug-08 02:06 cntracer.cpython-39-x86_64-linux-gnu.so
+-rw-rw-r--  2.0 unx      692 b- defN 23-Aug-08 02:06 cntracer-0.6.1.dist-info/RECORD
+-rw-r--r--  2.0 unx     2182 b- defN 23-Aug-08 02:06 cntracer-0.6.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      111 b- defN 23-Aug-08 02:06 cntracer-0.6.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      222 b- defN 23-Aug-08 02:06 cntracer-0.6.1.dist-info/METADATA
+-rw-r--r--  2.0 unx        9 b- defN 23-Aug-08 02:06 cntracer-0.6.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx    81257 b- defN 23-Aug-08 02:06 cntracer.libs/libgcc_s-a04fdf82.so.1
+-rwxr-xr-x  2.0 unx  2447393 b- defN 23-Aug-08 02:06 cntracer.libs/libstdc++-a9383cce.so.6.0.28
+10 files, 2815651 bytes uncompressed, 637717 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -1,19 +1,31 @@
-Filename: cntracer.cp39-win_amd64.pyd
+Filename: cntracer-0.6.1.dist-info/
 Comment: 
 
-Filename: cntracer-0.4.0.dist-info/LICENSE
+Filename: cntracer.libs/
 Comment: 
 
-Filename: cntracer-0.4.0.dist-info/METADATA
+Filename: cntracer.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: cntracer-0.4.0.dist-info/WHEEL
+Filename: cntracer-0.6.1.dist-info/RECORD
 Comment: 
 
-Filename: cntracer-0.4.0.dist-info/top_level.txt
+Filename: cntracer-0.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: cntracer-0.4.0.dist-info/RECORD
+Filename: cntracer-0.6.1.dist-info/WHEEL
+Comment: 
+
+Filename: cntracer-0.6.1.dist-info/METADATA
+Comment: 
+
+Filename: cntracer-0.6.1.dist-info/top_level.txt
+Comment: 
+
+Filename: cntracer.libs/libgcc_s-a04fdf82.so.1
+Comment: 
+
+Filename: cntracer.libs/libstdc++-a9383cce.so.6.0.28
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `cntracer-0.4.0.dist-info/LICENSE` & `cntracer-0.6.1.dist-info/LICENSE`

 * *Files identical despite different names*

