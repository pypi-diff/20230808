# Comparing `tmp/citsci_notebook_core_pipeline-0.0.4.tar.gz` & `tmp/citsci_notebook_core_pipeline-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citsci_notebook_core_pipeline-0.0.4.tar", last modified: Tue Aug  8 18:47:33 2023, max compression
+gzip compressed data, was "citsci_notebook_core_pipeline-0.1.tar", last modified: Tue Aug  8 18:53:20 2023, max compression
```

## Comparing `citsci_notebook_core_pipeline-0.0.4.tar` & `citsci_notebook_core_pipeline-0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:47:33.222340 citsci_notebook_core_pipeline-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-08-08 18:47:22.000000 citsci_notebook_core_pipeline-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-08 18:47:33.222340 citsci_notebook_core_pipeline-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-08 18:47:22.000000 citsci_notebook_core_pipeline-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-08 18:47:22.000000 citsci_notebook_core_pipeline-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 18:47:33.222340 citsci_notebook_core_pipeline-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:47:33.222340 citsci_notebook_core_pipeline-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:47:33.222340 citsci_notebook_core_pipeline-0.0.4/src/citsci_notebook_core_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:47:22.000000 citsci_notebook_core_pipeline-0.0.4/src/citsci_notebook_core_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-08-08 18:47:22.000000 citsci_notebook_core_pipeline-0.0.4/src/citsci_notebook_core_pipeline/rubin_citsci_core_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:47:33.222340 citsci_notebook_core_pipeline-0.0.4/src/citsci_notebook_core_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-08 18:47:33.000000 citsci_notebook_core_pipeline-0.0.4/src/citsci_notebook_core_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-08 18:47:33.000000 citsci_notebook_core_pipeline-0.0.4/src/citsci_notebook_core_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:47:33.000000 citsci_notebook_core_pipeline-0.0.4/src/citsci_notebook_core_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-08 18:47:33.000000 citsci_notebook_core_pipeline-0.0.4/src/citsci_notebook_core_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 18:47:33.000000 citsci_notebook_core_pipeline-0.0.4/src/citsci_notebook_core_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:53:20.182358 citsci_notebook_core_pipeline-0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-08-08 18:53:08.000000 citsci_notebook_core_pipeline-0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-08 18:53:20.182358 citsci_notebook_core_pipeline-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-08 18:53:08.000000 citsci_notebook_core_pipeline-0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-08 18:53:08.000000 citsci_notebook_core_pipeline-0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 18:53:20.182358 citsci_notebook_core_pipeline-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:53:20.182358 citsci_notebook_core_pipeline-0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:53:20.182358 citsci_notebook_core_pipeline-0.1/src/citsci_notebook_core_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:53:08.000000 citsci_notebook_core_pipeline-0.1/src/citsci_notebook_core_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-08-08 18:53:08.000000 citsci_notebook_core_pipeline-0.1/src/citsci_notebook_core_pipeline/rubin_citsci_core_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:53:20.182358 citsci_notebook_core_pipeline-0.1/src/citsci_notebook_core_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-08 18:53:20.000000 citsci_notebook_core_pipeline-0.1/src/citsci_notebook_core_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-08 18:53:20.000000 citsci_notebook_core_pipeline-0.1/src/citsci_notebook_core_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:53:20.000000 citsci_notebook_core_pipeline-0.1/src/citsci_notebook_core_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-08 18:53:20.000000 citsci_notebook_core_pipeline-0.1/src/citsci_notebook_core_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 18:53:20.000000 citsci_notebook_core_pipeline-0.1/src/citsci_notebook_core_pipeline.egg-info/top_level.txt
```

### Comparing `citsci_notebook_core_pipeline-0.0.4/LICENSE` & `citsci_notebook_core_pipeline-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `citsci_notebook_core_pipeline-0.0.4/src/citsci_notebook_core_pipeline/rubin_citsci_core_pipeline.py` & `citsci_notebook_core_pipeline-0.1/src/citsci_notebook_core_pipeline/rubin_citsci_core_pipeline.py`

 * *Files identical despite different names*

