# Comparing `tmp/quao-0.4.0.3.tar.gz` & `tmp/quao-0.4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.4.0.3.tar", last modified: Tue Aug  8 05:08:33 2023, max compression
+gzip compressed data, was "quao-0.4.0.4.tar", last modified: Tue Aug  8 06:41:32 2023, max compression
```

## Comparing `quao-0.4.0.3.tar` & `quao-0.4.0.4.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.793717 quao-0.4.0.3/
--rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.4.0.3/LICENSE
--rw-rw-rw-   0        0        0     2841 2023-08-08 05:08:33.793717 quao-0.4.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.4.0.3/README.md
--rw-rw-rw-   0        0        0      950 2023-08-08 05:08:19.000000 quao-0.4.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-08 05:08:33.793717 quao-0.4.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.722057 quao-0.4.0.3/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.4.0.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.722057 quao-0.4.0.3/src/quao/
--rw-rw-rw-   0        0        0      148 2023-08-08 05:08:19.000000 quao-0.4.0.3/src/quao/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.741714 quao-0.4.0.3/src/quao/async_tasks/
--rw-rw-rw-   0        0        0        0 2023-08-02 07:11:24.000000 quao-0.4.0.3/src/quao/async_tasks/__init__.py
--rw-rw-rw-   0        0        0     2893 2023-08-03 09:28:55.000000 quao-0.4.0.3/src/quao/async_tasks/export_circuit_task.py
--rw-rw-rw-   0        0        0     2265 2023-08-08 02:48:14.000000 quao-0.4.0.3/src/quao/async_tasks/post_processing_task.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.742717 quao-0.4.0.3/src/quao/component/
--rw-rw-rw-   0        0        0        0 2023-08-02 07:59:07.000000 quao-0.4.0.3/src/quao/component/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.743714 quao-0.4.0.3/src/quao/component/backend/
--rw-rw-rw-   0        0        0        0 2023-08-02 08:48:32.000000 quao-0.4.0.3/src/quao/component/backend/__init__.py
--rw-rw-rw-   0        0        0     7206 2023-08-08 01:42:28.000000 quao-0.4.0.3/src/quao/component/backend/backend.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.745715 quao-0.4.0.3/src/quao/component/callback/
--rw-rw-rw-   0        0        0        0 2023-08-04 04:01:45.000000 quao-0.4.0.3/src/quao/component/callback/__init__.py
--rw-rw-rw-   0        0        0     1109 2023-08-08 05:03:57.000000 quao-0.4.0.3/src/quao/component/callback/update_job_metadata.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.746715 quao-0.4.0.3/src/quao/component/device/
--rw-rw-rw-   0        0        0        0 2023-08-02 07:59:14.000000 quao-0.4.0.3/src/quao/component/device/__init__.py
--rw-rw-rw-   0        0        0     1966 2023-08-03 09:28:55.000000 quao-0.4.0.3/src/quao/component/device/device_selection.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.748714 quao-0.4.0.3/src/quao/config/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.4.0.3/src/quao/config/__init__.py
--rw-rw-rw-   0        0        0      237 2023-07-25 09:50:22.000000 quao-0.4.0.3/src/quao/config/logging_config.py
--rw-rw-rw-   0        0        0      449 2023-08-02 09:08:05.000000 quao-0.4.0.3/src/quao/config/thread_config.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.749715 quao-0.4.0.3/src/quao/data/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.3/src/quao/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.750715 quao-0.4.0.3/src/quao/data/backend/
--rw-rw-rw-   0        0        0        0 2023-08-03 02:36:08.000000 quao-0.4.0.3/src/quao/data/backend/__init__.py
--rw-rw-rw-   0        0        0      399 2023-08-03 09:11:01.000000 quao-0.4.0.3/src/quao/data/backend/backend_information.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.751716 quao-0.4.0.3/src/quao/data/callback/
--rw-rw-rw-   0        0        0        0 2023-08-07 01:08:23.000000 quao-0.4.0.3/src/quao/data/callback/__init__.py
--rw-rw-rw-   0        0        0      354 2023-08-08 01:03:11.000000 quao-0.4.0.3/src/quao/data/callback/callback_url.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.753715 quao-0.4.0.3/src/quao/data/device/
--rw-rw-rw-   0        0        0        0 2023-08-03 02:52:17.000000 quao-0.4.0.3/src/quao/data/device/__init__.py
--rw-rw-rw-   0        0        0      400 2023-08-07 02:32:43.000000 quao-0.4.0.3/src/quao/data/device/circuit_running_option.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.755715 quao-0.4.0.3/src/quao/data/promise/
--rw-rw-rw-   0        0        0        0 2023-08-02 07:44:33.000000 quao-0.4.0.3/src/quao/data/promise/__init__.py
--rw-rw-rw-   0        0        0      503 2023-08-07 01:08:23.000000 quao-0.4.0.3/src/quao/data/promise/post_processing_promise.py
--rw-rw-rw-   0        0        0      391 2023-08-07 01:08:23.000000 quao-0.4.0.3/src/quao/data/promise/promise.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.759724 quao-0.4.0.3/src/quao/data/request/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.3/src/quao/data/request/__init__.py
--rw-rw-rw-   0        0        0     1084 2023-08-08 03:22:06.000000 quao-0.4.0.3/src/quao/data/request/invocation_request.py
--rw-rw-rw-   0        0        0      329 2023-08-08 02:48:14.000000 quao-0.4.0.3/src/quao/data/request/job_fetching_request.py
--rw-rw-rw-   0        0        0      532 2023-08-07 01:08:23.000000 quao-0.4.0.3/src/quao/data/request/request.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.761716 quao-0.4.0.3/src/quao/data/response/
--rw-rw-rw-   0        0        0        0 2023-08-02 07:35:22.000000 quao-0.4.0.3/src/quao/data/response/__init__.py
--rw-rw-rw-   0        0        0      268 2023-08-03 09:30:53.000000 quao-0.4.0.3/src/quao/data/response/authentication.py
--rw-rw-rw-   0        0        0     1420 2023-08-08 02:05:29.000000 quao-0.4.0.3/src/quao/data/response/job_response.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.768714 quao-0.4.0.3/src/quao/enum/
--rw-rw-rw-   0        0        0        0 2023-08-08 03:42:09.000000 quao-0.4.0.3/src/quao/enum/__init__.py
--rw-rw-rw-   0        0        0      243 2023-08-08 05:03:57.000000 quao-0.4.0.3/src/quao/enum/http_header.py
--rw-rw-rw-   0        0        0      230 2023-08-08 04:21:37.000000 quao-0.4.0.3/src/quao/enum/invocation_step.py
--rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.4.0.3/src/quao/enum/media_type.py
--rw-rw-rw-   0        0        0      205 2023-06-22 02:52:41.000000 quao-0.4.0.3/src/quao/enum/processing_unit.py
--rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.4.0.3/src/quao/enum/provider_type.py
--rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.4.0.3/src/quao/enum/sdk.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.770714 quao-0.4.0.3/src/quao/enum/status/
--rw-rw-rw-   0        0        0        0 2023-08-08 03:42:12.000000 quao-0.4.0.3/src/quao/enum/status/__init__.py
--rw-rw-rw-   0        0        0      213 2023-08-07 09:37:04.000000 quao-0.4.0.3/src/quao/enum/status/job_status.py
--rw-rw-rw-   0        0        0      213 2023-08-07 09:37:04.000000 quao-0.4.0.3/src/quao/enum/status/status_code.py
--rw-rw-rw-   0        0        0      169 2023-06-22 02:52:41.000000 quao-0.4.0.3/src/quao/enum/token_type.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.772715 quao-0.4.0.3/src/quao/factory/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.3/src/quao/factory/__init__.py
--rw-rw-rw-   0        0        0     1895 2023-08-07 02:50:02.000000 quao-0.4.0.3/src/quao/factory/device_factory.py
--rw-rw-rw-   0        0        0      539 2023-08-07 01:08:23.000000 quao-0.4.0.3/src/quao/factory/handler_factory.py
--rw-rw-rw-   0        0        0     1396 2023-08-07 01:08:23.000000 quao-0.4.0.3/src/quao/factory/provider_factory.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.775715 quao-0.4.0.3/src/quao/handler/
--rw-rw-rw-   0        0        0        0 2023-08-02 07:11:24.000000 quao-0.4.0.3/src/quao/handler/__init__.py
--rw-rw-rw-   0        0        0      197 2023-08-04 01:32:03.000000 quao-0.4.0.3/src/quao/handler/handler.py
--rw-rw-rw-   0        0        0     1360 2023-08-08 01:08:42.000000 quao-0.4.0.3/src/quao/handler/invocation_handler.py
--rw-rw-rw-   0        0        0     7252 2023-08-08 02:48:14.000000 quao-0.4.0.3/src/quao/handler/job_fetching_handler.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.776730 quao-0.4.0.3/src/quao/model/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.3/src/quao/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.782714 quao-0.4.0.3/src/quao/model/device/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.3/src/quao/model/device/__init__.py
--rw-rw-rw-   0        0        0     2419 2023-08-08 03:34:32.000000 quao-0.4.0.3/src/quao/model/device/aws_braket_device.py
--rw-rw-rw-   0        0        0     7856 2023-08-08 02:20:30.000000 quao-0.4.0.3/src/quao/model/device/device.py
--rw-rw-rw-   0        0        0      976 2023-08-07 02:49:49.000000 quao-0.4.0.3/src/quao/model/device/ibm_cloud_device.py
--rw-rw-rw-   0        0        0      735 2023-08-07 02:49:49.000000 quao-0.4.0.3/src/quao/model/device/ibm_quantum_device.py
--rw-rw-rw-   0        0        0     1239 2023-08-03 10:12:12.000000 quao-0.4.0.3/src/quao/model/device/qiskit_device.py
--rw-rw-rw-   0        0        0     3526 2023-08-08 04:16:49.000000 quao-0.4.0.3/src/quao/model/device/quao_device.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.786716 quao-0.4.0.3/src/quao/model/provider/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.3/src/quao/model/provider/__init__.py
--rw-rw-rw-   0        0        0     1251 2023-06-29 09:59:18.000000 quao-0.4.0.3/src/quao/model/provider/aws_braket_provider.py
--rw-rw-rw-   0        0        0     1004 2023-06-29 09:59:18.000000 quao-0.4.0.3/src/quao/model/provider/ibm_cloud_provider.py
--rw-rw-rw-   0        0        0      874 2023-06-29 09:59:18.000000 quao-0.4.0.3/src/quao/model/provider/ibm_quantum_provider.py
--rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.4.0.3/src/quao/model/provider/provider.py
--rw-rw-rw-   0        0        0     1397 2023-06-29 09:59:18.000000 quao-0.4.0.3/src/quao/model/provider/quao_provider.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.791716 quao-0.4.0.3/src/quao/util/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.3/src/quao/util/__init__.py
--rw-rw-rw-   0        0        0     1058 2023-08-04 04:10:07.000000 quao-0.4.0.3/src/quao/util/circuit_utils.py
--rw-rw-rw-   0        0        0      643 2023-08-08 05:08:06.000000 quao-0.4.0.3/src/quao/util/http_utils.py
--rw-rw-rw-   0        0        0      417 2023-08-07 09:11:31.000000 quao-0.4.0.3/src/quao/util/job_status_mapping_utils.py
--rw-rw-rw-   0        0        0     2322 2023-08-02 07:11:24.000000 quao-0.4.0.3/src/quao/util/json_parser_utils.py
--rw-rw-rw-   0        0        0     1614 2023-08-08 02:27:11.000000 quao-0.4.0.3/src/quao/util/response_utils.py
--rw-rw-rw-   0        0        0      890 2023-08-08 04:21:48.000000 quao-0.4.0.3/src/quao/util/status_code_mapping_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-08 05:08:33.739706 quao-0.4.0.3/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2841 2023-08-08 05:08:33.000000 quao-0.4.0.3/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2771 2023-08-08 05:08:33.000000 quao-0.4.0.3/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 05:08:33.000000 quao-0.4.0.3/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      190 2023-08-08 05:08:33.000000 quao-0.4.0.3/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-08-08 05:08:33.000000 quao-0.4.0.3/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.572747 quao-0.4.0.4/
+-rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.4.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2841 2023-08-08 06:41:32.571748 quao-0.4.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.4.0.4/README.md
+-rw-rw-rw-   0        0        0      950 2023-08-08 06:41:16.000000 quao-0.4.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 06:41:32.572747 quao-0.4.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.485747 quao-0.4.0.4/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.4.0.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.486747 quao-0.4.0.4/src/quao/
+-rw-rw-rw-   0        0        0      148 2023-08-08 06:41:16.000000 quao-0.4.0.4/src/quao/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.509749 quao-0.4.0.4/src/quao/async_tasks/
+-rw-rw-rw-   0        0        0        0 2023-08-02 07:11:24.000000 quao-0.4.0.4/src/quao/async_tasks/__init__.py
+-rw-rw-rw-   0        0        0     2893 2023-08-03 09:28:55.000000 quao-0.4.0.4/src/quao/async_tasks/export_circuit_task.py
+-rw-rw-rw-   0        0        0     2265 2023-08-08 02:48:14.000000 quao-0.4.0.4/src/quao/async_tasks/post_processing_task.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.511758 quao-0.4.0.4/src/quao/component/
+-rw-rw-rw-   0        0        0        0 2023-08-02 07:59:07.000000 quao-0.4.0.4/src/quao/component/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.512747 quao-0.4.0.4/src/quao/component/backend/
+-rw-rw-rw-   0        0        0        0 2023-08-02 08:48:32.000000 quao-0.4.0.4/src/quao/component/backend/__init__.py
+-rw-rw-rw-   0        0        0     7206 2023-08-08 01:42:28.000000 quao-0.4.0.4/src/quao/component/backend/backend.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.514748 quao-0.4.0.4/src/quao/component/callback/
+-rw-rw-rw-   0        0        0        0 2023-08-04 04:01:45.000000 quao-0.4.0.4/src/quao/component/callback/__init__.py
+-rw-rw-rw-   0        0        0     1109 2023-08-08 05:03:57.000000 quao-0.4.0.4/src/quao/component/callback/update_job_metadata.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.516746 quao-0.4.0.4/src/quao/component/device/
+-rw-rw-rw-   0        0        0        0 2023-08-02 07:59:14.000000 quao-0.4.0.4/src/quao/component/device/__init__.py
+-rw-rw-rw-   0        0        0     1966 2023-08-03 09:28:55.000000 quao-0.4.0.4/src/quao/component/device/device_selection.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.519748 quao-0.4.0.4/src/quao/config/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.4.0.4/src/quao/config/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-07-25 09:50:22.000000 quao-0.4.0.4/src/quao/config/logging_config.py
+-rw-rw-rw-   0        0        0      449 2023-08-02 09:08:05.000000 quao-0.4.0.4/src/quao/config/thread_config.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.520750 quao-0.4.0.4/src/quao/data/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.4/src/quao/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.522749 quao-0.4.0.4/src/quao/data/backend/
+-rw-rw-rw-   0        0        0        0 2023-08-03 02:36:08.000000 quao-0.4.0.4/src/quao/data/backend/__init__.py
+-rw-rw-rw-   0        0        0      399 2023-08-03 09:11:01.000000 quao-0.4.0.4/src/quao/data/backend/backend_information.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.523749 quao-0.4.0.4/src/quao/data/callback/
+-rw-rw-rw-   0        0        0        0 2023-08-07 01:08:23.000000 quao-0.4.0.4/src/quao/data/callback/__init__.py
+-rw-rw-rw-   0        0        0      354 2023-08-08 01:03:11.000000 quao-0.4.0.4/src/quao/data/callback/callback_url.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.525748 quao-0.4.0.4/src/quao/data/device/
+-rw-rw-rw-   0        0        0        0 2023-08-03 02:52:17.000000 quao-0.4.0.4/src/quao/data/device/__init__.py
+-rw-rw-rw-   0        0        0      400 2023-08-07 02:32:43.000000 quao-0.4.0.4/src/quao/data/device/circuit_running_option.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.528749 quao-0.4.0.4/src/quao/data/promise/
+-rw-rw-rw-   0        0        0        0 2023-08-02 07:44:33.000000 quao-0.4.0.4/src/quao/data/promise/__init__.py
+-rw-rw-rw-   0        0        0      503 2023-08-07 01:08:23.000000 quao-0.4.0.4/src/quao/data/promise/post_processing_promise.py
+-rw-rw-rw-   0        0        0      391 2023-08-07 01:08:23.000000 quao-0.4.0.4/src/quao/data/promise/promise.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.531749 quao-0.4.0.4/src/quao/data/request/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.4/src/quao/data/request/__init__.py
+-rw-rw-rw-   0        0        0     1084 2023-08-08 03:22:06.000000 quao-0.4.0.4/src/quao/data/request/invocation_request.py
+-rw-rw-rw-   0        0        0      329 2023-08-08 02:48:14.000000 quao-0.4.0.4/src/quao/data/request/job_fetching_request.py
+-rw-rw-rw-   0        0        0      532 2023-08-07 01:08:23.000000 quao-0.4.0.4/src/quao/data/request/request.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.533748 quao-0.4.0.4/src/quao/data/response/
+-rw-rw-rw-   0        0        0        0 2023-08-02 07:35:22.000000 quao-0.4.0.4/src/quao/data/response/__init__.py
+-rw-rw-rw-   0        0        0      268 2023-08-03 09:30:53.000000 quao-0.4.0.4/src/quao/data/response/authentication.py
+-rw-rw-rw-   0        0        0     1420 2023-08-08 02:05:29.000000 quao-0.4.0.4/src/quao/data/response/job_response.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.540748 quao-0.4.0.4/src/quao/enum/
+-rw-rw-rw-   0        0        0        0 2023-08-08 03:42:09.000000 quao-0.4.0.4/src/quao/enum/__init__.py
+-rw-rw-rw-   0        0        0      243 2023-08-08 05:03:57.000000 quao-0.4.0.4/src/quao/enum/http_header.py
+-rw-rw-rw-   0        0        0      230 2023-08-08 04:21:37.000000 quao-0.4.0.4/src/quao/enum/invocation_step.py
+-rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.4.0.4/src/quao/enum/media_type.py
+-rw-rw-rw-   0        0        0      205 2023-06-22 02:52:41.000000 quao-0.4.0.4/src/quao/enum/processing_unit.py
+-rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.4.0.4/src/quao/enum/provider_type.py
+-rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.4.0.4/src/quao/enum/sdk.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.544748 quao-0.4.0.4/src/quao/enum/status/
+-rw-rw-rw-   0        0        0        0 2023-08-08 03:42:12.000000 quao-0.4.0.4/src/quao/enum/status/__init__.py
+-rw-rw-rw-   0        0        0      213 2023-08-07 09:37:04.000000 quao-0.4.0.4/src/quao/enum/status/job_status.py
+-rw-rw-rw-   0        0        0      213 2023-08-07 09:37:04.000000 quao-0.4.0.4/src/quao/enum/status/status_code.py
+-rw-rw-rw-   0        0        0      169 2023-06-22 02:52:41.000000 quao-0.4.0.4/src/quao/enum/token_type.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.547748 quao-0.4.0.4/src/quao/factory/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.4/src/quao/factory/__init__.py
+-rw-rw-rw-   0        0        0     1895 2023-08-07 02:50:02.000000 quao-0.4.0.4/src/quao/factory/device_factory.py
+-rw-rw-rw-   0        0        0      539 2023-08-07 01:08:23.000000 quao-0.4.0.4/src/quao/factory/handler_factory.py
+-rw-rw-rw-   0        0        0     1396 2023-08-07 01:08:23.000000 quao-0.4.0.4/src/quao/factory/provider_factory.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.550746 quao-0.4.0.4/src/quao/handler/
+-rw-rw-rw-   0        0        0        0 2023-08-02 07:11:24.000000 quao-0.4.0.4/src/quao/handler/__init__.py
+-rw-rw-rw-   0        0        0      197 2023-08-04 01:32:03.000000 quao-0.4.0.4/src/quao/handler/handler.py
+-rw-rw-rw-   0        0        0     1360 2023-08-08 01:08:42.000000 quao-0.4.0.4/src/quao/handler/invocation_handler.py
+-rw-rw-rw-   0        0        0     7252 2023-08-08 02:48:14.000000 quao-0.4.0.4/src/quao/handler/job_fetching_handler.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.551748 quao-0.4.0.4/src/quao/model/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.4/src/quao/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.557748 quao-0.4.0.4/src/quao/model/device/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.4/src/quao/model/device/__init__.py
+-rw-rw-rw-   0        0        0     2419 2023-08-08 03:34:32.000000 quao-0.4.0.4/src/quao/model/device/aws_braket_device.py
+-rw-rw-rw-   0        0        0     7856 2023-08-08 02:20:30.000000 quao-0.4.0.4/src/quao/model/device/device.py
+-rw-rw-rw-   0        0        0      976 2023-08-07 02:49:49.000000 quao-0.4.0.4/src/quao/model/device/ibm_cloud_device.py
+-rw-rw-rw-   0        0        0      735 2023-08-07 02:49:49.000000 quao-0.4.0.4/src/quao/model/device/ibm_quantum_device.py
+-rw-rw-rw-   0        0        0     1239 2023-08-03 10:12:12.000000 quao-0.4.0.4/src/quao/model/device/qiskit_device.py
+-rw-rw-rw-   0        0        0     3526 2023-08-08 04:16:49.000000 quao-0.4.0.4/src/quao/model/device/quao_device.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.563749 quao-0.4.0.4/src/quao/model/provider/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.4/src/quao/model/provider/__init__.py
+-rw-rw-rw-   0        0        0     1251 2023-06-29 09:59:18.000000 quao-0.4.0.4/src/quao/model/provider/aws_braket_provider.py
+-rw-rw-rw-   0        0        0     1004 2023-06-29 09:59:18.000000 quao-0.4.0.4/src/quao/model/provider/ibm_cloud_provider.py
+-rw-rw-rw-   0        0        0      874 2023-06-29 09:59:18.000000 quao-0.4.0.4/src/quao/model/provider/ibm_quantum_provider.py
+-rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.4.0.4/src/quao/model/provider/provider.py
+-rw-rw-rw-   0        0        0     1397 2023-06-29 09:59:18.000000 quao-0.4.0.4/src/quao/model/provider/quao_provider.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.570748 quao-0.4.0.4/src/quao/util/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.4.0.4/src/quao/util/__init__.py
+-rw-rw-rw-   0        0        0     1058 2023-08-04 04:10:07.000000 quao-0.4.0.4/src/quao/util/circuit_utils.py
+-rw-rw-rw-   0        0        0      645 2023-08-08 06:39:49.000000 quao-0.4.0.4/src/quao/util/http_utils.py
+-rw-rw-rw-   0        0        0      417 2023-08-07 09:11:31.000000 quao-0.4.0.4/src/quao/util/job_status_mapping_utils.py
+-rw-rw-rw-   0        0        0     2322 2023-08-02 07:11:24.000000 quao-0.4.0.4/src/quao/util/json_parser_utils.py
+-rw-rw-rw-   0        0        0     1620 2023-08-08 06:41:16.000000 quao-0.4.0.4/src/quao/util/response_utils.py
+-rw-rw-rw-   0        0        0      890 2023-08-08 04:21:48.000000 quao-0.4.0.4/src/quao/util/status_code_mapping_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-08 06:41:32.506749 quao-0.4.0.4/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2841 2023-08-08 06:41:32.000000 quao-0.4.0.4/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2771 2023-08-08 06:41:32.000000 quao-0.4.0.4/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 06:41:32.000000 quao-0.4.0.4/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      190 2023-08-08 06:41:32.000000 quao-0.4.0.4/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-08 06:41:32.000000 quao-0.4.0.4/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.4.0.3/LICENSE` & `quao-0.4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/PKG-INFO` & `quao-0.4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.4.0.3
+Version: 0.4.0.4
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.4.0.3/README.md` & `quao-0.4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/pyproject.toml` & `quao-0.4.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.4.0.3"
+version = "0.4.0.4"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `quao-0.4.0.3/src/quao/async_tasks/export_circuit_task.py` & `quao-0.4.0.4/src/quao/async_tasks/export_circuit_task.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/async_tasks/post_processing_task.py` & `quao-0.4.0.4/src/quao/async_tasks/post_processing_task.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/component/backend/backend.py` & `quao-0.4.0.4/src/quao/component/backend/backend.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/component/callback/update_job_metadata.py` & `quao-0.4.0.4/src/quao/component/callback/update_job_metadata.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/component/device/device_selection.py` & `quao-0.4.0.4/src/quao/component/device/device_selection.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/data/request/invocation_request.py` & `quao-0.4.0.4/src/quao/data/request/invocation_request.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/data/request/request.py` & `quao-0.4.0.4/src/quao/data/request/request.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/data/response/job_response.py` & `quao-0.4.0.4/src/quao/data/response/job_response.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/factory/device_factory.py` & `quao-0.4.0.4/src/quao/factory/device_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/factory/handler_factory.py` & `quao-0.4.0.4/src/quao/factory/handler_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/factory/provider_factory.py` & `quao-0.4.0.4/src/quao/factory/provider_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/handler/invocation_handler.py` & `quao-0.4.0.4/src/quao/handler/invocation_handler.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/handler/job_fetching_handler.py` & `quao-0.4.0.4/src/quao/handler/job_fetching_handler.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/model/device/aws_braket_device.py` & `quao-0.4.0.4/src/quao/model/device/aws_braket_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/model/device/device.py` & `quao-0.4.0.4/src/quao/model/device/device.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/model/device/ibm_cloud_device.py` & `quao-0.4.0.4/src/quao/model/device/ibm_cloud_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/model/device/ibm_quantum_device.py` & `quao-0.4.0.4/src/quao/model/device/ibm_quantum_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/model/device/qiskit_device.py` & `quao-0.4.0.4/src/quao/model/device/qiskit_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/model/device/quao_device.py` & `quao-0.4.0.4/src/quao/model/device/quao_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/model/provider/aws_braket_provider.py` & `quao-0.4.0.4/src/quao/model/provider/aws_braket_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/model/provider/ibm_cloud_provider.py` & `quao-0.4.0.4/src/quao/model/provider/ibm_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/model/provider/ibm_quantum_provider.py` & `quao-0.4.0.4/src/quao/model/provider/ibm_quantum_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/model/provider/provider.py` & `quao-0.4.0.4/src/quao/model/provider/provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/model/provider/quao_provider.py` & `quao-0.4.0.4/src/quao/model/provider/quao_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/util/circuit_utils.py` & `quao-0.4.0.4/src/quao/util/circuit_utils.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/util/http_utils.py` & `quao-0.4.0.4/src/quao/util/http_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 
     @staticmethod
     def create_application_json_header(token):
         return {
             HttpHeader.AUTHORIZATION.value: TokenType.BEARER.value + ' ' + token,
             HttpHeader.CONTENT_TYPE.value: MediaType.APPLICATION_JSON.value,
             HttpHeader.ACCEPT.value: MediaType.APPLICATION_JSON.value
-        }
+        }
```

### Comparing `quao-0.4.0.3/src/quao/util/json_parser_utils.py` & `quao-0.4.0.4/src/quao/util/json_parser_utils.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao/util/response_utils.py` & `quao-0.4.0.4/src/quao/util/response_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             }
 
             mapping_key = job_response.invocation_step \
                 if JobStatusMappingUtils.resolve_job_status(job_response.job_status) is None \
                 else job_response.job_status
 
             response = {
-                "statusCode": StatusCodeMappingUtils.resolve_status_code(mapping_key),
+                "statusCode": StatusCodeMappingUtils.resolve_status_code(mapping_key).value,
                 "body": job_dict,
                 "userIdentity": job_response.user_identity,
                 "userToken": job_response.user_token
             }
 
         else:
             response = {
```

### Comparing `quao-0.4.0.3/src/quao/util/status_code_mapping_utils.py` & `quao-0.4.0.4/src/quao/util/status_code_mapping_utils.py`

 * *Files identical despite different names*

### Comparing `quao-0.4.0.3/src/quao.egg-info/PKG-INFO` & `quao-0.4.0.4/src/quao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.4.0.3
+Version: 0.4.0.4
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.4.0.3/src/quao.egg-info/SOURCES.txt` & `quao-0.4.0.4/src/quao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

