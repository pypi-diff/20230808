# Comparing `tmp/ha-services-0.3.2.tar.gz` & `tmp/ha-services-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ha-services-0.3.2.tar", last modified: Sun May 21 09:32:56 2023, max compression
+gzip compressed data, was "ha-services-0.3.3.tar", last modified: Tue Aug  8 16:13:16 2023, max compression
```

## Comparing `ha-services-0.3.2.tar` & `ha-services-0.3.3.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.669398 ha-services-0.3.2/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-05-09 16:39:25.000000 ha-services-0.3.2/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-05-09 16:39:25.000000 ha-services-0.3.2/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.665398 ha-services-0.3.2/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.665398 ha-services-0.3.2/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-09 16:39:25.000000 ha-services-0.3.2/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-05-09 16:39:25.000000 ha-services-0.3.2/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)     6951 2023-05-21 09:32:56.669398 ha-services-0.3.2/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     6538 2023-05-18 14:20:06.000000 ha-services-0.3.2/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-11 18:48:55.000000 ha-services-0.3.2/cli.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-09 16:39:25.000000 ha-services-0.3.2/dev-cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.665398 ha-services-0.3.2/ha_services/
--rw-rw-r--   0 jens      (1000) users      (100)      165 2023-05-21 09:30:45.000000 ha-services-0.3.2/ha_services/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      195 2023-05-09 16:39:25.000000 ha-services-0.3.2/ha_services/__main__.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.669398 ha-services-0.3.2/ha_services/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.3.2/ha_services/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     8352 2023-05-19 19:35:24.000000 ha-services-0.3.2/ha_services/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)     7184 2023-05-19 19:56:41.000000 ha-services-0.3.2/ha_services/cli/dev.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.669398 ha-services-0.3.2/ha_services/cli_tools/
--rw-rw-r--   0 jens      (1000) users      (100)      120 2023-05-11 06:15:16.000000 ha-services-0.3.2/ha_services/cli_tools/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1445 2023-05-19 19:49:27.000000 ha-services-0.3.2/ha_services/cli_tools/dev_tools.py
--rw-rw-r--   0 jens      (1000) users      (100)     1364 2023-05-18 05:57:33.000000 ha-services-0.3.2/ha_services/cli_tools/dict_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     2529 2023-05-11 17:34:50.000000 ha-services-0.3.2/ha_services/cli_tools/path_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     3729 2023-05-11 20:05:42.000000 ha-services-0.3.2/ha_services/cli_tools/rich_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.669398 ha-services-0.3.2/ha_services/cli_tools/test_utils/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.3.2/ha_services/cli_tools/test_utils/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1048 2023-05-18 12:56:44.000000 ha-services-0.3.2/ha_services/cli_tools/test_utils/assertion.py
--rw-rw-r--   0 jens      (1000) users      (100)      911 2023-05-18 09:57:15.000000 ha-services-0.3.2/ha_services/cli_tools/test_utils/cli_readme.py
--rw-rw-r--   0 jens      (1000) users      (100)     1261 2023-05-18 04:14:32.000000 ha-services-0.3.2/ha_services/cli_tools/test_utils/environment_fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)     4932 2023-05-18 14:16:23.000000 ha-services-0.3.2/ha_services/cli_tools/test_utils/rich_test_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)      220 2023-05-20 10:46:47.000000 ha-services-0.3.2/ha_services/cli_tools/test_utils/shutil_mocks.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.669398 ha-services-0.3.2/ha_services/cli_tools/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.3.2/ha_services/cli_tools/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      432 2023-05-18 05:10:52.000000 ha-services-0.3.2/ha_services/cli_tools/tests/test_dict_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)      693 2023-05-11 07:38:00.000000 ha-services-0.3.2/ha_services/cli_tools/tests/test_environ_fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)     2220 2023-05-18 12:58:25.000000 ha-services-0.3.2/ha_services/cli_tools/tests/test_mock_rich.py
--rw-rw-r--   0 jens      (1000) users      (100)     1918 2023-05-11 07:37:29.000000 ha-services-0.3.2/ha_services/cli_tools/tests/test_path_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)      998 2023-05-19 19:18:58.000000 ha-services-0.3.2/ha_services/cli_tools/verbosity.py
--rw-rw-r--   0 jens      (1000) users      (100)      164 2023-05-09 16:59:30.000000 ha-services-0.3.2/ha_services/constants.py
--rw-rw-r--   0 jens      (1000) users      (100)     3448 2023-05-19 19:30:01.000000 ha-services-0.3.2/ha_services/example.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.669398 ha-services-0.3.2/ha_services/mqtt4homeassistant/
--rw-rw-r--   0 jens      (1000) users      (100)       22 2023-05-09 16:39:25.000000 ha-services-0.3.2/ha_services/mqtt4homeassistant/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1898 2023-05-09 16:39:25.000000 ha-services-0.3.2/ha_services/mqtt4homeassistant/converter.py
--rw-rw-r--   0 jens      (1000) users      (100)     1061 2023-05-09 16:39:25.000000 ha-services-0.3.2/ha_services/mqtt4homeassistant/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     4102 2023-05-19 19:30:59.000000 ha-services-0.3.2/ha_services/mqtt4homeassistant/mqtt.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.669398 ha-services-0.3.2/ha_services/mqtt4homeassistant/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.3.2/ha_services/mqtt4homeassistant/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2142 2023-05-09 16:39:25.000000 ha-services-0.3.2/ha_services/mqtt4homeassistant/tests/test_converter.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.669398 ha-services-0.3.2/ha_services/mqtt4homeassistant/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.3.2/ha_services/mqtt4homeassistant/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      315 2023-05-09 16:39:25.000000 ha-services-0.3.2/ha_services/mqtt4homeassistant/utilities/string_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.669398 ha-services-0.3.2/ha_services/systemd/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.3.2/ha_services/systemd/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     7684 2023-05-21 09:20:35.000000 ha-services-0.3.2/ha_services/systemd/api.py
--rw-rw-r--   0 jens      (1000) users      (100)     3441 2023-05-21 09:14:40.000000 ha-services-0.3.2/ha_services/systemd/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)      505 2023-05-10 07:16:49.000000 ha-services-0.3.2/ha_services/systemd/defaults.py
--rw-rw-r--   0 jens      (1000) users      (100)      104 2023-05-21 09:17:03.000000 ha-services-0.3.2/ha_services/systemd/exceptions.py
--rw-rw-r--   0 jens      (1000) users      (100)      320 2023-05-17 15:08:38.000000 ha-services-0.3.2/ha_services/systemd/service_template.txt
--rw-rw-r--   0 jens      (1000) users      (100)     1794 2023-05-09 19:43:34.000000 ha-services-0.3.2/ha_services/systemd/template.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.669398 ha-services-0.3.2/ha_services/systemd/test_utils/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-18 04:08:42.000000 ha-services-0.3.2/ha_services/systemd/test_utils/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2012 2023-05-18 05:54:08.000000 ha-services-0.3.2/ha_services/systemd/test_utils/mock_systemd_info.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.669398 ha-services-0.3.2/ha_services/systemd/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.3.2/ha_services/systemd/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     4801 2023-05-21 09:30:28.000000 ha-services-0.3.2/ha_services/systemd/tests/test_api.py
--rw-rw-r--   0 jens      (1000) users      (100)     1655 2023-05-21 09:20:38.000000 ha-services-0.3.2/ha_services/systemd/tests/test_data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     3000 2023-05-18 06:02:23.000000 ha-services-0.3.2/ha_services/systemd/tests/test_mock_systemd_info.py
--rw-rw-r--   0 jens      (1000) users      (100)      595 2023-05-18 06:01:09.000000 ha-services-0.3.2/ha_services/systemd/tests/test_mock_systemd_info_mock_1.snapshot.toml
--rw-rw-r--   0 jens      (1000) users      (100)     2471 2023-05-09 19:43:34.000000 ha-services-0.3.2/ha_services/systemd/tests/test_template.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.669398 ha-services-0.3.2/ha_services/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      296 2023-05-19 19:29:53.000000 ha-services-0.3.2/ha_services/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      217 2023-05-09 16:39:25.000000 ha-services-0.3.2/ha_services/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2579 2023-05-09 16:39:25.000000 ha-services-0.3.2/ha_services/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     2949 2023-05-18 14:20:00.000000 ha-services-0.3.2/ha_services/tests/test_readme.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.669398 ha-services-0.3.2/ha_services/toml_settings/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.3.2/ha_services/toml_settings/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     4234 2023-05-18 05:57:51.000000 ha-services-0.3.2/ha_services/toml_settings/api.py
--rw-rw-r--   0 jens      (1000) users      (100)      220 2023-05-09 20:53:17.000000 ha-services-0.3.2/ha_services/toml_settings/data_class_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     1352 2023-05-11 19:53:35.000000 ha-services-0.3.2/ha_services/toml_settings/debug.py
--rw-rw-r--   0 jens      (1000) users      (100)     3059 2023-05-09 20:53:17.000000 ha-services-0.3.2/ha_services/toml_settings/deserialize.py
--rw-rw-r--   0 jens      (1000) users      (100)       56 2023-05-09 16:39:25.000000 ha-services-0.3.2/ha_services/toml_settings/exceptions.py
--rw-rw-r--   0 jens      (1000) users      (100)      836 2023-05-20 10:50:56.000000 ha-services-0.3.2/ha_services/toml_settings/sensible_editor.py
--rw-rw-r--   0 jens      (1000) users      (100)     1847 2023-05-18 06:01:57.000000 ha-services-0.3.2/ha_services/toml_settings/serialize.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.669398 ha-services-0.3.2/ha_services/toml_settings/test_utils/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-18 05:26:41.000000 ha-services-0.3.2/ha_services/toml_settings/test_utils/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1153 2023-05-18 13:05:47.000000 ha-services-0.3.2/ha_services/toml_settings/test_utils/cli_mock.py
--rw-rw-r--   0 jens      (1000) users      (100)     3092 2023-05-18 08:32:52.000000 ha-services-0.3.2/ha_services/toml_settings/test_utils/data_class_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.669398 ha-services-0.3.2/ha_services/toml_settings/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.3.2/ha_services/toml_settings/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1383 2023-05-18 05:43:52.000000 ha-services-0.3.2/ha_services/toml_settings/tests/fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)     1044 2023-05-17 15:20:34.000000 ha-services-0.3.2/ha_services/toml_settings/tests/test_demo_settings.py
--rw-rw-r--   0 jens      (1000) users      (100)     5606 2023-05-18 06:01:57.000000 ha-services-0.3.2/ha_services/toml_settings/tests/test_deserialize.py
--rw-rw-r--   0 jens      (1000) users      (100)     1808 2023-05-20 10:49:05.000000 ha-services-0.3.2/ha_services/toml_settings/tests/test_sensible_editor.py
--rw-rw-r--   0 jens      (1000) users      (100)     3172 2023-05-18 05:24:56.000000 ha-services-0.3.2/ha_services/toml_settings/tests/test_serialize.py
--rw-rw-r--   0 jens      (1000) users      (100)     3205 2023-05-18 08:31:32.000000 ha-services-0.3.2/ha_services/toml_settings/tests/test_test_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-21 09:32:56.669398 ha-services-0.3.2/ha_services.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)     6951 2023-05-21 09:32:56.000000 ha-services-0.3.2/ha_services.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     3233 2023-05-21 09:32:56.000000 ha-services-0.3.2/ha_services.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-21 09:32:56.000000 ha-services-0.3.2/ha_services.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)      105 2023-05-21 09:32:56.000000 ha-services-0.3.2/ha_services.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      283 2023-05-21 09:32:56.000000 ha-services-0.3.2/ha_services.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)       12 2023-05-21 09:32:56.000000 ha-services-0.3.2/ha_services.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4934 2023-05-09 17:58:58.000000 ha-services-0.3.2/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    53004 2023-05-18 06:04:30.000000 ha-services-0.3.2/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)    22054 2023-05-18 06:04:13.000000 ha-services-0.3.2/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-21 09:32:56.669398 ha-services-0.3.2/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.023923 ha-services-0.3.3/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-05-09 16:39:25.000000 ha-services-0.3.3/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-05-09 16:39:25.000000 ha-services-0.3.3/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.019924 ha-services-0.3.3/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.019924 ha-services-0.3.3/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-09 16:39:25.000000 ha-services-0.3.3/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-05-09 16:39:25.000000 ha-services-0.3.3/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)     6951 2023-08-08 16:13:16.023923 ha-services-0.3.3/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     6538 2023-05-18 14:20:06.000000 ha-services-0.3.3/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-11 18:48:55.000000 ha-services-0.3.3/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-09 16:39:25.000000 ha-services-0.3.3/dev-cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.019924 ha-services-0.3.3/ha_services/
+-rw-rw-r--   0 jens      (1000) users      (100)      165 2023-08-08 16:05:41.000000 ha-services-0.3.3/ha_services/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      195 2023-05-09 16:39:25.000000 ha-services-0.3.3/ha_services/__main__.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.019924 ha-services-0.3.3/ha_services/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.3.3/ha_services/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     8352 2023-08-08 15:47:09.000000 ha-services-0.3.3/ha_services/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7184 2023-05-19 19:56:41.000000 ha-services-0.3.3/ha_services/cli/dev.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.019924 ha-services-0.3.3/ha_services/cli_tools/
+-rw-rw-r--   0 jens      (1000) users      (100)      120 2023-05-11 06:15:16.000000 ha-services-0.3.3/ha_services/cli_tools/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1445 2023-05-19 19:49:27.000000 ha-services-0.3.3/ha_services/cli_tools/dev_tools.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1364 2023-05-18 05:57:33.000000 ha-services-0.3.3/ha_services/cli_tools/dict_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2529 2023-05-11 17:34:50.000000 ha-services-0.3.3/ha_services/cli_tools/path_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3729 2023-05-11 20:05:42.000000 ha-services-0.3.3/ha_services/cli_tools/rich_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.019924 ha-services-0.3.3/ha_services/cli_tools/test_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.3.3/ha_services/cli_tools/test_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1048 2023-05-18 12:56:44.000000 ha-services-0.3.3/ha_services/cli_tools/test_utils/assertion.py
+-rw-rw-r--   0 jens      (1000) users      (100)      911 2023-05-18 09:57:15.000000 ha-services-0.3.3/ha_services/cli_tools/test_utils/cli_readme.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1261 2023-05-18 04:14:32.000000 ha-services-0.3.3/ha_services/cli_tools/test_utils/environment_fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4932 2023-05-18 14:16:23.000000 ha-services-0.3.3/ha_services/cli_tools/test_utils/rich_test_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)      220 2023-05-20 10:46:47.000000 ha-services-0.3.3/ha_services/cli_tools/test_utils/shutil_mocks.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.019924 ha-services-0.3.3/ha_services/cli_tools/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.3.3/ha_services/cli_tools/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      432 2023-05-18 05:10:52.000000 ha-services-0.3.3/ha_services/cli_tools/tests/test_dict_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)      693 2023-05-11 07:38:00.000000 ha-services-0.3.3/ha_services/cli_tools/tests/test_environ_fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2220 2023-05-18 12:58:25.000000 ha-services-0.3.3/ha_services/cli_tools/tests/test_mock_rich.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1918 2023-05-11 07:37:29.000000 ha-services-0.3.3/ha_services/cli_tools/tests/test_path_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)      998 2023-05-19 19:18:58.000000 ha-services-0.3.3/ha_services/cli_tools/verbosity.py
+-rw-rw-r--   0 jens      (1000) users      (100)      164 2023-05-09 16:59:30.000000 ha-services-0.3.3/ha_services/constants.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3448 2023-05-19 19:30:01.000000 ha-services-0.3.3/ha_services/example.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.019924 ha-services-0.3.3/ha_services/mqtt4homeassistant/
+-rw-rw-r--   0 jens      (1000) users      (100)       22 2023-05-09 16:39:25.000000 ha-services-0.3.3/ha_services/mqtt4homeassistant/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1898 2023-05-09 16:39:25.000000 ha-services-0.3.3/ha_services/mqtt4homeassistant/converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1061 2023-05-09 16:39:25.000000 ha-services-0.3.3/ha_services/mqtt4homeassistant/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4102 2023-05-19 19:30:59.000000 ha-services-0.3.3/ha_services/mqtt4homeassistant/mqtt.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.019924 ha-services-0.3.3/ha_services/mqtt4homeassistant/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.3.3/ha_services/mqtt4homeassistant/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2142 2023-05-09 16:39:25.000000 ha-services-0.3.3/ha_services/mqtt4homeassistant/tests/test_converter.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.019924 ha-services-0.3.3/ha_services/mqtt4homeassistant/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.3.3/ha_services/mqtt4homeassistant/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      315 2023-05-09 16:39:25.000000 ha-services-0.3.3/ha_services/mqtt4homeassistant/utilities/string_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.019924 ha-services-0.3.3/ha_services/systemd/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.3.3/ha_services/systemd/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7684 2023-05-21 09:20:35.000000 ha-services-0.3.3/ha_services/systemd/api.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3441 2023-08-08 15:51:06.000000 ha-services-0.3.3/ha_services/systemd/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)      505 2023-05-10 07:16:49.000000 ha-services-0.3.3/ha_services/systemd/defaults.py
+-rw-rw-r--   0 jens      (1000) users      (100)      104 2023-05-21 09:17:03.000000 ha-services-0.3.3/ha_services/systemd/exceptions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      320 2023-05-17 15:08:38.000000 ha-services-0.3.3/ha_services/systemd/service_template.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     1794 2023-05-09 19:43:34.000000 ha-services-0.3.3/ha_services/systemd/template.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.019924 ha-services-0.3.3/ha_services/systemd/test_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-18 04:08:42.000000 ha-services-0.3.3/ha_services/systemd/test_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2012 2023-05-18 05:54:08.000000 ha-services-0.3.3/ha_services/systemd/test_utils/mock_systemd_info.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.019924 ha-services-0.3.3/ha_services/systemd/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.3.3/ha_services/systemd/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4801 2023-05-21 09:30:28.000000 ha-services-0.3.3/ha_services/systemd/tests/test_api.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1655 2023-05-21 09:20:38.000000 ha-services-0.3.3/ha_services/systemd/tests/test_data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3000 2023-05-18 06:02:23.000000 ha-services-0.3.3/ha_services/systemd/tests/test_mock_systemd_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)      595 2023-05-18 06:01:09.000000 ha-services-0.3.3/ha_services/systemd/tests/test_mock_systemd_info_mock_1.snapshot.toml
+-rw-rw-r--   0 jens      (1000) users      (100)     2471 2023-05-09 19:43:34.000000 ha-services-0.3.3/ha_services/systemd/tests/test_template.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.019924 ha-services-0.3.3/ha_services/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      296 2023-05-19 19:29:53.000000 ha-services-0.3.3/ha_services/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      217 2023-05-09 16:39:25.000000 ha-services-0.3.3/ha_services/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2579 2023-05-09 16:39:25.000000 ha-services-0.3.3/ha_services/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2949 2023-05-18 14:20:00.000000 ha-services-0.3.3/ha_services/tests/test_readme.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.023923 ha-services-0.3.3/ha_services/toml_settings/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.3.3/ha_services/toml_settings/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4234 2023-05-18 05:57:51.000000 ha-services-0.3.3/ha_services/toml_settings/api.py
+-rw-rw-r--   0 jens      (1000) users      (100)      220 2023-05-09 20:53:17.000000 ha-services-0.3.3/ha_services/toml_settings/data_class_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1352 2023-05-11 19:53:35.000000 ha-services-0.3.3/ha_services/toml_settings/debug.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3247 2023-08-08 15:57:39.000000 ha-services-0.3.3/ha_services/toml_settings/deserialize.py
+-rw-rw-r--   0 jens      (1000) users      (100)       56 2023-05-09 16:39:25.000000 ha-services-0.3.3/ha_services/toml_settings/exceptions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      836 2023-05-20 10:50:56.000000 ha-services-0.3.3/ha_services/toml_settings/sensible_editor.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1847 2023-05-18 06:01:57.000000 ha-services-0.3.3/ha_services/toml_settings/serialize.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.023923 ha-services-0.3.3/ha_services/toml_settings/test_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-18 05:26:41.000000 ha-services-0.3.3/ha_services/toml_settings/test_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1153 2023-05-18 13:05:47.000000 ha-services-0.3.3/ha_services/toml_settings/test_utils/cli_mock.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3092 2023-05-18 08:32:52.000000 ha-services-0.3.3/ha_services/toml_settings/test_utils/data_class_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.023923 ha-services-0.3.3/ha_services/toml_settings/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.3.3/ha_services/toml_settings/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1383 2023-05-18 05:43:52.000000 ha-services-0.3.3/ha_services/toml_settings/tests/fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1044 2023-05-17 15:20:34.000000 ha-services-0.3.3/ha_services/toml_settings/tests/test_demo_settings.py
+-rw-rw-r--   0 jens      (1000) users      (100)     6244 2023-08-08 16:06:47.000000 ha-services-0.3.3/ha_services/toml_settings/tests/test_deserialize.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1808 2023-05-20 10:49:05.000000 ha-services-0.3.3/ha_services/toml_settings/tests/test_sensible_editor.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3172 2023-05-18 05:24:56.000000 ha-services-0.3.3/ha_services/toml_settings/tests/test_serialize.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3205 2023-05-18 08:31:32.000000 ha-services-0.3.3/ha_services/toml_settings/tests/test_test_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-08-08 16:13:16.019924 ha-services-0.3.3/ha_services.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)     6951 2023-08-08 16:13:16.000000 ha-services-0.3.3/ha_services.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     3233 2023-08-08 16:13:16.000000 ha-services-0.3.3/ha_services.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-08-08 16:13:16.000000 ha-services-0.3.3/ha_services.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      105 2023-08-08 16:13:16.000000 ha-services-0.3.3/ha_services.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      228 2023-08-08 16:13:16.000000 ha-services-0.3.3/ha_services.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       12 2023-08-08 16:13:16.000000 ha-services-0.3.3/ha_services.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     4811 2023-07-09 13:51:15.000000 ha-services-0.3.3/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    54223 2023-08-08 16:11:17.000000 ha-services-0.3.3/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)    30539 2023-08-08 16:11:03.000000 ha-services-0.3.3/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-08-08 16:13:16.023923 ha-services-0.3.3/setup.cfg
```

### Comparing `ha-services-0.3.2/.github/workflows/tests.yml` & `ha-services-0.3.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/PKG-INFO` & `ha-services-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ha-services
-Version: 0.3.2
+Version: 0.3.3
 Summary: Helpers to send periodic information via MQTT to Home Assistant
 Author-email: Jens Diemer <github@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/ha_services
 Project-URL: Source, https://github.com/jedie/ha_services
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
```

### Comparing `ha-services-0.3.2/README.md` & `ha-services-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/cli.py` & `ha-services-0.3.3/cli.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/dev-cli.py` & `ha-services-0.3.3/dev-cli.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/cli/cli_app.py` & `ha-services-0.3.3/ha_services/cli/cli_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,13 +280,13 @@
     print(f'[bold][green]ha-services[/green] DEMO cli v[cyan]{__version__}')
 
     console = Console()
     rich_traceback_install(
         width=console.size.width,  # full terminal width
         show_locals=True,
         suppress=[click, rich_click],
-        max_frames=2,
+        max_frames=8,
     )
 
     # Execute Click CLI:
     cli.name = './cli.py'
     cli()
```

### Comparing `ha-services-0.3.2/ha_services/cli/dev.py` & `ha-services-0.3.3/ha_services/cli/dev.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/cli_tools/dev_tools.py` & `ha-services-0.3.3/ha_services/cli_tools/dev_tools.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/cli_tools/dict_utils.py` & `ha-services-0.3.3/ha_services/cli_tools/dict_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/cli_tools/path_utils.py` & `ha-services-0.3.3/ha_services/cli_tools/path_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/cli_tools/rich_utils.py` & `ha-services-0.3.3/ha_services/cli_tools/rich_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/cli_tools/test_utils/assertion.py` & `ha-services-0.3.3/ha_services/cli_tools/test_utils/assertion.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/cli_tools/test_utils/cli_readme.py` & `ha-services-0.3.3/ha_services/cli_tools/test_utils/cli_readme.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/cli_tools/test_utils/environment_fixtures.py` & `ha-services-0.3.3/ha_services/cli_tools/test_utils/environment_fixtures.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/cli_tools/test_utils/rich_test_utils.py` & `ha-services-0.3.3/ha_services/cli_tools/test_utils/rich_test_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/cli_tools/tests/test_environ_fixtures.py` & `ha-services-0.3.3/ha_services/cli_tools/tests/test_environ_fixtures.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/cli_tools/tests/test_mock_rich.py` & `ha-services-0.3.3/ha_services/cli_tools/tests/test_mock_rich.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/cli_tools/tests/test_path_utils.py` & `ha-services-0.3.3/ha_services/cli_tools/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/cli_tools/verbosity.py` & `ha-services-0.3.3/ha_services/cli_tools/verbosity.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/example.py` & `ha-services-0.3.3/ha_services/example.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/mqtt4homeassistant/converter.py` & `ha-services-0.3.3/ha_services/mqtt4homeassistant/converter.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/mqtt4homeassistant/data_classes.py` & `ha-services-0.3.3/ha_services/mqtt4homeassistant/data_classes.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/mqtt4homeassistant/mqtt.py` & `ha-services-0.3.3/ha_services/mqtt4homeassistant/mqtt.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/mqtt4homeassistant/tests/test_converter.py` & `ha-services-0.3.3/ha_services/mqtt4homeassistant/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/systemd/api.py` & `ha-services-0.3.3/ha_services/systemd/api.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/systemd/data_classes.py` & `ha-services-0.3.3/ha_services/systemd/data_classes.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/systemd/template.py` & `ha-services-0.3.3/ha_services/systemd/template.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/systemd/test_utils/mock_systemd_info.py` & `ha-services-0.3.3/ha_services/systemd/test_utils/mock_systemd_info.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/systemd/tests/test_api.py` & `ha-services-0.3.3/ha_services/systemd/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/systemd/tests/test_data_classes.py` & `ha-services-0.3.3/ha_services/systemd/tests/test_data_classes.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/systemd/tests/test_mock_systemd_info.py` & `ha-services-0.3.3/ha_services/systemd/tests/test_mock_systemd_info.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/systemd/tests/test_mock_systemd_info_mock_1.snapshot.toml` & `ha-services-0.3.3/ha_services/systemd/tests/test_mock_systemd_info_mock_1.snapshot.toml`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/systemd/tests/test_template.py` & `ha-services-0.3.3/ha_services/systemd/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/tests/test_project_setup.py` & `ha-services-0.3.3/ha_services/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/tests/test_readme.py` & `ha-services-0.3.3/ha_services/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/toml_settings/api.py` & `ha-services-0.3.3/ha_services/toml_settings/api.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/toml_settings/debug.py` & `ha-services-0.3.3/ha_services/toml_settings/debug.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/toml_settings/deserialize.py` & `ha-services-0.3.3/ha_services/toml_settings/deserialize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import dataclasses
 import logging
 from pathlib import Path
 
 import tomlkit
 from tomlkit import TOMLDocument
 
+from ha_services.cli_tools.path_utils import expand_user
 from ha_services.toml_settings.data_class_utils import iter_dataclass
 from ha_services.toml_settings.serialize import add_dataclass
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -59,15 +60,17 @@
                     field_name,
                     value,
                     type(value).__name__,
                 )
                 document[field_name] = field_value  # Add default one
                 _changed = True
             else:
-                setattr(instance, field_name, Path(value))
+                path_value = Path(value)
+                path_value = expand_user(path_value)  # Use user ~ even if called via sudo
+                setattr(instance, field_name, path_value)
         elif not isinstance(field_value, type(doc_value.unwrap())):
             logger.error(
                 'Toml value %s=%r is type %r but must be type %r -> ignored and use default value!',
                 field_name,
                 doc_value,
                 type(doc_value.unwrap()).__name__,
                 type(field_value).__name__,
```

### Comparing `ha-services-0.3.2/ha_services/toml_settings/sensible_editor.py` & `ha-services-0.3.3/ha_services/toml_settings/sensible_editor.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/toml_settings/serialize.py` & `ha-services-0.3.3/ha_services/toml_settings/serialize.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/toml_settings/test_utils/cli_mock.py` & `ha-services-0.3.3/ha_services/toml_settings/test_utils/cli_mock.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/toml_settings/test_utils/data_class_utils.py` & `ha-services-0.3.3/ha_services/toml_settings/test_utils/data_class_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/toml_settings/tests/fixtures.py` & `ha-services-0.3.3/ha_services/toml_settings/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/toml_settings/tests/test_demo_settings.py` & `ha-services-0.3.3/ha_services/toml_settings/tests/test_demo_settings.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/toml_settings/tests/test_deserialize.py` & `ha-services-0.3.3/ha_services/toml_settings/tests/test_deserialize.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import inspect
 import logging
 from pathlib import Path
 from unittest import TestCase
 
 import tomlkit
 
+from ha_services.cli_tools.test_utils.environment_fixtures import AsSudoCallOverrideEnviron
 from ha_services.toml_settings.deserialize import toml2dataclass
 from ha_services.toml_settings.tests.fixtures import ComplexExample, PathExample, SimpleExample
 
 
 class DeserializeTestCase(TestCase):
     def test_toml2dataclass_simple(self):
         instance = SimpleExample()
@@ -100,14 +101,26 @@
         self.assertEqual(
             data,
             {
                 'path': Path('/to/some/other/place'),
             },
         )
 
+        # Path entries can use "~":
+        real_home = Path().home()
+        toml2dataclass(document=tomlkit.loads('path = "~/foo/"'), instance=instance)
+        self.assertEqual(instance.path, real_home / 'foo')
+
+        # sudo calls will be also use the user home and not /root/
+
+        with AsSudoCallOverrideEnviron():
+            self.assertEqual(Path('~').expanduser(), Path('/root'))
+            toml2dataclass(document=tomlkit.loads('path = "~/bar/"'), instance=instance)
+            self.assertEqual(instance.path, real_home / 'bar')
+
     def test_toml2dataclass_inheritance(self):
         instance = ComplexExample()
         data = dataclasses.asdict(instance)
         self.assertEqual(
             data,
             {
                 'foo': 'bar',
```

### Comparing `ha-services-0.3.2/ha_services/toml_settings/tests/test_sensible_editor.py` & `ha-services-0.3.3/ha_services/toml_settings/tests/test_sensible_editor.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/toml_settings/tests/test_serialize.py` & `ha-services-0.3.3/ha_services/toml_settings/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services/toml_settings/tests/test_test_utils.py` & `ha-services-0.3.3/ha_services/toml_settings/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/ha_services.egg-info/PKG-INFO` & `ha-services-0.3.3/ha_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ha-services
-Version: 0.3.2
+Version: 0.3.3
 Summary: Helpers to send periodic information via MQTT to Home Assistant
 Author-email: Jens Diemer <github@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/ha_services
 Project-URL: Source, https://github.com/jedie/ha_services
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
```

### Comparing `ha-services-0.3.2/ha_services.egg-info/SOURCES.txt` & `ha-services-0.3.3/ha_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ha-services-0.3.2/pyproject.toml` & `ha-services-0.3.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -37,21 +37,18 @@
     # https://github.com/akaihola/darker
     # https://github.com/ikamensh/flynt
     # https://github.com/pycqa/isort
     # https://github.com/pygments/pygments
     "darker[flynt, isort, color]",
 
     "tomli",  # https://github.com/hukkin/tomli
-    # tomli only needed for Python <3.11, but see bug:
-    # https://github.com/pypa/pip/issues/9644#issuecomment-1456583402
-    #"tomli;python_version<\"3.11\"",  # https://github.com/hukkin/tomli
-
-    # Work-a-round for:
-    # https://github.com/jazzband/pip-tools/issues/994#issuecomment-1321226661
-    "typing-extensions>=3.10;python_version<\"3.10\"",
+    #
+    # tomli only needed for Python <3.11, but see pip bug:
+    # https://github.com/pypa/pip/issues/9644 / https://github.com/jazzband/pip-tools/issues/1866
+    #'tomli;python_version<"3.11"',  # https://github.com/hukkin/tomli
 ]
 
 [project.urls]
 Documentation = "https://github.com/jedie/ha_services"
 Source = "https://github.com/jedie/ha_services"
 
 [project.scripts]
```

### Comparing `ha-services-0.3.2/requirements.dev.txt` & `ha-services-0.3.3/requirements.dev.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,75 +3,78 @@
 # by the following command:
 #
 #    ./cli.py update
 #
 arrow==1.2.3 \
     --hash=sha256:3934b30ca1b9f292376d9db15b19446088d12ec58629bc3f0da28fd55fb633a1 \
     --hash=sha256:5a49ab92e3b7b71d96cd6bfcc4df14efefc9dfa96ea19045815914a6ab6b1fe2
-    # via jinja2-time
+    # via cookiecutter
 astor==0.8.1 \
     --hash=sha256:070a54e890cefb5b3739d19f30f5a5ec840ffc9c50ffa7d23cc9fc1a38ebbfc5 \
     --hash=sha256:6a6effda93f4e1ce9f618779b2dd1d9d84f1e32812c23a29b3fff6fd7f63fa5e
     # via flynt
+autoflake==2.2.0 \
+    --hash=sha256:62e1f74a0fdad898a96fee6f99fe8241af90ad99c7110c884b35855778412251 \
+    --hash=sha256:de409b009a34c1c2a7cc2aae84c4c05047f9773594317c6a6968bd497600d4a0
+    # via manageprojects
 autopep8==2.0.2 \
     --hash=sha256:86e9303b5e5c8160872b2f5ef611161b2893e9bfe8ccc7e2f76385947d57a2f1 \
     --hash=sha256:f9849cdd62108cb739dbcdbfb7fdcc9a30d1b63c4cc3e1c1f893b5360941b61c
-    # via ha-services (pyproject.toml)
+    # via
+    #   ha-services (pyproject.toml)
+    #   manageprojects
 binaryornot==0.4.4 \
     --hash=sha256:359501dfc9d40632edc9fac890e19542db1a287bbcfa58175b66658392018061 \
     --hash=sha256:b8b71173c917bddcd2c16070412e369c3ed7f0528926f70cac18a6c97fd563e4
     # via cookiecutter
-black==23.3.0 \
-    --hash=sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5 \
-    --hash=sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915 \
-    --hash=sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326 \
-    --hash=sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940 \
-    --hash=sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b \
-    --hash=sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30 \
-    --hash=sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c \
-    --hash=sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c \
-    --hash=sha256:3a150542a204124ed00683f0db1f5cf1c2aaaa9cc3495b7a3b5976fb136090ab \
-    --hash=sha256:48f9d345675bb7fbc3dd85821b12487e1b9a75242028adad0333ce36ed2a6d27 \
-    --hash=sha256:50cb33cac881766a5cd9913e10ff75b1e8eb71babf4c7104f2e9c52da1fb7de2 \
-    --hash=sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961 \
-    --hash=sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9 \
-    --hash=sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb \
-    --hash=sha256:6f3c333ea1dd6771b2d3777482429864f8e258899f6ff05826c3a4fcc5ce3f70 \
-    --hash=sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331 \
-    --hash=sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2 \
-    --hash=sha256:92c543f6854c28a3c7f39f4d9b7694f9a6eb9d3c5e2ece488c327b6e7ea9b266 \
-    --hash=sha256:a6f6886c9869d4daae2d1715ce34a19bbc4b95006d20ed785ca00fa03cba312d \
-    --hash=sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6 \
-    --hash=sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b \
-    --hash=sha256:e114420bf26b90d4b9daa597351337762b63039752bdf72bf361364c1aa05925 \
-    --hash=sha256:e198cf27888ad6f4ff331ca1c48ffc038848ea9f031a3b40ba36aced7e22f2c8 \
-    --hash=sha256:ec751418022185b0c1bb7d7736e6933d40bbb14c14a0abcf9123d1b159f98dd4 \
-    --hash=sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3
+black==23.7.0 \
+    --hash=sha256:01ede61aac8c154b55f35301fac3e730baf0c9cf8120f65a9cd61a81cfb4a0c3 \
+    --hash=sha256:022a582720b0d9480ed82576c920a8c1dde97cc38ff11d8d8859b3bd6ca9eedb \
+    --hash=sha256:25cc308838fe71f7065df53aedd20327969d05671bac95b38fdf37ebe70ac087 \
+    --hash=sha256:27eb7a0c71604d5de083757fbdb245b1a4fae60e9596514c6ec497eb63f95320 \
+    --hash=sha256:327a8c2550ddc573b51e2c352adb88143464bb9d92c10416feb86b0f5aee5ff6 \
+    --hash=sha256:47e56d83aad53ca140da0af87678fb38e44fd6bc0af71eebab2d1f59b1acf1d3 \
+    --hash=sha256:501387a9edcb75d7ae8a4412bb8749900386eaef258f1aefab18adddea1936bc \
+    --hash=sha256:552513d5cd5694590d7ef6f46e1767a4df9af168d449ff767b13b084c020e63f \
+    --hash=sha256:5c4bc552ab52f6c1c506ccae05681fab58c3f72d59ae6e6639e8885e94fe2587 \
+    --hash=sha256:642496b675095d423f9b8448243336f8ec71c9d4d57ec17bf795b67f08132a91 \
+    --hash=sha256:6d1c6022b86f83b632d06f2b02774134def5d4d4f1dac8bef16d90cda18ba28a \
+    --hash=sha256:7f3bf2dec7d541b4619b8ce526bda74a6b0bffc480a163fed32eb8b3c9aed8ad \
+    --hash=sha256:831d8f54c3a8c8cf55f64d0422ee875eecac26f5f649fb6c1df65316b67c8926 \
+    --hash=sha256:8417dbd2f57b5701492cd46edcecc4f9208dc75529bcf76c514864e48da867d9 \
+    --hash=sha256:86cee259349b4448adb4ef9b204bb4467aae74a386bce85d56ba4f5dc0da27be \
+    --hash=sha256:893695a76b140881531062d48476ebe4a48f5d1e9388177e175d76234ca247cd \
+    --hash=sha256:9fd59d418c60c0348505f2ddf9609c1e1de8e7493eab96198fc89d9f865e7a96 \
+    --hash=sha256:ad0014efc7acf0bd745792bd0d8857413652979200ab924fbf239062adc12491 \
+    --hash=sha256:b5b0ee6d96b345a8b420100b7d71ebfdd19fab5e8301aff48ec270042cd40ac2 \
+    --hash=sha256:c333286dc3ddca6fdff74670b911cccedacb4ef0a60b34e491b8a67c833b343a \
+    --hash=sha256:f9062af71c59c004cd519e2fb8f5d25d39e46d3af011b41ab43b9c74e27e236f \
+    --hash=sha256:fb074d8b213749fa1d077d630db0d5f8cc3b2ae63587ad4116e8a436e9bbe995
     # via darker
 bleach==6.0.0 \
     --hash=sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414 \
     --hash=sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4
     # via readme-renderer
 build==0.10.0 \
     --hash=sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171 \
     --hash=sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269
     # via pip-tools
-bx-py-utils==81 \
-    --hash=sha256:5c2e189cccbeb852b058078bc7b0a8976f5f691ee7de657a87eef43fc89fa59a \
-    --hash=sha256:fd282f9e4ed8ed2842154ffe3fdd2ca56c428023021afc5b8ff765a53c02cddb
+bx-py-utils==85 \
+    --hash=sha256:8d6ee4bb0c431304b812f5bebb1bc8e2ab05f1b6c2f8d16d352cbcee5e916cd2 \
+    --hash=sha256:df023fa05cda8e969d2cbdb4cc348d8b7670567a2fe775faf7a0c869ec56eaa2
     # via
     #   ha-services (pyproject.toml)
     #   manageprojects
-cachetools==5.3.0 \
-    --hash=sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14 \
-    --hash=sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4
+cachetools==5.3.1 \
+    --hash=sha256:95ef631eeaea14ba2e36f06437f36463aac3a096799e876ee55e5cdccb102590 \
+    --hash=sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b
     # via tox
-certifi==2023.5.7 \
-    --hash=sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7 \
-    --hash=sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716
+certifi==2023.7.22 \
+    --hash=sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082 \
+    --hash=sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9
     # via requests
 cffi==1.15.1 \
     --hash=sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5 \
     --hash=sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef \
     --hash=sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104 \
     --hash=sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426 \
     --hash=sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405 \
@@ -131,397 +134,414 @@
     --hash=sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e \
     --hash=sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9 \
     --hash=sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6 \
     --hash=sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b \
     --hash=sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01 \
     --hash=sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0
     # via cryptography
-chardet==5.1.0 \
-    --hash=sha256:0d62712b956bc154f85fb0a266e2a3c5913c2967e00348701b32411d6def31e5 \
-    --hash=sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9
+chardet==5.2.0 \
+    --hash=sha256:1b3b6ff479a8c414bc3fa2c0852995695c4a026dcd6d0633b2dd092ca39c1cf7 \
+    --hash=sha256:e1cf59446890a00105fe7b7912492ea04b6e6f06d4b742b2c788469e34c82970
     # via
     #   binaryornot
     #   tox
-charset-normalizer==3.1.0 \
-    --hash=sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6 \
-    --hash=sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1 \
-    --hash=sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e \
-    --hash=sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373 \
-    --hash=sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62 \
-    --hash=sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230 \
-    --hash=sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be \
-    --hash=sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c \
-    --hash=sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0 \
-    --hash=sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448 \
-    --hash=sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f \
-    --hash=sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649 \
-    --hash=sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d \
-    --hash=sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0 \
-    --hash=sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706 \
-    --hash=sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a \
-    --hash=sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59 \
-    --hash=sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23 \
-    --hash=sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5 \
-    --hash=sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb \
-    --hash=sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e \
-    --hash=sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e \
-    --hash=sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c \
-    --hash=sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28 \
-    --hash=sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d \
-    --hash=sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41 \
-    --hash=sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974 \
-    --hash=sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce \
-    --hash=sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f \
-    --hash=sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1 \
-    --hash=sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d \
-    --hash=sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8 \
-    --hash=sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017 \
-    --hash=sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31 \
-    --hash=sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7 \
-    --hash=sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8 \
-    --hash=sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e \
-    --hash=sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14 \
-    --hash=sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd \
-    --hash=sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d \
-    --hash=sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795 \
-    --hash=sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b \
-    --hash=sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b \
-    --hash=sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b \
-    --hash=sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203 \
-    --hash=sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f \
-    --hash=sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19 \
-    --hash=sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1 \
-    --hash=sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a \
-    --hash=sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac \
-    --hash=sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9 \
-    --hash=sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0 \
-    --hash=sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137 \
-    --hash=sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f \
-    --hash=sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6 \
-    --hash=sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5 \
-    --hash=sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909 \
-    --hash=sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f \
-    --hash=sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0 \
-    --hash=sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324 \
-    --hash=sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755 \
-    --hash=sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb \
-    --hash=sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854 \
-    --hash=sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c \
-    --hash=sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60 \
-    --hash=sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84 \
-    --hash=sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0 \
-    --hash=sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b \
-    --hash=sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1 \
-    --hash=sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531 \
-    --hash=sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1 \
-    --hash=sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11 \
-    --hash=sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326 \
-    --hash=sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df \
-    --hash=sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab
+charset-normalizer==3.2.0 \
+    --hash=sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96 \
+    --hash=sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c \
+    --hash=sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710 \
+    --hash=sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706 \
+    --hash=sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020 \
+    --hash=sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252 \
+    --hash=sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad \
+    --hash=sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329 \
+    --hash=sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a \
+    --hash=sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f \
+    --hash=sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6 \
+    --hash=sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4 \
+    --hash=sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a \
+    --hash=sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46 \
+    --hash=sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2 \
+    --hash=sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23 \
+    --hash=sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace \
+    --hash=sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd \
+    --hash=sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982 \
+    --hash=sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10 \
+    --hash=sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2 \
+    --hash=sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea \
+    --hash=sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09 \
+    --hash=sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5 \
+    --hash=sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149 \
+    --hash=sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489 \
+    --hash=sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9 \
+    --hash=sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80 \
+    --hash=sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592 \
+    --hash=sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3 \
+    --hash=sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6 \
+    --hash=sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed \
+    --hash=sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c \
+    --hash=sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200 \
+    --hash=sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a \
+    --hash=sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e \
+    --hash=sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d \
+    --hash=sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6 \
+    --hash=sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623 \
+    --hash=sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669 \
+    --hash=sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3 \
+    --hash=sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa \
+    --hash=sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9 \
+    --hash=sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2 \
+    --hash=sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f \
+    --hash=sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1 \
+    --hash=sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4 \
+    --hash=sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a \
+    --hash=sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8 \
+    --hash=sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3 \
+    --hash=sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029 \
+    --hash=sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f \
+    --hash=sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959 \
+    --hash=sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22 \
+    --hash=sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7 \
+    --hash=sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952 \
+    --hash=sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346 \
+    --hash=sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e \
+    --hash=sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d \
+    --hash=sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299 \
+    --hash=sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd \
+    --hash=sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a \
+    --hash=sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3 \
+    --hash=sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037 \
+    --hash=sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94 \
+    --hash=sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c \
+    --hash=sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858 \
+    --hash=sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a \
+    --hash=sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449 \
+    --hash=sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c \
+    --hash=sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918 \
+    --hash=sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1 \
+    --hash=sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c \
+    --hash=sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac \
+    --hash=sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa
     # via requests
-click==8.1.3 \
-    --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
-    --hash=sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48
+click==8.1.6 \
+    --hash=sha256:48ee849951919527a045bfe3bf7baa8a959c423134e1a5b98c05c20ba75a1cbd \
+    --hash=sha256:fa244bb30b3b5ee2cae3da8f55c9e5e0c0e86093306301fb418eb9dc40fbded5
     # via
     #   black
     #   cookiecutter
     #   ha-services (pyproject.toml)
     #   manageprojects
     #   pip-tools
     #   rich-click
     #   safety
-codespell==2.2.4 \
-    --hash=sha256:0b4620473c257d9cde1ff8998b26b2bb209a35c2b7489f5dc3436024298ce83a \
-    --hash=sha256:7d984b8130108e6f82524b7d09f8b7bf2fb1e398c5d4b37d9e2bd310145b3e29
-    # via ha-services (pyproject.toml)
+codespell==2.2.5 \
+    --hash=sha256:6d9faddf6eedb692bf80c9a94ec13ab4f5fb585aabae5f3750727148d7b5be56 \
+    --hash=sha256:efa037f54b73c84f7bd14ce8e853d5f822cdd6386ef0ff32e957a3919435b9ec
+    # via
+    #   ha-services (pyproject.toml)
+    #   manageprojects
 colorama==0.4.6 \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
     # via tox
-cookiecutter==2.1.1 \
-    --hash=sha256:9f3ab027cec4f70916e28f03470bdb41e637a3ad354b4d65c765d93aad160022 \
-    --hash=sha256:f3982be8d9c53dac1261864013fdec7f83afd2e42ede6f6dd069c5e149c540d5
+cookiecutter==2.3.0 \
+    --hash=sha256:7e87944757c6e9f8729cf89a4139b6a35ab4d6dcbc6ae3e7d6360d44ad3ad383 \
+    --hash=sha256:942a794981747f6d7f439d6e49d39dc91a9a641283614160c93c474c72c29621
     # via manageprojects
-coverage==7.2.5 \
-    --hash=sha256:0342a28617e63ad15d96dca0f7ae9479a37b7d8a295f749c14f3436ea59fdcb3 \
-    --hash=sha256:066b44897c493e0dcbc9e6a6d9f8bbb6607ef82367cf6810d387c09f0cd4fe9a \
-    --hash=sha256:10b15394c13544fce02382360cab54e51a9e0fd1bd61ae9ce012c0d1e103c813 \
-    --hash=sha256:12580845917b1e59f8a1c2ffa6af6d0908cb39220f3019e36c110c943dc875b0 \
-    --hash=sha256:156192e5fd3dbbcb11cd777cc469cf010a294f4c736a2b2c891c77618cb1379a \
-    --hash=sha256:1637253b11a18f453e34013c665d8bf15904c9e3c44fbda34c643fbdc9d452cd \
-    --hash=sha256:292300f76440651529b8ceec283a9370532f4ecba9ad67d120617021bb5ef139 \
-    --hash=sha256:30dcaf05adfa69c2a7b9f7dfd9f60bc8e36b282d7ed25c308ef9e114de7fc23b \
-    --hash=sha256:338aa9d9883aaaad53695cb14ccdeb36d4060485bb9388446330bef9c361c252 \
-    --hash=sha256:373ea34dca98f2fdb3e5cb33d83b6d801007a8074f992b80311fc589d3e6b790 \
-    --hash=sha256:38c0a497a000d50491055805313ed83ddba069353d102ece8aef5d11b5faf045 \
-    --hash=sha256:40cc0f91c6cde033da493227797be2826cbf8f388eaa36a0271a97a332bfd7ce \
-    --hash=sha256:4436cc9ba5414c2c998eaedee5343f49c02ca93b21769c5fdfa4f9d799e84200 \
-    --hash=sha256:509ecd8334c380000d259dc66feb191dd0a93b21f2453faa75f7f9cdcefc0718 \
-    --hash=sha256:5c587f52c81211d4530fa6857884d37f514bcf9453bdeee0ff93eaaf906a5c1b \
-    --hash=sha256:5f3671662dc4b422b15776cdca89c041a6349b4864a43aa2350b6b0b03bbcc7f \
-    --hash=sha256:6599bf92f33ab041e36e06d25890afbdf12078aacfe1f1d08c713906e49a3fe5 \
-    --hash=sha256:6e8a95f243d01ba572341c52f89f3acb98a3b6d1d5d830efba86033dd3687ade \
-    --hash=sha256:706ec567267c96717ab9363904d846ec009a48d5f832140b6ad08aad3791b1f5 \
-    --hash=sha256:780551e47d62095e088f251f5db428473c26db7829884323e56d9c0c3118791a \
-    --hash=sha256:7ff8f3fb38233035028dbc93715551d81eadc110199e14bbbfa01c5c4a43f8d8 \
-    --hash=sha256:828189fcdda99aae0d6bf718ea766b2e715eabc1868670a0a07bf8404bf58c33 \
-    --hash=sha256:857abe2fa6a4973f8663e039ead8d22215d31db613ace76e4a98f52ec919068e \
-    --hash=sha256:883123d0bbe1c136f76b56276074b0c79b5817dd4238097ffa64ac67257f4b6c \
-    --hash=sha256:8877d9b437b35a85c18e3c6499b23674684bf690f5d96c1006a1ef61f9fdf0f3 \
-    --hash=sha256:8e575a59315a91ccd00c7757127f6b2488c2f914096077c745c2f1ba5b8c0969 \
-    --hash=sha256:97072cc90f1009386c8a5b7de9d4fc1a9f91ba5ef2146c55c1f005e7b5c5e068 \
-    --hash=sha256:9a22cbb5ede6fade0482111fa7f01115ff04039795d7092ed0db43522431b4f2 \
-    --hash=sha256:a063aad9f7b4c9f9da7b2550eae0a582ffc7623dca1c925e50c3fbde7a579771 \
-    --hash=sha256:a08c7401d0b24e8c2982f4e307124b671c6736d40d1c39e09d7a8687bddf83ed \
-    --hash=sha256:a0b273fe6dc655b110e8dc89b8ec7f1a778d78c9fd9b4bda7c384c8906072212 \
-    --hash=sha256:a2b3b05e22a77bb0ae1a3125126a4e08535961c946b62f30985535ed40e26614 \
-    --hash=sha256:a66e055254a26c82aead7ff420d9fa8dc2da10c82679ea850d8feebf11074d88 \
-    --hash=sha256:aa387bd7489f3e1787ff82068b295bcaafbf6f79c3dad3cbc82ef88ce3f48ad3 \
-    --hash=sha256:ae453f655640157d76209f42c62c64c4d4f2c7f97256d3567e3b439bd5c9b06c \
-    --hash=sha256:b5016e331b75310610c2cf955d9f58a9749943ed5f7b8cfc0bb89c6134ab0a84 \
-    --hash=sha256:b9a4ee55174b04f6af539218f9f8083140f61a46eabcaa4234f3c2a452c4ed11 \
-    --hash=sha256:bd3b4b8175c1db502adf209d06136c000df4d245105c8839e9d0be71c94aefe1 \
-    --hash=sha256:bebea5f5ed41f618797ce3ffb4606c64a5de92e9c3f26d26c2e0aae292f015c1 \
-    --hash=sha256:c10fbc8a64aa0f3ed136b0b086b6b577bc64d67d5581acd7cc129af52654384e \
-    --hash=sha256:c2c41c1b1866b670573657d584de413df701f482574bad7e28214a2362cb1fd1 \
-    --hash=sha256:cf97ed82ca986e5c637ea286ba2793c85325b30f869bf64d3009ccc1a31ae3fd \
-    --hash=sha256:d1f25ee9de21a39b3a8516f2c5feb8de248f17da7eead089c2e04aa097936b47 \
-    --hash=sha256:d2fbc2a127e857d2f8898aaabcc34c37771bf78a4d5e17d3e1f5c30cd0cbc62a \
-    --hash=sha256:dc945064a8783b86fcce9a0a705abd7db2117d95e340df8a4333f00be5efb64c \
-    --hash=sha256:ddc5a54edb653e9e215f75de377354e2455376f416c4378e1d43b08ec50acc31 \
-    --hash=sha256:e8834e5f17d89e05697c3c043d3e58a8b19682bf365048837383abfe39adaed5 \
-    --hash=sha256:ef9659d1cda9ce9ac9585c045aaa1e59223b143f2407db0eaee0b61a4f266fb6 \
-    --hash=sha256:f6f5cab2d7f0c12f8187a376cc6582c477d2df91d63f75341307fcdcb5d60303 \
-    --hash=sha256:f81c9b4bd8aa747d417407a7f6f0b1469a43b36a85748145e144ac4e8d303cb5 \
-    --hash=sha256:f99ef080288f09ffc687423b8d60978cf3a465d3f404a18d1a05474bd8575a47
-    # via ha-services (pyproject.toml)
-cryptography==40.0.2 \
-    --hash=sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440 \
-    --hash=sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288 \
-    --hash=sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b \
-    --hash=sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958 \
-    --hash=sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b \
-    --hash=sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d \
-    --hash=sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a \
-    --hash=sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404 \
-    --hash=sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b \
-    --hash=sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e \
-    --hash=sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2 \
-    --hash=sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c \
-    --hash=sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b \
-    --hash=sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9 \
-    --hash=sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b \
-    --hash=sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636 \
-    --hash=sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99 \
-    --hash=sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e \
-    --hash=sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9
+coverage==7.2.7 \
+    --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
+    --hash=sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2 \
+    --hash=sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a \
+    --hash=sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a \
+    --hash=sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01 \
+    --hash=sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6 \
+    --hash=sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7 \
+    --hash=sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f \
+    --hash=sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02 \
+    --hash=sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c \
+    --hash=sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063 \
+    --hash=sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a \
+    --hash=sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5 \
+    --hash=sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959 \
+    --hash=sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97 \
+    --hash=sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6 \
+    --hash=sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f \
+    --hash=sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9 \
+    --hash=sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5 \
+    --hash=sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f \
+    --hash=sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562 \
+    --hash=sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe \
+    --hash=sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9 \
+    --hash=sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f \
+    --hash=sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb \
+    --hash=sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb \
+    --hash=sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1 \
+    --hash=sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb \
+    --hash=sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250 \
+    --hash=sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e \
+    --hash=sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511 \
+    --hash=sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5 \
+    --hash=sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59 \
+    --hash=sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2 \
+    --hash=sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d \
+    --hash=sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3 \
+    --hash=sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4 \
+    --hash=sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de \
+    --hash=sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9 \
+    --hash=sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833 \
+    --hash=sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0 \
+    --hash=sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9 \
+    --hash=sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d \
+    --hash=sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050 \
+    --hash=sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d \
+    --hash=sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6 \
+    --hash=sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353 \
+    --hash=sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb \
+    --hash=sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e \
+    --hash=sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8 \
+    --hash=sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495 \
+    --hash=sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2 \
+    --hash=sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd \
+    --hash=sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27 \
+    --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
+    --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
+    --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
+    --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
+    --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
+    --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
+    # via ha-services (pyproject.toml)
+cryptography==41.0.3 \
+    --hash=sha256:0d09fb5356f975974dbcb595ad2d178305e5050656affb7890a1583f5e02a306 \
+    --hash=sha256:23c2d778cf829f7d0ae180600b17e9fceea3c2ef8b31a99e3c694cbbf3a24b84 \
+    --hash=sha256:3fb248989b6363906827284cd20cca63bb1a757e0a2864d4c1682a985e3dca47 \
+    --hash=sha256:41d7aa7cdfded09b3d73a47f429c298e80796c8e825ddfadc84c8a7f12df212d \
+    --hash=sha256:42cb413e01a5d36da9929baa9d70ca90d90b969269e5a12d39c1e0d475010116 \
+    --hash=sha256:4c2f0d35703d61002a2bbdcf15548ebb701cfdd83cdc12471d2bae80878a4207 \
+    --hash=sha256:4fd871184321100fb400d759ad0cddddf284c4b696568204d281c902fc7b0d81 \
+    --hash=sha256:5259cb659aa43005eb55a0e4ff2c825ca111a0da1814202c64d28a985d33b087 \
+    --hash=sha256:57a51b89f954f216a81c9d057bf1a24e2f36e764a1ca9a501a6964eb4a6800dd \
+    --hash=sha256:652627a055cb52a84f8c448185922241dd5217443ca194d5739b44612c5e6507 \
+    --hash=sha256:67e120e9a577c64fe1f611e53b30b3e69744e5910ff3b6e97e935aeb96005858 \
+    --hash=sha256:6af1c6387c531cd364b72c28daa29232162010d952ceb7e5ca8e2827526aceae \
+    --hash=sha256:6d192741113ef5e30d89dcb5b956ef4e1578f304708701b8b73d38e3e1461f34 \
+    --hash=sha256:7efe8041897fe7a50863e51b77789b657a133c75c3b094e51b5e4b5cec7bf906 \
+    --hash=sha256:84537453d57f55a50a5b6835622ee405816999a7113267739a1b4581f83535bd \
+    --hash=sha256:8f09daa483aedea50d249ef98ed500569841d6498aa9c9f4b0531b9964658922 \
+    --hash=sha256:95dd7f261bb76948b52a5330ba5202b91a26fbac13ad0e9fc8a3ac04752058c7 \
+    --hash=sha256:a74fbcdb2a0d46fe00504f571a2a540532f4c188e6ccf26f1f178480117b33c4 \
+    --hash=sha256:a983e441a00a9d57a4d7c91b3116a37ae602907a7618b882c8013b5762e80574 \
+    --hash=sha256:ab8de0d091acbf778f74286f4989cf3d1528336af1b59f3e5d2ebca8b5fe49e1 \
+    --hash=sha256:aeb57c421b34af8f9fe830e1955bf493a86a7996cc1338fe41b30047d16e962c \
+    --hash=sha256:ce785cf81a7bdade534297ef9e490ddff800d956625020ab2ec2780a556c313e \
+    --hash=sha256:d0d651aa754ef58d75cec6edfbd21259d93810b73f6ec246436a21b7841908de
     # via secretstorage
-darker[color,flynt,isort]==1.7.1 \
-    --hash=sha256:cf4173be4ad2982e5b2ebab7e08bd0d27173f2459ec1b1cf66aec9290da80cce \
-    --hash=sha256:d72126418194871aeaf1e8aa620ad06edc5472848bef71c4d393c22b65571878
-    # via ha-services (pyproject.toml)
-distlib==0.3.6 \
-    --hash=sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46 \
-    --hash=sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e
+darker[color,flynt,isort]==1.7.2 \
+    --hash=sha256:ec5b7c382d9537611c164f3ecca2e1b8a7923bc5a02bf22f6e7f6c8bcbdf593a \
+    --hash=sha256:ec9d130ab2a0f7fa49ab68a08fd231a5bec66147ecbbf94c92a1f33d97b5ef6f
+    # via
+    #   ha-services (pyproject.toml)
+    #   manageprojects
+distlib==0.3.7 \
+    --hash=sha256:2e24928bc811348f0feb63014e97aaae3037f2cf48712d51ae61df7fd6075057 \
+    --hash=sha256:9dafe54b34a028eafd95039d5e5d4851a13734540f1331060d31c9916e7147a8
     # via virtualenv
 docutils==0.20.1 \
     --hash=sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6 \
     --hash=sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b
     # via readme-renderer
-dparse==0.6.2 \
-    --hash=sha256:8097076f1dd26c377f30d4745e6ec18fef42f3bf493933b842ac5bafad8c345f \
-    --hash=sha256:d45255bda21f998bc7ddf2afd5e62505ba6134756ba2d42a84c56b0826614dfe
+dparse==0.6.3 \
+    --hash=sha256:0d8fe18714056ca632d98b24fbfc4e9791d4e47065285ab486182288813a5318 \
+    --hash=sha256:27bb8b4bcaefec3997697ba3f6e06b2447200ba273c0b085c3d012a04571b528
     # via safety
 editorconfig==0.12.3 \
     --hash=sha256:57f8ce78afcba15c8b18d46b5170848c88d56fd38f05c2ec60dbbfcb8996e89e \
     --hash=sha256:6b0851425aa875b08b16789ee0eeadbd4ab59666e9ebe728e526314c4a2e52c1
-    # via ha-services (pyproject.toml)
-filelock==3.12.0 \
-    --hash=sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9 \
-    --hash=sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718
+    # via
+    #   ha-services (pyproject.toml)
+    #   manageprojects
+filelock==3.12.2 \
+    --hash=sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81 \
+    --hash=sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec
     # via
     #   tox
     #   virtualenv
-flake8==6.0.0 \
-    --hash=sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7 \
-    --hash=sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181
-    # via ha-services (pyproject.toml)
+flake8==6.1.0 \
+    --hash=sha256:d5b3857f07c030bdb5bf41c7f53799571d75c4491748a3adcd47de929e34cd23 \
+    --hash=sha256:ffdfce58ea94c6580c77888a86506937f9a1a227dfcd15f245d694ae20a6b6e5
+    # via
+    #   ha-services (pyproject.toml)
+    #   manageprojects
 flynt==0.77 \
     --hash=sha256:2863ac8ec19d6ec8d29e760546e6ced644baf6dff3c7cdc77e03abbd29b80f14 \
     --hash=sha256:2bd1b37043ad88a3f3c3c34a76fc0b64d24e5f03d36ea6b48cb69cc642bff17e
     # via darker
 idna==3.4 \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via requests
-importlib-metadata==6.6.0 \
-    --hash=sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed \
-    --hash=sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705
+importlib-metadata==6.8.0 \
+    --hash=sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb \
+    --hash=sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743
     # via
     #   keyring
     #   twine
 isort==5.12.0 \
     --hash=sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504 \
     --hash=sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6
     # via darker
-jaraco-classes==3.2.3 \
-    --hash=sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158 \
-    --hash=sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a
+jaraco-classes==3.3.0 \
+    --hash=sha256:10afa92b6743f25c0cf5f37c6bb6e18e2c5bb84a16527ccfc0040ea377e7aaeb \
+    --hash=sha256:c063dd08e89217cee02c8d5e5ec560f2c8ce6cdc2fcdc2e68f7b2e5547ed3621
     # via keyring
 jeepney==0.8.0 \
     --hash=sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806 \
     --hash=sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2 \
     --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
     --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
-    # via
-    #   cookiecutter
-    #   jinja2-time
-jinja2-time==0.2.0 \
-    --hash=sha256:d14eaa4d315e7688daa4969f616f226614350c48730bfa1692d2caebd8c90d40 \
-    --hash=sha256:d3eab6605e3ec8b7a0863df09cc1d23714908fa61aa6986a845c20ba488b4efa
     # via cookiecutter
-keyring==23.13.1 \
-    --hash=sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd \
-    --hash=sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678
+keyring==24.2.0 \
+    --hash=sha256:4901caaf597bfd3bbd78c9a0c7c4c29fcd8310dab2cffefe749e916b6527acd6 \
+    --hash=sha256:ca0746a19ec421219f4d713f848fa297a661a8a8c1504867e55bfb5e09091509
     # via twine
-manageprojects==0.10.0 \
-    --hash=sha256:939d9cf9c629be755c2ab6f8ccd4019dfa1c7e39564c25f6087ec2f63867133a \
-    --hash=sha256:db457b77e52a73e3ec5fd4889e056df01926ec0c9b1476ab28c79db254d0465f
-    # via ha-services (pyproject.toml)
-markdown-it-py==2.2.0 \
-    --hash=sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30 \
-    --hash=sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1
+manageprojects==0.13.0 \
+    --hash=sha256:9feff7b752b1d9710f69cf047bc0e51b73d29d30823e55409b7b6df239f1d501 \
+    --hash=sha256:e12b2ff0f59cf407426e6e11929d254a11e38c6a090b7eb53db3fd15fc2996cf
+    # via ha-services (pyproject.toml)
+markdown-it-py==3.0.0 \
+    --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
+    --hash=sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb
     # via rich
-markupsafe==2.1.2 \
-    --hash=sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed \
-    --hash=sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc \
-    --hash=sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2 \
-    --hash=sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460 \
-    --hash=sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7 \
-    --hash=sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0 \
-    --hash=sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1 \
-    --hash=sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa \
-    --hash=sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03 \
-    --hash=sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323 \
-    --hash=sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65 \
-    --hash=sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013 \
-    --hash=sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036 \
-    --hash=sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f \
-    --hash=sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4 \
-    --hash=sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419 \
-    --hash=sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2 \
-    --hash=sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619 \
-    --hash=sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a \
-    --hash=sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a \
-    --hash=sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd \
-    --hash=sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7 \
-    --hash=sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666 \
-    --hash=sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65 \
-    --hash=sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859 \
-    --hash=sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625 \
-    --hash=sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff \
-    --hash=sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156 \
-    --hash=sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd \
-    --hash=sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba \
-    --hash=sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f \
-    --hash=sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1 \
-    --hash=sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094 \
-    --hash=sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a \
-    --hash=sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513 \
-    --hash=sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed \
-    --hash=sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d \
-    --hash=sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3 \
-    --hash=sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147 \
-    --hash=sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c \
-    --hash=sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603 \
-    --hash=sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601 \
-    --hash=sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a \
-    --hash=sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1 \
-    --hash=sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d \
-    --hash=sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3 \
-    --hash=sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54 \
-    --hash=sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2 \
-    --hash=sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6 \
-    --hash=sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58
+markupsafe==2.1.3 \
+    --hash=sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e \
+    --hash=sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e \
+    --hash=sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431 \
+    --hash=sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686 \
+    --hash=sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559 \
+    --hash=sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc \
+    --hash=sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c \
+    --hash=sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0 \
+    --hash=sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4 \
+    --hash=sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9 \
+    --hash=sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575 \
+    --hash=sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba \
+    --hash=sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d \
+    --hash=sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3 \
+    --hash=sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00 \
+    --hash=sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155 \
+    --hash=sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac \
+    --hash=sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52 \
+    --hash=sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f \
+    --hash=sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8 \
+    --hash=sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b \
+    --hash=sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24 \
+    --hash=sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea \
+    --hash=sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198 \
+    --hash=sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0 \
+    --hash=sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee \
+    --hash=sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be \
+    --hash=sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2 \
+    --hash=sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707 \
+    --hash=sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6 \
+    --hash=sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58 \
+    --hash=sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779 \
+    --hash=sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636 \
+    --hash=sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c \
+    --hash=sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad \
+    --hash=sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee \
+    --hash=sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc \
+    --hash=sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2 \
+    --hash=sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48 \
+    --hash=sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7 \
+    --hash=sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e \
+    --hash=sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b \
+    --hash=sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa \
+    --hash=sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5 \
+    --hash=sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e \
+    --hash=sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb \
+    --hash=sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9 \
+    --hash=sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57 \
+    --hash=sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc \
+    --hash=sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2
     # via jinja2
 mccabe==0.7.0 \
     --hash=sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325 \
     --hash=sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e
     # via flake8
 mdurl==0.1.2 \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
     # via markdown-it-py
-more-itertools==9.1.0 \
-    --hash=sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d \
-    --hash=sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3
+more-itertools==10.1.0 \
+    --hash=sha256:626c369fa0eb37bac0291bce8259b332fd59ac792fa5497b59837309cd5b114a \
+    --hash=sha256:64e0735fcfdc6f3464ea133afe8ea4483b1c5fe3a3d69852e6503b43a0b222e6
     # via jaraco-classes
-msgspec==0.15.0 \
-    --hash=sha256:05fc603508e0c8021249d3e531fa4bb72d167bdfa76d869d48f96a5b8f9b50bf \
-    --hash=sha256:07ee1d1a15e3b319dcd7326470216928a7b58d47460b253577ccd0ab5dcf5c3c \
-    --hash=sha256:0c75fd847709e30265f050375c408fec1c07797694162834aa86ab3b3cf055da \
-    --hash=sha256:1b5b7c1b69416eab3ab2ad1c9593b749226b80555532292fae5fe9d154794089 \
-    --hash=sha256:20bf8018bff6bb85f5315ba6fd47b2f9373ab67e8bb59b0d7a7def22bbbf9f70 \
-    --hash=sha256:22713a1f618b4094c0268c6fbeef530397e5f3fa5292e4afd51caddad645843f \
-    --hash=sha256:2b57b6869ef1717c0343465198e19284d1e6aa5f292af2726284e4dfedfedeef \
-    --hash=sha256:346960762d648a6512b51f30be7c1267630e0bbc6fd65e8b23a3f54e5f562656 \
-    --hash=sha256:381c7a891adcc741e617956ba987912bc21864f9dd27b8cfb03bfb0aded5e1fd \
-    --hash=sha256:415519f68cd3f1a224f87ed415459ac3b86e4f6e82815a036e4238c62006f696 \
-    --hash=sha256:42c2f9fe0b58dc6f2b15720490c67554b5ba0007d3ee94340ca4448bda917287 \
-    --hash=sha256:490c88d76d573cce16653434ace3d9a8a8675ef6e350f114752fe60e69b6a232 \
-    --hash=sha256:4d3cde786110a92f764666b9f963b4389d5d1798bf1aca2422a59931d8d1f694 \
-    --hash=sha256:550b359c49562d52849103b87b4f7381fbc0adf958afa316599befb9a3e3379e \
-    --hash=sha256:8a46a9818570362d4022161684cdb97ecd102953043059ee4902862940f48f8d \
-    --hash=sha256:8b7e0354c37b742e1c02fe0cd3ced97db516c8da62ac5a408609e9f5858aaf24 \
-    --hash=sha256:8cee590163788fce21c5998d09198ef08ec06c1ca68ef50f2d5ed9e54d308538 \
-    --hash=sha256:9178a7550a5516295c682e6e5c143782503719b4c816496349a4a0f1b62397ef \
-    --hash=sha256:9d61de44b248feef82c8979a1e9912c923527cfb1d01c93b7bb5d6ca93ed09d6 \
-    --hash=sha256:beb3789519253b22338cca48053ba5ac8b442633e3af8f58e264d776a98ff6d0 \
-    --hash=sha256:bf3ab3f8d5752dbe68babc77d21b42575b916793515442e3890aef680e212154 \
-    --hash=sha256:c4c7e0abfac3a67f3e1d51e1d1313fd4205528e17663ff264b1945c3370b18bd \
-    --hash=sha256:cc253e4ad51d360590358ab2cee5a6139f04ad994e0fcbff52e7f61fca475c3e \
-    --hash=sha256:cd198ed4445914ebc25a24b6cc6020902bb6b888fc9b39500ef4500841b1b437 \
-    --hash=sha256:d760ff747165d84965791bfcd14588f61f111708036d80f1980387e3760035e7 \
-    --hash=sha256:ddef8fdc06676dd1bec9fe67b3128f84079469ee6424384cbb29a90c9033b559 \
-    --hash=sha256:f77cc91d3cb8a7bccfba28fe4aec537178384509bfce222f8eca287b7e5d0214 \
-    --hash=sha256:ff80bd40469915cc61686086a2503b901e17040f8a191099d8ccaa45dc72df8c \
-    --hash=sha256:fffa7ec85f27577f7f5471b390bf902d58ccd89b3612cf40bfb92f4ba75e6c95
-    # via ha-services (pyproject.toml)
-mypy==1.3.0 \
-    --hash=sha256:1c4c42c60a8103ead4c1c060ac3cdd3ff01e18fddce6f1016e08939647a0e703 \
-    --hash=sha256:44797d031a41516fcf5cbfa652265bb994e53e51994c1bd649ffcd0c3a7eccbf \
-    --hash=sha256:473117e310febe632ddf10e745a355714e771ffe534f06db40702775056614c4 \
-    --hash=sha256:4c99c3ecf223cf2952638da9cd82793d8f3c0c5fa8b6ae2b2d9ed1e1ff51ba85 \
-    --hash=sha256:550a8b3a19bb6589679a7c3c31f64312e7ff482a816c96e0cecec9ad3a7564dd \
-    --hash=sha256:658fe7b674769a0770d4b26cb4d6f005e88a442fe82446f020be8e5f5efb2fae \
-    --hash=sha256:6e33bb8b2613614a33dff70565f4c803f889ebd2f859466e42b46e1df76018dd \
-    --hash=sha256:6e42d29e324cdda61daaec2336c42512e59c7c375340bd202efa1fe0f7b8f8ca \
-    --hash=sha256:74bc9b6e0e79808bf8678d7678b2ae3736ea72d56eede3820bd3849823e7f305 \
-    --hash=sha256:76ec771e2342f1b558c36d49900dfe81d140361dd0d2df6cd71b3db1be155409 \
-    --hash=sha256:7d23370d2a6b7a71dc65d1266f9a34e4cde9e8e21511322415db4b26f46f6b8c \
-    --hash=sha256:87df44954c31d86df96c8bd6e80dfcd773473e877ac6176a8e29898bfb3501cb \
-    --hash=sha256:8c5979d0deb27e0f4479bee18ea0f83732a893e81b78e62e2dda3e7e518c92ee \
-    --hash=sha256:95d8d31a7713510685b05fbb18d6ac287a56c8f6554d88c19e73f724a445448a \
-    --hash=sha256:a22435632710a4fcf8acf86cbd0d69f68ac389a3892cb23fbad176d1cddaf228 \
-    --hash=sha256:a8763e72d5d9574d45ce5881962bc8e9046bf7b375b0abf031f3e6811732a897 \
-    --hash=sha256:c1eb485cea53f4f5284e5baf92902cd0088b24984f4209e25981cc359d64448d \
-    --hash=sha256:c5d2cc54175bab47011b09688b418db71403aefad07cbcd62d44010543fc143f \
-    --hash=sha256:cbc07246253b9e3d7d74c9ff948cd0fd7a71afcc2b77c7f0a59c26e9395cb152 \
-    --hash=sha256:d0b6c62206e04061e27009481cb0ec966f7d6172b5b936f3ead3d74f29fe3dcf \
-    --hash=sha256:ddae0f39ca146972ff6bb4399f3b2943884a774b8771ea0a8f50e971f5ea5ba8 \
-    --hash=sha256:e1f4d16e296f5135624b34e8fb741eb0eadedca90862405b1f1fde2040b9bd11 \
-    --hash=sha256:e86c2c6852f62f8f2b24cb7a613ebe8e0c7dc1402c61d36a609174f63e0ff017 \
-    --hash=sha256:ebc95f8386314272bbc817026f8ce8f4f0d2ef7ae44f947c4664efac9adec929 \
-    --hash=sha256:f9dca1e257d4cc129517779226753dbefb4f2266c4eaad610fc15c6a7e14283e \
-    --hash=sha256:faff86aa10c1aa4a10e1a301de160f3d8fc8703b88c7e98de46b531ff1276a9a
-    # via ha-services (pyproject.toml)
+msgspec==0.17.0 \
+    --hash=sha256:025986a5b1fd81c3dd1bb591bbc01ac03844b57685fcf4a14ed07ae1967b6d03 \
+    --hash=sha256:0aded9cd083d3a966610b6b01787106fa6aab495486420163a7b872704767da0 \
+    --hash=sha256:23581f8c1ffa488c2c3c78359868ee408528dad5e02af94e87e8d4773d118399 \
+    --hash=sha256:396908a124f633c3e267ec01b5bffdbefd592b15ddfda63c1af798e0102c35c8 \
+    --hash=sha256:3adc3f4016aa5ea1bd51c8d5c2a38172f1965dd231e03defed04ff2a0effb361 \
+    --hash=sha256:3d39dc3a44a479f35afcc21d97c4ea90a385afee0b766c7780ca2bda99480e3c \
+    --hash=sha256:4b0c52118aec347d15f75354b2fa27f1c9cd29b6ec12b74ef2ef988a0d702f5d \
+    --hash=sha256:4e2f2faeeb7aef5c2e4c78e375443134238ee966e54bba75cdb1936939673da7 \
+    --hash=sha256:51aec8ae03348525749f4eff4ed59fc7369383877ad65e0f00de3e357c4ecfa6 \
+    --hash=sha256:556413e59a8017c12a177218b3d3c16bb7217dc0371853b61e4c98df19515088 \
+    --hash=sha256:59ab1e250a84516413dee3542ff2b43f46fe521adfdc01e628198ce94553ff1e \
+    --hash=sha256:5f1b7c9d9f41b8c7724dc206aadbbe84d1641d20a1ff6dab04f0caf2a5bfd438 \
+    --hash=sha256:79c3ab0bac7dd6492f6c03e347f0e9e5187d9658b8e7c85fdc96dd4820de970b \
+    --hash=sha256:7ab367dd0b8a8c989d295e8ef086305e41a3c73fa3208322da4826f04e24b3c5 \
+    --hash=sha256:7e7e016cd79dc12935b6f5e8ff358ea5908cb84756c84a9fa2f3d8e5405740f3 \
+    --hash=sha256:80021321fea9be9e03c7675f6bdce06d9c91dbfb4aec78044cd243491ed49fa9 \
+    --hash=sha256:832e841d17bc2b4d74eee6aa16c818074cc9104c9a79466dbd49162600af8e9b \
+    --hash=sha256:86ca5710174970d9aeefc2ced4fcc4a27f5ff065840356cf1c747399aa4ad5a8 \
+    --hash=sha256:93fcff4e7923050cbfb3be8b4763a95862c3bf35d198684f3ebc3c486a1f66a5 \
+    --hash=sha256:98995159d95b4ed65c8cc185bd877fec67f41cb23925237a82efb066ef778fa8 \
+    --hash=sha256:9fb9f68ae2068a96b29d92cc4d142440e616b0a077b53a68b3445c62a2f31edc \
+    --hash=sha256:b5e49b9a302acee0808466b1af31c675d7cf8fd5ee78874109b5a44cb40c67e8 \
+    --hash=sha256:bc3f9fbb3d127a0c9734d43870b565a809c1fe2a0913d04170fa1222dfb131dc \
+    --hash=sha256:c1a0c8390014ee2b65d0d36d9cc28e74092166e8f44adf3dcb85e1ef25933787 \
+    --hash=sha256:c7bb4fa0021198cc87ece9fd4cbaa7241782f6c1d7b4fab71bb59c30e83c95c8 \
+    --hash=sha256:cccef9b4216c28f470855540d2649cbcf9eefd74c17984259ed3cbbaaa818c5d \
+    --hash=sha256:ce2a7da8669887b17bed92d3143aa0cc936fabdadcdd43c9ed09cfaca71a2fc5 \
+    --hash=sha256:de90a979e48e95ab6175a59f3f256a88984ff599edd5d3948993dfd6ecff83d0 \
+    --hash=sha256:f8096ca82e9a3e6fa09106bfac27eb8296c4cead02fdd297bb8af87254e58bad
+    # via ha-services (pyproject.toml)
+mypy==1.4.1 \
+    --hash=sha256:01fd2e9f85622d981fd9063bfaef1aed6e336eaacca00892cd2d82801ab7c042 \
+    --hash=sha256:0dde1d180cd84f0624c5dcaaa89c89775550a675aff96b5848de78fb11adabcd \
+    --hash=sha256:141dedfdbfe8a04142881ff30ce6e6653c9685b354876b12e4fe6c78598b45e2 \
+    --hash=sha256:16f0db5b641ba159eff72cff08edc3875f2b62b2fa2bc24f68c1e7a4e8232d01 \
+    --hash=sha256:190b6bab0302cec4e9e6767d3eb66085aef2a1cc98fe04936d8a42ed2ba77bb7 \
+    --hash=sha256:2460a58faeea905aeb1b9b36f5065f2dc9a9c6e4c992a6499a2360c6c74ceca3 \
+    --hash=sha256:34a9239d5b3502c17f07fd7c0b2ae6b7dd7d7f6af35fbb5072c6208e76295816 \
+    --hash=sha256:43b592511672017f5b1a483527fd2684347fdffc041c9ef53428c8dc530f79a3 \
+    --hash=sha256:43d24f6437925ce50139a310a64b2ab048cb2d3694c84c71c3f2a1626d8101dc \
+    --hash=sha256:45d32cec14e7b97af848bddd97d85ea4f0db4d5a149ed9676caa4eb2f7402bb4 \
+    --hash=sha256:470c969bb3f9a9efcedbadcd19a74ffb34a25f8e6b0e02dae7c0e71f8372f97b \
+    --hash=sha256:566e72b0cd6598503e48ea610e0052d1b8168e60a46e0bfd34b3acf2d57f96a8 \
+    --hash=sha256:5703097c4936bbb9e9bce41478c8d08edd2865e177dc4c52be759f81ee4dd26c \
+    --hash=sha256:7549fbf655e5825d787bbc9ecf6028731973f78088fbca3a1f4145c39ef09462 \
+    --hash=sha256:8207b7105829eca6f3d774f64a904190bb2231de91b8b186d21ffd98005f14a7 \
+    --hash=sha256:8c4d8e89aa7de683e2056a581ce63c46a0c41e31bd2b6d34144e2c80f5ea53dc \
+    --hash=sha256:98324ec3ecf12296e6422939e54763faedbfcc502ea4a4c38502082711867258 \
+    --hash=sha256:9bbcd9ab8ea1f2e1c8031c21445b511442cc45c89951e49bbf852cbb70755b1b \
+    --hash=sha256:9d40652cc4fe33871ad3338581dca3297ff5f2213d0df345bcfbde5162abf0c9 \
+    --hash=sha256:a2746d69a8196698146a3dbe29104f9eb6a2a4d8a27878d92169a6c0b74435b6 \
+    --hash=sha256:ae704dcfaa180ff7c4cfbad23e74321a2b774f92ca77fd94ce1049175a21c97f \
+    --hash=sha256:bfdca17c36ae01a21274a3c387a63aa1aafe72bff976522886869ef131b937f1 \
+    --hash=sha256:c482e1246726616088532b5e964e39765b6d1520791348e6c9dc3af25b233828 \
+    --hash=sha256:ca637024ca67ab24a7fd6f65d280572c3794665eaf5edcc7e90a866544076878 \
+    --hash=sha256:e02d700ec8d9b1859790c0475df4e4092c7bf3272a4fd2c9f33d87fac4427b8f \
+    --hash=sha256:e5952d2d18b79f7dc25e62e014fe5a23eb1a3d2bc66318df8988a01b1a037c5b
+    # via
+    #   ha-services (pyproject.toml)
+    #   manageprojects
 mypy-extensions==1.0.0 \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
     # via
     #   black
     #   mypy
 packaging==23.1 \
@@ -533,181 +553,187 @@
     #   dparse
     #   pyproject-api
     #   safety
     #   tox
 paho-mqtt==1.6.1 \
     --hash=sha256:2a8291c81623aec00372b5a85558a372c747cbca8e9934dfe218638b8eefc26f
     # via ha-services (pyproject.toml)
-pathspec==0.11.1 \
-    --hash=sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687 \
-    --hash=sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293
+pathspec==0.11.2 \
+    --hash=sha256:1d6ed233af05e679efb96b1851550ea95bbb64b7c490b0f5aa52996c11e92a20 \
+    --hash=sha256:e0d8d0ac2f12da61956eb2306b69f9469b42f4deb0f3cb6ed47b9cce9996ced3
     # via black
-pip-tools==6.13.0 \
-    --hash=sha256:50943f151d87e752abddec8158622c34ad7f292e193836e90e30d87da60b19d9 \
-    --hash=sha256:61d46bd2eb8016ed4a924e196e6e5b0a268cd3babd79e593048720db23522bb1
+pip-tools==7.2.0 \
+    --hash=sha256:360b8d30bc9ee2531857494afb98c41e96534f2eec9dad6500ae2a71f7c631c4 \
+    --hash=sha256:616488b539e14b8aa85436ed597a33c291f4885c1d2e0bec97400abe5aff2c0d
     # via ha-services (pyproject.toml)
 pkginfo==1.9.6 \
     --hash=sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546 \
     --hash=sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046
     # via twine
-platformdirs==3.5.1 \
-    --hash=sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f \
-    --hash=sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5
+platformdirs==3.10.0 \
+    --hash=sha256:b45696dab2d7cc691a3226759c0d3b00c47c8b6e293d96f6436f733303f77f6d \
+    --hash=sha256:d7c24979f292f916dc9cbf8648319032f551ea8c49a4c9bf2fb556a02070ec1d
     # via
     #   black
     #   tox
     #   virtualenv
-pluggy==1.0.0 \
-    --hash=sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159 \
-    --hash=sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3
+pluggy==1.2.0 \
+    --hash=sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849 \
+    --hash=sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3
     # via tox
-pycodestyle==2.10.0 \
-    --hash=sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053 \
-    --hash=sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610
+pycodestyle==2.11.0 \
+    --hash=sha256:259bcc17857d8a8b3b4a2327324b79e5f020a13c16074670f9c8c8f872ea76d0 \
+    --hash=sha256:5d1013ba8dc7895b548be5afb05740ca82454fd899971563d2ef625d090326f8
     # via
     #   autopep8
     #   flake8
 pycparser==2.21 \
     --hash=sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9 \
     --hash=sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206
     # via cffi
-pyflakes==3.0.1 \
-    --hash=sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf \
-    --hash=sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd
+pyflakes==3.1.0 \
+    --hash=sha256:4132f6d49cb4dae6819e5379898f2b8cce3c5f23994194c24b77d5da2e36f774 \
+    --hash=sha256:a0aae034c444db0071aa077972ba4768d40c830d9539fd45bf4cd3f8f6992efc
     # via
+    #   autoflake
     #   flake8
     #   ha-services (pyproject.toml)
-pygments==2.15.1 \
-    --hash=sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c \
-    --hash=sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1
+    #   manageprojects
+pygments==2.16.1 \
+    --hash=sha256:13fc09fa63bc8d8671a6d247e1eb303c4b343eaee81d861f3404db2935653692 \
+    --hash=sha256:1daff0494820c69bc8941e407aa20f577374ee88364ee10a98fdbe0aece96e29
     # via
     #   darker
     #   readme-renderer
     #   rich
-pyproject-api==1.5.1 \
-    --hash=sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9 \
-    --hash=sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43
+pyproject-api==1.5.3 \
+    --hash=sha256:14cf09828670c7b08842249c1f28c8ee6581b872e893f81b62d5465bec41502f \
+    --hash=sha256:ffb5b2d7cad43f5b2688ab490de7c4d3f6f15e0b819cb588c4b771567c9729eb
     # via tox
 pyproject-hooks==1.0.0 \
     --hash=sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8 \
     --hash=sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5
     # via build
 python-dateutil==2.8.2 \
     --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
     --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
     # via arrow
 python-slugify==8.0.1 \
     --hash=sha256:70ca6ea68fe63ecc8fa4fcf00ae651fc8a5d02d93dcd12ae6d4fc7ca46c4d395 \
     --hash=sha256:ce0d46ddb668b3be82f4ed5e503dbc33dd815d83e2eb6824211310d3fb172a27
     # via cookiecutter
-pyupgrade==3.4.0 \
-    --hash=sha256:98b6bee32149f662da1aa038cb9baf93d592ae696059acd613db6ff583583048 \
-    --hash=sha256:f6bcf0d5e59170d178a2630e981d0e7b04d9b13f3c0e7e62f3e6bab582f841e4
-    # via ha-services (pyproject.toml)
-pyyaml==6.0 \
-    --hash=sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf \
-    --hash=sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293 \
-    --hash=sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b \
-    --hash=sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57 \
-    --hash=sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b \
-    --hash=sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4 \
-    --hash=sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07 \
-    --hash=sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba \
-    --hash=sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9 \
-    --hash=sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287 \
-    --hash=sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513 \
-    --hash=sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0 \
-    --hash=sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782 \
-    --hash=sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0 \
-    --hash=sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92 \
-    --hash=sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f \
-    --hash=sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2 \
-    --hash=sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc \
-    --hash=sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1 \
-    --hash=sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c \
-    --hash=sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86 \
-    --hash=sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4 \
-    --hash=sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c \
-    --hash=sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34 \
-    --hash=sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b \
-    --hash=sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d \
-    --hash=sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c \
-    --hash=sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb \
-    --hash=sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7 \
-    --hash=sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737 \
-    --hash=sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3 \
-    --hash=sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d \
-    --hash=sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358 \
-    --hash=sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53 \
-    --hash=sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78 \
-    --hash=sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803 \
-    --hash=sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a \
-    --hash=sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f \
-    --hash=sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174 \
-    --hash=sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5
+pyupgrade==3.10.1 \
+    --hash=sha256:1d8d138c2ccdd3c42b1419230ae036d5607dc69465a26feacc069642fc8d1b90 \
+    --hash=sha256:f565b4d26daa46ed522e98746834e77e444269103f8bc04413d77dad95169a24
+    # via
+    #   ha-services (pyproject.toml)
+    #   manageprojects
+pyyaml==6.0.1 \
+    --hash=sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc \
+    --hash=sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741 \
+    --hash=sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206 \
+    --hash=sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27 \
+    --hash=sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595 \
+    --hash=sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62 \
+    --hash=sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98 \
+    --hash=sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696 \
+    --hash=sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d \
+    --hash=sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867 \
+    --hash=sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47 \
+    --hash=sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486 \
+    --hash=sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6 \
+    --hash=sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3 \
+    --hash=sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007 \
+    --hash=sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938 \
+    --hash=sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c \
+    --hash=sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735 \
+    --hash=sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d \
+    --hash=sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba \
+    --hash=sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8 \
+    --hash=sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5 \
+    --hash=sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd \
+    --hash=sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3 \
+    --hash=sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0 \
+    --hash=sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515 \
+    --hash=sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c \
+    --hash=sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c \
+    --hash=sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924 \
+    --hash=sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34 \
+    --hash=sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43 \
+    --hash=sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859 \
+    --hash=sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673 \
+    --hash=sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a \
+    --hash=sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab \
+    --hash=sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa \
+    --hash=sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c \
+    --hash=sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585 \
+    --hash=sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d \
+    --hash=sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f
     # via cookiecutter
-readme-renderer==37.3 \
-    --hash=sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273 \
-    --hash=sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343
+readme-renderer==40.0 \
+    --hash=sha256:9f77b519d96d03d7d7dce44977ba543090a14397c4f60de5b6eb5b8048110aa4 \
+    --hash=sha256:e18feb2a1e7706f2865b81ebb460056d93fb29d69daa10b223c00faa7bd9a00a
     # via twine
-requests==2.30.0 \
-    --hash=sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294 \
-    --hash=sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4
+requests==2.31.0 \
+    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
+    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via
     #   cookiecutter
     #   requests-toolbelt
     #   safety
     #   twine
 requests-toolbelt==1.0.0 \
     --hash=sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6 \
     --hash=sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06
     # via twine
 rfc3986==2.0.0 \
     --hash=sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd \
     --hash=sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c
     # via twine
-rich==13.3.5 \
-    --hash=sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c \
-    --hash=sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704
+rich==13.5.2 \
+    --hash=sha256:146a90b3b6b47cac4a73c12866a499e9817426423f57c5a66949c086191a8808 \
+    --hash=sha256:fb9d6c0a0f643c99eed3875b5377a184132ba9be4d61516a55273d3554d75a39
     # via
+    #   cookiecutter
     #   ha-services (pyproject.toml)
     #   manageprojects
     #   rich-click
     #   twine
 rich-click==1.6.1 \
     --hash=sha256:0fcf4d1a09029d79322dd814ab0b2e66ac183633037561881d45abae8a161d95 \
     --hash=sha256:f8ff96693ec6e261d1544e9f7d9a5811c5ef5d74c8adb4978430fc0dac16777e
     # via
     #   ha-services (pyproject.toml)
     #   manageprojects
-ruamel-yaml==0.17.26 \
-    --hash=sha256:25d0ee82a0a9a6f44683dcf8c282340def4074a4562f3a24f55695bb254c1693 \
-    --hash=sha256:baa2d0a5aad2034826c439ce61c142c07082b76f4791d54145e131206e998059
+ruamel-yaml==0.17.32 \
+    --hash=sha256:23cd2ed620231677564646b0c6a89d138b6822a0d78656df7abda5879ec4f447 \
+    --hash=sha256:ec939063761914e14542972a5cba6d33c23b0859ab6342f61cf070cfc600efc2
     # via safety
 ruamel-yaml-clib==0.2.7 \
     --hash=sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e \
     --hash=sha256:15910ef4f3e537eea7fe45f8a5d19997479940d9196f357152a09031c5be59f3 \
     --hash=sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5 \
+    --hash=sha256:1a6391a7cabb7641c32517539ca42cf84b87b667bad38b78d4d42dd23e957c81 \
     --hash=sha256:1f08fd5a2bea9c4180db71678e850b995d2a5f4537be0e94557668cf0f5f9497 \
     --hash=sha256:2aa261c29a5545adfef9296b7e33941f46aa5bbd21164228e833412af4c9c75f \
     --hash=sha256:3110a99e0f94a4a3470ff67fc20d3f96c25b13d24c6980ff841e82bafe827cac \
     --hash=sha256:3243f48ecd450eddadc2d11b5feb08aca941b5cd98c9b1db14b2fd128be8c697 \
     --hash=sha256:370445fd795706fd291ab00c9df38a0caed0f17a6fb46b0f607668ecb16ce763 \
     --hash=sha256:40d030e2329ce5286d6b231b8726959ebbe0404c92f0a578c0e2482182e38282 \
     --hash=sha256:41d0f1fa4c6830176eef5b276af04c89320ea616655d01327d5ce65e50575c94 \
     --hash=sha256:4a4d8d417868d68b979076a9be6a38c676eca060785abaa6709c7b31593c35d1 \
     --hash=sha256:4b3a93bb9bc662fc1f99c5c3ea8e623d8b23ad22f861eb6fce9377ac07ad6072 \
     --hash=sha256:5bc0667c1eb8f83a3752b71b9c4ba55ef7c7058ae57022dd9b29065186a113d9 \
-    --hash=sha256:721bc4ba4525f53f6a611ec0967bdcee61b31df5a56801281027a3a6d1c2daf5 \
     --hash=sha256:763d65baa3b952479c4e972669f679fe490eee058d5aa85da483ebae2009d231 \
     --hash=sha256:7bdb4c06b063f6fd55e472e201317a3bb6cdeeee5d5a38512ea5c01e1acbdd93 \
     --hash=sha256:8831a2cedcd0f0927f788c5bdf6567d9dc9cc235646a434986a852af1cb54b4b \
     --hash=sha256:91a789b4aa0097b78c93e3dc4b40040ba55bef518f84a40d4442f713b4094acb \
     --hash=sha256:92460ce908546ab69770b2e576e4f99fbb4ce6ab4b245345a3869a0a0410488f \
     --hash=sha256:99e77daab5d13a48a4054803d052ff40780278240a902b880dd37a51ba01a307 \
+    --hash=sha256:9c7617df90c1365638916b98cdd9be833d31d337dbcd722485597b43c4a215bf \
     --hash=sha256:a234a20ae07e8469da311e182e70ef6b199d0fbeb6c6cc2901204dd87fb867e8 \
     --hash=sha256:a7b301ff08055d73223058b5c46c55638917f04d21577c95e00e0c4d79201a6b \
     --hash=sha256:be2a7ad8fd8f7442b24323d24ba0b56c51219513cfa45b9ada3b87b76c374d4b \
     --hash=sha256:bf9a6bc4a0221538b1a7de3ed7bca4c93c02346853f44e1cd764be0023cd3640 \
     --hash=sha256:c3ca1fbba4ae962521e5eb66d72998b51f0f4d0f608d3c0347a48e1af262efa7 \
     --hash=sha256:d000f258cf42fec2b1bbf2863c61d7b8918d31ffee905da62dede869254d3b8a \
     --hash=sha256:d5859983f26d8cd7bb5c287ef452e8aacc86501487634573d260968f753e1d71 \
@@ -735,82 +761,83 @@
     # via
     #   bleach
     #   python-dateutil
 text-unidecode==1.3 \
     --hash=sha256:1311f10e8b895935241623731c2ba64f4c455287888b18189350b67134a822e8 \
     --hash=sha256:bad6603bb14d279193107714b288be206cac565dfa49aa5b105294dd5c4aab93
     # via python-slugify
-tokenize-rt==5.0.0 \
-    --hash=sha256:3160bc0c3e8491312d0485171dea861fc160a240f5f5766b72a1165408d10740 \
-    --hash=sha256:c67772c662c6b3dc65edf66808577968fb10badfc2042e3027196bed4daf9e5a
+tokenize-rt==5.2.0 \
+    --hash=sha256:9fe80f8a5c1edad2d3ede0f37481cc0cc1538a2f442c9c2f9e4feacd2792d054 \
+    --hash=sha256:b79d41a65cfec71285433511b50271b05da3584a1da144a0752e9c621a285289
     # via pyupgrade
 toml==0.10.2 \
     --hash=sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b \
     --hash=sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f
-    # via
-    #   darker
-    #   dparse
+    # via darker
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via
+    #   autoflake
     #   autopep8
     #   black
     #   build
+    #   dparse
     #   flynt
     #   ha-services (pyproject.toml)
     #   mypy
+    #   pip-tools
     #   pyproject-api
     #   pyproject-hooks
     #   tox
-tomlkit==0.11.8 \
-    --hash=sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171 \
-    --hash=sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3
+tomlkit==0.12.1 \
+    --hash=sha256:38e1ff8edb991273ec9f6181244a6a391ac30e9f5098e7535640ea6be97a7c86 \
+    --hash=sha256:712cbd236609acc6a3e2e97253dfc52d4c2082982a88f61b640ecf0817eab899
     # via
     #   ha-services (pyproject.toml)
     #   manageprojects
-tox==4.5.1 \
-    --hash=sha256:5a2eac5fb816779dfdf5cb00fecbc27eb0524e4626626bb1de84747b24cacc56 \
-    --hash=sha256:d25a2e6cb261adc489604fafd76cd689efeadfa79709965e965668d6d3f63046
+tox==4.7.0 \
+    --hash=sha256:79399a3d4641d1fd15eb6bd62c2f35923988038bf0ecf37a688b5e7a767de7d7 \
+    --hash=sha256:89120e1568c763924301cfde61ba7d4b5c4615eeb1086d5370deb03e9cf63c41
     # via ha-services (pyproject.toml)
 twine==4.0.2 \
     --hash=sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8 \
     --hash=sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8
     # via ha-services (pyproject.toml)
-typing-extensions==4.5.0 \
-    --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
-    --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
+typing-extensions==4.7.1 \
+    --hash=sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36 \
+    --hash=sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2
     # via mypy
-urllib3==2.0.2 \
-    --hash=sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc \
-    --hash=sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e
+urllib3==2.0.4 \
+    --hash=sha256:8d22f86aae8ef5e410d4f539fde9ce6b2113a001bb4d189e0aed70642d602b11 \
+    --hash=sha256:de7df1803967d2c2a98e4b11bb7d6bd9210474c46e8a0401514e3a42a75ebde4
     # via
     #   requests
     #   twine
-virtualenv==20.23.0 \
-    --hash=sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e \
-    --hash=sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924
+virtualenv==20.24.2 \
+    --hash=sha256:43a3052be36080548bdee0b42919c88072037d50d56c28bd3f853cbe92b953ff \
+    --hash=sha256:fd8a78f46f6b99a67b7ec5cf73f92357891a7b3a40fd97637c27f854aae3b9e0
     # via tox
 webencodings==0.5.1 \
     --hash=sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78 \
     --hash=sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923
     # via bleach
-wheel==0.40.0 \
-    --hash=sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873 \
-    --hash=sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247
+wheel==0.41.1 \
+    --hash=sha256:12b911f083e876e10c595779709f8a88a59f45aacc646492a67fe9ef796c1b47 \
+    --hash=sha256:473219bd4cbedc62cea0cb309089b593e47c15c4a2531015f94e4e3b9a0f6981
     # via pip-tools
-zipp==3.15.0 \
-    --hash=sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b \
-    --hash=sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556
+zipp==3.16.2 \
+    --hash=sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0 \
+    --hash=sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==23.1.2 \
-    --hash=sha256:0e7c86f486935893c708287b30bd050a36ac827ec7fe5e43fe7cb198dd835fba \
-    --hash=sha256:3ef6ac33239e4027d9a5598a381b9d30880a1477e50039db2eac6e8a8f6d1b18
+pip==23.2.1 \
+    --hash=sha256:7ccf472345f20d35bdc9d1841ff5f313260c2c33fe417f48c30ac46cccabf5be \
+    --hash=sha256:fb0bd5435b3200c602b5bf61d2d43c2f13c02e29c1707567ae7fbc514eb9faf2
     # via pip-tools
-setuptools==67.7.2 \
-    --hash=sha256:23aaf86b85ca52ceb801d32703f12d77517b2556af839621c641fca11287952b \
-    --hash=sha256:f104fa03692a2602fa0fec6c6a9e63b6c8a968de13e17c026957dd1f53d80990
+setuptools==68.0.0 \
+    --hash=sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f \
+    --hash=sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235
     # via
     #   pip-tools
     #   safety
```

### Comparing `ha-services-0.3.2/requirements.txt` & `ha-services-0.3.3/requirements.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,296 +3,421 @@
 # by the following command:
 #
 #    ./cli.py update
 #
 arrow==1.2.3 \
     --hash=sha256:3934b30ca1b9f292376d9db15b19446088d12ec58629bc3f0da28fd55fb633a1 \
     --hash=sha256:5a49ab92e3b7b71d96cd6bfcc4df14efefc9dfa96ea19045815914a6ab6b1fe2
-    # via jinja2-time
+    # via cookiecutter
+astor==0.8.1 \
+    --hash=sha256:070a54e890cefb5b3739d19f30f5a5ec840ffc9c50ffa7d23cc9fc1a38ebbfc5 \
+    --hash=sha256:6a6effda93f4e1ce9f618779b2dd1d9d84f1e32812c23a29b3fff6fd7f63fa5e
+    # via flynt
+autoflake==2.2.0 \
+    --hash=sha256:62e1f74a0fdad898a96fee6f99fe8241af90ad99c7110c884b35855778412251 \
+    --hash=sha256:de409b009a34c1c2a7cc2aae84c4c05047f9773594317c6a6968bd497600d4a0
+    # via manageprojects
+autopep8==2.0.2 \
+    --hash=sha256:86e9303b5e5c8160872b2f5ef611161b2893e9bfe8ccc7e2f76385947d57a2f1 \
+    --hash=sha256:f9849cdd62108cb739dbcdbfb7fdcc9a30d1b63c4cc3e1c1f893b5360941b61c
+    # via manageprojects
 binaryornot==0.4.4 \
     --hash=sha256:359501dfc9d40632edc9fac890e19542db1a287bbcfa58175b66658392018061 \
     --hash=sha256:b8b71173c917bddcd2c16070412e369c3ed7f0528926f70cac18a6c97fd563e4
     # via cookiecutter
-bx-py-utils==81 \
-    --hash=sha256:5c2e189cccbeb852b058078bc7b0a8976f5f691ee7de657a87eef43fc89fa59a \
-    --hash=sha256:fd282f9e4ed8ed2842154ffe3fdd2ca56c428023021afc5b8ff765a53c02cddb
+black==23.7.0 \
+    --hash=sha256:01ede61aac8c154b55f35301fac3e730baf0c9cf8120f65a9cd61a81cfb4a0c3 \
+    --hash=sha256:022a582720b0d9480ed82576c920a8c1dde97cc38ff11d8d8859b3bd6ca9eedb \
+    --hash=sha256:25cc308838fe71f7065df53aedd20327969d05671bac95b38fdf37ebe70ac087 \
+    --hash=sha256:27eb7a0c71604d5de083757fbdb245b1a4fae60e9596514c6ec497eb63f95320 \
+    --hash=sha256:327a8c2550ddc573b51e2c352adb88143464bb9d92c10416feb86b0f5aee5ff6 \
+    --hash=sha256:47e56d83aad53ca140da0af87678fb38e44fd6bc0af71eebab2d1f59b1acf1d3 \
+    --hash=sha256:501387a9edcb75d7ae8a4412bb8749900386eaef258f1aefab18adddea1936bc \
+    --hash=sha256:552513d5cd5694590d7ef6f46e1767a4df9af168d449ff767b13b084c020e63f \
+    --hash=sha256:5c4bc552ab52f6c1c506ccae05681fab58c3f72d59ae6e6639e8885e94fe2587 \
+    --hash=sha256:642496b675095d423f9b8448243336f8ec71c9d4d57ec17bf795b67f08132a91 \
+    --hash=sha256:6d1c6022b86f83b632d06f2b02774134def5d4d4f1dac8bef16d90cda18ba28a \
+    --hash=sha256:7f3bf2dec7d541b4619b8ce526bda74a6b0bffc480a163fed32eb8b3c9aed8ad \
+    --hash=sha256:831d8f54c3a8c8cf55f64d0422ee875eecac26f5f649fb6c1df65316b67c8926 \
+    --hash=sha256:8417dbd2f57b5701492cd46edcecc4f9208dc75529bcf76c514864e48da867d9 \
+    --hash=sha256:86cee259349b4448adb4ef9b204bb4467aae74a386bce85d56ba4f5dc0da27be \
+    --hash=sha256:893695a76b140881531062d48476ebe4a48f5d1e9388177e175d76234ca247cd \
+    --hash=sha256:9fd59d418c60c0348505f2ddf9609c1e1de8e7493eab96198fc89d9f865e7a96 \
+    --hash=sha256:ad0014efc7acf0bd745792bd0d8857413652979200ab924fbf239062adc12491 \
+    --hash=sha256:b5b0ee6d96b345a8b420100b7d71ebfdd19fab5e8301aff48ec270042cd40ac2 \
+    --hash=sha256:c333286dc3ddca6fdff74670b911cccedacb4ef0a60b34e491b8a67c833b343a \
+    --hash=sha256:f9062af71c59c004cd519e2fb8f5d25d39e46d3af011b41ab43b9c74e27e236f \
+    --hash=sha256:fb074d8b213749fa1d077d630db0d5f8cc3b2ae63587ad4116e8a436e9bbe995
+    # via darker
+bx-py-utils==85 \
+    --hash=sha256:8d6ee4bb0c431304b812f5bebb1bc8e2ab05f1b6c2f8d16d352cbcee5e916cd2 \
+    --hash=sha256:df023fa05cda8e969d2cbdb4cc348d8b7670567a2fe775faf7a0c869ec56eaa2
     # via
     #   ha-services (pyproject.toml)
     #   manageprojects
-certifi==2023.5.7 \
-    --hash=sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7 \
-    --hash=sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716
+certifi==2023.7.22 \
+    --hash=sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082 \
+    --hash=sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9
     # via requests
-chardet==5.1.0 \
-    --hash=sha256:0d62712b956bc154f85fb0a266e2a3c5913c2967e00348701b32411d6def31e5 \
-    --hash=sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9
+chardet==5.2.0 \
+    --hash=sha256:1b3b6ff479a8c414bc3fa2c0852995695c4a026dcd6d0633b2dd092ca39c1cf7 \
+    --hash=sha256:e1cf59446890a00105fe7b7912492ea04b6e6f06d4b742b2c788469e34c82970
     # via binaryornot
-charset-normalizer==3.1.0 \
-    --hash=sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6 \
-    --hash=sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1 \
-    --hash=sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e \
-    --hash=sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373 \
-    --hash=sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62 \
-    --hash=sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230 \
-    --hash=sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be \
-    --hash=sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c \
-    --hash=sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0 \
-    --hash=sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448 \
-    --hash=sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f \
-    --hash=sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649 \
-    --hash=sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d \
-    --hash=sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0 \
-    --hash=sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706 \
-    --hash=sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a \
-    --hash=sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59 \
-    --hash=sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23 \
-    --hash=sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5 \
-    --hash=sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb \
-    --hash=sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e \
-    --hash=sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e \
-    --hash=sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c \
-    --hash=sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28 \
-    --hash=sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d \
-    --hash=sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41 \
-    --hash=sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974 \
-    --hash=sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce \
-    --hash=sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f \
-    --hash=sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1 \
-    --hash=sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d \
-    --hash=sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8 \
-    --hash=sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017 \
-    --hash=sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31 \
-    --hash=sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7 \
-    --hash=sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8 \
-    --hash=sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e \
-    --hash=sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14 \
-    --hash=sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd \
-    --hash=sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d \
-    --hash=sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795 \
-    --hash=sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b \
-    --hash=sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b \
-    --hash=sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b \
-    --hash=sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203 \
-    --hash=sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f \
-    --hash=sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19 \
-    --hash=sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1 \
-    --hash=sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a \
-    --hash=sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac \
-    --hash=sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9 \
-    --hash=sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0 \
-    --hash=sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137 \
-    --hash=sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f \
-    --hash=sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6 \
-    --hash=sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5 \
-    --hash=sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909 \
-    --hash=sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f \
-    --hash=sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0 \
-    --hash=sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324 \
-    --hash=sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755 \
-    --hash=sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb \
-    --hash=sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854 \
-    --hash=sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c \
-    --hash=sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60 \
-    --hash=sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84 \
-    --hash=sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0 \
-    --hash=sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b \
-    --hash=sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1 \
-    --hash=sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531 \
-    --hash=sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1 \
-    --hash=sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11 \
-    --hash=sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326 \
-    --hash=sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df \
-    --hash=sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab
+charset-normalizer==3.2.0 \
+    --hash=sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96 \
+    --hash=sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c \
+    --hash=sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710 \
+    --hash=sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706 \
+    --hash=sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020 \
+    --hash=sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252 \
+    --hash=sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad \
+    --hash=sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329 \
+    --hash=sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a \
+    --hash=sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f \
+    --hash=sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6 \
+    --hash=sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4 \
+    --hash=sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a \
+    --hash=sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46 \
+    --hash=sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2 \
+    --hash=sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23 \
+    --hash=sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace \
+    --hash=sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd \
+    --hash=sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982 \
+    --hash=sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10 \
+    --hash=sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2 \
+    --hash=sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea \
+    --hash=sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09 \
+    --hash=sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5 \
+    --hash=sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149 \
+    --hash=sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489 \
+    --hash=sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9 \
+    --hash=sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80 \
+    --hash=sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592 \
+    --hash=sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3 \
+    --hash=sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6 \
+    --hash=sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed \
+    --hash=sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c \
+    --hash=sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200 \
+    --hash=sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a \
+    --hash=sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e \
+    --hash=sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d \
+    --hash=sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6 \
+    --hash=sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623 \
+    --hash=sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669 \
+    --hash=sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3 \
+    --hash=sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa \
+    --hash=sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9 \
+    --hash=sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2 \
+    --hash=sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f \
+    --hash=sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1 \
+    --hash=sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4 \
+    --hash=sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a \
+    --hash=sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8 \
+    --hash=sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3 \
+    --hash=sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029 \
+    --hash=sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f \
+    --hash=sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959 \
+    --hash=sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22 \
+    --hash=sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7 \
+    --hash=sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952 \
+    --hash=sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346 \
+    --hash=sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e \
+    --hash=sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d \
+    --hash=sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299 \
+    --hash=sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd \
+    --hash=sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a \
+    --hash=sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3 \
+    --hash=sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037 \
+    --hash=sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94 \
+    --hash=sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c \
+    --hash=sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858 \
+    --hash=sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a \
+    --hash=sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449 \
+    --hash=sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c \
+    --hash=sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918 \
+    --hash=sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1 \
+    --hash=sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c \
+    --hash=sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac \
+    --hash=sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa
     # via requests
-click==8.1.3 \
-    --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
-    --hash=sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48
+click==8.1.6 \
+    --hash=sha256:48ee849951919527a045bfe3bf7baa8a959c423134e1a5b98c05c20ba75a1cbd \
+    --hash=sha256:fa244bb30b3b5ee2cae3da8f55c9e5e0c0e86093306301fb418eb9dc40fbded5
     # via
+    #   black
     #   cookiecutter
     #   ha-services (pyproject.toml)
     #   manageprojects
     #   rich-click
-cookiecutter==2.1.1 \
-    --hash=sha256:9f3ab027cec4f70916e28f03470bdb41e637a3ad354b4d65c765d93aad160022 \
-    --hash=sha256:f3982be8d9c53dac1261864013fdec7f83afd2e42ede6f6dd069c5e149c540d5
+codespell==2.2.5 \
+    --hash=sha256:6d9faddf6eedb692bf80c9a94ec13ab4f5fb585aabae5f3750727148d7b5be56 \
+    --hash=sha256:efa037f54b73c84f7bd14ce8e853d5f822cdd6386ef0ff32e957a3919435b9ec
+    # via manageprojects
+cookiecutter==2.3.0 \
+    --hash=sha256:7e87944757c6e9f8729cf89a4139b6a35ab4d6dcbc6ae3e7d6360d44ad3ad383 \
+    --hash=sha256:942a794981747f6d7f439d6e49d39dc91a9a641283614160c93c474c72c29621
+    # via manageprojects
+darker[color,flynt,isort]==1.7.2 \
+    --hash=sha256:ec5b7c382d9537611c164f3ecca2e1b8a7923bc5a02bf22f6e7f6c8bcbdf593a \
+    --hash=sha256:ec9d130ab2a0f7fa49ab68a08fd231a5bec66147ecbbf94c92a1f33d97b5ef6f
     # via manageprojects
+editorconfig==0.12.3 \
+    --hash=sha256:57f8ce78afcba15c8b18d46b5170848c88d56fd38f05c2ec60dbbfcb8996e89e \
+    --hash=sha256:6b0851425aa875b08b16789ee0eeadbd4ab59666e9ebe728e526314c4a2e52c1
+    # via manageprojects
+flake8==6.1.0 \
+    --hash=sha256:d5b3857f07c030bdb5bf41c7f53799571d75c4491748a3adcd47de929e34cd23 \
+    --hash=sha256:ffdfce58ea94c6580c77888a86506937f9a1a227dfcd15f245d694ae20a6b6e5
+    # via manageprojects
+flynt==0.77 \
+    --hash=sha256:2863ac8ec19d6ec8d29e760546e6ced644baf6dff3c7cdc77e03abbd29b80f14 \
+    --hash=sha256:2bd1b37043ad88a3f3c3c34a76fc0b64d24e5f03d36ea6b48cb69cc642bff17e
+    # via darker
 idna==3.4 \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via requests
+isort==5.12.0 \
+    --hash=sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504 \
+    --hash=sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6
+    # via darker
 jinja2==3.1.2 \
     --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
     --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
-    # via
-    #   cookiecutter
-    #   jinja2-time
-jinja2-time==0.2.0 \
-    --hash=sha256:d14eaa4d315e7688daa4969f616f226614350c48730bfa1692d2caebd8c90d40 \
-    --hash=sha256:d3eab6605e3ec8b7a0863df09cc1d23714908fa61aa6986a845c20ba488b4efa
     # via cookiecutter
-manageprojects==0.10.0 \
-    --hash=sha256:939d9cf9c629be755c2ab6f8ccd4019dfa1c7e39564c25f6087ec2f63867133a \
-    --hash=sha256:db457b77e52a73e3ec5fd4889e056df01926ec0c9b1476ab28c79db254d0465f
+manageprojects==0.13.0 \
+    --hash=sha256:9feff7b752b1d9710f69cf047bc0e51b73d29d30823e55409b7b6df239f1d501 \
+    --hash=sha256:e12b2ff0f59cf407426e6e11929d254a11e38c6a090b7eb53db3fd15fc2996cf
     # via ha-services (pyproject.toml)
-markdown-it-py==2.2.0 \
-    --hash=sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30 \
-    --hash=sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1
+markdown-it-py==3.0.0 \
+    --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
+    --hash=sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb
     # via rich
-markupsafe==2.1.2 \
-    --hash=sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed \
-    --hash=sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc \
-    --hash=sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2 \
-    --hash=sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460 \
-    --hash=sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7 \
-    --hash=sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0 \
-    --hash=sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1 \
-    --hash=sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa \
-    --hash=sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03 \
-    --hash=sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323 \
-    --hash=sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65 \
-    --hash=sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013 \
-    --hash=sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036 \
-    --hash=sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f \
-    --hash=sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4 \
-    --hash=sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419 \
-    --hash=sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2 \
-    --hash=sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619 \
-    --hash=sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a \
-    --hash=sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a \
-    --hash=sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd \
-    --hash=sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7 \
-    --hash=sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666 \
-    --hash=sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65 \
-    --hash=sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859 \
-    --hash=sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625 \
-    --hash=sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff \
-    --hash=sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156 \
-    --hash=sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd \
-    --hash=sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba \
-    --hash=sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f \
-    --hash=sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1 \
-    --hash=sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094 \
-    --hash=sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a \
-    --hash=sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513 \
-    --hash=sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed \
-    --hash=sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d \
-    --hash=sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3 \
-    --hash=sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147 \
-    --hash=sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c \
-    --hash=sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603 \
-    --hash=sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601 \
-    --hash=sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a \
-    --hash=sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1 \
-    --hash=sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d \
-    --hash=sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3 \
-    --hash=sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54 \
-    --hash=sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2 \
-    --hash=sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6 \
-    --hash=sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58
+markupsafe==2.1.3 \
+    --hash=sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e \
+    --hash=sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e \
+    --hash=sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431 \
+    --hash=sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686 \
+    --hash=sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559 \
+    --hash=sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc \
+    --hash=sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c \
+    --hash=sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0 \
+    --hash=sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4 \
+    --hash=sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9 \
+    --hash=sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575 \
+    --hash=sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba \
+    --hash=sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d \
+    --hash=sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3 \
+    --hash=sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00 \
+    --hash=sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155 \
+    --hash=sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac \
+    --hash=sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52 \
+    --hash=sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f \
+    --hash=sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8 \
+    --hash=sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b \
+    --hash=sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24 \
+    --hash=sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea \
+    --hash=sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198 \
+    --hash=sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0 \
+    --hash=sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee \
+    --hash=sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be \
+    --hash=sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2 \
+    --hash=sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707 \
+    --hash=sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6 \
+    --hash=sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58 \
+    --hash=sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779 \
+    --hash=sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636 \
+    --hash=sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c \
+    --hash=sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad \
+    --hash=sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee \
+    --hash=sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc \
+    --hash=sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2 \
+    --hash=sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48 \
+    --hash=sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7 \
+    --hash=sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e \
+    --hash=sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b \
+    --hash=sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa \
+    --hash=sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5 \
+    --hash=sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e \
+    --hash=sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb \
+    --hash=sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9 \
+    --hash=sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57 \
+    --hash=sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc \
+    --hash=sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2
     # via jinja2
+mccabe==0.7.0 \
+    --hash=sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325 \
+    --hash=sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e
+    # via flake8
 mdurl==0.1.2 \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
     # via markdown-it-py
-msgspec==0.15.0 \
-    --hash=sha256:05fc603508e0c8021249d3e531fa4bb72d167bdfa76d869d48f96a5b8f9b50bf \
-    --hash=sha256:07ee1d1a15e3b319dcd7326470216928a7b58d47460b253577ccd0ab5dcf5c3c \
-    --hash=sha256:0c75fd847709e30265f050375c408fec1c07797694162834aa86ab3b3cf055da \
-    --hash=sha256:1b5b7c1b69416eab3ab2ad1c9593b749226b80555532292fae5fe9d154794089 \
-    --hash=sha256:20bf8018bff6bb85f5315ba6fd47b2f9373ab67e8bb59b0d7a7def22bbbf9f70 \
-    --hash=sha256:22713a1f618b4094c0268c6fbeef530397e5f3fa5292e4afd51caddad645843f \
-    --hash=sha256:2b57b6869ef1717c0343465198e19284d1e6aa5f292af2726284e4dfedfedeef \
-    --hash=sha256:346960762d648a6512b51f30be7c1267630e0bbc6fd65e8b23a3f54e5f562656 \
-    --hash=sha256:381c7a891adcc741e617956ba987912bc21864f9dd27b8cfb03bfb0aded5e1fd \
-    --hash=sha256:415519f68cd3f1a224f87ed415459ac3b86e4f6e82815a036e4238c62006f696 \
-    --hash=sha256:42c2f9fe0b58dc6f2b15720490c67554b5ba0007d3ee94340ca4448bda917287 \
-    --hash=sha256:490c88d76d573cce16653434ace3d9a8a8675ef6e350f114752fe60e69b6a232 \
-    --hash=sha256:4d3cde786110a92f764666b9f963b4389d5d1798bf1aca2422a59931d8d1f694 \
-    --hash=sha256:550b359c49562d52849103b87b4f7381fbc0adf958afa316599befb9a3e3379e \
-    --hash=sha256:8a46a9818570362d4022161684cdb97ecd102953043059ee4902862940f48f8d \
-    --hash=sha256:8b7e0354c37b742e1c02fe0cd3ced97db516c8da62ac5a408609e9f5858aaf24 \
-    --hash=sha256:8cee590163788fce21c5998d09198ef08ec06c1ca68ef50f2d5ed9e54d308538 \
-    --hash=sha256:9178a7550a5516295c682e6e5c143782503719b4c816496349a4a0f1b62397ef \
-    --hash=sha256:9d61de44b248feef82c8979a1e9912c923527cfb1d01c93b7bb5d6ca93ed09d6 \
-    --hash=sha256:beb3789519253b22338cca48053ba5ac8b442633e3af8f58e264d776a98ff6d0 \
-    --hash=sha256:bf3ab3f8d5752dbe68babc77d21b42575b916793515442e3890aef680e212154 \
-    --hash=sha256:c4c7e0abfac3a67f3e1d51e1d1313fd4205528e17663ff264b1945c3370b18bd \
-    --hash=sha256:cc253e4ad51d360590358ab2cee5a6139f04ad994e0fcbff52e7f61fca475c3e \
-    --hash=sha256:cd198ed4445914ebc25a24b6cc6020902bb6b888fc9b39500ef4500841b1b437 \
-    --hash=sha256:d760ff747165d84965791bfcd14588f61f111708036d80f1980387e3760035e7 \
-    --hash=sha256:ddef8fdc06676dd1bec9fe67b3128f84079469ee6424384cbb29a90c9033b559 \
-    --hash=sha256:f77cc91d3cb8a7bccfba28fe4aec537178384509bfce222f8eca287b7e5d0214 \
-    --hash=sha256:ff80bd40469915cc61686086a2503b901e17040f8a191099d8ccaa45dc72df8c \
-    --hash=sha256:fffa7ec85f27577f7f5471b390bf902d58ccd89b3612cf40bfb92f4ba75e6c95
+msgspec==0.17.0 \
+    --hash=sha256:025986a5b1fd81c3dd1bb591bbc01ac03844b57685fcf4a14ed07ae1967b6d03 \
+    --hash=sha256:0aded9cd083d3a966610b6b01787106fa6aab495486420163a7b872704767da0 \
+    --hash=sha256:23581f8c1ffa488c2c3c78359868ee408528dad5e02af94e87e8d4773d118399 \
+    --hash=sha256:396908a124f633c3e267ec01b5bffdbefd592b15ddfda63c1af798e0102c35c8 \
+    --hash=sha256:3adc3f4016aa5ea1bd51c8d5c2a38172f1965dd231e03defed04ff2a0effb361 \
+    --hash=sha256:3d39dc3a44a479f35afcc21d97c4ea90a385afee0b766c7780ca2bda99480e3c \
+    --hash=sha256:4b0c52118aec347d15f75354b2fa27f1c9cd29b6ec12b74ef2ef988a0d702f5d \
+    --hash=sha256:4e2f2faeeb7aef5c2e4c78e375443134238ee966e54bba75cdb1936939673da7 \
+    --hash=sha256:51aec8ae03348525749f4eff4ed59fc7369383877ad65e0f00de3e357c4ecfa6 \
+    --hash=sha256:556413e59a8017c12a177218b3d3c16bb7217dc0371853b61e4c98df19515088 \
+    --hash=sha256:59ab1e250a84516413dee3542ff2b43f46fe521adfdc01e628198ce94553ff1e \
+    --hash=sha256:5f1b7c9d9f41b8c7724dc206aadbbe84d1641d20a1ff6dab04f0caf2a5bfd438 \
+    --hash=sha256:79c3ab0bac7dd6492f6c03e347f0e9e5187d9658b8e7c85fdc96dd4820de970b \
+    --hash=sha256:7ab367dd0b8a8c989d295e8ef086305e41a3c73fa3208322da4826f04e24b3c5 \
+    --hash=sha256:7e7e016cd79dc12935b6f5e8ff358ea5908cb84756c84a9fa2f3d8e5405740f3 \
+    --hash=sha256:80021321fea9be9e03c7675f6bdce06d9c91dbfb4aec78044cd243491ed49fa9 \
+    --hash=sha256:832e841d17bc2b4d74eee6aa16c818074cc9104c9a79466dbd49162600af8e9b \
+    --hash=sha256:86ca5710174970d9aeefc2ced4fcc4a27f5ff065840356cf1c747399aa4ad5a8 \
+    --hash=sha256:93fcff4e7923050cbfb3be8b4763a95862c3bf35d198684f3ebc3c486a1f66a5 \
+    --hash=sha256:98995159d95b4ed65c8cc185bd877fec67f41cb23925237a82efb066ef778fa8 \
+    --hash=sha256:9fb9f68ae2068a96b29d92cc4d142440e616b0a077b53a68b3445c62a2f31edc \
+    --hash=sha256:b5e49b9a302acee0808466b1af31c675d7cf8fd5ee78874109b5a44cb40c67e8 \
+    --hash=sha256:bc3f9fbb3d127a0c9734d43870b565a809c1fe2a0913d04170fa1222dfb131dc \
+    --hash=sha256:c1a0c8390014ee2b65d0d36d9cc28e74092166e8f44adf3dcb85e1ef25933787 \
+    --hash=sha256:c7bb4fa0021198cc87ece9fd4cbaa7241782f6c1d7b4fab71bb59c30e83c95c8 \
+    --hash=sha256:cccef9b4216c28f470855540d2649cbcf9eefd74c17984259ed3cbbaaa818c5d \
+    --hash=sha256:ce2a7da8669887b17bed92d3143aa0cc936fabdadcdd43c9ed09cfaca71a2fc5 \
+    --hash=sha256:de90a979e48e95ab6175a59f3f256a88984ff599edd5d3948993dfd6ecff83d0 \
+    --hash=sha256:f8096ca82e9a3e6fa09106bfac27eb8296c4cead02fdd297bb8af87254e58bad
     # via ha-services (pyproject.toml)
+mypy==1.4.1 \
+    --hash=sha256:01fd2e9f85622d981fd9063bfaef1aed6e336eaacca00892cd2d82801ab7c042 \
+    --hash=sha256:0dde1d180cd84f0624c5dcaaa89c89775550a675aff96b5848de78fb11adabcd \
+    --hash=sha256:141dedfdbfe8a04142881ff30ce6e6653c9685b354876b12e4fe6c78598b45e2 \
+    --hash=sha256:16f0db5b641ba159eff72cff08edc3875f2b62b2fa2bc24f68c1e7a4e8232d01 \
+    --hash=sha256:190b6bab0302cec4e9e6767d3eb66085aef2a1cc98fe04936d8a42ed2ba77bb7 \
+    --hash=sha256:2460a58faeea905aeb1b9b36f5065f2dc9a9c6e4c992a6499a2360c6c74ceca3 \
+    --hash=sha256:34a9239d5b3502c17f07fd7c0b2ae6b7dd7d7f6af35fbb5072c6208e76295816 \
+    --hash=sha256:43b592511672017f5b1a483527fd2684347fdffc041c9ef53428c8dc530f79a3 \
+    --hash=sha256:43d24f6437925ce50139a310a64b2ab048cb2d3694c84c71c3f2a1626d8101dc \
+    --hash=sha256:45d32cec14e7b97af848bddd97d85ea4f0db4d5a149ed9676caa4eb2f7402bb4 \
+    --hash=sha256:470c969bb3f9a9efcedbadcd19a74ffb34a25f8e6b0e02dae7c0e71f8372f97b \
+    --hash=sha256:566e72b0cd6598503e48ea610e0052d1b8168e60a46e0bfd34b3acf2d57f96a8 \
+    --hash=sha256:5703097c4936bbb9e9bce41478c8d08edd2865e177dc4c52be759f81ee4dd26c \
+    --hash=sha256:7549fbf655e5825d787bbc9ecf6028731973f78088fbca3a1f4145c39ef09462 \
+    --hash=sha256:8207b7105829eca6f3d774f64a904190bb2231de91b8b186d21ffd98005f14a7 \
+    --hash=sha256:8c4d8e89aa7de683e2056a581ce63c46a0c41e31bd2b6d34144e2c80f5ea53dc \
+    --hash=sha256:98324ec3ecf12296e6422939e54763faedbfcc502ea4a4c38502082711867258 \
+    --hash=sha256:9bbcd9ab8ea1f2e1c8031c21445b511442cc45c89951e49bbf852cbb70755b1b \
+    --hash=sha256:9d40652cc4fe33871ad3338581dca3297ff5f2213d0df345bcfbde5162abf0c9 \
+    --hash=sha256:a2746d69a8196698146a3dbe29104f9eb6a2a4d8a27878d92169a6c0b74435b6 \
+    --hash=sha256:ae704dcfaa180ff7c4cfbad23e74321a2b774f92ca77fd94ce1049175a21c97f \
+    --hash=sha256:bfdca17c36ae01a21274a3c387a63aa1aafe72bff976522886869ef131b937f1 \
+    --hash=sha256:c482e1246726616088532b5e964e39765b6d1520791348e6c9dc3af25b233828 \
+    --hash=sha256:ca637024ca67ab24a7fd6f65d280572c3794665eaf5edcc7e90a866544076878 \
+    --hash=sha256:e02d700ec8d9b1859790c0475df4e4092c7bf3272a4fd2c9f33d87fac4427b8f \
+    --hash=sha256:e5952d2d18b79f7dc25e62e014fe5a23eb1a3d2bc66318df8988a01b1a037c5b
+    # via manageprojects
+mypy-extensions==1.0.0 \
+    --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
+    --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
+    # via
+    #   black
+    #   mypy
+packaging==23.1 \
+    --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
+    --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
+    # via black
 paho-mqtt==1.6.1 \
     --hash=sha256:2a8291c81623aec00372b5a85558a372c747cbca8e9934dfe218638b8eefc26f
     # via ha-services (pyproject.toml)
-pygments==2.15.1 \
-    --hash=sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c \
-    --hash=sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1
-    # via rich
+pathspec==0.11.2 \
+    --hash=sha256:1d6ed233af05e679efb96b1851550ea95bbb64b7c490b0f5aa52996c11e92a20 \
+    --hash=sha256:e0d8d0ac2f12da61956eb2306b69f9469b42f4deb0f3cb6ed47b9cce9996ced3
+    # via black
+platformdirs==3.10.0 \
+    --hash=sha256:b45696dab2d7cc691a3226759c0d3b00c47c8b6e293d96f6436f733303f77f6d \
+    --hash=sha256:d7c24979f292f916dc9cbf8648319032f551ea8c49a4c9bf2fb556a02070ec1d
+    # via black
+pycodestyle==2.11.0 \
+    --hash=sha256:259bcc17857d8a8b3b4a2327324b79e5f020a13c16074670f9c8c8f872ea76d0 \
+    --hash=sha256:5d1013ba8dc7895b548be5afb05740ca82454fd899971563d2ef625d090326f8
+    # via
+    #   autopep8
+    #   flake8
+pyflakes==3.1.0 \
+    --hash=sha256:4132f6d49cb4dae6819e5379898f2b8cce3c5f23994194c24b77d5da2e36f774 \
+    --hash=sha256:a0aae034c444db0071aa077972ba4768d40c830d9539fd45bf4cd3f8f6992efc
+    # via
+    #   autoflake
+    #   flake8
+    #   manageprojects
+pygments==2.16.1 \
+    --hash=sha256:13fc09fa63bc8d8671a6d247e1eb303c4b343eaee81d861f3404db2935653692 \
+    --hash=sha256:1daff0494820c69bc8941e407aa20f577374ee88364ee10a98fdbe0aece96e29
+    # via
+    #   darker
+    #   rich
 python-dateutil==2.8.2 \
     --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
     --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
     # via arrow
 python-slugify==8.0.1 \
     --hash=sha256:70ca6ea68fe63ecc8fa4fcf00ae651fc8a5d02d93dcd12ae6d4fc7ca46c4d395 \
     --hash=sha256:ce0d46ddb668b3be82f4ed5e503dbc33dd815d83e2eb6824211310d3fb172a27
     # via cookiecutter
-pyyaml==6.0 \
-    --hash=sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf \
-    --hash=sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293 \
-    --hash=sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b \
-    --hash=sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57 \
-    --hash=sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b \
-    --hash=sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4 \
-    --hash=sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07 \
-    --hash=sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba \
-    --hash=sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9 \
-    --hash=sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287 \
-    --hash=sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513 \
-    --hash=sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0 \
-    --hash=sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782 \
-    --hash=sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0 \
-    --hash=sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92 \
-    --hash=sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f \
-    --hash=sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2 \
-    --hash=sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc \
-    --hash=sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1 \
-    --hash=sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c \
-    --hash=sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86 \
-    --hash=sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4 \
-    --hash=sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c \
-    --hash=sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34 \
-    --hash=sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b \
-    --hash=sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d \
-    --hash=sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c \
-    --hash=sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb \
-    --hash=sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7 \
-    --hash=sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737 \
-    --hash=sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3 \
-    --hash=sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d \
-    --hash=sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358 \
-    --hash=sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53 \
-    --hash=sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78 \
-    --hash=sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803 \
-    --hash=sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a \
-    --hash=sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f \
-    --hash=sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174 \
-    --hash=sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5
+pyupgrade==3.10.1 \
+    --hash=sha256:1d8d138c2ccdd3c42b1419230ae036d5607dc69465a26feacc069642fc8d1b90 \
+    --hash=sha256:f565b4d26daa46ed522e98746834e77e444269103f8bc04413d77dad95169a24
+    # via manageprojects
+pyyaml==6.0.1 \
+    --hash=sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc \
+    --hash=sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741 \
+    --hash=sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206 \
+    --hash=sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27 \
+    --hash=sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595 \
+    --hash=sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62 \
+    --hash=sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98 \
+    --hash=sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696 \
+    --hash=sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d \
+    --hash=sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867 \
+    --hash=sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47 \
+    --hash=sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486 \
+    --hash=sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6 \
+    --hash=sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3 \
+    --hash=sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007 \
+    --hash=sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938 \
+    --hash=sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c \
+    --hash=sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735 \
+    --hash=sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d \
+    --hash=sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba \
+    --hash=sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8 \
+    --hash=sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5 \
+    --hash=sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd \
+    --hash=sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3 \
+    --hash=sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0 \
+    --hash=sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515 \
+    --hash=sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c \
+    --hash=sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c \
+    --hash=sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924 \
+    --hash=sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34 \
+    --hash=sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43 \
+    --hash=sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859 \
+    --hash=sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673 \
+    --hash=sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a \
+    --hash=sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab \
+    --hash=sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa \
+    --hash=sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c \
+    --hash=sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585 \
+    --hash=sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d \
+    --hash=sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f
     # via cookiecutter
-requests==2.30.0 \
-    --hash=sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294 \
-    --hash=sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4
+requests==2.31.0 \
+    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
+    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via cookiecutter
-rich==13.3.5 \
-    --hash=sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c \
-    --hash=sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704
+rich==13.5.2 \
+    --hash=sha256:146a90b3b6b47cac4a73c12866a499e9817426423f57c5a66949c086191a8808 \
+    --hash=sha256:fb9d6c0a0f643c99eed3875b5377a184132ba9be4d61516a55273d3554d75a39
     # via
+    #   cookiecutter
     #   ha-services (pyproject.toml)
     #   manageprojects
     #   rich-click
 rich-click==1.6.1 \
     --hash=sha256:0fcf4d1a09029d79322dd814ab0b2e66ac183633037561881d45abae8a161d95 \
     --hash=sha256:f8ff96693ec6e261d1544e9f7d9a5811c5ef5d74c8adb4978430fc0dac16777e
     # via
@@ -302,17 +427,38 @@
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
     # via python-dateutil
 text-unidecode==1.3 \
     --hash=sha256:1311f10e8b895935241623731c2ba64f4c455287888b18189350b67134a822e8 \
     --hash=sha256:bad6603bb14d279193107714b288be206cac565dfa49aa5b105294dd5c4aab93
     # via python-slugify
-tomlkit==0.11.8 \
-    --hash=sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171 \
-    --hash=sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3
+tokenize-rt==5.2.0 \
+    --hash=sha256:9fe80f8a5c1edad2d3ede0f37481cc0cc1538a2f442c9c2f9e4feacd2792d054 \
+    --hash=sha256:b79d41a65cfec71285433511b50271b05da3584a1da144a0752e9c621a285289
+    # via pyupgrade
+toml==0.10.2 \
+    --hash=sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b \
+    --hash=sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f
+    # via darker
+tomli==2.0.1 \
+    --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
+    --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
+    # via
+    #   autoflake
+    #   autopep8
+    #   black
+    #   flynt
+    #   mypy
+tomlkit==0.12.1 \
+    --hash=sha256:38e1ff8edb991273ec9f6181244a6a391ac30e9f5098e7535640ea6be97a7c86 \
+    --hash=sha256:712cbd236609acc6a3e2e97253dfc52d4c2082982a88f61b640ecf0817eab899
     # via
     #   ha-services (pyproject.toml)
     #   manageprojects
-urllib3==2.0.2 \
-    --hash=sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc \
-    --hash=sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e
+typing-extensions==4.7.1 \
+    --hash=sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36 \
+    --hash=sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2
+    # via mypy
+urllib3==2.0.4 \
+    --hash=sha256:8d22f86aae8ef5e410d4f539fde9ce6b2113a001bb4d189e0aed70642d602b11 \
+    --hash=sha256:de7df1803967d2c2a98e4b11bb7d6bd9210474c46e8a0401514e3a42a75ebde4
     # via requests
```

