# Comparing `tmp/bimbam-5.1.tar.gz` & `tmp/bimbam-5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bimbam-5.1.tar", last modified: Tue Aug  8 00:33:37 2023, max compression
+gzip compressed data, was "bimbam-5.2.tar", last modified: Tue Aug  8 00:36:36 2023, max compression
```

## Comparing `bimbam-5.1.tar` & `bimbam-5.2.tar`

### file list

```diff
@@ -1,80 +1,84 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.952432 bimbam-5.1/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-08-08 00:33:37.952432 bimbam-5.1/PKG-INFO
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.940431 bimbam-5.1/bimbam.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-08-08 00:33:37.000000 bimbam-5.1/bimbam.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2648 2023-08-08 00:33:37.000000 bimbam-5.1/bimbam.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-08-08 00:33:37.000000 bimbam-5.1/bimbam.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-08 00:33:37.000000 bimbam-5.1/bimbam.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-08 00:33:37.000000 bimbam-5.1/bimbam.egg-info/top_level.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-08-08 00:33:37.952432 bimbam-5.1/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2054 2023-08-08 00:33:21.000000 bimbam-5.1/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.940431 bimbam-5.1/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1741 2023-08-01 23:02:20.000000 bimbam-5.1/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.944431 bimbam-5.1/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17236 2023-08-01 23:42:41.000000 bimbam-5.1/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-5.1/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-31 20:39:03.000000 bimbam-5.1/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-5.1/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5653 2023-07-31 20:57:44.000000 bimbam-5.1/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.944431 bimbam-5.1/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-5.1/thonnycontrib/backend/verdicts/ExampleVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/backend/verdicts/ExceptionVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-5.1/thonnycontrib/backend/verdicts/FailedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-5.1/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/backend/verdicts/PassedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.944431 bimbam-5.1/thonnycontrib/docs/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.948431 bimbam-5.1/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/error_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-5.1/thonnycontrib/docs/res/exception_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-5.1/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/failed_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/outline_class.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/outline_method.gif
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-5.1/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2144 2023-08-01 23:56:58.000000 bimbam-5.1/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/restart_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/success_green_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.948431 bimbam-5.1/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      585 2023-07-29 21:42:29.000000 bimbam-5.1/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16176 2023-08-01 23:32:20.000000 bimbam-5.1/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7054 2023-07-22 09:12:15.000000 bimbam-5.1/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-5.1/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3521 2023-08-02 21:47:51.000000 bimbam-5.1/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.948431 bimbam-5.1/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2991 2023-07-23 10:41:36.000000 bimbam-5.1/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.948431 bimbam-5.1/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-5.1/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-5.1/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-5.1/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2749 2023-07-23 16:34:32.000000 bimbam-5.1/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    23597 2023-08-02 21:48:21.000000 bimbam-5.1/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41636 2023-08-01 23:49:06.000000 bimbam-5.1/thonnycontrib/l1test_frontend/l1test_treeview.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.952432 bimbam-5.1/thonnycontrib/main_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-5.1/thonnycontrib/main_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5301 2023-07-28 14:35:18.000000 bimbam-5.1/thonnycontrib/main_generator/main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5453 2023-07-30 12:38:45.000000 bimbam-5.1/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2962 2023-07-27 19:06:48.000000 bimbam-5.1/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.952432 bimbam-5.1/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/tests/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.952432 bimbam-5.1/thonnycontrib/tests/fixtures/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-5.1/thonnycontrib/tests/fixtures/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/tests/fixtures/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-5.1/thonnycontrib/tests/fixtures/workbench_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2505 2023-07-30 12:46:52.000000 bimbam-5.1/thonnycontrib/tests/tests_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-5.1/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-5.1/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-5.1/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-5.1/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-5.1/thonnycontrib/tests/tests_main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-5.1/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-5.1/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17858 2023-08-01 23:47:43.000000 bimbam-5.1/thonnycontrib/utils.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.242019 bimbam-5.2/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-08-08 00:36:36.242019 bimbam-5.2/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.226019 bimbam-5.2/bimbam.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-08-08 00:36:36.000000 bimbam-5.2/bimbam.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2751 2023-08-08 00:36:36.000000 bimbam-5.2/bimbam.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-08-08 00:36:36.000000 bimbam-5.2/bimbam.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-08 00:36:36.000000 bimbam-5.2/bimbam.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-08 00:36:36.000000 bimbam-5.2/bimbam.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-08-08 00:36:36.242019 bimbam-5.2/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2054 2023-08-08 00:36:29.000000 bimbam-5.2/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.230019 bimbam-5.2/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1741 2023-08-01 23:02:20.000000 bimbam-5.2/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.230019 bimbam-5.2/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17261 2023-08-03 20:16:42.000000 bimbam-5.2/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-5.2/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-31 20:39:03.000000 bimbam-5.2/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-5.2/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5653 2023-07-31 20:57:44.000000 bimbam-5.2/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.230019 bimbam-5.2/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-5.2/thonnycontrib/backend/verdicts/ExampleVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/backend/verdicts/ExceptionVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-5.2/thonnycontrib/backend/verdicts/FailedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-5.2/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/backend/verdicts/PassedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.230019 bimbam-5.2/thonnycontrib/docs/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.234019 bimbam-5.2/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/error_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-5.2/thonnycontrib/docs/res/exception_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-5.2/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/failed_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/outline_class.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/outline_method.gif
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-5.2/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2144 2023-08-01 23:56:58.000000 bimbam-5.2/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/restart_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/success_green_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.234019 bimbam-5.2/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      585 2023-07-29 21:42:29.000000 bimbam-5.2/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    15559 2023-08-07 21:56:45.000000 bimbam-5.2/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6751 2023-08-03 22:03:53.000000 bimbam-5.2/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-5.2/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3665 2023-08-07 21:57:09.000000 bimbam-5.2/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.234019 bimbam-5.2/thonnycontrib/i18n/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:28:42.000000 bimbam-5.2/thonnycontrib/i18n/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      702 2023-08-07 23:25:41.000000 bimbam-5.2/thonnycontrib/i18n/languages.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.234019 bimbam-5.2/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3406 2023-08-07 22:33:46.000000 bimbam-5.2/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.238019 bimbam-5.2/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-5.2/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-5.2/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-5.2/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2744 2023-08-06 23:32:11.000000 bimbam-5.2/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    24297 2023-08-07 21:44:20.000000 bimbam-5.2/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41795 2023-08-08 00:07:19.000000 bimbam-5.2/thonnycontrib/l1test_frontend/l1test_treeview.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.238019 bimbam-5.2/thonnycontrib/main_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-5.2/thonnycontrib/main_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5352 2023-08-07 21:48:38.000000 bimbam-5.2/thonnycontrib/main_generator/main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5723 2023-08-07 23:33:25.000000 bimbam-5.2/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3129 2023-08-07 21:29:17.000000 bimbam-5.2/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.238019 bimbam-5.2/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/tests/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:36:36.242019 bimbam-5.2/thonnycontrib/tests/fixtures/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-5.2/thonnycontrib/tests/fixtures/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-5.2/thonnycontrib/tests/fixtures/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-5.2/thonnycontrib/tests/fixtures/workbench_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-03 20:14:25.000000 bimbam-5.2/thonnycontrib/tests/tests_ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2505 2023-07-30 12:46:52.000000 bimbam-5.2/thonnycontrib/tests/tests_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-5.2/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-5.2/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-5.2/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-5.2/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-5.2/thonnycontrib/tests/tests_main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-5.2/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-5.2/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17903 2023-08-07 21:19:21.000000 bimbam-5.2/thonnycontrib/utils.py
```

### Comparing `bimbam-5.1/PKG-INFO` & `bimbam-5.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 5.1
+Version: 5.2
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-5.1/bimbam.egg-info/PKG-INFO` & `bimbam-5.2/bimbam.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 5.1
+Version: 5.2
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-5.1/bimbam.egg-info/SOURCES.txt` & `bimbam-5.2/bimbam.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,25 +37,28 @@
 thonnycontrib/docs/res/pending_icon.png
 thonnycontrib/docs/res/restart_icon.png
 thonnycontrib/docs/res/success_green_chip.png
 thonnycontrib/docs/res/warning.png
 thonnycontrib/docstring_generator/__init__.py
 thonnycontrib/docstring_generator/doc_generator.py
 thonnycontrib/docstring_generator/doc_template.py
+thonnycontrib/i18n/__init__.py
+thonnycontrib/i18n/languages.py
 thonnycontrib/l1test_configuration/__init__.py
 thonnycontrib/l1test_configuration/l1test_options.py
 thonnycontrib/l1test_frontend/__init__.py
 thonnycontrib/l1test_frontend/l1test_error_view.py
 thonnycontrib/l1test_frontend/l1test_outliner_menu.py
 thonnycontrib/l1test_frontend/l1test_reporter.py
 thonnycontrib/l1test_frontend/l1test_runner.py
 thonnycontrib/l1test_frontend/l1test_treeview.py
 thonnycontrib/main_generator/__init__.py
 thonnycontrib/main_generator/main_generator.py
 thonnycontrib/tests/__init__.py
+thonnycontrib/tests/tests_ast_parser.py
 thonnycontrib/tests/tests_doc_generator.py
 thonnycontrib/tests/tests_example_no_expected.py
 thonnycontrib/tests/tests_example_with_exception.py
 thonnycontrib/tests/tests_example_with_expected.py
 thonnycontrib/tests/tests_l1TestRunner.py
 thonnycontrib/tests/tests_main_generator.py
 thonnycontrib/tests/tests_test_finder.py
```

### Comparing `bimbam-5.1/setup.py` & `bimbam-5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     return {**py_packs, **other_packs, **i18n_packs}
 
 setupdir = os.path.dirname(__file__)
 
 
 setup(
     name="bimbam",
-    version="5.1",
+    version="5.2",
     author="idtaleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests""",
     url="https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests",
 #    keywords="IDE education programming tests in documentation",
```

### Comparing `bimbam-5.1/thonnycontrib/ThonnyLogsGenerator.py` & `bimbam-5.2/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/backend/ast_parser.py` & `bimbam-5.2/thonnycontrib/backend/ast_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,16 +338,15 @@
     
     The `L1DocTestParser`doesn't evaluate the created L1Doctests. Each yielded L1DocTest
     is initially unevaluated. It's the responsibility of the `Evaluator` to evaluate each 
     received L1DocTest.
     
     Example of use:
     >>> parser = L1DocTestParser("source", "filename.py")
-    >>> generator:  = parser.parse()
-    >>> 
+    >>> generator = parser.parse() # returns a generator of L1DocTests
     """
     def __init__(self, source:str="", filename:str="", mode="exec") -> None:
         self._filename = filename
         self._source = source
         self._mode = mode
 
     def parse(self, lineno:int=None):
```

### Comparing `bimbam-5.1/thonnycontrib/backend/doctest_parser.py` & `bimbam-5.2/thonnycontrib/backend/doctest_parser.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/backend/evaluator.py` & `bimbam-5.2/thonnycontrib/backend/evaluator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/backend/l1test_backend.py` & `bimbam-5.2/thonnycontrib/backend/l1test_backend.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/backend/test_finder.py` & `bimbam-5.2/thonnycontrib/backend/test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/backend/verdicts/ExampleVerdict.py` & `bimbam-5.2/thonnycontrib/backend/verdicts/ExampleVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/backend/verdicts/FailedVerdict.py` & `bimbam-5.2/thonnycontrib/backend/verdicts/FailedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py` & `bimbam-5.2/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/docs/res/error_icon.png` & `bimbam-5.2/thonnycontrib/docs/res/error_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/docs/res/exception_red_chip.png` & `bimbam-5.2/thonnycontrib/docs/res/exception_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/docs/res/failed.png` & `bimbam-5.2/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/docs/res/failed_red_chip.png` & `bimbam-5.2/thonnycontrib/docs/res/failed_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/docs/res/l1test_icon.png` & `bimbam-5.2/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/docs/res/l1test_icon_old.png` & `bimbam-5.2/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/docs/res/outline_class.png` & `bimbam-5.2/thonnycontrib/docs/res/outline_class.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/docs/res/outline_method.gif` & `bimbam-5.2/thonnycontrib/docs/res/outline_method.gif`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/docs/res/passed.png` & `bimbam-5.2/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/docs/res/pending_icon.png` & `bimbam-5.2/thonnycontrib/docs/res/pending_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/docs/res/restart_icon.png` & `bimbam-5.2/thonnycontrib/docs/res/restart_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/docs/res/success_green_chip.png` & `bimbam-5.2/thonnycontrib/docs/res/success_green_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/docs/res/warning.png` & `bimbam-5.2/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/docstring_generator/__init__.py` & `bimbam-5.2/thonnycontrib/docstring_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/docstring_generator/doc_generator.py` & `bimbam-5.2/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-import re
-import sys
-import textwrap
-from typing import List
-
-from .doc_template import DocTemplate
-from ..backend.ast_parser import L1TestAstParser
 from .doc_template import *
 from ..properties import CANNOT_GENERATE_THE_DOCSTRING
-from thonny.tktextext import *  
+from ..l1test_frontend import get_l1test_runner
 from ..exceptions import DocGeneratorParserException, FrontendException, NoFunctionSelectedToDocumentException
 from ..utils import replace_error_line, get_last_exception
-from thonny.editors import EditorCodeViewText
 from ..ThonnyLogsGenerator import log_doc_in_thonny
+import thonnycontrib.docstring_generator as docstring_generator
+
+from typing import List
+from thonny.tktextext import *  
+from thonny.editors import EditorCodeViewText
 from thonny import get_workbench
-from .. l1test_frontend import get_l1test_runner
-from thonnycontrib import docstring_generator
+import re, sys, textwrap
+
 
 r""" Docstring Generator Module
 Description:
 ------------
 This module generates a docstring using the templates.
 
 For a selected line the `DocGenerator` tries to verify if the selected line
@@ -30,19 +27,19 @@
 
 About templates, the docstring generator invokes the `DefaultDocTemplate` by default. 
 The `DocTemplate.DefaultDocTemplate` class contains an implementation 
 of a default template. 
 
 How to use the Generator in thonny IDE:
 ---------------------------------------
-- Right click on a function or a class declaration(it's prototype) and choose 
-in the `edit menu` ~Generate Docstring~ button. You can also select the short cut 
-Alt+d after putting the cursor on the function(or a class) declaration.
+- Right click on a function or a class and choose in the `edit menu` ~Generate Docstring~ 
+button. You can also click on the body of the function to generate the docstring.
 
-- Just a return on a function declaration will generate its docstring.
+- Just a return on a function declaration will generate its docstring. The declaration
+should be finished by a ":" caractere.
 """
 
 class DocParser:
     def __init__(self, filename="", source=""):
         self._filename = filename
         self._source = source
     
@@ -84,15 +81,15 @@
     def get_source(self):
         return self._source 
     
     def set_ast_parser(self, parser) :
         self._ast_parser = parser
 
 class DocGenerationStrategy(ABC):
-    _SIGNATURE_REGEX = r"\s*(?P<id>def|class)\s*.*\s*$"
+    _SIGNATURE_REGEX = r"\s*(?P<id>def|class)\s*.*\s*:\s*$"
     
     def __init__(self, text_widget:EditorCodeViewText, parser:DocParser=DocParser()):
         self._parser = parser 
         self._text_widget = text_widget
     
     @abstractmethod
     def can_generate(self, selected_lineno:int) -> bool:
@@ -127,19 +124,17 @@
         """
         if signature is None: signature = ""
         
         # We should check that the line is a function declaration and that ends with ':' character. 
         declaration_match = re.match(self._SIGNATURE_REGEX, signature)
 
         if not declaration_match:
-            raise NoFunctionSelectedToDocumentException("No signature is selected to document!\n")
-        else:   
-            id_signature = declaration_match.group("id") # c'est le tag <id> dans l'expression régulière
-            
-            template:DocTemplate = DocTemplateFactory.create_template(id_signature) 
+            raise NoFunctionSelectedToDocumentException()
+        else:               
+            template:DocTemplate = DocTemplateFactory.create_template(declaration_match.group("id")) 
             
             generated_temp = self.__get_generated_template(template, signature, selected_lineno)
             
             indent = self.__compute_indent(signature)
             generated_doc = textwrap.indent(generated_temp, indent)
             if self._text_widget:
                 # c'est içi que la docstring est ajoutée à l'éditeur
@@ -185,25 +180,22 @@
 
         Args:
             signature (str): a signature of a function
 
         Returns:
             int: returns the indentation based on the whitespaces located in the given `signature`.
         """
+        print(signature)
         space_match = re.search("^(\s+)", signature)
         python_indent = 4
         sig_indent = len(space_match.group(1)) if space_match else 0
         return " " * (sig_indent + python_indent)
     
     def _create_custom_body(self, signature:str):
         signature = signature.strip()
-        # on supprime tous ce qu'il vient après les ":" dans la signature. Car, on veut juste la signature.
-        # En python on peut avoir une syntaxe comme : def foo(): pass, cela pose problème pour l'ast parser
-        # il faut donc qu'on ait juste la signature sans le corps de la fonction.
-        signature = re.sub(r"\s*(?P<id>def|class)(?P<signature>\s*.*\s*:)(?P<body>\s*.*)$", r"\g<id>\g<signature>", signature)
         indent = " " * 4
         return signature + "\n" + indent + "pass"
     
     def set_parser(self, parser: DocParser):
         self._parser = parser
         
     def get_parser(self):
@@ -218,17 +210,17 @@
 class AutoGenerationStrategy(DocGenerationStrategy):
     def __init__(self, text_widget:EditorCodeViewText=None, parser=DocParser()):
         super().__init__(text_widget, parser)
         self.__selected_sig = None
         self.__selected_lineno = None
     
     def can_generate(self, selected_lineno:int) -> bool:
-        selected_sig = self._text_widget.get(str(selected_lineno)+".0", str(selected_lineno+1)+".0").strip().strip("\n")
-        if selected_sig != "":
-            self.__selected_sig = selected_sig
+        line_content = self._text_widget.get(str(selected_lineno)+".0", str(selected_lineno+1)+".0")
+        if line_content.strip().strip("\n") != "":
+            self.__selected_sig = line_content
             self.__selected_lineno = selected_lineno
         return self.__selected_sig != ""
     
     def generate(self):
         return super()._generate(self.__selected_sig, self.__selected_lineno)
         
 class ManualGenerationStrategy(DocGenerationStrategy):
```

### Comparing `bimbam-5.1/thonnycontrib/docstring_generator/doc_template.py` & `bimbam-5.2/thonnycontrib/docstring_generator/doc_template.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,66 @@
 from abc import *
 import ast
-from collections import namedtuple
+from typing import List
 
-# Un objet pour représenter le vocabulaire utilisé par le template 
-class TemplateVocabulary:
-    def __init__(self, todo_label="", summary_label="", param_label="",
-                cu_label="", rtype_label="", rvalue_label="", test_label="", **kw) -> None:
-        self.todo_label = todo_label
-        self.summary_label = summary_label
-        self.param_label = param_label,
-        self.cu_label = cu_label,
-        self.rtype_label = rtype_label,
-        self.rvalue_label = rvalue_label,
-        self.test_label = test_label
-        
-        # Le vocabulaire est flexible pour introduire d'autre mots
-        for attribute, value in kw.items():
-            setattr(self, attribute, value)
-        
 class DocTemplate(ABC):
     # Ces constantes peuvent être utilisées dans les classes d'implémention
     NEW_LINE = "\n"
     DOCSTRING_SYMBOL = '"""'
     
-    def __init__(self, vocabulary=TemplateVocabulary()) -> None:
-        vocabulary.todo_label = ""
-        vocabulary.summary_label = "x_résumé_x"
-        vocabulary.param_label = "Paramètres :"
-        vocabulary.test_label = "Exemples :\n$$$ "
-        vocabulary.cu_label = "Contraintes d'utilisation : "
-        self.vocabulary = vocabulary
-                            
-    @abstractmethod
-    def _format_general_summary(self) -> str:
+    # Les mots utilisés dans le template par défault
+    TODO_LABEL = "" #"__à compléter__"
+    
+    SUMMARY_LABEL = "x_résumé_x"
+    PARAM_LABEL = "Paramètres :" 
+    CU_LABEL = "Contraintes d'utilisation : "
+    DOCTEST_LABEL = "Exemples :\n$$$ "
+    
+    def _format_params(self, params) -> str:
         """
+        Args:
+            params (List): It's a list of the arguments.
+
         Returns:
-            str: Returns a label which will indicate to write a summary of the function.
+            str: Returns the parameter representation section of a node in a docstring. 
         """
-        pass
+        if params is None:
+            return ""
+        args_to_exclude = ["self", "cls"]
+        label = self.PARAM_LABEL + self.NEW_LINE
+        format_params = ""
+        for p in params:
+            arg_type = ast.unparse(p.annotation) if p.annotation else ""     
+            arg_name = p.arg 
+            if arg_name not in args_to_exclude: 
+                format_params += "- %s (%s) : %s\n" %(arg_name, arg_type, self.TODO_LABEL)
+        return label + format_params
     
     @abstractmethod
-    def _format_params(self, params) -> str:
+    def get_parameters(self, node:ast.AST) -> List:
         """
+        Get the paramters of a given node.
+        
         Args:
-            params (List): It's a list of the arguments.
+            node (ast.AST): An AST node. 
 
         Returns:
-            str: Returns the parameter representation section of a node in a docstring. 
+            List: Returns a List of arguments of the given node.
+        """
+        for node in node.body:
+            if isinstance(node, ast.FunctionDef) and node.name == "__init__":
+                # Trouver les paramètres de la méthode __init__
+                return node.args.args
+        return []
+    
+    @abstractmethod
+    def _format_general_summary(self) -> str:
+        """
+        Returns:
+            str: Returns a label which will indicate to write a summary of the function.
         """
         pass
     
     @abstractmethod
     def _format_usage_constraints(self) -> str:
         """
         Returns:
@@ -91,60 +101,45 @@
     def get_id_signature(self) -> str: 
         pass      
     
 class DocFunctionTemplate(DocTemplate):
     '''
     Modifié pour coller au cours d'Info L1
     '''
-    def __init__(self) -> None:
-        super().__init__()
-        self.vocabulary.rvalue_label = "Valeur de retour "
-        self.vocabulary.rtype_label = "(%s) :"
-        
+    RETURN_LABEL = "Valeur de retour " 
+    RETURN_TYPE_LABEL = "(%s) :" #"__type de retour ?__ (%s)%s"
+    
     def get_parameters(self, node:ast.AST):
         """
         Get the paramters of a given node.
         
         Args:
             node (ast.AST): An AST node. Must be an ast.FunctionDef or ast.AsyncFunctionDef
 
         Returns:
             List: Returns a List of arguments of the given node.
         """
-        if isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef)):
+        if isinstance(node, ast.FunctionDef):
             return node.args.args
         return []
 
     def _format_general_summary(self):
-        return self.vocabulary.summary_label + self.NEW_LINE
-    
-    def _format_params(self, params):
-        if params is None:
-            return ""
-        args_to_exclude = ["self", "cls"]
-        label = self.vocabulary.param_label + self.NEW_LINE
-        format_params = ""
-        for p in params:
-            arg_type = ast.unparse(p.annotation) if p.annotation else ""     
-            arg_name = p.arg 
-            if arg_name not in args_to_exclude: 
-                format_params += "- %s (%s) : %s\n" %(arg_name, arg_type, self.vocabulary.todo_label)
-        return label + format_params
+        return self.SUMMARY_LABEL + self.NEW_LINE
     
     def _format_usage_constraints(self):
-        return self.vocabulary.cu_label + self.vocabulary.todo_label + self.NEW_LINE   
+        return self.CU_LABEL + self.TODO_LABEL + self.NEW_LINE   
 
     def _format_return_value(self, node: ast):
         return_type = ast.unparse(node.returns) if node.returns else ""
-        return_descr = self.vocabulary.rtype_label % return_type + self.NEW_LINE
-        return self.vocabulary.rvalue_label  + return_descr
+        return_descr = self.RETURN_TYPE_LABEL % return_type + self.NEW_LINE
+        return self.RETURN_LABEL + return_descr
     
     def _format_test_examples(self):
-        label = self.vocabulary.test_label + self.NEW_LINE
-        todo = self.vocabulary.todo_label + self.NEW_LINE
+        label = self.DOCTEST_LABEL + self.NEW_LINE
+        todo = self.TODO_LABEL + self.NEW_LINE
         return label + todo
         
     def get_template(self, node: ast.AST):
         return (
             self.DOCSTRING_SYMBOL + 
             self._format_general_summary() + self.NEW_LINE + 
             self._format_params(self.get_parameters(node))  + 
@@ -155,35 +150,41 @@
         )
     
     def get_id_signature(self): 
         return "def" 
 
 class DocClassTemplate(DocTemplate): 
     def _format_general_summary(self):
-        return self.vocabulary.summary_label + self.NEW_LINE
+        return self.SUMMARY_LABEL + self.NEW_LINE
     
-    def _format_params(self):
-        return self.vocabulary.param_label
+    def get_parameters(self, node):
+        # Parcourir les définitions de méthodes dans la classe
+        for sub_node in node.body:
+            if isinstance(sub_node, ast.FunctionDef) and sub_node.name == "__init__":
+                # Trouver les paramètres de la méthode __init__
+                return sub_node.args.args
+        return []
      
     def _format_usage_constraints(self):
-        return (self.vocabulary.cu_label +
-                self.vocabulary.todo_label +
+        return (self.CU_LABEL +
+                self.TODO_LABEL +
                 self.NEW_LINE 
             )  
 
     def _format_return_value(self):
-        return self.vocabulary.rvalue_label
+        return ""
     
     def _format_test_examples(self):
-        label = self.vocabulary.test_label + self.NEW_LINE
-        todo = self.vocabulary.todo_label + self.NEW_LINE
+        label = self.DOCTEST_LABEL + self.NEW_LINE
+        todo = self.TODO_LABEL + self.NEW_LINE
         return label + todo
             
     def get_template(self, node):
         return self.DOCSTRING_SYMBOL + \
+               self._format_params(self.get_parameters(node)) + \
                self._format_general_summary() + self.NEW_LINE + \
                self._format_usage_constraints() + \
                self._format_test_examples() + \
                self.DOCSTRING_SYMBOL + self.NEW_LINE
 
     def get_id_signature(self): 
         return "class"
```

### Comparing `bimbam-5.1/thonnycontrib/environement_vars.py` & `bimbam-5.2/thonnycontrib/environement_vars.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/exceptions.py` & `bimbam-5.2/thonnycontrib/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,12 +107,18 @@
     """
     Exception raised when no docstring cannot be generated by the generator.
     This exception is raised when a function signature contains a compilation
     error.
     """
     pass
 
-class BackendNotRestartedYetException(FrontendException):
+class BackendNotReadyYetException(FrontendException):
     """
     Exception raised when the backend is not restarted yet. 
     """
+    pass
+
+class BackendCoudntBeRestartedException(FrontendException):
+    """
+    Exception raised when the backend couldn't be restarted. 
+    """
     pass
```

### Comparing `bimbam-5.1/thonnycontrib/l1test_configuration/l1test_options.py` & `bimbam-5.2/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 from thonny.config_ui import ConfigurationPage
 from ..properties import PLUGIN_NAME
 from thonny import get_workbench
+from ..i18n.languages import tr
 
 # Default config
 DEFAULT_DOC_GENERATION_AFTER_RETURN = True
 DEFAULT_IMPORT_MODULE_IN_SHELL = True
 DEFAULT_CLOSE_FUNCTION_ROWS = False
 DEFAULT_OPEN_RED_TESTS = False
 DEFAULT_OPEN_ONLY_RED_FUNCTIONS = True
 DEFAULT_HIGHLIGHT_EXCEPTIONS = False
 DEFAULT_REPORT_EXCEPTION_DETAIL = True 
+DEFAULT_MOVE_ERRORVIEW_TO_BOTTOM = False
 
 # Option names
 AUTO_GENERATON_DOC = "auto_generaton_doc"
 IMPORT_MODULE = "import_module"
 OPEN_RED_TEST_ROWS = "open_red_rows"
 CLOSE_FUNCTION_ROWS = "close_function_rows"
 OPEN_ONLY_RED_FUNCTIONS = "open_only_red_functions"
 HIGHLIGHT_EXCEPTIONS = "highlight_exceptions"
 REPORT_EXCEPTION_DETAIL = "exception_detail"
+MOVE_ERRORVIEW_TO_BOTTOM = "move_errorview_to_bottom"
 
 # Dict of options name and default value
 OPTIONS = {
     AUTO_GENERATON_DOC : DEFAULT_DOC_GENERATION_AFTER_RETURN,
     IMPORT_MODULE : DEFAULT_IMPORT_MODULE_IN_SHELL,
     CLOSE_FUNCTION_ROWS: DEFAULT_CLOSE_FUNCTION_ROWS,
     OPEN_RED_TEST_ROWS : DEFAULT_OPEN_RED_TESTS,
     OPEN_ONLY_RED_FUNCTIONS : DEFAULT_OPEN_ONLY_RED_FUNCTIONS,
     HIGHLIGHT_EXCEPTIONS: DEFAULT_HIGHLIGHT_EXCEPTIONS,
-    REPORT_EXCEPTION_DETAIL: DEFAULT_REPORT_EXCEPTION_DETAIL
+    REPORT_EXCEPTION_DETAIL: DEFAULT_REPORT_EXCEPTION_DETAIL,
+    MOVE_ERRORVIEW_TO_BOTTOM: DEFAULT_MOVE_ERRORVIEW_TO_BOTTOM
 }
 
 def init_options():
     """
     Initialise dans le workbench les options du plugin.
     """
     for opt in OPTIONS :
@@ -52,23 +56,27 @@
     get_workbench().set_option("%s." % PLUGIN_NAME + name, value)
 
 class L1TestConfigurationPage(ConfigurationPage):
     def __init__(self, master):
         ConfigurationPage.__init__(self, master)
         
         self.add_checkbox("%s.%s" % (PLUGIN_NAME, AUTO_GENERATON_DOC), 
-                          "Générer la docstring automatiquement après un saut de ligne au niveau du nom d'une fonction.")
+                          tr("Generate the docstring automatically after a line break at a function name."))
 
         self.add_checkbox("%s.%s" % (PLUGIN_NAME, IMPORT_MODULE), 
-                          "Importer le module exécuté dans le shell.")
+                          tr("Import the module executed in the shell."))
         
         self.add_checkbox("%s.%s" % (PLUGIN_NAME, CLOSE_FUNCTION_ROWS),
-                          "Fermer toutes les lignes de fonctions dans la vue %s." % PLUGIN_NAME)
+                          tr("Close all function lines in %s view.") % PLUGIN_NAME)
          
         self.add_checkbox("%s.%s" % (PLUGIN_NAME, OPEN_ONLY_RED_FUNCTIONS),
-                          "Ouvrir seulement les lignes de fonctions rouges dans la vue %s." % PLUGIN_NAME)
+                          tr("Open only red function lines in %s view.") % PLUGIN_NAME)
         
         self.add_checkbox("%s.%s" % (PLUGIN_NAME, OPEN_RED_TEST_ROWS), 
-                          "Ouvrir les tests en echec dans la vue %s." % PLUGIN_NAME)
+                          tr("Open failed tests in %s view.") % PLUGIN_NAME)
         
         self.add_checkbox("%s.%s" % (PLUGIN_NAME, HIGHLIGHT_EXCEPTIONS), 
-                          "Mettre en évidence les tests en échec (seulement ceux qui lèvent une exception).")
+                          tr("Highlight failed tests (only those that throw an exception)."))
+        
+        self.add_checkbox("%s.%s" % (PLUGIN_NAME, MOVE_ERRORVIEW_TO_BOTTOM), 
+                          tr("Place the error view at the bottom of the Thonny IDE (next to the `Shell` view). " + 
+                             "By default, the error view is placed below the `L1Test` view."))
```

### Comparing `bimbam-5.1/thonnycontrib/l1test_frontend/__init__.py` & `bimbam-5.2/thonnycontrib/l1test_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/l1test_frontend/l1test_error_view.py` & `bimbam-5.2/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/l1test_frontend/l1test_outliner_menu.py` & `bimbam-5.2/thonnycontrib/l1test_frontend/l1test_outliner_menu.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/l1test_frontend/l1test_reporter.py` & `bimbam-5.2/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 
 class L1TestReporter():    
     def __init__(self, main_view_class=L1TestTreeView, error_view_class=L1TestErrorView):
         self.__treeview_class = main_view_class
         self.__error_view_class = error_view_class 
         
         self._workbench = thonny.get_workbench()
-
         self.__treeview: L1TestTreeView = self._workbench.get_view(self.__treeview_class.__name__)
         self.__error_view: L1TestErrorView = self._workbench.get_view(self.__error_view_class.__name__)
-    
+
     def display_error_msg(self, error_msg:str, title=CANNOT_RUN_TESTS_MSG, color="red"):
         """Display an error message into the `L1TestErrorView`.
         The `prefix_info` is the title preceding the error message.
         
         Args:
             error_msg (str): the error message to be displayed
             prefix_info (str, optional): the title preceding the error message.
```

### Comparing `bimbam-5.1/thonnycontrib/l1test_frontend/l1test_runner.py` & `bimbam-5.2/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 from thonny.common import ToplevelResponse, InlineResponse
 from thonny.workbench import WorkbenchEvent
 from thonnycontrib import l1test_frontend 
 from thonny.editors import EditorNotebook
 from thonny import editors
 import thonny
 from ..ThonnyLogsGenerator import log_in_thonny
-import pickle, inspect, thonny, time
+import pickle, inspect, thonny
 from ..l1test_configuration import l1test_options 
+from ..i18n.languages import tr
 
 
 # ErrorMsg déclare deux champs : le préfixe et le message d'erreur
 # le préfix est juste le titre qui précède le message d'erreur sur la Error view
 ErrorMsg = namedtuple("ErrorMsg", "title msg")
 
 # Le nom de l'event qui lance le redémarrage du backend thonny
@@ -74,42 +75,42 @@
             selected_line (int): The number of the selected line. 
             Default is 0 if no line is selected.
         """
         try:
             editor: EditorNotebook = get_workbench().get_editor_notebook()
             # si aucun editeur n'est ouvert sur le workbench
             if not editor.get_current_editor():
-                raise NoEditorFoundException("No editor found !\n\nPlease open an editor before running the tests.")
+                raise NoEditorFoundException(tr("No editor found !\n\nPlease open an editor before running the tests."))
             
             # cette ligne demande de sauver le fichier s'il n'a pas encore été sauvé sur
             # la machine. Si le fichier est déjà sauvé, il va permettre d'enregistrer la nouvelle
             # version du fichier.
             filename = editors.get_saved_current_script_filename(force=True)          
 
             # si le filename est null alors le fichier n'a  pas été sauvé sur machine.  
             # Ce cas survient quand l'utilisatur quitte la fenetre de sauvegarde sans sauver le fichier.
             if not filename: 
-                msg = "The file is not saved.\n\nConsider to save the file before running the tests."
+                msg = tr("The file is not saved.\n\nConsider to save the file before running the tests.")
                 raise NotSavedFileException(msg)
 
             self._filename = filename
             
             if not editor.get_current_editor_content().strip():  # L'éditeur est vide. 
                 # on a pas envie d'envoyer une commande au backend si le fichier est vide.
                 # Dans tous les cas y a rien à tester.
-                raise EmptyEditorException("The editor is empty!\n")
+                raise EmptyEditorException(tr("The editor is empty!\n"))
             
             # si on est là alors le fichier est bien sauvegardé et contient quelque chose.
             self.request_backend(selected_line)         
         except FrontendException as e: # on catche que les exception coté view
             self.terminate_running()
             self.set_has_exception(True) 
             self.show_error_view(str(e))
     
-    def request_backend(self, selected_line:int):
+    def request_backend(self, selected_line:int, count=0):
         """Allows to execute the `L1test` magic command. 
         
         There's two cases : 
         1. if the `L1test` is invoked only one time so the command is sent to 
         backend to be executed by the thonny's runner. 
         2. if the `L1test` is invoked a lot of times (lot of clicks), then we only
         consider the first invocation (first click) of the `L1test` command. While 
@@ -117,27 +118,34 @@
 
         Args:
             selected_line (int): The number of the selected line.
         """
         treeview = self._reporter.get_treeview()
         if not self.is_running(): # si l1test n'est est pas déjà en cours d'execution
             try:
-                if not thonny.get_runner().is_waiting_toplevel_command():
-                    raise BackendNotRestartedYetException("The backend is not restarted yet !")
-                
+                # si le backend n'est pas en cours prêt à recevoir une commande.
+                # cette vérification est nécessaire pour éviter le problème décrit 
+                # dans l'issue #17 (https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework/-/issues/17)
+                if not thonny.get_runner().is_waiting_toplevel_command(): 
+                    raise BackendNotReadyYetException(tr("The backend is not ready yet !"))
+                # si on est là alors le backend est prêt à recevoir une commande
                 self.set_is_running()
                 self.__request_backend(selected_line=selected_line)
-            except BackendNotRestartedYetException as e:
+            except BackendNotReadyYetException as e:
+                # si le backend n'est pas prêt à recevoir une commande alors on
+                # attend 1 seconde avant de réessayer. 
                 self.set_is_running(False)
-                treeview.insert_in_header("Waiting for the backend to restart completely...", 
+                treeview.insert_in_header(tr("Waiting for the backend to restart completely ..."), 
                                           clear=True, tags=("red"), image=ERROR_ICON)
-                thonny.get_workbench().after(1000, self.request_backend, selected_line)
+                if count > 0: # si on a déjà essayé une fois alors on arrête
+                    raise BackendCoudntBeRestartedException()
+                thonny.get_workbench().after(1000, self.request_backend, selected_line, count+1)
             except:
                 self.set_is_running(False)
-                treeview.insert_in_header("Coudn't restart the backend.\nPlease restart with the 'Stop' button !", 
+                treeview.insert_in_header(tr("Coudn't restart the backend.\nPlease restart with the 'Stop' button !"), 
                                           clear=True, tags=("red"), image=ERROR_ICON)
             finally:
                 clear_env_vars(IMPORT_MODULE_VAR, SELECTED_LINE_VAR)
         
     def __request_backend(self, command_name=BACKEND_COMMAND, selected_line:int=None):
         """
         Sends a command to the Thonny's backend to execute the current script.
@@ -342,15 +350,15 @@
             # Si c'est False alors c'est un redémarrage partiel du backend (c'est le cas d'un appel 
             # d'une nouvelle commande).
             if event.get("full"):
                 self.terminate_running()
                 self.clean_treeview(clear_all=True, clear_verdicts_data=True) 
             elif self.is_running(): # si le plugin a été lancé par l'utilisateur
                 self.clean_treeview(clear_all=True, clear_verdicts_data=True) 
-                treeview.insert_in_header("Starting executing tests ...", clear=True, tags="gray", 
+                treeview.insert_in_header(tr("Starting executing tests ..."), clear=True, tags="gray", 
                                             image=PENDING_ICON)
             else: # probablement une autre commande a déclenché le Restart du backend -> on fait rien
                 pass
             self.hide_errorview_and_show_treeview()
     
     def _handle_execution_state(self, msg: InlineResponse):
         """
```

### Comparing `bimbam-5.1/thonnycontrib/l1test_frontend/l1test_treeview.py` & `bimbam-5.2/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
         self.menu.add_command(label=FOLD_ALL, command=self.fold_rows, accelerator=BINDINGS[ALT_O])
         self.menu.add_separator() 
         self.menu.add_command(label=UPDATE_FONT_LABEL, command=self.update_font, accelerator=BINDINGS[ALT_F])
         self.menu.add_command(label=INCREASE_SPACE_BETWEEN_ROWS, command=self.increase_row_height, accelerator=BINDINGS[ALT_I])
         self.menu.add_command(label=DECREASE_SPACE_BETWEEN_ROWS, command=self.decrease_row_height, accelerator=BINDINGS[ALT_D])
         self.menu.add_separator()
         self.menu.add_command(label=CLEAR_LABEL, command=partial(self.clear_tree, clear_verdicts_data=True))
-          
+        
     def resize_header_bar(self, event=None):
         """ 
         Resize the height of the header. 
         Always keep this method otherwise the header will take the whole treeview.
         """
         height = self.tk.call((self.header_bar, "count", "-update", "-displaylines", "1.0", "end"))
         self.header_bar.configure(height=height)
@@ -466,15 +466,15 @@
         """
         widget = event.widget if event else self.treeview
         if (isinstance(widget, ttk.Treeview)): 
             view = self.workbench.get_view(self.__class__.__name__)
             if view.winfo_ismapped() :  
                 if not self.is_empty():
                     width = view.winfo_width()
-                    if self.__width_is_changed(width): # on ne met à jour que si la hauteur de la treeview n'a pas changé        
+                    if self.__width_is_changed(width): # on ne met à jour que si la largeur de la treeview a changé        
                         chars_per_pixels = width // get_font_size_option() 
                         visible_nodes = self.get_all_tree_childrens()
                         longest_length = self.__update_wrapped_texts(visible_nodes, chars_per_pixels)
                         new_rowheight = self.__compute_optimal_height(longest_length, margin)
                         self.update_row_height(new_rowheight)
                     self.__old_width = width
     
@@ -547,15 +547,15 @@
         self._restore_row_selection_effect() 
         self.clear_tree(clear_all=clear_header, clear_errorview=clear_errorview)
     
         if not self.__check_if_editor_is_open():
             return
         
         if not l1doctests:
-            self.insert_in_header("No test found !", image="warning.png", clear=True, tags=("orange",))
+            self.insert_in_header(NO_TEST_FOUND_MSG, image="warning.png", clear=True, tags=("orange",))
             return
         
         self.enable_menu()
         self.__add_verdicts_to_treeview(l1doctests, parent)
         
         # on insère le summarize dans le header bar que si la treeview n'est pas vide
         if not self.is_empty() and clear_header:
@@ -571,15 +571,15 @@
         o_names = [c_l1doctest.get_name() for c_l1doctest in self._origin_l1doctests]
         
         for l1doctest in l1doctests:
             o_index = o_names.index(l1doctest.get_name())
             current_node = self._add_node_to_tree(self._origin_l1doctests[o_index], parent)
             if l1doctest.get_flag() == L1DocTestFlag.EMPTY_FLAG:
                 self.treeview.insert(current_node, "end", values=l1doctest.get_node_lineno(), 
-                                     text="No tests found", tags=("nonClickable", l1doctest.get_flag().get_color()))
+                                     text=NO_TEST_FOUND_MSG, tags=("nonClickable", l1doctest.get_flag().get_color()))
             else:    
                 self._add_verdicts_to_node(current_node, l1doctest.get_examples())
          
         self.__wrap_tree_content()
     
     def _add_node_to_tree(self, l1doctest: L1DocTest, parent=""):  
         flag: L1DocTestFlag = l1doctest.get_flag()
@@ -649,39 +649,42 @@
         """
         Get a string that represents how many tests are passed of the given l1doctest. 
         If the l1docstest is empty, returns only the name of the l1doctest.
         """
         # The first space is necessary so that all text will be aligned
         if l1doctest.get_flag() == L1DocTestFlag.EMPTY_FLAG:
             return " %s" % l1doctest.get_name()
-        return " %s ~ %s/%s passed" %(l1doctest.get_name(), l1doctest.count_passed_tests(), l1doctest.count_tests())
+        return " %s ~ %s/%s %s" % (l1doctest.get_name(), 
+                                   l1doctest.count_passed_tests(), 
+                                   l1doctest.count_tests(),
+                                   tr("passed"))
         
     def insert_summarize_in_header_bar(self, summarize:Summarize, view: tktextext.TweakableText):
         """
         Builds the summarize test to be inserted in the header of the treeview.
         
         Args:
             summarize (Summarize): a named tuple that contains the summarize infos.
         """
-        tests_run = "Tests run: %s\n" % summarize.total
+        tests_run = "%s: %s\n" % (tr("Tests run"), summarize.total)
         view.direct_insert("end", tests_run)
         
         insert_label = lambda label, color : view.direct_insert("end", label, tags=(color,)) 
         insert_how_many = lambda how_many, is_last=False: view.direct_insert("end", f"{how_many}" if is_last else f"{how_many}, ")
       
-        insert_label("Success: ", "green")
+        insert_label(tr("Success") + ": ", "green")
         insert_how_many(summarize.success)
         
-        insert_label("Failures: ", "darkred")
+        insert_label(tr("Failures") + ": ", "darkred")
         insert_how_many(summarize.failures)
         
-        insert_label("Errors: ", "darkred")
+        insert_label(tr("Errors") + ": ", "darkred")
         insert_how_many(summarize.errors)
         
-        insert_label("Empty: ", "orange")
+        insert_label(tr("Empty") + ": ", "orange")
         insert_how_many(summarize.empty, is_last=True)
             
     def build_summarize_object(self, l1doctests:List[L1DocTest]) -> Summarize:
         """
         Builds the summarize informations. 
         The summarize contains :
             - Total number of executed tests.
```

### Comparing `bimbam-5.1/thonnycontrib/main_generator/main_generator.py` & `bimbam-5.2/thonnycontrib/main_generator/main_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from thonny.editors import EditorCodeViewText
 import re
 import tkinter as tk
 from thonny import ui_utils
 from thonnycontrib import utils
+from ..i18n.languages import tr
 
 # The regex to check if the __main__ already exists
 # The regex checks if a string already contains the __main__ and not commented.
 _REGEX = re.compile(r"(?m)^\s*if\s+__name__\s*==\s*['\"]__main__['\"]\s*:\s*")
 
 # The generated `__main__` function. 
 # Leave a blank line before the `if __name__ == '__main__':` line, 
@@ -17,16 +18,16 @@
 if __name__ == '__main__':
     # éxécuté qd ce module n'est pas initialisé par un import.
     pass
 """
 )
 
 # used to tell the user whether the __main_ is generated or not
-MAIN_EXISTS_MSG = "`__main__` existe déjà"
-MAIN_GENERATED_MSG = "`__main__` généré"
+MAIN_EXISTS_MSG = "`__main__` " + tr("already exists")
+MAIN_GENERATED_MSG = "`__main__` " + tr("generated")
 
 class MainGenerator(): 
     """
     This class is responsible for generating the __main__ function.
     It takes a source code as input and generates the __main__ function 
     at the bottom of the source code.
```

### Comparing `bimbam-5.1/thonnycontrib/plugin_loader.py` & `bimbam-5.2/thonnycontrib/plugin_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from thonny import get_workbench
 from thonny.ui_utils import select_sequence
-from .docstring_generator.doc_generator import DocGenerator
 from .l1test_frontend.l1test_reporter import L1TestErrorView, L1TestTreeView
 from .main_generator.main_generator import MainGenerator
-from .exceptions import *
 from .properties import  ERROR_VIEW_LABEL, PLUGIN_NAME
 from .utils import (
     assert_one_line_is_selected,
     get_focused_writable_text,
     get_selected_line, 
     get_image_path
 )
 from .l1test_configuration.l1test_options import *
 from .l1test_frontend import get_l1test_runner
 from .l1test_frontend import get_outliner
-from .environement_vars import *
 from functools import partial
 from .docstring_generator import get_doc_generator
+import thonnycontrib.i18n.languages as languages
+
 
 def run_all_tests():
     """
     Cette fonction est invoquée quand le button `l1test` est cliqué.
     Cette fonction permet d'envoyer au l1test_backend la commande L1test.
     """
     get_l1test_runner().run_l1test()
+    
       
 def generate_docstring(auto: bool, event=None): 
     """
     Cette fonction est invoquée quand le button `doc_generator` est cliqué. Ou quand on 
     réalise un saut de ligne après la déclaration d'une fonction.
 
     Args:
@@ -39,14 +39,15 @@
     """
     if _writable_text_is_focused(): # on vérifie si la zone séléctionnée est une zone de l'éditeur
         text_widget = get_focused_writable_text()
         selected_line = get_selected_line(text_widget) 
         docGenerator = get_doc_generator(auto)  
         docGenerator.run(selected_line - 1 if auto else selected_line, text_widget)
 
+
 def generate_main():
     """
     Generate the __main__ function.
     """
     text_widget = get_focused_writable_text()
     main_generator = MainGenerator(text_widget.get("1.0", "end"))
     main_generator.generate(text_widget)
@@ -57,52 +58,58 @@
     """
     Returns:
         boolean: Returns True if the selected zone is a writable text.
     """
     return get_focused_writable_text() is not None
 
 
+## PRIVATE FUNCTIONS : constructing and configuring of the plugin ##
+####################################################################
+
+def __init_language():
+    languages.set_language(get_workbench().get_option("general.language"))
+
 def __init_l1test_options():
     init_options()
     get_workbench().add_configuration_page(PLUGIN_NAME, PLUGIN_NAME, L1TestConfigurationPage, 30)
 
 def __init_l1test_views():
     get_workbench().add_view(L1TestTreeView, PLUGIN_NAME, "nw", visible_by_default=True)
-    get_workbench().add_view(L1TestErrorView, ERROR_VIEW_LABEL, "sw", visible_by_default=False)
+    get_workbench().add_view(L1TestErrorView, ERROR_VIEW_LABEL, "sw" if not get_option(MOVE_ERRORVIEW_TO_BOTTOM) else "s", visible_by_default=False)
 
 def __init_l1test_commands():
     # Création du button l1test au niveau de la barre des commandes
     get_workbench().add_command(command_id=PLUGIN_NAME,
                                 menu_name=PLUGIN_NAME,  
-                                command_label="Run all tests",
+                                command_label=tr("Run all tests"),
                                 handler=run_all_tests,
                                 include_in_toolbar=True, #j'inclue ici ce bouton dans la toolbar 
                                 image=get_image_path("l1test_icon.png"),
                                 caption=PLUGIN_NAME)
     
     # Création du button L1Test dans la barre de menu en haut.  
     get_workbench().add_command(command_id="Run one test",
                                 menu_name=PLUGIN_NAME,  
-                                command_label="Run tests for ...",
+                                command_label=tr("Run tests for ..."),
                                 image=get_image_path("l1test_icon.png"),
                                 submenu=get_outliner().get_menu()
     )
     
     # Création du bouton dans le menu 'Edit' pour lancer la génération de docstring
     get_workbench().add_command(command_id="doc_generator",
                                 menu_name="edit",  
-                                command_label="Generate a docstring",
+                                command_label=tr("Generate a docstring"),
                                 handler=partial(generate_docstring, auto=False), 
                                 tester=_writable_text_is_focused and assert_one_line_is_selected,
     )
      
     # Création du bouton dans le menu 'Edit' pour générer le main
     get_workbench().add_command(command_id="main_generator",
                                 menu_name="edit",  
-                                command_label="Generate a main",
+                                command_label=tr("Generate a __main__"),
                                 handler=generate_main, 
                                 tester=_writable_text_is_focused,
                                 default_sequence=select_sequence("<Alt-m>", "<Command-Alt-m>", "<Alt-m>"),
                                 accelerator="Alt+m"
     )
 
 def __add_event_binding():
@@ -113,11 +120,12 @@
                                lambda event: generate_docstring(auto=get_option(AUTO_GENERATON_DOC), event=event))
 
 def load_plugin():
     """
     load_plugin est un nom de fonction spécifique qui permet à thonny de charger les élements du plugin
     """
     # these functions should be called in this order
+    __init_language()
     __init_l1test_options()
     __init_l1test_views()    
     __init_l1test_commands()
-    __add_event_binding()
+    __add_event_binding()
```

### Comparing `bimbam-5.1/thonnycontrib/properties.py` & `bimbam-5.2/thonnycontrib/properties.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from .i18n.languages import tr
+
 PLUGIN_NAME = "L1Test"
-DEBUG_NAME = "L1Test debugger"
 ERROR_VIEW_LABEL = '%s errors' % PLUGIN_NAME
 
 # ici vous pouvez changer la syntaxe du doctest. 
 # version 2022 PJI : Actuellement on garde la syntaxe `$py`.
 L1TEST_SYMBOL = "[$]py"
 # version 2022 avant la rentrée
 L1TEST_SYMBOL1 = "[$][$][$]"
@@ -25,38 +26,41 @@
 # Le nom de l'attribut contenant les résulats des tests renvoyés par l1test_backend
 VERDICTS = "verdicts"
 # Le nom de l'attribut contenant une exception levée et renvoyée par l1test_backend
 L1TEST_EXCEPTION = "l1test_exception"
 
 
 # ############ Les labels des buttons du menu l1test treeview ############
-PLACE_RED_TEST_ON_TOP_LABEL = "Place the red tests on the top"
-RESUME_ORIGINAL_ORDER = "Resume original order"
-SHOW_ONLY_RED_TESTS = "Show only red tests"
-SHOW_ALL_TESTS = "Show all the tests"
-GROUP_BY_VERDICTS = "Group by verdicts"
-EXPAND_ALL = "Expand all"
-FOLD_ALL = "Fold all"
-UPDATE_FONT_LABEL = "Update the font"
-INCREASE_SPACE_BETWEEN_ROWS = "Inrease row height"
-DECREASE_SPACE_BETWEEN_ROWS = "Decrease row height"
-CLEAR_LABEL = "Clear"
+PLACE_RED_TEST_ON_TOP_LABEL = tr("Place the red tests on the top")
+RESUME_ORIGINAL_ORDER = tr("Resume original order")
+SHOW_ONLY_RED_TESTS = tr("Show only red tests")
+SHOW_ALL_TESTS = tr("Show all the tests")
+GROUP_BY_VERDICTS = tr("Group by verdicts")
+EXPAND_ALL = tr("Expand all")
+FOLD_ALL = tr("Fold all")
+UPDATE_FONT_LABEL = tr("Update the font")
+INCREASE_SPACE_BETWEEN_ROWS = tr("Inrease row height")
+DECREASE_SPACE_BETWEEN_ROWS = tr("Decrease row height")
+CLEAR_LABEL = tr("Clear")
 
 # Le message affiché sur la treeview quand `l1test` est en cours d'execution
-L1TEST_IN_PROGRESS = "Executing tests in progress"
+L1TEST_IN_PROGRESS = tr("Executing tests in progress")
+
+# Le message affiché sur la treeview quand il n'existe aucun test
+NO_TEST_FOUND_MSG = tr("No test found !")
 
 # the evaluation states
 PENDING_STATE = "Pending" 
 EXECUTED_STATE = "Executed" 
 FINISHED_STATE = "Finished"
 
 # The title of the error view when the docstring genertor shows the raised error
-CANNOT_GENERATE_THE_DOCSTRING = "Cannot generate the docstring :"
+CANNOT_GENERATE_THE_DOCSTRING = tr("Cannot generate the docstring :")
 # The title of the error view when the l1test shows the raised error
-CANNOT_RUN_TESTS_MSG = "Cannot run %s :" %(PLUGIN_NAME)
+CANNOT_RUN_TESTS_MSG = tr("Cannot run %s :" %(PLUGIN_NAME))
 
 # A special event that `L1TestTreeview` sends to `L1TestRunner` when clicking on an exception test
 # The event transfers the details of the clicked exception to the `L1TestRunner` 
 # which will show it in the error view.
 L1TREE_VIEW_EVENT = "L1TreeviewEvent"
 
 # Les images utilisées par la treeview
```

### Comparing `bimbam-5.1/thonnycontrib/tests/fixtures/workbench_mock.py` & `bimbam-5.2/thonnycontrib/tests/fixtures/workbench_mock.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/tests/tests_doc_generator.py` & `bimbam-5.2/thonnycontrib/tests/tests_doc_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/tests/tests_example_no_expected.py` & `bimbam-5.2/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/tests/tests_example_with_exception.py` & `bimbam-5.2/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/tests/tests_example_with_expected.py` & `bimbam-5.2/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/tests/tests_l1TestRunner.py` & `bimbam-5.2/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/tests/tests_main_generator.py` & `bimbam-5.2/thonnycontrib/tests/tests_main_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/tests/tests_test_finder.py` & `bimbam-5.2/thonnycontrib/tests/tests_test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/tests/tests_view.py` & `bimbam-5.2/thonnycontrib/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.1/thonnycontrib/utils.py` & `bimbam-5.2/thonnycontrib/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from thonny import get_workbench
 from thonnycontrib.exceptions import CannotImportModuleException, CompilationError
 from .properties import BACKEND_COMMAND 
 from .environement_vars import *
 import os, re, ast, traceback, textwrap, tkinter as tk
 import thonny
 from thonny.editors import EditorCodeViewText
+from .i18n.languages import tr
 
 def wrap(string:str, length=8, break_long_words=False):   
     """Wrap a text using the `wraptext` module.
 
     Args:
         string (str): the string to wrap.
         length (int, optional): the min length from which the string will be wrapped. Defaults to 8.
@@ -257,19 +258,19 @@
     
     # import the module specification. 
     # To learn more about ModuleSpec `https://peps.python.org/pep-0451/`    
     module_name = get_module_name(filename)
     spec = iu.spec_from_file_location(module_name, filename)
     if not spec: 
         if not filename.endswith(".py"):
-            msg_error = "The file \"%s\" cannot be imported.\n\n" % filename + \
-                        "Please, be sure that the extension of the file is `.py`" 
+            msg_error = tr("The file \"%s\" cannot be imported.\n\n" + 
+                           "Please, be sure that the extension of the file is `.py`") % filename 
         else:
-            msg_error = "Cannot found the file `%s`" %filename 
-        msg_error = "Error when importing the module \"%s\":\n" % module_name + msg_error
+            msg_error = tr("Cannot found the file `%s`") %filename 
+        msg_error = tr("Error when importing the module \"%s\":\n") % module_name + msg_error
         raise CannotImportModuleException(msg_error)
     
     imported_source = iu.module_from_spec(spec)
     
     workingdir = os.path.split(imported_source.__file__)
     if (len(workingdir) > 0):
         basedir = workingdir[0]
```

