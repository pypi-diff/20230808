# Comparing `tmp/InputUtilsSidd-1.1.3.tar.gz` & `tmp/InputUtilsSidd-1.1.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InputUtilsSidd-1.1.3.tar", last modified: Sun Aug  6 18:52:17 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

