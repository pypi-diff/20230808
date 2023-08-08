# Comparing `tmp/awesome_library-0.1.0.tar.gz` & `tmp/awesome_library-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awesome_library-0.1.0.tar", max compression
+gzip compressed data, was "awesome_library-0.1.1.tar", max compression
```

## Comparing `awesome_library-0.1.0.tar` & `awesome_library-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-08-08 12:58:23.164279 awesome_library-0.1.0/README.md
--rw-r--r--   0        0        0       77 2023-08-08 13:30:50.079760 awesome_library-0.1.0/awesome_library/__init__.py
--rw-r--r--   0        0        0      352 2023-08-08 13:07:08.910388 awesome_library-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 awesome_library-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-08 12:58:23.164279 awesome_library-0.1.1/README.md
+-rw-r--r--   0        0        0       56 2023-08-08 13:38:45.678133 awesome_library-0.1.1/awesome_library/awesome.py
+-rw-r--r--   0        0        0      352 2023-08-08 13:41:09.132083 awesome_library-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 awesome_library-0.1.1/PKG-INFO
```

