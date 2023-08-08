# Comparing `tmp/xw_cbase-1.0.3-cp39-cp39-win_amd64.whl.zip` & `tmp/xw_cbase-16.0.1-cp39-cp39-musllinux_1_1_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,12 @@
-Zip file size: 77956 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   171008 b- defN 23-Aug-02 08:04 xw_cbase.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2182 b- defN 23-Aug-02 08:04 xw_cbase-1.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      233 b- defN 23-Aug-02 08:04 xw_cbase-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-02 08:04 xw_cbase-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Aug-02 08:04 xw_cbase-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      476 b- defN 23-Aug-02 08:04 xw_cbase-1.0.3.dist-info/RECORD
-6 files, 174008 bytes uncompressed, 77096 bytes compressed:  55.7%
+Zip file size: 783743 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 17:20 xw_cbase.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 17:20 xw_cbase-16.0.1.dist-info/
+-rwxr-xr-x  2.0 unx  1189065 b- defN 23-Aug-08 17:20 xw_cbase.cpython-39-aarch64-linux-gnu.so
+-rwxr-xr-x  2.0 unx  2599041 b- defN 23-Aug-08 17:20 xw_cbase.libs/libstdc++-fd9f4683.so.6.0.28
+-rw-r--r--  2.0 unx   134393 b- defN 23-Aug-08 17:20 xw_cbase.libs/libgcc_s-4e37474d.so.1
+-rw-r--r--  2.0 unx      217 b- defN 23-Aug-08 17:20 xw_cbase-16.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      112 b- defN 23-Aug-08 17:20 xw_cbase-16.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx     2182 b- defN 23-Aug-08 17:20 xw_cbase-16.0.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      700 b- defN 23-Aug-08 17:20 xw_cbase-16.0.1.dist-info/RECORD
+-rw-r--r--  2.0 unx        9 b- defN 23-Aug-08 17:20 xw_cbase-16.0.1.dist-info/top_level.txt
+10 files, 3925719 bytes uncompressed, 782307 bytes compressed:  80.1%
```

## zipnote {}

```diff
@@ -1,19 +1,31 @@
-Filename: xw_cbase.cp39-win_amd64.pyd
+Filename: xw_cbase.libs/
 Comment: 
 
-Filename: xw_cbase-1.0.3.dist-info/LICENSE
+Filename: xw_cbase-16.0.1.dist-info/
 Comment: 
 
-Filename: xw_cbase-1.0.3.dist-info/METADATA
+Filename: xw_cbase.cpython-39-aarch64-linux-gnu.so
 Comment: 
 
-Filename: xw_cbase-1.0.3.dist-info/WHEEL
+Filename: xw_cbase.libs/libstdc++-fd9f4683.so.6.0.28
 Comment: 
 
-Filename: xw_cbase-1.0.3.dist-info/top_level.txt
+Filename: xw_cbase.libs/libgcc_s-4e37474d.so.1
 Comment: 
 
-Filename: xw_cbase-1.0.3.dist-info/RECORD
+Filename: xw_cbase-16.0.1.dist-info/METADATA
+Comment: 
+
+Filename: xw_cbase-16.0.1.dist-info/WHEEL
+Comment: 
+
+Filename: xw_cbase-16.0.1.dist-info/LICENSE
+Comment: 
+
+Filename: xw_cbase-16.0.1.dist-info/RECORD
+Comment: 
+
+Filename: xw_cbase-16.0.1.dist-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `xw_cbase-1.0.3.dist-info/LICENSE` & `xw_cbase-16.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

