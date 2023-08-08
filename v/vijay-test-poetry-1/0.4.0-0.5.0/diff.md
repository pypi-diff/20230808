# Comparing `tmp/vijay_test_poetry_1-0.4.0.tar.gz` & `tmp/vijay_test_poetry_1-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vijay_test_poetry_1-0.4.0.tar", max compression
+gzip compressed data, was "vijay_test_poetry_1-0.5.0.tar", max compression
```

## Comparing `vijay_test_poetry_1-0.4.0.tar` & `vijay_test_poetry_1-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-08-07 06:07:12.055091 vijay_test_poetry_1-0.4.0/README.md
--rw-r--r--   0        0        0      321 2023-08-08 06:51:34.154493 vijay_test_poetry_1-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-08-08 06:51:13.243381 vijay_test_poetry_1-0.4.0/vijay_test_poetry_1/__init__.py
--rw-r--r--   0        0        0       57 2023-08-08 06:42:57.175991 vijay_test_poetry_1-0.4.0/vijay_test_poetry_1/clean.py
--rw-r--r--   0        0        0      342 1970-01-01 00:00:00.000000 vijay_test_poetry_1-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-07 06:07:12.055091 vijay_test_poetry_1-0.5.0/README.md
+-rw-r--r--   0        0        0      321 2023-08-08 07:10:05.259148 vijay_test_poetry_1-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-08 07:09:51.862828 vijay_test_poetry_1-0.5.0/vijay_test_poetry_1/__init__.py
+-rw-r--r--   0        0        0       57 2023-08-08 06:42:57.175991 vijay_test_poetry_1-0.5.0/vijay_test_poetry_1/clean.py
+-rw-r--r--   0        0        0      342 1970-01-01 00:00:00.000000 vijay_test_poetry_1-0.5.0/PKG-INFO
```

