# Comparing `tmp/e2b-0.1.2.tar.gz` & `tmp/e2b-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2b-0.1.2.tar", max compression
+gzip compressed data, was "e2b-0.1.3.tar", max compression
```

## Comparing `e2b-0.1.2.tar` & `e2b-0.1.3.tar`

### file list

```diff
@@ -1,65 +1,66 @@
--rw-r--r--   0        0        0     2876 2023-08-07 00:59:38.602804 e2b-0.1.2/README.md
--rw-r--r--   0        0        0      322 2023-08-07 00:43:25.922405 e2b-0.1.2/e2b/__init__.py
--rw-r--r--   0        0        0     1608 2023-08-07 00:43:25.922993 e2b-0.1.2/e2b/api/.openapi-generator/FILES
--rw-r--r--   0        0        0        5 2023-08-07 00:43:25.923180 e2b-0.1.2/e2b/api/.openapi-generator/VERSION
--rw-r--r--   0        0        0     1040 2023-08-07 00:43:25.922714 e2b-0.1.2/e2b/api/.openapi-generator-ignore
--rw-r--r--   0        0        0        0 2023-08-07 00:43:25.923217 e2b-0.1.2/e2b/api/__init__.py
--rw-r--r--   0        0        0     1723 2023-08-07 00:43:25.923543 e2b-0.1.2/e2b/api/client/__init__.py
--rw-r--r--   0        0        0      205 2023-08-07 00:43:25.923792 e2b-0.1.2/e2b/api/client/api/__init__.py
--rw-r--r--   0        0        0     6652 2023-08-07 00:43:25.923953 e2b-0.1.2/e2b/api/client/api/default_api.py
--rw-r--r--   0        0        0    52514 2023-08-07 00:43:25.924274 e2b-0.1.2/e2b/api/client/api/envs_api.py
--rw-r--r--   0        0        0    28662 2023-08-07 00:43:25.924476 e2b-0.1.2/e2b/api/client/api/sessions_api.py
--rw-r--r--   0        0        0    28991 2023-08-07 00:43:25.924795 e2b-0.1.2/e2b/api/client/api_client.py
--rw-r--r--   0        0        0      805 2023-08-07 00:43:25.925073 e2b-0.1.2/e2b/api/client/api_response.py
--rw-r--r--   0        0        0    16423 2023-08-07 00:43:25.925346 e2b-0.1.2/e2b/api/client/configuration.py
--rw-r--r--   0        0        0     1650 2023-08-07 00:43:25.925814 e2b-0.1.2/e2b/api/client/docs/DefaultApi.md
--rw-r--r--   0        0        0    14912 2023-08-07 00:43:25.926025 e2b-0.1.2/e2b/api/client/docs/EnvsApi.md
--rw-r--r--   0        0        0     8210 2023-08-07 00:43:25.926175 e2b-0.1.2/e2b/api/client/docs/SessionsApi.md
--rw-r--r--   0        0        0     5000 2023-08-07 00:43:25.926379 e2b-0.1.2/e2b/api/client/exceptions.py
--rw-r--r--   0        0        0     1021 2023-08-07 00:43:25.926552 e2b-0.1.2/e2b/api/client/models/__init__.py
--rw-r--r--   0        0        0     2232 2023-08-07 00:43:25.926809 e2b-0.1.2/e2b/api/client/models/environment.py
--rw-r--r--   0        0        0      688 2023-08-07 00:43:25.927003 e2b-0.1.2/e2b/api/client/models/environment_state.py
--rw-r--r--   0        0        0     2135 2023-08-07 00:43:25.927152 e2b-0.1.2/e2b/api/client/models/environment_state_update.py
--rw-r--r--   0        0        0     2095 2023-08-07 00:43:25.927312 e2b-0.1.2/e2b/api/client/models/environment_title_update.py
--rw-r--r--   0        0        0     2340 2023-08-07 00:43:25.927550 e2b-0.1.2/e2b/api/client/models/envs_get200_response_inner.py
--rw-r--r--   0        0        0     2049 2023-08-07 00:43:25.927681 e2b-0.1.2/e2b/api/client/models/error.py
--rw-r--r--   0        0        0     2134 2023-08-07 00:43:25.927838 e2b-0.1.2/e2b/api/client/models/new_environment.py
--rw-r--r--   0        0        0     2574 2023-08-07 00:43:25.927985 e2b-0.1.2/e2b/api/client/models/new_session.py
--rw-r--r--   0        0        0     2769 2023-08-07 00:43:25.928104 e2b-0.1.2/e2b/api/client/models/session.py
--rw-r--r--   0        0        0     2949 2023-08-07 00:43:25.928239 e2b-0.1.2/e2b/api/client/models/sessions_get200_response_inner.py
--rw-r--r--   0        0        0      747 2023-08-07 00:43:25.928446 e2b-0.1.2/e2b/api/client/models/template.py
--rw-r--r--   0        0        0     9445 2023-08-07 00:43:25.928592 e2b-0.1.2/e2b/api/client/rest.py
--rw-r--r--   0        0        0        0 2023-08-07 00:43:25.928651 e2b-0.1.2/e2b/api/client/test/__init__.py
--rw-r--r--   0        0        0      725 2023-08-07 00:43:25.928780 e2b-0.1.2/e2b/api/client/test/test_default_api.py
--rw-r--r--   0        0        0     1452 2023-08-07 00:43:25.928914 e2b-0.1.2/e2b/api/client/test/test_environment.py
--rw-r--r--   0        0        0      729 2023-08-07 00:43:25.929049 e2b-0.1.2/e2b/api/client/test/test_environment_state.py
--rw-r--r--   0        0        0     1558 2023-08-07 00:43:25.929182 e2b-0.1.2/e2b/api/client/test/test_environment_state_update.py
--rw-r--r--   0        0        0     1514 2023-08-07 00:43:25.929318 e2b-0.1.2/e2b/api/client/test/test_environment_title_update.py
--rw-r--r--   0        0        0     1381 2023-08-07 00:43:25.929473 e2b-0.1.2/e2b/api/client/test/test_envs_api.py
--rw-r--r--   0        0        0     1611 2023-08-07 00:43:25.929610 e2b-0.1.2/e2b/api/client/test/test_envs_get200_response_inner.py
--rw-r--r--   0        0        0     1384 2023-08-07 00:43:25.929850 e2b-0.1.2/e2b/api/client/test/test_error.py
--rw-r--r--   0        0        0     1470 2023-08-07 00:43:25.929964 e2b-0.1.2/e2b/api/client/test/test_new_environment.py
--rw-r--r--   0        0        0     1445 2023-08-07 00:43:25.930081 e2b-0.1.2/e2b/api/client/test/test_new_session.py
--rw-r--r--   0        0        0     1576 2023-08-07 00:43:25.930204 e2b-0.1.2/e2b/api/client/test/test_session.py
--rw-r--r--   0        0        0     1069 2023-08-07 00:43:25.930323 e2b-0.1.2/e2b/api/client/test/test_sessions_api.py
--rw-r--r--   0        0        0     1831 2023-08-07 00:43:25.930455 e2b-0.1.2/e2b/api/client/test/test_sessions_get200_response_inner.py
--rw-r--r--   0        0        0      672 2023-08-07 00:43:25.930661 e2b-0.1.2/e2b/api/client/test/test_template.py
--rw-r--r--   0        0        0     4174 2023-08-07 00:43:25.930793 e2b-0.1.2/e2b/api/client_README.md
--rw-r--r--   0        0        0      300 2023-08-07 00:43:25.930960 e2b-0.1.2/e2b/api/main.py
--rw-r--r--   0        0        0      142 2023-08-07 00:43:25.931223 e2b-0.1.2/e2b/constants.py
--rw-r--r--   0        0        0      407 2023-08-07 00:43:25.931463 e2b-0.1.2/e2b/session/__init__.py
--rw-r--r--   0        0        0     2997 2023-08-07 00:43:25.931792 e2b-0.1.2/e2b/session/code_snippet.py
--rw-r--r--   0        0        0       50 2023-08-07 00:43:25.932000 e2b-0.1.2/e2b/session/env_vars.py
--rw-r--r--   0        0        0     3514 2023-08-07 00:43:25.932208 e2b-0.1.2/e2b/session/filesystem.py
--rw-r--r--   0        0        0     2130 2023-08-07 00:43:25.932587 e2b-0.1.2/e2b/session/filesystem_watcher.py
--rw-r--r--   0        0        0     4619 2023-08-07 00:43:25.932799 e2b-0.1.2/e2b/session/main.py
--rw-r--r--   0        0        0      404 2023-08-07 00:43:25.932980 e2b-0.1.2/e2b/session/out.py
--rw-r--r--   0        0        0     5941 2023-08-07 00:43:25.933179 e2b-0.1.2/e2b/session/process.py
--rw-r--r--   0        0        0     7933 2023-08-07 00:43:25.933420 e2b-0.1.2/e2b/session/session_connection.py
--rw-r--r--   0        0        0     5171 2023-08-07 00:43:25.933595 e2b-0.1.2/e2b/session/session_daemon.py
--rw-r--r--   0        0        0     5699 2023-08-07 00:43:25.933791 e2b-0.1.2/e2b/session/terminal.py
--rw-r--r--   0        0        0     1109 2023-08-07 00:43:25.934032 e2b-0.1.2/e2b/utils/future.py
--rw-r--r--   0        0        0      166 2023-08-07 00:43:25.934248 e2b-0.1.2/e2b/utils/id.py
--rw-r--r--   0        0        0       34 2023-08-07 00:43:25.934414 e2b-0.1.2/e2b/utils/noop.py
--rw-r--r--   0        0        0      731 2023-08-07 01:00:37.800581 e2b-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 e2b-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2876 2023-08-07 00:59:38.602804 e2b-0.1.3/README.md
+-rw-r--r--   0        0        0      425 2023-08-08 21:35:42.595307 e2b-0.1.3/e2b/__init__.py
+-rw-r--r--   0        0        0     1608 2023-08-07 00:43:25.922993 e2b-0.1.3/e2b/api/.openapi-generator/FILES
+-rw-r--r--   0        0        0        5 2023-08-07 00:43:25.923180 e2b-0.1.3/e2b/api/.openapi-generator/VERSION
+-rw-r--r--   0        0        0     1040 2023-08-07 00:43:25.922714 e2b-0.1.3/e2b/api/.openapi-generator-ignore
+-rw-r--r--   0        0        0        0 2023-08-07 00:43:25.923217 e2b-0.1.3/e2b/api/__init__.py
+-rw-r--r--   0        0        0     1723 2023-08-07 00:43:25.923543 e2b-0.1.3/e2b/api/client/__init__.py
+-rw-r--r--   0        0        0      205 2023-08-07 00:43:25.923792 e2b-0.1.3/e2b/api/client/api/__init__.py
+-rw-r--r--   0        0        0     6652 2023-08-07 00:43:25.923953 e2b-0.1.3/e2b/api/client/api/default_api.py
+-rw-r--r--   0        0        0    52514 2023-08-07 00:43:25.924274 e2b-0.1.3/e2b/api/client/api/envs_api.py
+-rw-r--r--   0        0        0    28662 2023-08-07 00:43:25.924476 e2b-0.1.3/e2b/api/client/api/sessions_api.py
+-rw-r--r--   0        0        0    28991 2023-08-07 00:43:25.924795 e2b-0.1.3/e2b/api/client/api_client.py
+-rw-r--r--   0        0        0      805 2023-08-07 00:43:25.925073 e2b-0.1.3/e2b/api/client/api_response.py
+-rw-r--r--   0        0        0    16423 2023-08-07 00:43:25.925346 e2b-0.1.3/e2b/api/client/configuration.py
+-rw-r--r--   0        0        0     1650 2023-08-07 00:43:25.925814 e2b-0.1.3/e2b/api/client/docs/DefaultApi.md
+-rw-r--r--   0        0        0    14912 2023-08-07 00:43:25.926025 e2b-0.1.3/e2b/api/client/docs/EnvsApi.md
+-rw-r--r--   0        0        0     8210 2023-08-07 00:43:25.926175 e2b-0.1.3/e2b/api/client/docs/SessionsApi.md
+-rw-r--r--   0        0        0     5000 2023-08-07 00:43:25.926379 e2b-0.1.3/e2b/api/client/exceptions.py
+-rw-r--r--   0        0        0     1021 2023-08-07 00:43:25.926552 e2b-0.1.3/e2b/api/client/models/__init__.py
+-rw-r--r--   0        0        0     2232 2023-08-07 00:43:25.926809 e2b-0.1.3/e2b/api/client/models/environment.py
+-rw-r--r--   0        0        0      688 2023-08-07 00:43:25.927003 e2b-0.1.3/e2b/api/client/models/environment_state.py
+-rw-r--r--   0        0        0     2135 2023-08-07 00:43:25.927152 e2b-0.1.3/e2b/api/client/models/environment_state_update.py
+-rw-r--r--   0        0        0     2095 2023-08-07 00:43:25.927312 e2b-0.1.3/e2b/api/client/models/environment_title_update.py
+-rw-r--r--   0        0        0     2340 2023-08-07 00:43:25.927550 e2b-0.1.3/e2b/api/client/models/envs_get200_response_inner.py
+-rw-r--r--   0        0        0     2049 2023-08-07 00:43:25.927681 e2b-0.1.3/e2b/api/client/models/error.py
+-rw-r--r--   0        0        0     2134 2023-08-07 00:43:25.927838 e2b-0.1.3/e2b/api/client/models/new_environment.py
+-rw-r--r--   0        0        0     2574 2023-08-07 00:43:25.927985 e2b-0.1.3/e2b/api/client/models/new_session.py
+-rw-r--r--   0        0        0     2769 2023-08-07 00:43:25.928104 e2b-0.1.3/e2b/api/client/models/session.py
+-rw-r--r--   0        0        0     2949 2023-08-07 00:43:25.928239 e2b-0.1.3/e2b/api/client/models/sessions_get200_response_inner.py
+-rw-r--r--   0        0        0      747 2023-08-07 00:43:25.928446 e2b-0.1.3/e2b/api/client/models/template.py
+-rw-r--r--   0        0        0     9445 2023-08-07 00:43:25.928592 e2b-0.1.3/e2b/api/client/rest.py
+-rw-r--r--   0        0        0        0 2023-08-07 00:43:25.928651 e2b-0.1.3/e2b/api/client/test/__init__.py
+-rw-r--r--   0        0        0      725 2023-08-07 00:43:25.928780 e2b-0.1.3/e2b/api/client/test/test_default_api.py
+-rw-r--r--   0        0        0     1452 2023-08-07 00:43:25.928914 e2b-0.1.3/e2b/api/client/test/test_environment.py
+-rw-r--r--   0        0        0      729 2023-08-07 00:43:25.929049 e2b-0.1.3/e2b/api/client/test/test_environment_state.py
+-rw-r--r--   0        0        0     1558 2023-08-07 00:43:25.929182 e2b-0.1.3/e2b/api/client/test/test_environment_state_update.py
+-rw-r--r--   0        0        0     1514 2023-08-07 00:43:25.929318 e2b-0.1.3/e2b/api/client/test/test_environment_title_update.py
+-rw-r--r--   0        0        0     1381 2023-08-07 00:43:25.929473 e2b-0.1.3/e2b/api/client/test/test_envs_api.py
+-rw-r--r--   0        0        0     1611 2023-08-07 00:43:25.929610 e2b-0.1.3/e2b/api/client/test/test_envs_get200_response_inner.py
+-rw-r--r--   0        0        0     1384 2023-08-07 00:43:25.929850 e2b-0.1.3/e2b/api/client/test/test_error.py
+-rw-r--r--   0        0        0     1470 2023-08-07 00:43:25.929964 e2b-0.1.3/e2b/api/client/test/test_new_environment.py
+-rw-r--r--   0        0        0     1445 2023-08-07 00:43:25.930081 e2b-0.1.3/e2b/api/client/test/test_new_session.py
+-rw-r--r--   0        0        0     1576 2023-08-07 00:43:25.930204 e2b-0.1.3/e2b/api/client/test/test_session.py
+-rw-r--r--   0        0        0     1069 2023-08-07 00:43:25.930323 e2b-0.1.3/e2b/api/client/test/test_sessions_api.py
+-rw-r--r--   0        0        0     1831 2023-08-07 00:43:25.930455 e2b-0.1.3/e2b/api/client/test/test_sessions_get200_response_inner.py
+-rw-r--r--   0        0        0      672 2023-08-07 00:43:25.930661 e2b-0.1.3/e2b/api/client/test/test_template.py
+-rw-r--r--   0        0        0     4174 2023-08-07 00:43:25.930793 e2b-0.1.3/e2b/api/client_README.md
+-rw-r--r--   0        0        0      300 2023-08-07 00:43:25.930960 e2b-0.1.3/e2b/api/main.py
+-rw-r--r--   0        0        0      142 2023-08-08 08:54:57.172806 e2b-0.1.3/e2b/constants.py
+-rw-r--r--   0        0        0      557 2023-08-08 21:35:42.595619 e2b-0.1.3/e2b/session/__init__.py
+-rw-r--r--   0        0        0     3317 2023-08-08 21:35:42.596286 e2b-0.1.3/e2b/session/code_snippet.py
+-rw-r--r--   0        0        0       50 2023-08-07 00:43:25.932000 e2b-0.1.3/e2b/session/env_vars.py
+-rw-r--r--   0        0        0      445 2023-08-08 21:35:42.596727 e2b-0.1.3/e2b/session/exception.py
+-rw-r--r--   0        0        0     4090 2023-08-08 21:35:42.597233 e2b-0.1.3/e2b/session/filesystem.py
+-rw-r--r--   0        0        0     2500 2023-08-08 21:35:42.597648 e2b-0.1.3/e2b/session/filesystem_watcher.py
+-rw-r--r--   0        0        0     4619 2023-08-07 00:43:25.932799 e2b-0.1.3/e2b/session/main.py
+-rw-r--r--   0        0        0      404 2023-08-07 00:43:25.932980 e2b-0.1.3/e2b/session/out.py
+-rw-r--r--   0        0        0     6039 2023-08-08 21:35:42.598237 e2b-0.1.3/e2b/session/process.py
+-rw-r--r--   0        0        0     8506 2023-08-08 21:35:42.598694 e2b-0.1.3/e2b/session/session_connection.py
+-rw-r--r--   0        0        0     5758 2023-08-08 21:35:42.599168 e2b-0.1.3/e2b/session/session_rpc.py
+-rw-r--r--   0        0        0     6154 2023-08-08 21:35:42.599464 e2b-0.1.3/e2b/session/terminal.py
+-rw-r--r--   0        0        0     1002 2023-08-08 21:35:42.599777 e2b-0.1.3/e2b/utils/future.py
+-rw-r--r--   0        0        0      166 2023-08-07 00:43:25.934248 e2b-0.1.3/e2b/utils/id.py
+-rw-r--r--   0        0        0       34 2023-08-07 00:43:25.934414 e2b-0.1.3/e2b/utils/noop.py
+-rw-r--r--   0        0        0      731 2023-08-08 21:35:42.600352 e2b-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 e2b-0.1.3/PKG-INFO
```

### Comparing `e2b-0.1.2/README.md` & `e2b-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/.openapi-generator/FILES` & `e2b-0.1.3/e2b/api/.openapi-generator/FILES`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/.openapi-generator-ignore` & `e2b-0.1.3/e2b/api/.openapi-generator-ignore`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/__init__.py` & `e2b-0.1.3/e2b/api/client/__init__.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/api/default_api.py` & `e2b-0.1.3/e2b/api/client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/api/envs_api.py` & `e2b-0.1.3/e2b/api/client/api/envs_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/api/sessions_api.py` & `e2b-0.1.3/e2b/api/client/api/sessions_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/api_client.py` & `e2b-0.1.3/e2b/api/client/api_client.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/api_response.py` & `e2b-0.1.3/e2b/api/client/api_response.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/configuration.py` & `e2b-0.1.3/e2b/api/client/configuration.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/docs/DefaultApi.md` & `e2b-0.1.3/e2b/api/client/docs/DefaultApi.md`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/docs/EnvsApi.md` & `e2b-0.1.3/e2b/api/client/docs/EnvsApi.md`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/docs/SessionsApi.md` & `e2b-0.1.3/e2b/api/client/docs/SessionsApi.md`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/exceptions.py` & `e2b-0.1.3/e2b/api/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/models/__init__.py` & `e2b-0.1.3/e2b/api/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/models/environment.py` & `e2b-0.1.3/e2b/api/client/models/environment.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/models/environment_state.py` & `e2b-0.1.3/e2b/api/client/models/environment_state.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/models/environment_state_update.py` & `e2b-0.1.3/e2b/api/client/models/environment_state_update.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/models/environment_title_update.py` & `e2b-0.1.3/e2b/api/client/models/environment_title_update.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/models/envs_get200_response_inner.py` & `e2b-0.1.3/e2b/api/client/models/envs_get200_response_inner.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/models/error.py` & `e2b-0.1.3/e2b/api/client/models/error.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/models/new_environment.py` & `e2b-0.1.3/e2b/api/client/models/new_environment.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/models/new_session.py` & `e2b-0.1.3/e2b/api/client/models/new_session.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/models/session.py` & `e2b-0.1.3/e2b/api/client/models/session.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/models/sessions_get200_response_inner.py` & `e2b-0.1.3/e2b/api/client/models/sessions_get200_response_inner.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/models/template.py` & `e2b-0.1.3/e2b/api/client/models/template.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/rest.py` & `e2b-0.1.3/e2b/api/client/rest.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/test/test_default_api.py` & `e2b-0.1.3/e2b/api/client/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/test/test_environment.py` & `e2b-0.1.3/e2b/api/client/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/test/test_environment_state.py` & `e2b-0.1.3/e2b/api/client/test/test_environment_state.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/test/test_environment_state_update.py` & `e2b-0.1.3/e2b/api/client/test/test_environment_state_update.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/test/test_environment_title_update.py` & `e2b-0.1.3/e2b/api/client/test/test_environment_title_update.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/test/test_envs_api.py` & `e2b-0.1.3/e2b/api/client/test/test_envs_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/test/test_envs_get200_response_inner.py` & `e2b-0.1.3/e2b/api/client/test/test_envs_get200_response_inner.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/test/test_error.py` & `e2b-0.1.3/e2b/api/client/test/test_error.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/test/test_new_environment.py` & `e2b-0.1.3/e2b/api/client/test/test_new_environment.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/test/test_new_session.py` & `e2b-0.1.3/e2b/api/client/test/test_new_session.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/test/test_session.py` & `e2b-0.1.3/e2b/api/client/test/test_session.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/test/test_sessions_api.py` & `e2b-0.1.3/e2b/api/client/test/test_sessions_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/test/test_sessions_get200_response_inner.py` & `e2b-0.1.3/e2b/api/client/test/test_sessions_get200_response_inner.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client/test/test_template.py` & `e2b-0.1.3/e2b/api/client/test/test_template.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/api/client_README.md` & `e2b-0.1.3/e2b/api/client_README.md`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/session/code_snippet.py` & `e2b-0.1.3/e2b/session/code_snippet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Optional, ClassVar, Callable, List, Any
 from pydantic import BaseModel
 from enum import Enum
 
+from e2b.session.exception import SessionException, MultipleExceptions
 from e2b.session.out import OutStderrResponse, OutStdoutResponse
 from e2b.session.session_connection import SessionConnection
 from e2b.session.env_vars import EnvVars
+from e2b.session.session_rpc import RpcException
 
 
 class OpenPort(BaseModel):
     ip: str
     port: int
     state: str
 
@@ -51,16 +53,16 @@
             self.service_name, "stop"
         )
         if self.on_state_change:
             self.on_state_change(state)
         return state
 
     async def _subscribe(self):
-        await self.session._handle_subscriptions(
-            [
+        try:
+            await self.session._handle_subscriptions(
                 self.session._subscribe(
                     self.service_name, self.on_state_change, "state"
                 )
                 if self.on_state_change
                 else None,
                 self.session._subscribe(self.service_name, self.on_stderr, "stderr")
                 if self.on_stderr
@@ -82,11 +84,14 @@
                     )
                     if self.on_scan_ports
                     else None,
                     "scanOpenedPorts",
                 )
                 if self.on_scan_ports
                 else None,
-            ],
-        )
+            )
+        except RpcException as e:
+            raise SessionException(e.message) from e
+        except MultipleExceptions as e:
+            raise SessionException("Failed to subscribe to RPC services") from e
 
         return self
```

### Comparing `e2b-0.1.2/e2b/session/filesystem.py` & `e2b-0.1.3/e2b/session/filesystem.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import base64
 
-from pathlib import Path, PosixPath
 from typing import List, Any
 from pydantic import BaseModel
 
 from e2b.session.session_connection import SessionConnection
 from e2b.session.filesystem_watcher import FilesystemWatcher
+from e2b.session.session_rpc import RpcException
+from e2b.session.exception import FilesystemException
 
 
 class FileInfo(BaseModel):
     is_dir: bool
     name: str
 
 
@@ -48,64 +49,78 @@
     async def read(self, path: str) -> str:
         """
         Reads the whole content of a file as an array of bytes.
 
         :param path: path to a file
         :return: content of a file
         """
-        result: str = await self._session._call(self._service_name, "read", [path])
-        return result
+        try:
+            result: str = await self._session._call(self._service_name, "read", [path])
+            return result
+        except RpcException as e:
+            raise FilesystemException(e.message) from e
 
     async def write(self, path: str, content: str) -> None:
         """
         Writes content to a file.
 
         :param path: path to a file
         :param content: content to write
         """
-        await self._session._call(self._service_name, "write", [path, content])
+        try:
+            await self._session._call(self._service_name, "write", [path, content])
+        except RpcException as e:
+            raise FilesystemException(e.message) from e
 
     async def remove(self, path: str) -> None:
         """
         Removes a file or a directory.
 
         :param path: path to a file or a directory
         """
-        await self._session._call(self._service_name, "remove", [path])
+        try:
+            await self._session._call(self._service_name, "remove", [path])
+        except RpcException as e:
+            raise FilesystemException(e.message) from e
 
     async def list(self, path: str) -> List[FileInfo]:
         """
         List files in a directory.
 
         :param path: path to a directory
         :return: array of files in a directory
         """
-        result: List[Any] = await self._session._call(
-            self._service_name, "list", [path]
-        )
-        return [
-            FileInfo(is_dir=file_info["isDir"], name=file_info["name"])
-            for file_info in result
-        ]
+        try:
+            result: List[Any] = await self._session._call(
+                self._service_name, "list", [path]
+            )
+            return [
+                FileInfo(is_dir=file_info["isDir"], name=file_info["name"])
+                for file_info in result
+            ]
+        except RpcException as e:
+            raise FilesystemException(e.message) from e
 
     async def make_dir(self, path: str) -> None:
         """
         Creates a new directory and all directories along the way if needed on the specified path.
 
         :param path: path to a new directory. For example '/dirA/dirB' when creating 'dirB'
         """
-        await self._session._call(self._service_name, "makeDir", [path])
+        try:
+            await self._session._call(self._service_name, "makeDir", [path])
+        except RpcException as e:
+            raise FilesystemException(e.message) from e
 
     async def watch_dir(self, path: str) -> FilesystemWatcher:
         """
         Watches directory for filesystem events.
 
         :param path: path to a directory that will be watched
 
         :return: New watcher
         """
-        npath = PosixPath(Path(path).resolve())
         return FilesystemWatcher(
             connection=self._session,
-            path=str(npath),
+            path=path,
             service_name=self._service_name,
         )
```

### Comparing `e2b-0.1.2/e2b/session/filesystem_watcher.py` & `e2b-0.1.3/e2b/session/filesystem_watcher.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from enum import Enum
-from typing import Callable, Set, Any
+from typing import Callable, Set, Any, Awaitable, Optional
 from pydantic import BaseModel
 
 from e2b.session.session_connection import SessionConnection
+from e2b.session.exception import FilesystemException
+from e2b.session.session_rpc import RpcException
 
 
 class FilesystemOperation(str, Enum):
     Create = "Create"
     Write = "Write"
     Remove = "Remove"
     Rename = "Rename"
@@ -37,38 +39,45 @@
         connection: SessionConnection,
         path: str,
         service_name: str,
     ):
         self._connection = connection
         self._path = path
         self._service_name = service_name
-        self._rpc_subscription_id: str | None = None
+        self._unsubscribe: Optional[Callable[[], Awaitable[Any]]] = None
         self._listeners: Set[Callable[[FilesystemEvent], Any]] = set()
 
     async def start(self) -> None:
         """
         Starts the filesystem watcher.
         """
-        if self._rpc_subscription_id:
+        if self._unsubscribe:
             return
 
-        self._rpc_subscription_id = await self._connection._subscribe(
-            self._service_name,
-            self._handle_filesystem_events,
-            "watchDir",
-            self.path,
-        )
+        try:
+            self._unsubscribe = await self._connection._subscribe(
+                self._service_name,
+                self._handle_filesystem_events,
+                "watchDir",
+                self.path,
+            )
+        except RpcException as e:
+            raise FilesystemException(e.message) from e
 
     async def stop(self) -> None:
         """
         Stops the filesystem watcher.
         """
         self._listeners.clear()
-        if self._rpc_subscription_id:
-            await self._connection._unsubscribe(self._rpc_subscription_id)
+        if self._unsubscribe:
+            try:
+                await self._unsubscribe()
+                self._unsubscribe = None
+            except RpcException as e:
+                raise FilesystemException(e.message) from e
 
     def add_event_listener(self, listener: Callable[[FilesystemEvent], Any]):
         """
         Adds a listener for filesystem events.
 
         :param listener: a listener to add
```

### Comparing `e2b-0.1.2/e2b/session/main.py` & `e2b-0.1.3/e2b/session/main.py`

 * *Files identical despite different names*

### Comparing `e2b-0.1.2/e2b/session/process.py` & `e2b-0.1.3/e2b/session/process.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from e2b.utils.noop import noop
 from e2b.session.out import OutStdoutResponse, OutStderrResponse
 from e2b.utils.future import DeferredFuture
 from e2b.session.env_vars import EnvVars
 from e2b.session.session_connection import SessionConnection
 from e2b.utils.id import create_id
+from e2b.session.session_rpc import RpcException
+from e2b.session.exception import ProcessException, MultipleExceptions
+
 
 logger = logging.getLogger(__name__)
 
 
 class Process:
     @property
     def finished(self):
@@ -46,25 +49,31 @@
 
     async def send_stdin(self, data: str) -> None:
         """
         Sends data to the process stdin.
 
         :param data: Data to send
         """
-        await self._session._call(
-            ProcessManager._service_name, "stdin", [self.process_id, data]
-        )
+        try:
+            await self._session._call(
+                ProcessManager._service_name, "stdin", [self.process_id, data]
+            )
+        except RpcException as e:
+            raise ProcessException(e.message) from e
 
     async def kill(self) -> None:
         """
         Kills the process.
         """
-        await self._session._call(
-            ProcessManager._service_name, "kill", [self.process_id]
-        )
+        try:
+            await self._session._call(
+                ProcessManager._service_name, "kill", [self.process_id]
+            )
+        except RpcException as e:
+            raise ProcessException(e.message) from e
         await self._trigger_exit()
 
 
 class ProcessManager:
     _service_name = "process"
 
     def __init__(self, session: SessionConnection):
@@ -103,75 +112,63 @@
 
         :return: A process object.
         """
 
         future_exit = DeferredFuture(self._process_cleanup)
         process_id = process_id or create_id(12)
 
-        (
-            on_exit_sub_id,
-            on_stdout_sub_id,
-            on_stderr_sub_id,
-        ) = await self._session._handle_subscriptions(
-            [
+        unsub_all: Optional[Callable[[], Awaitable[Any]]] = None
+
+        try:
+            unsub_all = await self._session._handle_subscriptions(
                 self._session._subscribe(
                     self._service_name, future_exit, "onExit", process_id
                 ),
                 self._session._subscribe(
                     self._service_name, on_stdout, "onStdout", process_id
                 )
                 if on_stdout
                 else None,
                 self._session._subscribe(
                     self._service_name, on_stderr, "onStderr", process_id
                 )
                 if on_stderr
                 else None,
-            ],
-        )
+            )
+        except (RpcException, MultipleExceptions) as e:
+            future_exit.cancel()
+
+            if isinstance(e, RpcException):
+                raise ProcessException(e.message) from e
+            elif isinstance(e, MultipleExceptions):
+                raise ProcessException(
+                    "Failed to subscribe to RPC services necessary for starting process"
+                ) from e
 
         future_exit_handler_finish = DeferredFuture(self._process_cleanup)
 
         async def exit_handler():
             await future_exit
             logger.info(
                 f"Handling process exit {process_id} - {future_exit.future.done()}",
             )
-            await asyncio.gather(
-                self._session._unsubscribe(on_exit_sub_id)
-                if on_exit_sub_id
-                else noop(),
-                self._session._unsubscribe(on_stdout_sub_id)
-                if on_stdout_sub_id
-                else noop(),
-                self._session._unsubscribe(on_stderr_sub_id)
-                if on_stderr_sub_id
-                else noop(),
-                return_exceptions=True,
-            )
+            if unsub_all:
+                await unsub_all()
             if on_exit:
                 on_exit()
             future_exit_handler_finish(None)
 
         exit_task = asyncio.create_task(exit_handler())
         self._process_cleanup.append(exit_task.cancel)
 
         async def trigger_exit():
             logger.info("Triggering exit")
             future_exit(None)
             await future_exit_handler_finish
 
-        if (
-            not on_exit_sub_id
-            or (not on_stdout_sub_id and on_stdout)
-            or (not on_stderr_sub_id and on_stderr)
-        ):
-            await trigger_exit()
-            raise Exception("Failed to subscribe to process service")
-
         try:
             await self._session._call(
                 self._service_name,
                 "start",
                 [
                     process_id,
                     cmd,
@@ -181,10 +178,10 @@
             )
             return Process(
                 session=self._session,
                 process_id=process_id,
                 trigger_exit=trigger_exit,
                 finished=future_exit_handler_finish,
             )
-        except:
+        except RpcException as e:
             await trigger_exit()
-            raise
+            raise ProcessException(e.message) from e
```

### Comparing `e2b-0.1.2/e2b/session/session_connection.py` & `e2b-0.1.3/e2b/session/session_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import asyncio
 import logging
 
-from typing import Awaitable, Literal, Optional, Callable, List, Any
+from typing import Awaitable, Literal, Optional, Callable, List, Any, Coroutine
 from pydantic import BaseModel
 
+from e2b.session.exception import MultipleExceptions
 from e2b.utils.future import DeferredFuture
 from e2b.utils.future import format_settled_errors
-from e2b.session.session_daemon import SessionDaemon, Notification
+from e2b.session.session_rpc import SessionRpc, Notification
 from e2b.api.client import NewSession, Session as SessionInfo
 from e2b.utils.noop import noop
 from e2b.api.main import client, configuration
 from e2b.constants import (
     SESSION_DOMAIN,
     WS_PORT,
     WS_ROUTE,
@@ -61,15 +62,15 @@
         self._edit_enabled = edit_enabled
 
         self._session: Optional[SessionInfo] = None
         self._is_open = False
         self._process_cleanup: List[Callable[[], Any]] = []
         self._refreshing_task: Optional[asyncio.Task] = None
         self._subscribers = {}
-        self._daemon: SessionDaemon
+        self._rpc: SessionRpc
         self._finished = DeferredFuture(self._process_cleanup)
 
         logger.info(f"Session for code snippet {self._id} initialized")
 
     def get_hostname(self, port: Optional[int] = None):
         """
         Get the hostname for the session or for the specified session's port.
@@ -101,16 +102,16 @@
         Close the session and unsubscribe from all the subscriptions.
         """
         self._close()
 
         if self._is_open:
             logger.info(f"Closing session {self._session}")
             self._is_open = False
-            if self._daemon:
-                await self._daemon.close()
+            if self._rpc:
+                await self._rpc.close()
 
     def __del__(self):
         self._close()
 
     def _close(self):
         self._subscribers.clear()
 
@@ -149,41 +150,63 @@
         hostname = self.get_hostname(self._debug_port or WS_PORT)
         protocol = "ws" if self._debug_dev_env == "local" else "wss"
 
         session_url = f"{protocol}://{hostname}{WS_ROUTE}"
 
         try:
             logger.info(f"Connection to session: {self._session}")
-            self._daemon = SessionDaemon(
+            self._rpc = SessionRpc(
                 url=session_url,
                 on_message=self._handle_notification,
             )
-            await self._daemon.connect()
+            await self._rpc.connect()
         except Exception as e:
             logger.info(e)
             raise e
 
     async def _call(self, service: str, method: str, params: List[Any] = []):
-        return await self._daemon.send_message(f"{service}_{method}", params)
+        return await self._rpc.send_message(f"{service}_{method}", params)
 
-    async def _handle_subscriptions(self, subs: List[Awaitable[str] | None]):
-        results: List[str | Exception | None] = await asyncio.gather(
+    async def _handle_subscriptions(
+        self,
+        *subs: Awaitable[Callable[[], Awaitable[None]]] | None,
+    ):
+        results: List[
+            Callable[[], Awaitable[None]] | None | Exception
+        ] = await asyncio.gather(
             *[sub if sub else noop() for sub in subs],
             return_exceptions=True,
         )
 
-        if any([isinstance(r, Exception) for r in results]):
-            await asyncio.gather(
-                *[self._unsubscribe(r) for r in results if isinstance(r, str)],
+        exceptions = [e for e in results if isinstance(e, Exception)]
+
+        async def unsub_all():
+            return await asyncio.gather(
+                *[
+                    unsub()
+                    for unsub in results
+                    if not isinstance(unsub, Exception) and unsub
+                ],
                 return_exceptions=True,
             )
-            logger.info(f"Failed to subscribe: {results}")
-            raise Exception(format_settled_errors(results))
 
-        return [r for r in results if isinstance(r, str) or not r]
+        if len(exceptions) > 0:
+            await unsub_all()
+
+            if len(exceptions) == 1:
+                raise exceptions[0]
+
+            error_message = format_settled_errors(exceptions)
+            logger.info(f"Failed to subscribe: {error_message}")
+            raise MultipleExceptions(
+                message=error_message,
+                exceptions=exceptions,
+            )
+
+        return unsub_all
 
     async def _unsubscribe(self, sub_id: str):
         sub = self._subscribers[sub_id]
         await self._call(sub.service, "unsubscribe", [sub.id])
         del self._subscribers[sub_id]
         logger.info(f"Unsubscribed from {sub_id}")
 
@@ -194,15 +217,19 @@
 
         self._subscribers[sub_id] = Subscription(
             service=service, id=sub_id, handler=handler
         )
         logger.info(
             f"Subscribed to {service}_{method} with params [{', '.join(params)}] and with id {sub_id}"
         )
-        return sub_id
+
+        async def unsub():
+            await self._unsubscribe(sub_id)
+
+        return unsub
 
     def _handle_notification(self, data: Notification):
         logger.info(f"Notification {data}")
 
         for id, sub in self._subscribers.items():
             if id == data.params["subscription"]:
                 sub.handler(data.params["result"])
```

### Comparing `e2b-0.1.2/e2b/session/session_daemon.py` & `e2b-0.1.3/e2b/session/session_rpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,20 +14,36 @@
     Iterator,
 )
 from pydantic import BaseModel, PrivateAttr
 from jsonrpcclient import request_json, Ok
 from jsonrpcclient.id_generators import decimal as decimal_id_generator
 from jsonrpcclient.responses import Response, Error, Deserialized
 from websockets.typing import Data
+from e2b.session.exception import SessionException
 
 from e2b.utils.future import DeferredFuture
 
 logger = logging.getLogger(__name__)
 
 
+class RpcException(SessionException):
+    def __init__(
+        self,
+        message: str,
+        code: int,
+        id: str,
+        data: Optional[Dict] = None,
+    ):
+        super().__init__(message)
+        self.data = data
+        self.code = code
+        self.message = message
+        self.id = id
+
+
 class Notification(BaseModel):
     """Nofification"""
 
     method: str
     params: Dict
 
 
@@ -60,15 +76,15 @@
     return (
         map(to_response_or_notification, deserialized)
         if isinstance(deserialized, list)
         else to_response_or_notification(deserialized)
     )
 
 
-class SessionDaemon(BaseModel):
+class SessionRpc(BaseModel):
     url: str
     on_message: Callable[[Notification], None]
 
     _id_generator: Iterator[int] = PrivateAttr(default_factory=decimal_id_generator)
     _waiting_for_replies: Dict[int, DeferredFuture] = PrivateAttr(default_factory=dict)
     _ws: Optional[WebSocketClientProtocol] = PrivateAttr()
 
@@ -135,15 +151,22 @@
                 self._waiting_for_replies[message.id](message.result)
                 return
         elif isinstance(message, Error):
             if (
                 message.id in self._waiting_for_replies
                 and self._waiting_for_replies[message.id]
             ):
-                self._waiting_for_replies[message.id].reject(Exception(message))
+                self._waiting_for_replies[message.id].reject(
+                    RpcException(
+                        code=message.code,
+                        message=message.message,
+                        id=message.id,
+                        data=message.data,
+                    )
+                )
                 return
 
         elif isinstance(message, Notification):
             self.on_message(message)
 
     def __del__(self):
         self._close()
```

### Comparing `e2b-0.1.2/e2b/session/terminal.py` & `e2b-0.1.3/e2b/session/terminal.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 from typing import Awaitable, Callable, Optional, Coroutine, Any, List
 
 from e2b.utils.noop import noop
 from e2b.utils.future import DeferredFuture
 from e2b.session.env_vars import EnvVars
 from e2b.session.session_connection import SessionConnection
 from e2b.utils.id import create_id
+from e2b.session.exception import TerminalException, MultipleExceptions
+from e2b.session.session_rpc import RpcException
 
 
-class TerminalSession:
+class Terminal:
     @property
     def finished(self):
         """
         A future that is resolved when the terminal session exits.
         """
         return self._finished
 
@@ -41,52 +43,60 @@
 
     async def send_data(self, data: str) -> None:
         """
         Sends data to the terminal standard input.
 
         :param data: Data to send
         """
-        await self._session._call(
-            TerminalManager._service_name,
-            "data",
-            [self.terminal_id, data],
-        )
+        try:
+            await self._session._call(
+                TerminalManager._service_name,
+                "data",
+                [self.terminal_id, data],
+            )
+        except RpcException as e:
+            raise TerminalException(e.message) from e
 
     async def resize(self, cols: int, rows: int) -> None:
         """
         Resizes the terminal tty.
 
         :param cols: Number of columns
         :param rows: Number of rows
         """
-        await self._session._call(
-            TerminalManager._service_name,
-            "resize",
-            [self.terminal_id, cols, rows],
-        )
+        try:
+            await self._session._call(
+                TerminalManager._service_name,
+                "resize",
+                [self.terminal_id, cols, rows],
+            )
+        except RpcException as e:
+            raise TerminalException(e.message) from e
 
     async def kill(self) -> None:
         """
         Kill the terminal session.
         """
-        await self._session._call(
-            TerminalManager._service_name, "destroy", [self.terminal_id]
-        )
+        try:
+            await self._session._call(
+                TerminalManager._service_name, "destroy", [self.terminal_id]
+            )
+        except RpcException as e:
+            raise TerminalException(e.message) from e
         await self._trigger_exit()
 
 
 class TerminalManager:
     _service_name = "terminal"
 
     def __init__(self, session: SessionConnection):
         self._session = session
         self._process_cleanup: List[Callable[[], Any]] = []
 
     def __del__(self):
-        print("DELETING")
         self._close()
 
     def _close(self):
         for cleanup in self._process_cleanup:
             cleanup()
 
         self._process_cleanup.clear()
@@ -97,15 +107,15 @@
         cols: int,
         rows: int,
         rootdir: str,
         terminal_id: str | None = None,
         on_exit: Optional[Callable[[], Any]] = None,
         cmd: Optional[str] = None,
         env_vars: Optional[EnvVars] = None,
-    ) -> TerminalSession:
+    ) -> Terminal:
         """
         Start a new terminal session.
 
         :param on_data: Callback that will be called when the terminal sends data
         :param size: Initial size of the terminal
         :param rootdir: Working directory where will the terminal start
         :param terminal_id: Unique identifier of the terminal session
@@ -117,71 +127,69 @@
         :param env_vars: Environment variables that will be accessible inside of the terminal
 
         :return: Terminal session
         """
         future_exit = DeferredFuture(self._process_cleanup)
         terminal_id = terminal_id or create_id(12)
 
-        (
-            on_data_sub_id,
-            on_exit_sub_id,
-        ) = await self._session._handle_subscriptions(
-            [
+        unsub_all: Optional[Callable[[], Awaitable[Any]]] = None
+
+        try:
+            unsub_all = await self._session._handle_subscriptions(
                 self._session._subscribe(
                     self._service_name, on_data, "onData", terminal_id
                 ),
                 self._session._subscribe(
                     self._service_name, future_exit, "onExit", terminal_id
                 ),
-            ],
-        )
+            )
+        except (RpcException, MultipleExceptions) as e:
+            future_exit.cancel()
+
+            if isinstance(e, RpcException):
+                raise TerminalException(e.message) from e
+            elif isinstance(e, MultipleExceptions):
+                raise TerminalException(
+                    "Failed to subscribe to RPC services necessary for starting terminal"
+                ) from e
 
         future_exit_handler_finish = DeferredFuture(self._process_cleanup)
 
         async def exit_handler():
             await future_exit
-            await asyncio.gather(
-                self._session._unsubscribe(on_data_sub_id)
-                if on_data_sub_id
-                else noop(),
-                self._session._unsubscribe(on_exit_sub_id)
-                if on_exit_sub_id
-                else noop(),
-                return_exceptions=True,
-            )
+
+            if unsub_all:
+                await unsub_all()
+
             if on_exit:
                 on_exit()
             future_exit_handler_finish(None)
 
         exit_task = asyncio.create_task(exit_handler())
         self._process_cleanup.append(exit_task.cancel)
 
         async def trigger_exit():
             future_exit(None)
             await future_exit_handler_finish
 
-        if not on_data_sub_id or not on_exit_sub_id:
-            await trigger_exit()
-            raise Exception("Failed to subscribe to terminal service")
-
         try:
             await self._session._call(
                 self._service_name,
                 "start",
                 [
                     terminal_id,
                     cols,
                     rows,
                     env_vars if env_vars else {},
                     cmd,
                     rootdir,
                 ],
             )
-            return TerminalSession(
+            return Terminal(
                 terminal_id=terminal_id,
                 session=self._session,
                 trigger_exit=trigger_exit,
                 finished=future_exit,
             )
-        except:
+        except RpcException as e:
             await trigger_exit()
-            raise
+            raise TerminalException(e.message) from e
```

### Comparing `e2b-0.1.2/e2b/utils/future.py` & `e2b-0.1.3/e2b/utils/future.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 T = TypeVar("T")
 
 
 class DeferredFuture(Generic[T]):
     def __init__(self, cleanup_list: List[Callable[[], Any]] | None = None):
         self.future = asyncio.Future[T]()
         if cleanup_list is not None:
-            cleanup_list.append(self.future.cancel)
+            cleanup_list.append(self.cancel)
 
     def __call__(self, result: T):
         if not self.future.done():
             self.future.set_result(result)
 
     def __await__(self):
         result = yield from self.future.__await__()
@@ -25,17 +25,14 @@
             self.future.cancel()
 
     def reject(self, reason: Exception):
         if not self.future.done():
             self.future.set_exception(reason)
 
 
-def format_settled_errors(settled: List[str | Exception | None]):
-    if all(s is not Exception for s in settled if s is not None):
-        return None
-
+def format_settled_errors(settled: List[Exception]):
     errors = "errors:\n"
     for i, s in enumerate(settled):
         if s is Exception:
             errors += f"\n[{i}]: {json.dumps(s.exception().__str__())}"
 
     return errors
```

### Comparing `e2b-0.1.2/pyproject.toml` & `e2b-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "e2b"
-version = "0.1.2"
+version = "0.1.3"
 description = "E2B SDK that give agents cloud environments"
 authors = ["e2b <hello@e2b.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://e2b.dev/"
 repository = "https://github.com/e2b-dev/rest-api/tree/main/"
 packages = [{ include = "e2b" }]
```

### Comparing `e2b-0.1.2/PKG-INFO` & `e2b-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2b
-Version: 0.1.2
+Version: 0.1.3
 Summary: E2B SDK that give agents cloud environments
 Home-page: https://e2b.dev/
 License: MIT
 Author: e2b
 Author-email: hello@e2b.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

