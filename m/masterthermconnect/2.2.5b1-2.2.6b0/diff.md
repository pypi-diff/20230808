# Comparing `tmp/masterthermconnect-2.2.5b1.tar.gz` & `tmp/masterthermconnect-2.2.6b0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masterthermconnect-2.2.5b1.tar", last modified: Wed Jun 14 15:08:58 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

