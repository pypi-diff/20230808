# Comparing `tmp/bimbam-5.2.tar.gz` & `tmp/bimbam-5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bimbam-5.2.tar", last modified: Tue Aug  8 00:36:36 2023, max compression
+gzip compressed data, was "bimbam-5.8.tar", last modified: Tue Aug  8 18:08:27 2023, max compression
```

## Comparing `bimbam-5.2.tar` & `bimbam-5.8.tar`

### file list

```diff
@@ -1,84 +1,94 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.242019 bimbam-5.2/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-08-08 00:36:36.242019 bimbam-5.2/PKG-INFO
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.226019 bimbam-5.2/bimbam.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-08-08 00:36:36.000000 bimbam-5.2/bimbam.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2751 2023-08-08 00:36:36.000000 bimbam-5.2/bimbam.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-08-08 00:36:36.000000 bimbam-5.2/bimbam.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-08 00:36:36.000000 bimbam-5.2/bimbam.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-08 00:36:36.000000 bimbam-5.2/bimbam.egg-info/top_level.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-08-08 00:36:36.242019 bimbam-5.2/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2054 2023-08-08 00:36:29.000000 bimbam-5.2/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.230019 bimbam-5.2/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1741 2023-08-01 23:02:20.000000 bimbam-5.2/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.230019 bimbam-5.2/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17261 2023-08-03 20:16:42.000000 bimbam-5.2/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-5.2/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-31 20:39:03.000000 bimbam-5.2/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-5.2/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5653 2023-07-31 20:57:44.000000 bimbam-5.2/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.230019 bimbam-5.2/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-5.2/thonnycontrib/backend/verdicts/ExampleVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/backend/verdicts/ExceptionVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-5.2/thonnycontrib/backend/verdicts/FailedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-5.2/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/backend/verdicts/PassedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.230019 bimbam-5.2/thonnycontrib/docs/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.234019 bimbam-5.2/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/error_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-5.2/thonnycontrib/docs/res/exception_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-5.2/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/failed_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/outline_class.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/outline_method.gif
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-5.2/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2144 2023-08-01 23:56:58.000000 bimbam-5.2/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/restart_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/success_green_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.234019 bimbam-5.2/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      585 2023-07-29 21:42:29.000000 bimbam-5.2/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    15559 2023-08-07 21:56:45.000000 bimbam-5.2/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6751 2023-08-03 22:03:53.000000 bimbam-5.2/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-5.2/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3665 2023-08-07 21:57:09.000000 bimbam-5.2/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.234019 bimbam-5.2/thonnycontrib/i18n/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:28:42.000000 bimbam-5.2/thonnycontrib/i18n/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      702 2023-08-07 23:25:41.000000 bimbam-5.2/thonnycontrib/i18n/languages.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.234019 bimbam-5.2/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3406 2023-08-07 22:33:46.000000 bimbam-5.2/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.238019 bimbam-5.2/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-5.2/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-5.2/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-5.2/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2744 2023-08-06 23:32:11.000000 bimbam-5.2/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    24297 2023-08-07 21:44:20.000000 bimbam-5.2/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41795 2023-08-08 00:07:19.000000 bimbam-5.2/thonnycontrib/l1test_frontend/l1test_treeview.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.238019 bimbam-5.2/thonnycontrib/main_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-5.2/thonnycontrib/main_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5352 2023-08-07 21:48:38.000000 bimbam-5.2/thonnycontrib/main_generator/main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5723 2023-08-07 23:33:25.000000 bimbam-5.2/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3129 2023-08-07 21:29:17.000000 bimbam-5.2/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.238019 bimbam-5.2/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/tests/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.242019 bimbam-5.2/thonnycontrib/tests/fixtures/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-5.2/thonnycontrib/tests/fixtures/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/tests/fixtures/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-5.2/thonnycontrib/tests/fixtures/workbench_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-03 20:14:25.000000 bimbam-5.2/thonnycontrib/tests/tests_ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2505 2023-07-30 12:46:52.000000 bimbam-5.2/thonnycontrib/tests/tests_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-5.2/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-5.2/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-5.2/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-5.2/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-5.2/thonnycontrib/tests/tests_main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-5.2/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-5.2/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17903 2023-08-07 21:19:21.000000 bimbam-5.2/thonnycontrib/utils.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.743626 bimbam-5.8/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-08-08 18:08:27.743626 bimbam-5.8/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.727625 bimbam-5.8/bimbam.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-08-08 18:08:27.000000 bimbam-5.8/bimbam.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3002 2023-08-08 18:08:27.000000 bimbam-5.8/bimbam.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-08-08 18:08:27.000000 bimbam-5.8/bimbam.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-08 18:08:27.000000 bimbam-5.8/bimbam.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-08 18:08:27.000000 bimbam-5.8/bimbam.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-08-08 18:08:27.743626 bimbam-5.8/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1945 2023-08-08 18:08:24.000000 bimbam-5.8/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.727625 bimbam-5.8/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1741 2023-08-01 23:02:20.000000 bimbam-5.8/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.731626 bimbam-5.8/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17261 2023-08-03 20:16:42.000000 bimbam-5.8/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-5.8/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-31 20:39:03.000000 bimbam-5.8/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-5.8/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5653 2023-07-31 20:57:44.000000 bimbam-5.8/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.731626 bimbam-5.8/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-5.8/thonnycontrib/backend/verdicts/ExampleVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/backend/verdicts/ExceptionVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-5.8/thonnycontrib/backend/verdicts/FailedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-5.8/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/backend/verdicts/PassedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.731626 bimbam-5.8/thonnycontrib/docs/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2338 2023-08-08 00:05:02.000000 bimbam-5.8/thonnycontrib/docs/Readme.md
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.731626 bimbam-5.8/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/docs/res/error_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-5.8/thonnycontrib/docs/res/exception_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-5.8/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/docs/res/failed_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/docs/res/outline_class.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/docs/res/outline_method.gif
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-5.8/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2144 2023-08-01 23:56:58.000000 bimbam-5.8/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/docs/res/restart_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/docs/res/success_green_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.735626 bimbam-5.8/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      585 2023-07-29 21:42:29.000000 bimbam-5.8/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    15559 2023-08-07 21:56:45.000000 bimbam-5.8/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6751 2023-08-03 22:03:53.000000 bimbam-5.8/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-5.8/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3665 2023-08-07 21:57:09.000000 bimbam-5.8/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.735626 bimbam-5.8/thonnycontrib/i18n/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:28:42.000000 bimbam-5.8/thonnycontrib/i18n/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      702 2023-08-07 23:25:41.000000 bimbam-5.8/thonnycontrib/i18n/languages.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.735626 bimbam-5.8/thonnycontrib/i18n/locale/
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.723626 bimbam-5.8/thonnycontrib/i18n/locale/en_US/
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.735626 bimbam-5.8/thonnycontrib/i18n/locale/en_US/LC_MESSAGES/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      214 2023-08-08 00:11:21.000000 bimbam-5.8/thonnycontrib/i18n/locale/en_US/LC_MESSAGES/l1test.mo
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4522 2023-08-07 23:42:28.000000 bimbam-5.8/thonnycontrib/i18n/locale/en_US/LC_MESSAGES/l1test.po
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.723626 bimbam-5.8/thonnycontrib/i18n/locale/fr_FR/
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.735626 bimbam-5.8/thonnycontrib/i18n/locale/fr_FR/LC_MESSAGES/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4204 2023-08-08 00:22:18.000000 bimbam-5.8/thonnycontrib/i18n/locale/fr_FR/LC_MESSAGES/l1test.mo
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6187 2023-08-07 23:43:38.000000 bimbam-5.8/thonnycontrib/i18n/locale/fr_FR/LC_MESSAGES/l1test.po
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5087 2023-08-07 23:33:51.000000 bimbam-5.8/thonnycontrib/i18n/locale/l1test.pot
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.735626 bimbam-5.8/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3406 2023-08-07 22:33:46.000000 bimbam-5.8/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.735626 bimbam-5.8/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-5.8/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-5.8/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-5.8/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2744 2023-08-06 23:32:11.000000 bimbam-5.8/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    25479 2023-08-08 01:11:13.000000 bimbam-5.8/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41795 2023-08-08 00:07:19.000000 bimbam-5.8/thonnycontrib/l1test_frontend/l1test_treeview.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.735626 bimbam-5.8/thonnycontrib/main_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-5.8/thonnycontrib/main_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5352 2023-08-07 21:48:38.000000 bimbam-5.8/thonnycontrib/main_generator/main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5723 2023-08-07 23:33:25.000000 bimbam-5.8/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3142 2023-08-08 00:45:58.000000 bimbam-5.8/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.739626 bimbam-5.8/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/tests/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 18:08:27.743626 bimbam-5.8/thonnycontrib/tests/fixtures/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-5.8/thonnycontrib/tests/fixtures/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-5.8/thonnycontrib/tests/fixtures/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-5.8/thonnycontrib/tests/fixtures/workbench_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-03 20:14:25.000000 bimbam-5.8/thonnycontrib/tests/tests_ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2329 2023-08-08 17:34:23.000000 bimbam-5.8/thonnycontrib/tests/tests_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-5.8/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-5.8/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-5.8/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-5.8/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-5.8/thonnycontrib/tests/tests_main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-5.8/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-5.8/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17903 2023-08-07 21:19:21.000000 bimbam-5.8/thonnycontrib/utils.py
```

### Comparing `bimbam-5.2/PKG-INFO` & `bimbam-5.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 5.2
+Version: 5.8
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-5.2/bimbam.egg-info/PKG-INFO` & `bimbam-5.8/bimbam.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 5.2
+Version: 5.8
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-5.2/bimbam.egg-info/SOURCES.txt` & `bimbam-5.8/bimbam.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 thonnycontrib/backend/verdicts/ExampleVerdict.py
 thonnycontrib/backend/verdicts/ExceptionVerdict.py
 thonnycontrib/backend/verdicts/FailedVerdict.py
 thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
 thonnycontrib/backend/verdicts/PassedSetupVerdict.py
 thonnycontrib/backend/verdicts/PassedVerdict.py
 thonnycontrib/backend/verdicts/__init__.py
-thonnycontrib/docs/__init__.py
+thonnycontrib/docs/Readme.md
 thonnycontrib/docs/res/error_icon.png
 thonnycontrib/docs/res/exception_red_chip.png
 thonnycontrib/docs/res/failed.png
 thonnycontrib/docs/res/failed_red_chip.png
 thonnycontrib/docs/res/l1test_icon.png
 thonnycontrib/docs/res/l1test_icon_old.png
 thonnycontrib/docs/res/outline_class.png
@@ -39,14 +39,19 @@
 thonnycontrib/docs/res/success_green_chip.png
 thonnycontrib/docs/res/warning.png
 thonnycontrib/docstring_generator/__init__.py
 thonnycontrib/docstring_generator/doc_generator.py
 thonnycontrib/docstring_generator/doc_template.py
 thonnycontrib/i18n/__init__.py
 thonnycontrib/i18n/languages.py
+thonnycontrib/i18n/locale/l1test.pot
+thonnycontrib/i18n/locale/en_US/LC_MESSAGES/l1test.mo
+thonnycontrib/i18n/locale/en_US/LC_MESSAGES/l1test.po
+thonnycontrib/i18n/locale/fr_FR/LC_MESSAGES/l1test.mo
+thonnycontrib/i18n/locale/fr_FR/LC_MESSAGES/l1test.po
 thonnycontrib/l1test_configuration/__init__.py
 thonnycontrib/l1test_configuration/l1test_options.py
 thonnycontrib/l1test_frontend/__init__.py
 thonnycontrib/l1test_frontend/l1test_error_view.py
 thonnycontrib/l1test_frontend/l1test_outliner_menu.py
 thonnycontrib/l1test_frontend/l1test_reporter.py
 thonnycontrib/l1test_frontend/l1test_runner.py
```

### Comparing `bimbam-5.2/setup.py` & `bimbam-5.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 # Auteur : Esteban COLLARD, Nordine EL AMMARI
 # Modifications : Reda ID TALEB & Manal LAGHMICH
 
-from setuptools import setup
+from setuptools import find_packages, setup
 import os.path
 
-import thonnycontrib
 
-thonnycontrib_path = os.path.dirname(os.path.abspath(thonnycontrib.__file__))
-def get_packages_under_thonnycontrib(directory:str, namespace:str):
-    packages = []
-    for root, dirs, files in os.walk(directory):
-        if "__init__.py" in files:
-            splitted: list[str] = root.split(os.sep)            
-            try:
-                index = splitted.index(namespace)
-                sub_module = ".".join(splitted[index:])
-                packages.append(sub_module)
-            except:pass
-    return packages
+def recursive_files(directory):
+    paths = []
+    for (path, _, filenames) in os.walk(directory):
+        for filename in filenames:
+            if not filename.endswith(".pyc"):
+                paths.append(os.path.join('..', path, filename))
+    return paths
 
-packages = get_packages_under_thonnycontrib(thonnycontrib_path, "thonnycontrib")
+packages = find_packages()
 
 def get_packages_data(packages: list[str]=packages):
     py_packs = dict([(p, ["*.py"]) for p in packages if not p.endswith("docs")])
-    other_packs = dict([(p, ["res/*"]) for p in packages if p.endswith("docs")])
-    i18n_packs = dict([(p, ["i18n/*"]) for p in packages if "i18n" in p])
-    
-    return {**py_packs, **other_packs, **i18n_packs}
+    i18n_packs = dict([(p, ["*.py"]) for p in packages if p.endswith("i18n")])
+    unpackaged = {"": recursive_files("thonnycontrib/i18n/locale") + recursive_files("thonnycontrib/docs")}
+    return {**py_packs, **i18n_packs, **unpackaged} 
 
 setupdir = os.path.dirname(__file__)
 
 
+requirements = []
+for line in open(os.path.join(setupdir, "requirements.txt"), encoding="ASCII"):
+    if line.strip() and not line.startswith("#"):
+        requirements.append(line)
+        
 setup(
     name="bimbam",
-    version="5.2",
+    version="5.8",
     author="idtaleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests""",
     url="https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests",
 #    keywords="IDE education programming tests in documentation",
@@ -48,11 +46,11 @@
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education"
         ],
     platforms=["Windows", "macOS", "Linux"],
     python_requires=">=3.9",
     package_data=get_packages_data(),
-    install_requires=["thonny>=4.0.0"],
+    install_requires=requirements,
     packages=packages,
 )
```

### Comparing `bimbam-5.2/thonnycontrib/ThonnyLogsGenerator.py` & `bimbam-5.8/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/backend/ast_parser.py` & `bimbam-5.8/thonnycontrib/backend/ast_parser.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/backend/doctest_parser.py` & `bimbam-5.8/thonnycontrib/backend/doctest_parser.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/backend/evaluator.py` & `bimbam-5.8/thonnycontrib/backend/evaluator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/backend/l1test_backend.py` & `bimbam-5.8/thonnycontrib/backend/l1test_backend.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/backend/test_finder.py` & `bimbam-5.8/thonnycontrib/backend/test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/backend/verdicts/ExampleVerdict.py` & `bimbam-5.8/thonnycontrib/backend/verdicts/ExampleVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/backend/verdicts/FailedVerdict.py` & `bimbam-5.8/thonnycontrib/backend/verdicts/FailedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py` & `bimbam-5.8/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/docs/res/error_icon.png` & `bimbam-5.8/thonnycontrib/docs/res/error_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/docs/res/exception_red_chip.png` & `bimbam-5.8/thonnycontrib/docs/res/exception_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/docs/res/failed.png` & `bimbam-5.8/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/docs/res/failed_red_chip.png` & `bimbam-5.8/thonnycontrib/docs/res/failed_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/docs/res/l1test_icon.png` & `bimbam-5.8/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/docs/res/l1test_icon_old.png` & `bimbam-5.8/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/docs/res/outline_class.png` & `bimbam-5.8/thonnycontrib/docs/res/outline_class.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/docs/res/outline_method.gif` & `bimbam-5.8/thonnycontrib/docs/res/outline_method.gif`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/docs/res/passed.png` & `bimbam-5.8/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/docs/res/pending_icon.png` & `bimbam-5.8/thonnycontrib/docs/res/pending_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/docs/res/restart_icon.png` & `bimbam-5.8/thonnycontrib/docs/res/restart_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/docs/res/success_green_chip.png` & `bimbam-5.8/thonnycontrib/docs/res/success_green_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/docs/res/warning.png` & `bimbam-5.8/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/docstring_generator/__init__.py` & `bimbam-5.8/thonnycontrib/docstring_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/docstring_generator/doc_generator.py` & `bimbam-5.8/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/docstring_generator/doc_template.py` & `bimbam-5.8/thonnycontrib/docstring_generator/doc_template.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/environement_vars.py` & `bimbam-5.8/thonnycontrib/environement_vars.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/exceptions.py` & `bimbam-5.8/thonnycontrib/exceptions.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/i18n/languages.py` & `bimbam-5.8/thonnycontrib/i18n/languages.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/l1test_configuration/l1test_options.py` & `bimbam-5.8/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/l1test_frontend/__init__.py` & `bimbam-5.8/thonnycontrib/l1test_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/l1test_frontend/l1test_error_view.py` & `bimbam-5.8/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/l1test_frontend/l1test_outliner_menu.py` & `bimbam-5.8/thonnycontrib/l1test_frontend/l1test_outliner_menu.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/l1test_frontend/l1test_reporter.py` & `bimbam-5.8/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/l1test_frontend/l1test_runner.py` & `bimbam-5.8/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,24 +24,38 @@
 ErrorMsg = namedtuple("ErrorMsg", "title msg")
 
 # Le nom de l'event qui lance le redémarrage du backend thonny
 BACKEND_RESTART_EVENT = "BackendRestart"
 
 class L1TestRunner:
     """
-        The L1TestRunner is responsible for receiving the test results returned 
-        by the l1test_backend and displaying them on the treeview. The L1TestRunner 
-        is also responsible for displaying errors if the l1test_backend returns 
-        a response that carries an exception.
-        
-        Finally, the L1TestRunner decides which view (the Treeview or the ErrorView)
-        to display depending on the state of program execution.
+        The `L1TestRunner` is responsible for starting the execution of the plugin. It's like 
+        a controller that handles sending requests and receiving responses.
+
+        Firstly, it sends a request to the backend to evaluate the current source code. Then,
+        it handles the response receieved from the backend and parses it. The backend
+        send a response of type `TopLevelResponse` that contains results computed by the `Evaluator`.
+        The results can be the verdicts if it succeed or an exception if failed. 
+        In the both of case, `L1TestRunner` decides and invokes the `L1TestReporter` to show 
+        either the verdicts or the error message.
         
-        Note: L1TestRunner does not deal with the construction of the views but 
-        it allows to invoke the correct one.
+        The L1TestRunner handles also the state of the current execution of the plugin. It has 
+        three states : 
+        - _is_l1test_running : set to true when the button l1test is just invoked.
+        - _is_pending : set to true when the plugin is still runinng but not yet finished. 
+                        This state is sent from the backend to tell the `L1TestRunner` that the `Evaluator`
+                        didn't finished the evaluations yet. This is useful when the Evaluator encouter
+                        an infinite loop, in this case the L1TestRunner knows that the Evaluator is still 
+                        working (or blocked) but at the same time the L1testRunner shows the current state
+                        in the view. This is handy for junior devs to tell them why the plugin is still
+                        turning.
+        - _has_exception: when the backend sends an error message instead of the verdicts.
+
+        Note: `L1TestRunner` does not deal with the construction of the views but 
+        it allows to invoke the correct one. 
     """
     def __init__(self, reporter=None):
         l1test_frontend._l1test_runner = self
         
         self._reporter = L1TestReporter() if not reporter else reporter
         self._has_exception = False
         self._is_l1test_running = False
```

### Comparing `bimbam-5.2/thonnycontrib/l1test_frontend/l1test_treeview.py` & `bimbam-5.8/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/main_generator/main_generator.py` & `bimbam-5.8/thonnycontrib/main_generator/main_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/plugin_loader.py` & `bimbam-5.8/thonnycontrib/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/properties.py` & `bimbam-5.8/thonnycontrib/properties.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .i18n.languages import tr
+from thonnycontrib.i18n.languages import tr
 
 PLUGIN_NAME = "L1Test"
 ERROR_VIEW_LABEL = '%s errors' % PLUGIN_NAME
 
 # ici vous pouvez changer la syntaxe du doctest. 
 # version 2022 PJI : Actuellement on garde la syntaxe `$py`.
 L1TEST_SYMBOL = "[$]py"
```

### Comparing `bimbam-5.2/thonnycontrib/tests/fixtures/workbench_mock.py` & `bimbam-5.8/thonnycontrib/tests/fixtures/workbench_mock.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/tests/tests_doc_generator.py` & `bimbam-5.8/thonnycontrib/tests/tests_doc_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,16 +63,14 @@
         
         raised_exception = e.exception      
         self.assertTrue(SyntaxError.__name__ in str(raised_exception))
         
     def test_doc_generator_when_signature_doesnt_finish_with_colon(self):
         signature = "def func()"
         
-        with self.assertRaises(DocGeneratorParserException) as e:
+        with self.assertRaises(
+                               
+                               ) as e:
             self.docGenerationStrategy._generate(signature)
         
-        raised_exception = e.exception      
-        self.assertTrue(SyntaxError.__name__ in str(raised_exception))
-        self.assertTrue(SyntaxError.__name__+": expected ':'" in str(raised_exception))
-        
 if __name__ == '__main__':
     ut.main(verbosity=2)
```

### Comparing `bimbam-5.2/thonnycontrib/tests/tests_example_no_expected.py` & `bimbam-5.8/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/tests/tests_example_with_exception.py` & `bimbam-5.8/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/tests/tests_example_with_expected.py` & `bimbam-5.8/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/tests/tests_l1TestRunner.py` & `bimbam-5.8/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/tests/tests_main_generator.py` & `bimbam-5.8/thonnycontrib/tests/tests_main_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/tests/tests_test_finder.py` & `bimbam-5.8/thonnycontrib/tests/tests_test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/tests/tests_view.py` & `bimbam-5.8/thonnycontrib/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.2/thonnycontrib/utils.py` & `bimbam-5.8/thonnycontrib/utils.py`

 * *Files identical despite different names*

