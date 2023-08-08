# Comparing `tmp/pyrtlib-1.0.0.tar.gz` & `tmp/pyrtlib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtlib-1.0.0.tar", last modified: Sun Aug  6 16:15:44 2023, max compression
+gzip compressed data, was "pyrtlib-1.0.1.tar", last modified: Mon Aug  7 07:35:05 2023, max compression
```

## Comparing `pyrtlib-1.0.0.tar` & `pyrtlib-1.0.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:15:44.531717 pyrtlib-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-06 16:15:44.531717 pyrtlib-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:15:44.527717 pyrtlib-1.0.0/pyrtlib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:15:44.527717 pyrtlib-1.0.0/pyrtlib/_lineshape/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r03.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r16.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r17.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r18.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r19.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r19sd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r20.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r20sd.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r21sd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r22sd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r98.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_makarov11.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r16.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r17.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r18.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r19.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r19sd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r20.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r20sd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r22.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r98.py
--rw-r--r--   0 runner    (1001) docker     (123)    34769 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/o3ll_r18.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/_lineshape/o3ll_r22.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:15:44.531717 pyrtlib-1.0.0/pyrtlib/apiwebservices/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/apiwebservices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/apiwebservices/eps_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/apiwebservices/erafive.py
--rw-r--r--   0 runner    (1001) docker     (123)    20148 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/apiwebservices/igra2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/apiwebservices/webservices.py
--rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/apiwebservices/wyomingupperair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:15:44.531717 pyrtlib-1.0.0/pyrtlib/climatology/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/climatology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/climatology/atmospheric_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    27854 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/climatology/extrapolation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:15:44.531717 pyrtlib-1.0.0/pyrtlib/pyrtlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-06 16:15:44.000000 pyrtlib-1.0.0/pyrtlib/pyrtlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-06 16:15:44.000000 pyrtlib-1.0.0/pyrtlib/pyrtlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 16:15:44.000000 pyrtlib-1.0.0/pyrtlib/pyrtlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-06 16:15:44.000000 pyrtlib-1.0.0/pyrtlib/pyrtlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-06 16:15:44.000000 pyrtlib-1.0.0/pyrtlib/pyrtlib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:15:44.531717 pyrtlib-1.0.0/pyrtlib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/tests/test_apiwebservices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/tests/test_main_ground.py
--rw-r--r--   0 runner    (1001) docker     (123)    15303 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/tests/test_main_sat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/tests/test_uncertainty.py
--rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:15:44.531717 pyrtlib-1.0.0/pyrtlib/uncertainty/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/uncertainty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22800 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/uncertainty/absmod_uncertainty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:15:44.531717 pyrtlib-1.0.0/pyrtlib/uncertainty/covariance_matrix/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/pyrtlib/uncertainty/covariance_matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-06 16:15:44.531717 pyrtlib-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-06 16:15:34.000000 pyrtlib-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:35:05.796389 pyrtlib-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-08-07 07:35:05.796389 pyrtlib-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:35:05.788390 pyrtlib-1.0.1/pyrtlib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:35:05.792389 pyrtlib-1.0.1/pyrtlib/_lineshape/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r19.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r19sd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r20sd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r21sd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r22sd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r98.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_makarov11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r19.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r19sd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r20sd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r22.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r98.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34769 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/o3ll_r18.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/_lineshape/o3ll_r22.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:35:05.796389 pyrtlib-1.0.1/pyrtlib/apiwebservices/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/apiwebservices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/apiwebservices/eps_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/apiwebservices/erafive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20148 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/apiwebservices/igra2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/apiwebservices/webservices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/apiwebservices/wyomingupperair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:35:05.796389 pyrtlib-1.0.1/pyrtlib/climatology/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/climatology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/climatology/atmospheric_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27854 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/climatology/extrapolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:35:05.796389 pyrtlib-1.0.1/pyrtlib/pyrtlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-08-07 07:35:05.000000 pyrtlib-1.0.1/pyrtlib/pyrtlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-07 07:35:05.000000 pyrtlib-1.0.1/pyrtlib/pyrtlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 07:35:05.000000 pyrtlib-1.0.1/pyrtlib/pyrtlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-07 07:35:05.000000 pyrtlib-1.0.1/pyrtlib/pyrtlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-07 07:35:05.000000 pyrtlib-1.0.1/pyrtlib/pyrtlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:35:05.796389 pyrtlib-1.0.1/pyrtlib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/tests/test_apiwebservices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/tests/test_main_ground.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15303 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/tests/test_main_sat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/tests/test_uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:35:05.796389 pyrtlib-1.0.1/pyrtlib/uncertainty/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/uncertainty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22800 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/uncertainty/absmod_uncertainty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:35:05.796389 pyrtlib-1.0.1/pyrtlib/uncertainty/covariance_matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/pyrtlib/uncertainty/covariance_matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-07 07:35:05.796389 pyrtlib-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-07 07:34:55.000000 pyrtlib-1.0.1/setup.py
```

### Comparing `pyrtlib-1.0.0/LICENSE` & `pyrtlib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/README.md` & `pyrtlib-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 <img align="" src="https://raw.githubusercontent.com/SatCloP/pyrtlib/main/resources/logo/logo_large_new.png" width="400">
 
 # A Radiative Transfer Python Library (non-scattering)
 
 [![docker-image-ci](https://github.com/SatCloP/pyrtlib/workflows/docker-image-ci/badge.svg)](https://github.com/SatCloP/pyrtlib/actions/workflows/docker-image.yml)
 [![run-python-tests](https://github.com/SatCloP/pyrtlib/workflows/run-python-tests/badge.svg)](https://github.com/SatCloP/pyrtlib/actions/workflows/ci.yml)
 [![build-docs-action](https://github.com/SatCloP/pyrtlib/workflows/build-docs-action/badge.svg)](https://github.com/SatCloP/pyrtlib/actions/workflows/build_docs.yml)
+
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
+[![PyPI Latest Release](https://img.shields.io/pypi/v/pyrtlib.svg)](https://pypi.org/project/pyrtlib/)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/SatCloP/pyrtlib?display_name=tag)
 [![codecov](https://codecov.io/gh/SatCloP/pyrtlib/branch/main/graph/badge.svg?token=7DV4B4U1OZ)](https://codecov.io/gh/SatCloP/pyrtlib)
-[![GitHub commits since tagged version](https://img.shields.io/github/commits-since/SatCloP/pyrtlib/v1.0.0)](https://github.com/SatCloP/pyrtlib/commits/)
+
 [![license](https://img.shields.io/github/license/SatCloP/pyrtlib.svg)](https://github.com/SatCloP/pyrtlib/blob/main/LICENSE)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1234.svg)](https://doi.org/10.5281/zenodo.1234)
+[![DOI](https://zenodo.org/badge/345925671.svg)](https://zenodo.org/badge/latestdoi/345925671)
+
+<!--[![GitHub commits since tagged version](https://img.shields.io/github/commits-since/SatCloP/pyrtlib/v1.0.0)](https://github.com/SatCloP/pyrtlib/commits/) -->
 <!--[![GitHub commit](https://img.shields.io/github/last-commit/slarosa/pyrtlib)](https://github.com/SatCloP/pyrtlib/commits/main)-->
 <!-- [![license](https://img.shields.io/github/license/slarosa/pyrtlib.svg)](https://github.com/SatCloP/pyrtlib/blob/main/LICENSE.md) -->
 
 PyRTlib is a Python package, for non-scattering line-by-line microwave RT simulations. PyRTlib is a user-friendly tool for computing down and up-welling brightness temperatures and related quantities (e.g., atmospheric absorption, optical depth, opacity) in Python.
 
 ![spectrum](https://raw.githubusercontent.com/SatCloP/pyrtlib/main/resources/spectrum_r22.jpeg)
```

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r03.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r03.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r16.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r16.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r17.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r17.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r18.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r18.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r19.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r19.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r19sd.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r19sd.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r20.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r20.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r20sd.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r20sd.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r21sd.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r21sd.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r22sd.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r22sd.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/h2oll_r98.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/h2oll_r98.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_makarov11.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_makarov11.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r03.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r03.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r16.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r16.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r17.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r17.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r18.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r18.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r19.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r19.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r19sd.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r19sd.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r20.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r20.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r20sd.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r20sd.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r22.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r22.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/o2ll_r98.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/o2ll_r98.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/_lineshape/o3ll_r18.py` & `pyrtlib-1.0.1/pyrtlib/_lineshape/o3ll_r18.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/apiwebservices/eps_sandbox.py` & `pyrtlib-1.0.1/pyrtlib/apiwebservices/eps_sandbox.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/apiwebservices/erafive.py` & `pyrtlib-1.0.1/pyrtlib/apiwebservices/erafive.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/apiwebservices/igra2.py` & `pyrtlib-1.0.1/pyrtlib/apiwebservices/igra2.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/apiwebservices/webservices.py` & `pyrtlib-1.0.1/pyrtlib/apiwebservices/webservices.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/apiwebservices/wyomingupperair.py` & `pyrtlib-1.0.1/pyrtlib/apiwebservices/wyomingupperair.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/climatology/atmospheric_profiles.py` & `pyrtlib-1.0.1/pyrtlib/climatology/atmospheric_profiles.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/climatology/extrapolation.py` & `pyrtlib-1.0.1/pyrtlib/climatology/extrapolation.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/pyrtlib.egg-info/SOURCES.txt` & `pyrtlib-1.0.1/pyrtlib/pyrtlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/tests/test_apiwebservices.py` & `pyrtlib-1.0.1/pyrtlib/tests/test_apiwebservices.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/tests/test_main_ground.py` & `pyrtlib-1.0.1/pyrtlib/tests/test_main_ground.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/tests/test_main_sat.py` & `pyrtlib-1.0.1/pyrtlib/tests/test_main_sat.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/tests/test_uncertainty.py` & `pyrtlib-1.0.1/pyrtlib/tests/test_uncertainty.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/tests/test_utils.py` & `pyrtlib-1.0.1/pyrtlib/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/uncertainty/absmod_uncertainty.py` & `pyrtlib-1.0.1/pyrtlib/uncertainty/absmod_uncertainty.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/pyrtlib/uncertainty/covariance_matrix/__init__.py` & `pyrtlib-1.0.1/pyrtlib/uncertainty/covariance_matrix/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrtlib-1.0.0/setup.py` & `pyrtlib-1.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 from setuptools import setup, find_packages
+import os
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
+def read_file(filename):
+    with open(os.path.join(os.path.dirname(__file__), filename)) as file:
+        return file.read()
+
 setup(
     name='pyrtlib',
-    version='1.0.0',
+    version='1.0.1',
     include_package_data=True,
     package_dir={'': 'pyrtlib'},
     python_requires='>=3.6',
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     install_requires=required,
+    project_urls={
+        'documentation': 'https://satclop.github.io/pyrtlib',
+        'repository': 'https://github.com/SatCloP/pyrtlib'
+    },
     url='',
     license='GPLv3',
     author='slarosa',
     author_email='salvatore-larosa@cnr.it',
     description='pyrtlib - Radiative Transfer library',
+    long_description=read_file('README.md'),
     long_description_content_type='text/markdown',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Education',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Topic :: Scientific/Engineering',
```

