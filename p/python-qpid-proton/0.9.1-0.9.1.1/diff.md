# Comparing `tmp/python-qpid-proton-0.9.1.tar.bz2` & `tmp/python-qpid-proton-0.9.1.1.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-bzip2 compressed data, block size = 900k
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-Bzip2File
+ZipFile
```

