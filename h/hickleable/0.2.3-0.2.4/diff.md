# Comparing `tmp/hickleable-0.2.3.tar.gz` & `tmp/hickleable-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hickleable-0.2.3.tar", last modified: Wed Jul 12 06:03:59 2023, max compression
+gzip compressed data, was "hickleable-0.2.4.tar", last modified: Mon Aug  7 22:03:57 2023, max compression
```

## Comparing `hickleable-0.2.3.tar` & `hickleable-0.2.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 06:03:47.000000 hickleable-0.2.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-12 06:03:47.000000 hickleable-0.2.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.252550 hickleable-0.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/labels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.252550 hickleable-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/workflows/auto-merge-deps.yml
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/workflows/check-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/workflows/deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/workflows/release-draft.yml
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/workflows/testsuite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-12 06:03:47.000000 hickleable-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-12 06:03:47.000000 hickleable-0.2.3/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-12 06:03:47.000000 hickleable-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-12 06:03:47.000000 hickleable-0.2.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-12 06:03:47.000000 hickleable-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-12 06:03:59.260550 hickleable-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-12 06:03:47.000000 hickleable-0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/contents.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/docs/faqs/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/faqs/misc.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/docs/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-12 06:03:47.000000 hickleable-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-12 06:03:59.260550 hickleable-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 06:03:47.000000 hickleable-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.252550 hickleable-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/src/hickleable/
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-07-12 06:03:47.000000 hickleable-0.2.3/src/hickleable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/src/hickleable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-12 06:03:59.000000 hickleable-0.2.3/src/hickleable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-12 06:03:59.000000 hickleable-0.2.3/src/hickleable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 06:03:59.000000 hickleable-0.2.3/src/hickleable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 06:03:59.000000 hickleable-0.2.3/src/hickleable.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-12 06:03:59.000000 hickleable-0.2.3/src/hickleable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 06:03:59.000000 hickleable-0.2.3/src/hickleable.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-12 06:03:47.000000 hickleable-0.2.3/tests/test_hickleable.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-12 06:03:47.000000 hickleable-0.2.3/tests/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:03:57.627735 hickleable-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-07 22:03:46.000000 hickleable-0.2.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 22:03:46.000000 hickleable-0.2.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:03:57.623734 hickleable-0.2.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-07 22:03:46.000000 hickleable-0.2.4/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-07 22:03:46.000000 hickleable-0.2.4/.github/labels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-07 22:03:46.000000 hickleable-0.2.4/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:03:57.623734 hickleable-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-07 22:03:46.000000 hickleable-0.2.4/.github/workflows/auto-merge-deps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-07 22:03:46.000000 hickleable-0.2.4/.github/workflows/check-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-07 22:03:46.000000 hickleable-0.2.4/.github/workflows/deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-07 22:03:46.000000 hickleable-0.2.4/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-07 22:03:46.000000 hickleable-0.2.4/.github/workflows/release-draft.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-07 22:03:46.000000 hickleable-0.2.4/.github/workflows/testsuite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-07 22:03:46.000000 hickleable-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-07 22:03:46.000000 hickleable-0.2.4/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-07 22:03:46.000000 hickleable-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-07 22:03:46.000000 hickleable-0.2.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-07 22:03:46.000000 hickleable-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-08-07 22:03:57.627735 hickleable-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-08-07 22:03:46.000000 hickleable-0.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:03:57.627735 hickleable-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-08-07 22:03:46.000000 hickleable-0.2.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:03:57.627735 hickleable-0.2.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 22:03:46.000000 hickleable-0.2.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-07 22:03:46.000000 hickleable-0.2.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-08-07 22:03:46.000000 hickleable-0.2.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:03:46.000000 hickleable-0.2.4/docs/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-07 22:03:46.000000 hickleable-0.2.4/docs/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:03:57.627735 hickleable-0.2.4/docs/faqs/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-07 22:03:46.000000 hickleable-0.2.4/docs/faqs/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-07 22:03:46.000000 hickleable-0.2.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-07 22:03:46.000000 hickleable-0.2.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-07 22:03:46.000000 hickleable-0.2.4/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:03:57.627735 hickleable-0.2.4/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-07 22:03:46.000000 hickleable-0.2.4/docs/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:03:57.627735 hickleable-0.2.4/docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-07 22:03:46.000000 hickleable-0.2.4/docs/templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-07 22:03:46.000000 hickleable-0.2.4/docs/templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-07 22:03:46.000000 hickleable-0.2.4/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-07 22:03:46.000000 hickleable-0.2.4/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-07 22:03:46.000000 hickleable-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-07 22:03:57.627735 hickleable-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-07 22:03:46.000000 hickleable-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:03:57.619734 hickleable-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:03:57.627735 hickleable-0.2.4/src/hickleable/
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-08-07 22:03:46.000000 hickleable-0.2.4/src/hickleable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:03:57.627735 hickleable-0.2.4/src/hickleable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-08-07 22:03:57.000000 hickleable-0.2.4/src/hickleable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-07 22:03:57.000000 hickleable-0.2.4/src/hickleable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 22:03:57.000000 hickleable-0.2.4/src/hickleable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 22:03:57.000000 hickleable-0.2.4/src/hickleable.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-07 22:03:57.000000 hickleable-0.2.4/src/hickleable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 22:03:57.000000 hickleable-0.2.4/src/hickleable.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:03:57.627735 hickleable-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-08-07 22:03:46.000000 hickleable-0.2.4/tests/test_hickleable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-07 22:03:46.000000 hickleable-0.2.4/tests/test_yaml.py
```

### Comparing `hickleable-0.2.3/.github/labels.yml` & `hickleable-0.2.4/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.3/.github/release-drafter.yml` & `hickleable-0.2.4/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.3/.github/workflows/check-build.yml` & `hickleable-0.2.4/.github/workflows/check-build.yml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.3/.github/workflows/deploy.yaml` & `hickleable-0.2.4/.github/workflows/deploy.yaml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.3/.github/workflows/testsuite.yaml` & `hickleable-0.2.4/.github/workflows/testsuite.yaml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.3/.gitignore` & `hickleable-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.3/.pre-commit-config.yaml` & `hickleable-0.2.4/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   - id: debug-statements
   - id: end-of-file-fixer
   - id: requirements-txt-fixer
   - id: mixed-line-ending
     args: ['--fix=no']
 
 - repo: https://github.com/PyCQA/flake8
-  rev: 6.0.0
+  rev: 6.1.0
   hooks:
   - id: flake8
     additional_dependencies:
       - flake8-comprehensions
       - flake8-logging-format
       - flake8-builtins
       - flake8-eradicate
@@ -35,26 +35,26 @@
       - flake8-markdown
       - flake8-bugbear
       - flake8-comprehensions
       - flake8-print
 
 
 - repo: https://github.com/psf/black
-  rev: 23.3.0
+  rev: 23.7.0
   hooks:
   - id: black
 
 - repo: https://github.com/PyCQA/isort
   rev: 5.12.0
   hooks:
   - id: isort
 
 - repo: https://github.com/pre-commit/pygrep-hooks
   rev: v1.10.0
   hooks:
     - id: rst-backticks
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.9.0
+  rev: v3.10.1
   hooks:
   -   id: pyupgrade
       args: [--py38-plus]
```

### Comparing `hickleable-0.2.3/.readthedocs.yml` & `hickleable-0.2.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.3/LICENSE` & `hickleable-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.3/PKG-INFO` & `hickleable-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hickleable
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple decorator to make your classes hickle-able
 Home-page: https://github.com/steven-murray/hickleable
 Author: Steven Murray
 License: mit
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `hickleable-0.2.3/README.rst` & `hickleable-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.3/docs/Makefile` & `hickleable-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.3/docs/conf.py` & `hickleable-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.3/docs/index.rst` & `hickleable-0.2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.3/docs/templates/class.rst` & `hickleable-0.2.4/docs/templates/class.rst`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.3/docs/templates/module.rst` & `hickleable-0.2.4/docs/templates/module.rst`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.3/setup.cfg` & `hickleable-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.3/src/hickleable/__init__.py` & `hickleable-0.2.4/src/hickleable/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,17 @@
         py_obj_type
             Custom class (or subclass)
         """
         # the optional protected _content parameter of the PyContainer
         # __init__ method can be used to change the data structure used to
         # store the subitems passed to the append method of the PyContainer
         # class per default it is set to []
-        super().__init__(h5_attrs, base_type, object_type, _content=dict(h5_attrs))
+        _content = {k: v for k, v in h5_attrs.items() if k != "type"}
+
+        super().__init__(h5_attrs, base_type, object_type, _content=_content)
 
     def append(self, name: str, item: Any, h5_attrs: AttributeManager):
         """Add a particular item to the content defining the object.
 
         Parameters
         ----------
         name
```

### Comparing `hickleable-0.2.3/src/hickleable.egg-info/PKG-INFO` & `hickleable-0.2.4/src/hickleable.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hickleable
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple decorator to make your classes hickle-able
 Home-page: https://github.com/steven-murray/hickleable
 Author: Steven Murray
 License: mit
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `hickleable-0.2.3/src/hickleable.egg-info/SOURCES.txt` & `hickleable-0.2.4/src/hickleable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.3/tests/test_hickleable.py` & `hickleable-0.2.4/tests/test_hickleable.py`

 * *Files 4% similar despite different names*

```diff
@@ -201,7 +201,28 @@
 
 
 def test_bad_gethstate(tmpdir):
     a = ClassWithBadGetHState()
 
     with pytest.raises(TypeError, match="__gethstate__ must return a dictionary"):
         hickle.dump(a, tmpdir / "test.h5")
+
+
+@hickleable()
+class Nester:
+    def __init__(self, a):
+        self.a = a
+
+    def __gethstate__(self):
+        return self.__dict__
+
+    def __sethstate__(self, hstate):
+        self.__dict__.update(hstate)
+
+
+def test_nested_with_sethstate(tmpdir):
+    nested = Nester(Nester(3))
+
+    hickle.dump(nested, tmpdir / "test.h5")
+    new_nested = hickle.load(tmpdir / "test.h5")
+
+    assert new_nested.a.a == 3
```

