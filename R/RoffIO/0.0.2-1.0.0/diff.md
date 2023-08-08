# Comparing `tmp/RoffIO-0.0.2.tar.gz` & `tmp/RoffIO-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/RoffIO-0.0.2.tar", last modified: Thu Aug  5 11:33:17 2021, max compression
+gzip compressed data, was "RoffIO-1.0.0.tar", last modified: Tue Aug  8 11:21:09 2023, max compression
```

## Comparing `RoffIO-0.0.2.tar` & `RoffIO-1.0.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 11:33:17.000000 RoffIO-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 11:33:17.000000 RoffIO-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 11:33:17.000000 RoffIO-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      684 2021-08-05 11:33:09.000000 RoffIO-0.0.2/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)      334 2021-08-05 11:33:09.000000 RoffIO-0.0.2/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (121)      521 2021-08-05 11:33:09.000000 RoffIO-0.0.2/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (121)      403 2021-08-05 11:33:09.000000 RoffIO-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      401 2021-08-05 11:33:09.000000 RoffIO-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2021-08-05 11:33:09.000000 RoffIO-0.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     6513 2021-08-05 11:33:17.000000 RoffIO-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5853 2021-08-05 11:33:09.000000 RoffIO-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-08-05 11:33:09.000000 RoffIO-0.0.2/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      157 2021-08-05 11:33:17.000000 RoffIO-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2021-08-05 11:33:09.000000 RoffIO-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 11:33:17.000000 RoffIO-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 11:33:17.000000 RoffIO-0.0.2/src/RoffIO.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6513 2021-08-05 11:33:16.000000 RoffIO-0.0.2/src/RoffIO.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2021-08-05 11:33:17.000000 RoffIO-0.0.2/src/RoffIO.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-05 11:33:16.000000 RoffIO-0.0.2/src/RoffIO.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-08-05 11:33:16.000000 RoffIO-0.0.2/src/RoffIO.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-08-05 11:33:16.000000 RoffIO-0.0.2/src/RoffIO.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 11:33:17.000000 RoffIO-0.0.2/src/_roffio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/_roffio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/_roffio/endianess_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/_roffio/lazy_tuple.py
--rw-r--r--   0 runner    (1001) docker     (121)    12513 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/_roffio/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/_roffio/reading.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 11:33:17.000000 RoffIO-0.0.2/src/_roffio/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/_roffio/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4113 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/_roffio/tokenizer/abstract_roff_body_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     8097 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/_roffio/tokenizer/binary_roff_body_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/_roffio/tokenizer/combinators.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/_roffio/tokenizer/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      473 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/_roffio/tokenizer/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2304 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/_roffio/tokenizer/roff_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5642 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/_roffio/tokenizer/text_roff_body_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)      767 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/_roffio/tokenizer/token.py
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/_roffio/tokenizer/token_kind.py
--rw-r--r--   0 runner    (1001) docker     (121)    11484 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/_roffio/writing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 11:33:17.000000 RoffIO-0.0.2/src/roffio/
--rw-r--r--   0 runner    (1001) docker     (121)      213 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/roffio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      171 2021-08-05 11:33:09.000000 RoffIO-0.0.2/src/roffio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 11:33:17.000000 RoffIO-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-05 11:33:09.000000 RoffIO-0.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-05 11:33:17.000000 RoffIO-0.0.2/tests/generators/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-05 11:33:09.000000 RoffIO-0.0.2/tests/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5429 2021-08-05 11:33:09.000000 RoffIO-0.0.2/tests/generators/roff_file_contents.py
--rw-r--r--   0 runner    (1001) docker     (121)      439 2021-08-05 11:33:09.000000 RoffIO-0.0.2/tests/generators/roff_tag_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     6571 2021-08-05 11:33:09.000000 RoffIO-0.0.2/tests/test_binary_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2021-08-05 11:33:09.000000 RoffIO-0.0.2/tests/test_endianess_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      331 2021-08-05 11:33:09.000000 RoffIO-0.0.2/tests/test_lazy_tuple.py
--rw-r--r--   0 runner    (1001) docker     (121)    11305 2021-08-05 11:33:09.000000 RoffIO-0.0.2/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2021-08-05 11:33:09.000000 RoffIO-0.0.2/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (121)     5344 2021-08-05 11:33:09.000000 RoffIO-0.0.2/tests/test_read_write.py
--rw-r--r--   0 runner    (1001) docker     (121)     6714 2021-08-05 11:33:09.000000 RoffIO-0.0.2/tests/test_text_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2021-08-05 11:33:09.000000 RoffIO-0.0.2/tests/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)      753 2021-08-05 11:33:09.000000 RoffIO-0.0.2/tests/test_tokenizer_combinators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2021-08-05 11:33:09.000000 RoffIO-0.0.2/tests/test_write.py
--rw-r--r--   0 runner    (1001) docker     (121)      329 2021-08-05 11:33:09.000000 RoffIO-0.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:21:09.516004 RoffIO-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:21:09.512004 RoffIO-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:21:09.512004 RoffIO-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-08 11:20:58.000000 RoffIO-1.0.0/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-08 11:20:58.000000 RoffIO-1.0.0/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-08 11:20:58.000000 RoffIO-1.0.0/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-08 11:20:58.000000 RoffIO-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-08 11:20:58.000000 RoffIO-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-08 11:20:58.000000 RoffIO-1.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-08-08 11:21:09.516004 RoffIO-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-08-08 11:20:58.000000 RoffIO-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 11:20:58.000000 RoffIO-1.0.0/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-08 11:21:09.516004 RoffIO-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-08-08 11:20:58.000000 RoffIO-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:21:09.512004 RoffIO-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:21:09.516004 RoffIO-1.0.0/src/RoffIO.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-08-08 11:21:09.000000 RoffIO-1.0.0/src/RoffIO.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-08-08 11:21:09.000000 RoffIO-1.0.0/src/RoffIO.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 11:21:09.000000 RoffIO-1.0.0/src/RoffIO.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-08 11:21:09.000000 RoffIO-1.0.0/src/RoffIO.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-08 11:21:09.000000 RoffIO-1.0.0/src/RoffIO.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:21:09.516004 RoffIO-1.0.0/src/_roffio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/_roffio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/_roffio/endianess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/_roffio/lazy_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/_roffio/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/_roffio/reading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:21:09.516004 RoffIO-1.0.0/src/_roffio/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/_roffio/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/_roffio/tokenizer/abstract_roff_body_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/_roffio/tokenizer/binary_roff_body_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/_roffio/tokenizer/combinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/_roffio/tokenizer/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/_roffio/tokenizer/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/_roffio/tokenizer/roff_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/_roffio/tokenizer/text_roff_body_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/_roffio/tokenizer/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/_roffio/tokenizer/token_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/_roffio/writing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:21:09.516004 RoffIO-1.0.0/src/roffio/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/roffio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-08 11:20:58.000000 RoffIO-1.0.0/src/roffio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:21:09.516004 RoffIO-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:20:58.000000 RoffIO-1.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:21:09.516004 RoffIO-1.0.0/tests/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:20:58.000000 RoffIO-1.0.0/tests/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-08-08 11:20:58.000000 RoffIO-1.0.0/tests/generators/roff_file_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-08 11:20:58.000000 RoffIO-1.0.0/tests/generators/roff_tag_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-08-08 11:20:58.000000 RoffIO-1.0.0/tests/test_binary_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-08 11:20:58.000000 RoffIO-1.0.0/tests/test_endianess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-08 11:20:58.000000 RoffIO-1.0.0/tests/test_lazy_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-08-08 11:20:58.000000 RoffIO-1.0.0/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-08 11:20:58.000000 RoffIO-1.0.0/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-08-08 11:20:58.000000 RoffIO-1.0.0/tests/test_read_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-08-08 11:20:58.000000 RoffIO-1.0.0/tests/test_text_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-08 11:20:58.000000 RoffIO-1.0.0/tests/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-08 11:20:58.000000 RoffIO-1.0.0/tests/test_tokenizer_combinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-08-08 11:20:58.000000 RoffIO-1.0.0/tests/test_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-08 11:20:58.000000 RoffIO-1.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `RoffIO-0.0.2/.github/workflows/publish_to_pypi.yml` & `RoffIO-1.0.0/.github/workflows/publish_to_pypi.yml`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to PyPI
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@master
-    - name: Set up Python 3.7
-      uses: actions/setup-python@v1
+    - name: Set up Python 3.11
+      uses: actions/setup-python@v4
       with:
-        python-version: 3.7
+        python-version: "3.11"
     - name: Install dependencies
       run: pip install --upgrade setuptools wheel twine
     - name: Build package
       run: python setup.py sdist bdist_wheel
     - name: Upload deploy
       env:
         TWINE_USERNAME: __token__
```

### Comparing `RoffIO-0.0.2/.github/workflows/testing.yml` & `RoffIO-1.0.0/.github/workflows/testing.yml`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 jobs:
   tests:
     name: "Python ${{ matrix.python-version }}"
     runs-on: "ubuntu-latest"
     strategy:
       matrix:
-        python-version: ["3.6", "3.7", "3.8"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
-      - uses: actions/checkout@v1
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install tox
         run: pip install tox tox-gh-actions
       - name: Test with tox
         run: tox
```

### Comparing `RoffIO-0.0.2/LICENSE.md` & `RoffIO-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/PKG-INFO` & `RoffIO-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: RoffIO
-Version: 0.0.2
+Version: 1.0.0
 Summary: A (lazy) parser and writer for the Roxar Open File Format (ROFF).
 Home-page: https://github.com/equinor/roffio
 Author: Equinor
 Author-email: fg_sib-scout@equinor.com
 License: LGPL-3.0
 Platform: any
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 Roff IO
 ==========
 
 A (lazy) parser and writer for the Roxar Open File Format (ROFF) (binary and ascii).
@@ -280,9 +281,7 @@
 results in a roff file containing
 
 ```
 tag t
 array bytes key 2 0 1
 endtag
 ```
-
-
```

### Comparing `RoffIO-0.0.2/README.md` & `RoffIO-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/setup.py` & `RoffIO-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     packages=find_packages(where="src"),
     install_requires=["dataclasses>=0.6;python_version<'3.7'", "numpy"],
     platforms="any",
     classifiers=[
         "Development Status :: 1 - Planning",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     setup_requires=["setuptools_scm"],
     include_package_data=True,
 )
```

### Comparing `RoffIO-0.0.2/src/RoffIO.egg-info/PKG-INFO` & `RoffIO-1.0.0/src/RoffIO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: RoffIO
-Version: 0.0.2
+Version: 1.0.0
 Summary: A (lazy) parser and writer for the Roxar Open File Format (ROFF).
 Home-page: https://github.com/equinor/roffio
 Author: Equinor
 Author-email: fg_sib-scout@equinor.com
 License: LGPL-3.0
 Platform: any
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 Roff IO
 ==========
 
 A (lazy) parser and writer for the Roxar Open File Format (ROFF) (binary and ascii).
@@ -280,9 +281,7 @@
 results in a roff file containing
 
 ```
 tag t
 array bytes key 2 0 1
 endtag
 ```
-
-
```

### Comparing `RoffIO-0.0.2/src/RoffIO.egg-info/SOURCES.txt` & `RoffIO-1.0.0/src/RoffIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/src/_roffio/endianess_handler.py` & `RoffIO-1.0.0/src/_roffio/endianess_handler.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/src/_roffio/lazy_tuple.py` & `RoffIO-1.0.0/src/_roffio/lazy_tuple.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/src/_roffio/parser.py` & `RoffIO-1.0.0/src/_roffio/parser.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/src/_roffio/reading.py` & `RoffIO-1.0.0/src/_roffio/reading.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/src/_roffio/tokenizer/__init__.py` & `RoffIO-1.0.0/src/_roffio/tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/src/_roffio/tokenizer/abstract_roff_body_tokenizer.py` & `RoffIO-1.0.0/src/_roffio/tokenizer/abstract_roff_body_tokenizer.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/src/_roffio/tokenizer/binary_roff_body_tokenizer.py` & `RoffIO-1.0.0/src/_roffio/tokenizer/binary_roff_body_tokenizer.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/src/_roffio/tokenizer/combinators.py` & `RoffIO-1.0.0/src/_roffio/tokenizer/combinators.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/src/_roffio/tokenizer/common.py` & `RoffIO-1.0.0/src/_roffio/tokenizer/common.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/src/_roffio/tokenizer/roff_tokenizer.py` & `RoffIO-1.0.0/src/_roffio/tokenizer/roff_tokenizer.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/src/_roffio/tokenizer/text_roff_body_tokenizer.py` & `RoffIO-1.0.0/src/_roffio/tokenizer/text_roff_body_tokenizer.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/src/_roffio/tokenizer/token.py` & `RoffIO-1.0.0/src/_roffio/tokenizer/token.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/src/_roffio/tokenizer/token_kind.py` & `RoffIO-1.0.0/src/_roffio/tokenizer/token_kind.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/src/_roffio/writing.py` & `RoffIO-1.0.0/src/_roffio/writing.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import warnings
 from collections import OrderedDict
 from datetime import datetime
 from enum import Enum, unique
 from functools import wraps
 
 import numpy as np
+
 from roffio.version import version as roffio_version
 
 
 class RoffWriteError(Exception):
     pass
 
 
@@ -124,15 +125,15 @@
     elif type_str == "bool" and isinstance(value, bool):
         stream.write(str(int(value)))
     else:
         stream.write(str(value))
 
 
 def write_binary_tagkey(file_stream, tagkey_name, value):
-    if type(value) == np.ndarray:
+    if type(value) is np.ndarray:
         file_stream.write(b"array\0")
         value = cast_array_to_roff(value)
         file_stream.write(numpy_to_roff_dtype(value.dtype).encode("ascii"))
         file_stream.write(b"\0")
         write_binary_string(file_stream, tagkey_name)
         file_stream.write(len(value).to_bytes(4, "little"))
         file_stream.write(value.tobytes())
```

### Comparing `RoffIO-0.0.2/tests/generators/roff_file_contents.py` & `RoffIO-1.0.0/tests/generators/roff_file_contents.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,28 +46,28 @@
         num_bytes = tokenlen(kindstr)
         return draw(st.binary(min_size=num_bytes, max_size=num_bytes))
 
 
 ascii_values = st.builds(
     str,
     st.one_of(
-        st.integers(min_value=-(2 ** 30), max_value=2 ** 30),
+        st.integers(min_value=-(2**30), max_value=2**30),
         st.floats(allow_infinity=False, allow_nan=False),
         string_literals(),
     ),
 )
 
 
 def typed_ascii_values(kindstr):
     if kindstr == "bool":
         return st.integers(min_value=0, max_value=1)
     elif kindstr == "byte":
         return st.integers(min_value=0, max_value=127)
     elif kindstr == "int":
-        return st.integers(min_value=-(2 ** 30), max_value=2 ** 30)
+        return st.integers(min_value=-(2**30), max_value=2**30)
     elif kindstr == "float":
         return st.floats(allow_infinity=False, allow_nan=False)
     elif kindstr == "double":
         return st.floats(allow_infinity=False, allow_nan=False)
     elif kindstr == "char":
         return string_literals()
```

### Comparing `RoffIO-0.0.2/tests/test_binary_tokenizer.py` & `RoffIO-1.0.0/tests/test_binary_tokenizer.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/tests/test_endianess_handler.py` & `RoffIO-1.0.0/tests/test_endianess_handler.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/tests/test_parse.py` & `RoffIO-1.0.0/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/tests/test_read_write.py` & `RoffIO-1.0.0/tests/test_read_write.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/tests/test_text_tokenizer.py` & `RoffIO-1.0.0/tests/test_text_tokenizer.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/tests/test_tokenizer.py` & `RoffIO-1.0.0/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/tests/test_tokenizer_combinators.py` & `RoffIO-1.0.0/tests/test_tokenizer_combinators.py`

 * *Files identical despite different names*

### Comparing `RoffIO-0.0.2/tests/test_write.py` & `RoffIO-1.0.0/tests/test_write.py`

 * *Files identical despite different names*

