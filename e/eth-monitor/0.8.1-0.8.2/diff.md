# Comparing `tmp/eth-monitor-0.8.1.tar.gz` & `tmp/eth-monitor-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-monitor-0.8.1.tar", last modified: Sun Aug  6 18:33:29 2023, max compression
+gzip compressed data, was "eth-monitor-0.8.2.tar", last modified: Mon Aug  7 11:48:59 2023, max compression
```

## Comparing `eth-monitor-0.8.1.tar` & `eth-monitor-0.8.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/
--rw-r--r--   0 lash      (1000) lash      (1000)     1851 2023-08-06 18:31:42.000000 eth-monitor-0.8.1/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:56:11.000000 eth-monitor-0.8.1/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)      110 2023-05-13 20:45:22.000000 eth-monitor-0.8.1/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-08-06 18:33:29.411679 eth-monitor-0.8.1/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     9706 2023-05-13 20:42:58.000000 eth-monitor-0.8.1/README.md
--rw-r--r--   0 lash      (1000) lash      (1000)      871 2022-11-14 07:52:42.000000 eth-monitor-0.8.1/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:55:49.000000 eth-monitor-0.8.1/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.405012 eth-monitor-0.8.1/eth_monitor/
--rw-r--r--   0 lash      (1000) lash      (1000)      902 2022-11-11 05:56:27.000000 eth-monitor-0.8.1/eth_monitor/callback.py
--rw-r--r--   0 lash      (1000) lash      (1000)      645 2023-08-06 12:18:29.000000 eth-monitor-0.8.1/eth_monitor/chain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/eth_monitor/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)       65 2022-10-13 07:08:18.000000 eth-monitor-0.8.1/eth_monitor/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3361 2023-08-06 15:43:28.000000 eth-monitor-0.8.1/eth_monitor/cli/arg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1998 2023-08-06 15:47:56.000000 eth-monitor-0.8.1/eth_monitor/cli/config.py
--rw-r--r--   0 lash      (1000) lash      (1000)      518 2022-11-14 07:56:11.000000 eth-monitor-0.8.1/eth_monitor/cli/log.py
--rw-r--r--   0 lash      (1000) lash      (1000)      271 2022-10-13 07:08:18.000000 eth-monitor-0.8.1/eth_monitor/cli/rules.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1327 2022-04-20 19:19:25.000000 eth-monitor-0.8.1/eth_monitor/config.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.405012 eth-monitor-0.8.1/eth_monitor/data/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/eth_monitor/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)       40 2022-10-13 07:08:18.000000 eth-monitor-0.8.1/eth_monitor/data/config/cache.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-08-06 15:43:41.000000 eth-monitor-0.8.1/eth_monitor/data/config/filter.ini
--rw-r--r--   0 lash      (1000) lash      (1000)      257 2023-08-06 15:44:01.000000 eth-monitor-0.8.1/eth_monitor/data/config/monitor.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       22 2022-04-20 19:19:25.000000 eth-monitor-0.8.1/eth_monitor/data/config/renderer.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       87 2023-08-06 17:24:24.000000 eth-monitor-0.8.1/eth_monitor/driver.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/eth_monitor/filters/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-01-30 14:12:19.000000 eth-monitor-0.8.1/eth_monitor/filters/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      580 2023-08-06 16:02:41.000000 eth-monitor-0.8.1/eth_monitor/filters/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      263 2023-08-06 16:02:57.000000 eth-monitor-0.8.1/eth_monitor/filters/block.py
--rw-r--r--   0 lash      (1000) lash      (1000)      732 2023-08-06 16:03:10.000000 eth-monitor-0.8.1/eth_monitor/filters/cache.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2121 2023-08-06 16:02:35.000000 eth-monitor-0.8.1/eth_monitor/filters/out.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/eth_monitor/importers/
--rw-r--r--   0 lash      (1000) lash      (1000)     1521 2022-11-11 05:56:27.000000 eth-monitor-0.8.1/eth_monitor/importers/etherscan.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1450 2022-04-20 19:19:25.000000 eth-monitor-0.8.1/eth_monitor/index.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/eth_monitor/mock/
--rw-r--r--   0 lash      (1000) lash      (1000)      274 2022-01-30 14:12:19.000000 eth-monitor-0.8.1/eth_monitor/mock/filter_plain.py
--rw-r--r--   0 lash      (1000) lash      (1000)      417 2022-01-30 14:12:19.000000 eth-monitor-0.8.1/eth_monitor/mock/filter_ruled.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4240 2022-04-20 19:19:25.000000 eth-monitor-0.8.1/eth_monitor/rules.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/eth_monitor/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     5735 2022-04-20 19:19:25.000000 eth-monitor-0.8.1/eth_monitor/runnable/import.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3877 2022-04-20 19:19:25.000000 eth-monitor-0.8.1/eth_monitor/runnable/list.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3382 2023-08-06 16:04:50.000000 eth-monitor-0.8.1/eth_monitor/runnable/sync.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5125 2022-01-30 14:12:19.000000 eth-monitor-0.8.1/eth_monitor/runnable/sync_thread_range.py
--rw-r--r--   0 lash      (1000) lash      (1000)    13167 2023-08-06 16:04:32.000000 eth-monitor-0.8.1/eth_monitor/settings.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/eth_monitor.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-08-06 18:33:29.000000 eth-monitor-0.8.1/eth_monitor.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1259 2023-08-06 18:33:29.000000 eth-monitor-0.8.1/eth_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-06 18:33:29.000000 eth-monitor-0.8.1/eth_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      113 2023-08-06 18:33:29.000000 eth-monitor-0.8.1/eth_monitor.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      103 2023-08-06 18:33:29.000000 eth-monitor-0.8.1/eth_monitor.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       12 2023-08-06 18:33:29.000000 eth-monitor-0.8.1/eth_monitor.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.405012 eth-monitor-0.8.1/man/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/man/build/
--rw-r--r--   0 lash      (1000) lash      (1000)     5946 2023-05-13 20:02:53.000000 eth-monitor-0.8.1/man/build/eth-monitor-import.1
--rw-r--r--   0 lash      (1000) lash      (1000)     5557 2023-05-13 20:02:53.000000 eth-monitor-0.8.1/man/build/eth-monitor-list.1
--rw-r--r--   0 lash      (1000) lash      (1000)    10183 2023-05-13 20:02:53.000000 eth-monitor-0.8.1/man/build/eth-monitor-sync.1
--rw-r--r--   0 lash      (1000) lash      (1000)    10183 2023-05-13 20:02:53.000000 eth-monitor-0.8.1/man/build/eth-monitor.1
--rw-r--r--   0 lash      (1000) lash      (1000)      103 2023-08-06 18:24:22.000000 eth-monitor-0.8.1/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1002 2023-08-06 18:33:29.411679 eth-monitor-0.8.1/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      852 2023-05-13 20:44:09.000000 eth-monitor-0.8.1/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       76 2022-04-20 19:19:25.000000 eth-monitor-0.8.1/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     3524 2022-04-20 19:19:25.000000 eth-monitor-0.8.1/tests/test_basic.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1900 2023-08-07 11:42:05.000000 eth-monitor-0.8.2/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:56:11.000000 eth-monitor-0.8.2/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      110 2023-05-13 20:45:22.000000 eth-monitor-0.8.2/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     9706 2023-05-13 20:42:58.000000 eth-monitor-0.8.2/README.md
+-rw-r--r--   0 lash      (1000) lash      (1000)      871 2022-11-14 07:52:42.000000 eth-monitor-0.8.2/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:55:49.000000 eth-monitor-0.8.2/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.313188 eth-monitor-0.8.2/eth_monitor/
+-rw-r--r--   0 lash      (1000) lash      (1000)      902 2022-11-11 05:56:27.000000 eth-monitor-0.8.2/eth_monitor/callback.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      645 2023-08-06 12:18:29.000000 eth-monitor-0.8.2/eth_monitor/chain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.313188 eth-monitor-0.8.2/eth_monitor/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)       65 2022-10-13 07:08:18.000000 eth-monitor-0.8.2/eth_monitor/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3361 2023-08-07 11:45:49.000000 eth-monitor-0.8.2/eth_monitor/cli/arg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1998 2023-08-06 15:47:56.000000 eth-monitor-0.8.2/eth_monitor/cli/config.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      518 2022-11-14 07:56:11.000000 eth-monitor-0.8.2/eth_monitor/cli/log.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      271 2022-10-13 07:08:18.000000 eth-monitor-0.8.2/eth_monitor/cli/rules.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1327 2022-04-20 19:19:25.000000 eth-monitor-0.8.2/eth_monitor/config.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.309854 eth-monitor-0.8.2/eth_monitor/data/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.313188 eth-monitor-0.8.2/eth_monitor/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)       40 2022-10-13 07:08:18.000000 eth-monitor-0.8.2/eth_monitor/data/config/cache.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-08-06 15:43:41.000000 eth-monitor-0.8.2/eth_monitor/data/config/filter.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)      257 2023-08-06 15:44:01.000000 eth-monitor-0.8.2/eth_monitor/data/config/monitor.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       22 2022-04-20 19:19:25.000000 eth-monitor-0.8.2/eth_monitor/data/config/renderer.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       87 2023-08-06 17:24:24.000000 eth-monitor-0.8.2/eth_monitor/driver.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/eth_monitor/filters/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-01-30 14:12:19.000000 eth-monitor-0.8.2/eth_monitor/filters/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      580 2023-08-07 11:19:10.000000 eth-monitor-0.8.2/eth_monitor/filters/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      263 2023-08-06 16:02:57.000000 eth-monitor-0.8.2/eth_monitor/filters/block.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      732 2023-08-06 16:03:10.000000 eth-monitor-0.8.2/eth_monitor/filters/cache.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2121 2023-08-06 16:02:35.000000 eth-monitor-0.8.2/eth_monitor/filters/out.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/eth_monitor/importers/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1521 2022-11-11 05:56:27.000000 eth-monitor-0.8.2/eth_monitor/importers/etherscan.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1450 2022-04-20 19:19:25.000000 eth-monitor-0.8.2/eth_monitor/index.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/eth_monitor/mock/
+-rw-r--r--   0 lash      (1000) lash      (1000)      274 2022-01-30 14:12:19.000000 eth-monitor-0.8.2/eth_monitor/mock/filter_plain.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      417 2022-01-30 14:12:19.000000 eth-monitor-0.8.2/eth_monitor/mock/filter_ruled.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4240 2022-04-20 19:19:25.000000 eth-monitor-0.8.2/eth_monitor/rules.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/eth_monitor/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5735 2022-04-20 19:19:25.000000 eth-monitor-0.8.2/eth_monitor/runnable/import.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3877 2022-04-20 19:19:25.000000 eth-monitor-0.8.2/eth_monitor/runnable/list.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3381 2023-08-07 11:17:18.000000 eth-monitor-0.8.2/eth_monitor/runnable/sync.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5125 2022-01-30 14:12:19.000000 eth-monitor-0.8.2/eth_monitor/runnable/sync_thread_range.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    13210 2023-08-07 11:47:46.000000 eth-monitor-0.8.2/eth_monitor/settings.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.313188 eth-monitor-0.8.2/eth_monitor.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-08-07 11:48:59.000000 eth-monitor-0.8.2/eth_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1259 2023-08-07 11:48:59.000000 eth-monitor-0.8.2/eth_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-07 11:48:59.000000 eth-monitor-0.8.2/eth_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      113 2023-08-07 11:48:59.000000 eth-monitor-0.8.2/eth_monitor.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      103 2023-08-07 11:48:59.000000 eth-monitor-0.8.2/eth_monitor.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       12 2023-08-07 11:48:59.000000 eth-monitor-0.8.2/eth_monitor.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.313188 eth-monitor-0.8.2/man/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/man/build/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5946 2023-05-13 20:02:53.000000 eth-monitor-0.8.2/man/build/eth-monitor-import.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     5557 2023-05-13 20:02:53.000000 eth-monitor-0.8.2/man/build/eth-monitor-list.1
+-rw-r--r--   0 lash      (1000) lash      (1000)    10183 2023-05-13 20:02:53.000000 eth-monitor-0.8.2/man/build/eth-monitor-sync.1
+-rw-r--r--   0 lash      (1000) lash      (1000)    10183 2023-05-13 20:02:53.000000 eth-monitor-0.8.2/man/build/eth-monitor.1
+-rw-r--r--   0 lash      (1000) lash      (1000)      103 2023-08-07 11:41:42.000000 eth-monitor-0.8.2/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1002 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      852 2023-05-13 20:44:09.000000 eth-monitor-0.8.2/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       76 2022-04-20 19:19:25.000000 eth-monitor-0.8.2/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-07 11:48:59.316521 eth-monitor-0.8.2/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3524 2022-04-20 19:19:25.000000 eth-monitor-0.8.2/tests/test_basic.py
```

### Comparing `eth-monitor-0.8.1/CHANGELOG` & `eth-monitor-0.8.2/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+- 0.8.2
+	* Handle undefined content-key argument
 - 0.8.1
 	* Implement syncer context
 	* Add key-value parameter for cli, environment, config to pass to syncer context
 - 0.8.0
 	* Implement RPC batch limits for syncer
 - 0.7.6
 	* Make rpc dialect work with chain interface
```

### Comparing `eth-monitor-0.8.1/LICENSE` & `eth-monitor-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/PKG-INFO` & `eth-monitor-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-monitor
-Version: 0.8.1
+Version: 0.8.2
 Summary: Monitor and cache transactions using match filters
 Home-page: https://git.defalsify.org/eth-monitor
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-monitor-0.8.1/README.md` & `eth-monitor-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/WAIVER` & `eth-monitor-0.8.2/WAIVER`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/WAIVER.asc` & `eth-monitor-0.8.2/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/eth_monitor/callback.py` & `eth-monitor-0.8.2/eth_monitor/callback.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/eth_monitor/chain.py` & `eth-monitor-0.8.2/eth_monitor/chain.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/eth_monitor/cli/arg.py` & `eth-monitor-0.8.2/eth_monitor/cli/arg.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/eth_monitor/cli/config.py` & `eth-monitor-0.8.2/eth_monitor/cli/config.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/eth_monitor/cli/log.py` & `eth-monitor-0.8.2/eth_monitor/cli/log.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/eth_monitor/config.py` & `eth-monitor-0.8.2/eth_monitor/config.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/eth_monitor/filters/base.py` & `eth-monitor-0.8.2/eth_monitor/filters/base.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/eth_monitor/filters/cache.py` & `eth-monitor-0.8.2/eth_monitor/filters/cache.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/eth_monitor/filters/out.py` & `eth-monitor-0.8.2/eth_monitor/filters/out.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/eth_monitor/importers/etherscan.py` & `eth-monitor-0.8.2/eth_monitor/importers/etherscan.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/eth_monitor/index.py` & `eth-monitor-0.8.2/eth_monitor/index.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/eth_monitor/rules.py` & `eth-monitor-0.8.2/eth_monitor/rules.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/eth_monitor/runnable/import.py` & `eth-monitor-0.8.2/eth_monitor/runnable/import.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/eth_monitor/runnable/list.py` & `eth-monitor-0.8.2/eth_monitor/runnable/list.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/eth_monitor/runnable/sync.py` & `eth-monitor-0.8.2/eth_monitor/runnable/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,14 @@
 settings = process_settings_local(settings, config)
 logg.debug('loaded settings:\n{}'.format(settings))
 
 
 def main():
     logg.info('session is {}'.format(settings.get('SESSION_ID')))
 
-
     drv = ChainInterfaceDriver(
             settings.get('SYNC_STORE'),
             settings.get('SYNCER_INTERFACE'),
             offset=settings.get('SYNCER_OFFSET'),
             target=settings.get('SYNCER_LIMIT'),
             pre_callback=pre_callback,
             post_callback=post_callback,
```

### Comparing `eth-monitor-0.8.1/eth_monitor/runnable/sync_thread_range.py` & `eth-monitor-0.8.2/eth_monitor/runnable/sync_thread_range.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/eth_monitor/settings.py` & `eth-monitor-0.8.2/eth_monitor/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,17 +378,19 @@
     settings = process_cache_store(settings, config)
     settings = process_cache_rpc(settings, config)
     return settings
 
 
 def process_user_context(settings, config):
     ctx_usr = {}
-    for kv in config.get('ETHMONITOR_CONTEXT_KEY'):
-        (k, v) = kv.split('=', 1)
-        ctx_usr[k] = v
+    ks = config.get('ETHMONITOR_CONTEXT_KEY')
+    if ks != None:
+        for kv in ks:
+            (k, v) = kv.split('=', 1)
+            ctx_usr[k] = v
     ctx = {
         'driver': 'eth-monitor',
         'usr': ctx_usr,
             }
     settings.set('SYNCER_CONTEXT', ctx)
     return settings
```

### Comparing `eth-monitor-0.8.1/eth_monitor.egg-info/PKG-INFO` & `eth-monitor-0.8.2/eth_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-monitor
-Version: 0.8.1
+Version: 0.8.2
 Summary: Monitor and cache transactions using match filters
 Home-page: https://git.defalsify.org/eth-monitor
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-monitor-0.8.1/eth_monitor.egg-info/SOURCES.txt` & `eth-monitor-0.8.2/eth_monitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/man/build/eth-monitor-import.1` & `eth-monitor-0.8.2/man/build/eth-monitor-import.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/man/build/eth-monitor-list.1` & `eth-monitor-0.8.2/man/build/eth-monitor-list.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/man/build/eth-monitor-sync.1` & `eth-monitor-0.8.2/man/build/eth-monitor-sync.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/man/build/eth-monitor.1` & `eth-monitor-0.8.2/man/build/eth-monitor.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/setup.cfg` & `eth-monitor-0.8.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-monitor
-version = 0.8.1
+version = 0.8.2
 description = Monitor and cache transactions using match filters
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-monitor
 keywords = 
 	dlt
 	blockchain
```

### Comparing `eth-monitor-0.8.1/setup.py` & `eth-monitor-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.1/tests/test_basic.py` & `eth-monitor-0.8.2/tests/test_basic.py`

 * *Files identical despite different names*

