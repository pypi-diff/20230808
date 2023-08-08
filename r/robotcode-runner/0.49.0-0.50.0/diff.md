# Comparing `tmp/robotcode_runner-0.49.0.tar.gz` & `tmp/robotcode_runner-0.50.0.tar.gz`

## Comparing `robotcode_runner-0.49.0.tar` & `robotcode_runner-0.50.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/__version__.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/py.typed
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/cli/__init__.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/cli/libdoc.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/cli/rebot.py
--rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/cli/robot.py
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/cli/testdoc.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/cli/discover/__init__.py
--rw-r--r--   0        0        0    25481 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/src/robotcode/runner/cli/discover/discover.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/README.md
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/pyproject.toml
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.49.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.50.0/src/robotcode/runner/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.50.0/src/robotcode/runner/__version__.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.50.0/src/robotcode/runner/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.50.0/src/robotcode/runner/py.typed
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.50.0/src/robotcode/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 robotcode_runner-0.50.0/src/robotcode/runner/cli/libdoc.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 robotcode_runner-0.50.0/src/robotcode/runner/cli/rebot.py
+-rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 robotcode_runner-0.50.0/src/robotcode/runner/cli/robot.py
+-rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 robotcode_runner-0.50.0/src/robotcode/runner/cli/testdoc.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.50.0/src/robotcode/runner/cli/discover/__init__.py
+-rw-r--r--   0        0        0    25982 2020-02-02 00:00:00.000000 robotcode_runner-0.50.0/src/robotcode/runner/cli/discover/discover.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.50.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.50.0/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.50.0/README.md
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.50.0/pyproject.toml
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.50.0/PKG-INFO
```

### Comparing `robotcode_runner-0.49.0/src/robotcode/runner/cli/libdoc.py` & `robotcode_runner-0.50.0/src/robotcode/runner/cli/libdoc.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     robot_arguments = None
     try:
         _, robot_arguments = LibDoc().parse_arguments(robot_options_and_args)
     except (DataError, Information):
         pass
 
     config_files, root_folder, _ = get_config_files(
-        robot_arguments, app.config.config_files, raise_on_error=False, verbose_callback=app.verbose
+        robot_arguments, app.config.config_files, verbose_callback=app.verbose
     )
     try:
         profile = (
             load_config_from_path(*config_files)
             .combine_profiles(*(app.config.profiles or []), verbose_callback=app.verbose)
             .evaluated()
         )
```

### Comparing `robotcode_runner-0.49.0/src/robotcode/runner/cli/rebot.py` & `robotcode_runner-0.50.0/src/robotcode/runner/cli/rebot.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     robot_arguments = None
     try:
         _, robot_arguments = Rebot().parse_arguments(robot_options_and_args)
     except (DataError, Information):
         pass
 
     config_files, root_folder, _ = get_config_files(
-        robot_arguments, app.config.config_files, raise_on_error=False, verbose_callback=app.verbose
+        robot_arguments, app.config.config_files, verbose_callback=app.verbose
     )
 
     try:
         profile = (
             load_config_from_path(*config_files)
             .combine_profiles(*(app.config.profiles or []), verbose_callback=app.verbose)
             .evaluated()
```

### Comparing `robotcode_runner-0.49.0/src/robotcode/runner/cli/robot.py` & `robotcode_runner-0.50.0/src/robotcode/runner/cli/robot.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         _, robot_arguments = RobotFramework().parse_arguments(robot_options_and_args)
     except (DataError, Information):
         pass
     finally:
         sys.path = old_sys_path
 
     config_files, root_folder, _ = get_config_files(
-        robot_arguments, app.config.config_files, raise_on_error=False, verbose_callback=app.verbose
+        robot_arguments, app.config.config_files, verbose_callback=app.verbose
     )
     try:
         profile = (
             load_config_from_path(*config_files)
             .combine_profiles(*(app.config.profiles or []), verbose_callback=app.verbose)
             .evaluated()
         )
```

### Comparing `robotcode_runner-0.49.0/src/robotcode/runner/cli/testdoc.py` & `robotcode_runner-0.50.0/src/robotcode/runner/cli/testdoc.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     robot_arguments = None
     try:
         _, robot_arguments = TestDoc().parse_arguments(robot_options_and_args)
     except (DataError, Information):
         pass
 
     config_files, root_folder, _ = get_config_files(
-        robot_arguments, app.config.config_files, raise_on_error=False, verbose_callback=app.verbose
+        robot_arguments, app.config.config_files, verbose_callback=app.verbose
     )
 
     try:
         profile = (
             load_config_from_path(*config_files)
             .combine_profiles(*(app.config.profiles or []), verbose_callback=app.verbose)
             .evaluated()
```

### Comparing `robotcode_runner-0.49.0/src/robotcode/runner/cli/discover/discover.py` & `robotcode_runner-0.50.0/src/robotcode/runner/cli/discover/discover.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from robot.conf import RobotSettings
 from robot.errors import DATA_ERROR, INFO_PRINTED, DataError, Information
 from robot.model import ModelModifier, TestCase, TestSuite
 from robot.model.visitor import SuiteVisitor
 from robot.output import LOGGER, Message
 from robot.running.builder import TestSuiteBuilder
 from robot.running.builder.builders import SuiteStructureParser
-from robot.utils import NormalizedDict
+from robot.utils import NormalizedDict, normalize
 from robot.utils.filereader import FileReader
 from robotcode.core.dataclasses import from_json
 from robotcode.core.lsp.types import (
     Diagnostic,
     DiagnosticSeverity,
     DocumentUri,
     Position,
@@ -230,14 +230,15 @@
             uri=str(Uri.from_path(Path.cwd())),
             needs_parse_include=get_robot_version() >= (6, 1),
         )
         self._current = self.all
         self.suites: List[TestItem] = []
         self.tests: List[TestItem] = []
         self.tags: Dict[str, List[TestItem]] = defaultdict(list)
+        self.normalized_tags: Dict[str, List[TestItem]] = defaultdict(list)
         self.statistics = Statistics()
         self._collected = [NormalizedDict(ignore="_")]
 
     def visit_suite(self, suite: TestSuite) -> None:
         if suite.name in self._collected[-1] and suite.parent.source:
             LOGGER.warn(
                 (
@@ -317,14 +318,15 @@
                 tags=list(test.tags) if test.tags else None,
             )
         except ValueError as e:
             raise ValueError(f"Error while parsing suite {test.source}: {e}") from e
 
         for tag in test.tags:
             self.tags[str(tag)].append(item)
+            self.normalized_tags[normalize(str(tag), ignore="_")].append(item)
 
         self.tests.append(item)
         self._current.children.append(item)
 
         self.statistics.tests += 1
 
 
@@ -658,18 +660,25 @@
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
     epilog='Use "-- --help" to see `robot` help.',
 )
+@click.option(
+    "--normalized / --not-normalized",
+    "normalized",
+    default=True,
+    help="Whether or not normalized tags are shown.",
+)
 @add_options(*ROBOT_OPTIONS)
 @pass_application
 def tags(
     app: Application,
+    normalized: bool,
     by_longname: Tuple[str, ...],
     exclude_by_longname: Tuple[str, ...],
     robot_options_and_args: Tuple[str, ...],
 ) -> None:
     """\
     Discover tags with the selected configuration, profiles, options and
     arguments.
@@ -688,20 +697,22 @@
 
     if collector.all.children:
         if app.config.output_format is None or app.config.output_format == OutputFormat.TEXT:
 
             def print(tags: Dict[str, List[TestItem]]) -> Iterable[str]:
                 for tag, items in tags.items():
                     yield f"{tag}{os.linesep}"
+                    # for t in items:
+                    #     yield f"    {t.longname}{os.linesep}"
 
-            if collector.suites:
-                app.echo_via_pager(print(collector.tags))
+            if collector.normalized_tags:
+                app.echo_via_pager(print(collector.normalized_tags if normalized else collector.tags))
 
         else:
-            app.print_data(TagsResult(collector.tags), remove_defaults=True)
+            app.print_data(TagsResult(collector.normalized_tags), remove_defaults=True)
 
 
 @dataclass
 class Info:
     robot_version_string: str
     robot_env: Dict[str, str]
     robotcode_version_string: str
```

### Comparing `robotcode_runner-0.49.0/.gitignore` & `robotcode_runner-0.50.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.49.0/LICENSE.txt` & `robotcode_runner-0.50.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.49.0/README.md` & `robotcode_runner-0.50.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.49.0/pyproject.toml` & `robotcode_runner-0.50.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -24,17 +24,17 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-robot==0.49.0",
-  "robotcode-modifiers==0.49.0",
-  "robotcode==0.49.0",
+  "robotcode-robot==0.50.0",
+  "robotcode-modifiers==0.50.0",
+  "robotcode==0.50.0",
 ]
 
 [project.entry-points.robotcode]
 runner = "robotcode.runner.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_runner-0.49.0/PKG-INFO` & `robotcode_runner-0.50.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-runner
-Version: 0.49.0
+Version: 0.50.0
 Summary: RobotCode runner plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-modifiers==0.49.0
-Requires-Dist: robotcode-robot==0.49.0
-Requires-Dist: robotcode==0.49.0
+Requires-Dist: robotcode-modifiers==0.50.0
+Requires-Dist: robotcode-robot==0.50.0
+Requires-Dist: robotcode==0.50.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
```

