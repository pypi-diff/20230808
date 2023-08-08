# Comparing `tmp/je_web_runner_dev-0.0.80.tar.gz` & `tmp/je_web_runner_dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_web_runner_dev-0.0.80.tar", last modified: Tue Aug  8 06:58:21 2023, max compression
+gzip compressed data, was "dist\je_web_runner_dev-0.0.9.tar", last modified: Sun May 15 14:01:03 2022, max compression
```

## Comparing `je_web_runner_dev-0.0.80.tar` & `je_web_runner_dev-0.0.9.tar`

### file list

```diff
@@ -1,104 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.438090 je_web_runner_dev-0.0.80/
--rw-rw-rw-   0        0        0     1090 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/LICENSE
--rw-rw-rw-   0        0        0     3244 2023-08-08 06:58:21.438090 je_web_runner_dev-0.0.80/PKG-INFO
--rw-rw-rw-   0        0        0     2422 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/README.md
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.390460 je_web_runner_dev-0.0.80/je_web_runner/
--rw-rw-rw-   0        0        0     3303 2023-07-17 14:30:44.000000 je_web_runner_dev-0.0.80/je_web_runner/__init__.py
--rw-rw-rw-   0        0        0     1938 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/__main__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.391476 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/
--rw-rw-rw-   0        0        0        2 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.392455 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/element/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/element/__init__.py
--rw-rw-rw-   0        0        0    10295 2023-06-22 10:31:25.000000 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/element/web_element_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.393454 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/manager/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/manager/__init__.py
--rw-rw-rw-   0        0        0     6004 2023-06-22 10:31:25.000000 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/manager/webrunner_manager.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.393454 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/utils/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.394608 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/utils/selenium_utils_wrapper/
--rw-rw-rw-   0        0        0       72 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/utils/selenium_utils_wrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.395612 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/utils/selenium_utils_wrapper/desired_capabilities/
--rw-rw-rw-   0        0        0        2 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/utils/selenium_utils_wrapper/desired_capabilities/__init__.py
--rw-rw-rw-   0        0        0     1329 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/utils/selenium_utils_wrapper/desired_capabilities/desired_capabilities.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.396614 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/utils/selenium_utils_wrapper/keys/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/utils/selenium_utils_wrapper/keys/__init__.py
--rw-rw-rw-   0        0        0       64 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/utils/selenium_utils_wrapper/keys/selenium_keys.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.398613 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/webdriver/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/webdriver/__init__.py
--rw-rw-rw-   0        0        0     4371 2023-06-22 10:31:25.000000 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/webdriver/webdriver_with_options.py
--rw-rw-rw-   0        0        0    68213 2023-08-08 06:49:58.000000 je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/webdriver/webdriver_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.399613 je_web_runner_dev-0.0.80/je_web_runner/utils/
--rw-rw-rw-   0        0        0        2 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.400614 je_web_runner_dev-0.0.80/je_web_runner/utils/assert_value/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/assert_value/__init__.py
--rw-rw-rw-   0        0        0     5346 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/assert_value/result_check.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.402630 je_web_runner_dev-0.0.80/je_web_runner/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     9585 2023-07-17 14:02:28.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.404539 je_web_runner_dev-0.0.80/je_web_runner/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1227 2023-07-17 13:43:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      971 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.405544 je_web_runner_dev-0.0.80/je_web_runner/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/executor/__init__.py
--rw-rw-rw-   0        0        0    14048 2023-08-08 05:46:01.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.406544 je_web_runner_dev-0.0.80/je_web_runner/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      739 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.409570 je_web_runner_dev-0.0.80/je_web_runner/utils/generate_report/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/generate_report/__init__.py
--rw-rw-rw-   0        0        0     5075 2023-07-17 14:30:51.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/generate_report/generate_html_report.py
--rw-rw-rw-   0        0        0     3291 2023-07-17 14:30:57.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/generate_report/generate_json_report.py
--rw-rw-rw-   0        0        0     1981 2023-07-17 14:30:59.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/generate_report/generate_xml_report.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.409570 je_web_runner_dev-0.0.80/je_web_runner/utils/json/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/json/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.410545 je_web_runner_dev-0.0.80/je_web_runner/utils/json/json_file/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/json/json_file/__init__.py
--rw-rw-rw-   0        0        0     1288 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/json/json_file/json_file.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.412546 je_web_runner_dev-0.0.80/je_web_runner/utils/json/json_format/
--rw-rw-rw-   0        0        0        2 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/json/json_format/__init__.py
--rw-rw-rw-   0        0        0     1247 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/json/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.413545 je_web_runner_dev-0.0.80/je_web_runner/utils/logging/
--rw-rw-rw-   0        0        0        0 2023-06-22 10:31:25.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/logging/__init__.py
--rw-rw-rw-   0        0        0      586 2023-08-03 09:12:52.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/logging/loggin_instance.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.414574 je_web_runner_dev-0.0.80/je_web_runner/utils/package_manager/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/package_manager/__init__.py
--rw-rw-rw-   0        0        0     3542 2023-06-22 10:31:25.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.415545 je_web_runner_dev-0.0.80/je_web_runner/utils/project/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/project/__init__.py
--rw-rw-rw-   0        0        0     3120 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/project/create_project_structure.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.417543 je_web_runner_dev-0.0.80/je_web_runner/utils/project/template/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/project/template/__init__.py
--rw-rw-rw-   0        0        0      633 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/project/template/template_executor.py
--rw-rw-rw-   0        0        0      911 2023-07-17 14:02:28.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/project/template/template_keyword.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.418544 je_web_runner_dev-0.0.80/je_web_runner/utils/scheduler/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/scheduler/__init__.py
--rw-rw-rw-   0        0        0    11468 2023-07-17 14:02:22.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/scheduler/extend_apscheduler.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.419551 je_web_runner_dev-0.0.80/je_web_runner/utils/socket_server/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/socket_server/__init__.py
--rw-rw-rw-   0        0        0     2248 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/socket_server/web_runner_socket_server.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.420553 je_web_runner_dev-0.0.80/je_web_runner/utils/test_object/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/test_object/__init__.py
--rw-rw-rw-   0        0        0      968 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/test_object/test_object_class.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.421556 je_web_runner_dev-0.0.80/je_web_runner/utils/test_object/test_object_record/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/test_object/test_object_record/__init__.py
--rw-rw-rw-   0        0        0      739 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/test_object/test_object_record/test_object_record_class.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.423549 je_web_runner_dev-0.0.80/je_web_runner/utils/test_record/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0     1283 2023-06-22 10:31:25.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/test_record/test_record_class.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.423549 je_web_runner_dev-0.0.80/je_web_runner/utils/xml/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/xml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.424549 je_web_runner_dev-0.0.80/je_web_runner/utils/xml/change_xml_structure/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/xml/change_xml_structure/__init__.py
--rw-rw-rw-   0        0        0     2498 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/xml/change_xml_structure/change_xml_structure.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.425549 je_web_runner_dev-0.0.80/je_web_runner/utils/xml/xml_file/
--rw-rw-rw-   0        0        0        0 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/xml/xml_file/__init__.py
--rw-rw-rw-   0        0        0     2361 2023-06-22 08:52:10.000000 je_web_runner_dev-0.0.80/je_web_runner/utils/xml/xml_file/xml_file.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:58:21.437088 je_web_runner_dev-0.0.80/je_web_runner_dev.egg-info/
--rw-rw-rw-   0        0        0     3244 2023-08-08 06:58:21.000000 je_web_runner_dev-0.0.80/je_web_runner_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3428 2023-08-08 06:58:21.000000 je_web_runner_dev-0.0.80/je_web_runner_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 06:58:21.000000 je_web_runner_dev-0.0.80/je_web_runner_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-08-08 06:58:21.000000 je_web_runner_dev-0.0.80/je_web_runner_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-08-08 06:58:21.000000 je_web_runner_dev-0.0.80/je_web_runner_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1233 2023-08-08 06:58:08.000000 je_web_runner_dev-0.0.80/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-08 06:58:21.438090 je_web_runner_dev-0.0.80/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2022-05-06 19:45:56.000000 je_web_runner_dev-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      712 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       70 2022-05-06 19:45:56.000000 je_web_runner_dev-0.0.9/README.md
+-rw-rw-rw-   0        0        0      980 2022-05-15 14:01:01.000000 je_web_runner_dev-0.0.9/dev_setup.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:02.000000 je_web_runner_dev-0.0.9/je_web_runner/
+-rw-rw-rw-   0        0        0      995 2022-05-14 03:49:03.000000 je_web_runner_dev-0.0.9/je_web_runner/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-05-08 23:05:18.000000 je_web_runner_dev-0.0.9/je_web_runner/__main__.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:02.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_utils_wrapper/
+-rw-rw-rw-   0        0        0       52 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_utils_wrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_utils_wrapper/desired_capabilities/
+-rw-rw-rw-   0        0        0       73 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_utils_wrapper/desired_capabilities/__init__.py
+-rw-rw-rw-   0        0        0      855 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_utils_wrapper/desired_capabilities/desired_capabilities.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_wrapper/
+-rw-rw-rw-   0        0        0       46 2022-05-10 14:12:01.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     1513 2022-05-14 18:47:14.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_wrapper/web_element_wrapper.py
+-rw-rw-rw-   0        0        0     1831 2022-05-14 19:44:19.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_wrapper/webdriver_manager.py
+-rw-rw-rw-   0        0        0     2081 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_wrapper/webdriver_with_options.py
+-rw-rw-rw-   0        0        0     8213 2022-05-14 20:07:26.000000 je_web_runner_dev-0.0.9/je_web_runner/selenium_wrapper/webdriver_wrapper.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/
+-rw-rw-rw-   0        0        0       35 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/assert_value/
+-rw-rw-rw-   0        0        0        0 2022-05-08 22:50:02.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/assert_value/__init__.py
+-rw-rw-rw-   0        0        0     2793 2022-05-14 03:52:14.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/assert_value/result_check.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/exception/
+-rw-rw-rw-   0        0        0       45 2022-05-07 17:33:02.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      698 2022-05-09 03:28:45.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/exception/exception_tag.py
+-rw-rw-rw-   0        0        0      512 2022-05-13 15:16:15.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/executor/
+-rw-rw-rw-   0        0        0        0 2022-05-08 22:59:45.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     2821 2022-05-14 02:44:04.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/executor/executor.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0      298 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/file_process/create_project_structure.py
+-rw-rw-rw-   0        0        0      711 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/json/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/json/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/json/json_file/
+-rw-rw-rw-   0        0        0        0 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/json/json_file/__init__.py
+-rw-rw-rw-   0        0        0     1271 2022-05-09 03:28:46.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/json/json_file/json_file.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/json/json_format/
+-rw-rw-rw-   0        0        0        2 2022-05-06 19:46:48.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/json/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1094 2022-05-09 03:29:42.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/json/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_object/
+-rw-rw-rw-   0        0        0        0 2022-05-13 21:15:19.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_object/__init__.py
+-rw-rw-rw-   0        0        0      656 2022-05-11 07:54:28.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_object/test_object_class.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_object/test_object_record/
+-rw-rw-rw-   0        0        0        0 2022-05-08 22:49:43.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_object/test_object_record/__init__.py
+-rw-rw-rw-   0        0        0      549 2022-05-13 21:16:22.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_object/test_object_record/test_object_record_class.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_record/
+-rw-rw-rw-   0        0        0        0 2022-05-08 23:22:33.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_record/__init__.py
+-rw-rw-rw-   0        0        0      197 2022-05-08 23:44:10.000000 je_web_runner_dev-0.0.9/je_web_runner/utils/test_record/test_record.py
+drwxrwxrwx   0        0        0        0 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/je_web_runner_dev.egg-info/
+-rw-rw-rw-   0        0        0      712 2022-05-15 14:01:02.000000 je_web_runner_dev-0.0.9/je_web_runner_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1819 2022-05-15 14:01:02.000000 je_web_runner_dev-0.0.9/je_web_runner_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-15 14:01:02.000000 je_web_runner_dev-0.0.9/je_web_runner_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2022-05-15 14:01:02.000000 je_web_runner_dev-0.0.9/je_web_runner_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2022-05-15 14:01:02.000000 je_web_runner_dev-0.0.9/je_web_runner_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-05-15 14:01:03.000000 je_web_runner_dev-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      972 2022-05-13 20:58:08.000000 je_web_runner_dev-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `je_web_runner_dev-0.0.80/LICENSE` & `je_web_runner_dev-0.0.9/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021~2023 JE-Chen
+Copyright (c) 2021 JE-Chen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `je_web_runner_dev-0.0.80/je_web_runner/__main__.py` & `je_web_runner_dev-0.0.9/je_web_runner/utils/executor/executor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,76 @@
-# argparse
-import argparse
-import json
-import sys
+from sys import stderr
 
-from je_web_runner.utils.exception.exception_tags import argparse_get_wrong_data
+from je_web_runner.utils.exception.exception_tag import executor_data_error, executor_list_error
 from je_web_runner.utils.exception.exceptions import WebRunnerExecuteException
-from je_web_runner.utils.executor.action_executor import execute_action
-from je_web_runner.utils.executor.action_executor import execute_files
-from je_web_runner.utils.file_process.get_dir_file_list import get_dir_files_as_list
 from je_web_runner.utils.json.json_file.json_file import read_action_json
+from je_web_runner.utils.test_object.test_object_record.test_object_record_class import test_object_record
+from je_web_runner.selenium_wrapper.webdriver_manager import web_runner
 
-if __name__ == "__main__":
+event_dict = {
+    # webdriver manager
+    "get_webdriver_manager": web_runner.new_driver,
+    "change_index_of_webdriver": web_runner.change_webdriver,
+    "quit": web_runner.quit,
+    # test object
+    "SaveTestObject": test_object_record.save_test_object,
+    "CleanTestObject": test_object_record.clean_record,
+    # webdriver wrapper
+    "to_url": web_runner.webdriver_wrapper.to_url,
+    "implicitly_wait": web_runner.webdriver_wrapper.wait_implicitly,
+    "find_element": web_runner.webdriver_wrapper.find_element_with_test_object_record,
+    "find_elements": web_runner.webdriver_wrapper.find_elements_with_test_object_record,
+    # web element
+    "input_to_element": web_runner.webdriver_element.input_to_element,
+    "click_element": web_runner.webdriver_element.click_element,
+
+}
+
+
+def execute_event(action: list):
+    """
+    :param action: execute action
+    :return: what event return
+    """
+    event = event_dict.get(action[0])
+    if len(action) == 2:
+        return event(**action[1])
+    elif len(action) == 1:
+        event()
+    else:
+        raise WebRunnerExecuteException(executor_data_error)
+
+
+def execute_action(action_list: list):
+    """
+    :param action_list: like this structure
+    [
+
+    ]
+    for loop and use execute_event function to execute
+    :return: recode string, response as list
+    """
+    execute_record_string = ""
+    event_response_list = []
     try:
-        def preprocess_execute_action(file_path: str):
-            execute_action(read_action_json(file_path))
-
-
-        def preprocess_execute_files(file_path: str):
-            execute_files(get_dir_files_as_list(file_path))
+        if len(action_list) > 0 or type(action_list) is not list:
+            for action in action_list:
+                event_response = execute_event(action)
+                print("execute: ", str(action))
+                execute_record_string = "".join(execute_record_string)
+                event_response_list.append(event_response)
+        else:
+            raise WebRunnerExecuteException(executor_list_error)
+        return execute_record_string, event_response_list
+    except Exception as error:
+        print(repr(error), file=stderr)
 
 
-        def preprocess_read_str_execute_action(execute_str: str):
-            execute_str = json.loads(execute_str)
-            execute_action(execute_str)
-
-
-        argparse_event_dict = {
-            "execute_file": preprocess_execute_action,
-            "execute_dir": preprocess_execute_files,
-            "execute_str": preprocess_read_str_execute_action
-        }
-        parser = argparse.ArgumentParser()
-        parser.add_argument("-e", "--execute_file", type=str, help="choose action file to execute")
-        parser.add_argument("-d", "--execute_dir", type=str, help="choose dir include action file to execute")
-        parser.add_argument("--execute_str", type=str, help="execute json str")
-        args = parser.parse_args()
-        args = vars(args)
-        for key, value in args.items():
-            if value is not None:
-                argparse_event_dict.get(key)(value)
-        if all(value is None for value in args.values()):
-            raise WebRunnerExecuteException(argparse_get_wrong_data)
-    except Exception as error:
-        print(repr(error), file=sys.stderr)
-        sys.exit(1)
+def execute_files(execute_files_list: list):
+    """
+    :param execute_files_list: list include execute files path
+    :return: every execute detail as list
+    """
+    execute_detail_list = list()
+    for file in execute_files_list:
+        execute_detail_list.append(execute_action(read_action_json(file)))
+    return execute_detail_list
```

### Comparing `je_web_runner_dev-0.0.80/je_web_runner/je_web_runner/utils/selenium_utils_wrapper/desired_capabilities/desired_capabilities.py` & `je_web_runner_dev-0.0.9/je_web_runner/selenium_utils_wrapper/desired_capabilities/desired_capabilities.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,26 @@
-from typing import Any, Union
-
 from selenium.webdriver import DesiredCapabilities
 
-from je_web_runner.utils.exception.exception_tags import selenium_wrapper_web_driver_not_found_error
-from je_web_runner.utils.exception.exceptions import WebRunnerException
+from je_web_runner.utils.exception.exceptions import WebDriverException
+from je_web_runner.utils.exception.exception_tag import selenium_wrapper_web_driver_not_found_error
+
 
 desired_capabilities_dict = {
     "firefox": DesiredCapabilities.FIREFOX,
     "chrome": DesiredCapabilities.CHROME,
     "edge": DesiredCapabilities.EDGE,
+    "opera": DesiredCapabilities.OPERA,
     "safari": DesiredCapabilities.SAFARI,
 }
 
 
-def get_desired_capabilities_keys() -> Union[str, Any]:
-    """
-    :return: return all webdriver you can get desired capabilities
-    """
+def get_desired_capabilities_keys():
     return desired_capabilities_dict.keys()
 
 
-def get_desired_capabilities(webdriver_name: str) -> \
-        [
-            DesiredCapabilities.FIREFOX.copy(),
-            DesiredCapabilities.CHROME.copy(),
-            DesiredCapabilities.EDGE.copy(),
-            DesiredCapabilities.SAFARI.copy(),
-        ]:
-    """
-    choose webdriver to get desired capabilities
-    :param webdriver_name: name to get desired capabilities
-    :return: desired capabilities
-    """
+def get_desired_capabilities(webdriver_name: str):
     desired_capabilities = desired_capabilities_dict.get(webdriver_name)
     if desired_capabilities is None:
-        raise WebRunnerException(selenium_wrapper_web_driver_not_found_error)
+        raise WebDriverException(selenium_wrapper_web_driver_not_found_error)
     return desired_capabilities.copy()
+
+
```

### Comparing `je_web_runner_dev-0.0.80/je_web_runner/utils/file_process/get_dir_file_list.py` & `je_web_runner_dev-0.0.9/je_web_runner/utils/file_process/get_dir_file_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from os import getcwd
 from os import walk
+from os import getcwd
 from os.path import abspath
 from os.path import join
-from typing import List
 
 
-def get_dir_files_as_list(dir_path: str = getcwd(), default_search_file_extension: str = ".json") -> List[str]:
+def get_dir_files_as_list(dir_path: str = getcwd(), default_search_file_extension: str = ".json") -> list:
     """
     get dir file when end with default_search_file_extension
     :param dir_path: which dir we want to walk and get file list
     :param default_search_file_extension: which extension we want to search
     :return: [] if nothing searched or [file1, file2.... files] file was searched
     """
     return [
         abspath(join(dir_path, file)) for root, dirs, files in walk(dir_path)
         for file in files
         if file.endswith(default_search_file_extension.lower())
     ]
+
```

### Comparing `je_web_runner_dev-0.0.80/je_web_runner/utils/json/json_file/json_file.py` & `je_web_runner_dev-0.0.9/je_web_runner/utils/json/json_file/json_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 from pathlib import Path
 from threading import Lock
 
-from je_web_runner.utils.exception.exception_tags import cant_find_json_error, cant_save_json_error
+from je_web_runner.utils.exception.exception_tag import cant_find_json_error, cant_save_json_error
 from je_web_runner.utils.exception.exceptions import WebRunnerJsonException
 
 lock = Lock()
 
 
-def read_action_json(json_file_path: str) -> list:
+def read_action_json(json_file_path: str):
     """
     read the action json
     :param json_file_path json file's path to read
     """
     try:
         lock.acquire()
         file_path = Path(json_file_path)
@@ -30,12 +30,13 @@
     write action json
     :param json_save_path  json save path
     :param action_json the json str include action to write
     """
     try:
         lock.acquire()
         with open(json_save_path, "w+") as file_to_write:
-            file_to_write.write(json.dumps(action_json, indent=4))
+            file_to_write.write(json.dumps(action_json))
     except WebRunnerJsonException:
         raise WebRunnerJsonException(cant_save_json_error)
     finally:
         lock.release()
+
```

### Comparing `je_web_runner_dev-0.0.80/je_web_runner/utils/json/json_format/json_process.py` & `je_web_runner_dev-0.0.9/je_web_runner/utils/json/json_format/json_process.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json.decoder
 import sys
 from json import dumps
 from json import loads
 
-from je_web_runner.utils.exception.exception_tags import wrong_json_data_error, cant_reformat_json_error
+from je_web_runner.utils.exception.exception_tag import wrong_json_data_error, cant_reformat_json_error
 from je_web_runner.utils.exception.exceptions import WebRunnerJsonException
 
 
-def __process_json(json_string: str, **kwargs) -> str:
+def __process_json(json_string: str, **kwargs):
     """
     :param json_string: full json str (not json type)
     :param kwargs: any another kwargs for dumps
     :return: reformat str
     """
     try:
         return dumps(loads(json_string), indent=4, sort_keys=True, **kwargs)
@@ -21,17 +21,12 @@
     except TypeError:
         try:
             return dumps(json_string, indent=4, sort_keys=True, **kwargs)
         except TypeError:
             raise WebRunnerJsonException(wrong_json_data_error)
 
 
-def reformat_json(json_string: str, **kwargs) -> str:
-    """
-    :param json_string: Valid json string
-    :param kwargs: __process_json params
-    :return: reformat json string
-    """
+def reformat_json(json_string: str, **kwargs):
     try:
         return __process_json(json_string, **kwargs)
     except WebRunnerJsonException:
         raise WebRunnerJsonException(cant_reformat_json_error)
```

### Comparing `je_web_runner_dev-0.0.80/je_web_runner/utils/test_object/test_object_record/test_object_record_class.py` & `je_web_runner_dev-0.0.9/je_web_runner/utils/test_object/test_object_record/test_object_record_class.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-from typing import Any
-
 from je_web_runner.utils.test_object.test_object_class import TestObject
 
 
 class TestObjectRecord(object):
 
     def __init__(self):
         self.test_object_record_dict = dict()
 
-    def clean_record(self) -> None:
+    def clean_record(self):
         self.test_object_record_dict = dict()
 
-    def save_test_object(self, test_object_name: str, object_type: str = None, **kwargs) -> None:
+    def save_test_object(self, test_object_name: str, object_type=None, **kwargs):
         test_object = TestObject(test_object_name, object_type)
         self.test_object_record_dict.update({test_object.test_object_name: test_object})
 
-    def remove_test_object(self, test_object_name: str) -> Any:
-        return self.test_object_record_dict.pop(test_object_name, False)
-
 
 test_object_record = TestObjectRecord()
```

