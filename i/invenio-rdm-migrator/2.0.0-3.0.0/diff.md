# Comparing `tmp/invenio-rdm-migrator-2.0.0.tar.gz` & `tmp/invenio-rdm-migrator-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-rdm-migrator-2.0.0.tar", last modified: Tue Aug  1 12:46:07 2023, max compression
+gzip compressed data, was "dist/invenio-rdm-migrator-3.0.0.tar", last modified: Tue Aug  8 15:34:13 2023, max compression
```

## Comparing `invenio-rdm-migrator-2.0.0.tar` & `invenio-rdm-migrator-3.0.0.tar`

### file list

```diff
@@ -1,180 +1,184 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/actions/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/extract/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/extract/jsonlines.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/extract/null.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/extract/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/ids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/copy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/existing.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/single.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/sequences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/transactions/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/transactions/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/transactions/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/actions/drafts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/awards/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/awards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/awards/load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/funders/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/funders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/funders/load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/awards.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/communities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/funders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/pids.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/records.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/oauth/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/oauth/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/oauth/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/drafts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/parents.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/records.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/references.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/requests/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/requests/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/requests/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/users/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/users/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/users/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/users/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/invenio_rdm_migrator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/extract/test_base_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/extract/test_jsonlines.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/extract/test_null.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/load/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/load/test_base_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/load/test_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/load/test_postgresql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/streams/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/streams/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/actions/test_drafts_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/streams/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/communities/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/communities/test_communities_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/communities/test_communities_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/communities/test_communities_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/streams/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/files/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/files/test_files_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/files/test_files_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/files/test_files_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/streams/records/
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17205 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/records/test_records_table_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/streams/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/requests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/requests/test_requests_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/requests/test_requests_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/requests/test_requests_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/streams/test_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:46:07.000000 invenio-rdm-migrator-2.0.0/tests/transform/
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/transform/test_base_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/transform/test_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/transform/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-08-01 12:45:58.000000 invenio-rdm-migrator-2.0.0/tests/transform/test_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16453 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/actions/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/extract/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/extract/jsonlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/extract/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/extract/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/bulk/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/bulk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/bulk/copy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/existing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/sequences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/transactions/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/transactions/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/transactions/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/actions/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/actions/parents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/actions/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/awards/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/awards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/awards/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/communities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/communities/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/communities/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/communities/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/files/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/files/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/files/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/funders/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/funders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/funders/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/awards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/communities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/funders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/pids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/oauth/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/oauth/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/table_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/table_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/table_generators/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/table_generators/parents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/table_generators/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/table_generators/references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/table_generators/versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/requests/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/requests/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/requests/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/users/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/users/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/users/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/transform/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/transform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/transform/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/transform/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16453 2023-08-08 15:34:12.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-08-08 15:34:12.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:34:12.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:34:12.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-08 15:34:12.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 15:34:12.000000 invenio-rdm-migrator-3.0.0/invenio_rdm_migrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/tests/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/extract/test_base_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/extract/test_jsonlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/extract/test_null.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/tests/load/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/load/test_base_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/load/test_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/load/test_load_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/load/test_load_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/tests/streams/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/tests/streams/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/actions/test_drafts_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/actions/test_user_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/tests/streams/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/communities/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/communities/test_communities_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/communities/test_communities_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/communities/test_communities_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/tests/streams/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/files/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/files/test_files_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/files/test_files_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/files/test_files_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/tests/streams/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17205 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/records/test_records_table_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/tests/streams/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/requests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/requests/test_requests_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/requests/test_requests_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/requests/test_requests_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/streams/test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:34:13.000000 invenio-rdm-migrator-3.0.0/tests/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/transform/test_base_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/transform/test_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/transform/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-08-08 15:34:07.000000 invenio-rdm-migrator-3.0.0/tests/transform/test_transactions.py
```

### Comparing `invenio-rdm-migrator-2.0.0/.editorconfig` & `invenio-rdm-migrator-3.0.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/.github/workflows/pypi-publish.yml` & `invenio-rdm-migrator-3.0.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/.github/workflows/tests.yml` & `invenio-rdm-migrator-3.0.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/CONTRIBUTING.rst` & `invenio-rdm-migrator-3.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/LICENSE` & `invenio-rdm-migrator-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/MANIFEST.in` & `invenio-rdm-migrator-3.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/PKG-INFO` & `invenio-rdm-migrator-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-rdm-migrator
-Version: 2.0.0
+Version: 3.0.0
 Summary: InvenioRDM module for data migration.
 Home-page: https://github.com/inveniosoftware/invenio-rdm-migrator
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022-2023 CERN.
@@ -343,14 +343,22 @@
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
         
+        Version 3.0.0
+        
+        - `Operation` instances have split the model and the data into two attributes.
+        - Add user actions.
+        - `PostgreSQLTx` `resolve_references` function has now a default behaviour (`pass`).
+        - Add nullable configuration to draft and user related models.
+        - Minor bug fixes.
+        
         Version 2.0.0
         
         - Make state globally available.
         - Refactor transactions into actions. Create transaction and load data classes.
         - Removed empty kafka extract module.
         - Improved error handling and created specialized classes.
         - Move `dict_set` to utils.
```

### Comparing `invenio-rdm-migrator-2.0.0/README.rst` & `invenio-rdm-migrator-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/docs/Makefile` & `invenio-rdm-migrator-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/docs/conf.py` & `invenio-rdm-migrator-3.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/docs/index.rst` & `invenio-rdm-migrator-3.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/docs/make.bat` & `invenio-rdm-migrator-3.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/actions/base.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/actions/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             except AttributeError:
                 logger = Logger.get_logger()
                 logger.exception(f"Attribute {attr_name} not found", exc_info=1)
             except KeyError:
                 logger = Logger.get_logger()
                 logger.exception(f"Path {path} not found on record", exc_info=1)
 
-    def _resolve_references(self, data, **kwargs):  # pragma: no cover
+    def _resolve_references(self, **kwargs):  # pragma: no cover
         """Resolve references e.g communities slug names."""
         pass
 
     @abstractmethod
     def _generate_rows(self, **kwargs):  # pragma: no cover
         """Yield generated rows."""
```

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/extract/jsonlines.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/extract/jsonlines.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/extract/null.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/extract/null.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/base.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/base.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/ids.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/ids.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/copy.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/bulk/copy.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/existing.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/existing.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/single.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/single.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/table.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/bulk/generators/table.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/generators.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/sequences.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/sequences.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/transactions/execute.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/transactions/execute.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,49 +25,49 @@
 
     def _cleanup(self, db=False):
         """No cleanup."""
         logger = Logger.get_logger()
         logger.debug("PostgreSQLExecute does not implement _cleanup()")
         pass
 
-    def _update_obj(self, session, obj):
-        """Updates all attributes of an object."""
+    def _get_obj_by_pk(self, session, model, data):
+        """Get an object based on the primary key."""
         # this function accesses many private methods, variables, assumes indexes, etc.
         # pragmatic implementation, feel free to refactor.
-        pk = obj.__mapper__.primary_key[0].name
-        pk_value = getattr(obj, pk)
-        db_obj = session.get(obj.__class__, pk_value)
-        for column in db_obj.__table__.columns.keys():
-            value = getattr(obj, column)
-            setattr(db_obj, column, value)
+        pk = {}
+        for key in model.__mapper__.primary_key:
+            pk[key.name] = data[key.name]
 
-        return obj
+        return session.get(model, pk)
 
     def _load(self, transactions):
         """Performs the operations of a group transaction."""
         logger = Logger.get_logger()
 
         for action in transactions:
             operations = action.prepare()
 
             with Session(self._engine) as session:
                 for op in operations:
-                    type_ = op.type
-                    obj = op.obj
                     try:
-                        if type_ == OperationType.INSERT:
+                        if op.type == OperationType.INSERT:
+                            obj = op.model(**op.data)
                             session.add(obj)
-                        elif type_ == OperationType.DELETE:
+                        elif op.type == OperationType.DELETE:
+                            obj = self._get_obj_by_pk(session, op.model, op.data)
                             session.delete(obj)
-                        elif type_ == OperationType.UPDATE:
-                            self._update_obj(session, obj)
+                        elif op.type == OperationType.UPDATE:
+                            obj = self._get_obj_by_pk(session, op.model, op.data)
+                            for key, value in op.data.items():
+                                setattr(obj, key, value)
+
                         session.flush()
                     except Exception:
                         logger.exception(
-                            f"Could not load {action.tx_id} ({action.name})",
+                            f"Could not load {action.data.tx_id} ({action.name})",
                             exc_info=1,
                         )
                         session.rollback()
                         raise
                 # commit all transaction group or none
                 session.commit()
```

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/load/postgresql/transactions/operations.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/load/postgresql/transactions/operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """PostgreSQL Transaction load operations."""
 
 from enum import Enum
 
+from ..models import Model
+
 
 class OperationType(str, Enum):
     """SQL operation type enumeration."""
 
     INSERT = "C"
     UPDATE = "U"
     DELETE = "D"
@@ -28,12 +30,12 @@
 
 class Operation:
     """SQL operation.
 
     A transaction is composed by one or more operations.
     """
 
-    def __init__(self, type, obj):
+    def __init__(self, type: OperationType, model: Model, data: dict):
         """Constructor."""
-        assert isinstance(type, OperationType)
         self.type = type
-        self.obj = obj
+        self.model = model
+        self.data = data
```

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/logging.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/logging.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/state.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
         sa.Table(
             "pids",
             metadata,
             sa.Column("pid_value", sa.String, primary_key=True),
             sa.Column("id", sa.Integer, unique=True, nullable=False),
             sa.Column("pid_type", sa.String, nullable=False),
             sa.Column("status", sa.String, nullable=False),
-            sa.Column("created", sa.DateTime, nullable=False),
+            sa.Column("created", sa.String, nullable=False),
             # keep obj_type since the record needs this key dereferenced
             sa.Column("obj_type", sa.String),
             sqlite_autoincrement=False,
         )
 
         # e.g. key = max_pid_pk, value = 1_000_000
         sa.Table(
```

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/actions/drafts.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/actions/drafts.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 from ...actions import LoadAction, LoadData
 from ...load.ids import generate_pk, generate_recid, generate_uuid
 from ...load.postgresql.transactions.operations import Operation, OperationType
 from ...state import STATE
 from ..models.files import FilesBucket
 from ..models.pids import PersistentIdentifier
 from ..models.records import RDMDraftMetadata, RDMVersionState
-from ..records.table_generators.parents import generate_parent_rows
 from ..records.table_generators.references import (
     CommunitiesReferencesMixin,
     PIDsReferencesMixin,
 )
+from .parents import generate_parent_ops
 
 
 @dataclass
 class RDMDraftCreateData(LoadData):
     """Draft create action data."""
 
     # NOTE: we could go with some common ``typing.TypedDict`` definitions to help more
@@ -56,42 +56,30 @@
         yield from self._generate_bucket_rows(**kwargs)
         yield from self._generate_draft_rows(**kwargs)
 
     def _generate_pid_rows(self, **kwargs):
         """Generates rows for a new draft."""
         pid = self.data.pid
         if pid["pid_type"] != "depid":
-            # https://github.com/inveniosoftware/invenio-rdm-migrator/issues/123
-            from datetime import datetime
-
-            pid["created"] = datetime.fromtimestamp(pid["created"] / 1_000_000)
-            pid["updated"] = datetime.fromtimestamp(pid["updated"] / 1_000_000)
-
             # note would raise an exception if it exists
             STATE.PIDS.add(
                 pid["pid_value"],  # recid
                 {
                     "id": pid["id"],
                     "pid_type": pid["pid_type"],
                     "status": pid["status"],
                     "obj_type": pid["object_type"],
                     "created": pid["created"],
                 },
             )
-            yield Operation(OperationType.INSERT, PersistentIdentifier(**pid))
+            yield Operation(OperationType.INSERT, PersistentIdentifier, pid)
 
     def _generate_bucket_rows(self, **kwargs):
         """Generates rows for a new draft."""
-        # https://github.com/inveniosoftware/invenio-rdm-migrator/issues/123
-
-        bucket = self.data.bucket
-        bucket["created"] = datetime.fromtimestamp(bucket["created"] / 1_000_000)
-        bucket["updated"] = datetime.fromtimestamp(bucket["updated"] / 1_000_000)
-
-        yield Operation(OperationType.INSERT, FilesBucket(**bucket))
+        yield Operation(OperationType.INSERT, FilesBucket, self.data.bucket)
 
     def _generate_draft_rows(self, **kwargs):
         """Generates rows for a new draft."""
         now = datetime.utcnow().isoformat()
 
         draft = self.data.draft
         parent = self.data.parent
@@ -115,20 +103,15 @@
                 {
                     "id": parent["id"],
                     "next_draft_id": draft["id"],
                 },
             )
             # drafts have a parent on save
             # on the other hand there is no community parent/request
-            # https://github.com/inveniosoftware/invenio-rdm-migrator/issues/123
-            parent["created"] = datetime.fromtimestamp(parent["created"] / 1_000_000)
-            parent["updated"] = datetime.fromtimestamp(parent["updated"] / 1_000_000)
-            for obj in generate_parent_rows(parent):
-                # cannot use yield from because we have to add `op`
-                yield Operation(OperationType.INSERT, obj)
+            yield from generate_parent_ops(parent)
 
         else:  # case a and b
             parent["id"] = existing_parent["id"]
             draft["parent_id"] = existing_parent["id"]  # keep metadata consistent
             if not forked_published:
                 # it can only happen once
                 assert not existing_parent.get("next_draft_id")
@@ -145,33 +128,31 @@
             draft_pid = STATE.PIDS.get(draft["json"]["id"])
             assert draft_pid
 
             # update to add object_uuid
             # could avoid this operation but it is clearer on when and why this happens
             yield Operation(
                 OperationType.UPDATE,
-                PersistentIdentifier(
+                PersistentIdentifier,
+                dict(
                     id=draft_pid["id"],  # pk
                     pid_type=draft_pid["pid_type"],  # in drafts are recid
                     pid_value=draft["json"]["id"],
                     status=draft_pid["status"],
                     object_type="rec",  # hardcoded since the state has the initial one
                     object_uuid=draft["id"],
                     created=draft_pid["created"],
                     updated=now,
                 ),
             )
 
-        # https://github.com/inveniosoftware/invenio-rdm-migrator/issues/123
-        draft["created"] = datetime.fromtimestamp(draft["created"] / 1_000_000)
-        draft["updated"] = datetime.fromtimestamp(draft["updated"] / 1_000_000)
-
         yield Operation(
             OperationType.INSERT,
-            RDMDraftMetadata(
+            RDMDraftMetadata,
+            dict(
                 id=forked_published.get("id") or draft["id"],
                 json=draft["json"],
                 created=draft["created"],
                 updated=draft["updated"],
                 version_id=draft["version_id"],
                 index=forked_published.get("index") or draft["index"],
                 bucket_id=draft["bucket_id"],
@@ -180,19 +161,19 @@
                 fork_version_id=forked_published.get("fork_version_id")
                 or draft["fork_version_id"],
             ),
         )
 
         # this query can be avoided by keeping a consistent view across this method
         existing_parent = STATE.PARENTS.get(parent["json"]["id"])
-
         version_op = OperationType.UPDATE if forked_published else OperationType.INSERT
         yield Operation(
             version_op,
-            RDMVersionState(
+            RDMVersionState,
+            dict(
                 latest_index=existing_parent["latest_index"],
                 parent_id=existing_parent["id"],
                 latest_id=existing_parent["latest_id"],
                 next_draft_id=existing_parent["next_draft_id"],
             ),
         )
```

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/awards/load.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/awards/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/__init__.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/communities/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/load.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/communities/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/table_generator.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/communities/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/communities/transform.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/communities/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/__init__.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/files/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/load.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/files/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/table_generator.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/files/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/files/transform.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/files/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/funders/load.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/funders/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/awards.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/awards.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/communities.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/communities.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/files.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/files.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/funders.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/funders.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/oauth.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/oauth.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/pids.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/pids.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/records.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/records.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/models/requests.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/models/requests.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/oauth/__init__.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/oauth/load.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/oauth/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/oauth/transform.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/oauth/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/load.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/state.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/state.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/drafts.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/table_generators/drafts.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/parents.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/table_generators/parents.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/records.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/table_generators/records.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/references.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/table_generators/references.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/table_generators/versions.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/table_generators/versions.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/records/transform.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/records/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/requests/load.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/requests/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/requests/table_generator.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/requests/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/requests/transform.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/requests/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/runner.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/runner.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/streams.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/streams.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/users/load.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/users/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/users/table_generator.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/users/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/streams/users/transform.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/streams/users/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/__init__.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/base.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/transform/base.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/encrypt.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/transform/encrypt.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/errors.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/transform/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/identity.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/transform/identity.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/transform/transactions.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/transform/transactions.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator/utils.py` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,12 +50,9 @@
 
 
 def dict_set(source, key, value):
     """Set a value into a dict via a dot-notated key."""
     keys = parse_lookup_key(key)
     parent = source
     for key in keys[:-1]:
-        if isinstance(key, int):
-            parent = parent[key]
-        else:
-            parent = parent.setdefault(key, {})
+        parent = parent.setdefault(key, {})
     parent[keys[-1]] = value
```

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator.egg-info/PKG-INFO` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-rdm-migrator
-Version: 2.0.0
+Version: 3.0.0
 Summary: InvenioRDM module for data migration.
 Home-page: https://github.com/inveniosoftware/invenio-rdm-migrator
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022-2023 CERN.
@@ -343,14 +343,22 @@
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
         
+        Version 3.0.0
+        
+        - `Operation` instances have split the model and the data into two attributes.
+        - Add user actions.
+        - `PostgreSQLTx` `resolve_references` function has now a default behaviour (`pass`).
+        - Add nullable configuration to draft and user related models.
+        - Minor bug fixes.
+        
         Version 2.0.0
         
         - Make state globally available.
         - Refactor transactions into actions. Create transaction and load data classes.
         - Removed empty kafka extract module.
         - Improved error handling and created specialized classes.
         - Move `dict_set` to utils.
```

### Comparing `invenio-rdm-migrator-2.0.0/invenio_rdm_migrator.egg-info/SOURCES.txt` & `invenio-rdm-migrator-3.0.0/invenio_rdm_migrator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
 invenio_rdm_migrator/load/postgresql/transactions/execute.py
 invenio_rdm_migrator/load/postgresql/transactions/operations.py
 invenio_rdm_migrator/streams/__init__.py
 invenio_rdm_migrator/streams/runner.py
 invenio_rdm_migrator/streams/streams.py
 invenio_rdm_migrator/streams/actions/__init__.py
 invenio_rdm_migrator/streams/actions/drafts.py
+invenio_rdm_migrator/streams/actions/parents.py
+invenio_rdm_migrator/streams/actions/users.py
 invenio_rdm_migrator/streams/awards/__init__.py
 invenio_rdm_migrator/streams/awards/load.py
 invenio_rdm_migrator/streams/communities/__init__.py
 invenio_rdm_migrator/streams/communities/load.py
 invenio_rdm_migrator/streams/communities/table_generator.py
 invenio_rdm_migrator/streams/communities/transform.py
 invenio_rdm_migrator/streams/files/__init__.py
@@ -116,17 +118,19 @@
 tests/test_state.py
 tests/test_utils.py
 tests/extract/test_base_extract.py
 tests/extract/test_jsonlines.py
 tests/extract/test_null.py
 tests/load/test_base_load.py
 tests/load/test_ids.py
-tests/load/test_postgresql.py
+tests/load/test_load_bulk.py
+tests/load/test_load_transactions.py
 tests/streams/test_streams.py
 tests/streams/actions/test_drafts_actions.py
+tests/streams/actions/test_user_actions.py
 tests/streams/communities/conftest.py
 tests/streams/communities/test_communities_load.py
 tests/streams/communities/test_communities_table_generator.py
 tests/streams/communities/test_communities_transform.py
 tests/streams/files/conftest.py
 tests/streams/files/test_files_load.py
 tests/streams/files/test_files_table_generator.py
```

### Comparing `invenio-rdm-migrator-2.0.0/run-tests.sh` & `invenio-rdm-migrator-3.0.0/run-tests.sh`

 * *Files 7% similar despite different names*

```diff
@@ -36,10 +36,12 @@
 done
 
 export LC_TIME=en_US.UTF-8
 python -m check_manifest
 python -m sphinx.cmd.build -qnNW docs docs/_build/html
 # Note: expansion of pytest_args looks like below to not cause an unbound
 # variable error when 1) "nounset" and 2) the array is empty.
+eval "$(docker-services-cli up --db ${DB:-postgresql} --env)"
 python -m pytest ${pytest_args[@]+"${pytest_args[@]}"}
 tests_exit_code=$?
+eval "$(docker-services-cli down --env)"
 exit "$tests_exit_code"
```

### Comparing `invenio-rdm-migrator-2.0.0/setup.cfg` & `invenio-rdm-migrator-3.0.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 	PyYAML>=5.4.1
 
 [options.extras_require]
 tests = 
 	check-manifest>=0.25
 	coverage>=4.0,<5.0.0
 	dictdiffer>=0.9.0
+	docker-services-cli>=0.6.1
 	isort>=4.3
 	pydocstyle>=2.0.0
 	pytest>=4.6.1
 	pytest-black>=0.3.0
 	pytest-cov>=2.5.1
 	pytest-isort>=3.1.0
 	pytest-pep8>=1.0.6
```

### Comparing `invenio-rdm-migrator-2.0.0/tests/conftest.py` & `invenio-rdm-migrator-3.0.0/tests/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -61,7 +61,21 @@
     """Communities state.
 
     Keys are community slugs and values are UUIDs.
     """
     state.COMMUNITIES.add("comm", {"id": "12345678-abcd-1a2b-3c4d-123abc456def"})
 
     return state
+
+
+@pytest.fixture(scope="function")
+def secret_keys_state(state):
+    """Adds secret keys to global state."""
+    state.VALUES.add(
+        "old_secret_key",
+        {"value": bytes("OLDKEY", "utf-8")},
+    )
+    state.VALUES.add(
+        "new_secret_key",
+        {"value": bytes("NEWKEY", "utf-8")},
+    )
+    return
```

### Comparing `invenio-rdm-migrator-2.0.0/tests/extract/test_base_extract.py` & `invenio-rdm-migrator-3.0.0/tests/extract/test_base_extract.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/extract/test_jsonlines.py` & `invenio-rdm-migrator-3.0.0/tests/extract/test_jsonlines.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/extract/test_null.py` & `invenio-rdm-migrator-3.0.0/tests/extract/test_null.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/load/test_base_load.py` & `invenio-rdm-migrator-3.0.0/tests/load/test_base_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/load/test_ids.py` & `invenio-rdm-migrator-3.0.0/tests/load/test_ids.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/load/test_postgresql.py` & `invenio-rdm-migrator-3.0.0/tests/load/test_load_bulk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2023 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
-"""PostgreSQL load tests."""
+"""PostgreSQL bulk load tests."""
 
 import tempfile
 from dataclasses import InitVar
 from unittest.mock import patch
 
 import pytest
 from sqlalchemy.orm import Mapped, mapped_column
```

### Comparing `invenio-rdm-migrator-2.0.0/tests/streams/actions/test_drafts_actions.py` & `invenio-rdm-migrator-3.0.0/tests/streams/actions/test_drafts_actions.py`

 * *Files 22% similar despite different names*

```diff
@@ -39,16 +39,16 @@
         },
         "version_id": 1,
         "index": 1,
         "bucket_id": "0e12b4b6-9cc7-46df-9a04-c11c478de211",
         "parent_id": "9493793c-47d2-48e2-9867-ca597b4ebb41",
         "expires_at": None,
         "fork_version_id": None,
-        "created": 1620000000000,
-        "updated": 1620000000000,
+        "created": "2021-05-01T00:00:00",
+        "updated": "2021-05-01T00:00:00",
     }
 
 
 @pytest.fixture(scope="function")
 def parent_data():
     """Parent data."""
     return {
@@ -56,26 +56,26 @@
         "json": {
             "id": "1217214",
             "pid": {"pk": 2, "pid_type": "recid", "status": "R", "obj_type": "rec"},
             "access": {"owned_by": [{"user": 1234}]},
             "communities": {"ids": ["zenodo", "migration"], "default": "zenodo"},
         },
         "version_id": 1,
-        "created": 1620000000000,
-        "updated": 1620000000000,
+        "created": "2021-05-01T00:00:00",
+        "updated": "2021-05-01T00:00:00",
     }
 
 
 @pytest.fixture(scope="function")
 def bucket_data():
     """Bucket data."""
     return {
         "id": "0e12b4b6-9cc7-46df-9a04-c11c478de211",
-        "created": 1640995200000000,
-        "updated": 1640995200000000,
+        "created": "2022-01-01T00:00:00",
+        "updated": "2022-01-01T00:00:00",
         "default_location": 1,
         "default_storage_class": "L",
         "size": 0,
         "quota_size": 50000000000,
         "max_file_size": 50000000000,
         "locked": False,
         "deleted": False,
@@ -89,16 +89,16 @@
         "id": 12132090,
         "pid_type": "recid",
         "pid_value": "1217215",
         "pid_provider": None,
         "status": "K",
         "object_type": "rec",
         "object_uuid": "d94f793c-47d2-48e2-9867-ca597b4ebb41",
-        "created": 1640995200000000,
-        "updated": 1640995200000000,
+        "created": "2022-01-01T00:00:00",
+        "updated": "2022-01-01T00:00:00",
     }
 
 
 def test_create_draft_new(state, draft_data, parent_data, bucket_data, pid_data):
     data = dict(
         tx_id=1,
         pid=pid_data,
@@ -106,27 +106,27 @@
         draft=draft_data,
         parent=parent_data,
     )
     action = DraftCreateAction(data)
     rows = list(action.prepare())
     assert len(rows) == 7
     assert rows[0].type == OperationType.INSERT
-    assert isinstance(rows[0].obj, PersistentIdentifier)
+    assert rows[0].model == PersistentIdentifier
     assert rows[1].type == OperationType.INSERT
-    assert isinstance(rows[1].obj, FilesBucket)
+    assert rows[1].model == FilesBucket
     assert rows[2].type == OperationType.INSERT
-    assert isinstance(rows[2].obj, PersistentIdentifier)
+    assert rows[2].model == PersistentIdentifier
     assert rows[3].type == OperationType.INSERT
-    assert isinstance(rows[3].obj, RDMParentMetadata)
+    assert rows[3].model == RDMParentMetadata
     assert rows[4].type == OperationType.UPDATE
-    assert isinstance(rows[4].obj, PersistentIdentifier)
+    assert rows[4].model == PersistentIdentifier
     assert rows[5].type == OperationType.INSERT
-    assert isinstance(rows[5].obj, RDMDraftMetadata)
+    assert rows[5].model == RDMDraftMetadata
     assert rows[6].type == OperationType.INSERT
-    assert isinstance(rows[6].obj, RDMVersionState)
+    assert rows[6].model == RDMVersionState
 
 
 def test_create_draft_new_version(
     state, draft_data, parent_data, bucket_data, pid_data
 ):
     # set existing parent so the action goes on the new version path
     state.PARENTS.add(
@@ -145,23 +145,23 @@
         parent=parent_data,
     )
     action = DraftCreateAction(data)
 
     rows = list(action.prepare())
     assert len(rows) == 5
     assert rows[0].type == OperationType.INSERT
-    assert isinstance(rows[0].obj, PersistentIdentifier)
+    assert rows[0].model == PersistentIdentifier
     assert rows[1].type == OperationType.INSERT
-    assert isinstance(rows[1].obj, FilesBucket)
+    assert rows[1].model == FilesBucket
     assert rows[2].type == OperationType.UPDATE
-    assert isinstance(rows[2].obj, PersistentIdentifier)
+    assert rows[2].model == PersistentIdentifier
     assert rows[3].type == OperationType.INSERT
-    assert isinstance(rows[3].obj, RDMDraftMetadata)
+    assert rows[3].model == RDMDraftMetadata
     assert rows[4].type == OperationType.INSERT
-    assert isinstance(rows[4].obj, RDMVersionState)
+    assert rows[4].model == RDMVersionState
 
 
 def test_create_draft_published_draft(
     state, draft_data, parent_data, bucket_data, pid_data
 ):
     # set existing parent so the action goes on the new version path
     state.PARENTS.add(
@@ -190,14 +190,14 @@
         draft=draft_data,
         parent=parent_data,
     )
     action = DraftCreateAction(data)
     rows = list(action.prepare())
     assert len(rows) == 4
     assert rows[0].type == OperationType.INSERT
-    assert isinstance(rows[0].obj, PersistentIdentifier)
+    assert rows[0].model == PersistentIdentifier
     assert rows[1].type == OperationType.INSERT
-    assert isinstance(rows[1].obj, FilesBucket)
+    assert rows[1].model == FilesBucket
     assert rows[2].type == OperationType.INSERT
-    assert isinstance(rows[2].obj, RDMDraftMetadata)
+    assert rows[2].model == RDMDraftMetadata
     assert rows[3].type == OperationType.UPDATE
-    assert isinstance(rows[3].obj, RDMVersionState)
+    assert rows[3].model == RDMVersionState
```

### Comparing `invenio-rdm-migrator-2.0.0/tests/streams/communities/conftest.py` & `invenio-rdm-migrator-3.0.0/tests/streams/communities/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/streams/communities/test_communities_load.py` & `invenio-rdm-migrator-3.0.0/tests/streams/communities/test_communities_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/streams/communities/test_communities_table_generator.py` & `invenio-rdm-migrator-3.0.0/tests/streams/communities/test_communities_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/streams/communities/test_communities_transform.py` & `invenio-rdm-migrator-3.0.0/tests/streams/communities/test_communities_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/streams/files/conftest.py` & `invenio-rdm-migrator-3.0.0/tests/streams/files/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/streams/files/test_files_load.py` & `invenio-rdm-migrator-3.0.0/tests/streams/files/test_files_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/streams/files/test_files_table_generator.py` & `invenio-rdm-migrator-3.0.0/tests/streams/files/test_files_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/streams/files/test_files_transform.py` & `invenio-rdm-migrator-3.0.0/tests/streams/files/test_files_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/streams/records/conftest.py` & `invenio-rdm-migrator-3.0.0/tests/streams/records/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/streams/records/test_records_table_generator.py` & `invenio-rdm-migrator-3.0.0/tests/streams/records/test_records_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/streams/requests/conftest.py` & `invenio-rdm-migrator-3.0.0/tests/streams/requests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/streams/requests/test_requests_load.py` & `invenio-rdm-migrator-3.0.0/tests/streams/requests/test_requests_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/streams/requests/test_requests_table_generator.py` & `invenio-rdm-migrator-3.0.0/tests/streams/requests/test_requests_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/streams/requests/test_requests_transform.py` & `invenio-rdm-migrator-3.0.0/tests/streams/requests/test_requests_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/streams/test_streams.py` & `invenio-rdm-migrator-3.0.0/tests/streams/test_streams.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/test_logging.py` & `invenio-rdm-migrator-3.0.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/test_state.py` & `invenio-rdm-migrator-3.0.0/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/test_utils.py` & `invenio-rdm-migrator-3.0.0/tests/test_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Utils tests."""
 
 import json
+import re
 from uuid import UUID
 
+import pytest
+
 from invenio_rdm_migrator.utils import JSONEncoder, dict_set, ts
 
 ###
 # timestamp
 ###
 
 
@@ -21,25 +24,41 @@
     assert isinstance(ts(), str)
 
 
 def test_current_timestamp():
     assert isinstance(ts(iso=False), float)
 
 
+def test_current_timestamp_fmt():
+    value = ts(fmt="%Y-%m-%dT%H:%M:%S")
+    exp = re.compile(r"\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}")
+    assert exp.match(value)
+
+
 ###
 # JSONEncoder
 ###
 
 
 def test_no_uuid_values():
     data = {"key1": "value1", "key2": 2, "key3": [1, 2, 3]}
     encoded_data = JSONEncoder().encode(data)
     assert encoded_data == json.dumps(data)
 
 
+def test_unknown_values():
+    class Unknown:
+        """Needed to trigger the encoder type error."""
+
+        pass
+
+    data = {"key": Unknown()}
+    pytest.raises(TypeError, JSONEncoder().encode, data)
+
+
 def test_uuid_values():
     data = {
         "key1": UUID("123e4567-e89b-12d3-a456-426655440000"),
     }
     expected_data = {
         "key1": "123e4567-e89b-12d3-a456-426655440000",
     }
@@ -75,21 +94,53 @@
     source = {"a": {"b": 1}}
     key = "a.b"
     value = 2
     dict_set(source, key, value)
     assert source == {"a": {"b": 2}}
 
 
+def test_set_list():
+    source = {"a": {}}
+    key = "a.b"
+    value = [1, 2]
+    dict_set(source, key, value)
+    assert source == {"a": {"b": [1, 2]}}
+
+
 def test_set_empty_root():
     source = {}
     key = "a.b"
     value = 6
     dict_set(source, key, value)
     assert source == {"a": {"b": 6}}
 
 
+def test_set_empty_root_list_key():
+    source = {}
+    key = ["a", "b"]
+    value = 6
+    dict_set(source, key, value)
+    assert source == {"a": {"b": 6}}
+
+
 def test_nested_dict():
     source = {"a": {"b": {}}}
     key = "a.b.c.d"
     value = 3
     dict_set(source, key, value)
     assert source == {"a": {"b": {"c": {"d": 3}}}}
+
+
+def test_int_key():
+    source = {1: ""}
+    key = 1
+    value = 3
+    # "lookup must be string or list"
+    pytest.raises(TypeError, dict_set, source, key, value)
+
+
+def test_no_key():
+    source = {"a": "value"}
+    key = None
+    value = 3
+    # ("No lookup key specified"
+    pytest.raises(KeyError, dict_set, source, key, value)
```

### Comparing `invenio-rdm-migrator-2.0.0/tests/transform/test_base_transform.py` & `invenio-rdm-migrator-3.0.0/tests/transform/test_base_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/transform/test_encrypt.py` & `invenio-rdm-migrator-3.0.0/tests/transform/test_encrypt.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,28 +10,14 @@
 import pytest
 from sqlalchemy_utils.types.encrypted.encrypted_type import AesEngine
 
 from invenio_rdm_migrator.transform import EncryptMixin, Transform
 
 
 @pytest.fixture(scope="function")
-def secret_keys_state(state):
-    """Adds secret keys to global state."""
-    state.VALUES.add(
-        "old_secret_key",
-        {"value": bytes("OLDKEY", "utf-8")},
-    )
-    state.VALUES.add(
-        "new_secret_key",
-        {"value": bytes("NEWKEY", "utf-8")},
-    )
-    return
-
-
-@pytest.fixture(scope="function")
 def transform_with_mixin():
     """Test instance of a transform class with identity mixin"""
 
     class FixtureTransform(Transform, EncryptMixin):
         """Transform fixture class."""
 
         def _token(self, entry):
```

### Comparing `invenio-rdm-migrator-2.0.0/tests/transform/test_identity.py` & `invenio-rdm-migrator-3.0.0/tests/transform/test_identity.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-2.0.0/tests/transform/test_transactions.py` & `invenio-rdm-migrator-3.0.0/tests/transform/test_transactions.py`

 * *Files identical despite different names*

