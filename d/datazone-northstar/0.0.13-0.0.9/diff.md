# Comparing `tmp/datazone_northstar-0.0.13.tar.gz` & `tmp/datazone_northstar-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datazone_northstar-0.0.13.tar", max compression
+gzip compressed data, was "datazone_northstar-0.0.9.tar", max compression
```

## Comparing `datazone_northstar-0.0.13.tar` & `datazone_northstar-0.0.9.tar`

### file list

```diff
@@ -1,93 +1,92 @@
--rw-r--r--   0        0        0     2602 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/README.md
--rw-r--r--   0        0        0      198 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/__init__.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/auth/__init__.py
--rw-r--r--   0        0        0      656 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/auth/configure.py
--rw-r--r--   0        0        0      183 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/auth/login.py
--rw-r--r--   0        0        0      173 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/auth/main.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/dataset/__init__.py
--rw-r--r--   0        0        0      625 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/dataset/list.py
--rw-r--r--   0        0        0      365 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/dataset/main.py
--rw-r--r--   0        0        0     1054 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/dataset/show.py
--rw-r--r--   0        0        0     1057 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/dataset/transactions.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/dataset/view/__init__.py
--rw-r--r--   0        0        0      478 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/dataset/view/create.py
--rw-r--r--   0        0        0      262 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/dataset/view/delete.py
--rw-r--r--   0        0        0      717 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/dataset/view/list.py
--rw-r--r--   0        0        0      272 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/dataset/view/main.py
--rw-r--r--   0        0        0     1195 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/datazone_typer.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/execution/__init__.py
--rw-r--r--   0        0        0     1075 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/execution/history.py
--rw-r--r--   0        0        0     1349 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/execution/list.py
--rw-r--r--   0        0        0     2705 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/execution/log.py
--rw-r--r--   0        0        0      319 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/execution/main.py
--rw-r--r--   0        0        0     1209 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/execution/run.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/extract/__init__.py
--rw-r--r--   0        0        0      905 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/extract/create.py
--rw-r--r--   0        0        0      270 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/extract/delete.py
--rw-r--r--   0        0        0      565 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/extract/execute.py
--rw-r--r--   0        0        0      736 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/extract/history.py
--rw-r--r--   0        0        0      972 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/extract/list.py
--rw-r--r--   0        0        0      401 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/extract/main.py
--rw-r--r--   0        0        0     1289 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/main.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/pipeline/__init__.py
--rw-r--r--   0        0        0      505 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/pipeline/create.py
--rw-r--r--   0        0        0      105 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/pipeline/main.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/repository/__init__.py
--rw-r--r--   0        0        0     1816 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/repository/clone.py
--rw-r--r--   0        0        0     1011 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/repository/create.py
--rw-r--r--   0        0        0     3008 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/repository/deploy.py
--rw-r--r--   0        0        0      576 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/repository/list.py
--rw-r--r--   0        0        0      476 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/repository/main.py
--rw-r--r--   0        0        0      366 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/repository/pull.py
--rw-r--r--   0        0        0     2078 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/repository/summary.py
--rw-r--r--   0        0        0     1091 2023-08-08 21:11:02.431957 datazone_northstar-0.0.13/datazone/cli/repository/template_loader.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/cli/repository/templates/__init__.py
--rw-r--r--   0        0        0      127 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/cli/repository/templates/config.yml.jinja
--rw-r--r--   0        0        0      585 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/cli/repository/templates/hello_world.py.jinja
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/cli/schedule/__init__.py
--rw-r--r--   0        0        0     1225 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/cli/schedule/create.py
--rw-r--r--   0        0        0      273 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/cli/schedule/delete.py
--rw-r--r--   0        0        0      908 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/cli/schedule/list.py
--rw-r--r--   0        0        0      260 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/cli/schedule/main.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/cli/source/__init__.py
--rw-r--r--   0        0        0     1374 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/cli/source/create.py
--rw-r--r--   0        0        0      270 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/cli/source/delete.py
--rw-r--r--   0        0        0     1110 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/cli/source/list.py
--rw-r--r--   0        0        0      322 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/cli/source/main.py
--rw-r--r--   0        0        0     1364 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/cli/source/update.py
--rw-r--r--   0        0        0      191 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/constants.py
--rw-r--r--   0        0        0      146 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/context.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/core/__init__.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/core/common/__init__.py
--rw-r--r--   0        0        0     1834 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/core/common/config.py
--rw-r--r--   0        0        0      225 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/core/common/types.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/core/connections/__init__.py
--rw-r--r--   0        0        0     1576 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/core/connections/auth.py
--rw-r--r--   0        0        0      723 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/core/connections/config.py
--rw-r--r--   0        0        0     1621 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/core/connections/session.py
--rw-r--r--   0        0        0      266 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/core/dataset.py
--rw-r--r--   0        0        0      301 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/core/mappings.py
--rw-r--r--   0        0        0     1157 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/core/transform.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/decorators/__init__.py
--rw-r--r--   0        0        0      896 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/decorators/transform.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/errors/__init__.py
--rw-r--r--   0        0        0      178 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/errors/auth.py
--rw-r--r--   0        0        0      297 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/errors/base.py
--rw-r--r--   0        0        0      329 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/errors/common.py
--rw-r--r--   0        0        0      300 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/errors/local_errors.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/models/__init__.py
--rw-r--r--   0        0        0      891 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/models/common.py
--rw-r--r--   0        0        0      339 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/models/config.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/service_callers/__init__.py
--rw-r--r--   0        0        0     1038 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/service_callers/base.py
--rw-r--r--   0        0        0     1366 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/service_callers/crud.py
--rw-r--r--   0        0        0     1093 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/service_callers/dataset.py
--rw-r--r--   0        0        0      130 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/service_callers/git.py
--rw-r--r--   0        0        0     2680 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/service_callers/job.py
--rw-r--r--   0        0        0     1590 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/service_callers/repository.py
--rw-r--r--   0        0        0        0 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/utils/__init__.py
--rw-r--r--   0        0        0      161 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/utils/helpers.py
--rw-r--r--   0        0        0      704 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/datazone/utils/types.py
--rw-r--r--   0        0        0      894 2023-08-08 21:11:02.435958 datazone_northstar-0.0.13/pyproject.toml
--rw-r--r--   0        0        0     3525 1970-01-01 00:00:00.000000 datazone_northstar-0.0.13/PKG-INFO
+-rw-r--r--   0        0        0     2627 2023-07-19 19:57:28.284121 datazone_northstar-0.0.9/README.md
+-rw-r--r--   0        0        0      198 2023-06-02 16:42:34.660341 datazone_northstar-0.0.9/datazone/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 16:42:34.660432 datazone_northstar-0.0.9/datazone/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:31:23.609293 datazone_northstar-0.0.9/datazone/cli/auth/__init__.py
+-rw-r--r--   0        0        0      656 2023-06-08 13:41:10.817807 datazone_northstar-0.0.9/datazone/cli/auth/configure.py
+-rw-r--r--   0        0        0      183 2023-06-06 11:31:23.609736 datazone_northstar-0.0.9/datazone/cli/auth/login.py
+-rw-r--r--   0        0        0      173 2023-06-06 11:31:23.609872 datazone_northstar-0.0.9/datazone/cli/auth/main.py
+-rw-r--r--   0        0        0        0 2023-06-02 16:42:34.660841 datazone_northstar-0.0.9/datazone/cli/dataset/__init__.py
+-rw-r--r--   0        0        0      625 2023-06-09 09:33:00.099863 datazone_northstar-0.0.9/datazone/cli/dataset/list.py
+-rw-r--r--   0        0        0      365 2023-06-09 09:33:33.752868 datazone_northstar-0.0.9/datazone/cli/dataset/main.py
+-rw-r--r--   0        0        0     1054 2023-06-06 11:31:23.610313 datazone_northstar-0.0.9/datazone/cli/dataset/show.py
+-rw-r--r--   0        0        0     1057 2023-06-06 11:31:23.610719 datazone_northstar-0.0.9/datazone/cli/dataset/transactions.py
+-rw-r--r--   0        0        0        0 2023-06-02 16:42:34.661955 datazone_northstar-0.0.9/datazone/cli/dataset/view/__init__.py
+-rw-r--r--   0        0        0      478 2023-06-06 15:48:42.191818 datazone_northstar-0.0.9/datazone/cli/dataset/view/create.py
+-rw-r--r--   0        0        0      262 2023-06-07 11:17:25.898686 datazone_northstar-0.0.9/datazone/cli/dataset/view/delete.py
+-rw-r--r--   0        0        0      717 2023-06-06 15:52:11.454584 datazone_northstar-0.0.9/datazone/cli/dataset/view/list.py
+-rw-r--r--   0        0        0      272 2023-06-06 15:43:54.644730 datazone_northstar-0.0.9/datazone/cli/dataset/view/main.py
+-rw-r--r--   0        0        0        0 2023-06-02 16:42:34.661465 datazone_northstar-0.0.9/datazone/cli/execution/__init__.py
+-rw-r--r--   0        0        0     1075 2023-06-29 07:21:02.520894 datazone_northstar-0.0.9/datazone/cli/execution/history.py
+-rw-r--r--   0        0        0     1310 2023-07-19 14:58:14.677185 datazone_northstar-0.0.9/datazone/cli/execution/list.py
+-rw-r--r--   0        0        0     1994 2023-06-30 15:12:24.461918 datazone_northstar-0.0.9/datazone/cli/execution/log.py
+-rw-r--r--   0        0        0      319 2023-07-19 09:31:15.969544 datazone_northstar-0.0.9/datazone/cli/execution/main.py
+-rw-r--r--   0        0        0     1313 2023-07-19 14:55:47.768408 datazone_northstar-0.0.9/datazone/cli/execution/run.py
+-rw-r--r--   0        0        0        0 2023-06-02 16:42:34.661955 datazone_northstar-0.0.9/datazone/cli/extract/__init__.py
+-rw-r--r--   0        0        0      905 2023-06-21 12:47:12.942518 datazone_northstar-0.0.9/datazone/cli/extract/create.py
+-rw-r--r--   0        0        0      270 2023-06-06 11:31:23.612324 datazone_northstar-0.0.9/datazone/cli/extract/delete.py
+-rw-r--r--   0        0        0      565 2023-06-30 15:12:33.228953 datazone_northstar-0.0.9/datazone/cli/extract/execute.py
+-rw-r--r--   0        0        0      736 2023-06-29 07:22:13.936753 datazone_northstar-0.0.9/datazone/cli/extract/history.py
+-rw-r--r--   0        0        0      972 2023-06-25 21:17:38.481333 datazone_northstar-0.0.9/datazone/cli/extract/list.py
+-rw-r--r--   0        0        0      401 2023-06-29 07:24:12.316650 datazone_northstar-0.0.9/datazone/cli/extract/main.py
+-rw-r--r--   0        0        0     1245 2023-07-19 15:21:44.129433 datazone_northstar-0.0.9/datazone/cli/main.py
+-rw-r--r--   0        0        0        0 2023-06-02 16:42:34.661955 datazone_northstar-0.0.9/datazone/cli/pipeline/__init__.py
+-rw-r--r--   0        0        0      504 2023-07-19 15:36:18.780297 datazone_northstar-0.0.9/datazone/cli/pipeline/create.py
+-rw-r--r--   0        0        0      105 2023-07-19 15:04:59.907951 datazone_northstar-0.0.9/datazone/cli/pipeline/main.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:31:23.613566 datazone_northstar-0.0.9/datazone/cli/repository/__init__.py
+-rw-r--r--   0        0        0     1816 2023-07-19 12:45:33.067052 datazone_northstar-0.0.9/datazone/cli/repository/clone.py
+-rw-r--r--   0        0        0      819 2023-06-06 11:31:23.613714 datazone_northstar-0.0.9/datazone/cli/repository/create.py
+-rw-r--r--   0        0        0     2992 2023-06-28 21:13:37.090348 datazone_northstar-0.0.9/datazone/cli/repository/deploy.py
+-rw-r--r--   0        0        0      516 2023-07-19 12:16:54.212103 datazone_northstar-0.0.9/datazone/cli/repository/list.py
+-rw-r--r--   0        0        0      476 2023-07-19 12:42:05.956699 datazone_northstar-0.0.9/datazone/cli/repository/main.py
+-rw-r--r--   0        0        0      467 2023-07-19 12:46:15.175233 datazone_northstar-0.0.9/datazone/cli/repository/pull.py
+-rw-r--r--   0        0        0     1744 2023-06-06 14:21:01.400705 datazone_northstar-0.0.9/datazone/cli/repository/summary.py
+-rw-r--r--   0        0        0     1118 2023-06-09 07:19:45.445314 datazone_northstar-0.0.9/datazone/cli/repository/template_loader.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:31:23.614366 datazone_northstar-0.0.9/datazone/cli/repository/templates/__init__.py
+-rw-r--r--   0        0        0      139 2023-06-08 14:02:47.486458 datazone_northstar-0.0.9/datazone/cli/repository/templates/config.yml.jinja
+-rw-r--r--   0        0        0      585 2023-06-06 11:31:23.614625 datazone_northstar-0.0.9/datazone/cli/repository/templates/hello_world.py.jinja
+-rw-r--r--   0        0        0        0 2023-06-02 16:42:34.663393 datazone_northstar-0.0.9/datazone/cli/schedule/__init__.py
+-rw-r--r--   0        0        0     1225 2023-06-29 05:59:43.732507 datazone_northstar-0.0.9/datazone/cli/schedule/create.py
+-rw-r--r--   0        0        0      273 2023-06-06 11:31:23.615534 datazone_northstar-0.0.9/datazone/cli/schedule/delete.py
+-rw-r--r--   0        0        0      908 2023-06-19 11:16:37.955941 datazone_northstar-0.0.9/datazone/cli/schedule/list.py
+-rw-r--r--   0        0        0      260 2023-06-02 16:42:34.663747 datazone_northstar-0.0.9/datazone/cli/schedule/main.py
+-rw-r--r--   0        0        0        0 2023-06-02 16:42:34.663833 datazone_northstar-0.0.9/datazone/cli/source/__init__.py
+-rw-r--r--   0        0        0     1374 2023-07-11 13:44:43.212250 datazone_northstar-0.0.9/datazone/cli/source/create.py
+-rw-r--r--   0        0        0      270 2023-06-06 11:31:23.616295 datazone_northstar-0.0.9/datazone/cli/source/delete.py
+-rw-r--r--   0        0        0     1067 2023-07-11 13:46:06.569382 datazone_northstar-0.0.9/datazone/cli/source/list.py
+-rw-r--r--   0        0        0      322 2023-06-02 16:42:34.664227 datazone_northstar-0.0.9/datazone/cli/source/main.py
+-rw-r--r--   0        0        0     1364 2023-07-11 13:46:56.980176 datazone_northstar-0.0.9/datazone/cli/source/update.py
+-rw-r--r--   0        0        0      415 2023-07-05 10:34:40.628169 datazone_northstar-0.0.9/datazone/constants.py
+-rw-r--r--   0        0        0      146 2023-06-02 16:42:34.664755 datazone_northstar-0.0.9/datazone/context.py
+-rw-r--r--   0        0        0        0 2023-06-02 16:42:34.664850 datazone_northstar-0.0.9/datazone/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:31:23.617067 datazone_northstar-0.0.9/datazone/core/common/__init__.py
+-rw-r--r--   0        0        0     1834 2023-07-19 15:43:20.764260 datazone_northstar-0.0.9/datazone/core/common/config.py
+-rw-r--r--   0        0        0      225 2023-06-21 12:44:26.642351 datazone_northstar-0.0.9/datazone/core/common/types.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:31:23.617343 datazone_northstar-0.0.9/datazone/core/connections/__init__.py
+-rw-r--r--   0        0        0     1576 2023-06-25 21:12:14.148670 datazone_northstar-0.0.9/datazone/core/connections/auth.py
+-rw-r--r--   0        0        0      723 2023-06-06 11:31:23.617632 datazone_northstar-0.0.9/datazone/core/connections/config.py
+-rw-r--r--   0        0        0     1109 2023-07-19 10:36:29.345527 datazone_northstar-0.0.9/datazone/core/connections/session.py
+-rw-r--r--   0        0        0      266 2023-06-14 11:22:43.102876 datazone_northstar-0.0.9/datazone/core/dataset.py
+-rw-r--r--   0        0        0      301 2023-06-02 16:42:34.665080 datazone_northstar-0.0.9/datazone/core/mappings.py
+-rw-r--r--   0        0        0     1157 2023-06-02 16:42:34.665182 datazone_northstar-0.0.9/datazone/core/transform.py
+-rw-r--r--   0        0        0        0 2023-06-02 16:42:34.665272 datazone_northstar-0.0.9/datazone/decorators/__init__.py
+-rw-r--r--   0        0        0      896 2023-06-02 16:42:34.665409 datazone_northstar-0.0.9/datazone/decorators/transform.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:31:23.618028 datazone_northstar-0.0.9/datazone/errors/__init__.py
+-rw-r--r--   0        0        0      178 2023-06-06 11:31:23.618165 datazone_northstar-0.0.9/datazone/errors/auth.py
+-rw-r--r--   0        0        0       63 2023-06-02 16:42:34.665567 datazone_northstar-0.0.9/datazone/errors/base.py
+-rw-r--r--   0        0        0      241 2023-07-19 10:35:52.993609 datazone_northstar-0.0.9/datazone/errors/common.py
+-rw-r--r--   0        0        0      300 2023-06-09 12:48:01.899123 datazone_northstar-0.0.9/datazone/errors/local_errors.py
+-rw-r--r--   0        0        0        0 2023-06-02 16:42:34.665835 datazone_northstar-0.0.9/datazone/models/__init__.py
+-rw-r--r--   0        0        0      229 2023-06-06 11:31:23.618308 datazone_northstar-0.0.9/datazone/models/common.py
+-rw-r--r--   0        0        0      355 2023-07-19 15:36:47.213444 datazone_northstar-0.0.9/datazone/models/config.py
+-rw-r--r--   0        0        0      187 2023-07-18 19:59:54.555183 datazone_northstar-0.0.9/datazone/run.py
+-rw-r--r--   0        0        0        0 2023-06-02 16:42:34.666072 datazone_northstar-0.0.9/datazone/service_callers/__init__.py
+-rw-r--r--   0        0        0     1038 2023-06-06 11:31:23.618462 datazone_northstar-0.0.9/datazone/service_callers/base.py
+-rw-r--r--   0        0        0     1366 2023-07-19 09:28:15.689660 datazone_northstar-0.0.9/datazone/service_callers/crud.py
+-rw-r--r--   0        0        0     1093 2023-06-06 15:50:26.222019 datazone_northstar-0.0.9/datazone/service_callers/dataset.py
+-rw-r--r--   0        0        0      130 2023-06-06 12:07:05.921944 datazone_northstar-0.0.9/datazone/service_callers/git.py
+-rw-r--r--   0        0        0     2964 2023-06-30 15:13:18.248286 datazone_northstar-0.0.9/datazone/service_callers/job.py
+-rw-r--r--   0        0        0     1590 2023-06-06 11:31:23.619557 datazone_northstar-0.0.9/datazone/service_callers/repository.py
+-rw-r--r--   0        0        0        0 2023-06-09 08:57:31.544521 datazone_northstar-0.0.9/datazone/utils/__init__.py
+-rw-r--r--   0        0        0      704 2023-06-09 09:21:00.888518 datazone_northstar-0.0.9/datazone/utils/types.py
+-rw-r--r--   0        0        0      893 2023-07-19 19:57:12.371877 datazone_northstar-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 datazone_northstar-0.0.9/PKG-INFO
```

### Comparing `datazone_northstar-0.0.13/README.md` & `datazone_northstar-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-Datazone Northstar Client Library 👋
+# northstar-package-datazone
+Datazone Northstar Client Library
 
 ## Installation
 You can install package via pip
 ````shell
 pip install datazone-northstar
 ````
 
@@ -39,15 +40,15 @@
 
 After the deployment is complete, you can check your repository status via following command.
 
 ```shell
 datazone repository summary
 ```
 
-If repository has deployed, you can run your first execution with following command.
+If repository has deployed, you can run your first execution with following command. 
 ````shell
 datazone execution run <pipeline_id>
 ````
 
 ## Commands
 Also you can check all command with help sub command. `datazone auth --help` or `datazone repository summary --help`
 ```shell
```

### Comparing `datazone_northstar-0.0.13/datazone/cli/auth/configure.py` & `datazone_northstar-0.0.9/datazone/cli/auth/configure.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/cli/dataset/list.py` & `datazone_northstar-0.0.9/datazone/cli/dataset/list.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/cli/dataset/show.py` & `datazone_northstar-0.0.9/datazone/cli/dataset/show.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/cli/dataset/transactions.py` & `datazone_northstar-0.0.9/datazone/cli/dataset/transactions.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/cli/dataset/view/list.py` & `datazone_northstar-0.0.9/datazone/cli/dataset/view/list.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/cli/execution/history.py` & `datazone_northstar-0.0.9/datazone/cli/execution/history.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/cli/execution/list.py` & `datazone_northstar-0.0.9/datazone/cli/execution/list.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,15 @@
 from typing import Optional
 
 from rich.console import Console
 from rich.table import Table
 
 from datazone.service_callers.crud import CrudServiceCaller
 
-history_columns = [
-    "ID",
-    "Entity Type",
-    "Entity ID",
-    "Created At",
-    "Started At",
-    "Finished At",
-    "Created By",
-    "Run ID",
-    "Status",
-]
+history_columns = ["ID", "Entity Type", "Entity ID", "Created At", "Started At", "Finished At", "Created By", "Run ID", "Status"]
 
 
 def list_func(pipeline_id: Optional[str] = None, extract_id: Optional[str] = None) -> None:
     params = {}
     if pipeline_id is not None:
         params.update({"pipeline_id": pipeline_id})
     elif extract_id is not None:
```

### Comparing `datazone_northstar-0.0.13/datazone/cli/execution/run.py` & `datazone_northstar-0.0.9/datazone/cli/execution/run.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Optional
 
 from rich import print
 
+from datazone.core.common.config import ConfigReader
 from datazone.cli.execution.log import log
+from datazone.models.common import ExecutionTypes
 from datazone.service_callers.job import JobServiceCaller
 
 
 def run(
     extract_id: Optional[str] = None,
     pipeline_id: Optional[str] = None,
     transform_selection: Optional[str] = None,
@@ -15,15 +17,15 @@
     Start execution.
     Args:
         extract_id: Extract id
         pipeline_id: Pipeline id
         transform_selection (str): specific transform name to run
     """
     if not any([extract_id, pipeline_id]):
-        print("[bold red]You should pass extract id or pipeline id![/bold red]")
+        print(f"[bold red]You should pass extract id or pipeline id![/bold red]")
         return
 
     if extract_id is not None:
         response_data = JobServiceCaller.run_execution_extract(extract_id=extract_id)
     else:
         response_data = JobServiceCaller.run_execution_pipeline(
             pipeline_id=pipeline_id,
@@ -32,10 +34,10 @@
 
     _id = response_data.get("_id")
     if _id is None:
         error_message = response_data.get("message", "Run execution error!")
         print(f"[bold red]{error_message}[/bold red]")
         return
 
-    print("[bold blue]Execution has created... :tada: [/bold blue]")
+    print("[bold blue]Execution has started... :tada: [/bold blue]")
 
     log(execution_id=_id)
```

### Comparing `datazone_northstar-0.0.13/datazone/cli/extract/create.py` & `datazone_northstar-0.0.9/datazone/cli/extract/create.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/cli/extract/execute.py` & `datazone_northstar-0.0.9/datazone/cli/extract/execute.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/cli/extract/history.py` & `datazone_northstar-0.0.9/datazone/cli/extract/history.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/cli/extract/list.py` & `datazone_northstar-0.0.9/datazone/cli/extract/list.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/cli/main.py` & `datazone_northstar-0.0.9/datazone/cli/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from rich import print
-from datazone.cli.datazone_typer import DatazoneTyper
+import typer
 
 from datazone.cli.execution.main import app as execution_app
 from datazone.cli.dataset.main import app as dataset_app
 from datazone.cli.source.main import app as source_app
 from datazone.cli.extract.main import app as extract_app
 from datazone.cli.schedule.main import app as schedule_app
 from datazone.cli.repository.main import app as repository_app
 from datazone.cli.pipeline.main import app as pipeline_app
 from datazone.cli.auth.main import app as auth_app
 from datazone.core.connections.config import ConnectionConfig
 
-app = DatazoneTyper()
+app = typer.Typer()
 app.add_typer(execution_app, name="execution")
 app.add_typer(dataset_app, name="dataset")
 app.add_typer(source_app, name="source")
 app.add_typer(extract_app, name="extract")
 app.add_typer(schedule_app, name="schedule")
 app.add_typer(repository_app, name="repository")
 app.add_typer(pipeline_app, name="pipeline")
 app.add_typer(auth_app, name="auth")
 
 
 @app.command()
 def version():
     import pkg_resources
 
-    my_version = pkg_resources.get_distribution("datazone-northstar").version
+    my_version = pkg_resources.get_distribution("northstar-datazone").version
 
     print(f"Current version: {my_version}")
 
 
 @app.command()
 def info():
     config = ConnectionConfig()
     print(f"User: {config.username}")
-    print(f"Host: {config.host}")
+    print(f"Host: {config.host}")
```

### Comparing `datazone_northstar-0.0.13/datazone/cli/repository/clone.py` & `datazone_northstar-0.0.9/datazone/cli/repository/clone.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/cli/repository/create.py` & `datazone_northstar-0.0.9/datazone/cli/repository/create.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import shutil
 from pathlib import Path
 
 import typer
 
 from datazone.cli.repository.template_loader import load_template_files
-from datazone.service_callers.crud import CrudServiceCaller
 
 
 def create(repository_name: str) -> None:
     """
     Create new repository. If project with the same name exists, it will be truncated.
     Args:
         repository_name: name of the project
@@ -21,16 +20,12 @@
         )
         if not delete:
             return
 
         shutil.rmtree(path)
 
     os.mkdir(repository_name)
-
-    project = CrudServiceCaller(service_name="job", entity_name="project").create_entity(
-        payload={"name": repository_name},
-    )
-    contents = load_template_files(project)
+    contents = load_template_files(repository_name)
 
     for file_name, file_content in contents:
         with open(f"{repository_name}/{file_name}", "w") as f:
             f.write(file_content)
```

### Comparing `datazone_northstar-0.0.13/datazone/cli/repository/deploy.py` & `datazone_northstar-0.0.9/datazone/cli/repository/deploy.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,19 +3,26 @@
 from typing import Optional
 
 import git
 from rich import print
 
 from datazone.core.common.config import ConfigReader
 from datazone.models.config import Config
-from datazone.service_callers.crud import CrudServiceCaller
 from datazone.service_callers.git import GitServiceCaller
 from datazone.service_callers.job import JobServiceCaller
 from datazone.service_callers.repository import RepositoryServiceCaller
-from datazone.utils.helpers import is_git_repo
+
+
+def is_git_repo():
+    try:
+        _ = git.Repo()
+    except git.exc.InvalidGitRepositoryError:
+        return False
+    else:
+        return True
 
 
 def fetch_git_repo(repo_name: str, commit_message: Optional[str] = None) -> None:
     """
     Fetch git repository from the repository service.
     It uses the default server and default organisation. It creates a session with the given repository name.
     Also, it uses GitPython to fetch the repository and perform git operations.
@@ -69,22 +76,21 @@
     config_file = ConfigReader(file)
 
     if not config_file.is_config_file_exist():
         print("[bold red]Config file does not exist![/bold red]")
         return
 
     config: Config = config_file.read_config_file()
-    project = CrudServiceCaller(service_name="job", entity_name="project").get_entity_with_id(
-        entity_id=str(config.project_id),
-    )
     for pipeline in config.pipelines:
         pipeline_file = pipeline.path
         if not os.path.exists(pipeline_file):
             print(f"[bold red]Pipeline file {pipeline_file} does not exist![/bold red]")
             return
 
     print("[bold green]Deploying...[/bold green]")
 
-    repository_name = project.get("repository_name")
-    fetch_git_repo(repository_name, commit_message)
+    repository_id = str(config.repository_id)
+    if not is_git_repo():
+        RepositoryServiceCaller.create_repository(name=repository_id)
+    fetch_git_repo(repository_id, commit_message)
 
-    JobServiceCaller.inspect_project(project_id=str(config.project_id))
+    JobServiceCaller.inspect_repository(repository_id=repository_id)
```

### Comparing `datazone_northstar-0.0.13/datazone/cli/repository/list.py` & `datazone_northstar-0.0.9/datazone/cli/repository/list.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from rich.console import Console
 from rich.table import Table
 
 from datazone.service_callers.crud import CrudServiceCaller
 
-schedule_columns = ["ID", "Name", "Draft"]
+schedule_columns = ["ID", "Name"]
 
 
 def list_func():
     response_data = CrudServiceCaller(service_name="job", entity_name="project").get_entity_list()
     console = Console()
 
     table = Table(*schedule_columns)
     for datum in response_data:
         values = [
             datum.get("_id"),
             datum.get("name"),
-            "Y" if datum.get("is_draft") else "N",
         ]
         table.add_row(*values)
     console.print(table)
```

### Comparing `datazone_northstar-0.0.13/datazone/cli/repository/summary.py` & `datazone_northstar-0.0.9/datazone/cli/repository/summary.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from typing import Optional
-
-import typer
 from rich import print
 from rich.console import Console
 from rich.table import Table
 
 from datazone.core.common.config import ConfigReader
 from datazone.models.config import Config
 from datazone.service_callers.job import JobServiceCaller
@@ -17,36 +14,28 @@
     "Function Name",
     "Output Name",
     "Materialized",
     "Dataset ID",
 ]
 
 
-def get_repository_id_from_config_file() -> Optional[str]:
-    """It reads config yaml file in current directory and returns."""
+def summary() -> None:
+    """
+    Get summary about project
+    """
     config_file = ConfigReader()
 
     if not config_file.is_config_file_exist():
         print("[bold red]Config file does not exist![/bold red]")
-        raise typer.Exit(code=1)
+        return
 
     config: Config = config_file.read_config_file()
 
-    repository_id = str(config.project_id)
-    return repository_id
-
-
-def summary(repository_id: Optional[str] = None) -> None:
-    """
-    Get summary about project
-    """
-    if repository_id is None:
-        repository_id = get_repository_id_from_config_file()
-
-    response_data = JobServiceCaller.get_project_summary(project_id=repository_id)
+    repository_id = str(config.repository_id)
+    response_data = JobServiceCaller.get_repository_summary(repository_id=repository_id)
 
     pipelines = response_data["pipelines"]
 
     rows = []
     for pipeline in pipelines:
         transforms = pipeline.get("transforms")
         for transform in transforms:
```

### Comparing `datazone_northstar-0.0.13/datazone/cli/repository/template_loader.py` & `datazone_northstar-0.0.9/datazone/cli/repository/template_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+import uuid
 from pathlib import Path
-from typing import List, Dict
+from typing import List
 
 from bson import ObjectId
 from jinja2 import Environment, FileSystemLoader
 
 template_path = Path(__file__).parent / "templates"
 
 
-def load_template_files(project: Dict) -> List[tuple[str, str]]:
+def load_template_files(repository_name: str) -> List[tuple[str, str]]:
     """
     Load template files from the templates folder and render them.
     Args:
-        project: project data
+        repository_name: name of the repository
     Returns:
         List[tuple[str, str]]: List of tuples with file name and file content.
     """
     loader = FileSystemLoader(template_path)
     env = Environment(loader=loader)
     files: List[tuple[str, str]] = []
 
     pipeline_template = env.get_template("hello_world.py.jinja")
     rendered_pipeline_template = pipeline_template.render()
     files.append(("first_pipeline.py", rendered_pipeline_template))
 
     config_template = env.get_template("config.yml.jinja")
     rendered_config_template = config_template.render(
-        project_id=project.get("_id"),
-        project_name=project.get("name"),
+        repository_id=uuid.uuid4(),
+        repository_name=repository_name,
         pipeline_id=ObjectId(),
     )
     files.append(("config.yml", rendered_config_template))
 
     return files
```

### Comparing `datazone_northstar-0.0.13/datazone/cli/repository/templates/hello_world.py.jinja` & `datazone_northstar-0.0.9/datazone/cli/repository/templates/hello_world.py.jinja`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/cli/schedule/create.py` & `datazone_northstar-0.0.9/datazone/cli/schedule/create.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/cli/schedule/list.py` & `datazone_northstar-0.0.9/datazone/cli/schedule/list.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/cli/source/create.py` & `datazone_northstar-0.0.9/datazone/cli/source/create.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/cli/source/list.py` & `datazone_northstar-0.0.9/datazone/cli/source/list.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,13 @@
 from rich.console import Console
 from rich.table import Table
 
 from datazone.service_callers.crud import CrudServiceCaller
 
-source_columns = [
-    "ID",
-    "Name",
-    "Host",
-    "Port",
-    "User",
-    "Type",
-    "Database Name",
-    "Schema Name",
-    "Created At",
-    "Created By",
-]
+source_columns = ["ID", "Name", "Host", "Port", "User", "Type", "Database Name", "Schema Name", "Created At", "Created By"]
 
 
 def list_func():
     response_data = CrudServiceCaller(service_name="dataset", entity_name="source").get_entity_list()
 
     console = Console()
```

### Comparing `datazone_northstar-0.0.13/datazone/cli/source/update.py` & `datazone_northstar-0.0.9/datazone/cli/source/update.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/core/common/config.py` & `datazone_northstar-0.0.9/datazone/core/common/config.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/core/connections/auth.py` & `datazone_northstar-0.0.9/datazone/core/connections/auth.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/core/connections/config.py` & `datazone_northstar-0.0.9/datazone/core/connections/config.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/core/transform.py` & `datazone_northstar-0.0.9/datazone/core/transform.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/decorators/transform.py` & `datazone_northstar-0.0.9/datazone/decorators/transform.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/service_callers/base.py` & `datazone_northstar-0.0.9/datazone/service_callers/base.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/service_callers/crud.py` & `datazone_northstar-0.0.9/datazone/service_callers/crud.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/service_callers/dataset.py` & `datazone_northstar-0.0.9/datazone/service_callers/dataset.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/service_callers/job.py` & `datazone_northstar-0.0.9/datazone/service_callers/job.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional, Dict
 
+from datazone.models.common import ExecutionTypes
 from datazone.service_callers.base import BaseServiceCaller
 
 
 class JobServiceCaller(BaseServiceCaller):
     service_name = "job"
 
     @classmethod
@@ -36,39 +37,45 @@
         return response.json()
 
     @classmethod
     def run_execution_pipeline(
         cls,
         pipeline_id: str,
         transform_selection: Optional[str],
+        execution_type: Optional[ExecutionTypes] = None,
     ):
         body = {}
-        if transform_selection is not None:
-            body.update({"transform_selection": transform_selection})
+        if transform_selection is not None and execution_type is not None:
+            body.update(
+                {
+                    "transform_selection": transform_selection,
+                    "execution_type": execution_type,
+                },
+            )
 
         session = cls.get_session()
         response = session.post(
             f"{cls.get_service_url()}/execution/pipeline/{pipeline_id}",
             json=body,
         )
         return response.json()
 
     @classmethod
-    def inspect_project(cls, project_id: str):
+    def inspect_repository(cls, repository_id: str):
         session = cls.get_session()
         response = session.get(
-            f"{cls.get_service_url()}/project/inspect/{project_id}",
+            f"{cls.get_service_url()}/inspect/repository/{repository_id}",
         )
         return response.json()
 
     @classmethod
-    def get_project_summary(cls, project_id: str):
+    def get_repository_summary(cls, repository_id: str):
         session = cls.get_session()
         response = session.get(
-            f"{cls.get_service_url()}/project/summary/{project_id}",
+            f"{cls.get_service_url()}/pipeline/summary/{repository_id}",
         )
         return response.json()
 
     @classmethod
     def run_execution_extract(cls, extract_id: str):
         session = cls.get_session()
         response = session.post(f"{cls.get_service_url()}/execution/extract/{extract_id}")
```

### Comparing `datazone_northstar-0.0.13/datazone/service_callers/repository.py` & `datazone_northstar-0.0.9/datazone/service_callers/repository.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/datazone/utils/types.py` & `datazone_northstar-0.0.9/datazone/utils/types.py`

 * *Files identical despite different names*

### Comparing `datazone_northstar-0.0.13/pyproject.toml` & `datazone_northstar-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datazone-northstar"
-version = "0.0.13"
+version = "0.0.9"
 description = "Datazone Northstar Client Package"
 authors = ["resulyurttakalan <resul@datazone.co>"]
 readme = "README.md"
 packages = [{ include = "datazone" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `datazone_northstar-0.0.13/PKG-INFO` & `datazone_northstar-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datazone-northstar
-Version: 0.0.13
+Version: 0.0.9
 Summary: Datazone Northstar Client Package
 Author: resulyurttakalan
 Author-email: resul@datazone.co
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,15 +19,16 @@
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: pyspark (>=3.3.2,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests-oauthlib (>=1.3.1,<2.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
-Datazone Northstar Client Library 👋
+# northstar-package-datazone
+Datazone Northstar Client Library
 
 ## Installation
 You can install package via pip
 ````shell
 pip install datazone-northstar
 ````
 
@@ -64,15 +65,15 @@
 
 After the deployment is complete, you can check your repository status via following command.
 
 ```shell
 datazone repository summary
 ```
 
-If repository has deployed, you can run your first execution with following command.
+If repository has deployed, you can run your first execution with following command. 
 ````shell
 datazone execution run <pipeline_id>
 ````
 
 ## Commands
 Also you can check all command with help sub command. `datazone auth --help` or `datazone repository summary --help`
 ```shell
```

