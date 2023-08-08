# Comparing `tmp/vedro-gitlab-reporter-2.1.0.tar.gz` & `tmp/vedro-gitlab-reporter-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-gitlab-reporter-2.1.0.tar", last modified: Sat Jun 24 08:57:32 2023, max compression
+gzip compressed data, was "vedro-gitlab-reporter-2.1.1.tar", last modified: Tue Aug  8 09:04:16 2023, max compression
```

## Comparing `vedro-gitlab-reporter-2.1.0.tar` & `vedro-gitlab-reporter-2.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:57:32.671075 vedro-gitlab-reporter-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-24 08:57:32.671075 vedro-gitlab-reporter-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-24 08:57:32.671075 vedro-gitlab-reporter-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:57:32.667075 vedro-gitlab-reporter-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/tests/test_collapsable_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/tests/test_gitlab_collapsable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/tests/test_gitlab_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:57:32.671075 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter/_collapsable_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter/_gitlab_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 08:57:22.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:57:32.671075 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-24 08:57:32.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-24 08:57:32.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 08:57:32.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-24 08:57:32.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-24 08:57:32.000000 vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:04:16.230983 vedro-gitlab-reporter-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 09:04:06.000000 vedro-gitlab-reporter-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-08-08 09:04:16.230983 vedro-gitlab-reporter-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-08-08 09:04:06.000000 vedro-gitlab-reporter-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-08 09:04:16.230983 vedro-gitlab-reporter-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-08 09:04:06.000000 vedro-gitlab-reporter-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:04:16.230983 vedro-gitlab-reporter-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-08 09:04:06.000000 vedro-gitlab-reporter-2.1.1/tests/test_collapsable_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-08-08 09:04:06.000000 vedro-gitlab-reporter-2.1.1/tests/test_gitlab_collapsable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-08-08 09:04:06.000000 vedro-gitlab-reporter-2.1.1/tests/test_gitlab_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:04:16.230983 vedro-gitlab-reporter-2.1.1/vedro_gitlab_reporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-08 09:04:06.000000 vedro-gitlab-reporter-2.1.1/vedro_gitlab_reporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-08 09:04:06.000000 vedro-gitlab-reporter-2.1.1/vedro_gitlab_reporter/_collapsable_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-08-08 09:04:06.000000 vedro-gitlab-reporter-2.1.1/vedro_gitlab_reporter/_gitlab_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 09:04:06.000000 vedro-gitlab-reporter-2.1.1/vedro_gitlab_reporter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:04:16.230983 vedro-gitlab-reporter-2.1.1/vedro_gitlab_reporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-08-08 09:04:16.000000 vedro-gitlab-reporter-2.1.1/vedro_gitlab_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-08 09:04:16.000000 vedro-gitlab-reporter-2.1.1/vedro_gitlab_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 09:04:16.000000 vedro-gitlab-reporter-2.1.1/vedro_gitlab_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 09:04:16.000000 vedro-gitlab-reporter-2.1.1/vedro_gitlab_reporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 09:04:16.000000 vedro-gitlab-reporter-2.1.1/vedro_gitlab_reporter.egg-info/top_level.txt
```

### Comparing `vedro-gitlab-reporter-2.1.0/LICENSE` & `vedro-gitlab-reporter-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-gitlab-reporter-2.1.0/PKG-INFO` & `vedro-gitlab-reporter-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: vedro-gitlab-reporter
-Version: 2.1.0
+Version: 2.1.1
 Summary: GitLab reporter with collapsable sections for Vedro framework
 Home-page: https://github.com/vedro-universe/vedro-gitlab-reporter
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
+Project-URL: Docs, https://vedro.io/docs/integrations/gitlab-reporter
+Project-URL: GitHub, https://github.com/vedro-universe/vedro-gitlab-reporter
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
```

### Comparing `vedro-gitlab-reporter-2.1.0/README.md` & `vedro-gitlab-reporter-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vedro-gitlab-reporter-2.1.0/setup.cfg` & `vedro-gitlab-reporter-2.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.1.0
+current_version = 2.1.1
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-gitlab-reporter-2.1.0/setup.py` & `vedro-gitlab-reporter-2.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,22 +9,26 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-gitlab-reporter",
-    version="2.1.0",
+    version="2.1.1",
     description="GitLab reporter with collapsable sections for Vedro framework",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.7",
     url="https://github.com/vedro-universe/vedro-gitlab-reporter",
+    project_urls={
+        "Docs": "https://vedro.io/docs/integrations/gitlab-reporter",
+        "GitHub": "https://github.com/vedro-universe/vedro-gitlab-reporter",
+    },
     license="Apache-2.0",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"vedro_gitlab_reporter": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `vedro-gitlab-reporter-2.1.0/tests/test_gitlab_collapsable.py` & `vedro-gitlab-reporter-2.1.1/tests/test_gitlab_collapsable.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         await dispatcher.fire(StepFailedEvent(step_result))
         scenario_result.add_step_result(step_result)
 
         aggregated_result = make_aggregated_result(scenario_result.mark_failed())
         event = ScenarioReportedEvent(aggregated_result)
 
         printer_.reset_mock()
-        printer_.pretty_format = lambda self: "'val'"
 
     with when, patch_uuid() as uuid:
         await dispatcher.fire(event)
 
     with then:
         section_start, section_end = int(step_result.started_at), int(step_result.ended_at)
         assert printer_.mock_calls == [
@@ -53,15 +52,15 @@
             call.console.file.write(
                 f"\x1b[0Ksection_start:{section_start}:{uuid}[collapsed=true]\r\x1b[0K"),
             call.print_step_name(step_result.step_name,
                                  StepStatus.FAILED,
                                  elapsed=step_result.elapsed,
                                  prefix=" " * 3),
             call.print_scope_key("key", indent=5, line_break=True),
-            call.print_scope_val("'val'"),
+            call.print_scope_val("val"),
             call.console.file.write(f"\x1b[0Ksection_end:{section_end}:{uuid}\r\x1b[0K"),
         ]
 
 
 @pytest.mark.usefixtures(gitlab_reporter.__name__)
 async def test_collapsable_vars(*, dispatcher: Dispatcher, printer_: Mock):
     with given:
@@ -73,15 +72,14 @@
         await dispatcher.fire(StepFailedEvent(step_result))
         scenario_result.add_step_result(step_result)
 
         aggregated_result = make_aggregated_result(scenario_result.mark_failed())
         event = ScenarioReportedEvent(aggregated_result)
 
         printer_.reset_mock()
-        printer_.pretty_format = lambda self: "'val'"
 
     with when, patch_uuid() as uuid:
         await dispatcher.fire(event)
 
     with then:
         assert printer_.mock_calls == [
             call.print_scenario_subject(aggregated_result.scenario.subject,
@@ -92,15 +90,15 @@
             call.print_step_name(step_result.step_name,
                                  StepStatus.FAILED,
                                  elapsed=step_result.elapsed,
                                  prefix=" " * 3),
 
             call.console.file.write(f"\x1b[0Ksection_start:0:{uuid}[collapsed=true]\r\x1b[0K"),
             call.print_scope_key("key", indent=5, line_break=True),
-            call.print_scope_val("'val'"),
+            call.print_scope_val("val"),
             call.console.file.write(f"\x1b[0Ksection_end:0:{uuid}\r\x1b[0K"),
         ]
 
 
 @pytest.mark.usefixtures(gitlab_reporter.__name__)
 async def test_collapsable_scope(*, dispatcher: Dispatcher, printer_: Mock):
     with given:
```

### Comparing `vedro-gitlab-reporter-2.1.0/tests/test_gitlab_reporter.py` & `vedro-gitlab-reporter-2.1.1/tests/test_gitlab_reporter.py`

 * *Files identical despite different names*

### Comparing `vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter/_gitlab_reporter.py` & `vedro-gitlab-reporter-2.1.1/vedro_gitlab_reporter/_gitlab_reporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import operator
 import uuid
 from functools import reduce
-from typing import Callable, Dict, List, Set, Type, Union
+from typing import Any, Callable, Dict, List, Set, Type, Union
 
+import vedro
 from vedro.core import Dispatcher, PluginConfig, ScenarioResult
 from vedro.events import (
     ArgParsedEvent,
     ArgParseEvent,
     CleanupEvent,
     ScenarioReportedEvent,
     ScenarioRunEvent,
@@ -187,15 +188,15 @@
                                           elapsed=step_result.elapsed, prefix=prefix)
 
             scenario_steps = self._scenario_steps[index]
             for key, val in scenario_result.scope.items():
                 if key not in scenario_steps[step_result.step_name]:
                     continue
                 self._printer.print_scope_key(key, indent=len(prefix) + 2, line_break=True)
-                self._printer.print_scope_val(self._printer.pretty_format(val))
+                self._print_scope_val(val)
 
             ended_at = int(step_result.ended_at) if step_result.ended_at else 0
             self._print_section_end(section_name, ended_at)
 
     def _print_steps_with_collapsable_vars(self, scenario_result: ScenarioResult, *,
                                            index: int = 0, prefix: str = "") -> None:
         for step_result in scenario_result.step_results:
@@ -206,15 +207,15 @@
             for key, val in scenario_result.scope.items():
                 if key not in scenario_steps[step_result.step_name]:
                     continue
                 section_name = str(uuid.uuid4())
                 self._print_section_start(section_name)
 
                 self._printer.print_scope_key(key, indent=len(prefix) + 2, line_break=True)
-                self._printer.print_scope_val(self._printer.pretty_format(val))
+                self._print_scope_val(val)
 
                 self._print_section_end(section_name)
 
     def _print_exceptions(self, scenario_result: ScenarioResult) -> None:
         for step_result in scenario_result.step_results:
             if step_result.exc_info is None:
                 continue
@@ -225,14 +226,21 @@
 
     def _print_collapsable_scope(self, scenario_result: ScenarioResult) -> None:
         section_name = str(uuid.uuid4())
         self._print_section_start(section_name)
         self._printer.print_scope(scenario_result.scope)
         self._print_section_end(section_name)
 
+    def _print_scope_val(self, val: Any) -> None:
+        major, minor, *_ = vedro.__version__.split(".")
+        if (int(major), int(minor)) < (1, 10):
+            self._printer.print_scope_val(self._printer.pretty_format(val))
+        else:
+            self._printer.print_scope_val(val)
+
 
 class GitlabReporter(PluginConfig):
     plugin = GitlabReporterPlugin
 
     # Show internal calls in the traceback output
     tb_show_internal_calls: bool = False
```

### Comparing `vedro-gitlab-reporter-2.1.0/vedro_gitlab_reporter.egg-info/PKG-INFO` & `vedro-gitlab-reporter-2.1.1/vedro_gitlab_reporter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: vedro-gitlab-reporter
-Version: 2.1.0
+Version: 2.1.1
 Summary: GitLab reporter with collapsable sections for Vedro framework
 Home-page: https://github.com/vedro-universe/vedro-gitlab-reporter
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
+Project-URL: Docs, https://vedro.io/docs/integrations/gitlab-reporter
+Project-URL: GitHub, https://github.com/vedro-universe/vedro-gitlab-reporter
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
```

