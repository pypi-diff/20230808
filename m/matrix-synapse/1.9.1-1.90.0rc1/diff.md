# Comparing `tmp/matrix-synapse-1.9.1.tar.gz` & `tmp/matrix_synapse-1.90.0rc1-cp38-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/matrix-synapse-1.9.1.tar", last modified: Tue Jan 28 13:38:15 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

