# Comparing `tmp/adbpyg_adapter-1.1.0.tar.gz` & `tmp/adbpyg_adapter-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbpyg_adapter-1.1.0.tar", last modified: Wed Sep 21 18:13:42 2022, max compression
+gzip compressed data, was "adbpyg_adapter-1.1.1.tar", last modified: Tue Aug  8 14:38:39 2023, max compression
```

## Comparing `adbpyg_adapter-1.1.0.tar` & `adbpyg_adapter-1.1.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 maxk      (1001) maxk      (1001)        0 2022-09-21 18:13:42.568958 adbpyg_adapter-1.1.0/
--rw-r--r--   0 maxk      (1001) maxk      (1001)       45 2022-08-01 16:36:03.000000 adbpyg_adapter-1.1.0/.gitattributes
--rw-r--r--   0 maxk      (1001) maxk      (1001)    10058 2022-08-01 16:36:03.000000 adbpyg_adapter-1.1.0/.gitchangelog.rc
-drwxr-xr-x   0 maxk      (1001) maxk      (1001)        0 2022-09-21 18:13:42.568958 adbpyg_adapter-1.1.0/.github/
-drwxr-xr-x   0 maxk      (1001) maxk      (1001)        0 2022-09-21 18:13:42.568958 adbpyg_adapter-1.1.0/.github/workflows/
--rw-r--r--   0 maxk      (1001) maxk      (1001)     2452 2022-08-01 16:36:03.000000 adbpyg_adapter-1.1.0/.github/workflows/analyze.yml
--rw-r--r--   0 maxk      (1001) maxk      (1001)     1797 2022-08-01 16:48:14.000000 adbpyg_adapter-1.1.0/.github/workflows/build.yml
--rw-r--r--   0 maxk      (1001) maxk      (1001)     4578 2022-09-21 18:11:29.000000 adbpyg_adapter-1.1.0/.github/workflows/release.yml
--rw-r--r--   0 maxk      (1001) maxk      (1001)     1350 2022-08-01 16:36:03.000000 adbpyg_adapter-1.1.0/.gitignore
--rw-r--r--   0 maxk      (1001) maxk      (1001)      536 2022-08-01 16:36:03.000000 adbpyg_adapter-1.1.0/CHANGELOG.md
--rw-r--r--   0 maxk      (1001) maxk      (1001)    10273 2022-08-01 16:36:03.000000 adbpyg_adapter-1.1.0/LICENSE
--rw-r--r--   0 maxk      (1001) maxk      (1001)       52 2022-08-01 16:36:03.000000 adbpyg_adapter-1.1.0/MANIFEST.in
--rw-r--r--   0 maxk      (1001) maxk      (1001)    13324 2022-09-21 18:13:42.568958 adbpyg_adapter-1.1.0/PKG-INFO
--rw-r--r--   0 maxk      (1001) maxk      (1001)    12462 2022-08-05 20:33:56.000000 adbpyg_adapter-1.1.0/README.md
-drwxr-xr-x   0 maxk      (1001) maxk      (1001)        0 2022-09-21 18:13:42.568958 adbpyg_adapter-1.1.0/adbpyg_adapter/
--rw-r--r--   0 maxk      (1001) maxk      (1001)      134 2022-08-01 16:36:03.000000 adbpyg_adapter-1.1.0/adbpyg_adapter/__init__.py
--rw-r--r--   0 maxk      (1001) maxk      (1001)     2330 2022-08-01 17:34:42.000000 adbpyg_adapter-1.1.0/adbpyg_adapter/abc.py
--rw-r--r--   0 maxk      (1001) maxk      (1001)    37320 2022-08-05 14:03:07.000000 adbpyg_adapter-1.1.0/adbpyg_adapter/adapter.py
--rw-r--r--   0 maxk      (1001) maxk      (1001)     2126 2022-08-02 03:37:32.000000 adbpyg_adapter-1.1.0/adbpyg_adapter/controller.py
--rw-r--r--   0 maxk      (1001) maxk      (1001)     1112 2022-08-03 04:29:30.000000 adbpyg_adapter-1.1.0/adbpyg_adapter/encoders.py
--rw-r--r--   0 maxk      (1001) maxk      (1001)      471 2022-08-01 16:36:03.000000 adbpyg_adapter-1.1.0/adbpyg_adapter/exceptions.py
--rw-r--r--   0 maxk      (1001) maxk      (1001)      863 2022-08-04 02:09:07.000000 adbpyg_adapter-1.1.0/adbpyg_adapter/typings.py
--rw-r--r--   0 maxk      (1001) maxk      (1001)     6230 2022-08-05 01:44:55.000000 adbpyg_adapter-1.1.0/adbpyg_adapter/utils.py
--rw-r--r--   0 maxk      (1001) maxk      (1001)      142 2022-09-21 18:13:42.000000 adbpyg_adapter-1.1.0/adbpyg_adapter/version.py
-drwxr-xr-x   0 maxk      (1001) maxk      (1001)        0 2022-09-21 18:13:42.568958 adbpyg_adapter-1.1.0/adbpyg_adapter.egg-info/
--rw-r--r--   0 maxk      (1001) maxk      (1001)    13324 2022-09-21 18:13:42.000000 adbpyg_adapter-1.1.0/adbpyg_adapter.egg-info/PKG-INFO
--rw-r--r--   0 maxk      (1001) maxk      (1001)      632 2022-09-21 18:13:42.000000 adbpyg_adapter-1.1.0/adbpyg_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 maxk      (1001) maxk      (1001)        1 2022-09-21 18:13:42.000000 adbpyg_adapter-1.1.0/adbpyg_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 maxk      (1001) maxk      (1001)      333 2022-09-21 18:13:42.000000 adbpyg_adapter-1.1.0/adbpyg_adapter.egg-info/requires.txt
--rw-r--r--   0 maxk      (1001) maxk      (1001)       15 2022-09-21 18:13:42.000000 adbpyg_adapter-1.1.0/adbpyg_adapter.egg-info/top_level.txt
--rw-r--r--   0 maxk      (1001) maxk      (1001)      353 2022-08-01 16:36:03.000000 adbpyg_adapter-1.1.0/pyproject.toml
--rw-r--r--   0 maxk      (1001) maxk      (1001)      250 2022-09-21 18:13:42.568958 adbpyg_adapter-1.1.0/setup.cfg
--rw-r--r--   0 maxk      (1001) maxk      (1001)     1731 2022-08-01 16:36:03.000000 adbpyg_adapter-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:38:39.879435 adbpyg_adapter-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/.gitchangelog.rc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:38:39.879435 adbpyg_adapter-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:38:39.879435 adbpyg_adapter-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/.github/workflows/analyze.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/.github/workflows/build_self_hosted.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15984 2023-08-08 14:38:39.879435 adbpyg_adapter-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12860 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:38:39.879435 adbpyg_adapter-1.1.1/adbpyg_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/adbpyg_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/adbpyg_adapter/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44250 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/adbpyg_adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/adbpyg_adapter/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/adbpyg_adapter/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/adbpyg_adapter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/adbpyg_adapter/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/adbpyg_adapter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-08 14:38:39.000000 adbpyg_adapter-1.1.1/adbpyg_adapter/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:38:39.879435 adbpyg_adapter-1.1.1/adbpyg_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15984 2023-08-08 14:38:39.000000 adbpyg_adapter-1.1.1/adbpyg_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-08 14:38:39.000000 adbpyg_adapter-1.1.1/adbpyg_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:38:39.000000 adbpyg_adapter-1.1.1/adbpyg_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-08 14:38:39.000000 adbpyg_adapter-1.1.1/adbpyg_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-08 14:38:39.000000 adbpyg_adapter-1.1.1/adbpyg_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-08 14:38:39.883435 adbpyg_adapter-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-08 14:36:20.000000 adbpyg_adapter-1.1.1/setup.py
```

### Comparing `adbpyg_adapter-1.1.0/.gitchangelog.rc` & `adbpyg_adapter-1.1.1/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `adbpyg_adapter-1.1.0/.github/workflows/analyze.yml` & `adbpyg_adapter-1.1.1/.github/workflows/analyze.yml`

 * *Files identical despite different names*

### Comparing `adbpyg_adapter-1.1.0/.github/workflows/build.yml` & `adbpyg_adapter-1.1.1/.github/workflows/build_self_hosted.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-name: build
+name: build_self_hosted
 on:
   workflow_dispatch:
-  push:
-    branches: [ master ]
-  pull_request:
-    branches: [ master ]
 env:
   PACKAGE_DIR: adbpyg_adapter
   TESTS_DIR: tests
 jobs:
   build:
     runs-on: self-hosted
     defaults:
```

### Comparing `adbpyg_adapter-1.1.0/.github/workflows/release.yml` & `adbpyg_adapter-1.1.1/.github/workflows/release.yml`

 * *Files 25% similar despite different names*

```diff
@@ -4,117 +4,112 @@
   release:
     types: [published]
 env:
   PACKAGE_DIR: adbpyg_adapter
   TESTS_DIR: tests
 jobs:
   build:
-    runs-on: self-hosted
-    defaults:
-      run:
-        shell: bash -l {0}
+    runs-on: ubuntu-latest
     strategy:
       matrix:
-        include:
-          - python: "3.7"
-            DB_NAME: "py37"
-
-          - python: "3.8"
-            DB_NAME: "py38"
-
-          - python: "3.9"
-            DB_NAME: "py39"
-
-          - python: "3.10"
-            DB_NAME: "py310"
+        python: ["3.8", "3.9", "3.10", "3.11"]
     name: Python ${{ matrix.python }}
     steps:
-      - uses: actions/checkout@v2
-      - name: Set up pip & install packages
-        run: |
-          source ~/anaconda3/etc/profile.d/conda.sh
-          conda activate ${{ matrix.python }}
-          python -m pip install --upgrade pip setuptools wheel
-          pip install torch
-          pip install .[dev]
+      - uses: actions/checkout@v3
+      - name: Setup Python ${{ matrix.python }}
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python }}
+          cache: 'pip'
+          cache-dependency-path: setup.py
+      - name: Install packages
+        run: pip install torch && pip install -e .[dev]
       - name: Run black
-        run: conda run -n ${{ matrix.python }} black --check --verbose --diff --color ${{env.PACKAGE_DIR}} ${{env.TESTS_DIR}}
+        run: black --check --verbose --diff --color ${{env.PACKAGE_DIR}} ${{env.TESTS_DIR}}
       - name: Run flake8
         run: flake8 ${{env.PACKAGE_DIR}} ${{env.TESTS_DIR}}
       - name: Run isort
         run: isort --check --profile=black ${{env.PACKAGE_DIR}} ${{env.TESTS_DIR}}
       - name: Run mypy
-        run: conda run -n ${{ matrix.python }} mypy ${{env.PACKAGE_DIR}} ${{env.TESTS_DIR}}
-      - name: Run pytest in conda env
-        run: conda run -n ${{ matrix.python }} pytest --dbName ${{ matrix.DB_NAME }} --cov=${{env.PACKAGE_DIR}} --cov-report xml --cov-report term-missing -v --color=yes --no-cov-on-fail --code-highlight=yes
+        run: mypy ${{env.PACKAGE_DIR}} ${{env.TESTS_DIR}}
+      - name: Set up ArangoDB Instance via Docker
+        run: docker create --name adb -p 8529:8529 -e ARANGO_ROOT_PASSWORD= arangodb/arangodb
+      - name: Start ArangoDB Instance
+        run: docker start adb
+      - name: Run pytest
+        run: pytest --cov=${{env.PACKAGE_DIR}} --cov-report xml --cov-report term-missing -v --color=yes --no-cov-on-fail --code-highlight=yes
       - name: Publish to coveralls.io
         if: matrix.python == '3.8'
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-        run: conda run -n ${{ matrix.python }} coveralls --service=github
+        run: coveralls --service=github
 
   release:
     needs: build
-    runs-on: self-hosted
-    defaults:
-      run:
-        shell: bash -l {0}
+    runs-on: ubuntu-latest
     name: Release package
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
+      - name: Setup Python 3.8
+        uses: actions/setup-python@v4
+        with:
+          python-version: "3.8"
+          cache: 'pip'
+          cache-dependency-path: setup.py
 
       - name: Fetch complete history for all tags and branches
         run: git fetch --prune --unshallow
 
       - name: Install packages
         run: |
-          source ~/anaconda3/etc/profile.d/conda.sh
-          conda activate 3.8
           pip install setuptools wheel twine setuptools-scm[toml]
           pip install torch
           pip install .[dev]
 
       - name: Remove (old) distribution
         run: rm -rf dist
 
       - name: Build distribution
-        run: conda run -n 3.8 python setup.py sdist bdist_wheel
+        run: python setup.py sdist bdist_wheel
 
       - name: Publish to Test PyPi
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.TWINE_PASSWORD_TEST }}
-        run: conda run -n 3.8 twine upload --repository testpypi dist/* #--skip-existing
+        run: twine upload --repository testpypi dist/* #--skip-existing
+
       - name: Publish to PyPi
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.TWINE_PASSWORD }}
-        run: conda run -n "3.8" twine upload --repository pypi dist/* #--skip-existing
+        run: twine upload --repository pypi dist/* #--skip-existing
 
   changelog:
     needs: release
     runs-on: ubuntu-latest
     name: Update Changelog
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Create new branch
         run: git checkout -b actions/changelog
 
       - name: Set branch upstream
         run: git push -u origin actions/changelog
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
-      - name: Setup python
-        uses: actions/setup-python@v2
+      - name: Setup Python 3.8
+        uses: actions/setup-python@v4
         with:
           python-version: "3.8"
+          cache: 'pip'
+          cache-dependency-path: setup.py
 
       - name: Install release packages
         run: pip install wheel gitchangelog pystache
 
       - name: Set variables
         run: echo "VERSION=$(curl ${GITHUB_API_URL}/repos/${GITHUB_REPOSITORY}/releases/latest | python -c "import sys; import json; print(json.load(sys.stdin)['tag_name'])")" >> $GITHUB_ENV
```

### Comparing `adbpyg_adapter-1.1.0/.gitignore` & `adbpyg_adapter-1.1.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 celerybeat-schedule
 
 # SageMath parsed files
 *.sage.py
 
 # Environments
 .env
-.venv
+.venv*
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
 
 # Spyder project settings
```

### Comparing `adbpyg_adapter-1.1.0/LICENSE` & `adbpyg_adapter-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adbpyg_adapter-1.1.0/PKG-INFO` & `adbpyg_adapter-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,20 @@
-Metadata-Version: 2.1
-Name: adbpyg_adapter
-Version: 1.1.0
-Summary: Convert ArangoDB graphs to PyG & vice-versa.
-Home-page: https://github.com/arangoml/pyg-adapter
-Author: Anthony Mahanna
-Author-email: anthony.mahanna@arangodb.com
-License: Apache Software License
-Keywords: arangodb,pyg,adapter
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # ArangoDB-PyG Adapter
 
 [![build](https://github.com/arangoml/pyg-adapter/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/arangoml/pyg-adapter/actions/workflows/build.yml)
 [![CodeQL](https://github.com/arangoml/pyg-adapter/actions/workflows/analyze.yml/badge.svg?branch=master)](https://github.com/arangoml/pyg-adapter/actions/workflows/analyze.yml)
 [![Coverage Status](https://coveralls.io/repos/github/arangoml/pyg-adapter/badge.svg?branch=master)](https://coveralls.io/github/arangoml/pyg-adapter)
 [![Last commit](https://img.shields.io/github/last-commit/arangoml/pyg-adapter)](https://github.com/arangoml/pyg-adapter/commits/master)
 
 [![PyPI version badge](https://img.shields.io/pypi/v/adbpyg-adapter?color=3775A9&style=for-the-badge&logo=pypi&logoColor=FFD43B)](https://pypi.org/project/adbpyg-adapter/)
 [![Python versions badge](https://img.shields.io/pypi/pyversions/adbpyg-adapter?color=3776AB&style=for-the-badge&logo=python&logoColor=FFD43B)](https://pypi.org/project/adbpyg-adapter/)
 
 [![License](https://img.shields.io/github/license/arangoml/pyg-adapter?color=9E2165&style=for-the-badge)](https://github.com/arangoml/pyg-adapter/blob/master/LICENSE)
 [![Code style: black](https://img.shields.io/static/v1?style=for-the-badge&label=code%20style&message=black&color=black)](https://github.com/psf/black)
-[![Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&color=282661&label=Downloads&query=total_downloads&url=https://api.pepy.tech/api/projects/adbpyg-adapter)](https://pepy.tech/project/adbpyg-adapter)
+[![Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&color=282661&label=Downloads&query=total_downloads&url=https://api.pepy.tech/api/v2/projects/adbpyg-adapter)](https://pepy.tech/project/adbpyg-adapter)
 
 
 <a href="https://www.arangodb.com/" rel="arangodb.com">![](https://raw.githubusercontent.com/arangoml/pyg-adapter/master/examples/assets/adb_logo.png)</a>
 <a href="https://www.pyg.org/" rel="pyg.org"><img src="https://raw.githubusercontent.com/pyg-team/pyg_sphinx_theme/master/pyg_sphinx_theme/static/img/pyg_logo_text.svg?sanitize=true" width=40% /></a>
 
 The ArangoDB-PyG Adapter exports Graphs from ArangoDB, the multi-model database for graph & beyond, into PyTorch Geometric (PyG), a PyTorch-based Graph Neural Network library, and vice-versa.
 
@@ -62,14 +38,16 @@
 pip install git+https://github.com/arangoml/pyg-adapter.git
 ```
 
 ##  Quickstart
 
 [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/arangoml/pyg-adapter/blob/master/examples/ArangoDB_PyG_Adapter.ipynb)
 
+Also available as an ArangoDB Lunch & Learn session on YouTube: [Graph & Beyond Course: ArangoDB-PyG Adapter](https://www.youtube.com/watch?v=QtGR95NN8bA)
+
 ```py
 import torch
 import pandas
 from torch_geometric.datasets import FakeHeteroDataset
 
 from arango import ArangoClient  # Python-Arango driver
 
@@ -97,28 +75,33 @@
 Note: If the PyG graph contains `_key`, `_v_key`, or `_e_key` properties for any node / edge types, the adapter will assume to persist those values as [ArangoDB document keys](https://www.arangodb.com/docs/stable/data-modeling-naming-conventions-document-keys.html). See the `Full Cycle (ArangoDB -> PyG -> ArangoDB)` section below for an example.
 
 ```py
 # 1.1: PyG to ArangoDB
 adb_g = adbpyg_adapter.pyg_to_arangodb("FakeData", data)
 
 # 1.2: PyG to ArangoDB with a (completely optional) metagraph for customized adapter behaviour
-def y_tensor_to_2_column_dataframe(pyg_tensor):
+def y_tensor_to_2_column_dataframe(pyg_tensor, adb_df):
     """
     A user-defined function to create two
-    ArangoDB attributes out of the 'y' label tensor
+    ArangoDB attributes out of the 'user' label tensor
+
+    :param dgl_tensor: The DGL Tensor containing the data
+    :type dgl_tensor: torch.Tensor
+    :param adb_df: The ArangoDB DataFrame to populate, whose
+        size is preset to the length of **dgl_tensor**.
+    :type adb_df: pandas.DataFrame
 
-    NOTE: user-defined functions must return a Pandas Dataframe
+    NOTE: user-defined functions must return the modified **adb_df**
     """
     label_map = {0: "Kiwi", 1: "Blueberry", 2: "Avocado"}
 
-    df = pandas.DataFrame(columns=["label_num", "label_str"])
-    df["label_num"] = pyg_tensor.tolist()
-    df["label_str"] = df["label_num"].map(label_map)
+    adb_df["label_num"] = pyg_tensor.tolist()
+    adb_df["label_str"] = adb_df["label_num"].map(label_map)
 
-    return df
+    return adb_df
 
 
 metagraph = {
     "nodeTypes": {
         "v0": {
             "x": "features",  # 1) You can specify a string value if you want to rename your PyG data when stored in ArangoDB
             "y": y_tensor_to_2_column_dataframe,  # 2) you can specify a function for user-defined handling, as long as the function returns a Pandas DataFrame
@@ -270,17 +253,18 @@
 ##  Development & Testing
 
 Prerequisite: `arangorestore`
 
 1. `git clone https://github.com/arangoml/pyg-adapter.git`
 2. `cd pyg-adapter`
 3. (create virtual environment of choice)
-4. `pip install -e .[dev]`
-5. (create an ArangoDB instance with method of choice)
-6. `pytest --url <> --dbName <> --username <> --password <>`
+4. `pip install torch`
+5. `pip install -e .[dev]`
+6. (create an ArangoDB instance with method of choice)
+7. `pytest --url <> --dbName <> --username <> --password <>`
 
 **Note**: A `pytest` parameter can be omitted if the endpoint is using its default value:
 ```python
 def pytest_addoption(parser):
     parser.addoption("--url", action="store", default="http://localhost:8529")
     parser.addoption("--dbName", action="store", default="_system")
     parser.addoption("--username", action="store", default="root")
```

### Comparing `adbpyg_adapter-1.1.0/README.md` & `adbpyg_adapter-1.1.1/adbpyg_adapter.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,264 +1,297 @@
-# ArangoDB-PyG Adapter
-
-[![build](https://github.com/arangoml/pyg-adapter/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/arangoml/pyg-adapter/actions/workflows/build.yml)
-[![CodeQL](https://github.com/arangoml/pyg-adapter/actions/workflows/analyze.yml/badge.svg?branch=master)](https://github.com/arangoml/pyg-adapter/actions/workflows/analyze.yml)
-[![Coverage Status](https://coveralls.io/repos/github/arangoml/pyg-adapter/badge.svg?branch=master)](https://coveralls.io/github/arangoml/pyg-adapter)
-[![Last commit](https://img.shields.io/github/last-commit/arangoml/pyg-adapter)](https://github.com/arangoml/pyg-adapter/commits/master)
-
-[![PyPI version badge](https://img.shields.io/pypi/v/adbpyg-adapter?color=3775A9&style=for-the-badge&logo=pypi&logoColor=FFD43B)](https://pypi.org/project/adbpyg-adapter/)
-[![Python versions badge](https://img.shields.io/pypi/pyversions/adbpyg-adapter?color=3776AB&style=for-the-badge&logo=python&logoColor=FFD43B)](https://pypi.org/project/adbpyg-adapter/)
-
-[![License](https://img.shields.io/github/license/arangoml/pyg-adapter?color=9E2165&style=for-the-badge)](https://github.com/arangoml/pyg-adapter/blob/master/LICENSE)
-[![Code style: black](https://img.shields.io/static/v1?style=for-the-badge&label=code%20style&message=black&color=black)](https://github.com/psf/black)
-[![Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&color=282661&label=Downloads&query=total_downloads&url=https://api.pepy.tech/api/projects/adbpyg-adapter)](https://pepy.tech/project/adbpyg-adapter)
-
-
-<a href="https://www.arangodb.com/" rel="arangodb.com">![](https://raw.githubusercontent.com/arangoml/pyg-adapter/master/examples/assets/adb_logo.png)</a>
-<a href="https://www.pyg.org/" rel="pyg.org"><img src="https://raw.githubusercontent.com/pyg-team/pyg_sphinx_theme/master/pyg_sphinx_theme/static/img/pyg_logo_text.svg?sanitize=true" width=40% /></a>
-
-The ArangoDB-PyG Adapter exports Graphs from ArangoDB, the multi-model database for graph & beyond, into PyTorch Geometric (PyG), a PyTorch-based Graph Neural Network library, and vice-versa.
-
-## About PyG
-
-**PyG** *(PyTorch Geometric)* is a library built upon [PyTorch](https://pytorch.org/) to easily write and train Graph Neural Networks (GNNs) for a wide range of applications related to structured data.
-
-It consists of various methods for deep learning on graphs and other irregular structures, also known as *[geometric deep learning](http://geometricdeeplearning.com/)*, from a variety of published papers.
-In addition, it consists of easy-to-use mini-batch loaders for operating on many small and single giant graphs, [multi GPU-support](https://github.com/pyg-team/pytorch_geometric/tree/master/examples/multi_gpu), [`DataPipe` support](https://github.com/pyg-team/pytorch_geometric/blob/master/examples/datapipe.py), distributed graph learning via [Quiver](https://github.com/pyg-team/pytorch_geometric/tree/master/examples/quiver), a large number of common benchmark datasets (based on simple interfaces to create your own), the [GraphGym](https://pytorch-geometric.readthedocs.io/en/latest/notes/graphgym.html) experiment manager, and helpful transforms, both for learning on arbitrary graphs as well as on 3D meshes or point clouds.
-
-## Installation
-
-#### Latest Release
-```
-pip install torch
-pip install adbpyg-adapter
-```
-#### Current State
-```
-pip install torch
-pip install git+https://github.com/arangoml/pyg-adapter.git
-```
-
-##  Quickstart
-
-[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/arangoml/pyg-adapter/blob/master/examples/ArangoDB_PyG_Adapter.ipynb)
-
-```py
-import torch
-import pandas
-from torch_geometric.datasets import FakeHeteroDataset
-
-from arango import ArangoClient  # Python-Arango driver
-
-from adbpyg_adapter import ADBPyG_Adapter, ADBPyG_Controller
-from adbpyg_adapter.encoders import IdentityEncoder, CategoricalEncoder
-
-# Load some fake PyG data for demo purposes
-data = FakeHeteroDataset(
-    num_node_types=2,
-    num_edge_types=3,
-    avg_num_nodes=20,
-    avg_num_channels=3,  # avg number of features per node
-    edge_dim=2,  # number of features per edge
-    num_classes=3,  # number of unique label values
-)[0]
-
-# Let's assume that the ArangoDB "IMDB" dataset is imported to this endpoint
-db = ArangoClient(hosts="http://localhost:8529").db("_system", username="root", password="")
-
-adbpyg_adapter = ADBPyG_Adapter(db)
-```
-
-### PyG to ArangoDB
-
-Note: If the PyG graph contains `_key`, `_v_key`, or `_e_key` properties for any node / edge types, the adapter will assume to persist those values as [ArangoDB document keys](https://www.arangodb.com/docs/stable/data-modeling-naming-conventions-document-keys.html). See the `Full Cycle (ArangoDB -> PyG -> ArangoDB)` section below for an example.
-
-```py
-# 1.1: PyG to ArangoDB
-adb_g = adbpyg_adapter.pyg_to_arangodb("FakeData", data)
-
-# 1.2: PyG to ArangoDB with a (completely optional) metagraph for customized adapter behaviour
-def y_tensor_to_2_column_dataframe(pyg_tensor):
-    """
-    A user-defined function to create two
-    ArangoDB attributes out of the 'y' label tensor
-
-    NOTE: user-defined functions must return a Pandas Dataframe
-    """
-    label_map = {0: "Kiwi", 1: "Blueberry", 2: "Avocado"}
-
-    df = pandas.DataFrame(columns=["label_num", "label_str"])
-    df["label_num"] = pyg_tensor.tolist()
-    df["label_str"] = df["label_num"].map(label_map)
-
-    return df
-
-
-metagraph = {
-    "nodeTypes": {
-        "v0": {
-            "x": "features",  # 1) You can specify a string value if you want to rename your PyG data when stored in ArangoDB
-            "y": y_tensor_to_2_column_dataframe,  # 2) you can specify a function for user-defined handling, as long as the function returns a Pandas DataFrame
-        },
-        # 3) You can specify set of strings if you want to preserve the same PyG attribute names for the node/edge type
-        "v1": {"x"} # this is equivalent to {"x": "x"}
-    },
-    "edgeTypes": {
-        ("v0", "e0", "v0"): {
-            # 4) You can specify a list of strings for tensor dissasembly (if you know the number of node/edge features in advance)
-            "edge_attr": [ "a", "b"]  
-        },
-    },
-}
-
-
-adb_g = adbpyg_adapter.pyg_to_arangodb("FakeData", data, metagraph, explicit_metagraph=False)
-
-# 1.3: PyG to ArangoDB with the same (optional) metagraph, but with `explicit_metagraph=True`
-# With `explicit_metagraph=True`, the node & edge types omitted from the metagraph will NOT be converted to ArangoDB.
-# Only 'v0', 'v1' and ('v0', 'e0', 'v0') will be brought over (i.e 'v2', ('v0', 'e0', 'v1'), ... are ignored)
-adb_g = adbpyg_adapter.pyg_to_arangodb("FakeData", data, metagraph, explicit_metagraph=True)
-
-# 1.4: PyG to ArangoDB with a Custom Controller  (more user-defined behavior)
-class Custom_ADBPyG_Controller(ADBPyG_Controller):
-    def _prepare_pyg_node(self, pyg_node: dict, node_type: str) -> dict:
-        """Optionally modify a PyG node object before it gets inserted into its designated ArangoDB collection.
-
-        :param pyg_node: The PyG node object to (optionally) modify.
-        :param node_type: The PyG Node Type of the node.
-        :return: The PyG Node object
-        """
-        pyg_node["foo"] = "bar"
-        return pyg_node
-
-    def _prepare_pyg_edge(self, pyg_edge: dict, edge_type: tuple) -> dict:
-        """Optionally modify a PyG edge object before it gets inserted into its designated ArangoDB collection.
-
-        :param pyg_edge: The PyG edge object to (optionally) modify.
-        :param edge_type: The Edge Type of the PyG edge. Formatted
-            as (from_collection, edge_collection, to_collection)
-        :return: The PyG Edge object
-        """
-        pyg_edge["bar"] = "foo"
-        return pyg_edge
-
-
-adb_g = ADBPyG_Adapter(db, Custom_ADBPyG_Controller()).pyg_to_arangodb("FakeData", data)
-```
-
-### ArangoDB to PyG
-```py
-# Start from scratch!
-db.delete_graph("FakeData", drop_collections=True, ignore_missing=True)
-adbpyg_adapter.pyg_to_arangodb("FakeData", data)
-
-# 2.1: ArangoDB to PyG via Graph name (does not transfer attributes)
-pyg_g = adbpyg_adapter.arangodb_graph_to_pyg("FakeData")
-
-# 2.2: ArangoDB to PyG via Collection names (does not transfer attributes)
-pyg_g = adbpyg_adapter.arangodb_collections_to_pyg("FakeData", v_cols={"v0", "v1"}, e_cols={"e0"})
-
-# 2.3: ArangoDB to PyG via Metagraph v1 (transfer attributes "as is", meaning they are already formatted to PyG data standards)
-metagraph_v1 = {
-    "vertexCollections": {
-        # Move the "x" & "y" ArangoDB attributes to PyG as "x" & "y" Tensors
-        "v0": {"x", "y"}, # equivalent to {"x": "x", "y": "y"}
-        "v1": {"v1_x": "x"}, # store the 'x' feature matrix as 'v1_x' in PyG
-    },
-    "edgeCollections": {
-        "e0": {"edge_attr"},
-    },
-}
-pyg_g = adbpyg_adapter.arangodb_to_pyg("FakeData", metagraph_v1)
-
-# 2.4: ArangoDB to PyG via Metagraph v2 (transfer attributes via user-defined encoders)
-# For more info on user-defined encoders in PyG, see https://pytorch-geometric.readthedocs.io/en/latest/notes/load_csv.html
-metagraph_v2 = {
-    "vertexCollections": {
-        "Movies": {
-            "x": {  # Build a feature matrix from the "Action" & "Drama" document attributes
-                "Action": IdentityEncoder(dtype=torch.long),
-                "Drama": IdentityEncoder(dtype=torch.long),
+Metadata-Version: 2.1
+Name: adbpyg-adapter
+Version: 1.1.1
+Summary: Convert ArangoDB graphs to PyG & vice-versa.
+Home-page: https://github.com/arangoml/pyg-adapter
+Author: Anthony Mahanna
+Author-email: anthony.mahanna@arangodb.com
+License: Apache Software License
+Description: # ArangoDB-PyG Adapter
+        
+        [![build](https://github.com/arangoml/pyg-adapter/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/arangoml/pyg-adapter/actions/workflows/build.yml)
+        [![CodeQL](https://github.com/arangoml/pyg-adapter/actions/workflows/analyze.yml/badge.svg?branch=master)](https://github.com/arangoml/pyg-adapter/actions/workflows/analyze.yml)
+        [![Coverage Status](https://coveralls.io/repos/github/arangoml/pyg-adapter/badge.svg?branch=master)](https://coveralls.io/github/arangoml/pyg-adapter)
+        [![Last commit](https://img.shields.io/github/last-commit/arangoml/pyg-adapter)](https://github.com/arangoml/pyg-adapter/commits/master)
+        
+        [![PyPI version badge](https://img.shields.io/pypi/v/adbpyg-adapter?color=3775A9&style=for-the-badge&logo=pypi&logoColor=FFD43B)](https://pypi.org/project/adbpyg-adapter/)
+        [![Python versions badge](https://img.shields.io/pypi/pyversions/adbpyg-adapter?color=3776AB&style=for-the-badge&logo=python&logoColor=FFD43B)](https://pypi.org/project/adbpyg-adapter/)
+        
+        [![License](https://img.shields.io/github/license/arangoml/pyg-adapter?color=9E2165&style=for-the-badge)](https://github.com/arangoml/pyg-adapter/blob/master/LICENSE)
+        [![Code style: black](https://img.shields.io/static/v1?style=for-the-badge&label=code%20style&message=black&color=black)](https://github.com/psf/black)
+        [![Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&color=282661&label=Downloads&query=total_downloads&url=https://api.pepy.tech/api/v2/projects/adbpyg-adapter)](https://pepy.tech/project/adbpyg-adapter)
+        
+        
+        <a href="https://www.arangodb.com/" rel="arangodb.com">![](https://raw.githubusercontent.com/arangoml/pyg-adapter/master/examples/assets/adb_logo.png)</a>
+        <a href="https://www.pyg.org/" rel="pyg.org"><img src="https://raw.githubusercontent.com/pyg-team/pyg_sphinx_theme/master/pyg_sphinx_theme/static/img/pyg_logo_text.svg?sanitize=true" width=40% /></a>
+        
+        The ArangoDB-PyG Adapter exports Graphs from ArangoDB, the multi-model database for graph & beyond, into PyTorch Geometric (PyG), a PyTorch-based Graph Neural Network library, and vice-versa.
+        
+        ## About PyG
+        
+        **PyG** *(PyTorch Geometric)* is a library built upon [PyTorch](https://pytorch.org/) to easily write and train Graph Neural Networks (GNNs) for a wide range of applications related to structured data.
+        
+        It consists of various methods for deep learning on graphs and other irregular structures, also known as *[geometric deep learning](http://geometricdeeplearning.com/)*, from a variety of published papers.
+        In addition, it consists of easy-to-use mini-batch loaders for operating on many small and single giant graphs, [multi GPU-support](https://github.com/pyg-team/pytorch_geometric/tree/master/examples/multi_gpu), [`DataPipe` support](https://github.com/pyg-team/pytorch_geometric/blob/master/examples/datapipe.py), distributed graph learning via [Quiver](https://github.com/pyg-team/pytorch_geometric/tree/master/examples/quiver), a large number of common benchmark datasets (based on simple interfaces to create your own), the [GraphGym](https://pytorch-geometric.readthedocs.io/en/latest/notes/graphgym.html) experiment manager, and helpful transforms, both for learning on arbitrary graphs as well as on 3D meshes or point clouds.
+        
+        ## Installation
+        
+        #### Latest Release
+        ```
+        pip install torch
+        pip install adbpyg-adapter
+        ```
+        #### Current State
+        ```
+        pip install torch
+        pip install git+https://github.com/arangoml/pyg-adapter.git
+        ```
+        
+        ##  Quickstart
+        
+        [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/arangoml/pyg-adapter/blob/master/examples/ArangoDB_PyG_Adapter.ipynb)
+        
+        Also available as an ArangoDB Lunch & Learn session on YouTube: [Graph & Beyond Course: ArangoDB-PyG Adapter](https://www.youtube.com/watch?v=QtGR95NN8bA)
+        
+        ```py
+        import torch
+        import pandas
+        from torch_geometric.datasets import FakeHeteroDataset
+        
+        from arango import ArangoClient  # Python-Arango driver
+        
+        from adbpyg_adapter import ADBPyG_Adapter, ADBPyG_Controller
+        from adbpyg_adapter.encoders import IdentityEncoder, CategoricalEncoder
+        
+        # Load some fake PyG data for demo purposes
+        data = FakeHeteroDataset(
+            num_node_types=2,
+            num_edge_types=3,
+            avg_num_nodes=20,
+            avg_num_channels=3,  # avg number of features per node
+            edge_dim=2,  # number of features per edge
+            num_classes=3,  # number of unique label values
+        )[0]
+        
+        # Let's assume that the ArangoDB "IMDB" dataset is imported to this endpoint
+        db = ArangoClient(hosts="http://localhost:8529").db("_system", username="root", password="")
+        
+        adbpyg_adapter = ADBPyG_Adapter(db)
+        ```
+        
+        ### PyG to ArangoDB
+        
+        Note: If the PyG graph contains `_key`, `_v_key`, or `_e_key` properties for any node / edge types, the adapter will assume to persist those values as [ArangoDB document keys](https://www.arangodb.com/docs/stable/data-modeling-naming-conventions-document-keys.html). See the `Full Cycle (ArangoDB -> PyG -> ArangoDB)` section below for an example.
+        
+        ```py
+        # 1.1: PyG to ArangoDB
+        adb_g = adbpyg_adapter.pyg_to_arangodb("FakeData", data)
+        
+        # 1.2: PyG to ArangoDB with a (completely optional) metagraph for customized adapter behaviour
+        def y_tensor_to_2_column_dataframe(pyg_tensor, adb_df):
+            """
+            A user-defined function to create two
+            ArangoDB attributes out of the 'user' label tensor
+        
+            :param dgl_tensor: The DGL Tensor containing the data
+            :type dgl_tensor: torch.Tensor
+            :param adb_df: The ArangoDB DataFrame to populate, whose
+                size is preset to the length of **dgl_tensor**.
+            :type adb_df: pandas.DataFrame
+        
+            NOTE: user-defined functions must return the modified **adb_df**
+            """
+            label_map = {0: "Kiwi", 1: "Blueberry", 2: "Avocado"}
+        
+            adb_df["label_num"] = pyg_tensor.tolist()
+            adb_df["label_str"] = adb_df["label_num"].map(label_map)
+        
+            return adb_df
+        
+        
+        metagraph = {
+            "nodeTypes": {
+                "v0": {
+                    "x": "features",  # 1) You can specify a string value if you want to rename your PyG data when stored in ArangoDB
+                    "y": y_tensor_to_2_column_dataframe,  # 2) you can specify a function for user-defined handling, as long as the function returns a Pandas DataFrame
+                },
+                # 3) You can specify set of strings if you want to preserve the same PyG attribute names for the node/edge type
+                "v1": {"x"} # this is equivalent to {"x": "x"}
             },
-            "y": "Comedy",
-        },
-        "Users": {
-            "x": {
-                "Gender": CategoricalEncoder(mapping={"M": 0, "F": 1}),
-                "Age": IdentityEncoder(dtype=torch.long),
-            }
-        },
-    },
-    "edgeCollections": {
-        "Ratings": { "edge_weight": "Rating" } # Use the 'Rating' attribute for the PyG 'edge_weight' property
-    },
-}
-pyg_g = adbpyg_adapter.arangodb_to_pyg("IMDB", metagraph_v2)
-
-# 2.5: ArangoDB to PyG via Metagraph v3 (transfer attributes via user-defined functions)
-def udf_v0_x(v0_df):
-    # process v0_df here to return v0 "x" feature matrix
-    # v0_df["x"] = ...
-    return torch.tensor(v0_df["x"].to_list())
-
-
-def udf_v1_x(v1_df):
-    # process v1_df here to return v1 "x" feature matrix
-    # v1_df["x"] = ...
-    return torch.tensor(v1_df["x"].to_list())
-
-
-metagraph_v3 = {
-    "vertexCollections": {
-        "v0": {
-            "x": udf_v0_x,  # supports named functions
-            "y": lambda df: torch.tensor(df["y"].to_list()),  # also supports lambda functions
-        },
-        "v1": {"x": udf_v1_x},
-    },
-    "edgeCollections": {
-        "e0": {"edge_attr": (lambda df: torch.tensor(df["edge_attr"].to_list()))},
-    },
-}
-pyg_g = adbpyg_adapter.arangodb_to_pyg("FakeData", metagraph_v3)
-```
-
-### Experimental: `preserve_adb_keys`
-```py
-# With `preserve_adb_keys=True`, the adapter will preserve the ArangoDB vertex & edge _key values into the (newly created) PyG graph.
-# Users can then re-import their PyG graph into ArangoDB using the same _key values 
-pyg_g = adbpyg_adapter.arangodb_graph_to_pyg("imdb", preserve_adb_keys=True)
-
-# pyg_g["Movies"]["_key"] --> ["1", "2", ..., "1682"]
-# pyg_g["Users"]["_key"] --> ["1", "2", ..., "943"]
-# pyg_g[("Users", "Ratings", "Movies")]["_key"] --> ["2732620466", ..., "2730643624"]
-
-# Let's add a new PyG User Node by updating the _key property
-pyg_g["Users"]["_key"].append("new-user-here-944")
-
-# Note: Prior to the re-import, we must manually set the number of nodes in the PyG graph, since the `arangodb_graph_to_pyg` API creates featureless node data
-pyg_g["Movies"].num_nodes = len(pyg_g["Movies"]["_key"]) # 1682
-pyg_g["Users"].num_nodes = len(pyg_g["Users"]["_key"]) # 944 (prev. 943)
-
-# Re-import PyG graph into ArangoDB
-adbpyg_adapter.pyg_to_arangodb("imdb", pyg_g, on_duplicate="update")
-```
-
-##  Development & Testing
-
-Prerequisite: `arangorestore`
-
-1. `git clone https://github.com/arangoml/pyg-adapter.git`
-2. `cd pyg-adapter`
-3. (create virtual environment of choice)
-4. `pip install -e .[dev]`
-5. (create an ArangoDB instance with method of choice)
-6. `pytest --url <> --dbName <> --username <> --password <>`
-
-**Note**: A `pytest` parameter can be omitted if the endpoint is using its default value:
-```python
-def pytest_addoption(parser):
-    parser.addoption("--url", action="store", default="http://localhost:8529")
-    parser.addoption("--dbName", action="store", default="_system")
-    parser.addoption("--username", action="store", default="root")
-    parser.addoption("--password", action="store", default="")
-```
+            "edgeTypes": {
+                ("v0", "e0", "v0"): {
+                    # 4) You can specify a list of strings for tensor dissasembly (if you know the number of node/edge features in advance)
+                    "edge_attr": [ "a", "b"]  
+                },
+            },
+        }
+        
+        
+        adb_g = adbpyg_adapter.pyg_to_arangodb("FakeData", data, metagraph, explicit_metagraph=False)
+        
+        # 1.3: PyG to ArangoDB with the same (optional) metagraph, but with `explicit_metagraph=True`
+        # With `explicit_metagraph=True`, the node & edge types omitted from the metagraph will NOT be converted to ArangoDB.
+        # Only 'v0', 'v1' and ('v0', 'e0', 'v0') will be brought over (i.e 'v2', ('v0', 'e0', 'v1'), ... are ignored)
+        adb_g = adbpyg_adapter.pyg_to_arangodb("FakeData", data, metagraph, explicit_metagraph=True)
+        
+        # 1.4: PyG to ArangoDB with a Custom Controller  (more user-defined behavior)
+        class Custom_ADBPyG_Controller(ADBPyG_Controller):
+            def _prepare_pyg_node(self, pyg_node: dict, node_type: str) -> dict:
+                """Optionally modify a PyG node object before it gets inserted into its designated ArangoDB collection.
+        
+                :param pyg_node: The PyG node object to (optionally) modify.
+                :param node_type: The PyG Node Type of the node.
+                :return: The PyG Node object
+                """
+                pyg_node["foo"] = "bar"
+                return pyg_node
+        
+            def _prepare_pyg_edge(self, pyg_edge: dict, edge_type: tuple) -> dict:
+                """Optionally modify a PyG edge object before it gets inserted into its designated ArangoDB collection.
+        
+                :param pyg_edge: The PyG edge object to (optionally) modify.
+                :param edge_type: The Edge Type of the PyG edge. Formatted
+                    as (from_collection, edge_collection, to_collection)
+                :return: The PyG Edge object
+                """
+                pyg_edge["bar"] = "foo"
+                return pyg_edge
+        
+        
+        adb_g = ADBPyG_Adapter(db, Custom_ADBPyG_Controller()).pyg_to_arangodb("FakeData", data)
+        ```
+        
+        ### ArangoDB to PyG
+        ```py
+        # Start from scratch!
+        db.delete_graph("FakeData", drop_collections=True, ignore_missing=True)
+        adbpyg_adapter.pyg_to_arangodb("FakeData", data)
+        
+        # 2.1: ArangoDB to PyG via Graph name (does not transfer attributes)
+        pyg_g = adbpyg_adapter.arangodb_graph_to_pyg("FakeData")
+        
+        # 2.2: ArangoDB to PyG via Collection names (does not transfer attributes)
+        pyg_g = adbpyg_adapter.arangodb_collections_to_pyg("FakeData", v_cols={"v0", "v1"}, e_cols={"e0"})
+        
+        # 2.3: ArangoDB to PyG via Metagraph v1 (transfer attributes "as is", meaning they are already formatted to PyG data standards)
+        metagraph_v1 = {
+            "vertexCollections": {
+                # Move the "x" & "y" ArangoDB attributes to PyG as "x" & "y" Tensors
+                "v0": {"x", "y"}, # equivalent to {"x": "x", "y": "y"}
+                "v1": {"v1_x": "x"}, # store the 'x' feature matrix as 'v1_x' in PyG
+            },
+            "edgeCollections": {
+                "e0": {"edge_attr"},
+            },
+        }
+        pyg_g = adbpyg_adapter.arangodb_to_pyg("FakeData", metagraph_v1)
+        
+        # 2.4: ArangoDB to PyG via Metagraph v2 (transfer attributes via user-defined encoders)
+        # For more info on user-defined encoders in PyG, see https://pytorch-geometric.readthedocs.io/en/latest/notes/load_csv.html
+        metagraph_v2 = {
+            "vertexCollections": {
+                "Movies": {
+                    "x": {  # Build a feature matrix from the "Action" & "Drama" document attributes
+                        "Action": IdentityEncoder(dtype=torch.long),
+                        "Drama": IdentityEncoder(dtype=torch.long),
+                    },
+                    "y": "Comedy",
+                },
+                "Users": {
+                    "x": {
+                        "Gender": CategoricalEncoder(mapping={"M": 0, "F": 1}),
+                        "Age": IdentityEncoder(dtype=torch.long),
+                    }
+                },
+            },
+            "edgeCollections": {
+                "Ratings": { "edge_weight": "Rating" } # Use the 'Rating' attribute for the PyG 'edge_weight' property
+            },
+        }
+        pyg_g = adbpyg_adapter.arangodb_to_pyg("IMDB", metagraph_v2)
+        
+        # 2.5: ArangoDB to PyG via Metagraph v3 (transfer attributes via user-defined functions)
+        def udf_v0_x(v0_df):
+            # process v0_df here to return v0 "x" feature matrix
+            # v0_df["x"] = ...
+            return torch.tensor(v0_df["x"].to_list())
+        
+        
+        def udf_v1_x(v1_df):
+            # process v1_df here to return v1 "x" feature matrix
+            # v1_df["x"] = ...
+            return torch.tensor(v1_df["x"].to_list())
+        
+        
+        metagraph_v3 = {
+            "vertexCollections": {
+                "v0": {
+                    "x": udf_v0_x,  # supports named functions
+                    "y": lambda df: torch.tensor(df["y"].to_list()),  # also supports lambda functions
+                },
+                "v1": {"x": udf_v1_x},
+            },
+            "edgeCollections": {
+                "e0": {"edge_attr": (lambda df: torch.tensor(df["edge_attr"].to_list()))},
+            },
+        }
+        pyg_g = adbpyg_adapter.arangodb_to_pyg("FakeData", metagraph_v3)
+        ```
+        
+        ### Experimental: `preserve_adb_keys`
+        ```py
+        # With `preserve_adb_keys=True`, the adapter will preserve the ArangoDB vertex & edge _key values into the (newly created) PyG graph.
+        # Users can then re-import their PyG graph into ArangoDB using the same _key values 
+        pyg_g = adbpyg_adapter.arangodb_graph_to_pyg("imdb", preserve_adb_keys=True)
+        
+        # pyg_g["Movies"]["_key"] --> ["1", "2", ..., "1682"]
+        # pyg_g["Users"]["_key"] --> ["1", "2", ..., "943"]
+        # pyg_g[("Users", "Ratings", "Movies")]["_key"] --> ["2732620466", ..., "2730643624"]
+        
+        # Let's add a new PyG User Node by updating the _key property
+        pyg_g["Users"]["_key"].append("new-user-here-944")
+        
+        # Note: Prior to the re-import, we must manually set the number of nodes in the PyG graph, since the `arangodb_graph_to_pyg` API creates featureless node data
+        pyg_g["Movies"].num_nodes = len(pyg_g["Movies"]["_key"]) # 1682
+        pyg_g["Users"].num_nodes = len(pyg_g["Users"]["_key"]) # 944 (prev. 943)
+        
+        # Re-import PyG graph into ArangoDB
+        adbpyg_adapter.pyg_to_arangodb("imdb", pyg_g, on_duplicate="update")
+        ```
+        
+        ##  Development & Testing
+        
+        Prerequisite: `arangorestore`
+        
+        1. `git clone https://github.com/arangoml/pyg-adapter.git`
+        2. `cd pyg-adapter`
+        3. (create virtual environment of choice)
+        4. `pip install torch`
+        5. `pip install -e .[dev]`
+        6. (create an ArangoDB instance with method of choice)
+        7. `pytest --url <> --dbName <> --username <> --password <>`
+        
+        **Note**: A `pytest` parameter can be omitted if the endpoint is using its default value:
+        ```python
+        def pytest_addoption(parser):
+            parser.addoption("--url", action="store", default="http://localhost:8529")
+            parser.addoption("--dbName", action="store", default="_system")
+            parser.addoption("--username", action="store", default="root")
+            parser.addoption("--password", action="store", default="")
+        ```
+        
+Keywords: arangodb,pyg,pytorch,pytorch geometric,adapter
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `adbpyg_adapter-1.1.0/adbpyg_adapter/abc.py` & `adbpyg_adapter-1.1.1/adbpyg_adapter/abc.py`

 * *Files identical despite different names*

### Comparing `adbpyg_adapter-1.1.0/adbpyg_adapter/adapter.py` & `adbpyg_adapter-1.1.1/adbpyg_adapter/adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import logging
 from collections import defaultdict
-from typing import Any, DefaultDict, Dict, List, Set, Union
+from math import ceil
+from typing import Any, DefaultDict, Dict, List, Optional, Set, Union
 
+import torch
+from arango.cursor import Cursor
 from arango.database import Database
 from arango.graph import Graph as ADBGraph
-from pandas import DataFrame
+from pandas import DataFrame, Series
 from torch import Tensor, cat, tensor
 from torch_geometric.data import Data, HeteroData
 from torch_geometric.data.storage import EdgeStorage, NodeStorage
 from torch_geometric.typing import EdgeType
 
 from .abc import Abstract_ADBPyG_Adapter
 from .controller import ADBPyG_Controller
-from .exceptions import ADBMetagraphError, PyGMetagraphError
+from .exceptions import ADBMetagraphError, InvalidADBEdgesError, PyGMetagraphError
 from .typings import (
     ADBMap,
     ADBMetagraph,
     ADBMetagraphValues,
     Json,
     PyGMap,
     PyGMetagraph,
@@ -46,43 +49,44 @@
         self,
         db: Database,
         controller: ADBPyG_Controller = ADBPyG_Controller(),
         logging_lvl: Union[str, int] = logging.INFO,
     ):
         self.set_logging(logging_lvl)
 
-        if not issubclass(type(db), Database):
+        if not isinstance(db, Database):
             msg = "**db** parameter must inherit from arango.database.Database"
             raise TypeError(msg)
 
-        if not issubclass(type(controller), ADBPyG_Controller):
+        if not isinstance(controller, ADBPyG_Controller):
             msg = "**controller** parameter must inherit from ADBPyG_Controller"
             raise TypeError(msg)
 
         self.__db = db
         self.__cntrl = controller
 
         logger.info(f"Instantiated ADBPyG_Adapter with database '{db.name}'")
 
     @property
     def db(self) -> Database:
         return self.__db  # pragma: no cover
 
     @property
-    def cntrl(self) -> Database:
+    def cntrl(self) -> ADBPyG_Controller:
         return self.__cntrl  # pragma: no cover
 
     def set_logging(self, level: Union[int, str]) -> None:
         logger.setLevel(level)
 
     def arangodb_to_pyg(
         self,
         name: str,
         metagraph: ADBMetagraph,
         preserve_adb_keys: bool = False,
+        strict: bool = True,
         **query_options: Any,
     ) -> Union[Data, HeteroData]:
         """Create a PyG graph from ArangoDB data. DOES carry
             over node/edge features/labels, via the **metagraph**.
 
         :param name: The PyG graph name.
         :type name: str
@@ -123,14 +127,17 @@
             )
 
             NOTE: If your ArangoDB graph is Homogeneous, the ArangoDB keys will
             be preserved under `_v_key` & `_e_key` in your PyG graph. If your
             ArangoDB graph is Heterogeneous, the ArangoDB keys will be preserved
             under `_key` in your PyG graph.
         :type preserve_adb_keys: bool
+        :param strict: Set fault tolerance when loading a graph from ArangoDB. If set
+            to false, this will ignore invalid edges (e.g. dangling/half edges).
+        :type strict: bool
         :param query_options: Keyword arguments to specify AQL query options when
             fetching documents from the ArangoDB instance. Full parameter list:
             https://docs.python-arango.com/en/main/specs.html#arango.aql.AQL.execute
         :type query_options: Any
         :return: A PyG Data or HeteroData object
         :rtype: torch_geometric.data.Data | torch_geometric.data.HeteroData
         :raise adbpyg_adapter.exceptions.ADBMetagraphError: If invalid metagraph.
@@ -250,61 +257,99 @@
         adb_map: ADBMap = defaultdict(dict)
 
         data = Data() if is_homogeneous else HeteroData()
 
         for v_col, meta in metagraph["vertexCollections"].items():
             logger.debug(f"Preparing '{v_col}' vertices")
 
-            df = self.__fetch_adb_docs(v_col, meta == {}, query_options)
-            adb_map[v_col] = {
-                adb_id: pyg_id for pyg_id, adb_id in enumerate(df["_key"])
-            }
-
             node_data: NodeStorage = data if is_homogeneous else data[v_col]
-            self.__set_pyg_data(meta, node_data, df)
 
             if preserve_adb_keys:
-                k = "_v_key" if is_homogeneous else "_key"
-                node_data[k] = list(adb_map[v_col].keys())
+                preserve_key = "_v_key" if is_homogeneous else "_key"
+                node_data[preserve_key] = []
+
+            pyg_id = 0
+            cursor = self.__fetch_adb_docs(v_col, meta, query_options)
+            while not cursor.empty():
+                cursor_batch = len(cursor.batch())  # type: ignore
+                df = DataFrame([cursor.pop() for _ in range(cursor_batch)])
+
+                for adb_id in df["_key"]:
+                    adb_map[v_col][adb_id] = pyg_id
+                    pyg_id += 1
+
+                self.__set_pyg_data(meta, node_data, df)
+
+                if preserve_adb_keys:
+                    node_data[preserve_key].extend(list(df["_key"]))
+
+                if cursor.has_more():
+                    cursor.fetch()
+
+                df.drop(df.index, inplace=True)
 
         et_df: DataFrame
         v_cols: List[str] = list(metagraph["vertexCollections"].keys())
         for e_col, meta in metagraph.get("edgeCollections", {}).items():
             logger.debug(f"Preparing '{e_col}' edges")
 
-            df = self.__fetch_adb_docs(e_col, meta == {}, query_options)
-            df[["from_col", "from_key"]] = df["_from"].str.split("/", 1, True)
-            df[["to_col", "to_key"]] = df["_to"].str.split("/", 1, True)
+            cursor = self.__fetch_adb_docs(e_col, meta, query_options)
+            while not cursor.empty():
+                cursor_batch = len(cursor.batch())  # type: ignore
+                df = DataFrame([cursor.pop() for _ in range(cursor_batch)])
+
+                df[["from_col", "from_key"]] = self.__split_adb_ids(df["_from"])
+                df[["to_col", "to_key"]] = self.__split_adb_ids(df["_to"])
+
+                for (from_col, to_col), count in (
+                    df[["from_col", "to_col"]].value_counts().items()
+                ):
+                    edge_type = (from_col, e_col, to_col)
+                    edge_data: EdgeStorage = data if is_homogeneous else data[edge_type]
+
+                    if from_col not in v_cols or to_col not in v_cols:
+                        logger.debug(f"Skipping {edge_type}")
+                        continue  # partial edge collection import to pyg
+
+                    logger.debug(f"Preparing {count} '{edge_type}' edges")
+
+                    et_df = df[(df["from_col"] == from_col) & (df["to_col"] == to_col)]
+
+                    from_nodes = et_df["from_key"].map(adb_map[from_col]).tolist()
+                    to_nodes = et_df["to_key"].map(adb_map[to_col]).tolist()
+                    edge_index = tensor([from_nodes, to_nodes])
+
+                    edge_data.edge_index = torch.cat(
+                        (edge_data.get("edge_index", tensor([])), edge_index), dim=1
+                    )
+
+                    if torch.any(torch.isnan(edge_data.edge_index)):
+                        if strict:
+                            raise InvalidADBEdgesError(
+                                f"Invalid edges found in Edge Collection {e_col}, {from_col} -> {to_col}."  # noqa: E501
+                            )
+                        else:
+                            # Remove the invalid edges
+                            edge_data.edge_index = edge_data.edge_index[
+                                :, ~torch.any(edge_data.edge_index.isnan(), dim=0)
+                            ]
+
+                    self.__set_pyg_data(meta, edge_data, et_df)
+
+                    if preserve_adb_keys:
+                        preserve_key = "_e_key" if is_homogeneous else "_key"
+                        if preserve_key not in edge_data:
+                            edge_data[preserve_key] = []
 
-            for (from_col, to_col), count in (
-                df[["from_col", "to_col"]].value_counts().items()
-            ):
-                edge_type = (from_col, e_col, to_col)
-                if from_col not in v_cols or to_col not in v_cols:
-                    logger.debug(f"Skipping {edge_type}")
-                    continue  # partial edge collection import to pyg
-
-                logger.debug(f"Preparing {count} '{edge_type}' edges")
-
-                # Get the edge data corresponding to the current edge type
-                et_df = df[(df["from_col"] == from_col) & (df["to_col"] == to_col)]
-                adb_map[edge_type] = {
-                    adb_id: pyg_id for pyg_id, adb_id in enumerate(et_df["_key"])
-                }
+                        edge_data[preserve_key].extend(list(et_df["_key"]))
 
-                from_nodes = et_df["from_key"].map(adb_map[from_col]).tolist()
-                to_nodes = et_df["to_key"].map(adb_map[to_col]).tolist()
+                if cursor.has_more():
+                    cursor.fetch()
 
-                edge_data: EdgeStorage = data if is_homogeneous else data[edge_type]
-                edge_data.edge_index = tensor([from_nodes, to_nodes])
-                self.__set_pyg_data(meta, edge_data, et_df)
-
-                if preserve_adb_keys:
-                    k = "_e_key" if is_homogeneous else "_key"
-                    edge_data[k] = list(adb_map[edge_type].keys())
+                df.drop(df.index, inplace=True)
 
         logger.info(f"Created PyG '{name}' Graph")
         return data
 
     def arangodb_collections_to_pyg(
         self,
         name: str,
@@ -380,28 +425,30 @@
             https://docs.python-arango.com/en/main/specs.html#arango.aql.AQL.execute
         :type query_options: Any
         :return: A PyG Data or HeteroData object
         :rtype: torch_geometric.data.Data | torch_geometric.data.HeteroData
         :raise adbpyg_adapter.exceptions.ADBMetagraphError: If invalid metagraph.
         """
         graph = self.__db.graph(name)
-        v_cols = graph.vertex_collections()
-        e_cols = {col["edge_collection"] for col in graph.edge_definitions()}
+        v_cols: Set[str] = graph.vertex_collections()  # type: ignore
+        edge_definitions: List[Json] = graph.edge_definitions()  # type: ignore
+        e_cols: Set[str] = {c["edge_collection"] for c in edge_definitions}
 
         return self.arangodb_collections_to_pyg(
             name, v_cols, e_cols, preserve_adb_keys, **query_options
         )
 
     def pyg_to_arangodb(
         self,
         name: str,
         pyg_g: Union[Data, HeteroData],
         metagraph: PyGMetagraph = {},
         explicit_metagraph: bool = True,
         overwrite_graph: bool = False,
+        batch_size: Optional[int] = None,
         **import_options: Any,
     ) -> ADBGraph:
         """Create an ArangoDB graph from a PyG graph.
 
         :param name: The ArangoDB graph name.
         :type name: str
         :param pyg_g: The existing PyG graph.
@@ -434,35 +481,38 @@
             If False, node & edge types OMITTED from the metagraph will be
             brought over into ArangoDB. Also applies to node & edge attributes.
             Defaults to True.
         :type explicit_metagraph: bool
         :param overwrite_graph: Overwrites the graph if it already exists.
             Does not drop associated collections. Defaults to False.
         :type overwrite_graph: bool
+        :param batch_size: Process the PyG Nodes & Edges in batches of size
+            **batch_size**. Defaults to `None`, which processes each
+            NodeStorage & EdgeStorage in one batch.
+        :type batch_size: int
         :param import_options: Keyword arguments to specify additional
             parameters for ArangoDB document insertion. Full parameter list:
             https://docs.python-arango.com/en/main/specs.html#arango.collection.Collection.import_bulk
         :type import_options: Any
         :return: The ArangoDB Graph API wrapper.
         :rtype: arango.graph.Graph
         :raise adbpyg_adapter.exceptions.PyGMetagraphError: If invalid metagraph.
 
         **metagraph** example
 
         .. code-block:: python
-        def y_tensor_to_2_column_dataframe(pyg_tensor):
+        def y_tensor_to_2_column_dataframe(pyg_tensor, adb_df):
             # A user-defined function to create two ArangoDB attributes
             # out of the 'y' label tensor
             label_map = {0: "Kiwi", 1: "Blueberry", 2: "Avocado"}
 
-            df = pandas.DataFrame(columns=["label_num", "label_str"])
-            df["label_num"] = pyg_tensor.tolist()
-            df["label_str"] = df["label_num"].map(label_map)
+            adb_df["label_num"] = pyg_tensor.tolist()
+            adb_df["label_str"] = adb_df["label_num"].map(label_map)
 
-            return df
+            return adb_df
 
         metagraph = {
             "nodeTypes": {
                 "v0": {
                     "x": "features",  # 1)
                     "y": y_tensor_to_2_column_dataframe,  # 2)
                 },
@@ -481,14 +531,15 @@
         3) Transfers the PyG 'v1' 'x' feature matrix under the same name.
         4) Dissasembles the 2-feature Tensor into two ArangoDB attributes,
             where each attribute holds one feature value.
         """
         logger.debug(f"--pyg_to_arangodb('{name}')--")
 
         validate_pyg_metagraph(metagraph)
+        is_custom_controller = type(self.__cntrl) is not ADBPyG_Controller
 
         is_homogeneous = type(pyg_g) is Data
         if is_homogeneous and pyg_g.num_nodes == pyg_g.num_edges and not metagraph:
             msg = f"""
                 Ambiguity Error: can't convert to ArangoDB,
                 as the PyG graph has the same number
                 of nodes & edges {pyg_g.num_nodes}.
@@ -504,17 +555,17 @@
         edge_types: List[EdgeType]
         explicit_metagraph = metagraph != {} and explicit_metagraph
         if explicit_metagraph:
             node_types = metagraph.get("nodeTypes", {}).keys()  # type: ignore
             edge_types = metagraph.get("edgeTypes", {}).keys()  # type: ignore
 
         elif is_homogeneous:
-            n_type = name + "_N"
+            n_type = f"{name}_N"
             node_types = [n_type]
-            edge_types = [(n_type, name + "_E", n_type)]
+            edge_types = [(n_type, f"{name}_E", n_type)]
 
         else:
             node_types = pyg_g.node_types
             edge_types = pyg_g.edge_types
 
         if overwrite_graph:
             logger.debug("Overwrite graph flag is True. Deleting old graph.")
@@ -523,69 +574,105 @@
         if self.__db.has_graph(name):
             adb_graph = self.__db.graph(name)
         else:
             edge_definitions = self.etypes_to_edefinitions(edge_types)
             orphan_collections = self.ntypes_to_ocollections(node_types, edge_types)
             adb_graph = self.__db.create_graph(
                 name, edge_definitions, orphan_collections
-            )
+            )  # type: ignore
 
         # Define PyG data properties
         node_data: NodeStorage
         edge_data: EdgeStorage
 
         n_meta = metagraph.get("nodeTypes", {})
         for n_type in node_types:
+            meta = n_meta.get(n_type, {})
+
             node_data = pyg_g if is_homogeneous else pyg_g[n_type]
+            node_data_batch_size = batch_size or node_data.num_nodes
 
-            meta = n_meta.get(n_type, {})
-            empty_df = DataFrame(index=range(node_data.num_nodes))
-            df = self.__set_adb_data(empty_df, meta, node_data, explicit_metagraph)
+            start_index = 0
+            end_index = min(node_data_batch_size, node_data.num_nodes)
+            batches = ceil(node_data.num_nodes / node_data_batch_size)
+
+            for _ in range(batches):
+                df = self.__set_adb_data(
+                    DataFrame(index=range(start_index, end_index)),
+                    meta,
+                    node_data,
+                    node_data.num_nodes,
+                    start_index,
+                    end_index,
+                    explicit_metagraph,
+                )
 
-            if "_id" in df:
-                pyg_map[n_type] = df["_id"].to_dict()
-            else:
-                if "_key" not in df:
-                    df["_key"] = df.index.astype(str)
-
-                pyg_map[n_type] = (n_type + "/" + df["_key"]).to_dict()
-
-            if type(self.__cntrl) is not ADBPyG_Controller:
-                f = lambda n: self.__cntrl._prepare_pyg_node(n, n_type)
-                df = df.apply(f, axis=1)
+                if "_id" in df:
+                    pyg_map[n_type].update(df["_id"].to_dict())
+                else:
+                    df["_key"] = df.get("_key", df.index.astype(str))
+                    pyg_map[n_type].update((n_type + "/" + df["_key"]).to_dict())
+
+                if is_custom_controller:
+                    f = lambda n: self.__cntrl._prepare_pyg_node(n, n_type)
+                    df = df.apply(f, axis=1)
 
-            self.__insert_adb_docs(n_type, df, import_options)
+                self.__insert_adb_docs(n_type, df, import_options)
+
+                start_index = end_index
+                end_index = min(end_index + node_data_batch_size, node_data.num_nodes)
 
         e_meta = metagraph.get("edgeTypes", {})
         for e_type in edge_types:
-            edge_data = pyg_g if is_homogeneous else pyg_g[e_type]
+            meta = e_meta.get(e_type, {})
             src_n_type, _, dst_n_type = e_type
 
-            columns = ["_from", "_to"]
-            meta = e_meta.get(e_type, {})
-            df = DataFrame(zip(*(edge_data.edge_index.tolist())), columns=columns)
-            df = self.__set_adb_data(df, meta, edge_data, explicit_metagraph)
+            edge_data = pyg_g if is_homogeneous else pyg_g[e_type]
+            edge_data_batch_size = batch_size or edge_data.num_edges
 
-            df["_from"] = (
-                df["_from"].map(pyg_map[src_n_type])
-                if pyg_map[src_n_type]
-                else src_n_type + "/" + df["_from"].astype(str)
-            )
+            start_index = 0
+            end_index = min(edge_data_batch_size, edge_data.num_edges)
+            batches = ceil(edge_data.num_edges / edge_data_batch_size)
+
+            for _ in range(batches):
+                edge_index = edge_data.edge_index[:, start_index:end_index]
+                df = self.__set_adb_data(
+                    DataFrame(
+                        zip(*(edge_index.tolist())),
+                        index=range(start_index, end_index),
+                        columns=["_from", "_to"],
+                    ),
+                    meta,
+                    edge_data,
+                    edge_data.num_edges,
+                    start_index,
+                    end_index,
+                    explicit_metagraph,
+                )
 
-            df["_to"] = (
-                df["_to"].map(pyg_map[dst_n_type])
-                if pyg_map[dst_n_type]
-                else dst_n_type + "/" + df["_to"].astype(str)
-            )
+                df["_from"] = (
+                    df["_from"].map(pyg_map[src_n_type])
+                    if pyg_map[src_n_type]
+                    else src_n_type + "/" + df["_from"].astype(str)
+                )
+
+                df["_to"] = (
+                    df["_to"].map(pyg_map[dst_n_type])
+                    if pyg_map[dst_n_type]
+                    else dst_n_type + "/" + df["_to"].astype(str)
+                )
+
+                if is_custom_controller:
+                    f = lambda e: self.__cntrl._prepare_pyg_edge(e, e_type)
+                    df = df.apply(f, axis=1)
 
-            if type(self.__cntrl) is not ADBPyG_Controller:
-                f = lambda e: self.__cntrl._prepare_pyg_edge(e, e_type)
-                df = df.apply(f, axis=1)
+                self.__insert_adb_docs(e_type, df, import_options)
 
-            self.__insert_adb_docs(e_type, df, import_options)
+                start_index = end_index
+                end_index = min(end_index + edge_data_batch_size, edge_data.num_edges)
 
         logger.info(f"Created ArangoDB '{name}' Graph")
         return adb_graph
 
     def etypes_to_edefinitions(self, edge_types: List[EdgeType]) -> List[Json]:
         """Converts PyG edge_types to ArangoDB edge_definitions
 
@@ -649,51 +736,72 @@
             non_orphan_collections.add(from_col)
             non_orphan_collections.add(to_col)
 
         orphan_collections = set(node_types) ^ non_orphan_collections
         return list(orphan_collections)
 
     def __fetch_adb_docs(
-        self, col: str, empty_meta: bool, query_options: Any
-    ) -> DataFrame:
+        self,
+        col: str,
+        meta: Union[Set[str], Dict[str, ADBMetagraphValues]],
+        query_options: Any,
+    ) -> Cursor:
         """Fetches ArangoDB documents within a collection. Returns the
             documents in a DataFrame.
 
         :param col: The ArangoDB collection.
         :type col: str
-        :param empty_meta: Set to True if the metagraph specification
-            for **col** is empty.
-        :type empty_meta: bool
+        :param meta: The MetaGraph associated to **col**
+        :type meta: Set[str] | Dict[str, adbpyg_adapter.typings.ADBMetagraphValues]
         :param query_options: Keyword arguments to specify AQL query options
             when fetching documents from the ArangoDB instance.
         :type query_options: Any
         :return: A DataFrame representing the ArangoDB documents.
         :rtype: pandas.DataFrame
         """
-        # Only return the entire document if **empty_meta** is False
-        aql = f"""
-            FOR doc IN @@col
-                RETURN {
-                    "{ _key: doc._key, _from: doc._from, _to: doc._to }"
-                    if empty_meta
-                    else "doc"
-                }
-        """
+
+        def get_aql_return_value(
+            meta: Union[Set[str], Dict[str, ADBMetagraphValues]]
+        ) -> str:
+            """Helper method to formulate the AQL `RETURN` value based on
+            the document attributes specified in **meta**
+            """
+            attributes = []
+
+            if type(meta) is set:
+                attributes = list(meta)
+
+            elif type(meta) is dict:
+                for value in meta.values():
+                    if type(value) is str:
+                        attributes.append(value)
+                    elif type(value) is dict:
+                        attributes.extend(list(value.keys()))
+                    elif callable(value):
+                        # Cannot determine which attributes to extract if UDFs are used
+                        # Therefore we just return the entire document
+                        return "doc"
+
+            return f"""
+                MERGE(
+                    {{ _key: doc._key, _from: doc._from, _to: doc._to }},
+                    KEEP(doc, {list(attributes)})
+                )
+            """
 
         with progress(
             f"(ADB → PyG): {col}",
             text_style="#8929C2",
             spinner_style="#40A6F5",
         ) as p:
             p.add_task("__fetch_adb_docs")
-
-            return DataFrame(
-                self.__db.aql.execute(
-                    aql, count=True, bind_vars={"@col": col}, **query_options
-                )
+            return self.__db.aql.execute(  # type: ignore
+                f"FOR doc IN @@col RETURN {get_aql_return_value(meta)}",
+                bind_vars={"@col": col},
+                **{**{"stream": True}, **query_options},
             )
 
     def __insert_adb_docs(
         self, doc_type: Union[str, EdgeType], df: DataFrame, kwargs: Any
     ) -> None:
         """Insert ArangoDB documents into their ArangoDB collection.
 
@@ -713,14 +821,19 @@
             spinner_style="#994602",
         ) as p:
             p.add_task("__insert_adb_docs")
 
             docs = df.to_dict("records")
             result = self.__db.collection(col).import_bulk(docs, **kwargs)
             logger.debug(result)
+            df.drop(df.index, inplace=True)
+
+    def __split_adb_ids(self, s: Series) -> Series:
+        """Helper method to split the ArangoDB IDs within a Series into two columns"""
+        return s.str.split(pat="/", n=1, expand=True)
 
     def __set_pyg_data(
         self,
         meta: Union[Set[str], Dict[str, ADBMetagraphValues]],
         pyg_data: Union[Data, NodeStorage, EdgeStorage],
         df: DataFrame,
     ) -> None:
@@ -738,21 +851,32 @@
         :param df: The DataFrame representing the ArangoDB collection data
         :type df: pandas.DataFrame
         """
         valid_meta: Dict[str, ADBMetagraphValues]
         valid_meta = meta if type(meta) is dict else {m: m for m in meta}
 
         for k, v in valid_meta.items():
-            pyg_data[k] = self.__build_tensor_from_dataframe(df, k, v)
+            t = self.__build_tensor_from_dataframe(df, k, v)
+
+            if k not in pyg_data:
+                pyg_data[k] = t
+            elif isinstance(pyg_data[k], Tensor):
+                pyg_data[k] = cat((pyg_data[k], t))
+            else:  # pragma: no cover
+                m = f"'{k}' key in PyG Data must point to a Tensor"
+                raise TypeError(m)
 
     def __set_adb_data(
         self,
         df: DataFrame,
         meta: Union[Set[str], Dict[Any, PyGMetagraphValues]],
         pyg_data: Union[Data, NodeStorage, EdgeStorage],
+        pyg_data_size: int,
+        start_index: int,
+        end_index: int,
         explicit_metagraph: bool,
     ) -> DataFrame:
         """A helper method to build the ArangoDB Dataframe for the given
         collection. Is responsible for creating "sub-DataFrames" from PyG tensors
         or lists, and appending them to the main dataframe **df**. If the data
         does not adhere to the supported types, or is not of specific length,
         then it is silently skipped.
@@ -762,14 +886,22 @@
         :type df: pandas.DataFrame
         :param meta: The metagraph associated to the
             current PyG node or edge type. e.g metagraph['nodeTypes']['v0']
         :type meta: Set[str] | Dict[Any, adbpyg_adapter.typings.PyGMetagraphValues]
         :param pyg_data: The NodeStorage or EdgeStorage of the current
             PyG node or edge type.
         :type pyg_data: torch_geometric.data.storage.(NodeStorage | EdgeStorage)
+        :param pyg_data_size: The size of the NodeStorage or EdgeStorage of the
+            current PyG node or edge type.
+        :type pyg_data_size: int
+        :param start_index: The starting index of the current batch to process.
+        :type start_index: int
+        :param end_index: The ending index of the current batch to process.
+        :type end_index: int
+        :type pyg_data: torch_geometric.data.storage.(NodeStorage | EdgeStorage)
         :param explicit_metagraph: The value of **explicit_metagraph**
             in **pyg_to_arangodb**.
         :type explicit_metagraph: bool
         :return: The completed DataFrame for the (soon-to-be) ArangoDB collection.
         :rtype: pandas.DataFrame
         :raise ValueError: If an unsupported PyG data value is found.
         """
@@ -779,32 +911,42 @@
 
         valid_meta: Dict[Any, PyGMetagraphValues]
         valid_meta = meta if type(meta) is dict else {m: m for m in meta}
 
         if explicit_metagraph:
             pyg_keys = set(valid_meta.keys())
         else:
-            # can't do keys() (not compatible with Homogeneous graphs)
+            # can't do pyg_data.keys() (not compatible with Homogeneous graphs)
             pyg_keys = set(k for k, _ in pyg_data.items())
 
-        for k in pyg_keys:
-            if k == "edge_index":
+        for meta_key in pyg_keys:
+            if meta_key == "edge_index":
                 continue
 
-            data = pyg_data[k]
-            meta_val = valid_meta.get(k, str(k))
+            data = pyg_data[meta_key]
+            meta_val = valid_meta.get(meta_key, str(meta_key))
 
-            if type(meta_val) is str and type(data) is list and len(data) == len(df):
-                if meta_val in ["_v_key", "_e_key"]:  # Homogeneous situation
-                    meta_val = "_key"
-
-                df = df.join(DataFrame(data, columns=[meta_val]))
+            if (
+                type(meta_val) is str
+                and type(data) is list
+                and len(data) == pyg_data_size
+            ):
+                meta_val = "_key" if meta_val in ["_v_key", "_e_key"] else meta_val
+                df = df.join(DataFrame(data[start_index:end_index], columns=[meta_val]))
 
-            if type(data) is Tensor and len(data) == len(df):
-                df = df.join(self.__build_dataframe_from_tensor(data, k, meta_val))
+            if type(data) is Tensor and len(data) == pyg_data_size:
+                df = df.join(
+                    self.__build_dataframe_from_tensor(
+                        data[start_index:end_index],
+                        start_index,
+                        end_index,
+                        meta_key,
+                        meta_val,
+                    )
+                )
 
         return df
 
     def __build_tensor_from_dataframe(
         self,
         adb_df: DataFrame,
         meta_key: str,
@@ -842,36 +984,42 @@
                 else:  # pragma: no cover
                     msg = f"Invalid encoder for ArangoDB attribute '{attr}': {encoder}"
                     raise ADBMetagraphError(msg)
 
             return cat(data, dim=-1)
 
         if callable(meta_val):
-            # **meta_val** is a user-defined that returns a tensor
+            # **meta_val** is a user-defined function that returns a tensor
             user_defined_result = meta_val(adb_df)
 
             if type(user_defined_result) is not Tensor:  # pragma: no cover
                 msg = f"Invalid return type for function {meta_val} ('{meta_key}')"
                 raise ADBMetagraphError(msg)
 
             return user_defined_result
 
         raise ADBMetagraphError(f"Invalid {meta_val} type")  # pragma: no cover
 
     def __build_dataframe_from_tensor(
         self,
         pyg_tensor: Tensor,
+        start_index: int,
+        end_index: int,
         meta_key: Any,
         meta_val: PyGMetagraphValues,
     ) -> DataFrame:
         """Builds a DataFrame from PyG Tensor, based on
         the nature of the user-defined metagraph.
 
         :param pyg_tensor: The Tensor representing PyG data.
         :type pyg_tensor: torch.Tensor
+        :param start_index: The starting index of the current batch to process.
+        :type start_index: int
+        :param end_index: The ending index of the current batch to process.
+        :type end_index: int
         :param meta_key: The current PyG-ArangoDB metagraph key
         :type meta_key: Any
         :param meta_val: The value mapped to the PyG-ArangoDB metagraph key to
             help convert **tensor** into a DataFrame.
             e.g the value of `metagraph['nodeTypes']['users']['x']`.
         :type meta_val: adbpyg_adapter.typings.PyGMetagraphValues
         :return: A DataFrame equivalent to the Tensor
@@ -879,36 +1027,51 @@
         :raise adbpyg_adapter.exceptions.PyGMetagraphError: If invalid **meta_val**.
         """
         logger.debug(
             f"__build_dataframe_from_tensor(df, '{meta_key}', {type(meta_val)})"
         )
 
         if type(meta_val) is str:
-            df = DataFrame(columns=[meta_val])
+            df = DataFrame(index=range(start_index, end_index), columns=[meta_val])
             df[meta_val] = pyg_tensor.tolist()
             return df
 
         if type(meta_val) is list:
             num_features = pyg_tensor.size()[1]
             if len(meta_val) != num_features:  # pragma: no cover
                 msg = f"""
                     Invalid list length for **meta_val** ('{meta_key}'):
                     List length must match the number of
                     features found in the tensor ({num_features}).
                 """
                 raise PyGMetagraphError(msg)
 
-            df = DataFrame(columns=meta_val)
+            df = DataFrame(index=range(start_index, end_index), columns=meta_val)
             df[meta_val] = pyg_tensor.tolist()
             return df
 
         if callable(meta_val):
-            # **meta_val** is a user-defined function that returns a dataframe
-            user_defined_result = meta_val(pyg_tensor)
+            # **meta_val** is a user-defined function that populates
+            # and returns the empty dataframe
+            empty_df = DataFrame(index=range(start_index, end_index))
+            user_defined_result = meta_val(pyg_tensor, empty_df)
 
-            if type(user_defined_result) is not DataFrame:  # pragma: no cover
-                msg = f"Invalid return type for function {meta_val} ('{meta_key}')"
+            if not isinstance(user_defined_result, DataFrame):  # pragma: no cover
+                msg = f"""
+                    Invalid return type for function {meta_val} ('{meta_key}').
+                    Function must return Pandas DataFrame.
+                """
+                raise PyGMetagraphError(msg)
+
+            if (
+                user_defined_result.index.start != start_index
+                or user_defined_result.index.stop != end_index
+            ):  # pragma: no cover
+                msg = f"""
+                    User Defined Function {meta_val} ('{meta_key}') must return
+                    DataFrame with start index {start_index} & stop index {end_index}
+                """
                 raise PyGMetagraphError(msg)
 
             return user_defined_result
 
         raise PyGMetagraphError(f"Invalid {meta_val} type")  # pragma: no cover
```

### Comparing `adbpyg_adapter-1.1.0/adbpyg_adapter/controller.py` & `adbpyg_adapter-1.1.1/adbpyg_adapter/controller.py`

 * *Files identical despite different names*

### Comparing `adbpyg_adapter-1.1.0/adbpyg_adapter/encoders.py` & `adbpyg_adapter-1.1.1/adbpyg_adapter/encoders.py`

 * *Files identical despite different names*

### Comparing `adbpyg_adapter-1.1.0/adbpyg_adapter/typings.py` & `adbpyg_adapter-1.1.1/adbpyg_adapter/typings.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,27 +4,29 @@
     "ADBMetagraphValues",
     "PyGMetagraph",
     "PyGMetagraphValues",
     "ADBMap",
     "PyGMap",
 ]
 
-from typing import Any, Callable, DefaultDict, Dict, List, Tuple, Union
+from typing import Any, Callable, DefaultDict, Dict, List, Set, Tuple, Union
 
 from pandas import DataFrame
 from torch import Tensor
 
 Json = Dict[str, Any]
 
 DataFrameToTensor = Callable[[DataFrame], Tensor]
-TensorToDataFrame = Callable[[Tensor], DataFrame]
+TensorToDataFrame = Callable[[Tensor, DataFrame], DataFrame]
 
 ADBEncoders = Dict[str, DataFrameToTensor]
 ADBMetagraphValues = Union[str, DataFrameToTensor, ADBEncoders]
-ADBMetagraph = Dict[str, Dict[str, Dict[str, ADBMetagraphValues]]]
+ADBMetagraph = Dict[str, Dict[str, Union[Set[str], Dict[str, ADBMetagraphValues]]]]
 
 PyGDataTypes = Union[str, Tuple[str, str, str]]
 PyGMetagraphValues = Union[str, List[str], TensorToDataFrame]
-PyGMetagraph = Dict[str, Dict[PyGDataTypes, Dict[Any, PyGMetagraphValues]]]
+PyGMetagraph = Dict[
+    str, Dict[PyGDataTypes, Union[Set[str], Dict[Any, PyGMetagraphValues]]]
+]
 
 ADBMap = DefaultDict[PyGDataTypes, Dict[str, int]]
 PyGMap = DefaultDict[PyGDataTypes, Dict[int, str]]
```

### Comparing `adbpyg_adapter-1.1.0/adbpyg_adapter/utils.py` & `adbpyg_adapter-1.1.1/adbpyg_adapter/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,14 @@
             for elem in edge_type:
                 if type(elem) != str:
                     msg = f"{elem} in {edge_type} must be str"
                     raise PyGMetagraphError(msg)
 
     for parent_key in ["nodeTypes", "edgeTypes"]:
         for k, meta in metagraph.get(parent_key, {}).items():
-
             if type(meta) == set:
                 for m in meta:
                     if type(m) != str:
                         msg = f"""
                             Invalid set value type for {meta}:
                             {m} must be str
                         """
```

### Comparing `adbpyg_adapter-1.1.0/adbpyg_adapter.egg-info/PKG-INFO` & `adbpyg_adapter-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,288 +1,297 @@
 Metadata-Version: 2.1
-Name: adbpyg-adapter
-Version: 1.1.0
+Name: adbpyg_adapter
+Version: 1.1.1
 Summary: Convert ArangoDB graphs to PyG & vice-versa.
 Home-page: https://github.com/arangoml/pyg-adapter
 Author: Anthony Mahanna
 Author-email: anthony.mahanna@arangodb.com
 License: Apache Software License
-Keywords: arangodb,pyg,adapter
+Description: # ArangoDB-PyG Adapter
+        
+        [![build](https://github.com/arangoml/pyg-adapter/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/arangoml/pyg-adapter/actions/workflows/build.yml)
+        [![CodeQL](https://github.com/arangoml/pyg-adapter/actions/workflows/analyze.yml/badge.svg?branch=master)](https://github.com/arangoml/pyg-adapter/actions/workflows/analyze.yml)
+        [![Coverage Status](https://coveralls.io/repos/github/arangoml/pyg-adapter/badge.svg?branch=master)](https://coveralls.io/github/arangoml/pyg-adapter)
+        [![Last commit](https://img.shields.io/github/last-commit/arangoml/pyg-adapter)](https://github.com/arangoml/pyg-adapter/commits/master)
+        
+        [![PyPI version badge](https://img.shields.io/pypi/v/adbpyg-adapter?color=3775A9&style=for-the-badge&logo=pypi&logoColor=FFD43B)](https://pypi.org/project/adbpyg-adapter/)
+        [![Python versions badge](https://img.shields.io/pypi/pyversions/adbpyg-adapter?color=3776AB&style=for-the-badge&logo=python&logoColor=FFD43B)](https://pypi.org/project/adbpyg-adapter/)
+        
+        [![License](https://img.shields.io/github/license/arangoml/pyg-adapter?color=9E2165&style=for-the-badge)](https://github.com/arangoml/pyg-adapter/blob/master/LICENSE)
+        [![Code style: black](https://img.shields.io/static/v1?style=for-the-badge&label=code%20style&message=black&color=black)](https://github.com/psf/black)
+        [![Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&color=282661&label=Downloads&query=total_downloads&url=https://api.pepy.tech/api/v2/projects/adbpyg-adapter)](https://pepy.tech/project/adbpyg-adapter)
+        
+        
+        <a href="https://www.arangodb.com/" rel="arangodb.com">![](https://raw.githubusercontent.com/arangoml/pyg-adapter/master/examples/assets/adb_logo.png)</a>
+        <a href="https://www.pyg.org/" rel="pyg.org"><img src="https://raw.githubusercontent.com/pyg-team/pyg_sphinx_theme/master/pyg_sphinx_theme/static/img/pyg_logo_text.svg?sanitize=true" width=40% /></a>
+        
+        The ArangoDB-PyG Adapter exports Graphs from ArangoDB, the multi-model database for graph & beyond, into PyTorch Geometric (PyG), a PyTorch-based Graph Neural Network library, and vice-versa.
+        
+        ## About PyG
+        
+        **PyG** *(PyTorch Geometric)* is a library built upon [PyTorch](https://pytorch.org/) to easily write and train Graph Neural Networks (GNNs) for a wide range of applications related to structured data.
+        
+        It consists of various methods for deep learning on graphs and other irregular structures, also known as *[geometric deep learning](http://geometricdeeplearning.com/)*, from a variety of published papers.
+        In addition, it consists of easy-to-use mini-batch loaders for operating on many small and single giant graphs, [multi GPU-support](https://github.com/pyg-team/pytorch_geometric/tree/master/examples/multi_gpu), [`DataPipe` support](https://github.com/pyg-team/pytorch_geometric/blob/master/examples/datapipe.py), distributed graph learning via [Quiver](https://github.com/pyg-team/pytorch_geometric/tree/master/examples/quiver), a large number of common benchmark datasets (based on simple interfaces to create your own), the [GraphGym](https://pytorch-geometric.readthedocs.io/en/latest/notes/graphgym.html) experiment manager, and helpful transforms, both for learning on arbitrary graphs as well as on 3D meshes or point clouds.
+        
+        ## Installation
+        
+        #### Latest Release
+        ```
+        pip install torch
+        pip install adbpyg-adapter
+        ```
+        #### Current State
+        ```
+        pip install torch
+        pip install git+https://github.com/arangoml/pyg-adapter.git
+        ```
+        
+        ##  Quickstart
+        
+        [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/arangoml/pyg-adapter/blob/master/examples/ArangoDB_PyG_Adapter.ipynb)
+        
+        Also available as an ArangoDB Lunch & Learn session on YouTube: [Graph & Beyond Course: ArangoDB-PyG Adapter](https://www.youtube.com/watch?v=QtGR95NN8bA)
+        
+        ```py
+        import torch
+        import pandas
+        from torch_geometric.datasets import FakeHeteroDataset
+        
+        from arango import ArangoClient  # Python-Arango driver
+        
+        from adbpyg_adapter import ADBPyG_Adapter, ADBPyG_Controller
+        from adbpyg_adapter.encoders import IdentityEncoder, CategoricalEncoder
+        
+        # Load some fake PyG data for demo purposes
+        data = FakeHeteroDataset(
+            num_node_types=2,
+            num_edge_types=3,
+            avg_num_nodes=20,
+            avg_num_channels=3,  # avg number of features per node
+            edge_dim=2,  # number of features per edge
+            num_classes=3,  # number of unique label values
+        )[0]
+        
+        # Let's assume that the ArangoDB "IMDB" dataset is imported to this endpoint
+        db = ArangoClient(hosts="http://localhost:8529").db("_system", username="root", password="")
+        
+        adbpyg_adapter = ADBPyG_Adapter(db)
+        ```
+        
+        ### PyG to ArangoDB
+        
+        Note: If the PyG graph contains `_key`, `_v_key`, or `_e_key` properties for any node / edge types, the adapter will assume to persist those values as [ArangoDB document keys](https://www.arangodb.com/docs/stable/data-modeling-naming-conventions-document-keys.html). See the `Full Cycle (ArangoDB -> PyG -> ArangoDB)` section below for an example.
+        
+        ```py
+        # 1.1: PyG to ArangoDB
+        adb_g = adbpyg_adapter.pyg_to_arangodb("FakeData", data)
+        
+        # 1.2: PyG to ArangoDB with a (completely optional) metagraph for customized adapter behaviour
+        def y_tensor_to_2_column_dataframe(pyg_tensor, adb_df):
+            """
+            A user-defined function to create two
+            ArangoDB attributes out of the 'user' label tensor
+        
+            :param dgl_tensor: The DGL Tensor containing the data
+            :type dgl_tensor: torch.Tensor
+            :param adb_df: The ArangoDB DataFrame to populate, whose
+                size is preset to the length of **dgl_tensor**.
+            :type adb_df: pandas.DataFrame
+        
+            NOTE: user-defined functions must return the modified **adb_df**
+            """
+            label_map = {0: "Kiwi", 1: "Blueberry", 2: "Avocado"}
+        
+            adb_df["label_num"] = pyg_tensor.tolist()
+            adb_df["label_str"] = adb_df["label_num"].map(label_map)
+        
+            return adb_df
+        
+        
+        metagraph = {
+            "nodeTypes": {
+                "v0": {
+                    "x": "features",  # 1) You can specify a string value if you want to rename your PyG data when stored in ArangoDB
+                    "y": y_tensor_to_2_column_dataframe,  # 2) you can specify a function for user-defined handling, as long as the function returns a Pandas DataFrame
+                },
+                # 3) You can specify set of strings if you want to preserve the same PyG attribute names for the node/edge type
+                "v1": {"x"} # this is equivalent to {"x": "x"}
+            },
+            "edgeTypes": {
+                ("v0", "e0", "v0"): {
+                    # 4) You can specify a list of strings for tensor dissasembly (if you know the number of node/edge features in advance)
+                    "edge_attr": [ "a", "b"]  
+                },
+            },
+        }
+        
+        
+        adb_g = adbpyg_adapter.pyg_to_arangodb("FakeData", data, metagraph, explicit_metagraph=False)
+        
+        # 1.3: PyG to ArangoDB with the same (optional) metagraph, but with `explicit_metagraph=True`
+        # With `explicit_metagraph=True`, the node & edge types omitted from the metagraph will NOT be converted to ArangoDB.
+        # Only 'v0', 'v1' and ('v0', 'e0', 'v0') will be brought over (i.e 'v2', ('v0', 'e0', 'v1'), ... are ignored)
+        adb_g = adbpyg_adapter.pyg_to_arangodb("FakeData", data, metagraph, explicit_metagraph=True)
+        
+        # 1.4: PyG to ArangoDB with a Custom Controller  (more user-defined behavior)
+        class Custom_ADBPyG_Controller(ADBPyG_Controller):
+            def _prepare_pyg_node(self, pyg_node: dict, node_type: str) -> dict:
+                """Optionally modify a PyG node object before it gets inserted into its designated ArangoDB collection.
+        
+                :param pyg_node: The PyG node object to (optionally) modify.
+                :param node_type: The PyG Node Type of the node.
+                :return: The PyG Node object
+                """
+                pyg_node["foo"] = "bar"
+                return pyg_node
+        
+            def _prepare_pyg_edge(self, pyg_edge: dict, edge_type: tuple) -> dict:
+                """Optionally modify a PyG edge object before it gets inserted into its designated ArangoDB collection.
+        
+                :param pyg_edge: The PyG edge object to (optionally) modify.
+                :param edge_type: The Edge Type of the PyG edge. Formatted
+                    as (from_collection, edge_collection, to_collection)
+                :return: The PyG Edge object
+                """
+                pyg_edge["bar"] = "foo"
+                return pyg_edge
+        
+        
+        adb_g = ADBPyG_Adapter(db, Custom_ADBPyG_Controller()).pyg_to_arangodb("FakeData", data)
+        ```
+        
+        ### ArangoDB to PyG
+        ```py
+        # Start from scratch!
+        db.delete_graph("FakeData", drop_collections=True, ignore_missing=True)
+        adbpyg_adapter.pyg_to_arangodb("FakeData", data)
+        
+        # 2.1: ArangoDB to PyG via Graph name (does not transfer attributes)
+        pyg_g = adbpyg_adapter.arangodb_graph_to_pyg("FakeData")
+        
+        # 2.2: ArangoDB to PyG via Collection names (does not transfer attributes)
+        pyg_g = adbpyg_adapter.arangodb_collections_to_pyg("FakeData", v_cols={"v0", "v1"}, e_cols={"e0"})
+        
+        # 2.3: ArangoDB to PyG via Metagraph v1 (transfer attributes "as is", meaning they are already formatted to PyG data standards)
+        metagraph_v1 = {
+            "vertexCollections": {
+                # Move the "x" & "y" ArangoDB attributes to PyG as "x" & "y" Tensors
+                "v0": {"x", "y"}, # equivalent to {"x": "x", "y": "y"}
+                "v1": {"v1_x": "x"}, # store the 'x' feature matrix as 'v1_x' in PyG
+            },
+            "edgeCollections": {
+                "e0": {"edge_attr"},
+            },
+        }
+        pyg_g = adbpyg_adapter.arangodb_to_pyg("FakeData", metagraph_v1)
+        
+        # 2.4: ArangoDB to PyG via Metagraph v2 (transfer attributes via user-defined encoders)
+        # For more info on user-defined encoders in PyG, see https://pytorch-geometric.readthedocs.io/en/latest/notes/load_csv.html
+        metagraph_v2 = {
+            "vertexCollections": {
+                "Movies": {
+                    "x": {  # Build a feature matrix from the "Action" & "Drama" document attributes
+                        "Action": IdentityEncoder(dtype=torch.long),
+                        "Drama": IdentityEncoder(dtype=torch.long),
+                    },
+                    "y": "Comedy",
+                },
+                "Users": {
+                    "x": {
+                        "Gender": CategoricalEncoder(mapping={"M": 0, "F": 1}),
+                        "Age": IdentityEncoder(dtype=torch.long),
+                    }
+                },
+            },
+            "edgeCollections": {
+                "Ratings": { "edge_weight": "Rating" } # Use the 'Rating' attribute for the PyG 'edge_weight' property
+            },
+        }
+        pyg_g = adbpyg_adapter.arangodb_to_pyg("IMDB", metagraph_v2)
+        
+        # 2.5: ArangoDB to PyG via Metagraph v3 (transfer attributes via user-defined functions)
+        def udf_v0_x(v0_df):
+            # process v0_df here to return v0 "x" feature matrix
+            # v0_df["x"] = ...
+            return torch.tensor(v0_df["x"].to_list())
+        
+        
+        def udf_v1_x(v1_df):
+            # process v1_df here to return v1 "x" feature matrix
+            # v1_df["x"] = ...
+            return torch.tensor(v1_df["x"].to_list())
+        
+        
+        metagraph_v3 = {
+            "vertexCollections": {
+                "v0": {
+                    "x": udf_v0_x,  # supports named functions
+                    "y": lambda df: torch.tensor(df["y"].to_list()),  # also supports lambda functions
+                },
+                "v1": {"x": udf_v1_x},
+            },
+            "edgeCollections": {
+                "e0": {"edge_attr": (lambda df: torch.tensor(df["edge_attr"].to_list()))},
+            },
+        }
+        pyg_g = adbpyg_adapter.arangodb_to_pyg("FakeData", metagraph_v3)
+        ```
+        
+        ### Experimental: `preserve_adb_keys`
+        ```py
+        # With `preserve_adb_keys=True`, the adapter will preserve the ArangoDB vertex & edge _key values into the (newly created) PyG graph.
+        # Users can then re-import their PyG graph into ArangoDB using the same _key values 
+        pyg_g = adbpyg_adapter.arangodb_graph_to_pyg("imdb", preserve_adb_keys=True)
+        
+        # pyg_g["Movies"]["_key"] --> ["1", "2", ..., "1682"]
+        # pyg_g["Users"]["_key"] --> ["1", "2", ..., "943"]
+        # pyg_g[("Users", "Ratings", "Movies")]["_key"] --> ["2732620466", ..., "2730643624"]
+        
+        # Let's add a new PyG User Node by updating the _key property
+        pyg_g["Users"]["_key"].append("new-user-here-944")
+        
+        # Note: Prior to the re-import, we must manually set the number of nodes in the PyG graph, since the `arangodb_graph_to_pyg` API creates featureless node data
+        pyg_g["Movies"].num_nodes = len(pyg_g["Movies"]["_key"]) # 1682
+        pyg_g["Users"].num_nodes = len(pyg_g["Users"]["_key"]) # 944 (prev. 943)
+        
+        # Re-import PyG graph into ArangoDB
+        adbpyg_adapter.pyg_to_arangodb("imdb", pyg_g, on_duplicate="update")
+        ```
+        
+        ##  Development & Testing
+        
+        Prerequisite: `arangorestore`
+        
+        1. `git clone https://github.com/arangoml/pyg-adapter.git`
+        2. `cd pyg-adapter`
+        3. (create virtual environment of choice)
+        4. `pip install torch`
+        5. `pip install -e .[dev]`
+        6. (create an ArangoDB instance with method of choice)
+        7. `pytest --url <> --dbName <> --username <> --password <>`
+        
+        **Note**: A `pytest` parameter can be omitted if the endpoint is using its default value:
+        ```python
+        def pytest_addoption(parser):
+            parser.addoption("--url", action="store", default="http://localhost:8529")
+            parser.addoption("--dbName", action="store", default="_system")
+            parser.addoption("--username", action="store", default="root")
+            parser.addoption("--password", action="store", default="")
+        ```
+        
+Keywords: arangodb,pyg,pytorch,pytorch geometric,adapter
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-License-File: LICENSE
-
-# ArangoDB-PyG Adapter
-
-[![build](https://github.com/arangoml/pyg-adapter/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/arangoml/pyg-adapter/actions/workflows/build.yml)
-[![CodeQL](https://github.com/arangoml/pyg-adapter/actions/workflows/analyze.yml/badge.svg?branch=master)](https://github.com/arangoml/pyg-adapter/actions/workflows/analyze.yml)
-[![Coverage Status](https://coveralls.io/repos/github/arangoml/pyg-adapter/badge.svg?branch=master)](https://coveralls.io/github/arangoml/pyg-adapter)
-[![Last commit](https://img.shields.io/github/last-commit/arangoml/pyg-adapter)](https://github.com/arangoml/pyg-adapter/commits/master)
-
-[![PyPI version badge](https://img.shields.io/pypi/v/adbpyg-adapter?color=3775A9&style=for-the-badge&logo=pypi&logoColor=FFD43B)](https://pypi.org/project/adbpyg-adapter/)
-[![Python versions badge](https://img.shields.io/pypi/pyversions/adbpyg-adapter?color=3776AB&style=for-the-badge&logo=python&logoColor=FFD43B)](https://pypi.org/project/adbpyg-adapter/)
-
-[![License](https://img.shields.io/github/license/arangoml/pyg-adapter?color=9E2165&style=for-the-badge)](https://github.com/arangoml/pyg-adapter/blob/master/LICENSE)
-[![Code style: black](https://img.shields.io/static/v1?style=for-the-badge&label=code%20style&message=black&color=black)](https://github.com/psf/black)
-[![Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&color=282661&label=Downloads&query=total_downloads&url=https://api.pepy.tech/api/projects/adbpyg-adapter)](https://pepy.tech/project/adbpyg-adapter)
-
-
-<a href="https://www.arangodb.com/" rel="arangodb.com">![](https://raw.githubusercontent.com/arangoml/pyg-adapter/master/examples/assets/adb_logo.png)</a>
-<a href="https://www.pyg.org/" rel="pyg.org"><img src="https://raw.githubusercontent.com/pyg-team/pyg_sphinx_theme/master/pyg_sphinx_theme/static/img/pyg_logo_text.svg?sanitize=true" width=40% /></a>
-
-The ArangoDB-PyG Adapter exports Graphs from ArangoDB, the multi-model database for graph & beyond, into PyTorch Geometric (PyG), a PyTorch-based Graph Neural Network library, and vice-versa.
-
-## About PyG
-
-**PyG** *(PyTorch Geometric)* is a library built upon [PyTorch](https://pytorch.org/) to easily write and train Graph Neural Networks (GNNs) for a wide range of applications related to structured data.
-
-It consists of various methods for deep learning on graphs and other irregular structures, also known as *[geometric deep learning](http://geometricdeeplearning.com/)*, from a variety of published papers.
-In addition, it consists of easy-to-use mini-batch loaders for operating on many small and single giant graphs, [multi GPU-support](https://github.com/pyg-team/pytorch_geometric/tree/master/examples/multi_gpu), [`DataPipe` support](https://github.com/pyg-team/pytorch_geometric/blob/master/examples/datapipe.py), distributed graph learning via [Quiver](https://github.com/pyg-team/pytorch_geometric/tree/master/examples/quiver), a large number of common benchmark datasets (based on simple interfaces to create your own), the [GraphGym](https://pytorch-geometric.readthedocs.io/en/latest/notes/graphgym.html) experiment manager, and helpful transforms, both for learning on arbitrary graphs as well as on 3D meshes or point clouds.
-
-## Installation
-
-#### Latest Release
-```
-pip install torch
-pip install adbpyg-adapter
-```
-#### Current State
-```
-pip install torch
-pip install git+https://github.com/arangoml/pyg-adapter.git
-```
-
-##  Quickstart
-
-[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/arangoml/pyg-adapter/blob/master/examples/ArangoDB_PyG_Adapter.ipynb)
-
-```py
-import torch
-import pandas
-from torch_geometric.datasets import FakeHeteroDataset
-
-from arango import ArangoClient  # Python-Arango driver
-
-from adbpyg_adapter import ADBPyG_Adapter, ADBPyG_Controller
-from adbpyg_adapter.encoders import IdentityEncoder, CategoricalEncoder
-
-# Load some fake PyG data for demo purposes
-data = FakeHeteroDataset(
-    num_node_types=2,
-    num_edge_types=3,
-    avg_num_nodes=20,
-    avg_num_channels=3,  # avg number of features per node
-    edge_dim=2,  # number of features per edge
-    num_classes=3,  # number of unique label values
-)[0]
-
-# Let's assume that the ArangoDB "IMDB" dataset is imported to this endpoint
-db = ArangoClient(hosts="http://localhost:8529").db("_system", username="root", password="")
-
-adbpyg_adapter = ADBPyG_Adapter(db)
-```
-
-### PyG to ArangoDB
-
-Note: If the PyG graph contains `_key`, `_v_key`, or `_e_key` properties for any node / edge types, the adapter will assume to persist those values as [ArangoDB document keys](https://www.arangodb.com/docs/stable/data-modeling-naming-conventions-document-keys.html). See the `Full Cycle (ArangoDB -> PyG -> ArangoDB)` section below for an example.
-
-```py
-# 1.1: PyG to ArangoDB
-adb_g = adbpyg_adapter.pyg_to_arangodb("FakeData", data)
-
-# 1.2: PyG to ArangoDB with a (completely optional) metagraph for customized adapter behaviour
-def y_tensor_to_2_column_dataframe(pyg_tensor):
-    """
-    A user-defined function to create two
-    ArangoDB attributes out of the 'y' label tensor
-
-    NOTE: user-defined functions must return a Pandas Dataframe
-    """
-    label_map = {0: "Kiwi", 1: "Blueberry", 2: "Avocado"}
-
-    df = pandas.DataFrame(columns=["label_num", "label_str"])
-    df["label_num"] = pyg_tensor.tolist()
-    df["label_str"] = df["label_num"].map(label_map)
-
-    return df
-
-
-metagraph = {
-    "nodeTypes": {
-        "v0": {
-            "x": "features",  # 1) You can specify a string value if you want to rename your PyG data when stored in ArangoDB
-            "y": y_tensor_to_2_column_dataframe,  # 2) you can specify a function for user-defined handling, as long as the function returns a Pandas DataFrame
-        },
-        # 3) You can specify set of strings if you want to preserve the same PyG attribute names for the node/edge type
-        "v1": {"x"} # this is equivalent to {"x": "x"}
-    },
-    "edgeTypes": {
-        ("v0", "e0", "v0"): {
-            # 4) You can specify a list of strings for tensor dissasembly (if you know the number of node/edge features in advance)
-            "edge_attr": [ "a", "b"]  
-        },
-    },
-}
-
-
-adb_g = adbpyg_adapter.pyg_to_arangodb("FakeData", data, metagraph, explicit_metagraph=False)
-
-# 1.3: PyG to ArangoDB with the same (optional) metagraph, but with `explicit_metagraph=True`
-# With `explicit_metagraph=True`, the node & edge types omitted from the metagraph will NOT be converted to ArangoDB.
-# Only 'v0', 'v1' and ('v0', 'e0', 'v0') will be brought over (i.e 'v2', ('v0', 'e0', 'v1'), ... are ignored)
-adb_g = adbpyg_adapter.pyg_to_arangodb("FakeData", data, metagraph, explicit_metagraph=True)
-
-# 1.4: PyG to ArangoDB with a Custom Controller  (more user-defined behavior)
-class Custom_ADBPyG_Controller(ADBPyG_Controller):
-    def _prepare_pyg_node(self, pyg_node: dict, node_type: str) -> dict:
-        """Optionally modify a PyG node object before it gets inserted into its designated ArangoDB collection.
-
-        :param pyg_node: The PyG node object to (optionally) modify.
-        :param node_type: The PyG Node Type of the node.
-        :return: The PyG Node object
-        """
-        pyg_node["foo"] = "bar"
-        return pyg_node
-
-    def _prepare_pyg_edge(self, pyg_edge: dict, edge_type: tuple) -> dict:
-        """Optionally modify a PyG edge object before it gets inserted into its designated ArangoDB collection.
-
-        :param pyg_edge: The PyG edge object to (optionally) modify.
-        :param edge_type: The Edge Type of the PyG edge. Formatted
-            as (from_collection, edge_collection, to_collection)
-        :return: The PyG Edge object
-        """
-        pyg_edge["bar"] = "foo"
-        return pyg_edge
-
-
-adb_g = ADBPyG_Adapter(db, Custom_ADBPyG_Controller()).pyg_to_arangodb("FakeData", data)
-```
-
-### ArangoDB to PyG
-```py
-# Start from scratch!
-db.delete_graph("FakeData", drop_collections=True, ignore_missing=True)
-adbpyg_adapter.pyg_to_arangodb("FakeData", data)
-
-# 2.1: ArangoDB to PyG via Graph name (does not transfer attributes)
-pyg_g = adbpyg_adapter.arangodb_graph_to_pyg("FakeData")
-
-# 2.2: ArangoDB to PyG via Collection names (does not transfer attributes)
-pyg_g = adbpyg_adapter.arangodb_collections_to_pyg("FakeData", v_cols={"v0", "v1"}, e_cols={"e0"})
-
-# 2.3: ArangoDB to PyG via Metagraph v1 (transfer attributes "as is", meaning they are already formatted to PyG data standards)
-metagraph_v1 = {
-    "vertexCollections": {
-        # Move the "x" & "y" ArangoDB attributes to PyG as "x" & "y" Tensors
-        "v0": {"x", "y"}, # equivalent to {"x": "x", "y": "y"}
-        "v1": {"v1_x": "x"}, # store the 'x' feature matrix as 'v1_x' in PyG
-    },
-    "edgeCollections": {
-        "e0": {"edge_attr"},
-    },
-}
-pyg_g = adbpyg_adapter.arangodb_to_pyg("FakeData", metagraph_v1)
-
-# 2.4: ArangoDB to PyG via Metagraph v2 (transfer attributes via user-defined encoders)
-# For more info on user-defined encoders in PyG, see https://pytorch-geometric.readthedocs.io/en/latest/notes/load_csv.html
-metagraph_v2 = {
-    "vertexCollections": {
-        "Movies": {
-            "x": {  # Build a feature matrix from the "Action" & "Drama" document attributes
-                "Action": IdentityEncoder(dtype=torch.long),
-                "Drama": IdentityEncoder(dtype=torch.long),
-            },
-            "y": "Comedy",
-        },
-        "Users": {
-            "x": {
-                "Gender": CategoricalEncoder(mapping={"M": 0, "F": 1}),
-                "Age": IdentityEncoder(dtype=torch.long),
-            }
-        },
-    },
-    "edgeCollections": {
-        "Ratings": { "edge_weight": "Rating" } # Use the 'Rating' attribute for the PyG 'edge_weight' property
-    },
-}
-pyg_g = adbpyg_adapter.arangodb_to_pyg("IMDB", metagraph_v2)
-
-# 2.5: ArangoDB to PyG via Metagraph v3 (transfer attributes via user-defined functions)
-def udf_v0_x(v0_df):
-    # process v0_df here to return v0 "x" feature matrix
-    # v0_df["x"] = ...
-    return torch.tensor(v0_df["x"].to_list())
-
-
-def udf_v1_x(v1_df):
-    # process v1_df here to return v1 "x" feature matrix
-    # v1_df["x"] = ...
-    return torch.tensor(v1_df["x"].to_list())
-
-
-metagraph_v3 = {
-    "vertexCollections": {
-        "v0": {
-            "x": udf_v0_x,  # supports named functions
-            "y": lambda df: torch.tensor(df["y"].to_list()),  # also supports lambda functions
-        },
-        "v1": {"x": udf_v1_x},
-    },
-    "edgeCollections": {
-        "e0": {"edge_attr": (lambda df: torch.tensor(df["edge_attr"].to_list()))},
-    },
-}
-pyg_g = adbpyg_adapter.arangodb_to_pyg("FakeData", metagraph_v3)
-```
-
-### Experimental: `preserve_adb_keys`
-```py
-# With `preserve_adb_keys=True`, the adapter will preserve the ArangoDB vertex & edge _key values into the (newly created) PyG graph.
-# Users can then re-import their PyG graph into ArangoDB using the same _key values 
-pyg_g = adbpyg_adapter.arangodb_graph_to_pyg("imdb", preserve_adb_keys=True)
-
-# pyg_g["Movies"]["_key"] --> ["1", "2", ..., "1682"]
-# pyg_g["Users"]["_key"] --> ["1", "2", ..., "943"]
-# pyg_g[("Users", "Ratings", "Movies")]["_key"] --> ["2732620466", ..., "2730643624"]
-
-# Let's add a new PyG User Node by updating the _key property
-pyg_g["Users"]["_key"].append("new-user-here-944")
-
-# Note: Prior to the re-import, we must manually set the number of nodes in the PyG graph, since the `arangodb_graph_to_pyg` API creates featureless node data
-pyg_g["Movies"].num_nodes = len(pyg_g["Movies"]["_key"]) # 1682
-pyg_g["Users"].num_nodes = len(pyg_g["Users"]["_key"]) # 944 (prev. 943)
-
-# Re-import PyG graph into ArangoDB
-adbpyg_adapter.pyg_to_arangodb("imdb", pyg_g, on_duplicate="update")
-```
-
-##  Development & Testing
-
-Prerequisite: `arangorestore`
-
-1. `git clone https://github.com/arangoml/pyg-adapter.git`
-2. `cd pyg-adapter`
-3. (create virtual environment of choice)
-4. `pip install -e .[dev]`
-5. (create an ArangoDB instance with method of choice)
-6. `pytest --url <> --dbName <> --username <> --password <>`
-
-**Note**: A `pytest` parameter can be omitted if the endpoint is using its default value:
-```python
-def pytest_addoption(parser):
-    parser.addoption("--url", action="store", default="http://localhost:8529")
-    parser.addoption("--dbName", action="store", default="_system")
-    parser.addoption("--username", action="store", default="root")
-    parser.addoption("--password", action="store", default="")
-```
```

### Comparing `adbpyg_adapter-1.1.0/adbpyg_adapter.egg-info/SOURCES.txt` & `adbpyg_adapter-1.1.1/adbpyg_adapter.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/analyze.yml
 .github/workflows/build.yml
+.github/workflows/build_self_hosted.yml
 .github/workflows/release.yml
 adbpyg_adapter/__init__.py
 adbpyg_adapter/abc.py
 adbpyg_adapter/adapter.py
 adbpyg_adapter/controller.py
 adbpyg_adapter/encoders.py
 adbpyg_adapter/exceptions.py
```

### Comparing `adbpyg_adapter-1.1.0/setup.py` & `adbpyg_adapter-1.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,36 +7,36 @@
     name="adbpyg_adapter",
     author="Anthony Mahanna",
     author_email="anthony.mahanna@arangodb.com",
     description="Convert ArangoDB graphs to PyG & vice-versa.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arangoml/pyg-adapter",
-    keywords=["arangodb", "pyg", "adapter"],
+    keywords=["arangodb", "pyg", "pytorch", "pytorch geometric", "adapter"],
     packages=["adbpyg_adapter"],
     include_package_data=True,
     python_requires=">=3.7",
     license="Apache Software License",
     install_requires=[
         "requests>=2.27.1",
         "rich>=12.5.1",
         "pandas>=1.3.5",
-        "python-arango>=7.4.1",
+        "python-arango==7.6.0",
         "torch>=1.12.0",
         "torch-sparse>=0.6.14",
         "torch-scatter>=2.0.9",
         "torch-geometric>=2.0.4",
         "setuptools>=45",
     ],
     extras_require={
         "dev": [
-            "black>=22.6.0",
-            "flake8>=3.8.0",
-            "isort>=5.0.0",
-            "mypy>=0.790",
+            "black==23.3.0",
+            "flake8==6.0.0",
+            "isort==5.12.0",
+            "mypy==1.4.1",
             "pytest>=6.0.0",
             "pytest-cov>=2.0.0",
             "coveralls>=3.3.1",
             "types-setuptools>=57.4.9",
             "types-requests>=2.27.11",
             "networkx>=2.5.1",
         ],
@@ -46,11 +46,12 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Utilities",
         "Typing :: Typed",
     ],
 )
```

