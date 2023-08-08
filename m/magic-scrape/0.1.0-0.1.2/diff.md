# Comparing `tmp/magic_scrape-0.1.0.tar.gz` & `tmp/magic_scrape-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magic_scrape-0.1.0.tar", last modified: Sat Aug  5 18:56:41 2023, max compression
+gzip compressed data, was "magic_scrape-0.1.2.tar", last modified: Tue Aug  8 00:43:46 2023, max compression
```

## Comparing `magic_scrape-0.1.0.tar` & `magic_scrape-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,14 @@
--rw-r--r--   0        0        0      534 2023-08-05 17:50:40.160547 magic_scrape-0.1.0/README.md
--rw-r--r--   0        0        0      522 2023-08-05 18:56:41.443942 magic_scrape-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       57 2023-08-05 17:24:51.701599 magic_scrape-0.1.0/src/magic_scrape/__init__.py
--rw-r--r--   0        0        0        0 2023-08-05 11:41:58.000000 magic_scrape-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 magic_scrape-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      661 2023-08-08 00:43:32.799912 magic_scrape-0.1.2/README.md
+-rw-r--r--   0        0        0     1396 2023-08-08 00:43:46.331840 magic_scrape-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-08-08 00:43:32.799912 magic_scrape-0.1.2/src/magic_scrape/__init__.py
+-rw-r--r--   0        0        0     1005 2023-08-08 00:15:37.752174 magic_scrape-0.1.2/src/magic_scrape/cli.py
+-rw-r--r--   0        0        0     1835 2023-08-08 00:15:37.752174 magic_scrape-0.1.2/src/magic_scrape/config.py
+-rw-r--r--   0        0        0       96 2023-08-08 00:15:37.752174 magic_scrape-0.1.2/src/magic_scrape/log.py
+-rw-r--r--   0        0        0     1805 2023-08-08 00:15:37.752174 magic_scrape-0.1.2/src/magic_scrape/scrape.py
+-rw-r--r--   0        0        0        0 2023-08-05 11:41:58.000000 magic_scrape-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     2577 2023-08-08 00:15:37.752174 magic_scrape-0.1.2/tests/cli_test.py
+-rw-r--r--   0        0        0      161 2023-08-08 00:15:37.752174 magic_scrape-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0      575 2023-08-08 00:15:37.752174 magic_scrape-0.1.2/tests/helpers/extraction.py
+-rw-r--r--   0        0        0     1416 2023-08-08 00:15:37.752174 magic_scrape-0.1.2/tests/helpers/fixtures.py
+-rw-r--r--   0        0        0     2170 2023-08-08 00:15:37.752174 magic_scrape-0.1.2/tests/scrape_test.py
+-rw-r--r--   0        0        0     1670 1970-01-01 00:00:00.000000 magic_scrape-0.1.2/PKG-INFO
```

### Comparing `magic_scrape-0.1.0/README.md` & `magic_scrape-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
 # magic-scrape
 
 ![PyPI](https://img.shields.io/pypi/v/magic-scrape?logo=python&logoColor=%23cccccc)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/lmmx/magic-scrape/master.svg)](https://results.pre-commit.ci/latest/github/lmmx/magic-scrape/master)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/magic-scrape.svg)](https://pypi.org/project/magic-scrape)
 
 <!-- [![build status](https://github.com/lmmx/magic-scrape/actions/workflows/master.yml/badge.svg)](https://github.com/lmmx/magic-scrape/actions/workflows/master.yml) -->
```

