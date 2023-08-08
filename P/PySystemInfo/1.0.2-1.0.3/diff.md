# Comparing `tmp/PySystemInfo-1.0.2.tar.gz` & `tmp/PySystemInfo-1.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySystemInfo-1.0.2.tar", last modified: Tue Aug  8 05:25:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

