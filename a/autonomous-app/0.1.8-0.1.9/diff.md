# Comparing `tmp/autonomous-app-0.1.8.tar.gz` & `tmp/autonomous-app-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomous-app-0.1.8.tar", last modified: Wed Aug  2 17:38:23 2023, max compression
+gzip compressed data, was "autonomous-app-0.1.9.tar", last modified: Wed Aug  2 18:26:28 2023, max compression
```

## Comparing `autonomous-app-0.1.8.tar` & `autonomous-app-0.1.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.899062 autonomous-app-0.1.8/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-03-07 12:36:40.000000 autonomous-app-0.1.8/LICENSE
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-08-02 17:38:23.898062 autonomous-app-0.1.8/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2011 2023-06-20 21:09:23.000000 autonomous-app-0.1.8/README.md
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1469 2023-07-20 14:57:42.000000 autonomous-app-0.1.8/pyproject.toml
--rw-r--r--   0 samoore   (1000) samoore   (1000)      523 2023-07-27 14:43:37.000000 autonomous-app-0.1.8/requirements.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-08-02 17:38:23.900061 autonomous-app-0.1.8/setup.cfg
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-04-04 14:14:59.000000 autonomous-app-0.1.8/setup.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.891062 autonomous-app-0.1.8/src/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.893061 autonomous-app-0.1.8/src/autonomous/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       86 2023-08-02 17:38:13.000000 autonomous-app-0.1.8/src/autonomous/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.893061 autonomous-app-0.1.8/src/autonomous/apis/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       27 2023-06-20 19:34:19.000000 autonomous-app-0.1.8/src/autonomous/apis/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2149 2023-07-07 13:12:31.000000 autonomous-app-0.1.8/src/autonomous/apis/openai.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.894062 autonomous-app-0.1.8/src/autonomous/apis/version_control/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1069 2023-03-07 16:24:11.000000 autonomous-app-0.1.8/src/autonomous/apis/version_control/GHCallbacks.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1155 2023-03-07 21:09:26.000000 autonomous-app-0.1.8/src/autonomous/apis/version_control/GHOrganization.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4622 2023-03-07 16:24:11.000000 autonomous-app-0.1.8/src/autonomous/apis/version_control/GHRepo.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      196 2023-03-07 16:24:11.000000 autonomous-app-0.1.8/src/autonomous/apis/version_control/GHVersionControl.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      117 2023-03-07 16:24:11.000000 autonomous-app-0.1.8/src/autonomous/apis/version_control/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.890062 autonomous-app-0.1.8/src/autonomous/app_template/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.894062 autonomous-app-0.1.8/src/autonomous/app_template/app/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       54 2023-07-28 15:13:30.000000 autonomous-app-0.1.8/src/autonomous/app_template/app/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1598 2023-07-27 16:48:05.000000 autonomous-app-0.1.8/src/autonomous/app_template/app/app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1316 2023-07-27 17:51:13.000000 autonomous-app-0.1.8/src/autonomous/app_template/app/config.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.894062 autonomous-app-0.1.8/src/autonomous/app_template/app/models/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-04-04 14:32:12.000000 autonomous-app-0.1.8/src/autonomous/app_template/app/models/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      203 2023-04-04 15:41:08.000000 autonomous-app-0.1.8/src/autonomous/app_template/app/models/model.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      517 2023-07-28 15:15:34.000000 autonomous-app-0.1.8/src/autonomous/app_template/app/tasks.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.894062 autonomous-app-0.1.8/src/autonomous/app_template/app/views/
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-04 14:32:12.000000 autonomous-app-0.1.8/src/autonomous/app_template/app/views/admin.py
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-28 17:48:57.000000 autonomous-app-0.1.8/src/autonomous/app_template/app/views/index.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.895062 autonomous-app-0.1.8/src/autonomous/app_template/tests/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-04 14:32:12.000000 autonomous-app-0.1.8/src/autonomous/app_template/tests/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      545 2023-07-28 15:11:47.000000 autonomous-app-0.1.8/src/autonomous/app_template/tests/conftest.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      432 2023-08-02 17:36:52.000000 autonomous-app-0.1.8/src/autonomous/app_template/tests/test_app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1021 2023-07-28 15:54:14.000000 autonomous-app-0.1.8/src/autonomous/app_template/tests/test_tasks.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.895062 autonomous-app-0.1.8/src/autonomous/app_template/vendor/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1124 2023-04-13 17:57:17.000000 autonomous-app-0.1.8/src/autonomous/app_template/vendor/gunicorn.conf.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2252 2023-06-08 19:19:57.000000 autonomous-app-0.1.8/src/autonomous/assets.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)       42 2023-04-04 14:14:59.000000 autonomous-app-0.1.8/src/autonomous/cli.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.895062 autonomous-app-0.1.8/src/autonomous/db/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       94 2023-07-07 12:00:23.000000 autonomous-app-0.1.8/src/autonomous/db/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      812 2023-07-07 12:05:15.000000 autonomous-app-0.1.8/src/autonomous/db/autodb.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      531 2023-04-04 14:14:59.000000 autonomous-app-0.1.8/src/autonomous/db/storage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2521 2023-06-20 21:17:55.000000 autonomous-app-0.1.8/src/autonomous/db/table.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1245 2023-06-01 20:06:24.000000 autonomous-app-0.1.8/src/autonomous/logger.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.896062 autonomous-app-0.1.8/src/autonomous/model/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-02 18:01:05.000000 autonomous-app-0.1.8/src/autonomous/model/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4159 2023-08-02 16:53:49.000000 autonomous-app-0.1.8/src/autonomous/model/automodel.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      683 2023-08-02 17:35:38.000000 autonomous-app-0.1.8/src/autonomous/model/orm.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.896062 autonomous-app-0.1.8/src/autonomous/storage/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       88 2023-06-13 18:11:53.000000 autonomous-app-0.1.8/src/autonomous/storage/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      447 2023-06-05 17:49:27.000000 autonomous-app-0.1.8/src/autonomous/storage/basestorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1620 2023-07-07 13:13:20.000000 autonomous-app-0.1.8/src/autonomous/storage/cloudinarystorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      156 2023-06-13 18:11:43.000000 autonomous-app-0.1.8/src/autonomous/storage/localstorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1381 2023-06-13 18:12:16.000000 autonomous-app-0.1.8/src/autonomous/storage/s3storage.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.896062 autonomous-app-0.1.8/src/autonomous/tasks/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       34 2023-07-27 15:55:55.000000 autonomous-app-0.1.8/src/autonomous/tasks/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      615 2023-07-28 14:38:22.000000 autonomous-app-0.1.8/src/autonomous/tasks/task.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 17:38:23.898062 autonomous-app-0.1.8/src/autonomous_app.egg-info/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-08-02 17:38:23.000000 autonomous-app-0.1.8/src/autonomous_app.egg-info/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1788 2023-08-02 17:38:23.000000 autonomous-app-0.1.8/src/autonomous_app.egg-info/SOURCES.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-08-02 17:38:23.000000 autonomous-app-0.1.8/src/autonomous_app.egg-info/dependency_links.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       53 2023-08-02 17:38:23.000000 autonomous-app-0.1.8/src/autonomous_app.egg-info/entry_points.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)      162 2023-08-02 17:38:23.000000 autonomous-app-0.1.8/src/autonomous_app.egg-info/requires.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       11 2023-08-02 17:38:23.000000 autonomous-app-0.1.8/src/autonomous_app.egg-info/top_level.txt
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 18:26:28.270416 autonomous-app-0.1.9/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-03-07 12:36:40.000000 autonomous-app-0.1.9/LICENSE
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3810 2023-08-02 18:26:28.269416 autonomous-app-0.1.9/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2012 2023-08-02 17:40:38.000000 autonomous-app-0.1.9/README.md
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1469 2023-07-20 14:57:42.000000 autonomous-app-0.1.9/pyproject.toml
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      523 2023-07-27 14:43:37.000000 autonomous-app-0.1.9/requirements.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-08-02 18:26:28.270416 autonomous-app-0.1.9/setup.cfg
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-04-04 14:14:59.000000 autonomous-app-0.1.9/setup.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 18:26:28.261416 autonomous-app-0.1.9/src/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 18:26:28.263416 autonomous-app-0.1.9/src/autonomous/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       86 2023-08-02 18:26:11.000000 autonomous-app-0.1.9/src/autonomous/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 18:26:28.263416 autonomous-app-0.1.9/src/autonomous/apis/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       27 2023-06-20 19:34:19.000000 autonomous-app-0.1.9/src/autonomous/apis/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2149 2023-07-07 13:12:31.000000 autonomous-app-0.1.9/src/autonomous/apis/openai.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 18:26:28.264416 autonomous-app-0.1.9/src/autonomous/apis/version_control/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1069 2023-03-07 16:24:11.000000 autonomous-app-0.1.9/src/autonomous/apis/version_control/GHCallbacks.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1155 2023-03-07 21:09:26.000000 autonomous-app-0.1.9/src/autonomous/apis/version_control/GHOrganization.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     4622 2023-03-07 16:24:11.000000 autonomous-app-0.1.9/src/autonomous/apis/version_control/GHRepo.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      196 2023-03-07 16:24:11.000000 autonomous-app-0.1.9/src/autonomous/apis/version_control/GHVersionControl.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      117 2023-03-07 16:24:11.000000 autonomous-app-0.1.9/src/autonomous/apis/version_control/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 18:26:28.261416 autonomous-app-0.1.9/src/autonomous/app_template/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 18:26:28.264416 autonomous-app-0.1.9/src/autonomous/app_template/app/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       54 2023-07-28 15:13:30.000000 autonomous-app-0.1.9/src/autonomous/app_template/app/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1598 2023-07-27 16:48:05.000000 autonomous-app-0.1.9/src/autonomous/app_template/app/app.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1316 2023-07-27 17:51:13.000000 autonomous-app-0.1.9/src/autonomous/app_template/app/config.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 18:26:28.265416 autonomous-app-0.1.9/src/autonomous/app_template/app/models/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-04-04 14:32:12.000000 autonomous-app-0.1.9/src/autonomous/app_template/app/models/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      203 2023-04-04 15:41:08.000000 autonomous-app-0.1.9/src/autonomous/app_template/app/models/model.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      517 2023-07-28 15:15:34.000000 autonomous-app-0.1.9/src/autonomous/app_template/app/tasks.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 18:26:28.265416 autonomous-app-0.1.9/src/autonomous/app_template/app/views/
+-rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-04 14:32:12.000000 autonomous-app-0.1.9/src/autonomous/app_template/app/views/admin.py
+-rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-28 17:48:57.000000 autonomous-app-0.1.9/src/autonomous/app_template/app/views/index.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 18:26:28.265416 autonomous-app-0.1.9/src/autonomous/app_template/tests/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-04 14:32:12.000000 autonomous-app-0.1.9/src/autonomous/app_template/tests/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      545 2023-07-28 15:11:47.000000 autonomous-app-0.1.9/src/autonomous/app_template/tests/conftest.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      425 2023-08-02 18:25:53.000000 autonomous-app-0.1.9/src/autonomous/app_template/tests/test_app.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1021 2023-07-28 15:54:14.000000 autonomous-app-0.1.9/src/autonomous/app_template/tests/test_tasks.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 18:26:28.265416 autonomous-app-0.1.9/src/autonomous/app_template/vendor/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1124 2023-04-13 17:57:17.000000 autonomous-app-0.1.9/src/autonomous/app_template/vendor/gunicorn.conf.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2252 2023-06-08 19:19:57.000000 autonomous-app-0.1.9/src/autonomous/assets.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       42 2023-04-04 14:14:59.000000 autonomous-app-0.1.9/src/autonomous/cli.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 18:26:28.266416 autonomous-app-0.1.9/src/autonomous/db/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       94 2023-07-07 12:00:23.000000 autonomous-app-0.1.9/src/autonomous/db/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      812 2023-07-07 12:05:15.000000 autonomous-app-0.1.9/src/autonomous/db/autodb.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      531 2023-04-04 14:14:59.000000 autonomous-app-0.1.9/src/autonomous/db/storage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2521 2023-06-20 21:17:55.000000 autonomous-app-0.1.9/src/autonomous/db/table.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1245 2023-06-01 20:06:24.000000 autonomous-app-0.1.9/src/autonomous/logger.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 18:26:28.266416 autonomous-app-0.1.9/src/autonomous/model/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-02 18:01:05.000000 autonomous-app-0.1.9/src/autonomous/model/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     4226 2023-08-02 18:17:39.000000 autonomous-app-0.1.9/src/autonomous/model/automodel.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      687 2023-08-02 18:18:54.000000 autonomous-app-0.1.9/src/autonomous/model/orm.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 18:26:28.267416 autonomous-app-0.1.9/src/autonomous/storage/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       88 2023-06-13 18:11:53.000000 autonomous-app-0.1.9/src/autonomous/storage/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      447 2023-06-05 17:49:27.000000 autonomous-app-0.1.9/src/autonomous/storage/basestorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1620 2023-07-07 13:13:20.000000 autonomous-app-0.1.9/src/autonomous/storage/cloudinarystorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      156 2023-06-13 18:11:43.000000 autonomous-app-0.1.9/src/autonomous/storage/localstorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1381 2023-06-13 18:12:16.000000 autonomous-app-0.1.9/src/autonomous/storage/s3storage.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 18:26:28.267416 autonomous-app-0.1.9/src/autonomous/tasks/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       34 2023-07-27 15:55:55.000000 autonomous-app-0.1.9/src/autonomous/tasks/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      615 2023-07-28 14:38:22.000000 autonomous-app-0.1.9/src/autonomous/tasks/task.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-08-02 18:26:28.268416 autonomous-app-0.1.9/src/autonomous_app.egg-info/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3810 2023-08-02 18:26:28.000000 autonomous-app-0.1.9/src/autonomous_app.egg-info/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1788 2023-08-02 18:26:28.000000 autonomous-app-0.1.9/src/autonomous_app.egg-info/SOURCES.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-08-02 18:26:28.000000 autonomous-app-0.1.9/src/autonomous_app.egg-info/dependency_links.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       53 2023-08-02 18:26:28.000000 autonomous-app-0.1.9/src/autonomous_app.egg-info/entry_points.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      162 2023-08-02 18:26:28.000000 autonomous-app-0.1.9/src/autonomous_app.egg-info/requires.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       11 2023-08-02 18:26:28.000000 autonomous-app-0.1.9/src/autonomous_app.egg-info/top_level.txt
```

### Comparing `autonomous-app-0.1.8/LICENSE` & `autonomous-app-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/PKG-INFO` & `autonomous-app-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.1.8
+Version: 0.1.9
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,16 +34,16 @@
 
 # Autonomous
 
 :warning: :warning: :warning: WiP :warning: :warning: :warning:
 
 ![Tests](https://github.com/Sallenmoore/autonomous/actions/workflows/tests.yml/badge.svg)
 
-A local, containerized, service based application library built on top of Flask. 
-The goal is to make it easy to create self-contained Python applications with minimal dependencies and built in libraries for many different kinds of tasks.
+A local, containerized, service based application library built on top of Flask.
+The goal is to make it easy to create self-contained Python applications with minimal dependencies using built in libraries for many different kinds of tasks.
 
 - **[pypi](https://test.pypi.org/project/autonomous)**
 - **[github](https://github.com/Sallenmoore/autonomous)**
 
 ## Features
 
 - Fully containerized, service based Python application framework
```

### Comparing `autonomous-app-0.1.8/README.md` & `autonomous-app-0.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Autonomous
 
 :warning: :warning: :warning: WiP :warning: :warning: :warning:
 
 ![Tests](https://github.com/Sallenmoore/autonomous/actions/workflows/tests.yml/badge.svg)
 
-A local, containerized, service based application library built on top of Flask. 
-The goal is to make it easy to create self-contained Python applications with minimal dependencies and built in libraries for many different kinds of tasks.
+A local, containerized, service based application library built on top of Flask.
+The goal is to make it easy to create self-contained Python applications with minimal dependencies using built in libraries for many different kinds of tasks.
 
 - **[pypi](https://test.pypi.org/project/autonomous)**
 - **[github](https://github.com/Sallenmoore/autonomous)**
 
 ## Features
 
 - Fully containerized, service based Python application framework
```

### Comparing `autonomous-app-0.1.8/pyproject.toml` & `autonomous-app-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/requirements.txt` & `autonomous-app-0.1.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/apis/openai.py` & `autonomous-app-0.1.9/src/autonomous/apis/openai.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/apis/version_control/GHCallbacks.py` & `autonomous-app-0.1.9/src/autonomous/apis/version_control/GHCallbacks.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/apis/version_control/GHOrganization.py` & `autonomous-app-0.1.9/src/autonomous/apis/version_control/GHOrganization.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/apis/version_control/GHRepo.py` & `autonomous-app-0.1.9/src/autonomous/apis/version_control/GHRepo.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/app_template/app/app.py` & `autonomous-app-0.1.9/src/autonomous/app_template/app/app.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/app_template/app/config.py` & `autonomous-app-0.1.9/src/autonomous/app_template/app/config.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/app_template/app/tasks.py` & `autonomous-app-0.1.9/src/autonomous/app_template/app/tasks.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/app_template/app/views/admin.py` & `autonomous-app-0.1.9/src/autonomous/app_template/app/views/admin.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/app_template/app/views/index.py` & `autonomous-app-0.1.9/src/autonomous/app_template/app/views/index.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/app_template/tests/conftest.py` & `autonomous-app-0.1.9/src/autonomous/app_template/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/app_template/tests/test_tasks.py` & `autonomous-app-0.1.9/src/autonomous/app_template/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/app_template/vendor/gunicorn.conf.py` & `autonomous-app-0.1.9/src/autonomous/app_template/vendor/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/assets.py` & `autonomous-app-0.1.9/src/autonomous/assets.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/db/autodb.py` & `autonomous-app-0.1.9/src/autonomous/db/autodb.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/db/storage.py` & `autonomous-app-0.1.9/src/autonomous/db/storage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/db/table.py` & `autonomous-app-0.1.9/src/autonomous/db/table.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/logger.py` & `autonomous-app-0.1.9/src/autonomous/logger.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/model/automodel.py` & `autonomous-app-0.1.9/src/autonomous/model/automodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,30 +17,29 @@
     attributes = {}
 
     def __new__(cls, *args, **kwargs):
         obj = super().__new__(cls)
 
         # set default attributes
         cls.attributes["pk"] = None
-
+        log(f"Creating {cls.__name__}")
         obj.pk = kwargs.pop("pk", None)
         result = cls.table().get(obj.pk) or {}
         for k, v in cls.attributes.items():
             setattr(obj, k, result.get(k, v))
         obj.__dict__ |= kwargs
         # log(obj, kwargs)
         cls._deserialize(obj.__dict__)
         return obj
 
     @classmethod
     def table(cls):
         """The ORM table for this model"""
-
-        if not cls._table:
-            table_name = cls._table_name or cls.__name__
+        table_name = cls._table_name or cls.__name__
+        if not cls._table or cls._table.name != table_name:
             log(f"Creating table {table_name}")
             cls._table = cls._orm(table=table_name)
         return cls._table
 
     @classmethod
     def model_name(cls):
         """The fully qualified name of this model"""
```

### Comparing `autonomous-app-0.1.8/src/autonomous/model/orm.py` & `autonomous-app-0.1.9/src/autonomous/model/orm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ..db import db as _database
 
 
 class ORM:
     def __init__(self, table):
-        self._table_name = table
         self._table = _database.get_table(table=table)
+        self.name = self._table.name
 
     @property
     def table(self):
         return self._table
 
     def save(self, data):
         return self._table.save(data)
```

### Comparing `autonomous-app-0.1.8/src/autonomous/storage/cloudinarystorage.py` & `autonomous-app-0.1.9/src/autonomous/storage/cloudinarystorage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/storage/s3storage.py` & `autonomous-app-0.1.9/src/autonomous/storage/s3storage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous/tasks/task.py` & `autonomous-app-0.1.9/src/autonomous/tasks/task.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.8/src/autonomous_app.egg-info/PKG-INFO` & `autonomous-app-0.1.9/src/autonomous_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.1.8
+Version: 0.1.9
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,16 +34,16 @@
 
 # Autonomous
 
 :warning: :warning: :warning: WiP :warning: :warning: :warning:
 
 ![Tests](https://github.com/Sallenmoore/autonomous/actions/workflows/tests.yml/badge.svg)
 
-A local, containerized, service based application library built on top of Flask. 
-The goal is to make it easy to create self-contained Python applications with minimal dependencies and built in libraries for many different kinds of tasks.
+A local, containerized, service based application library built on top of Flask.
+The goal is to make it easy to create self-contained Python applications with minimal dependencies using built in libraries for many different kinds of tasks.
 
 - **[pypi](https://test.pypi.org/project/autonomous)**
 - **[github](https://github.com/Sallenmoore/autonomous)**
 
 ## Features
 
 - Fully containerized, service based Python application framework
```

### Comparing `autonomous-app-0.1.8/src/autonomous_app.egg-info/SOURCES.txt` & `autonomous-app-0.1.9/src/autonomous_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

