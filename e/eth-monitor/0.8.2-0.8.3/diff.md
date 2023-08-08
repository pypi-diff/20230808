# Comparing `tmp/eth-monitor-0.8.2.tar.gz` & `tmp/eth-monitor-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-monitor-0.8.2.tar", last modified: Mon Aug  7 11:48:59 2023, max compression
+gzip compressed data, was "eth-monitor-0.8.3.tar", last modified: Tue Aug  8 08:11:27 2023, max compression
```

## Comparing `eth-monitor-0.8.2.tar` & `eth-monitor-0.8.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/
--rw-r--r--   0 lash      (1000) lash      (1000)     1900 2023-08-07 11:42:05.000000 eth-monitor-0.8.2/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:56:11.000000 eth-monitor-0.8.2/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)      110 2023-05-13 20:45:22.000000 eth-monitor-0.8.2/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     9706 2023-05-13 20:42:58.000000 eth-monitor-0.8.2/README.md
--rw-r--r--   0 lash      (1000) lash      (1000)      871 2022-11-14 07:52:42.000000 eth-monitor-0.8.2/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:55:49.000000 eth-monitor-0.8.2/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.313188 eth-monitor-0.8.2/eth_monitor/
--rw-r--r--   0 lash      (1000) lash      (1000)      902 2022-11-11 05:56:27.000000 eth-monitor-0.8.2/eth_monitor/callback.py
--rw-r--r--   0 lash      (1000) lash      (1000)      645 2023-08-06 12:18:29.000000 eth-monitor-0.8.2/eth_monitor/chain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.313188 eth-monitor-0.8.2/eth_monitor/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)       65 2022-10-13 07:08:18.000000 eth-monitor-0.8.2/eth_monitor/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3361 2023-08-07 11:45:49.000000 eth-monitor-0.8.2/eth_monitor/cli/arg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1998 2023-08-06 15:47:56.000000 eth-monitor-0.8.2/eth_monitor/cli/config.py
--rw-r--r--   0 lash      (1000) lash      (1000)      518 2022-11-14 07:56:11.000000 eth-monitor-0.8.2/eth_monitor/cli/log.py
--rw-r--r--   0 lash      (1000) lash      (1000)      271 2022-10-13 07:08:18.000000 eth-monitor-0.8.2/eth_monitor/cli/rules.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1327 2022-04-20 19:19:25.000000 eth-monitor-0.8.2/eth_monitor/config.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.309854 eth-monitor-0.8.2/eth_monitor/data/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.313188 eth-monitor-0.8.2/eth_monitor/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)       40 2022-10-13 07:08:18.000000 eth-monitor-0.8.2/eth_monitor/data/config/cache.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-08-06 15:43:41.000000 eth-monitor-0.8.2/eth_monitor/data/config/filter.ini
--rw-r--r--   0 lash      (1000) lash      (1000)      257 2023-08-06 15:44:01.000000 eth-monitor-0.8.2/eth_monitor/data/config/monitor.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       22 2022-04-20 19:19:25.000000 eth-monitor-0.8.2/eth_monitor/data/config/renderer.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       87 2023-08-06 17:24:24.000000 eth-monitor-0.8.2/eth_monitor/driver.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/eth_monitor/filters/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-01-30 14:12:19.000000 eth-monitor-0.8.2/eth_monitor/filters/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      580 2023-08-07 11:19:10.000000 eth-monitor-0.8.2/eth_monitor/filters/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      263 2023-08-06 16:02:57.000000 eth-monitor-0.8.2/eth_monitor/filters/block.py
--rw-r--r--   0 lash      (1000) lash      (1000)      732 2023-08-06 16:03:10.000000 eth-monitor-0.8.2/eth_monitor/filters/cache.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2121 2023-08-06 16:02:35.000000 eth-monitor-0.8.2/eth_monitor/filters/out.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/eth_monitor/importers/
--rw-r--r--   0 lash      (1000) lash      (1000)     1521 2022-11-11 05:56:27.000000 eth-monitor-0.8.2/eth_monitor/importers/etherscan.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1450 2022-04-20 19:19:25.000000 eth-monitor-0.8.2/eth_monitor/index.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/eth_monitor/mock/
--rw-r--r--   0 lash      (1000) lash      (1000)      274 2022-01-30 14:12:19.000000 eth-monitor-0.8.2/eth_monitor/mock/filter_plain.py
--rw-r--r--   0 lash      (1000) lash      (1000)      417 2022-01-30 14:12:19.000000 eth-monitor-0.8.2/eth_monitor/mock/filter_ruled.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4240 2022-04-20 19:19:25.000000 eth-monitor-0.8.2/eth_monitor/rules.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/eth_monitor/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     5735 2022-04-20 19:19:25.000000 eth-monitor-0.8.2/eth_monitor/runnable/import.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3877 2022-04-20 19:19:25.000000 eth-monitor-0.8.2/eth_monitor/runnable/list.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3381 2023-08-07 11:17:18.000000 eth-monitor-0.8.2/eth_monitor/runnable/sync.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5125 2022-01-30 14:12:19.000000 eth-monitor-0.8.2/eth_monitor/runnable/sync_thread_range.py
--rw-r--r--   0 lash      (1000) lash      (1000)    13210 2023-08-07 11:47:46.000000 eth-monitor-0.8.2/eth_monitor/settings.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.313188 eth-monitor-0.8.2/eth_monitor.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-08-07 11:48:59.000000 eth-monitor-0.8.2/eth_monitor.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1259 2023-08-07 11:48:59.000000 eth-monitor-0.8.2/eth_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-07 11:48:59.000000 eth-monitor-0.8.2/eth_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      113 2023-08-07 11:48:59.000000 eth-monitor-0.8.2/eth_monitor.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      103 2023-08-07 11:48:59.000000 eth-monitor-0.8.2/eth_monitor.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       12 2023-08-07 11:48:59.000000 eth-monitor-0.8.2/eth_monitor.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.313188 eth-monitor-0.8.2/man/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/man/build/
--rw-r--r--   0 lash      (1000) lash      (1000)     5946 2023-05-13 20:02:53.000000 eth-monitor-0.8.2/man/build/eth-monitor-import.1
--rw-r--r--   0 lash      (1000) lash      (1000)     5557 2023-05-13 20:02:53.000000 eth-monitor-0.8.2/man/build/eth-monitor-list.1
--rw-r--r--   0 lash      (1000) lash      (1000)    10183 2023-05-13 20:02:53.000000 eth-monitor-0.8.2/man/build/eth-monitor-sync.1
--rw-r--r--   0 lash      (1000) lash      (1000)    10183 2023-05-13 20:02:53.000000 eth-monitor-0.8.2/man/build/eth-monitor.1
--rw-r--r--   0 lash      (1000) lash      (1000)      103 2023-08-07 11:41:42.000000 eth-monitor-0.8.2/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1002 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      852 2023-05-13 20:44:09.000000 eth-monitor-0.8.2/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       76 2022-04-20 19:19:25.000000 eth-monitor-0.8.2/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     3524 2022-04-20 19:19:25.000000 eth-monitor-0.8.2/tests/test_basic.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 08:11:26.997528 eth-monitor-0.8.3/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1928 2023-08-08 08:10:02.000000 eth-monitor-0.8.3/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:56:11.000000 eth-monitor-0.8.3/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      110 2023-05-13 20:45:22.000000 eth-monitor-0.8.3/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-08-08 08:11:26.997528 eth-monitor-0.8.3/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     9706 2023-05-13 20:42:58.000000 eth-monitor-0.8.3/README.md
+-rw-r--r--   0 lash      (1000) lash      (1000)      871 2022-11-14 07:52:42.000000 eth-monitor-0.8.3/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:55:49.000000 eth-monitor-0.8.3/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 08:11:26.994195 eth-monitor-0.8.3/eth_monitor/
+-rw-r--r--   0 lash      (1000) lash      (1000)      902 2022-11-11 05:56:27.000000 eth-monitor-0.8.3/eth_monitor/callback.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      645 2023-08-06 12:18:29.000000 eth-monitor-0.8.3/eth_monitor/chain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 08:11:26.994195 eth-monitor-0.8.3/eth_monitor/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)       65 2022-10-13 07:08:18.000000 eth-monitor-0.8.3/eth_monitor/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3361 2023-08-07 11:45:49.000000 eth-monitor-0.8.3/eth_monitor/cli/arg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1998 2023-08-06 15:47:56.000000 eth-monitor-0.8.3/eth_monitor/cli/config.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      518 2022-11-14 07:56:11.000000 eth-monitor-0.8.3/eth_monitor/cli/log.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      269 2023-08-08 07:54:29.000000 eth-monitor-0.8.3/eth_monitor/cli/rules.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1327 2022-04-20 19:19:25.000000 eth-monitor-0.8.3/eth_monitor/config.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 08:11:26.990861 eth-monitor-0.8.3/eth_monitor/data/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 08:11:26.994195 eth-monitor-0.8.3/eth_monitor/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)       40 2022-10-13 07:08:18.000000 eth-monitor-0.8.3/eth_monitor/data/config/cache.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-08-06 15:43:41.000000 eth-monitor-0.8.3/eth_monitor/data/config/filter.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)      257 2023-08-06 15:44:01.000000 eth-monitor-0.8.3/eth_monitor/data/config/monitor.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       22 2022-04-20 19:19:25.000000 eth-monitor-0.8.3/eth_monitor/data/config/renderer.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       87 2023-08-06 17:24:24.000000 eth-monitor-0.8.3/eth_monitor/driver.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 08:11:26.994195 eth-monitor-0.8.3/eth_monitor/filters/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-01-30 14:12:19.000000 eth-monitor-0.8.3/eth_monitor/filters/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      580 2023-08-07 11:19:10.000000 eth-monitor-0.8.3/eth_monitor/filters/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      263 2023-08-06 16:02:57.000000 eth-monitor-0.8.3/eth_monitor/filters/block.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      732 2023-08-06 16:03:10.000000 eth-monitor-0.8.3/eth_monitor/filters/cache.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2121 2023-08-06 16:02:35.000000 eth-monitor-0.8.3/eth_monitor/filters/out.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 08:11:26.994195 eth-monitor-0.8.3/eth_monitor/importers/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1521 2022-11-11 05:56:27.000000 eth-monitor-0.8.3/eth_monitor/importers/etherscan.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1450 2022-04-20 19:19:25.000000 eth-monitor-0.8.3/eth_monitor/index.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 08:11:26.994195 eth-monitor-0.8.3/eth_monitor/mock/
+-rw-r--r--   0 lash      (1000) lash      (1000)      274 2022-01-30 14:12:19.000000 eth-monitor-0.8.3/eth_monitor/mock/filter_plain.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      417 2022-01-30 14:12:19.000000 eth-monitor-0.8.3/eth_monitor/mock/filter_ruled.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4240 2022-04-20 19:19:25.000000 eth-monitor-0.8.3/eth_monitor/rules.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 08:11:26.994195 eth-monitor-0.8.3/eth_monitor/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5735 2022-04-20 19:19:25.000000 eth-monitor-0.8.3/eth_monitor/runnable/import.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3877 2022-04-20 19:19:25.000000 eth-monitor-0.8.3/eth_monitor/runnable/list.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3381 2023-08-07 11:17:18.000000 eth-monitor-0.8.3/eth_monitor/runnable/sync.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5125 2022-01-30 14:12:19.000000 eth-monitor-0.8.3/eth_monitor/runnable/sync_thread_range.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    13210 2023-08-07 11:47:46.000000 eth-monitor-0.8.3/eth_monitor/settings.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 08:11:26.994195 eth-monitor-0.8.3/eth_monitor.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-08-08 08:11:26.000000 eth-monitor-0.8.3/eth_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1259 2023-08-08 08:11:26.000000 eth-monitor-0.8.3/eth_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-08 08:11:26.000000 eth-monitor-0.8.3/eth_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      113 2023-08-08 08:11:26.000000 eth-monitor-0.8.3/eth_monitor.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      103 2023-08-08 08:11:26.000000 eth-monitor-0.8.3/eth_monitor.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       12 2023-08-08 08:11:26.000000 eth-monitor-0.8.3/eth_monitor.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 08:11:26.990861 eth-monitor-0.8.3/man/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 08:11:26.997528 eth-monitor-0.8.3/man/build/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5946 2023-08-08 08:09:52.000000 eth-monitor-0.8.3/man/build/eth-monitor-import.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     5557 2023-08-08 08:09:52.000000 eth-monitor-0.8.3/man/build/eth-monitor-list.1
+-rw-r--r--   0 lash      (1000) lash      (1000)    10507 2023-08-08 08:09:52.000000 eth-monitor-0.8.3/man/build/eth-monitor-sync.1
+-rw-r--r--   0 lash      (1000) lash      (1000)    10507 2023-08-08 08:09:52.000000 eth-monitor-0.8.3/man/build/eth-monitor.1
+-rw-r--r--   0 lash      (1000) lash      (1000)      103 2023-08-07 11:41:42.000000 eth-monitor-0.8.3/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1002 2023-08-08 08:11:26.997528 eth-monitor-0.8.3/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      852 2023-05-13 20:44:09.000000 eth-monitor-0.8.3/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       76 2022-04-20 19:19:25.000000 eth-monitor-0.8.3/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-08 08:11:26.997528 eth-monitor-0.8.3/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3524 2022-04-20 19:19:25.000000 eth-monitor-0.8.3/tests/test_basic.py
```

### Comparing `eth-monitor-0.8.2/CHANGELOG` & `eth-monitor-0.8.3/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+- 0.8.3
+	* Update man pages
 - 0.8.2
 	* Handle undefined content-key argument
 - 0.8.1
 	* Implement syncer context
 	* Add key-value parameter for cli, environment, config to pass to syncer context
 - 0.8.0
 	* Implement RPC batch limits for syncer
```

### Comparing `eth-monitor-0.8.2/LICENSE` & `eth-monitor-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/PKG-INFO` & `eth-monitor-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-monitor
-Version: 0.8.2
+Version: 0.8.3
 Summary: Monitor and cache transactions using match filters
 Home-page: https://git.defalsify.org/eth-monitor
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-monitor-0.8.2/README.md` & `eth-monitor-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/WAIVER` & `eth-monitor-0.8.3/WAIVER`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/WAIVER.asc` & `eth-monitor-0.8.3/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/callback.py` & `eth-monitor-0.8.3/eth_monitor/callback.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/chain.py` & `eth-monitor-0.8.3/eth_monitor/chain.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/cli/arg.py` & `eth-monitor-0.8.3/eth_monitor/cli/arg.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/cli/config.py` & `eth-monitor-0.8.3/eth_monitor/cli/config.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/cli/log.py` & `eth-monitor-0.8.3/eth_monitor/cli/log.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/config.py` & `eth-monitor-0.8.3/eth_monitor/config.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/filters/base.py` & `eth-monitor-0.8.3/eth_monitor/filters/base.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/filters/cache.py` & `eth-monitor-0.8.3/eth_monitor/filters/cache.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/filters/out.py` & `eth-monitor-0.8.3/eth_monitor/filters/out.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/importers/etherscan.py` & `eth-monitor-0.8.3/eth_monitor/importers/etherscan.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/index.py` & `eth-monitor-0.8.3/eth_monitor/index.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/rules.py` & `eth-monitor-0.8.3/eth_monitor/rules.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/runnable/import.py` & `eth-monitor-0.8.3/eth_monitor/runnable/import.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/runnable/list.py` & `eth-monitor-0.8.3/eth_monitor/runnable/list.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/runnable/sync.py` & `eth-monitor-0.8.3/eth_monitor/runnable/sync.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/runnable/sync_thread_range.py` & `eth-monitor-0.8.3/eth_monitor/runnable/sync_thread_range.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor/settings.py` & `eth-monitor-0.8.3/eth_monitor/settings.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/eth_monitor.egg-info/PKG-INFO` & `eth-monitor-0.8.3/eth_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-monitor
-Version: 0.8.2
+Version: 0.8.3
 Summary: Monitor and cache transactions using match filters
 Home-page: https://git.defalsify.org/eth-monitor
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-monitor-0.8.2/eth_monitor.egg-info/SOURCES.txt` & `eth-monitor-0.8.3/eth_monitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/man/build/eth-monitor-import.1` & `eth-monitor-0.8.3/man/build/eth-monitor-import.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/man/build/eth-monitor-list.1` & `eth-monitor-0.8.3/man/build/eth-monitor-list.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/man/build/eth-monitor-sync.1` & `eth-monitor-0.8.3/man/build/eth-monitor-sync.1`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,19 @@
 Add an address of interest to match any role. Complements \fB--address-file\fP.
 
 .TP
 \fB-c \fI\fIconfig_dir\fP\fP, \fB--config \fI\fIconfig_dir\fP\fP
 Load configuration files from given directory. All files with an .ini extension will be loaded, of which all must contain valid ini file data.
 
 .TP
+\fB--context-key \fI\fIkey=value
+\fP\fP
+Add a key-value pair that gets passed to the syncer context. May be specified several times.
+
+.TP
 \fB--dumpconfig \fI\fIformat\fP\fP
 Output configuration settings rendered from environment and inputs. Valid arguments are \fIini\fP for ini file output, and \fIenv\fP for environment variable output. See \fBCONFIGURATION\fP.
 
 .TP
 \fB--env-prefix\fP
 Environment prefix for variables to overwrite configuration. Example: If \fB--env-prefix\fP is set to \fBFOO\fP then configuration variable \fBBAR_BAZ\fP would be set by environment variable \fBFOO_BAZ_BAR\fP. Also see \fBENVIRONMENT\fP.
 
@@ -207,22 +212,27 @@
 Filters for rendering may be specified by specifying python modules to the \fB--renderer\fP option. This option may be specified multiple times.
 .P
 Rendering filters will be executed in order, and the first filter to return \fIFalse\fP
 
 
 .SH DEFINING FILTERS
 
+Filters will strictly be executed in the order which they are defined on the command line.
+
 A python module used for filter must fulfill two conditions:
 
 .IP
 1. It must provide a class named \fIFilter\fP in the package base namespace.
 .IP
-2. The \fIFilter\fP class must include a method named \fIfilter\fP with the signature \fIdef filter(self, conn, block, tx, db_session=None)\fP. 
+2. The \fIFilter\fP class must extend the \fIchainsyncer.filter.SyncFilter\fP interface, and at least override the \fIfilter\fP method.
 
-Filters will strictly be executed in the order which they are defined on the command line.
+
+.SS SYNCER AND FILTER CONTEXT
+
+Key-value pairs specified with `--context-key` will be passed to the filter's \fIprepare\fP method, aswell as the \fIctx\fP parameter of the \fIfilter\fP method.
 
 
 .SH FURTHER READING
 
 Refer to the \fBchainsyncer\fP chapter n \fIinfo chaintool\fP for in-depth information on the subjects of syncing and filtering.
 .SH ENVIRONMENT
```

### Comparing `eth-monitor-0.8.2/man/build/eth-monitor.1` & `eth-monitor-0.8.3/man/build/eth-monitor.1`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,19 @@
 Add an address of interest to match any role. Complements \fB--address-file\fP.
 
 .TP
 \fB-c \fI\fIconfig_dir\fP\fP, \fB--config \fI\fIconfig_dir\fP\fP
 Load configuration files from given directory. All files with an .ini extension will be loaded, of which all must contain valid ini file data.
 
 .TP
+\fB--context-key \fI\fIkey=value
+\fP\fP
+Add a key-value pair that gets passed to the syncer context. May be specified several times.
+
+.TP
 \fB--dumpconfig \fI\fIformat\fP\fP
 Output configuration settings rendered from environment and inputs. Valid arguments are \fIini\fP for ini file output, and \fIenv\fP for environment variable output. See \fBCONFIGURATION\fP.
 
 .TP
 \fB--env-prefix\fP
 Environment prefix for variables to overwrite configuration. Example: If \fB--env-prefix\fP is set to \fBFOO\fP then configuration variable \fBBAR_BAZ\fP would be set by environment variable \fBFOO_BAZ_BAR\fP. Also see \fBENVIRONMENT\fP.
 
@@ -207,22 +212,27 @@
 Filters for rendering may be specified by specifying python modules to the \fB--renderer\fP option. This option may be specified multiple times.
 .P
 Rendering filters will be executed in order, and the first filter to return \fIFalse\fP
 
 
 .SH DEFINING FILTERS
 
+Filters will strictly be executed in the order which they are defined on the command line.
+
 A python module used for filter must fulfill two conditions:
 
 .IP
 1. It must provide a class named \fIFilter\fP in the package base namespace.
 .IP
-2. The \fIFilter\fP class must include a method named \fIfilter\fP with the signature \fIdef filter(self, conn, block, tx, db_session=None)\fP. 
+2. The \fIFilter\fP class must extend the \fIchainsyncer.filter.SyncFilter\fP interface, and at least override the \fIfilter\fP method.
 
-Filters will strictly be executed in the order which they are defined on the command line.
+
+.SS SYNCER AND FILTER CONTEXT
+
+Key-value pairs specified with `--context-key` will be passed to the filter's \fIprepare\fP method, aswell as the \fIctx\fP parameter of the \fIfilter\fP method.
 
 
 .SH FURTHER READING
 
 Refer to the \fBchainsyncer\fP chapter n \fIinfo chaintool\fP for in-depth information on the subjects of syncing and filtering.
 .SH ENVIRONMENT
```

### Comparing `eth-monitor-0.8.2/setup.cfg` & `eth-monitor-0.8.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-monitor
-version = 0.8.2
+version = 0.8.3
 description = Monitor and cache transactions using match filters
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-monitor
 keywords = 
 	dlt
 	blockchain
```

### Comparing `eth-monitor-0.8.2/setup.py` & `eth-monitor-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.2/tests/test_basic.py` & `eth-monitor-0.8.3/tests/test_basic.py`

 * *Files identical despite different names*

