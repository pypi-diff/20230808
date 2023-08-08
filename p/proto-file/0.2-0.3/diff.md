# Comparing `tmp/proto-file-0.2.tar.gz` & `tmp/proto_file-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proto-file-0.2.tar", last modified: Tue Aug  8 08:02:24 2023, max compression
+gzip compressed data, was "proto_file-0.3.tar", last modified: Tue Aug  8 08:08:28 2023, max compression
```

## Comparing `proto-file-0.2.tar` & `proto_file-0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 08:02:24.316044 proto-file-0.2/
--rw-rw-rw-   0        0        0       79 2023-08-08 08:02:24.316044 proto-file-0.2/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-08-02 06:59:30.000000 proto-file-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-08 08:02:24.315046 proto-file-0.2/proto_file.egg-info/
--rw-rw-rw-   0        0        0       79 2023-08-08 08:02:24.000000 proto-file-0.2/proto_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      154 2023-08-08 08:02:24.000000 proto-file-0.2/proto_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 08:02:24.000000 proto-file-0.2/proto_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 08:02:24.000000 proto-file-0.2/proto_file.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-08 08:02:24.316044 proto-file-0.2/setup.cfg
--rw-rw-rw-   0        0        0      258 2023-08-08 08:02:13.000000 proto-file-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 08:08:28.215029 proto_file-0.3/
+-rw-rw-rw-   0        0        0       79 2023-08-08 08:08:28.215029 proto_file-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-08-02 06:59:30.000000 proto_file-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 08:08:28.214029 proto_file-0.3/proto_file.egg-info/
+-rw-rw-rw-   0        0        0       79 2023-08-08 08:08:28.000000 proto_file-0.3/proto_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2023-08-08 08:08:28.000000 proto_file-0.3/proto_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 08:08:28.000000 proto_file-0.3/proto_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 08:08:28.000000 proto_file-0.3/proto_file.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 08:08:28.215029 proto_file-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      258 2023-08-08 08:07:50.000000 proto_file-0.3/setup.py
```

