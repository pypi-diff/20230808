# Comparing `tmp/rzpipe-0.5.1.tar.gz` & `tmp/rzpipe-0.6.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rzpipe-0.5.1.tar", last modified: Thu May 25 17:32:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

