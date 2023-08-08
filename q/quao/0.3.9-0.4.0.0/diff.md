# Comparing `tmp/quao-0.3.9.tar.gz` & `tmp/quao-0.4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.3.9.tar", last modified: Thu Jul 13 07:49:43 2023, max compression
+gzip compressed data, was "quao-0.4.0.0.tar", last modified: Tue Aug  8 02:49:19 2023, max compression
```

## Comparing `quao-0.3.9.tar` & `quao-0.4.0.0.tar`

### file list

```diff
@@ -1,67 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.053020 quao-0.3.9/
--rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.3.9/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-07-13 07:49:43.053020 quao-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.3.9/README.md
--rw-rw-rw-   0        0        0      967 2023-07-13 07:49:22.000000 quao-0.3.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-13 07:49:43.054021 quao-0.3.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-13 07:49:42.987010 quao-0.3.9/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.3.9/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:49:42.991011 quao-0.3.9/src/quao/
--rw-rw-rw-   0        0        0      262 2023-07-13 07:49:22.000000 quao-0.3.9/src/quao/__init__.py
--rw-rw-rw-   0        0        0     7544 2023-07-13 04:03:03.000000 quao-0.3.9/src/quao/backend.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.016021 quao-0.3.9/src/quao/config/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.3.9/src/quao/config/__init__.py
--rw-rw-rw-   0        0        0      237 2023-06-29 09:59:18.000000 quao-0.3.9/src/quao/config/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.017021 quao-0.3.9/src/quao/data/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.018023 quao-0.3.9/src/quao/data/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/data/job/__init__.py
--rw-rw-rw-   0        0        0      971 2023-07-12 01:46:07.000000 quao-0.3.9/src/quao/data/job/job_response.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.020021 quao-0.3.9/src/quao/data/request/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/data/request/__init__.py
--rw-rw-rw-   0        0        0      680 2023-06-22 02:52:41.000000 quao-0.3.9/src/quao/data/request/request_data.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.030036 quao-0.3.9/src/quao/enum/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/enum/__init__.py
--rw-rw-rw-   0        0        0      185 2023-06-22 02:52:41.000000 quao-0.3.9/src/quao/enum/http_header.py
--rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/enum/http_status.py
--rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.3.9/src/quao/enum/job_status.py
--rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/enum/media_type.py
--rw-rw-rw-   0        0        0      205 2023-06-22 02:52:41.000000 quao-0.3.9/src/quao/enum/processing_unit.py
--rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/enum/provider_type.py
--rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/enum/sdk.py
--rw-rw-rw-   0        0        0      169 2023-06-22 02:52:41.000000 quao-0.3.9/src/quao/enum/token_type.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.032024 quao-0.3.9/src/quao/factory/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/factory/__init__.py
--rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.3.9/src/quao/factory/device_factory.py
--rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.3.9/src/quao/factory/provider_factory.py
--rw-rw-rw-   0        0        0      751 2023-07-13 07:49:10.000000 quao-0.3.9/src/quao/invocation_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.033021 quao-0.3.9/src/quao/model/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.039021 quao-0.3.9/src/quao/model/device/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/model/device/__init__.py
--rw-rw-rw-   0        0        0     2463 2023-07-13 04:03:03.000000 quao-0.3.9/src/quao/model/device/aws_braket_device.py
--rw-rw-rw-   0        0        0     3612 2023-07-13 04:03:03.000000 quao-0.3.9/src/quao/model/device/device.py
--rw-rw-rw-   0        0        0     1008 2023-07-07 07:51:32.000000 quao-0.3.9/src/quao/model/device/ibm_cloud_device.py
--rw-rw-rw-   0        0        0      788 2023-07-12 04:24:43.000000 quao-0.3.9/src/quao/model/device/ibm_quantum_device.py
--rw-rw-rw-   0        0        0     1170 2023-07-13 04:03:03.000000 quao-0.3.9/src/quao/model/device/qiskit_device.py
--rw-rw-rw-   0        0        0     3337 2023-07-13 04:03:03.000000 quao-0.3.9/src/quao/model/device/quao_device.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.041022 quao-0.3.9/src/quao/model/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/model/job/__init__.py
--rw-rw-rw-   0        0        0     3938 2023-07-13 04:03:03.000000 quao-0.3.9/src/quao/model/job/qiskit_status.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.048023 quao-0.3.9/src/quao/model/provider/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/model/provider/__init__.py
--rw-rw-rw-   0        0        0     1251 2023-06-29 09:59:18.000000 quao-0.3.9/src/quao/model/provider/aws_braket_provider.py
--rw-rw-rw-   0        0        0     1004 2023-06-29 09:59:18.000000 quao-0.3.9/src/quao/model/provider/ibm_cloud_provider.py
--rw-rw-rw-   0        0        0      874 2023-06-29 09:59:18.000000 quao-0.3.9/src/quao/model/provider/ibm_quantum_provider.py
--rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.3.9/src/quao/model/provider/provider.py
--rw-rw-rw-   0        0        0     1397 2023-06-29 09:59:18.000000 quao-0.3.9/src/quao/model/provider/quao_provider.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.052021 quao-0.3.9/src/quao/util/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/util/__init__.py
--rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.3.9/src/quao/util/json_parser_util.py
--rw-rw-rw-   0        0        0     1631 2023-07-12 01:46:07.000000 quao-0.3.9/src/quao/util/response_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.014024 quao-0.3.9/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-07-13 07:49:42.000000 quao-0.3.9/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1568 2023-07-13 07:49:42.000000 quao-0.3.9/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 07:49:42.000000 quao-0.3.9/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      201 2023-07-13 07:49:42.000000 quao-0.3.9/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-13 07:49:42.000000 quao-0.3.9/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:19.109789 quao-0.4.0.0/
+-rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.4.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2841 2023-08-08 02:49:19.109789 quao-0.4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.4.0.0/README.md
+-rw-rw-rw-   0        0        0      950 2023-08-08 02:30:12.000000 quao-0.4.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 02:49:19.109789 quao-0.4.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.763698 quao-0.4.0.0/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.4.0.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.764698 quao-0.4.0.0/src/quao/
+-rw-rw-rw-   0        0        0      148 2023-08-08 02:30:12.000000 quao-0.4.0.0/src/quao/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.796725 quao-0.4.0.0/src/quao/async_tasks/
+-rw-rw-rw-   0        0        0        0 2023-08-02 07:11:24.000000 quao-0.4.0.0/src/quao/async_tasks/__init__.py
+-rw-rw-rw-   0        0        0     2893 2023-08-03 09:28:55.000000 quao-0.4.0.0/src/quao/async_tasks/export_circuit_task.py
+-rw-rw-rw-   0        0        0     2265 2023-08-08 02:48:14.000000 quao-0.4.0.0/src/quao/async_tasks/post_processing_task.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.796725 quao-0.4.0.0/src/quao/component/
+-rw-rw-rw-   0        0        0        0 2023-08-02 07:59:07.000000 quao-0.4.0.0/src/quao/component/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.798712 quao-0.4.0.0/src/quao/component/backend/
+-rw-rw-rw-   0        0        0        0 2023-08-02 08:48:32.000000 quao-0.4.0.0/src/quao/component/backend/__init__.py
+-rw-rw-rw-   0        0        0     7206 2023-08-08 01:42:28.000000 quao-0.4.0.0/src/quao/component/backend/backend.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.809711 quao-0.4.0.0/src/quao/component/callback/
+-rw-rw-rw-   0        0        0        0 2023-08-04 04:01:45.000000 quao-0.4.0.0/src/quao/component/callback/__init__.py
+-rw-rw-rw-   0        0        0     1099 2023-08-08 01:09:51.000000 quao-0.4.0.0/src/quao/component/callback/update_job_metadata.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.819715 quao-0.4.0.0/src/quao/component/device/
+-rw-rw-rw-   0        0        0        0 2023-08-02 07:59:14.000000 quao-0.4.0.0/src/quao/component/device/__init__.py
+-rw-rw-rw-   0        0        0     1966 2023-08-03 09:28:55.000000 quao-0.4.0.0/src/quao/component/device/device_selection.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.830712 quao-0.4.0.0/src/quao/config/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.4.0.0/src/quao/config/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-07-25 09:50:22.000000 quao-0.4.0.0/src/quao/config/logging_config.py
+-rw-rw-rw-   0        0        0      449 2023-08-02 09:08:05.000000 quao-0.4.0.0/src/quao/config/thread_config.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.832714 quao-0.4.0.0/src/quao/data/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.0/src/quao/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.840722 quao-0.4.0.0/src/quao/data/backend/
+-rw-rw-rw-   0        0        0        0 2023-08-03 02:36:08.000000 quao-0.4.0.0/src/quao/data/backend/__init__.py
+-rw-rw-rw-   0        0        0      399 2023-08-03 09:11:01.000000 quao-0.4.0.0/src/quao/data/backend/backend_information.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.846712 quao-0.4.0.0/src/quao/data/callback/
+-rw-rw-rw-   0        0        0        0 2023-08-07 01:08:23.000000 quao-0.4.0.0/src/quao/data/callback/__init__.py
+-rw-rw-rw-   0        0        0      354 2023-08-08 01:03:11.000000 quao-0.4.0.0/src/quao/data/callback/callback_url.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.854713 quao-0.4.0.0/src/quao/data/device/
+-rw-rw-rw-   0        0        0        0 2023-08-03 02:52:17.000000 quao-0.4.0.0/src/quao/data/device/__init__.py
+-rw-rw-rw-   0        0        0      400 2023-08-07 02:32:43.000000 quao-0.4.0.0/src/quao/data/device/circuit_running_option.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.868713 quao-0.4.0.0/src/quao/data/promise/
+-rw-rw-rw-   0        0        0        0 2023-08-02 07:44:33.000000 quao-0.4.0.0/src/quao/data/promise/__init__.py
+-rw-rw-rw-   0        0        0      503 2023-08-07 01:08:23.000000 quao-0.4.0.0/src/quao/data/promise/post_processing_promise.py
+-rw-rw-rw-   0        0        0      391 2023-08-07 01:08:23.000000 quao-0.4.0.0/src/quao/data/promise/promise.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.887718 quao-0.4.0.0/src/quao/data/request/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.0/src/quao/data/request/__init__.py
+-rw-rw-rw-   0        0        0     1086 2023-08-07 03:02:26.000000 quao-0.4.0.0/src/quao/data/request/invocation_request.py
+-rw-rw-rw-   0        0        0      329 2023-08-08 02:48:14.000000 quao-0.4.0.0/src/quao/data/request/job_fetching_request.py
+-rw-rw-rw-   0        0        0      532 2023-08-07 01:08:23.000000 quao-0.4.0.0/src/quao/data/request/request.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.894710 quao-0.4.0.0/src/quao/data/response/
+-rw-rw-rw-   0        0        0        0 2023-08-02 07:35:22.000000 quao-0.4.0.0/src/quao/data/response/__init__.py
+-rw-rw-rw-   0        0        0      268 2023-08-03 09:30:53.000000 quao-0.4.0.0/src/quao/data/response/authentication.py
+-rw-rw-rw-   0        0        0     1420 2023-08-08 02:05:29.000000 quao-0.4.0.0/src/quao/data/response/job_response.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.940712 quao-0.4.0.0/src/quao/enum/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.0/src/quao/enum/__init__.py
+-rw-rw-rw-   0        0        0      185 2023-06-22 02:52:41.000000 quao-0.4.0.0/src/quao/enum/http_header.py
+-rw-rw-rw-   0        0        0      224 2023-08-07 08:13:28.000000 quao-0.4.0.0/src/quao/enum/invocation_step.py
+-rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.4.0.0/src/quao/enum/media_type.py
+-rw-rw-rw-   0        0        0      205 2023-06-22 02:52:41.000000 quao-0.4.0.0/src/quao/enum/processing_unit.py
+-rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.4.0.0/src/quao/enum/provider_type.py
+-rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.4.0.0/src/quao/enum/sdk.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.954712 quao-0.4.0.0/src/quao/enum/status/
+-rw-rw-rw-   0        0        0        0 2023-08-07 01:56:06.000000 quao-0.4.0.0/src/quao/enum/status/__init__.py
+-rw-rw-rw-   0        0        0      213 2023-08-07 09:37:04.000000 quao-0.4.0.0/src/quao/enum/status/job_status.py
+-rw-rw-rw-   0        0        0      213 2023-08-07 09:37:04.000000 quao-0.4.0.0/src/quao/enum/status/status_code.py
+-rw-rw-rw-   0        0        0      169 2023-06-22 02:52:41.000000 quao-0.4.0.0/src/quao/enum/token_type.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.976712 quao-0.4.0.0/src/quao/factory/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.0/src/quao/factory/__init__.py
+-rw-rw-rw-   0        0        0     1895 2023-08-07 02:50:02.000000 quao-0.4.0.0/src/quao/factory/device_factory.py
+-rw-rw-rw-   0        0        0      539 2023-08-07 01:08:23.000000 quao-0.4.0.0/src/quao/factory/handler_factory.py
+-rw-rw-rw-   0        0        0     1396 2023-08-07 01:08:23.000000 quao-0.4.0.0/src/quao/factory/provider_factory.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.992712 quao-0.4.0.0/src/quao/handler/
+-rw-rw-rw-   0        0        0        0 2023-08-02 07:11:24.000000 quao-0.4.0.0/src/quao/handler/__init__.py
+-rw-rw-rw-   0        0        0      197 2023-08-04 01:32:03.000000 quao-0.4.0.0/src/quao/handler/handler.py
+-rw-rw-rw-   0        0        0     1360 2023-08-08 01:08:42.000000 quao-0.4.0.0/src/quao/handler/invocation_handler.py
+-rw-rw-rw-   0        0        0     7252 2023-08-08 02:48:14.000000 quao-0.4.0.0/src/quao/handler/job_fetching_handler.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.993712 quao-0.4.0.0/src/quao/model/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.0/src/quao/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:19.036791 quao-0.4.0.0/src/quao/model/device/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.0/src/quao/model/device/__init__.py
+-rw-rw-rw-   0        0        0     2412 2023-08-07 02:49:49.000000 quao-0.4.0.0/src/quao/model/device/aws_braket_device.py
+-rw-rw-rw-   0        0        0     7856 2023-08-08 02:20:30.000000 quao-0.4.0.0/src/quao/model/device/device.py
+-rw-rw-rw-   0        0        0      976 2023-08-07 02:49:49.000000 quao-0.4.0.0/src/quao/model/device/ibm_cloud_device.py
+-rw-rw-rw-   0        0        0      735 2023-08-07 02:49:49.000000 quao-0.4.0.0/src/quao/model/device/ibm_quantum_device.py
+-rw-rw-rw-   0        0        0     1239 2023-08-03 10:12:12.000000 quao-0.4.0.0/src/quao/model/device/qiskit_device.py
+-rw-rw-rw-   0        0        0     3519 2023-08-07 02:49:49.000000 quao-0.4.0.0/src/quao/model/device/quao_device.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:19.072793 quao-0.4.0.0/src/quao/model/provider/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.0/src/quao/model/provider/__init__.py
+-rw-rw-rw-   0        0        0     1251 2023-06-29 09:59:18.000000 quao-0.4.0.0/src/quao/model/provider/aws_braket_provider.py
+-rw-rw-rw-   0        0        0     1004 2023-06-29 09:59:18.000000 quao-0.4.0.0/src/quao/model/provider/ibm_cloud_provider.py
+-rw-rw-rw-   0        0        0      874 2023-06-29 09:59:18.000000 quao-0.4.0.0/src/quao/model/provider/ibm_quantum_provider.py
+-rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.4.0.0/src/quao/model/provider/provider.py
+-rw-rw-rw-   0        0        0     1397 2023-06-29 09:59:18.000000 quao-0.4.0.0/src/quao/model/provider/quao_provider.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:19.107791 quao-0.4.0.0/src/quao/util/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.0/src/quao/util/__init__.py
+-rw-rw-rw-   0        0        0     1058 2023-08-04 04:10:07.000000 quao-0.4.0.0/src/quao/util/circuit_utils.py
+-rw-rw-rw-   0        0        0      274 2023-08-02 08:22:37.000000 quao-0.4.0.0/src/quao/util/http_utils.py
+-rw-rw-rw-   0        0        0      417 2023-08-07 09:11:31.000000 quao-0.4.0.0/src/quao/util/job_status_mapping_utils.py
+-rw-rw-rw-   0        0        0     2322 2023-08-02 07:11:24.000000 quao-0.4.0.0/src/quao/util/json_parser_utils.py
+-rw-rw-rw-   0        0        0     1614 2023-08-08 02:27:11.000000 quao-0.4.0.0/src/quao/util/response_utils.py
+-rw-rw-rw-   0        0        0      890 2023-08-07 09:37:04.000000 quao-0.4.0.0/src/quao/util/status_code_mapping_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:49:18.787702 quao-0.4.0.0/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2841 2023-08-08 02:49:18.000000 quao-0.4.0.0/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2771 2023-08-08 02:49:18.000000 quao-0.4.0.0/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 02:49:18.000000 quao-0.4.0.0/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      190 2023-08-08 02:49:18.000000 quao-0.4.0.0/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-08 02:49:18.000000 quao-0.4.0.0/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.3.9/LICENSE` & `quao-0.4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.3.9/PKG-INFO` & `quao-0.4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.3.9
+Version: 0.4.0.0
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.3.9/README.md` & `quao-0.4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.3.9/pyproject.toml` & `quao-0.4.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.3.9"
+version = "0.4.0.0"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["quao", "quantum"]
 dependencies = [
     "qiskit==0.42.1",
-    "qiskit-aer==0.12.0",
-    "qiskit-aer-gpu",
+    "qiskit-aer-gpu==0.11.2",
     "qbraid==0.4.0",
     "amazon-braket-sdk==1.38.1",
     "qiskit-ibm-runtime",
     "qiskit-ibm-provider",
     "matplotlib",
     "pylatexenc",
     "loguru"
```

### Comparing `quao-0.3.9/src/quao/factory/device_factory.py` & `quao-0.4.0.0/src/quao/factory/device_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 """
     QuaO Project device_factory.py Copyright © CITYNOW Co. Ltd. All rights reserved.
 """
+from ..enum.processing_unit import ProcessingUnit
 from ..enum.provider_type import ProviderType
 from ..model.device.aws_braket_device import AwsBraketDevice
 from ..model.device.ibm_cloud_device import IbmCloudDevice
 from ..model.device.ibm_quantum_device import IbmQuantumDevice
 from ..model.device.quao_device import QuaoDevice
 from ..model.provider.provider import Provider
 
 
 class DeviceFactory:
     @staticmethod
-    def create_device(provider: Provider, device_specification: str, authentication: dict, sdk: str):
+    def create_device(provider: Provider,
+                      device_specification: str,
+                      authentication: dict,
+                      sdk: str,
+                      processing_unit: ProcessingUnit):
         """
 
+        @param processing_unit:
+        @param sdk:
         @param provider:
         @param device_specification:
         @param authentication:
         @return:
         """
 
         provider_type = provider.get_provider_type().value
 
         if ProviderType.QUAO_QUANTUM_SIMULATOR.value.__eq__(provider_type):
-            return QuaoDevice(provider, device_specification, sdk)
+            return QuaoDevice(provider,
+                              device_specification,
+                              sdk,
+                              processing_unit)
 
         if ProviderType.IBM_QUANTUM.value.__eq__(provider_type):
             return IbmQuantumDevice(provider, device_specification)
 
         if ProviderType.IBM_CLOUD.value.__eq__(provider_type):
             return IbmCloudDevice(provider, device_specification)
```

### Comparing `quao-0.3.9/src/quao/factory/provider_factory.py` & `quao-0.4.0.0/src/quao/factory/provider_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,33 +5,35 @@
 from ..model.provider.aws_braket_provider import AwsBraketProvider
 from ..model.provider.ibm_cloud_provider import IbmCloudProvider
 from ..model.provider.ibm_quantum_provider import IbmQuantumProvider
 from ..model.provider.quao_provider import QuaoProvider
 
 
 class ProviderFactory:
-
     @staticmethod
     def create_provider(provider_type: str, authentication: dict):
         """
 
         @param provider_type:
         @param authentication:
         @return:
         """
 
         if ProviderType.QUAO_QUANTUM_SIMULATOR.value.__eq__(provider_type):
             return QuaoProvider()
 
         if ProviderType.IBM_QUANTUM.value.__eq__(provider_type):
-            return IbmQuantumProvider(authentication.get('token'))
+            return IbmQuantumProvider(authentication.get("token"))
 
         if ProviderType.IBM_CLOUD.value.__eq__(provider_type):
-            return IbmCloudProvider(authentication.get('token'), authentication.get('crn'))
+            return IbmCloudProvider(
+                authentication.get("token"), authentication.get("crn")
+            )
 
         if ProviderType.AWS_BRAKET.value.__eq__(provider_type):
             return AwsBraketProvider(
-                authentication.get('accessKey'),
-                authentication.get('secretKey'),
-                authentication.get('regionName'))
+                authentication.get("accessKey"),
+                authentication.get("secretKey"),
+                authentication.get("regionName"),
+            )
 
         raise Exception("Unsupported provider!")
```

### Comparing `quao-0.3.9/src/quao/model/device/aws_braket_device.py` & `quao-0.4.0.0/src/quao/model/device/aws_braket_device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     QuaO Project aws_braket_device.py Copyright © CITYNOW Co. Ltd. All rights reserved.
 """
 from ..device.device import Device
 from ..provider.provider import Provider
+from ...data.device.circuit_running_option import CircuitRunningOption
 from ...enum.job_status import JobStatus
-from ...util.json_parser_util import JsonParserUtils
-from ...config.logging_config import *
+from ...config.logging_config import logger
 from dateutil.parser import parse
 
 
 class AwsBraketDevice(Device):
     def _get_name(self) -> str:
         return str(self.device.name)
 
     def __init__(self, provider: Provider,
                  device_specification: str,
                  s3_bucket_name: str,
                  s3_prefix: str):
         super().__init__(provider, device_specification)
         self.s3_folder = (s3_bucket_name, s3_prefix)
 
-    def _create_job(self, circuit, shots):
-        logger.debug('Create AWS Braket job with {0} shots'.format(shots))
+    def _create_job(self, circuit,  options: CircuitRunningOption):
+        logger.debug('Create AWS Braket job with {0} shots'.format(options.shots))
 
         job = self.device.run(task_specification=circuit,
                               s3_destination_folder=self.s3_folder,
-                              shots=shots)
+                              shots=options.shots)
         return job
 
     def _is_simulator(self) -> bool:
         return 'SIMULATOR'.__eq__(self.device.type.value)
 
     def _produce_histogram_data(self, job_result) -> dict:
         return dict(job_result.measurement_counts)
@@ -39,17 +39,14 @@
 
     def _get_job_status(self, job) -> str:
         job_state = job.state()
         if JobStatus.COMPLETED.value.__eq__(job_state):
             job_state = JobStatus.DONE.value
         return job_state
 
-    def _parse_job_result(self, job_result) -> dict:
-        return JsonParserUtils.parse(job_result.__dict__)
-
     def _calculate_execution_time(self, job_result):
         if 'task_metadata' not in job_result:
             return
 
         task_metadata = job_result['task_metadata']
 
         if task_metadata is None \
```

### Comparing `quao-0.3.9/src/quao/model/device/ibm_quantum_device.py` & `quao-0.4.0.0/src/quao/model/device/ibm_quantum_device.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """
     QuaO Project ibm_quantum_device.py Copyright © CITYNOW Co. Ltd. All rights reserved.
 """
 
 from qiskit import transpile
 
+from ...data.device.circuit_running_option import CircuitRunningOption
 from ...model.device.qiskit_device import QiskitDevice
-from ...util.json_parser_util import JsonParserUtils
-from ...config.logging_config import *
+from ...config.logging_config import logger
 
 
 class IbmQuantumDevice(QiskitDevice):
 
     def _is_simulator(self) -> bool:
         return self.device.configuration().simulator
 
-    def _parse_job_result(self, job_result) -> dict:
-        return JsonParserUtils.parse(job_result.to_dict())
-
-    def _create_job(self, circuit, shots):
-        logger.debug('Create Ibm Quantum job with {0} shots'.format(shots))
+    def _create_job(self, circuit, options: CircuitRunningOption):
+        logger.debug('Create Ibm Quantum job with {0} shots'.format(options.shots))
         transpile_circuit = transpile(circuit, self.device)
 
-        return self.device.run(transpile_circuit, shots=shots)
+        return self.device.run(transpile_circuit, shots=options.shots)
```

### Comparing `quao-0.3.9/src/quao/model/device/qiskit_device.py` & `quao-0.4.0.0/src/quao/model/device/qiskit_device.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     QuaO Project qiskit_device.py Copyright © CITYNOW Co. Ltd. All rights reserved.
 """
 from abc import ABC
 
 from qiskit import QiskitError
 
 from ...model.device.device import Device
-from ...config.logging_config import *
+from ...config.logging_config import logger
 
 
 class QiskitDevice(Device, ABC):
 
     def _produce_histogram_data(self, job_result) -> dict:
         try:
             histogram_data = job_result.get_counts()
@@ -26,16 +26,16 @@
     def _get_job_status(self, job) -> str:
         return job.status().name
 
     def _get_name(self) -> str:
         return str(self.device.configuration().backend_name)
 
     def _calculate_execution_time(self, job_result):
-        if 'metadata' not in job_result:
-            return
+        if "_metadata" not in job_result:
+            return None
 
-        metadata = job_result['metadata']
+        metadata = job_result["_metadata"]["metadata"]
 
-        if metadata is None or not bool(metadata):
-            return
+        if metadata is None or not bool(metadata) or "time_taken_execute" not in metadata:
+            return None
 
-        self.execution_time = metadata['time_taken_execute']
+        self.execution_time = metadata["time_taken_execute"]
```

### Comparing `quao-0.3.9/src/quao/model/device/quao_device.py` & `quao-0.4.0.0/src/quao/model/device/quao_device.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 """
     QuaO Project quao_device.py Copyright © CITYNOW Co. Ltd. All rights reserved.
 """
 from qiskit import transpile
 from qiskit import QiskitError
 
+from ...data.device.circuit_running_option import CircuitRunningOption
 from ...enum.job_status import JobStatus
 from ...enum.processing_unit import ProcessingUnit
-from ...util.json_parser_util import JsonParserUtils
 from ...enum.sdk import Sdk
 from ..device.device import Device
 from ..provider.provider import Provider
-from ...config.logging_config import *
+from ...config.logging_config import logger
 
 
 class QuaoDevice(Device):
-    def _get_name(self) -> str:
-        return str(self.device.configuration().backend_name)
 
-    def __init__(self, provider: Provider, device_specification: str, sdk: str):
+    def __init__(self, provider: Provider,
+                 device_specification: str,
+                 sdk: str,
+                 processing_unit: ProcessingUnit):
         super().__init__(provider, device_specification)
         self.sdk = sdk
+        self.processing_unit = processing_unit
+
+    def _get_name(self) -> str:
+        if Sdk.QISKIT.value.__eq__(self.sdk):
+            return str(self.device.configuration().backend_name)
+
+        if Sdk.BRAKET.value.__eq__(self.sdk):
+            return str(self.device.name)
+
+        raise Exception("Sdk not supported!")
 
-    def _create_job(self, circuit, shots):
-        logger.debug('Create Quao job with {0} shots'.format(shots))
+    def _create_job(self, circuit,  options: CircuitRunningOption):
+        logger.debug('Create Quao job with {0} shots'.format(options.shots))
         if Sdk.QISKIT.value.__eq__(self.sdk):
-            self.device.set_options(device=ProcessingUnit.GPU.value, shots=shots)
+            self.device.set_options(device=self.processing_unit.value, shots=options.shots)
             transpiled_circuit = transpile(circuits=circuit, backend=self.device)
 
             return self.device.run(transpiled_circuit)
 
         if Sdk.BRAKET.value.__eq__(self.sdk):
             import time
 
             start_time = time.time()
 
-            job = self.device.run(task_specification=circuit, shots=shots)
+            job = self.device.run(task_specification=circuit, shots=options.shots)
 
             self.execution_time = time.time() - start_time
 
             return job
 
         raise Exception("Sdk not supported!")
 
     def _is_simulator(self) -> bool:
         return True
 
-    def _parse_job_result(self, job_result) -> dict:
-        if Sdk.QISKIT.value.__eq__(self.sdk):
-            return JsonParserUtils.parse(job_result.to_dict())
-
-        if Sdk.BRAKET.value.__eq__(self.sdk):
-            return JsonParserUtils.parse(job_result.__dict__)
-
     def _produce_histogram_data(self, job_result) -> dict:
         if Sdk.QISKIT.value.__eq__(self.sdk):
             try:
                 histogram_data = job_result.get_counts()
             except QiskitError as qiskit_error:
                 logger.debug("Can't produce histogram with error: {0}".format(str(qiskit_error)))
                 histogram_data = None
@@ -80,18 +84,20 @@
             job_state = job.state()
             if JobStatus.COMPLETED.value.__eq__(job_state):
                 job_state = JobStatus.DONE.value
             return job_state
 
     def _calculate_execution_time(self, job_result):
         if Sdk.QISKIT.value.__eq__(self.sdk):
-            if 'metadata' not in job_result:
-                return
-
-            metadata = job_result['metadata']
-
-            if metadata is None \
-                    or not bool(metadata)\
-                    or 'time_taken_execute' not in metadata:
-                return
-
-            self.execution_time = metadata['time_taken_execute']
+            if "_metadata" not in job_result:
+                return None
+    
+            metadata = job_result["_metadata"]["metadata"]
+    
+            if (
+                metadata is None
+                or not bool(metadata)
+                or "time_taken_execute" not in metadata
+            ):
+                return None
+    
+            self.execution_time = metadata["time_taken_execute"]
```

### Comparing `quao-0.3.9/src/quao/model/provider/aws_braket_provider.py` & `quao-0.4.0.0/src/quao/model/provider/aws_braket_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.9/src/quao/model/provider/ibm_cloud_provider.py` & `quao-0.4.0.0/src/quao/model/provider/ibm_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.9/src/quao/model/provider/ibm_quantum_provider.py` & `quao-0.4.0.0/src/quao/model/provider/ibm_quantum_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.9/src/quao/model/provider/provider.py` & `quao-0.4.0.0/src/quao/model/provider/provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.9/src/quao/model/provider/quao_provider.py` & `quao-0.4.0.0/src/quao/model/provider/quao_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.9/src/quao/util/response_utils.py` & `quao-0.4.0.0/src/quao/util/response_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 """
     QuaO Project response_utils.py Copyright © CITYNOW Co. Ltd. All rights reserved.
 """
-from ..data.job.job_response import JobResponse
-from ..enum.http_status import HttpStatus
-from ..enum.job_status import JobStatus
+from .job_status_mapping_utils import JobStatusMappingUtils
+from .status_code_mapping_utils import StatusCodeMappingUtils
+from ..data.response.job_response import JobResponse
 
 
 class ResponseUtils:
 
     @staticmethod
     def generate_response(job_response: JobResponse) -> dict:
         if job_response:
-            status_code = HttpStatus.NOT_YET_FINISHED.value
-
-            if JobStatus.DONE.value.__eq__(job_response.job_status):
-                status_code = HttpStatus.SUCCESS.value
-
-            elif JobStatus.ERROR.value.__eq__(job_response.job_status):
-                status_code = HttpStatus.ERROR.value
 
             job_dict = {
                 "providerJobId": job_response.provider_job_id,
                 "jobStatus": job_response.job_status,
                 "jobResult": job_response.job_result,
-                "contentType": job_response.content_type,
+                "contentType": job_response.content_type.value,
                 "histogram": job_response.job_histogram,
                 "executionTime": job_response.execution_time
             }
 
+            mapping_key = job_response.invocation_step \
+                if JobStatusMappingUtils.resolve_job_status(job_response.job_status) is None \
+                else job_response.job_status
+
             response = {
-                "statusCode": status_code,
+                "statusCode": StatusCodeMappingUtils.resolve_status_code(mapping_key),
                 "body": job_dict,
                 "userIdentity": job_response.user_identity,
                 "userToken": job_response.user_token
             }
+
         else:
             response = {
                 "statusCode": 500,
                 "body": "Error in function code. Please contact the developer.",
                 "userIdentity": job_response.user_identity,
                 "userToken": job_response.user_token
             }
+
         return response
```

### Comparing `quao-0.3.9/src/quao.egg-info/PKG-INFO` & `quao-0.4.0.0/src/quao.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.3.9
+Version: 0.4.0.0
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

