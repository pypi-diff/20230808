# Comparing `tmp/bimbam-5.0.tar.gz` & `tmp/bimbam-5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bimbam-5.0.tar", last modified: Wed Aug  2 21:49:48 2023, max compression
+gzip compressed data, was "bimbam-5.1.tar", last modified: Tue Aug  8 00:33:37 2023, max compression
```

## Comparing `bimbam-5.0.tar` & `bimbam-5.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 21:49:48.420767 bimbam-5.0/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-08-02 21:49:48.420767 bimbam-5.0/PKG-INFO
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 21:49:48.408766 bimbam-5.0/bimbam.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-08-02 21:49:48.000000 bimbam-5.0/bimbam.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2648 2023-08-02 21:49:48.000000 bimbam-5.0/bimbam.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-08-02 21:49:48.000000 bimbam-5.0/bimbam.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-02 21:49:48.000000 bimbam-5.0/bimbam.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-02 21:49:48.000000 bimbam-5.0/bimbam.egg-info/top_level.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-08-02 21:49:48.420767 bimbam-5.0/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1961 2023-08-02 21:49:44.000000 bimbam-5.0/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 21:49:48.408766 bimbam-5.0/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1741 2023-08-01 23:02:20.000000 bimbam-5.0/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 21:49:48.412767 bimbam-5.0/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17236 2023-08-01 23:42:41.000000 bimbam-5.0/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-5.0/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-31 20:39:03.000000 bimbam-5.0/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-5.0/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5653 2023-07-31 20:57:44.000000 bimbam-5.0/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 21:49:48.412767 bimbam-5.0/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-5.0/thonnycontrib/backend/verdicts/ExampleVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/backend/verdicts/ExceptionVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-5.0/thonnycontrib/backend/verdicts/FailedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-5.0/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/backend/verdicts/PassedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 21:49:48.412767 bimbam-5.0/thonnycontrib/docs/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/docs/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 21:49:48.416767 bimbam-5.0/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/docs/res/error_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-5.0/thonnycontrib/docs/res/exception_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-5.0/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/docs/res/failed_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/docs/res/outline_class.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/docs/res/outline_method.gif
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-5.0/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2144 2023-08-01 23:56:58.000000 bimbam-5.0/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/docs/res/restart_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/docs/res/success_green_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 21:49:48.416767 bimbam-5.0/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      585 2023-07-29 21:42:29.000000 bimbam-5.0/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16176 2023-08-01 23:32:20.000000 bimbam-5.0/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7054 2023-07-22 09:12:15.000000 bimbam-5.0/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-5.0/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3521 2023-08-02 21:47:51.000000 bimbam-5.0/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 21:49:48.416767 bimbam-5.0/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2991 2023-07-23 10:41:36.000000 bimbam-5.0/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 21:49:48.416767 bimbam-5.0/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-5.0/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-5.0/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-5.0/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2749 2023-07-23 16:34:32.000000 bimbam-5.0/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    23597 2023-08-02 21:48:21.000000 bimbam-5.0/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41636 2023-08-01 23:49:06.000000 bimbam-5.0/thonnycontrib/l1test_frontend/l1test_treeview.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 21:49:48.416767 bimbam-5.0/thonnycontrib/main_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-5.0/thonnycontrib/main_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5301 2023-07-28 14:35:18.000000 bimbam-5.0/thonnycontrib/main_generator/main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5453 2023-07-30 12:38:45.000000 bimbam-5.0/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2962 2023-07-27 19:06:48.000000 bimbam-5.0/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 21:49:48.420767 bimbam-5.0/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/tests/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-02 21:49:48.420767 bimbam-5.0/thonnycontrib/tests/fixtures/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-5.0/thonnycontrib/tests/fixtures/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-5.0/thonnycontrib/tests/fixtures/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-5.0/thonnycontrib/tests/fixtures/workbench_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2505 2023-07-30 12:46:52.000000 bimbam-5.0/thonnycontrib/tests/tests_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-5.0/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-5.0/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-5.0/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-5.0/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-5.0/thonnycontrib/tests/tests_main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-5.0/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-5.0/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17858 2023-08-01 23:47:43.000000 bimbam-5.0/thonnycontrib/utils.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.952432 bimbam-5.1/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-08-08 00:33:37.952432 bimbam-5.1/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.940431 bimbam-5.1/bimbam.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-08-08 00:33:37.000000 bimbam-5.1/bimbam.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2648 2023-08-08 00:33:37.000000 bimbam-5.1/bimbam.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-08-08 00:33:37.000000 bimbam-5.1/bimbam.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-08 00:33:37.000000 bimbam-5.1/bimbam.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-08 00:33:37.000000 bimbam-5.1/bimbam.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-08-08 00:33:37.952432 bimbam-5.1/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2054 2023-08-08 00:33:21.000000 bimbam-5.1/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.940431 bimbam-5.1/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1741 2023-08-01 23:02:20.000000 bimbam-5.1/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.944431 bimbam-5.1/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17236 2023-08-01 23:42:41.000000 bimbam-5.1/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-5.1/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-31 20:39:03.000000 bimbam-5.1/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-5.1/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5653 2023-07-31 20:57:44.000000 bimbam-5.1/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.944431 bimbam-5.1/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-5.1/thonnycontrib/backend/verdicts/ExampleVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/backend/verdicts/ExceptionVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-5.1/thonnycontrib/backend/verdicts/FailedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-5.1/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/backend/verdicts/PassedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.944431 bimbam-5.1/thonnycontrib/docs/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.948431 bimbam-5.1/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/error_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-5.1/thonnycontrib/docs/res/exception_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-5.1/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/failed_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/outline_class.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/outline_method.gif
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-5.1/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2144 2023-08-01 23:56:58.000000 bimbam-5.1/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/restart_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/success_green_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.948431 bimbam-5.1/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      585 2023-07-29 21:42:29.000000 bimbam-5.1/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16176 2023-08-01 23:32:20.000000 bimbam-5.1/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7054 2023-07-22 09:12:15.000000 bimbam-5.1/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-5.1/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3521 2023-08-02 21:47:51.000000 bimbam-5.1/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.948431 bimbam-5.1/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2991 2023-07-23 10:41:36.000000 bimbam-5.1/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.948431 bimbam-5.1/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-5.1/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-5.1/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-5.1/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2749 2023-07-23 16:34:32.000000 bimbam-5.1/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    23597 2023-08-02 21:48:21.000000 bimbam-5.1/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41636 2023-08-01 23:49:06.000000 bimbam-5.1/thonnycontrib/l1test_frontend/l1test_treeview.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.952432 bimbam-5.1/thonnycontrib/main_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-5.1/thonnycontrib/main_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5301 2023-07-28 14:35:18.000000 bimbam-5.1/thonnycontrib/main_generator/main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5453 2023-07-30 12:38:45.000000 bimbam-5.1/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2962 2023-07-27 19:06:48.000000 bimbam-5.1/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.952432 bimbam-5.1/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/tests/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:33:37.952432 bimbam-5.1/thonnycontrib/tests/fixtures/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-5.1/thonnycontrib/tests/fixtures/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-5.1/thonnycontrib/tests/fixtures/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-5.1/thonnycontrib/tests/fixtures/workbench_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2505 2023-07-30 12:46:52.000000 bimbam-5.1/thonnycontrib/tests/tests_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-5.1/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-5.1/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-5.1/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-5.1/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-5.1/thonnycontrib/tests/tests_main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-5.1/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-5.1/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17858 2023-08-01 23:47:43.000000 bimbam-5.1/thonnycontrib/utils.py
```

### Comparing `bimbam-5.0/PKG-INFO` & `bimbam-5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 5.0
+Version: 5.1
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-5.0/bimbam.egg-info/PKG-INFO` & `bimbam-5.1/bimbam.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 5.0
+Version: 5.1
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-5.0/bimbam.egg-info/SOURCES.txt` & `bimbam-5.1/bimbam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/setup.py` & `bimbam-5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,23 +20,24 @@
     return packages
 
 packages = get_packages_under_thonnycontrib(thonnycontrib_path, "thonnycontrib")
 
 def get_packages_data(packages: list[str]=packages):
     py_packs = dict([(p, ["*.py"]) for p in packages if not p.endswith("docs")])
     other_packs = dict([(p, ["res/*"]) for p in packages if p.endswith("docs")])
+    i18n_packs = dict([(p, ["i18n/*"]) for p in packages if "i18n" in p])
     
-    return py_packs | other_packs
+    return {**py_packs, **other_packs, **i18n_packs}
 
 setupdir = os.path.dirname(__file__)
 
 
 setup(
     name="bimbam",
-    version="5.0",
+    version="5.1",
     author="idtaleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests""",
     url="https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests",
 #    keywords="IDE education programming tests in documentation",
```

### Comparing `bimbam-5.0/thonnycontrib/ThonnyLogsGenerator.py` & `bimbam-5.1/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/backend/ast_parser.py` & `bimbam-5.1/thonnycontrib/backend/ast_parser.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/backend/doctest_parser.py` & `bimbam-5.1/thonnycontrib/backend/doctest_parser.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/backend/evaluator.py` & `bimbam-5.1/thonnycontrib/backend/evaluator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/backend/l1test_backend.py` & `bimbam-5.1/thonnycontrib/backend/l1test_backend.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/backend/test_finder.py` & `bimbam-5.1/thonnycontrib/backend/test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/backend/verdicts/ExampleVerdict.py` & `bimbam-5.1/thonnycontrib/backend/verdicts/ExampleVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/backend/verdicts/FailedVerdict.py` & `bimbam-5.1/thonnycontrib/backend/verdicts/FailedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py` & `bimbam-5.1/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/docs/res/error_icon.png` & `bimbam-5.1/thonnycontrib/docs/res/error_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/docs/res/exception_red_chip.png` & `bimbam-5.1/thonnycontrib/docs/res/exception_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/docs/res/failed.png` & `bimbam-5.1/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/docs/res/failed_red_chip.png` & `bimbam-5.1/thonnycontrib/docs/res/failed_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/docs/res/l1test_icon.png` & `bimbam-5.1/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/docs/res/l1test_icon_old.png` & `bimbam-5.1/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/docs/res/outline_class.png` & `bimbam-5.1/thonnycontrib/docs/res/outline_class.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/docs/res/outline_method.gif` & `bimbam-5.1/thonnycontrib/docs/res/outline_method.gif`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/docs/res/passed.png` & `bimbam-5.1/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/docs/res/pending_icon.png` & `bimbam-5.1/thonnycontrib/docs/res/pending_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/docs/res/restart_icon.png` & `bimbam-5.1/thonnycontrib/docs/res/restart_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/docs/res/success_green_chip.png` & `bimbam-5.1/thonnycontrib/docs/res/success_green_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/docs/res/warning.png` & `bimbam-5.1/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/docstring_generator/__init__.py` & `bimbam-5.1/thonnycontrib/docstring_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/docstring_generator/doc_generator.py` & `bimbam-5.1/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/docstring_generator/doc_template.py` & `bimbam-5.1/thonnycontrib/docstring_generator/doc_template.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/environement_vars.py` & `bimbam-5.1/thonnycontrib/environement_vars.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/exceptions.py` & `bimbam-5.1/thonnycontrib/exceptions.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/l1test_configuration/l1test_options.py` & `bimbam-5.1/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/l1test_frontend/__init__.py` & `bimbam-5.1/thonnycontrib/l1test_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/l1test_frontend/l1test_error_view.py` & `bimbam-5.1/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/l1test_frontend/l1test_outliner_menu.py` & `bimbam-5.1/thonnycontrib/l1test_frontend/l1test_outliner_menu.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/l1test_frontend/l1test_reporter.py` & `bimbam-5.1/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/l1test_frontend/l1test_runner.py` & `bimbam-5.1/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/l1test_frontend/l1test_treeview.py` & `bimbam-5.1/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/main_generator/main_generator.py` & `bimbam-5.1/thonnycontrib/main_generator/main_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/plugin_loader.py` & `bimbam-5.1/thonnycontrib/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/properties.py` & `bimbam-5.1/thonnycontrib/properties.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/tests/fixtures/workbench_mock.py` & `bimbam-5.1/thonnycontrib/tests/fixtures/workbench_mock.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/tests/tests_doc_generator.py` & `bimbam-5.1/thonnycontrib/tests/tests_doc_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/tests/tests_example_no_expected.py` & `bimbam-5.1/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/tests/tests_example_with_exception.py` & `bimbam-5.1/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/tests/tests_example_with_expected.py` & `bimbam-5.1/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/tests/tests_l1TestRunner.py` & `bimbam-5.1/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/tests/tests_main_generator.py` & `bimbam-5.1/thonnycontrib/tests/tests_main_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/tests/tests_test_finder.py` & `bimbam-5.1/thonnycontrib/tests/tests_test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/tests/tests_view.py` & `bimbam-5.1/thonnycontrib/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.0/thonnycontrib/utils.py` & `bimbam-5.1/thonnycontrib/utils.py`

 * *Files identical despite different names*

