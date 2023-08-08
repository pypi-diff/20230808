# Comparing `tmp/meerschaum-1.7.0.dev2.tar.gz` & `tmp/meerschaum-1.7.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meerschaum-1.7.0.dev2.tar", last modified: Fri Aug  4 20:32:53 2023, max compression
+gzip compressed data, was "meerschaum-1.7.0.dev3.tar", last modified: Tue Aug  8 05:19:17 2023, max compression
```

## Comparing `meerschaum-1.7.0.dev2.tar` & `meerschaum-1.7.0.dev3.tar`

### file list

```diff
@@ -1,280 +1,282 @@
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.612284 meerschaum-1.7.0.dev2/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-1.7.0.dev2/LICENSE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-1.7.0.dev2/NOTICE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10803 2023-08-04 20:32:53.612284 meerschaum-1.7.0.dev2/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9248 2022-07-13 02:48:08.000000 meerschaum-1.7.0.dev2/README.md
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.599284 meerschaum-1.7.0.dev2/meerschaum/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1236 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2774 2022-10-22 06:28:47.000000 meerschaum-1.7.0.dev2/meerschaum/__main__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.600284 meerschaum-1.7.0.dev2/meerschaum/_internal/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.600284 meerschaum-1.7.0.dev2/meerschaum/_internal/arguments/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/arguments/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9741 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/arguments/_parse_arguments.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12586 2023-08-04 19:18:55.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/arguments/_parser.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.600284 meerschaum-1.7.0.dev2/meerschaum/_internal/docs/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/docs/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7719 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/docs/index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4625 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/entry.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.600284 meerschaum-1.7.0.dev2/meerschaum/_internal/gui/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1332 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/gui/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.601284 meerschaum-1.7.0.dev2/meerschaum/_internal/gui/app/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/gui/app/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/gui/app/_windows.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1016 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/gui/app/actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1678 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/gui/app/pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.601284 meerschaum-1.7.0.dev2/meerschaum/_internal/shell/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31489 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/shell/Shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2981 2022-10-22 06:28:01.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/shell/ShellCompleter.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/shell/ValidAutoSuggest.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/shell/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.601284 meerschaum-1.7.0.dev2/meerschaum/_internal/shell/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/shell/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.601284 meerschaum-1.7.0.dev2/meerschaum/_internal/term/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2021-12-09 07:32:03.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/term/TermPageHandler.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1960 2023-08-04 20:09:45.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/term/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      716 2023-08-04 03:39:01.000000 meerschaum-1.7.0.dev2/meerschaum/_internal/term/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.602284 meerschaum-1.7.0.dev2/meerschaum/actions/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8023 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev2/meerschaum/actions/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12109 2023-08-04 19:18:39.000000 meerschaum-1.7.0.dev2/meerschaum/actions/api.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14529 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/actions/bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4857 2022-08-23 06:14:42.000000 meerschaum-1.7.0.dev2/meerschaum/actions/clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6259 2023-06-28 23:16:36.000000 meerschaum-1.7.0.dev2/meerschaum/actions/copy.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15245 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev2/meerschaum/actions/delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2701 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev2/meerschaum/actions/drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9492 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/actions/edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7380 2022-10-18 06:13:35.000000 meerschaum-1.7.0.dev2/meerschaum/actions/install.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev2/meerschaum/actions/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-1.7.0.dev2/meerschaum/actions/os.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev2/meerschaum/actions/python.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11219 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/actions/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      605 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev2/meerschaum/actions/reload.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3211 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev2/meerschaum/actions/setup.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-1.7.0.dev2/meerschaum/actions/sh.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23468 2023-01-11 06:27:06.000000 meerschaum-1.7.0.dev2/meerschaum/actions/show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4224 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev2/meerschaum/actions/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5807 2023-06-28 23:16:36.000000 meerschaum-1.7.0.dev2/meerschaum/actions/stack.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18415 2023-08-04 20:28:19.000000 meerschaum-1.7.0.dev2/meerschaum/actions/start.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3948 2023-01-16 21:21:28.000000 meerschaum-1.7.0.dev2/meerschaum/actions/stop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15339 2022-12-15 02:09:06.000000 meerschaum-1.7.0.dev2/meerschaum/actions/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6073 2022-08-19 04:59:44.000000 meerschaum-1.7.0.dev2/meerschaum/actions/uninstall.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6307 2022-08-19 04:59:44.000000 meerschaum-1.7.0.dev2/meerschaum/actions/upgrade.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3348 2022-10-26 04:20:20.000000 meerschaum-1.7.0.dev2/meerschaum/actions/verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.603284 meerschaum-1.7.0.dev2/meerschaum/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7704 2023-08-04 03:03:40.000000 meerschaum-1.7.0.dev2/meerschaum/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev2/meerschaum/api/_chain.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1755 2023-08-04 04:30:57.000000 meerschaum-1.7.0.dev2/meerschaum/api/_events.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      961 2023-07-13 02:20:19.000000 meerschaum-1.7.0.dev2/meerschaum/api/_oauth2.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1226 2022-11-05 03:38:45.000000 meerschaum-1.7.0.dev2/meerschaum/api/_websockets.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.603284 meerschaum-1.7.0.dev2/meerschaum/api/dash/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2238 2023-01-09 08:57:26.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9600 2022-10-31 13:18:31.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/actions.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.604284 meerschaum-1.7.0.dev2/meerschaum/api/dash/assets/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/assets/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/assets/ansi_up.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/assets/banner_1920x320.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/assets/favicon.ico
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/assets/logo_48x48.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/assets/logo_500x500.png
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.604284 meerschaum-1.7.0.dev2/meerschaum/api/dash/callbacks/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      283 2023-07-21 01:07:26.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/callbacks/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    25324 2023-08-04 19:38:53.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/callbacks/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2529 2023-01-09 09:04:18.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/callbacks/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/callbacks/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3446 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/callbacks/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6289 2023-08-04 20:25:46.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/components.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2046 2023-08-04 04:44:53.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/graphs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3544 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13682 2022-10-31 13:18:31.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/keys.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.604284 meerschaum-1.7.0.dev2/meerschaum/api/dash/pages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-07-21 01:07:38.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/pages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3838 2023-08-04 19:40:54.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/pages/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      598 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/pages/error.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4601 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/pages/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1382 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/pages/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2398 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/pages/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15039 2022-10-31 14:15:34.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3054 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      895 2023-08-04 02:41:30.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/websockets.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2723 2023-08-04 20:28:01.000000 meerschaum-1.7.0.dev2/meerschaum/api/dash/webterm.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.605284 meerschaum-1.7.0.dev2/meerschaum/api/models/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/models/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/models/_interfaces.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/models/_locations.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/models/_metrics.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-1.7.0.dev2/meerschaum/api/models/_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.605284 meerschaum-1.7.0.dev2/meerschaum/api/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.605284 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.605284 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/css/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/css/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/css/bootstrap.min.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1674 2023-08-04 03:00:27.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/css/dash.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/css/dbc_dark.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/css/styles.css
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.605284 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/ico/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/ico/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/ico/logo.ico
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.605284 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/js/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/js/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/js/action_button.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/js/main.js
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.605284 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/png/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/static/png/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.606284 meerschaum-1.7.0.dev2/meerschaum/api/resources/templates/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/templates/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/templates/index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/templates/old_index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/templates/secret.html
--rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     2082 2021-12-09 07:32:03.000000 meerschaum-1.7.0.dev2/meerschaum/api/resources/templates/termpage.html
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.606284 meerschaum-1.7.0.dev2/meerschaum/api/routes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      734 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/api/routes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev2/meerschaum/api/routes/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1803 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev2/meerschaum/api/routes/_connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev2/meerschaum/api/routes/_index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1882 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev2/meerschaum/api/routes/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1714 2023-07-14 22:01:00.000000 meerschaum-1.7.0.dev2/meerschaum/api/routes/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21169 2023-01-21 08:00:50.000000 meerschaum-1.7.0.dev2/meerschaum/api/routes/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6152 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev2/meerschaum/api/routes/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7204 2023-07-14 20:54:29.000000 meerschaum-1.7.0.dev2/meerschaum/api/routes/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev2/meerschaum/api/routes/_version.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.606284 meerschaum-1.7.0.dev2/meerschaum/api/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      615 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev2/meerschaum/api/tables/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.607284 meerschaum-1.7.0.dev2/meerschaum/config/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11629 2023-01-11 04:28:52.000000 meerschaum-1.7.0.dev2/meerschaum/config/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5135 2023-05-05 04:35:54.000000 meerschaum-1.7.0.dev2/meerschaum/config/_default.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8807 2022-07-13 02:48:16.000000 meerschaum-1.7.0.dev2/meerschaum/config/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4507 2022-10-22 07:29:33.000000 meerschaum-1.7.0.dev2/meerschaum/config/_environment.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5556 2022-05-02 19:58:56.000000 meerschaum-1.7.0.dev2/meerschaum/config/_formatting.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      647 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev2/meerschaum/config/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1508 2023-01-11 05:57:34.000000 meerschaum-1.7.0.dev2/meerschaum/config/_patch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6648 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev2/meerschaum/config/_paths.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev2/meerschaum/config/_preprocess.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14567 2022-10-14 04:34:51.000000 meerschaum-1.7.0.dev2/meerschaum/config/_read_config.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3589 2021-11-21 05:32:46.000000 meerschaum-1.7.0.dev2/meerschaum/config/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4968 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev2/meerschaum/config/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       76 2023-08-04 20:25:58.000000 meerschaum-1.7.0.dev2/meerschaum/config/_version.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.607284 meerschaum-1.7.0.dev2/meerschaum/config/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/config/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.607284 meerschaum-1.7.0.dev2/meerschaum/config/stack/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8616 2023-06-28 23:16:36.000000 meerschaum-1.7.0.dev2/meerschaum/config/stack/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.607284 meerschaum-1.7.0.dev2/meerschaum/config/stack/grafana/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-1.7.0.dev2/meerschaum/config/stack/grafana/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.607284 meerschaum-1.7.0.dev2/meerschaum/config/stack/mosquitto/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/config/stack/mosquitto/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.607284 meerschaum-1.7.0.dev2/meerschaum/config/stack/mosquitto/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/config/stack/mosquitto/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.607284 meerschaum-1.7.0.dev2/meerschaum/config/stack/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/config/stack/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.607284 meerschaum-1.7.0.dev2/meerschaum/config/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3719 2023-08-04 04:10:20.000000 meerschaum-1.7.0.dev2/meerschaum/config/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.607284 meerschaum-1.7.0.dev2/meerschaum/connectors/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/Connector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12064 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.608284 meerschaum-1.7.0.dev2/meerschaum/connectors/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4055 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/api/APIConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2759 2022-10-22 06:21:34.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/api/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/api/_delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2056 2022-11-01 03:12:07.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/api/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1572 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/api/_get.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2054 2022-11-18 03:44:05.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/api/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1185 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/api/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      933 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/api/_patch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19986 2023-04-26 08:12:59.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/api/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5227 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/api/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      922 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/api/_post.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/api/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5303 2022-08-19 04:59:44.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/api/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4048 2022-10-18 06:13:35.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/parse.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.608284 meerschaum-1.7.0.dev2/meerschaum/connectors/plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/plugin/PluginConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/plugin/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7215 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/poll.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.609284 meerschaum-1.7.0.dev2/meerschaum/connectors/sql/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9067 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/sql/SQLConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/sql/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3495 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/sql/_cli.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10197 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/sql/_create_engine.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12669 2023-06-28 23:16:36.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/sql/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    86905 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/sql/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8126 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/sql/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    26997 2023-07-13 02:20:19.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/sql/_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3312 2022-10-18 01:38:49.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/sql/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10095 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/sql/_users.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.609284 meerschaum-1.7.0.dev2/meerschaum/connectors/sql/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6489 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/sql/tables/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/sql/tables/types.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev2/meerschaum/connectors/sql/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.609284 meerschaum-1.7.0.dev2/meerschaum/core/
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.609284 meerschaum-1.7.0.dev2/meerschaum/core/Pipe/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15032 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev2/meerschaum/core/Pipe/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_attributes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2112 2022-11-13 04:57:20.000000 meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11702 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_data.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1854 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3146 2023-07-13 00:51:30.000000 meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3182 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    26496 2023-07-13 00:51:30.000000 meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_sync.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.609284 meerschaum-1.7.0.dev2/meerschaum/core/Plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev2/meerschaum/core/Plugin/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.610284 meerschaum-1.7.0.dev2/meerschaum/core/User/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev2/meerschaum/core/User/_User.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev2/meerschaum/core/User/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev2/meerschaum/core/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.610284 meerschaum-1.7.0.dev2/meerschaum/plugins/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    33813 2023-01-21 08:00:50.000000 meerschaum-1.7.0.dev2/meerschaum/plugins/_Plugin.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18398 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/plugins/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.611284 meerschaum-1.7.0.dev2/meerschaum/utils/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      444 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev2/meerschaum/utils/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.611284 meerschaum-1.7.0.dev2/meerschaum/utils/daemon/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24450 2023-08-04 04:19:36.000000 meerschaum-1.7.0.dev2/meerschaum/utils/daemon/Daemon.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3170 2023-01-09 03:01:33.000000 meerschaum-1.7.0.dev2/meerschaum/utils/daemon/Log.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5355 2023-01-09 09:50:51.000000 meerschaum-1.7.0.dev2/meerschaum/utils/daemon/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4302 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev2/meerschaum/utils/daemon/_names.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev2/meerschaum/utils/debug.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.611284 meerschaum-1.7.0.dev2/meerschaum/utils/formatting/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9387 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev2/meerschaum/utils/formatting/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2939 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev2/meerschaum/utils/formatting/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12729 2022-10-25 06:38:00.000000 meerschaum-1.7.0.dev2/meerschaum/utils/formatting/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3032 2022-10-18 06:13:35.000000 meerschaum-1.7.0.dev2/meerschaum/utils/formatting/_pprint.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3844 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev2/meerschaum/utils/formatting/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11791 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev2/meerschaum/utils/get_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3419 2022-10-18 06:13:35.000000 meerschaum-1.7.0.dev2/meerschaum/utils/interactive.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    62176 2023-07-13 00:51:30.000000 meerschaum-1.7.0.dev2/meerschaum/utils/misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev2/meerschaum/utils/networking.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.612284 meerschaum-1.7.0.dev2/meerschaum/utils/packages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    53718 2023-07-13 00:51:30.000000 meerschaum-1.7.0.dev2/meerschaum/utils/packages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7989 2023-07-14 22:02:27.000000 meerschaum-1.7.0.dev2/meerschaum/utils/packages/_packages.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-1.7.0.dev2/meerschaum/utils/packages/lazy_loader.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2781 2022-08-23 06:14:42.000000 meerschaum-1.7.0.dev2/meerschaum/utils/pool.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev2/meerschaum/utils/process.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16060 2022-05-02 19:58:56.000000 meerschaum-1.7.0.dev2/meerschaum/utils/prompt.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1886 2023-07-13 02:20:19.000000 meerschaum-1.7.0.dev2/meerschaum/utils/schedule.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34702 2023-07-13 00:51:30.000000 meerschaum-1.7.0.dev2/meerschaum/utils/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2152 2022-10-25 06:38:00.000000 meerschaum-1.7.0.dev2/meerschaum/utils/threading.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2535 2023-07-14 20:36:10.000000 meerschaum-1.7.0.dev2/meerschaum/utils/typing.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.612284 meerschaum-1.7.0.dev2/meerschaum/utils/venv/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3479 2022-10-25 06:38:00.000000 meerschaum-1.7.0.dev2/meerschaum/utils/venv/_Venv.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    22150 2023-04-26 08:12:59.000000 meerschaum-1.7.0.dev2/meerschaum/utils/venv/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6535 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev2/meerschaum/utils/warnings.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev2/meerschaum/utils/yaml.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 20:32:53.600284 meerschaum-1.7.0.dev2/meerschaum.egg-info/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10803 2023-08-04 20:32:53.000000 meerschaum-1.7.0.dev2/meerschaum.egg-info/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7865 2023-08-04 20:32:53.000000 meerschaum-1.7.0.dev2/meerschaum.egg-info/SOURCES.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-08-04 20:32:53.000000 meerschaum-1.7.0.dev2/meerschaum.egg-info/dependency_links.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2023-08-04 20:32:53.000000 meerschaum-1.7.0.dev2/meerschaum.egg-info/entry_points.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4657 2023-08-04 20:32:53.000000 meerschaum-1.7.0.dev2/meerschaum.egg-info/requires.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2023-08-04 20:32:53.000000 meerschaum-1.7.0.dev2/meerschaum.egg-info/top_level.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-08-04 20:32:53.000000 meerschaum-1.7.0.dev2/meerschaum.egg-info/zip-safe
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2023-08-04 20:32:53.612284 meerschaum-1.7.0.dev2/setup.cfg
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3056 2023-07-14 22:02:27.000000 meerschaum-1.7.0.dev2/setup.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.971783 meerschaum-1.7.0.dev3/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-1.7.0.dev3/LICENSE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-1.7.0.dev3/NOTICE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10803 2023-08-08 05:19:17.971783 meerschaum-1.7.0.dev3/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9248 2022-07-13 02:48:08.000000 meerschaum-1.7.0.dev3/README.md
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.953783 meerschaum-1.7.0.dev3/meerschaum/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1236 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2774 2022-10-22 06:28:47.000000 meerschaum-1.7.0.dev3/meerschaum/__main__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.954783 meerschaum-1.7.0.dev3/meerschaum/_internal/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.954783 meerschaum-1.7.0.dev3/meerschaum/_internal/arguments/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/arguments/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9741 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/arguments/_parse_arguments.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12586 2023-08-04 19:18:55.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/arguments/_parser.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.954783 meerschaum-1.7.0.dev3/meerschaum/_internal/docs/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/docs/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7719 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/docs/index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4625 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/entry.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.954783 meerschaum-1.7.0.dev3/meerschaum/_internal/gui/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1332 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/gui/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.955783 meerschaum-1.7.0.dev3/meerschaum/_internal/gui/app/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/gui/app/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/gui/app/_windows.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1016 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/gui/app/actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1678 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/gui/app/pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.955783 meerschaum-1.7.0.dev3/meerschaum/_internal/shell/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31489 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/shell/Shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2981 2022-10-22 06:28:01.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/shell/ShellCompleter.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/shell/ValidAutoSuggest.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/shell/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.955783 meerschaum-1.7.0.dev3/meerschaum/_internal/shell/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/shell/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.955783 meerschaum-1.7.0.dev3/meerschaum/_internal/term/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2021-12-09 07:32:03.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/term/TermPageHandler.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1960 2023-08-04 20:09:45.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/term/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      716 2023-08-04 03:39:01.000000 meerschaum-1.7.0.dev3/meerschaum/_internal/term/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.958783 meerschaum-1.7.0.dev3/meerschaum/actions/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8023 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev3/meerschaum/actions/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12109 2023-08-04 19:18:39.000000 meerschaum-1.7.0.dev3/meerschaum/actions/api.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14529 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/actions/bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4857 2022-08-23 06:14:42.000000 meerschaum-1.7.0.dev3/meerschaum/actions/clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6259 2023-06-28 23:16:36.000000 meerschaum-1.7.0.dev3/meerschaum/actions/copy.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15245 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev3/meerschaum/actions/delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2701 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev3/meerschaum/actions/drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9492 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/actions/edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7380 2022-10-18 06:13:35.000000 meerschaum-1.7.0.dev3/meerschaum/actions/install.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev3/meerschaum/actions/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-1.7.0.dev3/meerschaum/actions/os.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev3/meerschaum/actions/python.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11219 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/actions/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      605 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev3/meerschaum/actions/reload.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3211 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev3/meerschaum/actions/setup.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-1.7.0.dev3/meerschaum/actions/sh.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23468 2023-01-11 06:27:06.000000 meerschaum-1.7.0.dev3/meerschaum/actions/show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4224 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev3/meerschaum/actions/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5807 2023-06-28 23:16:36.000000 meerschaum-1.7.0.dev3/meerschaum/actions/stack.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18419 2023-08-08 04:43:35.000000 meerschaum-1.7.0.dev3/meerschaum/actions/start.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3948 2023-01-16 21:21:28.000000 meerschaum-1.7.0.dev3/meerschaum/actions/stop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15339 2022-12-15 02:09:06.000000 meerschaum-1.7.0.dev3/meerschaum/actions/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6073 2022-08-19 04:59:44.000000 meerschaum-1.7.0.dev3/meerschaum/actions/uninstall.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6307 2022-08-19 04:59:44.000000 meerschaum-1.7.0.dev3/meerschaum/actions/upgrade.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3348 2022-10-26 04:20:20.000000 meerschaum-1.7.0.dev3/meerschaum/actions/verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.958783 meerschaum-1.7.0.dev3/meerschaum/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7704 2023-08-04 03:03:40.000000 meerschaum-1.7.0.dev3/meerschaum/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev3/meerschaum/api/_chain.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1603 2023-08-08 00:12:13.000000 meerschaum-1.7.0.dev3/meerschaum/api/_events.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      961 2023-07-13 02:20:19.000000 meerschaum-1.7.0.dev3/meerschaum/api/_oauth2.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1432 2023-08-07 23:39:46.000000 meerschaum-1.7.0.dev3/meerschaum/api/_websockets.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.959783 meerschaum-1.7.0.dev3/meerschaum/api/dash/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2238 2023-01-09 08:57:26.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9788 2023-08-08 04:18:54.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/actions.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.960783 meerschaum-1.7.0.dev3/meerschaum/api/dash/assets/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/assets/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/assets/ansi_up.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/assets/banner_1920x320.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/assets/favicon.ico
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/assets/logo_48x48.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/assets/logo_500x500.png
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.960783 meerschaum-1.7.0.dev3/meerschaum/api/dash/callbacks/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      283 2023-07-21 01:07:26.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/callbacks/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    25742 2023-08-08 05:07:38.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/callbacks/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2613 2023-08-07 23:57:37.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/callbacks/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/callbacks/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3446 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/callbacks/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6272 2023-08-08 05:07:02.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/components.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2046 2023-08-04 04:44:53.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/graphs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3544 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13682 2022-10-31 13:18:31.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/keys.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.961783 meerschaum-1.7.0.dev3/meerschaum/api/dash/pages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-07-21 01:07:38.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/pages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3838 2023-08-08 05:03:38.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/pages/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      598 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/pages/error.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4601 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/pages/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1382 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/pages/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2398 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/pages/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15039 2022-10-31 14:15:34.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3054 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      895 2023-08-04 02:41:30.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/websockets.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3645 2023-08-08 05:10:38.000000 meerschaum-1.7.0.dev3/meerschaum/api/dash/webterm.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.961783 meerschaum-1.7.0.dev3/meerschaum/api/models/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/models/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/models/_interfaces.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/models/_locations.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/models/_metrics.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-1.7.0.dev3/meerschaum/api/models/_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.961783 meerschaum-1.7.0.dev3/meerschaum/api/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.961783 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.962783 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/css/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/css/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/css/bootstrap.min.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1674 2023-08-04 03:00:27.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/css/dash.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/css/dbc_dark.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/css/styles.css
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.962783 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/ico/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/ico/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/ico/logo.ico
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.962783 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/js/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/js/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/js/action_button.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/js/main.js
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.962783 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/png/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/png/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1083 2023-08-08 04:00:43.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/static/terminado.js
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.963783 meerschaum-1.7.0.dev3/meerschaum/api/resources/templates/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/templates/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/templates/index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/templates/old_index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/templates/secret.html
+-rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     2082 2021-12-09 07:32:03.000000 meerschaum-1.7.0.dev3/meerschaum/api/resources/templates/termpage.html
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.963783 meerschaum-1.7.0.dev3/meerschaum/api/routes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      564 2023-08-08 02:14:51.000000 meerschaum-1.7.0.dev3/meerschaum/api/routes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev3/meerschaum/api/routes/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1803 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev3/meerschaum/api/routes/_connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev3/meerschaum/api/routes/_index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1882 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev3/meerschaum/api/routes/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1714 2023-07-14 22:01:00.000000 meerschaum-1.7.0.dev3/meerschaum/api/routes/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21169 2023-01-21 08:00:50.000000 meerschaum-1.7.0.dev3/meerschaum/api/routes/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6151 2023-08-08 04:25:41.000000 meerschaum-1.7.0.dev3/meerschaum/api/routes/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7204 2023-07-14 20:54:29.000000 meerschaum-1.7.0.dev3/meerschaum/api/routes/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev3/meerschaum/api/routes/_version.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3096 2023-08-08 05:06:06.000000 meerschaum-1.7.0.dev3/meerschaum/api/routes/_webterm.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.964783 meerschaum-1.7.0.dev3/meerschaum/api/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      615 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev3/meerschaum/api/tables/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.964783 meerschaum-1.7.0.dev3/meerschaum/config/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11629 2023-01-11 04:28:52.000000 meerschaum-1.7.0.dev3/meerschaum/config/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5135 2023-05-05 04:35:54.000000 meerschaum-1.7.0.dev3/meerschaum/config/_default.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8807 2022-07-13 02:48:16.000000 meerschaum-1.7.0.dev3/meerschaum/config/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4507 2022-10-22 07:29:33.000000 meerschaum-1.7.0.dev3/meerschaum/config/_environment.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5556 2022-05-02 19:58:56.000000 meerschaum-1.7.0.dev3/meerschaum/config/_formatting.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      647 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev3/meerschaum/config/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1508 2023-01-11 05:57:34.000000 meerschaum-1.7.0.dev3/meerschaum/config/_patch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6648 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev3/meerschaum/config/_paths.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev3/meerschaum/config/_preprocess.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14567 2022-10-14 04:34:51.000000 meerschaum-1.7.0.dev3/meerschaum/config/_read_config.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3589 2021-11-21 05:32:46.000000 meerschaum-1.7.0.dev3/meerschaum/config/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4968 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev3/meerschaum/config/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       76 2023-08-08 05:17:32.000000 meerschaum-1.7.0.dev3/meerschaum/config/_version.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.965783 meerschaum-1.7.0.dev3/meerschaum/config/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/config/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.965783 meerschaum-1.7.0.dev3/meerschaum/config/stack/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8616 2023-06-28 23:16:36.000000 meerschaum-1.7.0.dev3/meerschaum/config/stack/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.965783 meerschaum-1.7.0.dev3/meerschaum/config/stack/grafana/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-1.7.0.dev3/meerschaum/config/stack/grafana/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.965783 meerschaum-1.7.0.dev3/meerschaum/config/stack/mosquitto/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/config/stack/mosquitto/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.965783 meerschaum-1.7.0.dev3/meerschaum/config/stack/mosquitto/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/config/stack/mosquitto/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.965783 meerschaum-1.7.0.dev3/meerschaum/config/stack/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/config/stack/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.965783 meerschaum-1.7.0.dev3/meerschaum/config/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3719 2023-08-04 04:10:20.000000 meerschaum-1.7.0.dev3/meerschaum/config/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.965783 meerschaum-1.7.0.dev3/meerschaum/connectors/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/Connector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12064 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.966783 meerschaum-1.7.0.dev3/meerschaum/connectors/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4055 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/api/APIConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2759 2022-10-22 06:21:34.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/api/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/api/_delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2056 2022-11-01 03:12:07.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/api/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1572 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/api/_get.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2054 2022-11-18 03:44:05.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/api/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1185 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/api/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      933 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/api/_patch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19986 2023-04-26 08:12:59.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/api/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5227 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/api/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      922 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/api/_post.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/api/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5303 2022-08-19 04:59:44.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/api/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4048 2022-10-18 06:13:35.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/parse.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.966783 meerschaum-1.7.0.dev3/meerschaum/connectors/plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/plugin/PluginConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/plugin/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7215 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/poll.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.967783 meerschaum-1.7.0.dev3/meerschaum/connectors/sql/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9067 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/sql/SQLConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/sql/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3495 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/sql/_cli.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10197 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/sql/_create_engine.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12669 2023-06-28 23:16:36.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/sql/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    86905 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/sql/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8126 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/sql/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    26997 2023-07-13 02:20:19.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/sql/_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3312 2022-10-18 01:38:49.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/sql/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10095 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/sql/_users.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.967783 meerschaum-1.7.0.dev3/meerschaum/connectors/sql/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6489 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/sql/tables/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/sql/tables/types.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev3/meerschaum/connectors/sql/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.967783 meerschaum-1.7.0.dev3/meerschaum/core/
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.968783 meerschaum-1.7.0.dev3/meerschaum/core/Pipe/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15032 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev3/meerschaum/core/Pipe/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_attributes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2112 2022-11-13 04:57:20.000000 meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11702 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_data.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1854 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3146 2023-07-13 00:51:30.000000 meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3182 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    26496 2023-07-13 00:51:30.000000 meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_sync.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.968783 meerschaum-1.7.0.dev3/meerschaum/core/Plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev3/meerschaum/core/Plugin/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.969783 meerschaum-1.7.0.dev3/meerschaum/core/User/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev3/meerschaum/core/User/_User.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev3/meerschaum/core/User/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev3/meerschaum/core/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.969783 meerschaum-1.7.0.dev3/meerschaum/plugins/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    33813 2023-01-21 08:00:50.000000 meerschaum-1.7.0.dev3/meerschaum/plugins/_Plugin.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18398 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/plugins/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.970783 meerschaum-1.7.0.dev3/meerschaum/utils/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      444 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev3/meerschaum/utils/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.970783 meerschaum-1.7.0.dev3/meerschaum/utils/daemon/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24459 2023-08-08 00:43:38.000000 meerschaum-1.7.0.dev3/meerschaum/utils/daemon/Daemon.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3170 2023-01-09 03:01:33.000000 meerschaum-1.7.0.dev3/meerschaum/utils/daemon/Log.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5355 2023-01-09 09:50:51.000000 meerschaum-1.7.0.dev3/meerschaum/utils/daemon/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4302 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev3/meerschaum/utils/daemon/_names.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev3/meerschaum/utils/debug.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.970783 meerschaum-1.7.0.dev3/meerschaum/utils/formatting/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9387 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev3/meerschaum/utils/formatting/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2939 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev3/meerschaum/utils/formatting/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12729 2022-10-25 06:38:00.000000 meerschaum-1.7.0.dev3/meerschaum/utils/formatting/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3032 2022-10-18 06:13:35.000000 meerschaum-1.7.0.dev3/meerschaum/utils/formatting/_pprint.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3844 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev3/meerschaum/utils/formatting/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11791 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev3/meerschaum/utils/get_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3419 2022-10-18 06:13:35.000000 meerschaum-1.7.0.dev3/meerschaum/utils/interactive.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    62176 2023-07-13 00:51:30.000000 meerschaum-1.7.0.dev3/meerschaum/utils/misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev3/meerschaum/utils/networking.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.971783 meerschaum-1.7.0.dev3/meerschaum/utils/packages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    53718 2023-07-13 00:51:30.000000 meerschaum-1.7.0.dev3/meerschaum/utils/packages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8106 2023-08-08 03:25:33.000000 meerschaum-1.7.0.dev3/meerschaum/utils/packages/_packages.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-1.7.0.dev3/meerschaum/utils/packages/lazy_loader.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2781 2022-08-23 06:14:42.000000 meerschaum-1.7.0.dev3/meerschaum/utils/pool.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev3/meerschaum/utils/process.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16060 2022-05-02 19:58:56.000000 meerschaum-1.7.0.dev3/meerschaum/utils/prompt.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1886 2023-07-13 02:20:19.000000 meerschaum-1.7.0.dev3/meerschaum/utils/schedule.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34702 2023-07-13 00:51:30.000000 meerschaum-1.7.0.dev3/meerschaum/utils/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2152 2022-10-25 06:38:00.000000 meerschaum-1.7.0.dev3/meerschaum/utils/threading.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2535 2023-07-14 20:36:10.000000 meerschaum-1.7.0.dev3/meerschaum/utils/typing.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.971783 meerschaum-1.7.0.dev3/meerschaum/utils/venv/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3479 2022-10-25 06:38:00.000000 meerschaum-1.7.0.dev3/meerschaum/utils/venv/_Venv.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    22150 2023-04-26 08:12:59.000000 meerschaum-1.7.0.dev3/meerschaum/utils/venv/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6535 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev3/meerschaum/utils/warnings.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev3/meerschaum/utils/yaml.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-08 05:19:17.954783 meerschaum-1.7.0.dev3/meerschaum.egg-info/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10803 2023-08-08 05:19:17.000000 meerschaum-1.7.0.dev3/meerschaum.egg-info/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7944 2023-08-08 05:19:17.000000 meerschaum-1.7.0.dev3/meerschaum.egg-info/SOURCES.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-08-08 05:19:17.000000 meerschaum-1.7.0.dev3/meerschaum.egg-info/dependency_links.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2023-08-08 05:19:17.000000 meerschaum-1.7.0.dev3/meerschaum.egg-info/entry_points.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4685 2023-08-08 05:19:17.000000 meerschaum-1.7.0.dev3/meerschaum.egg-info/requires.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2023-08-08 05:19:17.000000 meerschaum-1.7.0.dev3/meerschaum.egg-info/top_level.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-08-08 05:19:17.000000 meerschaum-1.7.0.dev3/meerschaum.egg-info/zip-safe
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2023-08-08 05:19:17.971783 meerschaum-1.7.0.dev3/setup.cfg
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3056 2023-07-14 22:02:27.000000 meerschaum-1.7.0.dev3/setup.py
```

### Comparing `meerschaum-1.7.0.dev2/LICENSE` & `meerschaum-1.7.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/PKG-INFO` & `meerschaum-1.7.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 1.7.0.dev2
+Version: 1.7.0.dev3
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
```

### Comparing `meerschaum-1.7.0.dev2/README.md` & `meerschaum-1.7.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/__main__.py` & `meerschaum-1.7.0.dev3/meerschaum/__main__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/_internal/arguments/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/_internal/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/_internal/arguments/_parse_arguments.py` & `meerschaum-1.7.0.dev3/meerschaum/_internal/arguments/_parse_arguments.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/_internal/arguments/_parser.py` & `meerschaum-1.7.0.dev3/meerschaum/_internal/arguments/_parser.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/_internal/docs/index.py` & `meerschaum-1.7.0.dev3/meerschaum/_internal/docs/index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/_internal/entry.py` & `meerschaum-1.7.0.dev3/meerschaum/_internal/entry.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/_internal/gui/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/_internal/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/_internal/gui/app/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/_internal/gui/app/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/_internal/gui/app/_windows.py` & `meerschaum-1.7.0.dev3/meerschaum/_internal/gui/app/_windows.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/_internal/gui/app/actions.py` & `meerschaum-1.7.0.dev3/meerschaum/_internal/gui/app/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/_internal/gui/app/pipes.py` & `meerschaum-1.7.0.dev3/meerschaum/_internal/gui/app/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/_internal/shell/Shell.py` & `meerschaum-1.7.0.dev3/meerschaum/_internal/shell/Shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/_internal/shell/ShellCompleter.py` & `meerschaum-1.7.0.dev3/meerschaum/_internal/shell/ShellCompleter.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/_internal/shell/ValidAutoSuggest.py` & `meerschaum-1.7.0.dev3/meerschaum/_internal/shell/ValidAutoSuggest.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/_internal/term/TermPageHandler.py` & `meerschaum-1.7.0.dev3/meerschaum/_internal/term/TermPageHandler.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/_internal/term/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/_internal/term/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/_internal/term/tools.py` & `meerschaum-1.7.0.dev3/meerschaum/_internal/term/tools.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/api.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/api.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/bootstrap.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/clear.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/copy.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/copy.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/delete.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/drop.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/edit.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/install.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/install.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/login.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/os.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/os.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/python.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/python.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/register.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/reload.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/reload.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/setup.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/setup.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/sh.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/sh.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/show.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/sql.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/stack.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/stack.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/start.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/start.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,24 +411,24 @@
     Options:
         - `-p`, `--port`
             The port to which the webterm binds.
             Defaults to 8765, and `--force` will choose the next available port.
     
         - `--host`
             The host interface to which the webterm binds.
-            Defaults to '0.0.0.0'.
+            Defaults to '127.0.0.1'.
     """
     from meerschaum._internal.term import get_webterm_app_and_manager, tornado, tornado_ioloop
     from meerschaum._internal.term.tools import is_webterm_running
     from meerschaum.utils.networking import find_open_ports, is_port_in_use
     from meerschaum.utils.packages import attempt_import
     from meerschaum.utils.warnings import info
 
     if host is None:
-        host = '0.0.0.0'
+        host = '127.0.0.1'
     if port is None:
         port = 8765
     if sysargs is None:
         sysargs = ['start', 'webterm']
     tornado_app, term_manager = get_webterm_app_and_manager()
 
     if is_webterm_running(host, port):
```

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/stop.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/stop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/sync.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/uninstall.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/uninstall.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/upgrade.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/upgrade.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/actions/verify.py` & `meerschaum-1.7.0.dev3/meerschaum/actions/verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/api/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/_chain.py` & `meerschaum-1.7.0.dev3/meerschaum/api/_chain.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/_events.py` & `meerschaum-1.7.0.dev3/meerschaum/api/_events.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,30 +3,42 @@
 # vim:fenc=utf-8
 
 """
 Declare FastAPI events in this module (startup, shutdown, etc.).
 """
 
 import sys, os, time
-from meerschaum.api import app, get_api_connector, get_uvicorn_config, debug, uvicorn_config_path
+from meerschaum.api import (
+    app,
+    get_api_connector,
+    get_uvicorn_config,
+    debug,
+    no_dash,
+    uvicorn_config_path,
+)
 from meerschaum.utils.debug import dprint
 from meerschaum.connectors.poll import retry_connect
-from meerschaum.utils.threading import Thread
 from meerschaum.utils.warnings import warn
+from meerschaum._internal.term.tools import is_webterm_running
 
 @app.on_event("startup")
 async def startup():
     conn = get_api_connector()
     try:
+        if not no_dash:
+            from meerschaum.api.dash.webterm import start_webterm
+            start_webterm()
         connected = retry_connect(
             get_api_connector(),
             workers = get_uvicorn_config().get('workers', None),
             debug = debug
         )
     except Exception as e:
+        import traceback
+        traceback.print_exc()
         connected = False
     if not connected:
         await shutdown()
         os._exit(1)
 
 
 @app.on_event("shutdown")
@@ -35,21 +47,11 @@
         dprint("Closing connection...")
     if get_api_connector().type == 'sql':
         get_api_connector().engine.dispose()
 
     ### Terminate any running jobs left over.
     if 'meerschaum.api.dash' in sys.modules:
         from meerschaum.api.dash.actions import running_jobs, stop_action
-        from meerschaum.utils.packages import run_python_package
-        from meerschaum.config.static import STATIC_CONFIG
-        from meerschaum._internal.term.tools import is_webterm_running
-        run_python_package(
-            'meerschaum', [
-                'delete', 'job',
-                STATIC_CONFIG['api']['webterm_job_name'], '-y'
-            ],
-            venv = None,
-            foreground = False,
-            capture_output = True,
-        )
+        from meerschaum.api.dash.webterm import stop_webterm
+        stop_webterm()
         for session_id in running_jobs:
             stop_action({'session-store.data': {'session-id': session_id}})
```

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/_oauth2.py` & `meerschaum-1.7.0.dev3/meerschaum/api/_oauth2.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/_websockets.py` & `meerschaum-1.7.0.dev3/meerschaum/api/_websockets.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,9 +37,19 @@
     await websocket.send_text(join_msg)
     websockets[session_id] = websocket
     while True:
         try:
             data = await websocket.receive_text()
             await websocket.send_text(str(datetime.datetime.utcnow()))
         except fastapi.WebSocketDisconnect:
-            del websockets[session_id]
+            delete_websocket_session(session_id)
             break
+
+
+def delete_websocket_session(session_id: str) -> None:
+    """
+    Delete a websocket session if it exists.
+    """
+    try:
+        del websockets[session_id]
+    except KeyError:
+        pass
```

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/actions.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from meerschaum.api import debug, CHECK_UPDATE
 from meerschaum.api.dash import (
     running_jobs, stopped_jobs, running_monitors, stopped_monitors, active_sessions
 )
 from meerschaum.api import get_api_connector
 from meerschaum.api.dash.connectors import get_web_connector
 from meerschaum.api.dash.components import alert_from_success_tuple, console_div
+from meerschaum.api.dash.webterm import get_webterm
 from meerschaum.api.dash.pipes import pipes_from_state, keys_from_state
 from meerschaum.api.dash.websockets import ws_send
 from meerschaum.api._websockets import websockets
 html, dcc = import_html(check_update=CHECK_UPDATE), import_dcc(check_update=CHECK_UPDATE)
 from meerschaum.config import get_config
 from meerschaum.core import User
 
@@ -259,11 +260,13 @@
     session_id = state['session-store.data'].get('session-id', None)
     thread = running_jobs.get(session_id, {}).get('parent_thread', None)
     proc = running_jobs.get(session_id, {}).get('child_process', None)
     if proc is not None and proc.poll() is None:
         proc.terminate()
         thread.join()
     success_tuple = True, "Success"
+    webterm_iframe, webterm_alerts = get_webterm(state)
+    console_to_return = console_div if webterm_alerts else webterm_iframe
     return (
-        [console_div],
+        [console_to_return],
         [alert_from_success_tuple(success_tuple)]
     )
```

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/assets/ansi_up.js` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/assets/ansi_up.js`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/assets/banner_1920x320.png` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/assets/banner_1920x320.png`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/assets/favicon.ico` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/assets/logo_48x48.png` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/assets/logo_48x48.png`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/assets/logo_500x500.png` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/assets/logo_500x500.png`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/callbacks/dashboard.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/callbacks/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 from meerschaum.connectors.parse import parse_instance_keys
 from meerschaum.api.dash.pipes import get_pipes_cards, pipe_from_ctx, accordion_items_from_pipe
 from meerschaum.api.dash.jobs import get_jobs_cards
 from meerschaum.api.dash.plugins import get_plugins_cards
 from meerschaum.api.dash.users import get_users_cards
 from meerschaum.api.dash.graphs import get_graphs_cards
 from meerschaum.api.dash.webterm import get_webterm
-from meerschaum.api.dash.components import alert_from_success_tuple, console_div, build_cards_grid
+from meerschaum.api.dash.components import (
+    alert_from_success_tuple, console_div, build_cards_grid,
+)
 from meerschaum.api.dash.actions import execute_action, check_input_interval, stop_action
 import meerschaum.api.dash.pages as pages
 from meerschaum.utils.typing import Dict
 from meerschaum.utils.debug import dprint
 from meerschaum.utils.packages import attempt_import, import_html, import_dcc
 from meerschaum.utils.misc import (
     string_to_dict, get_connector_labels, json_serialize_datetime, filter_keywords
@@ -102,43 +104,50 @@
 _required_login = {''}
  
 @dash_app.callback(
     Output('page-layout-div', 'children'),
     Output('session-store', 'data'),
     Input('location', 'pathname'),
     Input('session-store', 'data'),
+    State('location', 'href'),
 )
-def update_page_layout_div(pathname: str, session_store_data: Dict[str, Any]):
+def update_page_layout_div(
+        pathname: str, 
+        session_store_data: Dict[str, Any],
+        location_href: str,
+    ) -> Tuple[List[Any], Dict[str, Any]]:
     """
     Route the user to the correct page.
 
     Parameters
     ----------
     pathname: str :
         The path in the browser.
         
     session_store_data: Dict[str, Any]:
         The stored session data.
 
     Returns
     -------
-    A tuple of the page layout, new session store data, and the web socket connection.
-
+    A tuple of the page layout and new session store data.
     """
     ctx = dash.callback_context
     dash_endpoint = endpoints['dash']
     try:
         session_id = session_store_data.get('session-id', None) 
     except AttributeError:
         session_id = None
 
     ### Bypass login if `--no-auth` is specified.
     if session_id not in active_sessions and no_auth:
         session_store_data['session-id'] = str(uuid.uuid4())
         active_sessions[session_store_data['session-id']] = {'username': 'no-auth'}
+
+        ### Sometimes the href is an empty string, so store it here for later.
+        session_store_data['location.href'] = location_href
         session_store_to_return = session_store_data
     else:
         session_store_to_return = dash.no_update
 
     _path = (
         pathname.rstrip('/') + '/'
     ).replace(
@@ -165,41 +174,41 @@
     Input('go-button', 'n_clicks'),
     Input('cancel-button', 'n_clicks'),
     Input('get-pipes-button', 'n_clicks'),
     Input('get-jobs-button', 'n_clicks'),
     Input('get-plugins-button', 'n_clicks'),
     Input('get-users-button', 'n_clicks'),
     Input('get-graphs-button', 'n_clicks'),
-    Input('open-shell-button', 'n_clicks'),
     Input('check-input-interval', 'n_intervals'),
     State('location', 'href'),
     State('session-store', 'data'),
     *keys_state,
-    #  prevent_initial_call=True,
 )
 def update_content(*args):
     """
     Determine which trigger is seeking to update the content div,
     and execute the appropriate function.
     """
     ctx = dash.callback_context
+    location_href = ctx.states['session-store.data'].get('location.href', None)
     websocket_div_children = (
         dex.WebSocket(
             id = 'ws',
-            url = ws_url_from_href(ctx.states['location.href']),
+            url = ws_url_from_href(location_href),
             protocols = ['ws', 'wss']
-        ) if not ctx.states.get('ws.url', None) and ctx.states.get('location.href', None)
+        ) if not ctx.states.get('ws.url', None) and location_href
         else dash.no_update
     )
 
     trigger = None
+    initial_load = False
     ### Open the webterm on the initial load.
     if not ctx.triggered:
-        #  trigger = 'open-shell-button'
-        return [], [], True, websocket_div_children
+        initial_load = True
+        trigger = 'open-shell-button'
 
     if len(ctx.triggered) > 1 and 'check-input-interval.n_intervals' in ctx.triggered:
         ctx.triggered.remove('check-input-interval.n_intervals')
     trigger = ctx.triggered[0]['prop_id'].split('.')[0] if not trigger else trigger
 
     session_data = args[-1]
 
@@ -231,14 +240,20 @@
     )
     enable_check_input_interval = False
 
     content, alerts = triggers[trigger](
         ctx.states,
         **filter_keywords(triggers[trigger], session_data=session_data)
     )
+
+    ### If the webterm fails on initial load (e.g. insufficient permissions),
+    ### don't display the alerts just yet.
+    if initial_load and alerts:
+        return console_div, [], True, websocket_div_children
+
     if trigger.startswith('get-') and trigger.endswith('-button'):
         content = build_cards_grid(content, num_columns=trigger_num_cols.get(trigger, 3))
     return content, alerts, not enable_check_input_interval, websocket_div_children
 
 @dash_app.callback(
     Output('action-dropdown', 'value'),
     Output('subaction-dropdown', 'value'),
@@ -493,15 +508,15 @@
 def ws_receive(message):
     """
     Display received messages.
     """
     if not message and message != '':
         raise PreventUpdate
     if not message.get('data', None):
-        return console_div
+        raise PreventUpdate
     return [html.Div(
         [html.Pre(message['data'], id='console-pre')],
         id = 'console-div',
     )]
 
 dash_app.clientside_callback(
     """
```

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/callbacks/login.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/callbacks/login.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,31 +40,33 @@
     Output('username-input', 'className'),
     Output('location', 'pathname'),
     Input('username-input', 'n_submit'),
     Input('password-input', 'n_submit'),
     Input('login-button', 'n_clicks'),
     State('username-input', 'value'),
     State('password-input', 'value'),
+    State('location', 'href'),
 )
 def login_button_click(
         username_submit,
         password_submit,
         n_clicks,
         username,
         password,
+        location_href,
     ):
     """
     When the user submits the login form, check the login.
     On successful login, set the session id.
     """
     form_class = 'form-control'
     ctx = dash.callback_context
     if not username or not password or not ctx.triggered:
         return {}, form_class, dash.no_update
     try:
-        token_dict = login({'username' : username, 'password' : password})
-        session_data = {'session-id': str(uuid.uuid4())}
+        token_dict = login({'username': username, 'password': password})
+        session_data = {'session-id': str(uuid.uuid4()), 'location.href': location_href}
         active_sessions[session_data['session-id']] = {'username': username}
     except HTTPException:
         form_class += ' is-invalid'
         session_data = None
     return session_data, form_class, (dash.no_update if not session_data else endpoints['dash'])
```

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/callbacks/plugins.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/callbacks/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/callbacks/register.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/components.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,15 @@
     dbc.CardBody(
         dbc.Row([
             dbc.Col(go_button, lg=3, md=3),
             dbc.Col(cancel_button, lg=3, md=3),
             dbc.Col(show_pipes_button, lg=3, md=3),
             dbc.Col(lg=True, md=False),
             dbc.Col(get_items_menu, lg=2, md=2),
-        ],
-        #  no_gutters=False
-        )
+        ])
     )
 )
 console_div = html.Div(id='console-div', children=[html.Pre(get_shell().intro, id='console-pre')])
 
 location = dcc.Location(id='location', refresh=False)
 
 search_parameters_editor = dash_ace.DashAceEditor(
@@ -111,21 +109,21 @@
                 href = '/docs',
                 style = {"textDecoration": "none"},
             ),
             dbc.NavbarToggler(id="navbar-toggler", n_clicks=0),
             dbc.Collapse(
                 dbc.Row(
                     [
-                        dbc.Col(
-                            dbc.Button(
-                                html.B("Open Shell"),
-                                outline = True,
-                                id = "open-shell-button"
-                            ),
-                        ),
+                        #  dbc.Col(
+                            #  dbc.Button(
+                                #  html.B("Open Shell"),
+                                #  outline = True,
+                                #  id = "open-shell-button"
+                            #  ),
+                        #  ),
                         dbc.Col(instance_select),
                         dbc.Col(
                             dbc.Button(
                                 "Sign out",
                                 color = 'link',
                                 style = {'margin-left': '30px'},
                                 id = 'sign-out-button',
```

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/connectors.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/graphs.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/graphs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/jobs.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/keys.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/keys.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/pages/dashboard.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/pages/dashboard.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/pages/error.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/pages/error.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/pages/login.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/pages/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/pages/plugins.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/pages/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/pages/register.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/pages/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/pipes.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/plugins.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/users.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/dash/websockets.py` & `meerschaum-1.7.0.dev3/meerschaum/api/dash/websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/resources/static/css/bootstrap.min.css` & `meerschaum-1.7.0.dev3/meerschaum/api/resources/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/resources/static/css/dash.css` & `meerschaum-1.7.0.dev3/meerschaum/api/resources/static/css/dash.css`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/resources/static/css/dbc_dark.css` & `meerschaum-1.7.0.dev3/meerschaum/api/resources/static/css/dbc_dark.css`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/resources/static/ico/logo.ico` & `meerschaum-1.7.0.dev3/meerschaum/api/resources/static/ico/logo.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/resources/static/js/action_button.js` & `meerschaum-1.7.0.dev3/meerschaum/api/resources/static/js/action_button.js`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/resources/templates/index.html` & `meerschaum-1.7.0.dev3/meerschaum/api/resources/templates/index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/resources/templates/old_index.html` & `meerschaum-1.7.0.dev3/meerschaum/api/resources/templates/old_index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/resources/templates/termpage.html` & `meerschaum-1.7.0.dev3/meerschaum/api/resources/templates/termpage.html`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/routes/_actions.py` & `meerschaum-1.7.0.dev3/meerschaum/api/routes/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/routes/_connectors.py` & `meerschaum-1.7.0.dev3/meerschaum/api/routes/_connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/routes/_index.py` & `meerschaum-1.7.0.dev3/meerschaum/api/routes/_index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/routes/_login.py` & `meerschaum-1.7.0.dev3/meerschaum/api/routes/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/routes/_misc.py` & `meerschaum-1.7.0.dev3/meerschaum/api/routes/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/routes/_pipes.py` & `meerschaum-1.7.0.dev3/meerschaum/api/routes/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/routes/_plugins.py` & `meerschaum-1.7.0.dev3/meerschaum/api/routes/_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 plugins_endpoint = endpoints['plugins']
 
 @app.post(plugins_endpoint + '/{name}', tags=['Plugins'])
 def register_plugin(
         name: str,
         version: str = None,
         attributes: str = None,
-        archive : UploadFile = File(...),
+        archive: UploadFile = File(...),
         curr_user = (
             fastapi.Depends(manager) if not no_auth else None
         ),
     ) -> SuccessTuple:
     """
     Register a plugin and save its archive file.
```

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/routes/_users.py` & `meerschaum-1.7.0.dev3/meerschaum/api/routes/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/routes/_version.py` & `meerschaum-1.7.0.dev3/meerschaum/api/routes/_version.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/api/tables/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/api/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/config/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/config/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/config/_default.py` & `meerschaum-1.7.0.dev3/meerschaum/config/_default.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/config/_edit.py` & `meerschaum-1.7.0.dev3/meerschaum/config/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/config/_environment.py` & `meerschaum-1.7.0.dev3/meerschaum/config/_environment.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/config/_formatting.py` & `meerschaum-1.7.0.dev3/meerschaum/config/_formatting.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/config/_jobs.py` & `meerschaum-1.7.0.dev3/meerschaum/config/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/config/_patch.py` & `meerschaum-1.7.0.dev3/meerschaum/config/_patch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/config/_paths.py` & `meerschaum-1.7.0.dev3/meerschaum/config/_paths.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/config/_preprocess.py` & `meerschaum-1.7.0.dev3/meerschaum/config/_preprocess.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/config/_read_config.py` & `meerschaum-1.7.0.dev3/meerschaum/config/_read_config.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/config/_shell.py` & `meerschaum-1.7.0.dev3/meerschaum/config/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/config/_sync.py` & `meerschaum-1.7.0.dev3/meerschaum/config/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/config/stack/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/config/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/config/stack/grafana/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/config/stack/grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/config/static/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/config/static/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/Connector.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/Connector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/api/APIConnector.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/api/APIConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/api/_actions.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/api/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/api/_delete.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/api/_delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/api/_fetch.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/api/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/api/_get.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/api/_get.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/api/_login.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/api/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/api/_misc.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/api/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/api/_patch.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/api/_patch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/api/_pipes.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/api/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/api/_plugins.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/api/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/api/_post.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/api/_post.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/api/_uri.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/api/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/api/_users.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/api/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/parse.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/parse.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/plugin/PluginConnector.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/plugin/PluginConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/poll.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/poll.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/sql/SQLConnector.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/sql/SQLConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/sql/_cli.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/sql/_cli.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/sql/_create_engine.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/sql/_create_engine.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/sql/_fetch.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/sql/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/sql/_pipes.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/sql/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/sql/_plugins.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/sql/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/sql/_sql.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/sql/_sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/sql/_uri.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/sql/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/sql/_users.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/sql/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/sql/tables/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/sql/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/connectors/sql/tables/types.py` & `meerschaum-1.7.0.dev3/meerschaum/connectors/sql/tables/types.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/core/Pipe/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/core/Pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_attributes.py` & `meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_attributes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_bootstrap.py` & `meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_clear.py` & `meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_data.py` & `meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_data.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_delete.py` & `meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_drop.py` & `meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_dtypes.py` & `meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_dtypes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_edit.py` & `meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_fetch.py` & `meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_register.py` & `meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_show.py` & `meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/core/Pipe/_sync.py` & `meerschaum-1.7.0.dev3/meerschaum/core/Pipe/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/core/User/_User.py` & `meerschaum-1.7.0.dev3/meerschaum/core/User/_User.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/plugins/_Plugin.py` & `meerschaum-1.7.0.dev3/meerschaum/plugins/_Plugin.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/plugins/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/daemon/Daemon.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/daemon/Daemon.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             Override reading from the properties JSON by providing an existing dictionary.
             Defaults to `None`.
         """
         _pickle = self.__dict__.get('_pickle', False)
         if daemon_id is not None:
             self.daemon_id = daemon_id
             if not self.pickle_path.exists() and not target and ('target' not in self.__dict__):
-                error(
+                raise Exception(
                     f"Daemon '{self.daemon_id}' does not exist. "
                     + "Pass a target to create a new Daemon."
                 )
         if 'target' not in self.__dict__:
             if target is None:
                 error(f"Cannot create a Daemon without a target.")
             self.target = target
@@ -397,15 +397,15 @@
                 str(self.pid_path.as_posix()),
                 sigint = _quit,
                 sigterm = _quit,
                 sigabrt = _quit,
             )
         return self._sighandler
 
-    def mkdir_if_not_exists(self, allow_dirty_run : bool = False):
+    def mkdir_if_not_exists(self, allow_dirty_run: bool = False):
         """Create the Daemon's directory.
         If `allow_dirty_run` is `False` and the directory already exists,
         raise a `FileExistsError`.
         """
         try:
             self.path.mkdir(parents=True, exist_ok=False)
             _already_exists = False
```

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/daemon/Log.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/daemon/Log.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/daemon/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/daemon/_names.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/daemon/_names.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/debug.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/debug.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/formatting/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/formatting/_jobs.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/formatting/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/formatting/_pipes.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/formatting/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/formatting/_pprint.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/formatting/_pprint.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/formatting/_shell.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/formatting/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/get_pipes.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/get_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/interactive.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/interactive.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/misc.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/networking.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/networking.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/packages/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/packages/_packages.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/packages/_packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,16 @@
     'dotenv'                         : 'python-dotenv>=0.20.0',
     'websockets'                     : 'websockets>=11.0.3',
     'fastapi'                        : 'fastapi>=0.100.0',
     'passlib'                        : 'passlib>=1.7.4',
     'fastapi_login'                  : 'fastapi-login>=1.7.2',
     'multipart'                      : 'python-multipart>=0.0.5',
     'pydantic'                       : 'pydantic>=1.7.4',
+    'httpx'                          : 'httpx>=0.24.1',
+    'websockets'                     : 'websockets>=11.0.3',
 }
 packages['api'].update(packages['sql'])
 packages['api'].update(packages['formatting'])
 packages['api'].update(packages['dash'])
 
 all_packages = {}
 for group, import_names in packages.items():
```

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/packages/lazy_loader.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/packages/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/pool.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/pool.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/process.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/process.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/prompt.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/schedule.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/schedule.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/sql.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/threading.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/threading.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/typing.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/typing.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/venv/_Venv.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/venv/_Venv.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/venv/__init__.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/warnings.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum/utils/yaml.py` & `meerschaum-1.7.0.dev3/meerschaum/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.7.0.dev2/meerschaum.egg-info/PKG-INFO` & `meerschaum-1.7.0.dev3/meerschaum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 1.7.0.dev2
+Version: 1.7.0.dev3
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
```

### Comparing `meerschaum-1.7.0.dev2/meerschaum.egg-info/SOURCES.txt` & `meerschaum-1.7.0.dev3/meerschaum.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 meerschaum/api/models/__init__.py
 meerschaum/api/models/_interfaces.py
 meerschaum/api/models/_locations.py
 meerschaum/api/models/_metrics.py
 meerschaum/api/models/_pipes.py
 meerschaum/api/resources/__init__.py
 meerschaum/api/resources/static/__init__.py
+meerschaum/api/resources/static/terminado.js
 meerschaum/api/resources/static/css/__init__.py
 meerschaum/api/resources/static/css/bootstrap.min.css
 meerschaum/api/resources/static/css/dash.css
 meerschaum/api/resources/static/css/dbc_dark.css
 meerschaum/api/resources/static/css/styles.css
 meerschaum/api/resources/static/ico/__init__.py
 meerschaum/api/resources/static/ico/logo.ico
@@ -120,14 +121,15 @@
 meerschaum/api/routes/_index.py
 meerschaum/api/routes/_login.py
 meerschaum/api/routes/_misc.py
 meerschaum/api/routes/_pipes.py
 meerschaum/api/routes/_plugins.py
 meerschaum/api/routes/_users.py
 meerschaum/api/routes/_version.py
+meerschaum/api/routes/_webterm.py
 meerschaum/api/tables/__init__.py
 meerschaum/config/__init__.py
 meerschaum/config/_default.py
 meerschaum/config/_edit.py
 meerschaum/config/_environment.py
 meerschaum/config/_formatting.py
 meerschaum/config/_jobs.py
```

### Comparing `meerschaum-1.7.0.dev2/meerschaum.egg-info/requires.txt` & `meerschaum-1.7.0.dev3/meerschaum.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 python-dotenv>=0.20.0
 websockets>=11.0.3
 fastapi>=0.100.0
 passlib>=1.7.4
 fastapi-login>=1.7.2
 python-multipart>=0.0.5
 pydantic>=1.7.4
+httpx>=0.24.1
 numpy>=1.18.5
 pandas>=1.5.3
 pytz>=2022.1.0
 joblib>=0.17.0
 SQLAlchemy>=2.0.5
 databases>=0.4.0
 aiosqlite>=0.16.0
@@ -218,14 +219,15 @@
 python-dotenv>=0.20.0
 websockets>=11.0.3
 fastapi>=0.100.0
 passlib>=1.7.4
 fastapi-login>=1.7.2
 python-multipart>=0.0.5
 pydantic>=1.7.4
+httpx>=0.24.1
 
 [gui]
 toga>=0.3.0-dev29
 terminado>=0.12.1
 tornado>=6.1.0
 tornado-xstatic>=0.2.0
 XStatic>=1.0.2
```

### Comparing `meerschaum-1.7.0.dev2/setup.py` & `meerschaum-1.7.0.dev3/setup.py`

 * *Files identical despite different names*

