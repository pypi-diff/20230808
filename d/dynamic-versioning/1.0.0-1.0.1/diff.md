# Comparing `tmp/dynamic-versioning-1.0.0.tar.gz` & `tmp/dynamic_versioning-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-versioning-1.0.0.tar", last modified: Wed Oct 20 03:34:58 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

