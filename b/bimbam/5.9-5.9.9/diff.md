# Comparing `tmp/bimbam-5.9.tar.gz` & `tmp/bimbam-5.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bimbam-5.9.tar", last modified: Tue Aug  8 21:07:56 2023, max compression
+gzip compressed data, was "bimbam-5.9.9.tar", last modified: Tue Aug  8 21:17:55 2023, max compression
```

## Comparing `bimbam-5.9.tar` & `bimbam-5.9.9.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.776820 bimbam-5.9/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-08-08 21:07:56.776820 bimbam-5.9/PKG-INFO
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.760819 bimbam-5.9/bimbam.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-08-08 21:07:56.000000 bimbam-5.9/bimbam.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2973 2023-08-08 21:07:56.000000 bimbam-5.9/bimbam.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-08-08 21:07:56.000000 bimbam-5.9/bimbam.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-08 21:07:56.000000 bimbam-5.9/bimbam.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-08 21:07:56.000000 bimbam-5.9/bimbam.egg-info/top_level.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-08-08 21:07:56.776820 bimbam-5.9/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1945 2023-08-08 21:07:32.000000 bimbam-5.9/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.764819 bimbam-5.9/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1741 2023-08-01 23:02:20.000000 bimbam-5.9/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 20:38:37.000000 bimbam-5.9/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.764819 bimbam-5.9/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17261 2023-08-03 20:16:42.000000 bimbam-5.9/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-5.9/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-31 20:39:03.000000 bimbam-5.9/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-5.9/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5653 2023-07-31 20:57:44.000000 bimbam-5.9/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.768819 bimbam-5.9/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-5.9/thonnycontrib/backend/verdicts/ExampleVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/backend/verdicts/ExceptionVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-5.9/thonnycontrib/backend/verdicts/FailedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-5.9/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/backend/verdicts/PassedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.760819 bimbam-5.9/thonnycontrib/docs/
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.768819 bimbam-5.9/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/docs/res/error_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-5.9/thonnycontrib/docs/res/exception_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-5.9/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/docs/res/failed_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/docs/res/outline_class.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/docs/res/outline_method.gif
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-5.9/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2144 2023-08-01 23:56:58.000000 bimbam-5.9/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/docs/res/restart_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/docs/res/success_green_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.768819 bimbam-5.9/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      585 2023-07-29 21:42:29.000000 bimbam-5.9/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    15559 2023-08-08 20:41:15.000000 bimbam-5.9/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6751 2023-08-03 22:03:53.000000 bimbam-5.9/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-5.9/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3665 2023-08-07 21:57:09.000000 bimbam-5.9/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.768819 bimbam-5.9/thonnycontrib/i18n/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:28:42.000000 bimbam-5.9/thonnycontrib/i18n/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      702 2023-08-08 20:51:21.000000 bimbam-5.9/thonnycontrib/i18n/languages.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.768819 bimbam-5.9/thonnycontrib/i18n/locale/
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.760819 bimbam-5.9/thonnycontrib/i18n/locale/en_US/
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.768819 bimbam-5.9/thonnycontrib/i18n/locale/en_US/LC_MESSAGES/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      214 2023-08-08 19:53:22.000000 bimbam-5.9/thonnycontrib/i18n/locale/en_US/LC_MESSAGES/l1test.mo
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4601 2023-08-08 19:52:54.000000 bimbam-5.9/thonnycontrib/i18n/locale/en_US/LC_MESSAGES/l1test.po
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.760819 bimbam-5.9/thonnycontrib/i18n/locale/fr_FR/
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.772819 bimbam-5.9/thonnycontrib/i18n/locale/fr_FR/LC_MESSAGES/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4231 2023-08-08 19:53:22.000000 bimbam-5.9/thonnycontrib/i18n/locale/fr_FR/LC_MESSAGES/l1test.mo
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6271 2023-08-08 19:52:44.000000 bimbam-5.9/thonnycontrib/i18n/locale/fr_FR/LC_MESSAGES/l1test.po
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5169 2023-08-08 19:52:04.000000 bimbam-5.9/thonnycontrib/i18n/locale/l1test.pot
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.772819 bimbam-5.9/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3406 2023-08-07 22:33:46.000000 bimbam-5.9/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.772819 bimbam-5.9/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-5.9/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-5.9/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-5.9/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2744 2023-08-08 20:38:56.000000 bimbam-5.9/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    25479 2023-08-08 20:38:50.000000 bimbam-5.9/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41800 2023-08-08 21:03:53.000000 bimbam-5.9/thonnycontrib/l1test_frontend/l1test_treeview.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.772819 bimbam-5.9/thonnycontrib/main_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-5.9/thonnycontrib/main_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5361 2023-08-08 18:21:40.000000 bimbam-5.9/thonnycontrib/main_generator/main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5723 2023-08-08 20:49:14.000000 bimbam-5.9/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3380 2023-08-08 21:02:09.000000 bimbam-5.9/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.776820 bimbam-5.9/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/tests/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:07:56.776820 bimbam-5.9/thonnycontrib/tests/fixtures/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-5.9/thonnycontrib/tests/fixtures/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-5.9/thonnycontrib/tests/fixtures/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-5.9/thonnycontrib/tests/fixtures/workbench_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-03 20:14:25.000000 bimbam-5.9/thonnycontrib/tests/tests_ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2302 2023-08-08 18:13:09.000000 bimbam-5.9/thonnycontrib/tests/tests_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-5.9/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-5.9/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-5.9/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-5.9/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-5.9/thonnycontrib/tests/tests_main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-5.9/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-5.9/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17903 2023-08-07 21:19:21.000000 bimbam-5.9/thonnycontrib/utils.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.988592 bimbam-5.9.9/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      666 2023-08-08 21:17:55.988592 bimbam-5.9.9/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.976592 bimbam-5.9.9/bimbam.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      666 2023-08-08 21:17:55.000000 bimbam-5.9.9/bimbam.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2973 2023-08-08 21:17:55.000000 bimbam-5.9.9/bimbam.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-08-08 21:17:55.000000 bimbam-5.9.9/bimbam.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-08 21:17:55.000000 bimbam-5.9.9/bimbam.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-08-08 21:17:55.000000 bimbam-5.9.9/bimbam.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-08-08 21:17:55.988592 bimbam-5.9.9/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1947 2023-08-08 21:17:14.000000 bimbam-5.9.9/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.976592 bimbam-5.9.9/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1741 2023-08-01 23:02:20.000000 bimbam-5.9.9/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 20:38:37.000000 bimbam-5.9.9/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.976592 bimbam-5.9.9/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17261 2023-08-03 20:16:42.000000 bimbam-5.9.9/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-5.9.9/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-31 20:39:03.000000 bimbam-5.9.9/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-5.9.9/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5653 2023-07-31 20:57:44.000000 bimbam-5.9.9/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.980592 bimbam-5.9.9/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-5.9.9/thonnycontrib/backend/verdicts/ExampleVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/backend/verdicts/ExceptionVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-5.9.9/thonnycontrib/backend/verdicts/FailedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-5.9.9/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/backend/verdicts/PassedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.972592 bimbam-5.9.9/thonnycontrib/docs/
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.980592 bimbam-5.9.9/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/docs/res/error_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-5.9.9/thonnycontrib/docs/res/exception_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-5.9.9/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/docs/res/failed_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/docs/res/outline_class.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/docs/res/outline_method.gif
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-5.9.9/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2144 2023-08-01 23:56:58.000000 bimbam-5.9.9/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/docs/res/restart_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/docs/res/success_green_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.980592 bimbam-5.9.9/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      585 2023-07-29 21:42:29.000000 bimbam-5.9.9/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    15559 2023-08-08 20:41:15.000000 bimbam-5.9.9/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6751 2023-08-03 22:03:53.000000 bimbam-5.9.9/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-5.9.9/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3665 2023-08-07 21:57:09.000000 bimbam-5.9.9/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.984592 bimbam-5.9.9/thonnycontrib/i18n/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 00:28:42.000000 bimbam-5.9.9/thonnycontrib/i18n/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      702 2023-08-08 20:51:21.000000 bimbam-5.9.9/thonnycontrib/i18n/languages.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.984592 bimbam-5.9.9/thonnycontrib/i18n/locale/
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.972592 bimbam-5.9.9/thonnycontrib/i18n/locale/en_US/
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.984592 bimbam-5.9.9/thonnycontrib/i18n/locale/en_US/LC_MESSAGES/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      214 2023-08-08 19:53:22.000000 bimbam-5.9.9/thonnycontrib/i18n/locale/en_US/LC_MESSAGES/l1test.mo
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4601 2023-08-08 19:52:54.000000 bimbam-5.9.9/thonnycontrib/i18n/locale/en_US/LC_MESSAGES/l1test.po
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.972592 bimbam-5.9.9/thonnycontrib/i18n/locale/fr_FR/
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.984592 bimbam-5.9.9/thonnycontrib/i18n/locale/fr_FR/LC_MESSAGES/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4231 2023-08-08 19:53:22.000000 bimbam-5.9.9/thonnycontrib/i18n/locale/fr_FR/LC_MESSAGES/l1test.mo
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6271 2023-08-08 19:52:44.000000 bimbam-5.9.9/thonnycontrib/i18n/locale/fr_FR/LC_MESSAGES/l1test.po
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5169 2023-08-08 19:52:04.000000 bimbam-5.9.9/thonnycontrib/i18n/locale/l1test.pot
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.984592 bimbam-5.9.9/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3406 2023-08-07 22:33:46.000000 bimbam-5.9.9/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.984592 bimbam-5.9.9/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-5.9.9/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-5.9.9/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-5.9.9/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2744 2023-08-08 20:38:56.000000 bimbam-5.9.9/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    25479 2023-08-08 20:38:50.000000 bimbam-5.9.9/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41868 2023-08-08 21:15:05.000000 bimbam-5.9.9/thonnycontrib/l1test_frontend/l1test_treeview.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.984592 bimbam-5.9.9/thonnycontrib/main_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-5.9.9/thonnycontrib/main_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5361 2023-08-08 18:21:40.000000 bimbam-5.9.9/thonnycontrib/main_generator/main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5723 2023-08-08 20:49:14.000000 bimbam-5.9.9/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3380 2023-08-08 21:02:09.000000 bimbam-5.9.9/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.988592 bimbam-5.9.9/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/tests/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-08 21:17:55.988592 bimbam-5.9.9/thonnycontrib/tests/fixtures/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-5.9.9/thonnycontrib/tests/fixtures/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-5.9.9/thonnycontrib/tests/fixtures/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-5.9.9/thonnycontrib/tests/fixtures/workbench_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-08-03 20:14:25.000000 bimbam-5.9.9/thonnycontrib/tests/tests_ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2302 2023-08-08 18:13:09.000000 bimbam-5.9.9/thonnycontrib/tests/tests_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-5.9.9/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-5.9.9/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-5.9.9/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-5.9.9/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-5.9.9/thonnycontrib/tests/tests_main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-5.9.9/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-5.9.9/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17903 2023-08-07 21:19:21.000000 bimbam-5.9.9/thonnycontrib/utils.py
```

### Comparing `bimbam-5.9/PKG-INFO` & `bimbam-5.9.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 5.9
+Version: 5.9.9
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-5.9/bimbam.egg-info/PKG-INFO` & `bimbam-5.9.9/bimbam.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 5.9
+Version: 5.9.9
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-5.9/bimbam.egg-info/SOURCES.txt` & `bimbam-5.9.9/bimbam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/setup.py` & `bimbam-5.9.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 requirements = []
 for line in open(os.path.join(setupdir, "requirements.txt"), encoding="ASCII"):
     if line.strip() and not line.startswith("#"):
         requirements.append(line)
         
 setup(
     name="bimbam",
-    version="5.9",
+    version="5.9.9",
     author="idtaleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests""",
     url="https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests",
 #    keywords="IDE education programming tests in documentation",
```

### Comparing `bimbam-5.9/thonnycontrib/ThonnyLogsGenerator.py` & `bimbam-5.9.9/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/backend/ast_parser.py` & `bimbam-5.9.9/thonnycontrib/backend/ast_parser.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/backend/doctest_parser.py` & `bimbam-5.9.9/thonnycontrib/backend/doctest_parser.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/backend/evaluator.py` & `bimbam-5.9.9/thonnycontrib/backend/evaluator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/backend/l1test_backend.py` & `bimbam-5.9.9/thonnycontrib/backend/l1test_backend.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/backend/test_finder.py` & `bimbam-5.9.9/thonnycontrib/backend/test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/backend/verdicts/ExampleVerdict.py` & `bimbam-5.9.9/thonnycontrib/backend/verdicts/ExampleVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/backend/verdicts/FailedVerdict.py` & `bimbam-5.9.9/thonnycontrib/backend/verdicts/FailedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py` & `bimbam-5.9.9/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/docs/res/error_icon.png` & `bimbam-5.9.9/thonnycontrib/docs/res/error_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/docs/res/exception_red_chip.png` & `bimbam-5.9.9/thonnycontrib/docs/res/exception_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/docs/res/failed.png` & `bimbam-5.9.9/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/docs/res/failed_red_chip.png` & `bimbam-5.9.9/thonnycontrib/docs/res/failed_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/docs/res/l1test_icon.png` & `bimbam-5.9.9/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/docs/res/l1test_icon_old.png` & `bimbam-5.9.9/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/docs/res/outline_class.png` & `bimbam-5.9.9/thonnycontrib/docs/res/outline_class.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/docs/res/outline_method.gif` & `bimbam-5.9.9/thonnycontrib/docs/res/outline_method.gif`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/docs/res/passed.png` & `bimbam-5.9.9/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/docs/res/pending_icon.png` & `bimbam-5.9.9/thonnycontrib/docs/res/pending_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/docs/res/restart_icon.png` & `bimbam-5.9.9/thonnycontrib/docs/res/restart_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/docs/res/success_green_chip.png` & `bimbam-5.9.9/thonnycontrib/docs/res/success_green_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/docs/res/warning.png` & `bimbam-5.9.9/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/docstring_generator/__init__.py` & `bimbam-5.9.9/thonnycontrib/docstring_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/docstring_generator/doc_generator.py` & `bimbam-5.9.9/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/docstring_generator/doc_template.py` & `bimbam-5.9.9/thonnycontrib/docstring_generator/doc_template.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/environement_vars.py` & `bimbam-5.9.9/thonnycontrib/environement_vars.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/exceptions.py` & `bimbam-5.9.9/thonnycontrib/exceptions.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/i18n/languages.py` & `bimbam-5.9.9/thonnycontrib/i18n/languages.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/i18n/locale/en_US/LC_MESSAGES/l1test.po` & `bimbam-5.9.9/thonnycontrib/i18n/locale/en_US/LC_MESSAGES/l1test.po`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/i18n/locale/fr_FR/LC_MESSAGES/l1test.mo` & `bimbam-5.9.9/thonnycontrib/i18n/locale/fr_FR/LC_MESSAGES/l1test.mo`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/i18n/locale/fr_FR/LC_MESSAGES/l1test.po` & `bimbam-5.9.9/thonnycontrib/i18n/locale/fr_FR/LC_MESSAGES/l1test.po`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/i18n/locale/l1test.pot` & `bimbam-5.9.9/thonnycontrib/i18n/locale/l1test.pot`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/l1test_configuration/l1test_options.py` & `bimbam-5.9.9/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/l1test_frontend/__init__.py` & `bimbam-5.9.9/thonnycontrib/l1test_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/l1test_frontend/l1test_error_view.py` & `bimbam-5.9.9/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/l1test_frontend/l1test_outliner_menu.py` & `bimbam-5.9.9/thonnycontrib/l1test_frontend/l1test_outliner_menu.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/l1test_frontend/l1test_reporter.py` & `bimbam-5.9.9/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/l1test_frontend/l1test_runner.py` & `bimbam-5.9.9/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/l1test_frontend/l1test_treeview.py` & `bimbam-5.9.9/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,15 @@
         status_groups = ordered_groups
         
         return status_groups
     
     def group_by_verdicts(self):  
         grouped = self.__group_by_verdicts(self._origin_l1doctests)
         if not self.is_empty(): # on met à jour que si la treeview possède des éléments
-            self.clear_tree(clear_all=False) 
+            self.clear_tree(clear_all=False, disable_menu=False) 
             for status, l1doctests in grouped.items():
                 row_id = self.treeview.insert(parent='', index="end", text=status.short_name(), open=status.is_failing(), 
                                          tags=(status.get_color(),))
                 self.__add_verdicts_to_treeview(l1doctests, row_id)
         
     def expand_rows(self, event=None): 
         """ Spreads the function rows and the red tests. """
@@ -699,15 +699,15 @@
         success = sum([l1doctest.count_passed_tests() for l1doctest in l1doctests])
         failures = sum([l1doctest.count_failed_tests() for l1doctest in l1doctests])
         errors = sum([l1doctest.count_error_tests() for l1doctest in l1doctests])
         empty = sum([1 for l1doctest in l1doctests if l1doctest.get_flag() == L1DocTestFlag.EMPTY_FLAG])
         total = success + failures + errors
         return Summarize(total, success, failures, errors, empty)
                    
-    def clear_tree(self, clear_verdicts_data=False, clear_all=True, clear_errorview=False):
+    def clear_tree(self, clear_verdicts_data=False, clear_all=True, clear_errorview=False, disable_menu=True):
         """Clears the treeview by deleting all items. This method is called by
         the `update_tree_contents` method to clear the treeview before inserting
         the new rows.
         
         Note: this method is also called when the button `clear` is clicked. In 
         this case, the `event` is not None, then the original/copy lists of l1doctests
         will be cleared. Finally, the treeview or/and header or/and the errorview 
@@ -728,15 +728,16 @@
         if clear_all:
             self.clear_header_bar()  # on supprime le contenu du header
         if clear_errorview:
             error_view:L1TestErrorView = self.workbench.get_view(L1TestErrorView.__name__)
             error_view.clear()
         self.treeview.delete(*self.treeview.get_children())
         self.__init_special_attributes()
-        self.disable_menu()
+        if disable_menu:
+            self.disable_menu()
         
     def clear_header_bar(self):
         """Clears the header of the treeview."""
         if self.header_bar:
             self.header_bar.direct_delete("1.0", "end")
             self.resize_header_bar()
```

### Comparing `bimbam-5.9/thonnycontrib/main_generator/main_generator.py` & `bimbam-5.9.9/thonnycontrib/main_generator/main_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/plugin_loader.py` & `bimbam-5.9.9/thonnycontrib/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/properties.py` & `bimbam-5.9.9/thonnycontrib/properties.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/tests/fixtures/workbench_mock.py` & `bimbam-5.9.9/thonnycontrib/tests/fixtures/workbench_mock.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/tests/tests_doc_generator.py` & `bimbam-5.9.9/thonnycontrib/tests/tests_doc_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/tests/tests_example_no_expected.py` & `bimbam-5.9.9/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/tests/tests_example_with_exception.py` & `bimbam-5.9.9/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/tests/tests_example_with_expected.py` & `bimbam-5.9.9/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/tests/tests_l1TestRunner.py` & `bimbam-5.9.9/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/tests/tests_main_generator.py` & `bimbam-5.9.9/thonnycontrib/tests/tests_main_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/tests/tests_test_finder.py` & `bimbam-5.9.9/thonnycontrib/tests/tests_test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/tests/tests_view.py` & `bimbam-5.9.9/thonnycontrib/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-5.9/thonnycontrib/utils.py` & `bimbam-5.9.9/thonnycontrib/utils.py`

 * *Files identical despite different names*

