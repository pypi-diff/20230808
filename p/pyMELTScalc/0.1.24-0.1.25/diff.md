# Comparing `tmp/pyMELTScalc-0.1.24.tar.gz` & `tmp/pyMELTScalc-0.1.25-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyMELTScalc-0.1.24.tar", last modified: Thu Jul  6 19:41:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

