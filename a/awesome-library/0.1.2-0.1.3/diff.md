# Comparing `tmp/awesome_library-0.1.2.tar.gz` & `tmp/awesome_library-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awesome_library-0.1.2.tar", max compression
+gzip compressed data, was "awesome_library-0.1.3.tar", max compression
```

## Comparing `awesome_library-0.1.2.tar` & `awesome_library-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-08-08 12:58:23.164279 awesome_library-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-08-08 13:46:04.589986 awesome_library-0.1.2/awesome_library/__init__.py
--rw-r--r--   0        0        0       56 2023-08-08 13:38:45.678133 awesome_library-0.1.2/awesome_library/awesome.py
--rw-r--r--   0        0        0      352 2023-08-08 13:46:25.371385 awesome_library-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 awesome_library-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-08 12:58:23.164279 awesome_library-0.1.3/README.md
+-rw-r--r--   0        0        0       55 2023-08-08 13:53:34.679272 awesome_library-0.1.3/awesome_library/__init__.py
+-rw-r--r--   0        0        0       56 2023-08-08 13:38:45.678133 awesome_library-0.1.3/awesome_library/awesome.py
+-rw-r--r--   0        0        0      352 2023-08-08 13:53:34.683345 awesome_library-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 awesome_library-0.1.3/PKG-INFO
```

