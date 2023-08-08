# Comparing `tmp/sdssdb-0.6.2.tar.gz` & `tmp/sdssdb-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdssdb-0.6.2.tar", last modified: Sun Feb 12 20:32:48 2023, max compression
+gzip compressed data, was "sdssdb-0.6.4.tar", last modified: Tue Aug  8 20:32:15 2023, max compression
```

## Comparing `sdssdb-0.6.2.tar` & `sdssdb-0.6.4.tar`

### file list

```diff
@@ -1,69 +1,72 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-12 20:32:48.015323 sdssdb-0.6.2/
--rw-r--r--   0 runner     (501) staff       (20)     1504 2023-02-12 20:30:08.000000 sdssdb-0.6.2/LICENSE.md
--rw-r--r--   0 runner     (501) staff       (20)     2185 2023-02-12 20:32:48.015520 sdssdb-0.6.2/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1215 2023-02-12 20:30:08.000000 sdssdb-0.6.2/README.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-12 20:32:47.981858 sdssdb-0.6.2/python/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-12 20:32:47.990915 sdssdb-0.6.2/python/sdssdb/
--rw-r--r--   0 runner     (501) staff       (20)      586 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    22028 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/connection.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-12 20:32:47.994376 sdssdb-0.6.2/python/sdssdb/etc/
--rw-r--r--   0 runner     (501) staff       (20)     1268 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/etc/sdssdb.yml
--rw-r--r--   0 runner     (501) staff       (20)     1789 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/exceptions.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-12 20:32:47.994836 sdssdb-0.6.2/python/sdssdb/peewee/
--rw-r--r--   0 runner     (501) staff       (20)    13557 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/peewee/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-12 20:32:47.996970 sdssdb-0.6.2/python/sdssdb/peewee/operationsdb/
--rw-r--r--   0 runner     (501) staff       (20)      668 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/peewee/operationsdb/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    10312 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/peewee/operationsdb/apogeeqldb.py
--rw-r--r--   0 runner     (501) staff       (20)     6387 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/peewee/operationsdb/mangadb.py
--rw-r--r--   0 runner     (501) staff       (20)    28649 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/peewee/operationsdb/platedb.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-12 20:32:48.000656 sdssdb-0.6.2/python/sdssdb/peewee/sdss5db/
--rw-r--r--   0 runner     (501) staff       (20)      998 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/peewee/sdss5db/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2040 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/peewee/sdss5db/apogee_drpdb.py
--rw-r--r--   0 runner     (501) staff       (20)    61795 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/peewee/sdss5db/catalogdb.py
--rw-r--r--   0 runner     (501) staff       (20)     6383 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/peewee/sdss5db/deprecated.py
--rw-r--r--   0 runner     (501) staff       (20)     9383 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/peewee/sdss5db/opsdb.py
--rw-r--r--   0 runner     (501) staff       (20)    10607 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/peewee/sdss5db/sandbox.py
--rw-r--r--   0 runner     (501) staff       (20)    16448 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/peewee/sdss5db/targetdb.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-12 20:32:48.001194 sdssdb-0.6.2/python/sdssdb/sqlalchemy/
--rw-r--r--   0 runner     (501) staff       (20)     4785 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-12 20:32:48.002172 sdssdb-0.6.2/python/sdssdb/sqlalchemy/archive/
--rw-r--r--   0 runner     (501) staff       (20)      832 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/archive/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6609 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/archive/sas.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-12 20:32:48.004998 sdssdb-0.6.2/python/sdssdb/sqlalchemy/mangadb/
--rw-r--r--   0 runner     (501) staff       (20)      782 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/mangadb/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1177 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/mangadb/auxdb.py
--rw-r--r--   0 runner     (501) staff       (20)    10958 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/mangadb/dapdb.py
--rw-r--r--   0 runner     (501) staff       (20)    22440 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/mangadb/datadb.py
--rw-r--r--   0 runner     (501) staff       (20)    10213 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/mangadb/sampledb.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-12 20:32:48.007192 sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/
--rw-r--r--   0 runner     (501) staff       (20)      724 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2979 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/apogeeqldb.py
--rw-r--r--   0 runner     (501) staff       (20)     6523 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/mangadb.py
--rw-r--r--   0 runner     (501) staff       (20)    40377 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/platedb.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-12 20:32:48.010957 sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/tools/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/tools/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3418 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/tools/astrodatetime.py
--rw-r--r--   0 runner     (501) staff       (20)    33824 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/tools/convert.py
--rw-r--r--   0 runner     (501) staff       (20)     2072 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/tools/dateObs2HA.py
--rw-r--r--   0 runner     (501) staff       (20)    21382 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/tools/geometry.py
--rw-r--r--   0 runner     (501) staff       (20)     6597 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/tools/moon.py
--rw-r--r--   0 runner     (501) staff       (20)     1821 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/tools/sun.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-12 20:32:48.013985 sdssdb-0.6.2/python/sdssdb/utils/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/utils/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3613 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/utils/adaptors.py
--rw-r--r--   0 runner     (501) staff       (20)    18463 2023-02-12 20:30:09.000000 sdssdb-0.6.2/python/sdssdb/utils/ingest.py
--rw-r--r--   0 runner     (501) staff       (20)    11140 2023-02-12 20:30:10.000000 sdssdb-0.6.2/python/sdssdb/utils/internals.py
--rw-r--r--   0 runner     (501) staff       (20)     5991 2023-02-12 20:30:10.000000 sdssdb-0.6.2/python/sdssdb/utils/registry.py
--rw-r--r--   0 runner     (501) staff       (20)    11512 2023-02-12 20:30:10.000000 sdssdb-0.6.2/python/sdssdb/utils/schemadisplay.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-12 20:32:47.993927 sdssdb-0.6.2/python/sdssdb.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2185 2023-02-12 20:32:47.000000 sdssdb-0.6.2/python/sdssdb.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2047 2023-02-12 20:32:47.000000 sdssdb-0.6.2/python/sdssdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-02-12 20:32:47.000000 sdssdb-0.6.2/python/sdssdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-02-12 20:32:36.000000 sdssdb-0.6.2/python/sdssdb.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)      480 2023-02-12 20:32:47.000000 sdssdb-0.6.2/python/sdssdb.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        7 2023-02-12 20:32:47.000000 sdssdb-0.6.2/python/sdssdb.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     2214 2023-02-12 20:32:48.016981 sdssdb-0.6.2/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)       73 2023-02-12 20:30:13.000000 sdssdb-0.6.2/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-12 20:32:48.014948 sdssdb-0.6.2/tests/
--rw-r--r--   0 runner     (501) staff       (20)     1372 2023-02-12 20:30:14.000000 sdssdb-0.6.2/tests/test_connection.py
--rw-r--r--   0 runner     (501) staff       (20)     2008 2023-02-12 20:30:14.000000 sdssdb-0.6.2/tests/test_utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-08 20:32:15.812139 sdssdb-0.6.4/
+-rw-r--r--   0 runner     (501) staff       (20)     1504 2023-08-08 20:31:30.000000 sdssdb-0.6.4/LICENSE.md
+-rw-r--r--   0 runner     (501) staff       (20)     2185 2023-08-08 20:32:15.812361 sdssdb-0.6.4/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1215 2023-08-08 20:31:30.000000 sdssdb-0.6.4/README.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-08 20:32:15.768932 sdssdb-0.6.4/python/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-08 20:32:15.777975 sdssdb-0.6.4/python/sdssdb/
+-rw-r--r--   0 runner     (501) staff       (20)      586 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    21972 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/connection.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-08 20:32:15.782807 sdssdb-0.6.4/python/sdssdb/etc/
+-rw-r--r--   0 runner     (501) staff       (20)     1468 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/etc/sdssdb.yml
+-rw-r--r--   0 runner     (501) staff       (20)     1789 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/exceptions.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-08 20:32:15.783471 sdssdb-0.6.4/python/sdssdb/peewee/
+-rw-r--r--   0 runner     (501) staff       (20)    13557 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/peewee/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-08 20:32:15.784911 sdssdb-0.6.4/python/sdssdb/peewee/lvmdb/
+-rw-r--r--   0 runner     (501) staff       (20)      876 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/peewee/lvmdb/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5968 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/peewee/lvmdb/lvmopsdb.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-08 20:32:15.787391 sdssdb-0.6.4/python/sdssdb/peewee/operationsdb/
+-rw-r--r--   0 runner     (501) staff       (20)      668 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/peewee/operationsdb/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    10312 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/peewee/operationsdb/apogeeqldb.py
+-rw-r--r--   0 runner     (501) staff       (20)     6387 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/peewee/operationsdb/mangadb.py
+-rw-r--r--   0 runner     (501) staff       (20)    28649 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/peewee/operationsdb/platedb.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-08 20:32:15.792892 sdssdb-0.6.4/python/sdssdb/peewee/sdss5db/
+-rw-r--r--   0 runner     (501) staff       (20)      998 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/peewee/sdss5db/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2040 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/peewee/sdss5db/apogee_drpdb.py
+-rw-r--r--   0 runner     (501) staff       (20)    62977 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/peewee/sdss5db/catalogdb.py
+-rw-r--r--   0 runner     (501) staff       (20)     6383 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/peewee/sdss5db/deprecated.py
+-rw-r--r--   0 runner     (501) staff       (20)     9940 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/peewee/sdss5db/opsdb.py
+-rw-r--r--   0 runner     (501) staff       (20)    11763 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/peewee/sdss5db/sandbox.py
+-rw-r--r--   0 runner     (501) staff       (20)    17219 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/peewee/sdss5db/targetdb.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-08 20:32:15.793526 sdssdb-0.6.4/python/sdssdb/sqlalchemy/
+-rw-r--r--   0 runner     (501) staff       (20)     4785 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-08 20:32:15.794549 sdssdb-0.6.4/python/sdssdb/sqlalchemy/archive/
+-rw-r--r--   0 runner     (501) staff       (20)      832 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/archive/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6609 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/archive/sas.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-08 20:32:15.798080 sdssdb-0.6.4/python/sdssdb/sqlalchemy/mangadb/
+-rw-r--r--   0 runner     (501) staff       (20)      782 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/mangadb/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1177 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/mangadb/auxdb.py
+-rw-r--r--   0 runner     (501) staff       (20)    10958 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/mangadb/dapdb.py
+-rw-r--r--   0 runner     (501) staff       (20)    22440 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/mangadb/datadb.py
+-rw-r--r--   0 runner     (501) staff       (20)    10213 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/mangadb/sampledb.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-08 20:32:15.800524 sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/
+-rw-r--r--   0 runner     (501) staff       (20)      724 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2979 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/apogeeqldb.py
+-rw-r--r--   0 runner     (501) staff       (20)     6523 2023-08-08 20:31:30.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/mangadb.py
+-rw-r--r--   0 runner     (501) staff       (20)    40377 2023-08-08 20:31:31.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/platedb.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-08 20:32:15.805579 sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/tools/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-08-08 20:31:31.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/tools/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3418 2023-08-08 20:31:31.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/tools/astrodatetime.py
+-rw-r--r--   0 runner     (501) staff       (20)    33824 2023-08-08 20:31:31.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/tools/convert.py
+-rw-r--r--   0 runner     (501) staff       (20)     2072 2023-08-08 20:31:31.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/tools/dateObs2HA.py
+-rw-r--r--   0 runner     (501) staff       (20)    21382 2023-08-08 20:31:31.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/tools/geometry.py
+-rw-r--r--   0 runner     (501) staff       (20)     6597 2023-08-08 20:31:31.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/tools/moon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1821 2023-08-08 20:31:31.000000 sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/tools/sun.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-08 20:32:15.810346 sdssdb-0.6.4/python/sdssdb/utils/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-08-08 20:31:31.000000 sdssdb-0.6.4/python/sdssdb/utils/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3613 2023-08-08 20:31:31.000000 sdssdb-0.6.4/python/sdssdb/utils/adaptors.py
+-rw-r--r--   0 runner     (501) staff       (20)    18463 2023-08-08 20:31:31.000000 sdssdb-0.6.4/python/sdssdb/utils/ingest.py
+-rw-r--r--   0 runner     (501) staff       (20)    11140 2023-08-08 20:31:31.000000 sdssdb-0.6.4/python/sdssdb/utils/internals.py
+-rw-r--r--   0 runner     (501) staff       (20)     5991 2023-08-08 20:31:31.000000 sdssdb-0.6.4/python/sdssdb/utils/registry.py
+-rw-r--r--   0 runner     (501) staff       (20)    11512 2023-08-08 20:31:31.000000 sdssdb-0.6.4/python/sdssdb/utils/schemadisplay.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-08 20:32:15.782119 sdssdb-0.6.4/python/sdssdb.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     2185 2023-08-08 20:32:15.000000 sdssdb-0.6.4/python/sdssdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2125 2023-08-08 20:32:15.000000 sdssdb-0.6.4/python/sdssdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-08-08 20:32:15.000000 sdssdb-0.6.4/python/sdssdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-08-08 20:32:05.000000 sdssdb-0.6.4/python/sdssdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)      492 2023-08-08 20:32:15.000000 sdssdb-0.6.4/python/sdssdb.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        7 2023-08-08 20:32:15.000000 sdssdb-0.6.4/python/sdssdb.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     2227 2023-08-08 20:32:15.814117 sdssdb-0.6.4/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)       73 2023-08-08 20:31:31.000000 sdssdb-0.6.4/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-08 20:32:15.811642 sdssdb-0.6.4/tests/
+-rw-r--r--   0 runner     (501) staff       (20)     1372 2023-08-08 20:31:31.000000 sdssdb-0.6.4/tests/test_connection.py
+-rw-r--r--   0 runner     (501) staff       (20)     2008 2023-08-08 20:31:31.000000 sdssdb-0.6.4/tests/test_utils.py
```

### Comparing `sdssdb-0.6.2/LICENSE.md` & `sdssdb-0.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/PKG-INFO` & `sdssdb-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdssdb
-Version: 0.6.2
+Version: 0.6.4
 Summary: SDSS product for database management
 Home-page: https://github.com/sdss/sdssdb
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/sdssdb
 Project-URL: Documentation, https://sdssdb.readthedocs.org
```

### Comparing `sdssdb-0.6.2/README.rst` & `sdssdb-0.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/__init__.py` & `sdssdb-0.6.4/python/sdssdb/__init__.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/connection.py` & `sdssdb-0.6.4/python/sdssdb/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                             self._config['host'] = None
                         break
 
         if connect:
             if self.connected and self.profile == previous_profile:
                 pass
             elif self.dbname is not None:
-                self.connect()
+                self.connect(**self._config)
 
         return self.connected
 
     @abc.abstractmethod
     def _conn(self, dbname, **params):
         """Actually initialises the database connection.
 
@@ -233,16 +233,14 @@
         dbname = dbname or self.dbname
         if dbname is None:
             raise RuntimeError('the database name was not set when '
                                'DatabaseConnection was instantiated. '
                                'To set it in runtime change the dbname '
                                'attribute.')
 
-        params = {key: params[key] for key in params if params[key]}
-
         return self._conn(dbname, **params)
 
     @staticmethod
     def list_profiles(profile=None):
         """Returns a list of profiles.
 
         Parameters
```

### Comparing `sdssdb-0.6.2/python/sdssdb/etc/sdssdb.yml` & `sdssdb-0.6.4/python/sdssdb/etc/sdssdb.yml`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,21 @@
 lco:
     user: sdssdb
     admin: sdssdb_admin
     host: sdss4-db
     port: 5432
     domain: lco.cl
 
+lvm:
+    user: sdss_user
+    admin: sdss
+    host: lvm-webapp
+    port: 5432
+    domain: lvm-[a-z0-9]+.lco.cl
+
 local:
     domain: null
 
 lore:
     user: marvin
     host: localhost
     port: 5432
@@ -51,14 +58,19 @@
 operations:
     user: sdss_user
     admin: sdss
     host: operations.sdss.org
     port: 5432
     domain: operations.sdss.*
 
+pipelines:
+    host: pipelines.sdss.org
+    port: 5432
+    domain: pipelines.sdss.*
+    
 manga:
     user: sdss
     host: manga.wasatch.peaks
     port: 5432
     domain: manga.wasatch.peaks
 
 utahdb:
```

### Comparing `sdssdb-0.6.2/python/sdssdb/exceptions.py` & `sdssdb-0.6.4/python/sdssdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/peewee/__init__.py` & `sdssdb-0.6.4/python/sdssdb/peewee/__init__.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/peewee/operationsdb/__init__.py` & `sdssdb-0.6.4/python/sdssdb/peewee/operationsdb/__init__.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/peewee/operationsdb/apogeeqldb.py` & `sdssdb-0.6.4/python/sdssdb/peewee/operationsdb/apogeeqldb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/peewee/operationsdb/mangadb.py` & `sdssdb-0.6.4/python/sdssdb/peewee/operationsdb/mangadb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/peewee/operationsdb/platedb.py` & `sdssdb-0.6.4/python/sdssdb/peewee/operationsdb/platedb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/peewee/sdss5db/__init__.py` & `sdssdb-0.6.4/python/sdssdb/peewee/sdss5db/__init__.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/peewee/sdss5db/apogee_drpdb.py` & `sdssdb-0.6.4/python/sdssdb/peewee/sdss5db/apogee_drpdb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/peewee/sdss5db/catalogdb.py` & `sdssdb-0.6.4/python/sdssdb/peewee/sdss5db/catalogdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,30 @@
 
         RUN_N_BITS = 11  # Number of left-most bits reserved for the run_id
         run_id_mask = (2**RUN_N_BITS - 1) << (64 - RUN_N_BITS)
 
         return (self.catalogid & run_id_mask) >> (64 - RUN_N_BITS)
 
 
+class Catalog_ver25_to_ver31_full_unique(CatalogdbModel):
+
+    id = BigIntegerField(primary_key=True)
+
+    class Meta:
+        table_name = 'catalog_ver25_to_ver31_full_unique'
+
+
+class Catalog_ver25_to_ver31_full_all(CatalogdbModel):
+
+    id = BigIntegerField(primary_key=True)
+
+    class Meta:
+        table_name = 'catalog_ver25_to_ver31_full_all'
+
+
 class AllWise(CatalogdbModel):
 
     cntr = BigIntegerField(primary_key=True)
     designation = TextField()
     tmass_key = BigIntegerField()
 
     class Meta:
@@ -1925,14 +1941,22 @@
                           column_name='panstarrs1_catid_objid',
                           backref='+')
 
     class Meta:
         table_name = 'bhm_rm_v1'
 
 
+class BHM_RM_v1_1(BHM_RM_v1):
+    pass
+
+
+class BHM_RM_v1_3(BHM_RM_v1):
+    pass
+
+
 class BHM_RM_v0_2(BHM_RM_v0):
     pass
 
 
 class BHM_RM_Tweaks(CatalogdbModel):
 
     pkey = BigIntegerField(primary_key=True)
@@ -2069,64 +2093,99 @@
 
     objid = BigIntegerField(primary_key=True)
 
     class Meta:
         table_name = 'supercosmos'
 
 
+class RAVE_DR6_Gauguin_Madera(CatalogdbModel):
+
+    rave_obs_id = TextField(primary_key=True)
+
+    class Meta:
+        table_name = 'rave_dr6_gauguin_madera'
+
+
+class RAVE_DR6_Gaia_DR3_XMatch(CatalogdbModel):
+
+    obsid = TextField(primary_key=True)
+
+    class Meta:
+        table_name = 'rave_dr6_xgaiae3'
+
+
+class Gaia_Stellar_Parameters(CatalogdbModel):
+
+    gdr3_source_id = BigIntegerField(primary_key=True)
+
+    gaia = ForeignKeyField(Gaia_DR3,
+                           field='source_id',
+                           column_name='gdr3_source_id',
+                           object_id_name='gdr3_source_id',
+                           backref='stellar_parameters')
+
+    class Meta:
+        table_name = 'gaia_stellar_parameters'
+
+
 _Gaia_DR2_TwoMass_Deferred.set_model(Gaia_DR2_TwoMass_Best_Neighbour)
 _APOGEE_Star_Visit_Deferred.set_model(SDSS_DR16_APOGEE_Star_AllVisit)
 
 
 # Add relational tables to namespace.
 if database.connected and database.is_connection_usable():
     all_tables = database.get_tables('catalogdb')
 else:
     all_tables = []
 
 for rtname in all_tables:
     if rtname.startswith('catalog_to_'):
-
-        tname = rtname[len('catalog_to_'):]
-        fname = 'catalogdb.' + tname
-
-        if fname not in database.models:
-            warnings.warn(f'{rtname}: cannot find related table {tname!r}',
-                          SdssdbUserWarning)
-            continue
-
-        rel_model = database.models[fname]
-        model_name = 'CatalogTo' + rel_model.__name__
-
-        class Meta:
-            table_name = rtname
-            primary_key = False
-
-        RelationalModel = type(model_name, (CatalogdbModel,), {'Meta': Meta})
-
-        RelationalModel._meta.add_field('catalog',
-                                        ForeignKeyField(Catalog,
-                                                        column_name='catalogid',
-                                                        backref='+'))
-        RelationalModel._meta.add_field('target',
-                                        ForeignKeyField(rel_model,
+        direction = 'to'
+    elif rtname.startswith('catalog_from_'):
+        direction = 'from'
+    else:
+        continue
+
+    tname = rtname[len(f'catalog_{direction}_'):]
+    fname = 'catalogdb.' + tname
+
+    if fname not in database.models:
+        warnings.warn(f'{rtname}: cannot find related table {tname!r}',
+                      SdssdbUserWarning)
+        continue
+
+    rel_model = database.models[fname]
+    model_name = f'Catalog{direction.capitalize()}' + rel_model.__name__
+
+    class Meta:
+        table_name = rtname
+        primary_key = False
+
+    RelationalModel = type(model_name, (CatalogdbModel,), {'Meta': Meta})
+
+    RelationalModel._meta.add_field('catalog',
+                                    ForeignKeyField(Catalog,
+                                                    column_name='catalogid',
+                                                    backref='+'))
+    RelationalModel._meta.add_field('target',
+                                    ForeignKeyField(rel_model,
+                                                    column_name='target_id',
+                                                    backref='+'))
+    RelationalModel._meta.add_field('version',
+                                    ForeignKeyField(Version,
+                                                    column_name='version_id',
+                                                    backref='+'))
+
+    # Add a many-to-many to Catalog
+    Catalog._meta.add_field(rel_model.__name__.lower(),
+                            ManyToManyField(rel_model,
+                                            through_model=RelationalModel,
+                                            backref='+'))
+
+    if tname == 'sdss_dr13_photoobj_primary':
+        RelationalModel._meta.add_field('sdss_dr13_photoobj',
+                                        ForeignKeyField(SDSS_DR13_PhotoObj,
                                                         column_name='target_id',
+                                                        field='objid',
                                                         backref='+'))
-        RelationalModel._meta.add_field('version',
-                                        ForeignKeyField(Version,
-                                                        column_name='version_id',
-                                                        backref='+'))
-
-        # Add a many-to-many to Catalog
-        Catalog._meta.add_field(rel_model.__name__.lower(),
-                                ManyToManyField(rel_model,
-                                                through_model=RelationalModel,
-                                                backref='+'))
-
-        if tname == 'sdss_dr13_photoobj_primary':
-            RelationalModel._meta.add_field('sdss_dr13_photoobj',
-                                            ForeignKeyField(SDSS_DR13_PhotoObj,
-                                                            column_name='target_id',
-                                                            field='objid',
-                                                            backref='+'))
 
-        globals()[model_name] = RelationalModel
+    globals()[model_name] = RelationalModel
```

### Comparing `sdssdb-0.6.2/python/sdssdb/peewee/sdss5db/deprecated.py` & `sdssdb-0.6.4/python/sdssdb/peewee/sdss5db/deprecated.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/peewee/sdss5db/opsdb.py` & `sdssdb-0.6.4/python/sdssdb/peewee/sdss5db/opsdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -297,8 +297,30 @@
         if returnPositions:
             return positions
 
     class Meta:
         table_name = "queue"
 
 
+class PriorityVersion(OpsdbBase):
+    pk = AutoField()
+    label = TextField()
+
+    class Meta:
+        table_name = 'priority_version'
+
+
+class BasePriority(OpsdbBase):
+    pk = AutoField()
+    priority = IntegerField()
+    field = ForeignKeyField(targetdb.Field,
+                            column_name='field_pk',
+                            field='pk')
+    version = ForeignKeyField(PriorityVersion,
+                              column_name='version_pk',
+                              field='pk')
+
+    class Meta:
+        table_name = 'base_priority'
+
+
 FieldToPriorityDeferred.set_model(FieldToPriority)
```

### Comparing `sdssdb-0.6.2/python/sdssdb/peewee/sdss5db/sandbox.py` & `sdssdb-0.6.4/python/sdssdb/peewee/sdss5db/sandbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -315,7 +315,49 @@
 
     class Meta:
         table_name = 'magnitude'
 
 
 # AssignmentDeferred.set_model(Assignment)
 CartonToTargetDeferred.set_model(CartonToTarget)
+
+
+class Plate(TargetdbBase):
+    plate_id = IntegerField(null=False)
+    racen = FloatField()
+    deccen = FloatField()
+    cadence = TextField()
+    mode = TextField()
+    equiv_designs = IntegerField()
+
+    class Meta:
+        table_name = 'plate'
+
+
+class PlateToCatalog(TargetdbBase):
+    pk = AutoField()
+    plate_id = ForeignKeyField(column_name='plate_id',
+                               field='plate_id',
+                               model=Plate,
+                               null=False)
+    catalogid = ForeignKeyField(column_name='catalogid',
+                                field='catalogid',
+                                model=catalogdb.Catalog,
+                                null=False)
+
+    class Meta:
+        table_name = 'plate_to_catalog'
+
+
+class Epoch(TargetdbBase):
+    pk = AutoField()
+    plate_id = ForeignKeyField(column_name='plate_id',
+                               field='plate_id',
+                               model=Plate,
+                               null=False)
+    apogee_sn2 = FloatField()
+    r_sn2 = FloatField()
+    b_sn2 = FloatField()
+    mjd = FloatField()
+
+    class Meta:
+        table_name = 'epoch'
```

### Comparing `sdssdb-0.6.2/python/sdssdb/peewee/sdss5db/targetdb.py` & `sdssdb-0.6.4/python/sdssdb/peewee/sdss5db/targetdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,30 +5,18 @@
 # @Date: 2018-09-22
 # @Filename: targetdb.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 import datetime
 import os
 
-from peewee import (
-    SQL,
-    AutoField,
-    BigIntegerField,
-    BooleanField,
-    DateTimeField,
-    DeferredThroughModel,
-    DoubleField,
-    FloatField,
-    ForeignKeyField,
-    IntegerField,
-    SmallIntegerField,
-    TextField,
-    UUIDField,
-    fn
-)
+from peewee import (SQL, AutoField, BigIntegerField, BooleanField,
+                    DateTimeField, DeferredThroughModel, DoubleField,
+                    FloatField, ForeignKeyField, IntegerField,
+                    SmallIntegerField, TextField, UUIDField, fn)
 from playhouse.postgres_ext import ArrayField
 
 from .. import BaseModel
 from . import catalogdb, database  # noqa
 
 
 class TargetdbBase(BaseModel):
@@ -54,15 +42,16 @@
 
 
 class ObsMode(TargetdbBase):
     label = TextField(null=False)
     min_moon_sep = FloatField(null=True)
     min_deltav_ks91 = FloatField(null=True)
     min_twilight_ang = FloatField(null=True)
-    max_airmass = FloatField(null=True)
+    max_airmass_apo = FloatField(null=True)
+    max_airmass_lco = FloatField(null=True)
 
     class Meta:
         table_name = 'obsmode'
 
 
 class Cadence(TargetdbBase):
     label = TextField(null=False)
@@ -424,14 +413,36 @@
                                        model=CartonToTarget,
                                        backref='magnitudes')
 
     class Meta:
         table_name = 'magnitude'
 
 
+class RevisedMagnitude(TargetdbBase):
+    bp = FloatField(null=True)
+    g = FloatField(null=True)
+    h = FloatField(null=True)
+    i = FloatField(null=True)
+    z = FloatField(null=True)
+    pk = AutoField()
+    r = FloatField(null=True)
+    rp = FloatField(null=True)
+    gaia_g = FloatField(null=True)
+    j = FloatField(null=True)
+    k = FloatField(null=True)
+    optical_prov = TextField(null=True)
+    carton_to_target = ForeignKeyField(column_name='carton_to_target_pk',
+                                       field='pk',
+                                       model=CartonToTarget,
+                                       backref='revised_magnitudes')
+
+    class Meta:
+        table_name = 'revised_magnitude'
+
+
 class AssignedTargets(TargetdbBase):
     program = TextField()
     carton_pk = ForeignKeyField(column_name="carton_pk",
                                 field="pk",
                                 model=Carton)
     c2t_pk = ForeignKeyField(column_name="c2t_pk",
                              field="pk",
```

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/__init__.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/archive/__init__.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/archive/sas.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/archive/sas.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/mangadb/__init__.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/mangadb/__init__.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/mangadb/auxdb.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/mangadb/auxdb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/mangadb/dapdb.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/mangadb/dapdb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/mangadb/datadb.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/mangadb/datadb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/mangadb/sampledb.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/mangadb/sampledb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/__init__.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/__init__.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/apogeeqldb.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/apogeeqldb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/mangadb.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/mangadb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/platedb.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/platedb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/tools/astrodatetime.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/tools/astrodatetime.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/tools/convert.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/tools/convert.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/tools/dateObs2HA.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/tools/dateObs2HA.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/tools/geometry.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/tools/geometry.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/tools/moon.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/tools/moon.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/sqlalchemy/operationsdb/tools/sun.py` & `sdssdb-0.6.4/python/sdssdb/sqlalchemy/operationsdb/tools/sun.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/utils/adaptors.py` & `sdssdb-0.6.4/python/sdssdb/utils/adaptors.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/utils/ingest.py` & `sdssdb-0.6.4/python/sdssdb/utils/ingest.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/utils/internals.py` & `sdssdb-0.6.4/python/sdssdb/utils/internals.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/utils/registry.py` & `sdssdb-0.6.4/python/sdssdb/utils/registry.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb/utils/schemadisplay.py` & `sdssdb-0.6.4/python/sdssdb/utils/schemadisplay.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/python/sdssdb.egg-info/PKG-INFO` & `sdssdb-0.6.4/python/sdssdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdssdb
-Version: 0.6.2
+Version: 0.6.4
 Summary: SDSS product for database management
 Home-page: https://github.com/sdss/sdssdb
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/sdssdb
 Project-URL: Documentation, https://sdssdb.readthedocs.org
```

### Comparing `sdssdb-0.6.2/python/sdssdb.egg-info/SOURCES.txt` & `sdssdb-0.6.4/python/sdssdb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 python/sdssdb.egg-info/SOURCES.txt
 python/sdssdb.egg-info/dependency_links.txt
 python/sdssdb.egg-info/not-zip-safe
 python/sdssdb.egg-info/requires.txt
 python/sdssdb.egg-info/top_level.txt
 python/sdssdb/etc/sdssdb.yml
 python/sdssdb/peewee/__init__.py
+python/sdssdb/peewee/lvmdb/__init__.py
+python/sdssdb/peewee/lvmdb/lvmopsdb.py
 python/sdssdb/peewee/operationsdb/__init__.py
 python/sdssdb/peewee/operationsdb/apogeeqldb.py
 python/sdssdb/peewee/operationsdb/mangadb.py
 python/sdssdb/peewee/operationsdb/platedb.py
 python/sdssdb/peewee/sdss5db/__init__.py
 python/sdssdb/peewee/sdss5db/apogee_drpdb.py
 python/sdssdb/peewee/sdss5db/catalogdb.py
```

### Comparing `sdssdb-0.6.2/setup.cfg` & `sdssdb-0.6.4/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sdssdb
-version = 0.6.2
+version = 0.6.4
 author = José Sánchez-Gallego
 author_email = gallegoj@uw.edu
 description = SDSS product for database management
 url = https://github.com/sdss/sdssdb
 project_urls = 
 	Repository = https://github.com/sdss/sdssdb
 	Documentation = https://sdssdb.readthedocs.org
@@ -36,14 +36,15 @@
 	pgpasslib>=1.1.0
 	psycopg2-binary>=2.7.7
 	six>=1.12.0
 	peewee>=3.9.6
 	sqlalchemy>=1.3.6
 	sdsstools>=0.1.11
 	numpy>=1.18.2
+	h5py>=3.8.0
 
 [options.packages.find]
 where = 
 	python
 exclude = 
 	*.tests
```

### Comparing `sdssdb-0.6.2/tests/test_connection.py` & `sdssdb-0.6.4/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.6.2/tests/test_utils.py` & `sdssdb-0.6.4/tests/test_utils.py`

 * *Files identical despite different names*

