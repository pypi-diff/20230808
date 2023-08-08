# Comparing `tmp/chainlib-0.5.0.tar.gz` & `tmp/chainlib-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlib-0.5.0.tar", last modified: Sun Aug  6 12:53:10 2023, max compression
+gzip compressed data, was "chainlib-0.5.1.tar", last modified: Tue Aug  8 18:09:40 2023, max compression
```

## Comparing `chainlib-0.5.0.tar` & `chainlib-0.5.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:53:10.779686 chainlib-0.5.0/
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:02:45.000000 chainlib-0.5.0/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)      116 2023-06-03 10:49:41.000000 chainlib-0.5.0/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)    15563 2023-08-06 12:53:10.779686 chainlib-0.5.0/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)    14796 2023-06-03 10:49:46.000000 chainlib-0.5.0/README.md
--rw-r--r--   0 lash      (1000) lash      (1000)      868 2022-11-14 07:03:32.000000 chainlib-0.5.0/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1621 2022-11-14 07:04:27.000000 chainlib-0.5.0/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:53:10.776353 chainlib-0.5.0/chainlib/
--rw-r--r--   0 lash      (1000) lash      (1000)      699 2021-10-10 10:19:14.000000 chainlib-0.5.0/chainlib/auth.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1341 2023-02-10 19:31:04.000000 chainlib-0.5.0/chainlib/block.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5667 2021-12-21 15:02:23.000000 chainlib-0.5.0/chainlib/chain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:53:10.776353 chainlib-0.5.0/chainlib/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)      107 2022-11-04 07:26:52.000000 chainlib-0.5.0/chainlib/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6547 2023-08-06 12:08:07.000000 chainlib-0.5.0/chainlib/cli/arg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4911 2023-08-06 12:07:36.000000 chainlib-0.5.0/chainlib/cli/config.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1833 2023-02-14 06:42:51.000000 chainlib-0.5.0/chainlib/cli/gen.py
--rw-r--r--   0 lash      (1000) lash      (1000)      312 2023-02-14 06:42:51.000000 chainlib-0.5.0/chainlib/cli/log.py
--rw-r--r--   0 lash      (1000) lash      (1000)    12465 2022-11-12 13:30:44.000000 chainlib-0.5.0/chainlib/cli/man.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4567 2023-08-06 11:27:49.000000 chainlib-0.5.0/chainlib/cli/rpc.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4477 2022-11-03 17:13:57.000000 chainlib-0.5.0/chainlib/cli/wallet.py
--rw-r--r--   0 lash      (1000) lash      (1000)    13401 2023-08-06 11:50:17.000000 chainlib-0.5.0/chainlib/connection.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:53:10.773020 chainlib-0.5.0/chainlib/data/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:53:10.776353 chainlib-0.5.0/chainlib/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)      239 2023-08-06 12:04:30.000000 chainlib-0.5.0/chainlib/data/config/config.ini
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:53:10.776353 chainlib-0.5.0/chainlib/data/env/
--rw-r--r--   0 lash      (1000) lash      (1000)     1198 2022-04-28 15:42:34.000000 chainlib-0.5.0/chainlib/data/env/env.ini
--rw-r--r--   0 lash      (1000) lash      (1000)      290 2023-02-10 19:31:04.000000 chainlib-0.5.0/chainlib/dialect.py
--rw-r--r--   0 lash      (1000) lash      (1000)      962 2021-12-21 15:02:23.000000 chainlib-0.5.0/chainlib/encode.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1243 2022-10-13 13:02:39.000000 chainlib-0.5.0/chainlib/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)      216 2021-10-10 10:19:14.000000 chainlib-0.5.0/chainlib/fee.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1373 2023-03-28 14:47:02.000000 chainlib-0.5.0/chainlib/hash.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1150 2021-10-10 10:19:14.000000 chainlib-0.5.0/chainlib/http.py
--rw-r--r--   0 lash      (1000) lash      (1000)     8279 2023-08-06 12:16:14.000000 chainlib-0.5.0/chainlib/interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4354 2021-10-10 10:19:14.000000 chainlib-0.5.0/chainlib/jsonrpc.py
--rw-r--r--   0 lash      (1000) lash      (1000)      300 2022-10-13 13:12:24.000000 chainlib-0.5.0/chainlib/nonce.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:53:10.776353 chainlib-0.5.0/chainlib/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     3367 2023-02-18 18:54:43.000000 chainlib-0.5.0/chainlib/runnable/gen.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2137 2023-08-06 12:29:38.000000 chainlib-0.5.0/chainlib/settings.py
--rw-r--r--   0 lash      (1000) lash      (1000)      305 2021-10-10 10:19:14.000000 chainlib-0.5.0/chainlib/sign.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1791 2023-06-03 06:47:10.000000 chainlib-0.5.0/chainlib/src.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1203 2021-10-10 10:19:14.000000 chainlib-0.5.0/chainlib/stat.py
--rw-r--r--   0 lash      (1000) lash      (1000)      184 2022-10-13 13:02:39.000000 chainlib-0.5.0/chainlib/status.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2188 2023-02-10 19:31:04.000000 chainlib-0.5.0/chainlib/tx.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:53:10.776353 chainlib-0.5.0/chainlib.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)    15563 2023-08-06 12:53:10.000000 chainlib-0.5.0/chainlib.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1008 2023-08-06 12:53:10.000000 chainlib-0.5.0/chainlib.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-06 12:53:10.000000 chainlib-0.5.0/chainlib.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       60 2023-08-06 12:53:10.000000 chainlib-0.5.0/chainlib.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       94 2023-08-06 12:53:10.000000 chainlib-0.5.0/chainlib.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-08-06 12:53:10.000000 chainlib-0.5.0/chainlib.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:53:10.773020 chainlib-0.5.0/man/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:53:10.779686 chainlib-0.5.0/man/build/
--rw-r--r--   0 lash      (1000) lash      (1000)     1056 2023-05-08 06:49:04.000000 chainlib-0.5.0/man/build/chainlib-gen.1
--rw-r--r--   0 lash      (1000) lash      (1000)       75 2023-06-10 08:10:01.000000 chainlib-0.5.0/requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:53:10.779686 chainlib-0.5.0/scripts/
--rwxr-xr-x   0 lash      (1000) lash      (1000)     7382 2022-11-12 13:17:39.000000 chainlib-0.5.0/scripts/chainlib-man.py
--rw-r--r--   0 lash      (1000) lash      (1000)      712 2023-08-06 12:53:10.779686 chainlib-0.5.0/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      875 2023-06-03 10:49:01.000000 chainlib-0.5.0/setup.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:53:10.779686 chainlib-0.5.0/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     2560 2021-12-21 15:02:23.000000 chainlib-0.5.0/tests/test_chain.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3753 2023-08-05 16:21:01.000000 chainlib-0.5.0/tests/test_cli.py
--rw-r--r--   0 lash      (1000) lash      (1000)      579 2021-10-10 10:19:14.000000 chainlib-0.5.0/tests/test_interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2227 2023-02-10 19:31:04.000000 chainlib-0.5.0/tests/test_src.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 18:09:40.130944 chainlib-0.5.1/
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:02:45.000000 chainlib-0.5.1/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      116 2023-06-03 10:49:41.000000 chainlib-0.5.1/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)    15563 2023-08-08 18:09:40.130944 chainlib-0.5.1/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)    14796 2023-06-03 10:49:46.000000 chainlib-0.5.1/README.md
+-rw-r--r--   0 lash      (1000) lash      (1000)      868 2022-11-14 07:03:32.000000 chainlib-0.5.1/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1621 2022-11-14 07:04:27.000000 chainlib-0.5.1/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 18:09:40.127611 chainlib-0.5.1/chainlib/
+-rw-r--r--   0 lash      (1000) lash      (1000)      699 2021-10-10 10:19:14.000000 chainlib-0.5.1/chainlib/auth.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1341 2023-02-10 19:31:04.000000 chainlib-0.5.1/chainlib/block.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5667 2021-12-21 15:02:23.000000 chainlib-0.5.1/chainlib/chain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 18:09:40.130944 chainlib-0.5.1/chainlib/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)      107 2022-11-04 07:26:52.000000 chainlib-0.5.1/chainlib/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6547 2023-08-08 17:57:13.000000 chainlib-0.5.1/chainlib/cli/arg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4911 2023-08-06 12:07:36.000000 chainlib-0.5.1/chainlib/cli/config.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1833 2023-02-14 06:42:51.000000 chainlib-0.5.1/chainlib/cli/gen.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      312 2023-02-14 06:42:51.000000 chainlib-0.5.1/chainlib/cli/log.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    13041 2023-08-08 08:33:43.000000 chainlib-0.5.1/chainlib/cli/man.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4567 2023-08-06 11:27:49.000000 chainlib-0.5.1/chainlib/cli/rpc.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4477 2022-11-03 17:13:57.000000 chainlib-0.5.1/chainlib/cli/wallet.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    13401 2023-08-06 11:50:17.000000 chainlib-0.5.1/chainlib/connection.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 18:09:40.124277 chainlib-0.5.1/chainlib/data/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 18:09:40.130944 chainlib-0.5.1/chainlib/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)      239 2023-08-06 12:04:30.000000 chainlib-0.5.1/chainlib/data/config/config.ini
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 18:09:40.130944 chainlib-0.5.1/chainlib/data/env/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1572 2023-08-08 17:59:41.000000 chainlib-0.5.1/chainlib/data/env/env.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)      290 2023-02-10 19:31:04.000000 chainlib-0.5.1/chainlib/dialect.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      962 2021-12-21 15:02:23.000000 chainlib-0.5.1/chainlib/encode.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1243 2022-10-13 13:02:39.000000 chainlib-0.5.1/chainlib/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      216 2021-10-10 10:19:14.000000 chainlib-0.5.1/chainlib/fee.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1373 2023-03-28 14:47:02.000000 chainlib-0.5.1/chainlib/hash.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1150 2021-10-10 10:19:14.000000 chainlib-0.5.1/chainlib/http.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     8279 2023-08-06 12:16:14.000000 chainlib-0.5.1/chainlib/interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4354 2021-10-10 10:19:14.000000 chainlib-0.5.1/chainlib/jsonrpc.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      300 2022-10-13 13:12:24.000000 chainlib-0.5.1/chainlib/nonce.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 18:09:40.130944 chainlib-0.5.1/chainlib/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3367 2023-02-18 18:54:43.000000 chainlib-0.5.1/chainlib/runnable/gen.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2137 2023-08-06 12:29:38.000000 chainlib-0.5.1/chainlib/settings.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      305 2021-10-10 10:19:14.000000 chainlib-0.5.1/chainlib/sign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1791 2023-06-03 06:47:10.000000 chainlib-0.5.1/chainlib/src.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1203 2021-10-10 10:19:14.000000 chainlib-0.5.1/chainlib/stat.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      184 2022-10-13 13:02:39.000000 chainlib-0.5.1/chainlib/status.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2188 2023-02-10 19:31:04.000000 chainlib-0.5.1/chainlib/tx.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 18:09:40.127611 chainlib-0.5.1/chainlib.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)    15563 2023-08-08 18:09:40.000000 chainlib-0.5.1/chainlib.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1008 2023-08-08 18:09:40.000000 chainlib-0.5.1/chainlib.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-08 18:09:40.000000 chainlib-0.5.1/chainlib.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       60 2023-08-08 18:09:40.000000 chainlib-0.5.1/chainlib.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       94 2023-08-08 18:09:40.000000 chainlib-0.5.1/chainlib.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-08-08 18:09:40.000000 chainlib-0.5.1/chainlib.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 18:09:40.124277 chainlib-0.5.1/man/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 18:09:40.130944 chainlib-0.5.1/man/build/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1569 2023-08-08 17:54:31.000000 chainlib-0.5.1/man/build/chainlib-gen.1
+-rw-r--r--   0 lash      (1000) lash      (1000)       75 2023-06-10 08:10:01.000000 chainlib-0.5.1/requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 18:09:40.130944 chainlib-0.5.1/scripts/
+-rwxr-xr-x   0 lash      (1000) lash      (1000)     7382 2022-11-12 13:17:39.000000 chainlib-0.5.1/scripts/chainlib-man.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      712 2023-08-08 18:09:40.130944 chainlib-0.5.1/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      875 2023-06-03 10:49:01.000000 chainlib-0.5.1/setup.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 18:09:40.130944 chainlib-0.5.1/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2560 2021-12-21 15:02:23.000000 chainlib-0.5.1/tests/test_chain.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3753 2023-08-05 16:21:01.000000 chainlib-0.5.1/tests/test_cli.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      579 2021-10-10 10:19:14.000000 chainlib-0.5.1/tests/test_interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2227 2023-02-10 19:31:04.000000 chainlib-0.5.1/tests/test_src.py
```

### Comparing `chainlib-0.5.0/LICENSE` & `chainlib-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/PKG-INFO` & `chainlib-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlib
-Version: 0.5.0
+Version: 0.5.1
 Summary: Generic blockchain access library and tooling
 Home-page: https://git.defalsify.org/chainlib
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chainlib-0.5.0/README.md` & `chainlib-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/WAIVER` & `chainlib-0.5.1/WAIVER`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/WAIVER.asc` & `chainlib-0.5.1/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/auth.py` & `chainlib-0.5.1/chainlib/auth.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/block.py` & `chainlib-0.5.1/chainlib/block.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/chain.py` & `chainlib-0.5.1/chainlib/chain.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/cli/arg.py` & `chainlib-0.5.1/chainlib/cli/arg.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
         self.add('u', 'unsafe', typ=bool, help='Do not verify address checksums')
         self.set_long('u', 'unsafe')
 
         self.add_long('seq', 'seq', typ=bool, help='Use sequential rpc ids')
 
         self.add('y', 'key_file', help='Keystore file to use for signing or address')
-        self.set_long('y', 'key_file')
+        self.set_long('y', 'key-file')
         self.add('z', 'key_file', typ=bool, help='No password to unlock keystore file')
         self.add_long('passphrase-file', 'key_file', help='Keystore file to use for signing or address')
 
         self.add('s', 'send', typ=bool, help='Send to network')
         self.set_long('s', 'send')
 
         self.add('f', 'sender', type=str, help='Unsigned sender')
```

### Comparing `chainlib-0.5.0/chainlib/cli/config.py` & `chainlib-0.5.1/chainlib/cli/config.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/cli/gen.py` & `chainlib-0.5.1/chainlib/cli/gen.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/cli/man.py` & `chainlib-0.5.1/chainlib/cli/man.py`

 * *Files 6% similar despite different names*

```diff
@@ -199,14 +199,20 @@
             self.envs['p'] = 'RPC_PROVIDER'
 
             o = DocEntry('--rpc-dialect')
             o.set_groff('RPC backend dialect. If specified it \\fImay\\fP help with encoding and decoding issues.')
             self.docs['rpcdialect'] = o
             self.envs['rpcdialect'] = 'RPC_DIALECT'
 
+            o = DocEntry('--rpc-batch-limit')
+            o.set_groff('Set number of RPC requests that can be set to the RPC provider as a batch request. This is made available through settings to any request builder implementing batch requests. A value of 1 means no batch will be used. A value of 0 indicates that the limit is not relevant. Any other positive value signals the maximum number of requests to be batched together.')
+            self.docs['rpcbatchlimit'] = o
+            self.envs['rpcbatchlimit'] = 'RPC_BATCH_LIMIT'
+
+
             if self.arg_flags & self.__argflag_list.NO_TARGET == 0:
                 o = DocEntry('--height')
                 o.set_groff('Block height at which to query state for. Does not apply to transactions.')
                 self.docs['height'] = o
 
             if self.arg_flags & self.__argflag_list.RPC_AUTH:
                 o = DocEntry('--rpc-auth')
@@ -338,14 +344,15 @@
 
     def process(self):
         ks = []
         if self.arg_flags & self.__argflag_list.PROVIDER:
             ks += [
                     'RPC_PROVIDER',
                     'RPC_DIALECT',
+                    'RPC_BATCH_LIMIT',
                     ]
             if self.arg_flags & self.__argflag_list.RPC_AUTH:
                 ks += [
                         'RPC_AUTH',
                         'RPC_CREDENTIALS',
                         ]
```

### Comparing `chainlib-0.5.0/chainlib/cli/rpc.py` & `chainlib-0.5.1/chainlib/cli/rpc.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/cli/wallet.py` & `chainlib-0.5.1/chainlib/cli/wallet.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/connection.py` & `chainlib-0.5.1/chainlib/connection.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/data/env/env.ini` & `chainlib-0.5.1/chainlib/data/env/env.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [rpc]
 provider = Fully-qualified URL to the RPC endpoint of the blockchain node.
 auth = Authentication method to use for the \fIRPC_PROVIDER\fP. Currently only \fIbasic\fP is supported.
 credentials = Authentication credentials to use for \fIRPC_AUTH\fP. For \fIbasic\fP authentication the value must be given as \fI<user>:<pass>\fP.
 dialect = Enables translations of EVM node specific formatting and response codes.
 scheme = (needs content)
 verify = (needs content)
+batch_limit = Set number of RPC requests that can be set to the RPC provider as a batch request. This is made available through settings to any request builder implementing batch requests. A value of 1 means no batch will be used. A value of 0 indicates that the limit is not relevant. Any other positive value signals the maximum number of requests to be batched together.
 
 [chain]
 spec = String specifying the type of chain connected to, in the format \fI<engine>:<fork>:<network_id>:<common_name>\fP. For EVM nodes the \fIengine\fP value will always be \fIevm\fP.
 
 [wallet]
 key_file = The wallet key file containing private key to use for transaction signing. Overridden by \fB-y\fP. 
 passphrase = Passphrase to unlock wallet. \fBWARNING:\fP it is \fBunsafe\fP to pass the passphrase as an environment variable. If the key unlocks something of value, the passphrase should rather be in a configuration file, preferably as an encrypted entry. Alternatively, a passphrase can be read from file using the \fB--passphrase-file\fP option. Files containing passphrases should only be accessible by the owner.
```

### Comparing `chainlib-0.5.0/chainlib/encode.py` & `chainlib-0.5.1/chainlib/encode.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/error.py` & `chainlib-0.5.1/chainlib/error.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/hash.py` & `chainlib-0.5.1/chainlib/hash.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/http.py` & `chainlib-0.5.1/chainlib/http.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/interface.py` & `chainlib-0.5.1/chainlib/interface.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/jsonrpc.py` & `chainlib-0.5.1/chainlib/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/runnable/gen.py` & `chainlib-0.5.1/chainlib/runnable/gen.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/settings.py` & `chainlib-0.5.1/chainlib/settings.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/src.py` & `chainlib-0.5.1/chainlib/src.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/stat.py` & `chainlib-0.5.1/chainlib/stat.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib/tx.py` & `chainlib-0.5.1/chainlib/tx.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/chainlib.egg-info/PKG-INFO` & `chainlib-0.5.1/chainlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlib
-Version: 0.5.0
+Version: 0.5.1
 Summary: Generic blockchain access library and tooling
 Home-page: https://git.defalsify.org/chainlib
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chainlib-0.5.0/chainlib.egg-info/SOURCES.txt` & `chainlib-0.5.1/chainlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/scripts/chainlib-man.py` & `chainlib-0.5.1/scripts/chainlib-man.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/setup.cfg` & `chainlib-0.5.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = chainlib
 license = AGPLv3+
 author_email = dev@holbrook.no
 description = Generic blockchain access library and tooling
-version = 0.5.0
+version = 0.5.1
 url = https://git.defalsify.org/chainlib
 author = Louis Holbrook
 keywords = 
 	dlt
 	blockchain
 	cryptocurrency
 classifiers =
```

### Comparing `chainlib-0.5.0/setup.py` & `chainlib-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/tests/test_chain.py` & `chainlib-0.5.1/tests/test_chain.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/tests/test_cli.py` & `chainlib-0.5.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/tests/test_interface.py` & `chainlib-0.5.1/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `chainlib-0.5.0/tests/test_src.py` & `chainlib-0.5.1/tests/test_src.py`

 * *Files identical despite different names*

