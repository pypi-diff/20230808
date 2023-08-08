# Comparing `tmp/okerrupdate-2.0.0.tar.gz` & `tmp/okerrupdate-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okerrupdate-2.0.0.tar", last modified: Tue Apr  4 14:52:03 2023, max compression
+gzip compressed data, was "okerrupdate-2.0.1.tar", last modified: Tue Aug  8 07:32:24 2023, max compression
```

## Comparing `okerrupdate-2.0.0.tar` & `okerrupdate-2.0.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.589342 okerrupdate-2.0.0/
--rw-r--r--   0 xenon     (1000) xenon     (1000)       77 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/MANIFEST.in
--rw-r--r--   0 xenon     (1000) xenon     (1000)     5353 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)     4021 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/README.md
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.581342 okerrupdate-2.0.0/okerrupdate/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    13621 2023-04-04 14:47:05.000000 okerrupdate-2.0.0/okerrupdate/__init__.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.581342 okerrupdate-2.0.0/okerrupdate/contrib/
--rw-r--r--   0 xenon     (1000) xenon     (1000)       86 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/contrib/okerrmod
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.581342 okerrupdate-2.0.0/okerrupdate/mods-available/
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.581342 okerrupdate-2.0.0/okerrupdate/mods-available/backups/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      972 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/backups/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)       73 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/backups/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2094 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/backups/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.581342 okerrupdate-2.0.0/okerrupdate/mods-available/client_ip/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      168 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/client_ip/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)       58 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/client_ip/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)      699 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/client_ip/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.581342 okerrupdate-2.0.0/okerrupdate/mods-available/df/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      431 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/df/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)       56 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/df/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1368 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/df/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.581342 okerrupdate-2.0.0/okerrupdate/mods-available/dirsize/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      517 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/dirsize/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)       56 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/dirsize/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2799 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/dirsize/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/okerrupdate/mods-available/empty/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      385 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/empty/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)      113 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/empty/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2135 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/empty/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/okerrupdate/mods-available/la/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      157 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/la/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)       53 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/la/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)      517 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/la/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/okerrupdate/mods-available/la3/
--rw-r--r--   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/la3/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)       92 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/la3/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)      517 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/la3/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/okerrupdate/mods-available/linecount/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      481 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/linecount/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)       79 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/linecount/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1624 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/linecount/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/okerrupdate/mods-available/maxfilesz/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      366 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/maxfilesz/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)       88 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/maxfilesz/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1375 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/maxfilesz/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/okerrupdate/mods-available/notempty/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      380 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/notempty/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)       89 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/notempty/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1838 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/notempty/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/okerrupdate/mods-available/ok/
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)       40 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/ok/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/okerrupdate/mods-available/opentcp/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      593 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/opentcp/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)       79 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/opentcp/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2147 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/opentcp/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/okerrupdate/mods-available/runline/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      959 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/runline/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)       77 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/runline/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1655 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/runline/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/okerrupdate/mods-available/runstatus/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      764 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/runstatus/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)       72 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/runstatus/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1189 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/runstatus/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/okerrupdate/mods-available/runtime/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      183 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/runtime/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)       99 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/runtime/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1124 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/runtime/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/okerrupdate/mods-available/sql/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      340 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/sql/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)       71 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/sql/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1396 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/sql/check
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)      193 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/sql/preenable
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/okerrupdate/mods-available/traffic/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      129 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/traffic/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)       65 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/traffic/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1491 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/traffic/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/okerrupdate/mods-available/uptime/
--rw-r--r--   0 xenon     (1000) xenon     (1000)      157 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/uptime/_config
--rw-r--r--   0 xenon     (1000) xenon     (1000)       53 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/uptime/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)      725 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/uptime/check
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/okerrupdate/mods-available/version/
--rw-r--r--   0 xenon     (1000) xenon     (1000)       74 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/version/_info
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)      169 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/mods-available/version/check
--rw-r--r--   0 xenon     (1000) xenon     (1000)      350 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/okerrupdate/utils.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)       22 2023-04-04 14:41:04.000000 okerrupdate-2.0.0/okerrupdate/version.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.581342 okerrupdate-2.0.0/okerrupdate.egg-info/
--rw-r--r--   0 xenon     (1000) xenon     (1000)     5353 2023-04-04 14:52:03.000000 okerrupdate-2.0.0/okerrupdate.egg-info/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)     2637 2023-04-04 14:52:03.000000 okerrupdate-2.0.0/okerrupdate.egg-info/SOURCES.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-04-04 14:52:03.000000 okerrupdate-2.0.0/okerrupdate.egg-info/dependency_links.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-04-04 14:52:03.000000 okerrupdate-2.0.0/okerrupdate.egg-info/not-zip-safe
--rw-r--r--   0 xenon     (1000) xenon     (1000)       30 2023-04-04 14:52:03.000000 okerrupdate-2.0.0/okerrupdate.egg-info/requires.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)       12 2023-04-04 14:52:03.000000 okerrupdate-2.0.0/okerrupdate.egg-info/top_level.txt
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-04-04 14:52:03.585342 okerrupdate-2.0.0/scripts/
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     4283 2023-04-04 14:49:29.000000 okerrupdate-2.0.0/scripts/okerrapi
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)    17308 2023-04-04 14:50:09.000000 okerrupdate-2.0.0/scripts/okerrmod
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2149 2023-04-04 14:47:59.000000 okerrupdate-2.0.0/scripts/okerrupdate
--rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-04-04 14:52:03.589342 okerrupdate-2.0.0/setup.cfg
--rw-r--r--   0 xenon     (1000) xenon     (1000)      762 2023-04-04 14:39:24.000000 okerrupdate-2.0.0/setup.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.444373 okerrupdate-2.0.1/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       77 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/MANIFEST.in
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     5510 2023-08-08 07:32:24.444373 okerrupdate-2.0.1/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     4130 2023-08-08 07:31:40.000000 okerrupdate-2.0.1/README.md
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.428372 okerrupdate-2.0.1/okerrupdate/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)    13621 2023-08-08 06:53:20.000000 okerrupdate-2.0.1/okerrupdate/__init__.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.432372 okerrupdate-2.0.1/okerrupdate/contrib/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       86 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/contrib/okerrmod
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.428372 okerrupdate-2.0.1/okerrupdate/mods-available/
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.432372 okerrupdate-2.0.1/okerrupdate/mods-available/backups/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      972 2021-02-03 17:04:10.000000 okerrupdate-2.0.1/okerrupdate/mods-available/backups/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       73 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/backups/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2094 2021-02-03 17:00:03.000000 okerrupdate-2.0.1/okerrupdate/mods-available/backups/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.432372 okerrupdate-2.0.1/okerrupdate/mods-available/client_ip/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      168 2021-06-22 17:40:08.000000 okerrupdate-2.0.1/okerrupdate/mods-available/client_ip/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       58 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/client_ip/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)      699 2021-06-22 17:30:46.000000 okerrupdate-2.0.1/okerrupdate/mods-available/client_ip/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.432372 okerrupdate-2.0.1/okerrupdate/mods-available/df/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      431 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/df/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       56 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/df/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1368 2023-01-17 19:46:36.000000 okerrupdate-2.0.1/okerrupdate/mods-available/df/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.432372 okerrupdate-2.0.1/okerrupdate/mods-available/dirsize/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      517 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/dirsize/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       56 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/dirsize/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2799 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/dirsize/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.436373 okerrupdate-2.0.1/okerrupdate/mods-available/empty/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      385 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/empty/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      113 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/empty/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2135 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/empty/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.436373 okerrupdate-2.0.1/okerrupdate/mods-available/la/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      157 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/la/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       53 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/la/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)      517 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/la/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.436373 okerrupdate-2.0.1/okerrupdate/mods-available/la3/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        0 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/la3/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       92 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/la3/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)      517 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/la3/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.436373 okerrupdate-2.0.1/okerrupdate/mods-available/linecount/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      481 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/linecount/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       79 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/linecount/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1624 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/linecount/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.436373 okerrupdate-2.0.1/okerrupdate/mods-available/maxfilesz/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      366 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/maxfilesz/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       88 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/maxfilesz/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1375 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/maxfilesz/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.436373 okerrupdate-2.0.1/okerrupdate/mods-available/notempty/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      380 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/notempty/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       89 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/notempty/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1838 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/notempty/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.436373 okerrupdate-2.0.1/okerrupdate/mods-available/ok/
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)       40 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/ok/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.436373 okerrupdate-2.0.1/okerrupdate/mods-available/opentcp/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      593 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/opentcp/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       79 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/opentcp/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2147 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/opentcp/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.440373 okerrupdate-2.0.1/okerrupdate/mods-available/runline/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      959 2023-01-17 15:50:05.000000 okerrupdate-2.0.1/okerrupdate/mods-available/runline/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       77 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/runline/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1655 2022-07-05 16:29:48.000000 okerrupdate-2.0.1/okerrupdate/mods-available/runline/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.440373 okerrupdate-2.0.1/okerrupdate/mods-available/runstatus/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      764 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/runstatus/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       72 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/runstatus/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1189 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/runstatus/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.440373 okerrupdate-2.0.1/okerrupdate/mods-available/runtime/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      183 2021-04-12 10:39:58.000000 okerrupdate-2.0.1/okerrupdate/mods-available/runtime/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       99 2021-04-12 11:00:06.000000 okerrupdate-2.0.1/okerrupdate/mods-available/runtime/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1124 2023-01-17 20:08:37.000000 okerrupdate-2.0.1/okerrupdate/mods-available/runtime/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.440373 okerrupdate-2.0.1/okerrupdate/mods-available/sql/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      340 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/sql/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       71 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/sql/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1396 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/sql/check
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)      193 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/sql/preenable
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.444373 okerrupdate-2.0.1/okerrupdate/mods-available/traffic/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      129 2023-01-17 20:17:34.000000 okerrupdate-2.0.1/okerrupdate/mods-available/traffic/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       65 2023-01-17 17:41:56.000000 okerrupdate-2.0.1/okerrupdate/mods-available/traffic/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     1491 2023-01-17 20:21:27.000000 okerrupdate-2.0.1/okerrupdate/mods-available/traffic/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.444373 okerrupdate-2.0.1/okerrupdate/mods-available/uptime/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      157 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/uptime/_config
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       53 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/uptime/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)      725 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/uptime/check
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.444373 okerrupdate-2.0.1/okerrupdate/mods-available/version/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       74 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/version/_info
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)      169 2020-11-29 10:21:52.000000 okerrupdate-2.0.1/okerrupdate/mods-available/version/check
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      350 2023-01-17 19:47:51.000000 okerrupdate-2.0.1/okerrupdate/utils.py
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       22 2023-08-08 07:31:56.000000 okerrupdate-2.0.1/okerrupdate/version.py
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.432372 okerrupdate-2.0.1/okerrupdate.egg-info/
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     5510 2023-08-08 07:32:24.000000 okerrupdate-2.0.1/okerrupdate.egg-info/PKG-INFO
+-rw-r--r--   0 xenon     (1000) xenon     (1000)     2637 2023-08-08 07:32:24.000000 okerrupdate-2.0.1/okerrupdate.egg-info/SOURCES.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-08-08 07:32:24.000000 okerrupdate-2.0.1/okerrupdate.egg-info/dependency_links.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2020-12-19 16:15:29.000000 okerrupdate-2.0.1/okerrupdate.egg-info/not-zip-safe
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       54 2023-08-08 07:32:24.000000 okerrupdate-2.0.1/okerrupdate.egg-info/requires.txt
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       12 2023-08-08 07:32:24.000000 okerrupdate-2.0.1/okerrupdate.egg-info/top_level.txt
+drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-08-08 07:32:24.444373 okerrupdate-2.0.1/scripts/
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     4283 2023-08-08 06:53:20.000000 okerrupdate-2.0.1/scripts/okerrapi
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)    17308 2023-08-08 06:53:20.000000 okerrupdate-2.0.1/scripts/okerrmod
+-rwxr-xr-x   0 xenon     (1000) xenon     (1000)     2149 2023-08-08 06:53:20.000000 okerrupdate-2.0.1/scripts/okerrupdate
+-rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-08-08 07:32:24.444373 okerrupdate-2.0.1/setup.cfg
+-rw-r--r--   0 xenon     (1000) xenon     (1000)      793 2023-08-08 07:30:36.000000 okerrupdate-2.0.1/setup.py
```

### Comparing `okerrupdate-2.0.0/PKG-INFO` & `okerrupdate-2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: okerrupdate
-Version: 2.0.0
+Version: 2.0.1
 Summary: client-side okerr module and utilities
 Home-page: https://github.com/yaroslaff/okerrupdate
 Author: Yaroslav Polyakov
 Author-email: yaroslaff@gmail.com
 License: MIT
 Description: # okerrupdate - client-side okerr module and utilities
         
         ## Installation 
         
         ```shell
+        # newer method with pipx
+        sudo pipx install okerrupdate
+        
+        # old method with pip3, if you cannot install pipx
         sudo pip3 install okerrupdate
+        
+        
         sudo okerrmod --init # enable few basic modules, create /etc/cron.d/ job, create okerrupdate config template
         sudo vim /etc/okerr/okerrupdate
         ```
         
         and modify okerrupdate file:
         ~~~
         # Stub for okerrmod
```

### Comparing `okerrupdate-2.0.0/README.md` & `okerrupdate-2.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # okerrupdate - client-side okerr module and utilities
 
 ## Installation 
 
 ```shell
+# newer method with pipx
+sudo pipx install okerrupdate
+
+# old method with pip3, if you cannot install pipx
 sudo pip3 install okerrupdate
+
+
 sudo okerrmod --init # enable few basic modules, create /etc/cron.d/ job, create okerrupdate config template
 sudo vim /etc/okerr/okerrupdate
 ```
 
 and modify okerrupdate file:
 ~~~
 # Stub for okerrmod
```

### Comparing `okerrupdate-2.0.0/okerrupdate/__init__.py` & `okerrupdate-2.0.1/okerrupdate/__init__.py`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/backups/_config` & `okerrupdate-2.0.1/okerrupdate/mods-available/backups/_config`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/backups/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/backups/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/client_ip/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/client_ip/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/df/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/df/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/dirsize/_config` & `okerrupdate-2.0.1/okerrupdate/mods-available/dirsize/_config`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/dirsize/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/dirsize/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/empty/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/empty/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/la/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/la/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/la3/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/la3/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/linecount/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/linecount/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/maxfilesz/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/maxfilesz/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/notempty/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/notempty/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/opentcp/_config` & `okerrupdate-2.0.1/okerrupdate/mods-available/opentcp/_config`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/opentcp/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/opentcp/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/runline/_config` & `okerrupdate-2.0.1/okerrupdate/mods-available/runline/_config`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/runline/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/runline/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/runstatus/_config` & `okerrupdate-2.0.1/okerrupdate/mods-available/runstatus/_config`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/runstatus/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/runstatus/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/runtime/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/runtime/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/sql/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/sql/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/traffic/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/traffic/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate/mods-available/uptime/check` & `okerrupdate-2.0.1/okerrupdate/mods-available/uptime/check`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/okerrupdate.egg-info/PKG-INFO` & `okerrupdate-2.0.1/okerrupdate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: okerrupdate
-Version: 2.0.0
+Version: 2.0.1
 Summary: client-side okerr module and utilities
 Home-page: https://github.com/yaroslaff/okerrupdate
 Author: Yaroslav Polyakov
 Author-email: yaroslaff@gmail.com
 License: MIT
 Description: # okerrupdate - client-side okerr module and utilities
         
         ## Installation 
         
         ```shell
+        # newer method with pipx
+        sudo pipx install okerrupdate
+        
+        # old method with pip3, if you cannot install pipx
         sudo pip3 install okerrupdate
+        
+        
         sudo okerrmod --init # enable few basic modules, create /etc/cron.d/ job, create okerrupdate config template
         sudo vim /etc/okerr/okerrupdate
         ```
         
         and modify okerrupdate file:
         ~~~
         # Stub for okerrmod
```

### Comparing `okerrupdate-2.0.0/okerrupdate.egg-info/SOURCES.txt` & `okerrupdate-2.0.1/okerrupdate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/scripts/okerrapi` & `okerrupdate-2.0.1/scripts/okerrapi`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/scripts/okerrmod` & `okerrupdate-2.0.1/scripts/okerrmod`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/scripts/okerrupdate` & `okerrupdate-2.0.1/scripts/okerrupdate`

 * *Files identical despite different names*

### Comparing `okerrupdate-2.0.0/setup.py` & `okerrupdate-2.0.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,11 +16,11 @@
       packages=['okerrupdate'],
       scripts=['scripts/okerrupdate', 'scripts/okerrmod', 'scripts/okerrapi'],
       include_package_data=True,
 
       long_description = read('README.md'),
       long_description_content_type='text/markdown',
 
-      install_requires=['requests', 'psutil', 'python-dotenv'],
+      install_requires=['requests == 2.25.1', 'urllib3 == 1.26.5', 'psutil', 'python-dotenv'],
       zip_safe=False
       )
```

