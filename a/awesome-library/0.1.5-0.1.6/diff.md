# Comparing `tmp/awesome_library-0.1.5.tar.gz` & `tmp/awesome_library-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awesome_library-0.1.5.tar", max compression
+gzip compressed data, was "awesome_library-0.1.6.tar", max compression
```

## Comparing `awesome_library-0.1.5.tar` & `awesome_library-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-08-08 12:58:23.164279 awesome_library-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-08-08 13:54:40.486662 awesome_library-0.1.5/awesome_library/__init__.py
--rw-r--r--   0        0        0       56 2023-08-08 13:38:45.678133 awesome_library-0.1.5/awesome_library/awesome.py
--rw-r--r--   0        0        0      387 2023-08-08 14:02:35.524864 awesome_library-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 awesome_library-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-08 12:58:23.164279 awesome_library-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-08-08 13:54:40.486662 awesome_library-0.1.6/awesome_library/__init__.py
+-rw-r--r--   0        0        0       56 2023-08-08 13:38:45.678133 awesome_library-0.1.6/awesome_library/awesome.py
+-rw-r--r--   0        0        0      344 2023-08-08 14:03:34.109541 awesome_library-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 awesome_library-0.1.6/PKG-INFO
```

