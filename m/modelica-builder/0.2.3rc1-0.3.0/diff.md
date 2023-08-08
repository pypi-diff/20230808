# Comparing `tmp/modelica-builder-0.2.3rc1.tar.gz` & `tmp/modelica-builder-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelica-builder-0.2.3rc1.tar", last modified: Wed Mar  1 17:23:40 2023, max compression
+gzip compressed data, was "modelica-builder-0.3.0.tar", last modified: Tue Aug  8 21:14:50 2023, max compression
```

## Comparing `modelica-builder-0.2.3rc1.tar` & `modelica-builder-0.3.0.tar`

### file list

```diff
@@ -1,68 +1,36 @@
-drwxr-xr-x   0 nlong    (1200847960) 18434217        0 2023-03-01 17:23:40.860897 modelica-builder-0.2.3rc1/
-drwxr-xr-x   0 nlong    (1200847960) 18434217        0 2023-03-01 17:23:40.824304 modelica-builder-0.2.3rc1/.github/
-drwxr-xr-x   0 nlong    (1200847960) 18434217        0 2023-03-01 17:23:40.828508 modelica-builder-0.2.3rc1/.github/workflows/
--rw-r--r--   0 nlong    (1200847960) 18434217      726 2023-03-01 17:18:19.000000 modelica-builder-0.2.3rc1/.github/workflows/ci.yml
--rw-r--r--   0 nlong    (1200847960) 18434217      651 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/.gitignore
--rw-r--r--   0 nlong    (1200847960) 18434217      284 2020-02-20 01:04:51.000000 modelica-builder-0.2.3rc1/.isort.cfg
--rw-r--r--   0 nlong    (1200847960) 18434217     1406 2023-03-01 17:18:19.000000 modelica-builder-0.2.3rc1/.pre-commit-config.yaml
--rw-r--r--   0 nlong    (1200847960) 18434217      112 2020-02-20 01:04:52.000000 modelica-builder-0.2.3rc1/AUTHORS.rst
--rw-r--r--   0 nlong    (1200847960) 18434217      989 2023-03-01 17:22:02.000000 modelica-builder-0.2.3rc1/CHANGELOG.rst
--rw-r--r--   0 nlong    (1200847960) 18434217     1550 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/LICENSE.txt
--rw-r--r--   0 nlong    (1200847960) 18434217     5888 2023-03-01 17:23:40.861192 modelica-builder-0.2.3rc1/PKG-INFO
--rw-r--r--   0 nlong    (1200847960) 18434217     4999 2022-04-28 20:42:55.000000 modelica-builder-0.2.3rc1/README.rst
-drwxr-xr-x   0 nlong    (1200847960) 18434217        0 2023-03-01 17:23:40.828767 modelica-builder-0.2.3rc1/antlr/
--rw-r--r--   0 nlong    (1200847960) 18434217      253 2022-06-01 14:25:47.000000 modelica-builder-0.2.3rc1/antlr/Dockerfile
-drwxr-xr-x   0 nlong    (1200847960) 18434217        0 2023-03-01 17:23:40.830926 modelica-builder-0.2.3rc1/docs/
--rw-r--r--   0 nlong    (1200847960) 18434217     7622 2020-02-20 01:04:52.000000 modelica-builder-0.2.3rc1/docs/Makefile
-drwxr-xr-x   0 nlong    (1200847960) 18434217        0 2023-03-01 17:23:40.831208 modelica-builder-0.2.3rc1/docs/_static/
--rw-r--r--   0 nlong    (1200847960) 18434217       18 2020-02-20 01:04:52.000000 modelica-builder-0.2.3rc1/docs/_static/.gitignore
--rw-r--r--   0 nlong    (1200847960) 18434217       41 2020-02-20 01:04:52.000000 modelica-builder-0.2.3rc1/docs/authors.rst
--rw-r--r--   0 nlong    (1200847960) 18434217       43 2020-02-20 01:04:52.000000 modelica-builder-0.2.3rc1/docs/changelog.rst
--rw-r--r--   0 nlong    (1200847960) 18434217     9232 2021-03-04 01:39:13.000000 modelica-builder-0.2.3rc1/docs/conf.py
--rw-r--r--   0 nlong    (1200847960) 18434217     2257 2020-02-20 01:04:52.000000 modelica-builder-0.2.3rc1/docs/index.rst
--rw-r--r--   0 nlong    (1200847960) 18434217       67 2020-02-20 01:04:52.000000 modelica-builder-0.2.3rc1/docs/license.rst
-drwxr-xr-x   0 nlong    (1200847960) 18434217        0 2023-03-01 17:23:40.833964 modelica-builder-0.2.3rc1/modelica_builder/
--rw-r--r--   0 nlong    (1200847960) 18434217      525 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/modelica_builder/__init__.py
--rw-r--r--   0 nlong    (1200847960) 18434217     9387 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/modelica_builder/builder.py
--rw-r--r--   0 nlong    (1200847960) 18434217      591 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/modelica_builder/config.py
--rw-r--r--   0 nlong    (1200847960) 18434217     7173 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/modelica_builder/edit.py
--rw-r--r--   0 nlong    (1200847960) 18434217    15934 2023-03-01 17:18:19.000000 modelica-builder-0.2.3rc1/modelica_builder/model.py
-drwxr-xr-x   0 nlong    (1200847960) 18434217        0 2023-03-01 17:23:40.849704 modelica-builder-0.2.3rc1/modelica_builder/modelica_parser/
--rw-r--r--   0 nlong    (1200847960) 18434217       81 2020-09-30 14:57:17.000000 modelica-builder-0.2.3rc1/modelica_builder/modelica_parser/README.rst
--rw-r--r--   0 nlong    (1200847960) 18434217      301 2020-04-01 14:07:48.000000 modelica-builder-0.2.3rc1/modelica_builder/modelica_parser/__init__.py
--rw-r--r--   0 nlong    (1200847960) 18434217     9376 2020-06-25 16:05:30.000000 modelica-builder-0.2.3rc1/modelica_builder/modelica_parser/modelica.g4
--rw-r--r--   0 nlong    (1200847960) 18434217    37041 2022-06-01 14:23:15.000000 modelica-builder-0.2.3rc1/modelica_builder/modelica_parser/modelica.interp
--rw-r--r--   0 nlong    (1200847960) 18434217     1767 2022-06-01 14:23:16.000000 modelica-builder-0.2.3rc1/modelica_builder/modelica_parser/modelica.tokens
--rw-r--r--   0 nlong    (1200847960) 18434217    27251 2022-06-01 14:23:15.000000 modelica-builder-0.2.3rc1/modelica_builder/modelica_parser/modelicaLexer.interp
--rw-r--r--   0 nlong    (1200847960) 18434217    30762 2022-06-01 14:23:15.000000 modelica-builder-0.2.3rc1/modelica_builder/modelica_parser/modelicaLexer.py
--rw-r--r--   0 nlong    (1200847960) 18434217     1767 2022-06-01 14:23:15.000000 modelica-builder-0.2.3rc1/modelica_builder/modelica_parser/modelicaLexer.tokens
--rw-r--r--   0 nlong    (1200847960) 18434217    25878 2022-06-01 14:23:16.000000 modelica-builder-0.2.3rc1/modelica_builder/modelica_parser/modelicaListener.py
--rw-r--r--   0 nlong    (1200847960) 18434217   248104 2022-06-01 14:23:16.000000 modelica-builder-0.2.3rc1/modelica_builder/modelica_parser/modelicaParser.py
--rw-r--r--   0 nlong    (1200847960) 18434217     2151 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/modelica_builder/modelica_parser/utils.py
--rw-r--r--   0 nlong    (1200847960) 18434217    16877 2023-03-01 17:18:19.000000 modelica-builder-0.2.3rc1/modelica_builder/selector.py
--rw-r--r--   0 nlong    (1200847960) 18434217     8409 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/modelica_builder/transformation.py
--rw-r--r--   0 nlong    (1200847960) 18434217     1612 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/modelica_builder/transformer.py
-drwxr-xr-x   0 nlong    (1200847960) 18434217        0 2023-03-01 17:23:40.836675 modelica-builder-0.2.3rc1/modelica_builder.egg-info/
--rw-r--r--   0 nlong    (1200847960) 18434217     5888 2023-03-01 17:23:40.000000 modelica-builder-0.2.3rc1/modelica_builder.egg-info/PKG-INFO
--rw-r--r--   0 nlong    (1200847960) 18434217     1533 2023-03-01 17:23:40.000000 modelica-builder-0.2.3rc1/modelica_builder.egg-info/SOURCES.txt
--rw-r--r--   0 nlong    (1200847960) 18434217        1 2023-03-01 17:23:40.000000 modelica-builder-0.2.3rc1/modelica_builder.egg-info/dependency_links.txt
--rw-r--r--   0 nlong    (1200847960) 18434217        1 2022-06-07 20:35:23.000000 modelica-builder-0.2.3rc1/modelica_builder.egg-info/not-zip-safe
--rw-r--r--   0 nlong    (1200847960) 18434217       57 2023-03-01 17:23:40.000000 modelica-builder-0.2.3rc1/modelica_builder.egg-info/requires.txt
--rw-r--r--   0 nlong    (1200847960) 18434217       17 2023-03-01 17:23:40.000000 modelica-builder-0.2.3rc1/modelica_builder.egg-info/top_level.txt
--rw-r--r--   0 nlong    (1200847960) 18434217      194 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/requirements.txt
--rw-r--r--   0 nlong    (1200847960) 18434217     1609 2023-03-01 17:23:40.862845 modelica-builder-0.2.3rc1/setup.cfg
--rwxr-xr-x   0 nlong    (1200847960) 18434217     2874 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/setup.py
-drwxr-xr-x   0 nlong    (1200847960) 18434217        0 2023-03-01 17:23:40.854180 modelica-builder-0.2.3rc1/tests/
--rw-r--r--   0 nlong    (1200847960) 18434217        0 2020-02-20 01:04:52.000000 modelica-builder-0.2.3rc1/tests/__init__.py
--rw-r--r--   0 nlong    (1200847960) 18434217      517 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/tests/conftest.py
-drwxr-xr-x   0 nlong    (1200847960) 18434217        0 2023-03-01 17:23:40.860233 modelica-builder-0.2.3rc1/tests/data/
--rw-r--r--   0 nlong    (1200847960) 18434217      484 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/tests/data/DCMotor.mo
--rw-r--r--   0 nlong    (1200847960) 18434217      430 2022-04-28 20:42:55.000000 modelica-builder-0.2.3rc1/tests/data/DCMotorCRLF.mo
--rw-r--r--   0 nlong    (1200847960) 18434217    14560 2023-03-01 17:18:19.000000 modelica-builder-0.2.3rc1/tests/data/Office.mo
--rw-r--r--   0 nlong    (1200847960) 18434217     1057 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/tests/test_benchmarks.py
--rw-r--r--   0 nlong    (1200847960) 18434217     4611 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/tests/test_builder.py
--rw-r--r--   0 nlong    (1200847960) 18434217     1342 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/tests/test_edit.py
--rw-r--r--   0 nlong    (1200847960) 18434217    31413 2023-03-01 17:18:19.000000 modelica-builder-0.2.3rc1/tests/test_model.py
--rw-r--r--   0 nlong    (1200847960) 18434217     2919 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/tests/test_selector.py
--rw-r--r--   0 nlong    (1200847960) 18434217     5153 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/tests/tests.py
--rw-r--r--   0 nlong    (1200847960) 18434217      279 2022-06-07 20:34:21.000000 modelica-builder-0.2.3rc1/tox.ini
+drwxr-xr-x   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)        0 2023-08-08 21:14:50.907322 modelica-builder-0.3.0/
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)      112 2020-02-20 01:04:52.000000 modelica-builder-0.3.0/AUTHORS.rst
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)     1550 2023-04-11 11:34:29.000000 modelica-builder-0.3.0/LICENSE.txt
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)     6087 2023-08-08 21:14:50.907588 modelica-builder-0.3.0/PKG-INFO
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)     5188 2023-08-08 21:14:48.000000 modelica-builder-0.3.0/README.rst
+drwxr-xr-x   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)        0 2023-08-08 21:14:50.899671 modelica-builder-0.3.0/modelica_builder/
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)      525 2022-06-07 20:34:21.000000 modelica-builder-0.3.0/modelica_builder/__init__.py
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)     9387 2023-04-11 11:34:29.000000 modelica-builder-0.3.0/modelica_builder/builder.py
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)      591 2023-04-11 11:34:29.000000 modelica-builder-0.3.0/modelica_builder/config.py
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)     7173 2023-04-11 11:34:29.000000 modelica-builder-0.3.0/modelica_builder/edit.py
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)    19541 2023-08-08 21:14:48.000000 modelica-builder-0.3.0/modelica_builder/model.py
+drwxr-xr-x   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)        0 2023-08-08 21:14:50.903923 modelica-builder-0.3.0/modelica_builder/modelica_parser/
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)      301 2020-04-01 14:07:48.000000 modelica-builder-0.3.0/modelica_builder/modelica_parser/__init__.py
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)    30762 2022-06-01 14:23:15.000000 modelica-builder-0.3.0/modelica_builder/modelica_parser/modelicaLexer.py
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)    25878 2022-06-01 14:23:16.000000 modelica-builder-0.3.0/modelica_builder/modelica_parser/modelicaListener.py
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)   248104 2022-06-01 14:23:16.000000 modelica-builder-0.3.0/modelica_builder/modelica_parser/modelicaParser.py
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)     2151 2023-04-11 11:34:29.000000 modelica-builder-0.3.0/modelica_builder/modelica_parser/utils.py
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)    21715 2023-08-08 21:14:48.000000 modelica-builder-0.3.0/modelica_builder/selector.py
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)     8409 2023-04-11 11:34:29.000000 modelica-builder-0.3.0/modelica_builder/transformation.py
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)     1612 2023-04-11 11:34:29.000000 modelica-builder-0.3.0/modelica_builder/transformer.py
+drwxr-xr-x   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)        0 2023-08-08 21:14:50.901751 modelica-builder-0.3.0/modelica_builder.egg-info/
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)     6087 2023-08-08 21:14:50.000000 modelica-builder-0.3.0/modelica_builder.egg-info/PKG-INFO
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)      887 2023-08-08 21:14:50.000000 modelica-builder-0.3.0/modelica_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)        1 2023-08-08 21:14:50.000000 modelica-builder-0.3.0/modelica_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)        1 2023-08-08 19:54:16.000000 modelica-builder-0.3.0/modelica_builder.egg-info/not-zip-safe
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)       57 2023-08-08 21:14:50.000000 modelica-builder-0.3.0/modelica_builder.egg-info/requires.txt
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)       17 2023-08-08 21:14:50.000000 modelica-builder-0.3.0/modelica_builder.egg-info/top_level.txt
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)     1618 2023-08-08 21:14:50.909449 modelica-builder-0.3.0/setup.cfg
+-rwxr-xr-x   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)     2875 2023-08-08 21:14:48.000000 modelica-builder-0.3.0/setup.py
+drwxr-xr-x   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)        0 2023-08-08 21:14:50.906828 modelica-builder-0.3.0/tests/
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)     1057 2023-04-11 11:34:29.000000 modelica-builder-0.3.0/tests/test_benchmarks.py
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)     4611 2023-04-11 11:34:29.000000 modelica-builder-0.3.0/tests/test_builder.py
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)     1342 2023-04-11 11:34:29.000000 modelica-builder-0.3.0/tests/test_edit.py
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)    35131 2023-08-08 21:14:48.000000 modelica-builder-0.3.0/tests/test_model.py
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)     2919 2023-04-11 11:34:29.000000 modelica-builder-0.3.0/tests/test_selector.py
+-rw-r--r--   0 nlong    (1200847960) NREL_NT\Domain Users (18434217)     5153 2023-04-11 11:34:29.000000 modelica-builder-0.3.0/tests/tests.py
```

### Comparing `modelica-builder-0.2.3rc1/LICENSE.txt` & `modelica-builder-0.3.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2020-2022, Alliance for Sustainable Energy, LLC.
+Copyright (c) 2020-2023, Alliance for Sustainable Energy, LLC.
 All rights reserved.
 
 BSD 3-Clause License
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
```

### Comparing `modelica-builder-0.2.3rc1/PKG-INFO` & `modelica-builder-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: modelica-builder
-Version: 0.2.3rc1
-Summary: Modelica builder enables parsing and modification of Modelica files
+Version: 0.3.0
+Summary: Modelica builder enables programmatic parsing and modification of Modelica files
 Home-page: https://github.com/urbanopt/modelica-builder
 Author: Nicholas Long
 Author-email: nicholas.long@nrel.gov
 License: BSD-3 Clause
 Project-URL: Documentation, https://github.com/urbanopt/modelica-builder
 Project-URL: Source, https://github.com/urbanopt/modelica-builder
 Project-URL: Changelog, https://github.com/urbanopt/modelica-builder/blob/main/CHANGELOG.rst
@@ -15,19 +15,17 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 
-===========================
-Modelica Builder (ModBuild)
-===========================
-
-*Note: this project is still in flux and the name/methods/namespaces may change*
+================
+Modelica Builder
+================
 
 The Modelica Builder  project aims to make in-place modifcations to Modelica language files easier.
 The principal use case is to load, modify using higher level abstracted methods, and then save the
 resulting file. The user has access to the entire Abstract Syntax Tree of the entire Modelica grammar.
 
 The Modelica Builder project does not:
 
@@ -156,15 +154,19 @@
 
 * The transformations occur on strings which are immutable. Need to investigate using byte arrays. This does not cause errors, but can be slow when parsing really large modelica files.
 
 Release Instructions
 --------------------
 
 * Bump version to <NEW_VERSION> in setup.cfg (use semantic versioning as much as possible).
-* Run `autopep8` to nicely format the code (or run `pre-commit --all-files`).
+* Run `pre-commit --all-files`
+* In a prep-release branch, push the changes to GitHub and draft a release against the latest branch.
+    * Run 'auto-generate changelog' and copy the contents to the CHANGELOG.rst. Cull any items that are repeated.
+    * Discard the draft release (you will create an official one off of the main branch)
+* Merge the prep-release branch into develop.
 * Create a PR against develop into main.
 * Run `git tag <NEW_VERSION>`. (Note that `python setup.py --version` pulls from the latest tag`.)
 * After main branch passes, then merge and checkout the main branch. Build the distribution using the following code:
 
 .. code-block:: bash
 
     # Remove old dist packages
```

### Comparing `modelica-builder-0.2.3rc1/README.rst` & `modelica-builder-0.3.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-===========================
-Modelica Builder (ModBuild)
-===========================
-
-*Note: this project is still in flux and the name/methods/namespaces may change*
+================
+Modelica Builder
+================
 
 The Modelica Builder  project aims to make in-place modifcations to Modelica language files easier.
 The principal use case is to load, modify using higher level abstracted methods, and then save the
 resulting file. The user has access to the entire Abstract Syntax Tree of the entire Modelica grammar.
 
 The Modelica Builder project does not:
 
@@ -135,15 +133,19 @@
 
 * The transformations occur on strings which are immutable. Need to investigate using byte arrays. This does not cause errors, but can be slow when parsing really large modelica files.
 
 Release Instructions
 --------------------
 
 * Bump version to <NEW_VERSION> in setup.cfg (use semantic versioning as much as possible).
-* Run `autopep8` to nicely format the code (or run `pre-commit --all-files`).
+* Run `pre-commit --all-files`
+* In a prep-release branch, push the changes to GitHub and draft a release against the latest branch.
+    * Run 'auto-generate changelog' and copy the contents to the CHANGELOG.rst. Cull any items that are repeated.
+    * Discard the draft release (you will create an official one off of the main branch)
+* Merge the prep-release branch into develop.
 * Create a PR against develop into main.
 * Run `git tag <NEW_VERSION>`. (Note that `python setup.py --version` pulls from the latest tag`.)
 * After main branch passes, then merge and checkout the main branch. Build the distribution using the following code:
 
 .. code-block:: bash
 
     # Remove old dist packages
```

### Comparing `modelica-builder-0.2.3rc1/modelica_builder/__init__.py` & `modelica-builder-0.3.0/modelica_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `modelica-builder-0.2.3rc1/modelica_builder/builder.py` & `modelica-builder-0.3.0/modelica_builder/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ****************************************************************************************************
-:copyright (c) 2020-2022, Alliance for Sustainable Energy, LLC.
+:copyright (c) 2020-2023, Alliance for Sustainable Energy, LLC.
 All rights reserved.
 ****************************************************************************************************
 """
 
 
 from modelica_builder import config
 from modelica_builder.edit import Edit
```

### Comparing `modelica-builder-0.2.3rc1/modelica_builder/config.py` & `modelica-builder-0.3.0/modelica_builder/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ****************************************************************************************************
-:copyright (c) 2020-2022, Alliance for Sustainable Energy, LLC.
+:copyright (c) 2020-2023, Alliance for Sustainable Energy, LLC.
 All rights reserved.
 ****************************************************************************************************
 """
 
 # global config variables
 # If true, then each inserted component/annotation argument will be indented on a new line
 INDENT_INSERTED_COMPONENT_ARGS = False
```

### Comparing `modelica-builder-0.2.3rc1/modelica_builder/edit.py` & `modelica-builder-0.3.0/modelica_builder/edit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ****************************************************************************************************
-:copyright (c) 2020-2022, Alliance for Sustainable Energy, LLC.
+:copyright (c) 2020-2023, Alliance for Sustainable Energy, LLC.
 All rights reserved.
 ****************************************************************************************************
 """
 
 
 from modelica_builder import modelica_parser
```

### Comparing `modelica-builder-0.2.3rc1/modelica_builder/model.py` & `modelica-builder-0.3.0/modelica_builder/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ****************************************************************************************************
-:copyright (c) 2020-2022, Alliance for Sustainable Energy, LLC.
+:copyright (c) 2020-2023, Alliance for Sustainable Energy, LLC.
 All rights reserved.
 ****************************************************************************************************
 """
 
 import logging
 import os
 
@@ -18,16 +18,18 @@
 from modelica_builder.selector import (
     ComponentArgumentSelector,
     ComponentDeclarationSelector,
     ComponentModificationNameSelector,
     ComponentModificationValueSelector,
     ComponentRedeclarationSelector,
     ConnectClauseSelector,
+    ExtendedComponentWithRedeclarationSelector,
     ModelIdentifierSelector,
     NthChildSelector,
+    ParameterSelector,
     ParentSelector,
     WithinSelector
 )
 from modelica_builder.transformation import (
     ComponentModificationsTransformation,
     ModelAnnotationTransformation,
     SimpleTransformation
@@ -177,17 +179,67 @@
                     .chain(
             ComponentModificationNameSelector(
                 old_argument_name
             )))
 
         self.add(SimpleTransformation(selector, Edit.make_replace(f'{new_argument_name}')))
 
-    def overwrite_component_redeclaration(self, type_, identifier, new_redeclaration, existing_redeclaration=None):
+    def update_extended_component_modification(self, extended_type, type_, identifier, obj_name, arg_name, new_value, if_value=None):
+        """Update arguments that exist as part of the extended component modification. This is a very specific case to handle
+        this structure:
+
+            extends extended_type(
+                redeclare type_ identifier[X](final Y=Y),
+                obj_name(
+                    arg_1=8,
+                    arg_2=1029.114,
+                    arg_name=new_value (if_value)
+                )
+            );
+
+        :param extended_type: string, name of the type being extended
+        :param type_: string, instance type that is being redeclared in the extended type
+        :param identifier: string, object name that is being extended
+        :param obj_name: string, object name that is being updated
+        :param arg_name: string, name of the argument that will be updated
+        :param new_value: string, new argument value
+        :param if_value: string, if provided it will only update the value if the existing value matches this
         """
-        Overwrite the component redeclaration with a new string
+        selector = (ExtendedComponentWithRedeclarationSelector(extended_type, type_, identifier, obj_name).chain(
+            ComponentModificationValueSelector(
+                arg_name,
+                modification_value=if_value
+            )
+        ))
+
+        self.add(SimpleTransformation(selector, Edit.make_replace(new_value)))
+
+    def get_component_argument_value(self, type_, identifier, argument_name, type_cast=str):
+        """Get the argument value of a component
+
+        :param type_: string, type of the component
+        :param identifier: string, component identifier
+        :param argument_name: string, name of the new argument name
+        """
+        selector = (ComponentDeclarationSelector(type_, identifier)
+                    .chain(
+            ComponentModificationValueSelector(
+                argument_name
+            )))
+        result = self.apply_selector(selector)
+        if result:
+            result = result[0].getText()
+            # cast the result to the type specified, if possible
+            try:
+                return type_cast(result)
+            except ValueError:
+                raise ValueError(f"Unable to type cast the value {result} to a {type_cast}")
+
+    def overwrite_component_redeclaration(self, type_, identifier, new_redeclaration, existing_redeclaration=None):
+        """Overwrite the component redeclaration with a new string
 
         :param type_: string, type of the component
         :param identifier: string, component identifier
         :param new_redeclaration: string, new component redeclaration string. It is the entire string, i.e., redeclare argument=value
         :param existing_redeclaration: string, existing argument redeclaration string. Defaults to None.
         """
         # In the case of `redeclare a.b.c update`, the existing declaration query is
@@ -303,14 +355,47 @@
 
         # Make sure that 0 is an allowed value (i.e., check for not None instead of truthy)
         if assigned_value is not None:
             parameter.set_value(assigned_value)
 
         self.add(parameter.transformation())
 
+    def get_parameter_value(self, type_, identifier):
+        selector = (ParameterSelector(type_, identifier))
+        result = self.apply_selector(selector)
+        if result:
+            result = result[0].getText()
+
+            # cast the result to the type specified, if possible
+            if type_ == 'Real':
+                type_cast = float
+            elif type_ == 'Integer':
+                type_cast = int
+            elif type_ == 'String':
+                type_cast = str
+            elif type_ == 'Boolean':
+                return result.lower() == 'true'
+
+            try:
+                return type_cast(result)
+            except ValueError:
+                raise ValueError(f"Unable to type cast the value {result} to a {type_cast}")
+
+    def update_parameter(self, type_: str, identifier: str, new_value):
+        """Read in an existing parameter and update with the new_value
+
+        Args:
+            type_ (str): Type of the parameter to update
+            identifier (str): Object name of the parameter to update
+            new_value (any): New value
+        """
+        selector = (ParameterSelector(type_, identifier))
+
+        self.add(SimpleTransformation(selector, Edit.make_replace(new_value)))
+
     def update_model_annotation(self, modifications):
         """Updates the model annotation modifications. If a modification exists
         then it is updated, if it doesn't then it is inserted. If this method is
         called more than once, previous calls are IGNORED and only the last call
         is used.
 
         The modifications param is a dictionary. Each key represents a modification
```

### Comparing `modelica-builder-0.2.3rc1/modelica_builder/modelica_parser/modelicaLexer.py` & `modelica-builder-0.3.0/modelica_builder/modelica_parser/modelicaLexer.py`

 * *Files identical despite different names*

### Comparing `modelica-builder-0.2.3rc1/modelica_builder/modelica_parser/modelicaListener.py` & `modelica-builder-0.3.0/modelica_builder/modelica_parser/modelicaListener.py`

 * *Files identical despite different names*

### Comparing `modelica-builder-0.2.3rc1/modelica_builder/modelica_parser/modelicaParser.py` & `modelica-builder-0.3.0/modelica_builder/modelica_parser/modelicaParser.py`

 * *Files identical despite different names*

### Comparing `modelica-builder-0.2.3rc1/modelica_builder/modelica_parser/utils.py` & `modelica-builder-0.3.0/modelica_builder/modelica_parser/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ****************************************************************************************************
-:copyright (c) 2020-2022, Alliance for Sustainable Energy, LLC.
+:copyright (c) 2020-2023, Alliance for Sustainable Energy, LLC.
 All rights reserved.
 ****************************************************************************************************
 """
 
 import sys
 
 from antlr4 import FileStream, CommonTokenStream
```

### Comparing `modelica-builder-0.2.3rc1/modelica_builder/transformation.py` & `modelica-builder-0.3.0/modelica_builder/transformation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ****************************************************************************************************
-:copyright (c) 2020-2022, Alliance for Sustainable Energy, LLC.
+:copyright (c) 2020-2023, Alliance for Sustainable Energy, LLC.
 All rights reserved.
 ****************************************************************************************************
 """
 
 
 import logging
 from antlr4.xpath import XPath
```

### Comparing `modelica-builder-0.2.3rc1/modelica_builder/transformer.py` & `modelica-builder-0.3.0/modelica_builder/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ****************************************************************************************************
-:copyright (c) 2020-2022, Alliance for Sustainable Energy, LLC.
+:copyright (c) 2020-2023, Alliance for Sustainable Energy, LLC.
 All rights reserved.
 ****************************************************************************************************
 """
 
 
 from modelica_builder.edit import Edit
 from modelica_builder.modelica_parser import parse
```

### Comparing `modelica-builder-0.2.3rc1/modelica_builder.egg-info/PKG-INFO` & `modelica-builder-0.3.0/modelica_builder.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: modelica-builder
-Version: 0.2.3rc1
-Summary: Modelica builder enables parsing and modification of Modelica files
+Version: 0.3.0
+Summary: Modelica builder enables programmatic parsing and modification of Modelica files
 Home-page: https://github.com/urbanopt/modelica-builder
 Author: Nicholas Long
 Author-email: nicholas.long@nrel.gov
 License: BSD-3 Clause
 Project-URL: Documentation, https://github.com/urbanopt/modelica-builder
 Project-URL: Source, https://github.com/urbanopt/modelica-builder
 Project-URL: Changelog, https://github.com/urbanopt/modelica-builder/blob/main/CHANGELOG.rst
@@ -15,19 +15,17 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 
-===========================
-Modelica Builder (ModBuild)
-===========================
-
-*Note: this project is still in flux and the name/methods/namespaces may change*
+================
+Modelica Builder
+================
 
 The Modelica Builder  project aims to make in-place modifcations to Modelica language files easier.
 The principal use case is to load, modify using higher level abstracted methods, and then save the
 resulting file. The user has access to the entire Abstract Syntax Tree of the entire Modelica grammar.
 
 The Modelica Builder project does not:
 
@@ -156,15 +154,19 @@
 
 * The transformations occur on strings which are immutable. Need to investigate using byte arrays. This does not cause errors, but can be slow when parsing really large modelica files.
 
 Release Instructions
 --------------------
 
 * Bump version to <NEW_VERSION> in setup.cfg (use semantic versioning as much as possible).
-* Run `autopep8` to nicely format the code (or run `pre-commit --all-files`).
+* Run `pre-commit --all-files`
+* In a prep-release branch, push the changes to GitHub and draft a release against the latest branch.
+    * Run 'auto-generate changelog' and copy the contents to the CHANGELOG.rst. Cull any items that are repeated.
+    * Discard the draft release (you will create an official one off of the main branch)
+* Merge the prep-release branch into develop.
 * Create a PR against develop into main.
 * Run `git tag <NEW_VERSION>`. (Note that `python setup.py --version` pulls from the latest tag`.)
 * After main branch passes, then merge and checkout the main branch. Build the distribution using the following code:
 
 .. code-block:: bash
 
     # Remove old dist packages
```

### Comparing `modelica-builder-0.2.3rc1/setup.cfg` & `modelica-builder-0.3.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = modelica-builder
-description = Modelica builder enables parsing and modification of Modelica files
-version = 0.2.3-rc1
+description = Modelica builder enables programmatic parsing and modification of Modelica files
+version = 0.3.0
 author = Nicholas Long
 author_email = nicholas.long@nrel.gov
 license = BSD-3 Clause
 url = https://github.com/urbanopt/modelica-builder
 project_urls = 
 	Documentation = https://github.com/urbanopt/modelica-builder
 	Source = https://github.com/urbanopt/modelica-builder
```

### Comparing `modelica-builder-0.2.3rc1/setup.py` & `modelica-builder-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 import os
 import re
 import sys
 
 PYTHON_REGEX = re.compile(r'^""".\*{100}.*:copyright.*\*{100}."""$', re.MULTILINE | re.DOTALL)
 PYTHON_LICENSE = '''"""
 ****************************************************************************************************
-:copyright (c) 2020-2022, Alliance for Sustainable Energy, LLC.
+:copyright (c) 2020-2023, Alliance for Sustainable Energy, LLC.
 All rights reserved.
 ****************************************************************************************************
 """'''
 
 EXCLUDE_FILES = ["__init__.py", "modelicaLexer.py", "modelicaListener.py", "modelicaParser.py"]
 PATHS = [
     {"glob": "modelica_builder/**/*.py", "license": PYTHON_LICENSE, "REGEX": PYTHON_REGEX, },
     {"glob": "tests/**/*.py", "license": PYTHON_LICENSE, "REGEX": PYTHON_REGEX},
     # single files
     # { "glob": 'bin/resources/**/file.py', "license": PYTHON_LICENSE, "REGEX": PYTHON_REGEX },
 ]
 
 
 class UpdateLicenses(distutils.cmd.Command):
-    """Custom comand for updating the license doc strings."""
+    """Custom command for updating the license doc strings."""
 
     description = "Update the license/copyright headers"
 
     user_options = []
 
     def initialize_options(self):
         pass
```

### Comparing `modelica-builder-0.2.3rc1/tests/test_benchmarks.py` & `modelica-builder-0.3.0/tests/test_benchmarks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ****************************************************************************************************
-:copyright (c) 2020-2022, Alliance for Sustainable Energy, LLC.
+:copyright (c) 2020-2023, Alliance for Sustainable Energy, LLC.
 All rights reserved.
 ****************************************************************************************************
 """
 
 
 # -*- coding: utf-8 -*-
```

### Comparing `modelica-builder-0.2.3rc1/tests/test_builder.py` & `modelica-builder-0.3.0/tests/test_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ****************************************************************************************************
-:copyright (c) 2020-2022, Alliance for Sustainable Energy, LLC.
+:copyright (c) 2020-2023, Alliance for Sustainable Energy, LLC.
 All rights reserved.
 ****************************************************************************************************
 """
 
 
 # -*- coding: utf-8 -*-
```

### Comparing `modelica-builder-0.2.3rc1/tests/test_edit.py` & `modelica-builder-0.3.0/tests/test_edit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ****************************************************************************************************
-:copyright (c) 2020-2022, Alliance for Sustainable Energy, LLC.
+:copyright (c) 2020-2023, Alliance for Sustainable Energy, LLC.
 All rights reserved.
 ****************************************************************************************************
 """
 
 
 # -*- coding: utf-8 -*-
```

### Comparing `modelica-builder-0.2.3rc1/tests/test_model.py` & `modelica-builder-0.3.0/tests/test_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ****************************************************************************************************
-:copyright (c) 2020-2022, Alliance for Sustainable Energy, LLC.
+:copyright (c) 2020-2023, Alliance for Sustainable Energy, LLC.
 All rights reserved.
 ****************************************************************************************************
 """
 
 import os
 import tempfile
 from unittest import TestCase
@@ -308,15 +308,45 @@
         self.result = model.execute()
 
         # Assert
         self.assertHasAdditions(source_file, self.result,
                                 ['parameter String myParam="supercalifragilisticexpialidocious" "a comment"'])
         self.assertNoDeletions(source_file, self.result)
 
-    def test_model_reclaration_string_replacement(self):
+    def test_get_parameter_value(self):
+        # Setup
+        source_file = os.path.join(self.data_dir, 'Office.mo')
+        model = Model(source_file)
+
+        # Act
+        result = model.get_parameter_value('String', 'idfName')
+        result_int = model.get_parameter_value('Integer', 'nPorts')
+        result_real = model.get_parameter_value('Real', 'fraLat')
+        result_bool = model.get_parameter_value('Boolean', 'use_moisture_balance')
+
+        # Assert
+        self.assertEqual(result, '"modelica://a_project/Loads/B123/input.idf"')
+        self.assertEqual(result_int, 0)
+        self.assertEqual(result_real, 1.25)
+        self.assertFalse(result_bool)
+
+    def test_model_update_param(self):
+        # Setup
+        source_file = os.path.join(self.data_dir, 'Office.mo')
+        model = Model(source_file)
+
+        # Act
+        model.update_parameter('String', 'idfName', '"54321"')
+        self.result = model.execute()
+
+        # Assert
+        self.assertHasAdditions(source_file, self.result, ['54321'])
+        self.assertHasDeletions(source_file, self.result, ['modelica://a_project/Loads/B123/input.idf'])
+
+    def test_model_redeclaration_string_replacement(self):
         """Should update redeclaration of a component"""
         # Setup
         source_file = os.path.join(self.data_dir, 'Office.mo')
         model = Model(source_file)
 
         # Act
 
@@ -326,15 +356,15 @@
             'Medium = Buildings.Media.Air',)
         self.result = model.execute()
 
         # Assert
         self.assertHasAdditions(source_file, self.result, ['redeclare package Medium = Buildings.Media.Air'])
         self.assertHasDeletions(source_file, self.result, ['Modelica.Media.Air.DryAirNasa'])
 
-    def test_model_reclaration_string_no_assign_replacement(self):
+    def test_model_redeclaration_string_no_assign_replacement(self):
         """Update a redeclare statement with a string. This is used when the
         redeclare clause doesn't have a assignment
         """
         source_file = os.path.join(self.data_dir, 'Office.mo')
         model = Model(source_file)
 
         # Act
@@ -902,7 +932,83 @@
             self.result,
             expected_body_additions
             + [
                 f'for {identifier} in {expression} loop',
                 'end for;'
             ])
         self.assertNoDeletions(source_file, self.result)
+
+    def test_model_get_argument_value(self):
+        mo_file = """
+model Test
+  AnInstanceOfObj Obj(
+    redeclare package Medium=Modelica.Media.Air.DryAirNasa,
+    Resist=100,
+    Desist=true,
+    redeclare IDEAS.Buildings.Components.Occupants.Fixed occNum(nOccFix=25.0)
+  );
+equation
+end Test;"""
+        source_file = self.create_tmp_file(mo_file)
+        model = Model(source_file)
+
+        value = model.get_component_argument_value(
+            'AnInstanceOfObj', 'Obj', 'Resist', type_cast=int
+        )
+        self.assertEqual(value, 100)
+
+        value = model.get_component_argument_value(
+            'AnInstanceOfObj', 'Obj', 'Resist'
+        )
+        self.assertEqual(value, '100')
+
+        value = model.get_component_argument_value(
+            'AnInstanceOfObj', 'Obj', 'Desist', type_cast=bool
+        )
+        self.assertEqual(value, True)
+
+    def test_model_get_argument_with_array(self):
+        # Setup
+        source_file = os.path.join(self.data_dir, 'district.mo')
+        model = Model(source_file)
+
+        value = model.get_component_argument_value(
+            'Buildings.Controls.OBC.CDL.Continuous.Sources.Constant', 'THotWatSupSet', 'k', type_cast=str
+        )
+        self.assertEqual(value, 'fill(63+273.15,nBui)')
+
+        # try setting the argument value
+        model.update_component_modifications(
+            'Buildings.Controls.OBC.CDL.Continuous.Sources.Constant', 'THotWatSupSet',
+            {'k': 'fill(65 + 273.15, nBui)'}
+        )
+        self.result = model.execute()
+
+        # Assert
+        self.assertHasAdditions(source_file, self.result, [
+            'fill(65 + 273.15, nBui)',
+        ])
+        self.assertHasDeletions(source_file, self.result, [
+            'fill(63 + 273.15, nBui)'
+        ])
+
+    def test_model_update_argument_with_extends_and_redeclare(self):
+        # Setup
+        source_file = os.path.join(self.data_dir, 'district.mo')
+        model = Model(source_file)
+
+        model.update_extended_component_modification(
+            'Buildings.Experimental.DHC.Examples.Combined.BaseClasses.PartialSeries',
+            'Buildings.Experimental.DHC.Loads.Combined.BuildingTimeSeriesWithETS', 'bui',
+            'datDes',
+            'epsPla', '1.0', if_value='0.935'
+        )
+        self.result = model.execute()
+        model.save_as(os.path.join(self.data_dir, 'district_updated2.mo'))
+
+        # Assert
+        self.assertHasAdditions(source_file, self.result, [
+            'epsPla=1.0',
+        ])
+        self.assertHasDeletions(source_file, self.result, [
+            'epsPla=0.935',
+        ])
```

### Comparing `modelica-builder-0.2.3rc1/tests/test_selector.py` & `modelica-builder-0.3.0/tests/test_selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ****************************************************************************************************
-:copyright (c) 2020-2022, Alliance for Sustainable Energy, LLC.
+:copyright (c) 2020-2023, Alliance for Sustainable Energy, LLC.
 All rights reserved.
 ****************************************************************************************************
 """
 
 
 # -*- coding: utf-8 -*-
```

### Comparing `modelica-builder-0.2.3rc1/tests/tests.py` & `modelica-builder-0.3.0/tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ****************************************************************************************************
-:copyright (c) 2020-2022, Alliance for Sustainable Energy, LLC.
+:copyright (c) 2020-2023, Alliance for Sustainable Energy, LLC.
 All rights reserved.
 ****************************************************************************************************
 """
 
 
 import difflib
```

