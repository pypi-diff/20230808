# Comparing `tmp/anfema_django_testutils-0.4.0.tar.gz` & `tmp/anfema_django_testutils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anfema_django_testutils-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "anfema_django_testutils-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `anfema_django_testutils-0.4.0.tar` & `anfema_django_testutils-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1912 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/.github/workflows/publish_release_packages.yaml
--rw-r--r--   0        0        0       41 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/.gitignore
--rw-r--r--   0        0        0     1067 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/LICENSE
--rw-r--r--   0        0        0     1492 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/README.md
--rw-r--r--   0        0        0      336 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/anfema_django_testutils/__init__.py
--rw-r--r--   0        0        0      317 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/anfema_django_testutils/apps.py
--rw-r--r--   0        0        0    16161 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/anfema_django_testutils/runner.py
--rw-r--r--   0        0        0      959 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/anfema_django_testutils/settings.py
--rw-r--r--   0        0        0     2335 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/anfema_django_testutils/static/css/test-results.css
--rw-r--r--   0        0        0     1636 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/anfema_django_testutils/tags.py
--rw-r--r--   0        0        0    10501 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/anfema_django_testutils/templates/test-results-template.html
--rw-r--r--   0        0        0     4977 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/anfema_django_testutils/testcases.py
--rw-r--r--   0        0        0      638 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/docs/Makefile
--rw-r--r--   0        0        0      769 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/docs/make.bat
--rw-r--r--   0        0        0      569 2023-06-14 09:31:27.932429 anfema_django_testutils-0.4.0/docs/source/api.rst
--rw-r--r--   0        0        0     1791 2023-06-14 09:31:27.936429 anfema_django_testutils-0.4.0/docs/source/conf.py
--rw-r--r--   0        0        0     2829 2023-06-14 09:31:27.936429 anfema_django_testutils-0.4.0/docs/source/configuration.rst
--rw-r--r--   0        0        0       93 2023-06-14 09:31:27.936429 anfema_django_testutils-0.4.0/docs/source/index.rst
--rw-r--r--   0        0        0       46 2023-06-14 09:31:27.936429 anfema_django_testutils-0.4.0/docs/source/license.rst
--rw-r--r--   0        0        0     1259 2023-06-14 09:31:27.936429 anfema_django_testutils-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       38 2023-06-14 09:31:27.936429 anfema_django_testutils-0.4.0/setup.py
--rw-r--r--   0        0        0      189 2023-06-14 09:31:27.936429 anfema_django_testutils-0.4.0/tox.ini
--rw-r--r--   0        0        0     2447 1970-01-01 00:00:00.000000 anfema_django_testutils-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1912 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/.github/workflows/publish_release_packages.yaml
+-rw-r--r--   0        0        0       41 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1067 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1492 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/README.md
+-rw-r--r--   0        0        0      336 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/anfema_django_testutils/__init__.py
+-rw-r--r--   0        0        0      317 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/anfema_django_testutils/apps.py
+-rw-r--r--   0        0        0    18610 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/anfema_django_testutils/runner.py
+-rw-r--r--   0        0        0      959 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/anfema_django_testutils/settings.py
+-rw-r--r--   0        0        0     2335 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/anfema_django_testutils/static/css/test-results.css
+-rw-r--r--   0        0        0     1636 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/anfema_django_testutils/tags.py
+-rw-r--r--   0        0        0    10501 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/anfema_django_testutils/templates/test-results-template.html
+-rw-r--r--   0        0        0     6932 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/anfema_django_testutils/testcases.py
+-rw-r--r--   0        0        0      638 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/docs/Makefile
+-rw-r--r--   0        0        0      769 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/docs/make.bat
+-rw-r--r--   0        0        0      577 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/docs/source/api.rst
+-rw-r--r--   0        0        0     1791 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/docs/source/conf.py
+-rw-r--r--   0        0        0     2829 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/docs/source/configuration.rst
+-rw-r--r--   0        0        0       93 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/docs/source/index.rst
+-rw-r--r--   0        0        0       46 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/docs/source/license.rst
+-rw-r--r--   0        0        0     1259 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/setup.py
+-rw-r--r--   0        0        0      189 2023-08-08 13:45:10.559587 anfema_django_testutils-0.5.0/tox.ini
+-rw-r--r--   0        0        0     2447 1970-01-01 00:00:00.000000 anfema_django_testutils-0.5.0/PKG-INFO
```

### Comparing `anfema_django_testutils-0.4.0/.github/workflows/publish_release_packages.yaml` & `anfema_django_testutils-0.5.0/.github/workflows/publish_release_packages.yaml`

 * *Files identical despite different names*

### Comparing `anfema_django_testutils-0.4.0/LICENSE` & `anfema_django_testutils-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anfema_django_testutils-0.4.0/README.md` & `anfema_django_testutils-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `anfema_django_testutils-0.4.0/anfema_django_testutils/runner.py` & `anfema_django_testutils-0.5.0/anfema_django_testutils/runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """This module provides a TestRunner."""
 from __future__ import annotations
 
 
 __all__ = ('TestRunner',)
 
-
 import argparse
 import contextlib
 import datetime
 import itertools
+import os
 import pathlib
 import re
 import sys
 import textwrap
 import unittest.runner
 from collections import defaultdict, namedtuple
 from contextlib import nullcontext
@@ -20,17 +20,19 @@
 from typing import TYPE_CHECKING
 from unittest.result import TestResult
 from unittest.runner import TextTestRunner
 from unittest.suite import _ErrorHolder
 from unittest.util import strclass
 
 from django.contrib.staticfiles import finders
+from django.core.management import color
+from django.core.management.base import OutputWrapper
 from django.template.loader import render_to_string
 from django.test.runner import DiscoverRunner
-from django.utils import timezone
+from django.utils import termcolors, timezone
 
 from coverage import Coverage
 from snapshottest.django import TestRunnerMixin as SnapshotTestRunnerMixin
 
 from .settings import get_config
 
 
@@ -53,26 +55,29 @@
 
     :param str report_dir: Path to where the coverage report shall be stored.
     """
 
     def __init__(self, report_dir: str) -> None:
         super().__init__()
         self._report_dir = f"{report_dir}/coverage"
+        self.stdout = OutputWrapper(sys.stdout)
+        self.stderr = OutputWrapper(sys.stderr)
+        self.style = color.no_style()
+        self.stderr.style_func = self.style.ERROR
 
     def __enter__(self) -> CoverageContext:
         self.erase()
         self.start()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         self.stop()
         self.save()
         self.html_report(directory=self._report_dir)
-        # ToDo: use stream instead of print
-        print(f'Generated coverage report: "{pathlib.Path(self._report_dir, "index.html").absolute()}"')
+        self.stdout.write(f'Generated coverage report: "{pathlib.Path(self._report_dir, "index.html").absolute()}"')
 
 
 class CodeCoverageTestRunnerMixin:
     """A TestRunner mixin class which takes code coverage into account."""
 
     def __init__(self, **kwargs) -> None:
         code_coverage_disabled = not kwargs["code_coverage_enabled"]
@@ -96,26 +101,59 @@
         'unexpected_success',
         'precondition_failure',
     )
 
     TestResultData = namedtuple('TestResultData', field_names=('name', 'result', 'duration', 'outcome'))
     _subtest_result_map: defaultdict[unittest.case.TestCase, list[tuple[_SubTest, str, _SysExcInfoType]]]
 
+    @classmethod
+    def create_color_style(cls) -> color.Style:
+        """Create and return a custom color style based on the available options.
+
+        This method creates a custom color style for console output based on the available options.
+        If the `no-color` option is set or the console does not support color, the style will be configured
+        to have no color for each supported result. Otherwise, individual styles will be created for each
+        supported result, such as 'RESULT_ERROR', 'RESULT_FAILURE', 'RESULT_SKIPPED', etc., with specific
+        color and text formatting.
+
+        :returns: A custom color style object for console output.
+        """
+        style = color.color_style()
+
+        if cls.options.get("no_color") or not color.supports_color():
+            for result in cls.supported_results:
+                setattr(style, f"RESULT_{result.upper()}", termcolors.make_style(""))
+        else:
+            style.RESULT_ERROR = termcolors.make_style(fg='red', opts=('bold',))
+            style.RESULT_FAILURE = termcolors.make_style(fg='yellow', opts=('bold',))
+            style.RESULT_SKIPPED = termcolors.make_style(fg='white', opts=('bold',))
+            style.RESULT_PASSED = termcolors.make_style(fg='green', opts=('bold',))
+            style.RESULT_EXPECTED_FAILURE = termcolors.make_style(fg='magenta', opts=('bold',))
+            style.RESULT_UNEXPECTED_SUCCESS = termcolors.make_style(fg='yellow', opts=('bold',))
+            style.RESULT_PRECONDITION_FAILURE = termcolors.make_style(fg='yellow', opts=('bold',))
+
+        return style
+
     def __init__(self, *args, tests=None, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.dots = False
         self.showAll = False
         self.passed = []
         self.precondition_failures = []
         self.timestamp_start_testrun = None
         self.timestamp_stop_testrun = None
         self._test_result_data = defaultdict(list)
         self._subtest_result_map = defaultdict(list)
         self._all_tests = tests
 
+        self.stdout = OutputWrapper(sys.stdout)
+        self.stderr = OutputWrapper(sys.stderr)
+        self.style = self.create_color_style()
+        self.stderr.style_func = self.style.ERROR
+
     def _add_test_result_data(self, test, result, outcome=None) -> None:
         if isinstance(test, _ErrorHolder):
             # In case an _ErrorHolder instance has been passed, which means setting up the testcase has been failed,
             # none of the testcase`s test methods have been executed, and thus they will all be set to the same result.
             parent = re.search('\((.+)\)', test.description).group(1)
             module, testcase_name = parent.rsplit('.', 1)
             testcase_class = getattr(sys.modules[module], testcase_name)
@@ -146,16 +184,15 @@
 
             # Copy css file into the report directory
             with contextlib.suppress(TypeError):
                 css_file = pathlib.Path(get_config()['TEST_REPORT_CSS'] or None)
                 if not css_file.is_absolute():
                     css_file = pathlib.Path(finders.find(pathlib.Path('css', css_file)))
                 results_html_file.with_name(css_file.name).write_text(css_file.read_text())
-            # ToDo: use stream instead of print
-            print(f'Generated test report: "{results_html_file.absolute()}"')
+            self.stdout.write(f'Generated test report: "{results_html_file.absolute()}"')
 
     def make_result_data(self) -> Dict[str, Any]:
         test_suite_exec_summary = dict()
         test_suite_exec_summary['testcases'] = {}
         test_suite_exec_summary.setdefault(
             'summary',
             dict(  # noqa: C406
@@ -194,16 +231,15 @@
 
         return test_suite_exec_summary
 
     def startTestRun(self) -> None:
         """Called once before any tests are executed."""
         self.timestamp_start_testrun = timezone.now()
         self.timestamp_stop_testrun = None
-        # ToDo: use stream instead of print
-        print()
+        self.stdout.write()
 
     def startTest(self, test: unittest.case.TestCase) -> None:
         """Called when the given test is about to be run"""
         test.timestamp = test.start_time = timezone.now()
         super().startTest(test)
 
     def stopTestRun(self) -> None:
@@ -269,33 +305,41 @@
                 self.stop()
 
     def wasSuccessful(self) -> bool:
         """Tells whether or not this result was a success."""
         return len(self.precondition_failures) == 0 and super().wasSuccessful()
 
     def print_test_result(self, test: unittest.case.TestCase, result: str) -> None:
-        result_width = max(map(len, self.supported_results)) + 10
-        # ToDo: use stream instead of print
-        print(f"{result.upper().replace('_', ' '):.<{result_width}} {test}")
+        max_result_width = max(map(len, self.supported_results)) + 10
+        cur_result_width = len(result)
+        style = getattr(self.style, f"RESULT_{result.upper()}")
+
+        self.stdout.write(style(result.upper()), ending="")
+        self.stdout.write("." * (max_result_width - cur_result_width), ending="")
+        self.stdout.write(" " + str(test))
 
     def printErrors(self) -> None:
         results = list(map(attrgetter('result'), itertools.chain.from_iterable(self._test_result_data.values())))
         skipped = results.count('skipped')
         passed = results.count('passed')
         expected_failures = results.count('expected_failure')
         precondition_failures = results.count('precondition_failure')
         failures = results.count('failure')
         unexpected_successes = results.count('unexpected_success')
         errors = results.count('error')
 
-        print()
-        print(
-            f'{"OK" if self.wasSuccessful() else "FAILED"} (skipped={skipped}, passed={passed}, '
-            f'expected failures={expected_failures}, precondition failures={precondition_failures}, '
-            f'failures={failures}, unexpected successes={unexpected_successes}, errors={errors})'
+        style = self.style.SUCCESS if self.wasSuccessful() else self.style.ERROR
+
+        self.stdout.write()
+        self.stdout.write(
+            style(
+                f'{"OK" if self.wasSuccessful() else "FAILED"} (skipped={skipped}, passed={passed}, '
+                f'expected failures={expected_failures}, precondition failures={precondition_failures}, '
+                f'failures={failures}, unexpected successes={unexpected_successes}, errors={errors})'
+            )
         )
 
     def _resolve_subtests_results(
         self, test: unittest.case.TestCase, results: list[tuple[_SubTest, str, _SysExcInfoType]]
     ) -> tuple[str, str]:
         result_priority_map = {'error': 1, 'failure': 2, 'precondition_failure': 3}
         reverse_result_priority_map = {v: k for k, v in result_priority_map.items()}
@@ -328,14 +372,18 @@
             result = 'error'
         self._subtest_result_map[test].append((subtest, result, err))
 
 
 class HtmlTestRunner(TextTestRunner):
     resultclass = HtmlTestResult
 
+    def __init__(self, *args, **kwargs):
+        kwargs.setdefault('stream', open(os.devnull, 'w'))
+        super().__init__(*args, **kwargs)
+
     def run(self, test: unittest.suite.TestSuite) -> HtmlTestResult:
         # ToDo: Consider to override the run() method to keep 'test'
         self._tests = list(test)
         result = super().run(test)
         result.create_report(result.make_result_data())
         return result
```

### Comparing `anfema_django_testutils-0.4.0/anfema_django_testutils/settings.py` & `anfema_django_testutils-0.5.0/anfema_django_testutils/settings.py`

 * *Files identical despite different names*

### Comparing `anfema_django_testutils-0.4.0/anfema_django_testutils/static/css/test-results.css` & `anfema_django_testutils-0.5.0/anfema_django_testutils/static/css/test-results.css`

 * *Files identical despite different names*

### Comparing `anfema_django_testutils-0.4.0/anfema_django_testutils/tags.py` & `anfema_django_testutils-0.5.0/anfema_django_testutils/tags.py`

 * *Files identical despite different names*

### Comparing `anfema_django_testutils-0.4.0/anfema_django_testutils/templates/test-results-template.html` & `anfema_django_testutils-0.5.0/anfema_django_testutils/templates/test-results-template.html`

 * *Files identical despite different names*

### Comparing `anfema_django_testutils-0.4.0/docs/Makefile` & `anfema_django_testutils-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `anfema_django_testutils-0.4.0/docs/make.bat` & `anfema_django_testutils-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `anfema_django_testutils-0.4.0/docs/source/api.rst` & `anfema_django_testutils-0.5.0/docs/source/api.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 API
 ===
 
 anfema_django_testutils.testcases
 ---------------------------------
 
 .. automodule:: anfema_django_testutils.testcases
-   :members: PreconditionError, PreconditionContext, precondition
+   :members: PreconditionError, PreconditionContext, precondition, repeat
 
 .. autoclass:: anfema_django_testutils.testcases.SimpleTestCase
    :members:
    :inherited-members:
 
 .. autoclass:: anfema_django_testutils.testcases.TransactionTestCase
    :members:
```

### Comparing `anfema_django_testutils-0.4.0/docs/source/conf.py` & `anfema_django_testutils-0.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `anfema_django_testutils-0.4.0/docs/source/configuration.rst` & `anfema_django_testutils-0.5.0/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `anfema_django_testutils-0.4.0/pyproject.toml` & `anfema_django_testutils-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anfema_django_testutils-0.4.0/PKG-INFO` & `anfema_django_testutils-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anfema-django-testutils
-Version: 0.4.0
+Version: 0.5.0
 Summary: Testrunner for django which covers html report and code coverage
 Keywords: django,tests,coverage,testrunner
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

