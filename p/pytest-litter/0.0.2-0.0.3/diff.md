# Comparing `tmp/pytest-litter-0.0.2.tar.gz` & `tmp/pytest-litter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-litter-0.0.2.tar", last modified: Fri Aug  4 17:22:17 2023, max compression
+gzip compressed data, was "pytest-litter-0.0.3.tar", last modified: Tue Aug  8 08:16:04 2023, max compression
```

## Comparing `pytest-litter-0.0.2.tar` & `pytest-litter-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/requirements-lint.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/src/pytest_litter/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/src/pytest_litter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/src/pytest_litter/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/src/pytest_litter/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/src/pytest_litter/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/src/pytest_litter/plugin/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/src/pytest_litter/snapshots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/src/pytest_litter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-08-04 17:22:17.000000 pytest-litter-0.0.2/src/pytest_litter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-04 17:22:17.000000 pytest-litter-0.0.2/src/pytest_litter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 17:22:17.000000 pytest-litter-0.0.2/src/pytest_litter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-04 17:22:17.000000 pytest-litter-0.0.2/src/pytest_litter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 17:22:17.000000 pytest-litter-0.0.2/src/pytest_litter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-04 17:22:17.000000 pytest-litter-0.0.2/src/pytest_litter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/tests/pytester/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/tests/pytester/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/tests/pytester/pytester_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:22:17.952226 pytest-litter-0.0.2/tests/system_test/
--rwxr-xr-x   0 runner    (1001) docker     (123)      596 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/tests/system_test/system_test.sh
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/tests/test_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-04 17:22:09.000000 pytest-litter-0.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:16:04.662665 pytest-litter-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:16:04.658665 pytest-litter-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:16:04.662665 pytest-litter-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-08-08 08:16:04.662665 pytest-litter-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/requirements-lint.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 08:16:04.662665 pytest-litter-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:16:04.658665 pytest-litter-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:16:04.662665 pytest-litter-0.0.3/src/pytest_litter/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/src/pytest_litter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:16:04.662665 pytest-litter-0.0.3/src/pytest_litter/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/src/pytest_litter/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/src/pytest_litter/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/src/pytest_litter/plugin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/src/pytest_litter/snapshots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:16:04.662665 pytest-litter-0.0.3/src/pytest_litter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-08-08 08:16:04.000000 pytest-litter-0.0.3/src/pytest_litter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-08 08:16:04.000000 pytest-litter-0.0.3/src/pytest_litter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 08:16:04.000000 pytest-litter-0.0.3/src/pytest_litter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-08 08:16:04.000000 pytest-litter-0.0.3/src/pytest_litter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 08:16:04.000000 pytest-litter-0.0.3/src/pytest_litter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 08:16:04.000000 pytest-litter-0.0.3/src/pytest_litter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:16:04.662665 pytest-litter-0.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:16:04.662665 pytest-litter-0.0.3/tests/suite/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/tests/suite/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/tests/suite/suite_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:16:04.662665 pytest-litter-0.0.3/tests/system_test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      593 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/tests/system_test/system_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/tests/test_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-08 08:15:54.000000 pytest-litter-0.0.3/tox.ini
```

### Comparing `pytest-litter-0.0.2/.github/workflows/ci.yaml` & `pytest-litter-0.0.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pytest-litter-0.0.2/.github/workflows/publish.yaml` & `pytest-litter-0.0.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `pytest-litter-0.0.2/.gitignore` & `pytest-litter-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-litter-0.0.2/LICENSE` & `pytest-litter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-litter-0.0.2/PKG-INFO` & `pytest-litter-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-litter
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pytest plugin which verifies that tests do not modify file trees.
 Author: Anton Vikström
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pytest-litter-0.0.2/pyproject.toml` & `pytest-litter-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 [tool.setuptools.packages.find]
 where = ["src"]
 namespaces = false
 
 [tool.pytest.ini_options]
 addopts = "--random-order -p no:pytest-litter -p pytester -vv"
 testpaths = ["tests"]
-pytester_example_dir = "tests/pytester"
+pytester_example_dir = "tests/suite"
 
 [tool.coverage.run]
 branch = true
 source_pkgs = ["pytest_litter"]
 
 [tool.coverage.report]
 show_missing = true
```

### Comparing `pytest-litter-0.0.2/src/pytest_litter/plugin/plugin.py` & `pytest-litter-0.0.3/src/pytest_litter/plugin/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,40 +2,48 @@
 
 from typing import Optional
 
 import pytest
 
 from pytest_litter.plugin.utils import (
     COMPARATOR_KEY,
+    SNAPSHOT_FACTORY_KEY,
     SNAPSHOT_KEY,
     raise_test_error_from_comparison,
     run_snapshot_comparison,
 )
 from pytest_litter.snapshots import (
     DirectoryIgnoreSpec,
     IgnoreSpec,
-    RegexIgnoreSpec,
+    LitterConfig,
+    NameIgnoreSpec,
     SnapshotComparator,
-    TreeSnapshot,
+    TreeSnapshotFactory,
 )
 
 
 def pytest_configure(config: pytest.Config) -> None:
     """Configure pytest-litter plugin (pytest hook function)."""
     ignore_specs: list[IgnoreSpec] = []
     basetemp: Optional[str] = config.getoption("basetemp", None)
     if basetemp is not None:
         ignore_specs.append(
             DirectoryIgnoreSpec(
                 directory=config.rootpath / basetemp,
             )
         )
-    ignore_specs.append(RegexIgnoreSpec(regex=r".*/__pycache__.*"))
-    config.stash[SNAPSHOT_KEY] = TreeSnapshot(root=config.rootpath)
-    config.stash[COMPARATOR_KEY] = SnapshotComparator(ignore_specs=ignore_specs)
+    ignore_specs.append(NameIgnoreSpec(name="__pycache__"))
+    ignore_specs.append(NameIgnoreSpec(name="venv"))
+    ignore_specs.append(NameIgnoreSpec(name=".venv"))
+    ignore_specs.append(NameIgnoreSpec(name=".pytest_cache"))
+    litter_config = LitterConfig(ignore_specs=ignore_specs)
+    snapshot_factory = TreeSnapshotFactory(config=litter_config)
+    config.stash[SNAPSHOT_FACTORY_KEY] = snapshot_factory
+    config.stash[SNAPSHOT_KEY] = snapshot_factory.create_snapshot(root=config.rootpath)
+    config.stash[COMPARATOR_KEY] = SnapshotComparator(config=litter_config)
 
 
 @pytest.hookimpl(hookwrapper=True)  # type: ignore[misc]
 def pytest_runtest_call(item: pytest.Item):  # type: ignore[no-untyped-def]
     yield
     run_snapshot_comparison(
         test_name=item.name,
```

### Comparing `pytest-litter-0.0.2/src/pytest_litter/plugin/utils.py` & `pytest-litter-0.0.3/src/pytest_litter/plugin/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from collections.abc import Iterable
 from pathlib import Path
 from typing import Callable
 
 import pytest
 
-from pytest_litter.snapshots import SnapshotComparator, SnapshotComparison, TreeSnapshot
+from pytest_litter.snapshots import (
+    SnapshotComparator,
+    SnapshotComparison,
+    TreeSnapshot,
+    TreeSnapshotFactory,
+)
 
+SNAPSHOT_FACTORY_KEY = pytest.StashKey[TreeSnapshotFactory]()
 SNAPSHOT_KEY = pytest.StashKey[TreeSnapshot]()
 COMPARATOR_KEY = pytest.StashKey[SnapshotComparator]()
 
 
 class ProblematicTestLitterError(Exception):
     """Raised when a test causes littering, i.e., modifies file tree."""
 
@@ -46,15 +52,18 @@
 def run_snapshot_comparison(
     test_name: str,
     config: pytest.Config,
     mismatch_cb: Callable[[str, SnapshotComparison], None],
 ) -> None:
     """Compare current and old snapshots and call mismatch_cb if there is a mismatch."""
     original_snapshot: TreeSnapshot = config.stash[SNAPSHOT_KEY]
-    new_snapshot: TreeSnapshot = TreeSnapshot(root=original_snapshot.root)
+    snapshot_factory: TreeSnapshotFactory = config.stash[SNAPSHOT_FACTORY_KEY]
+    new_snapshot: TreeSnapshot = snapshot_factory.create_snapshot(
+        root=original_snapshot.root
+    )
     config.stash[SNAPSHOT_KEY] = new_snapshot
 
     comparator: SnapshotComparator = config.stash[COMPARATOR_KEY]
     comparison: SnapshotComparison = comparator.compare(original_snapshot, new_snapshot)
 
     if not comparison.matches:
         mismatch_cb(test_name, comparison)
```

### Comparing `pytest-litter-0.0.2/src/pytest_litter/snapshots.py` & `pytest-litter-0.0.3/src/pytest_litter/snapshots.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,79 @@
 from typing import Any, Optional, Union
 
 
 class UnexpectedLitterError(Exception):
     """Error that should not occur normally, indicative of some programming error."""
 
 
+class IgnoreSpec(abc.ABC):
+    """Specification about paths to ignore in comparisons."""
+
+    __slots__ = ()
+
+    @abc.abstractmethod
+    def matches(self, path: Path) -> bool:
+        ...  # pragma: no cover
+
+
+class DirectoryIgnoreSpec(IgnoreSpec):
+    """Specification to ignore everything in a given directory."""
+
+    __slots__ = ("_directory",)
+
+    def __init__(self, directory: Path) -> None:
+        self._directory = directory
+
+    def matches(self, path: Path) -> bool:
+        return self._directory == path or self._directory in path.parents
+
+
+class NameIgnoreSpec(IgnoreSpec):
+    """Specification to ignore all directories/files with a given name."""
+
+    __slots__ = ("_name",)
+
+    def __init__(self, name: str) -> None:
+        self._name = name
+
+    def matches(self, path: Path) -> bool:
+        return self._name in path.parts
+
+
+class RegexIgnoreSpec(IgnoreSpec):
+    """Regex-based specification about paths to ignore in comparisons."""
+
+    __slots__ = ("_regex",)
+
+    def __init__(self, regex: Union[str, re.Pattern[str]]) -> None:
+        self._regex: re.Pattern[str] = re.compile(regex)
+
+    def matches(self, path: Path) -> bool:
+        return self._regex.fullmatch(str(path)) is not None
+
+
+class LitterConfig:
+    """Configuration for pytest-litter."""
+
+    __slots__ = ("_ignore_specs",)
+
+    def __init__(self, ignore_specs: Optional[Iterable[IgnoreSpec]] = None) -> None:
+        """Initialize.
+
+        Args:
+            ignore_specs: Specifies paths to ignore when doing the comparison.
+
+        """
+        self._ignore_specs: frozenset[IgnoreSpec] = frozenset(ignore_specs or [])
+
+    @property
+    def ignore_specs(self) -> frozenset[IgnoreSpec]:
+        return self._ignore_specs
+
+
 class PathSnapshot:
     """A snapshot of a path."""
 
     __slots__ = ("_path",)
 
     def __init__(self, path: Path) -> None:
         self._path: Path = path
@@ -38,39 +103,78 @@
 
 
 class TreeSnapshot:
     """A snapshot of a directory tree."""
 
     __slots__ = ("_root", "_paths")
 
-    def __init__(self, root: Path) -> None:
+    def __init__(self, root: Path, paths: Iterable[Path]) -> None:
         """Initialize.
 
         Args:
             root: The root directory of the tree.
+            paths: All paths in the snapshot.
 
         """
         if not root.is_dir():
             raise UnexpectedLitterError(f"'{root}' is not a directory.")
         self._root: Path = root
         self._paths: frozenset[PathSnapshot] = frozenset(
-            PathSnapshot(path=path) for path in self._root.rglob("*")
+            PathSnapshot(path=path) for path in paths
         )
 
     @property
     def root(self) -> Path:
         """The root directory of the tree."""
         return self._root
 
     @property
     def paths(self) -> frozenset[PathSnapshot]:
         """The paths in the snapshot."""
         return self._paths
 
 
+class TreeSnapshotFactory:
+    """Factory class for TreeSnapshotFactory."""
+
+    __slots__ = ("_ignore_specs",)
+
+    def __init__(self, config: LitterConfig) -> None:
+        """Initialize.
+
+        Args:
+            config: pytest-litter configuration.
+
+        """
+        self._ignore_specs: frozenset[IgnoreSpec] = frozenset(config.ignore_specs or [])
+
+    def _should_be_ignored(self, path: Path) -> bool:
+        return path.name == "." or any(
+            ignore_spec.matches(path) for ignore_spec in self._ignore_specs
+        )
+
+    def create_snapshot(self, root: Path) -> TreeSnapshot:
+        paths: set[Path] = set()
+
+        def traverse(current: Path) -> None:
+            sub_paths = {
+                p for p in current.glob("*") if not self._should_be_ignored(path=p)
+            }
+            paths.update(sub_paths)
+            for sub_path in sub_paths:
+                traverse(sub_path)
+
+        traverse(root)
+
+        return TreeSnapshot(
+            root=root,
+            paths=paths,
+        )
+
+
 class SnapshotComparison:
     """A comparison of two TreeSnapshots."""
 
     __slots__ = ("_only_a", "_only_b")
 
     def __init__(
         self, only_a: Iterable[PathSnapshot], only_b: Iterable[PathSnapshot]
@@ -97,75 +201,37 @@
 
     @property
     def matches(self) -> bool:
         """If snapshots A and B match each other."""
         return not self._only_a and not self._only_b
 
 
-class IgnoreSpec(abc.ABC):
-    """Specification about paths to ignore in comparisons."""
-
-    __slots__ = ()
-
-    @abc.abstractmethod
-    def matches(self, path: PathSnapshot) -> bool:
-        ...  # pragma: no cover
-
-
-class DirectoryIgnoreSpec(IgnoreSpec):
-    """Specification to ignore everything in a given directory."""
-
-    __slots__ = ("_directory",)
-
-    def __init__(self, directory: Path) -> None:
-        self._directory = directory
-
-    def matches(self, path: PathSnapshot) -> bool:
-        return self._directory == path.path or self._directory in path.path.parents
-
-
-class RegexIgnoreSpec(IgnoreSpec):
-    """Regex-based specification about paths to ignore in comparisons."""
-
-    __slots__ = ("_regex",)
-
-    def __init__(self, regex: Union[str, re.Pattern[str]]) -> None:
-        self._regex: re.Pattern[str] = re.compile(regex)
-
-    def matches(self, path: PathSnapshot) -> bool:
-        return self._regex.fullmatch(str(path)) is not None
-
-
 class SnapshotComparator:
     """Compare TreeSnapshots with each other."""
 
     __slots__ = ("_ignore_specs",)
 
-    def __init__(self, ignore_specs: Optional[Iterable[IgnoreSpec]] = None) -> None:
+    def __init__(self, config: LitterConfig) -> None:
         """Initialize.
 
         Args:
-            ignore_specs: Glob patterns to ignore when doing the comparison.
+            config: pytest-litter configuration.
 
         """
-        self._ignore_specs: frozenset[IgnoreSpec] = frozenset(ignore_specs or [])
-
-    def _should_be_ignored(self, path: PathSnapshot) -> bool:
-        return any(ignore_spec.matches(path) for ignore_spec in self._ignore_specs)
+        self._ignore_specs: frozenset[IgnoreSpec] = frozenset(config.ignore_specs or [])
 
+    @staticmethod
     def compare(
-        self, snapshot_a: TreeSnapshot, snapshot_b: TreeSnapshot
+        snapshot_a: TreeSnapshot, snapshot_b: TreeSnapshot
     ) -> SnapshotComparison:
         """Compare snapshot_a and snapshot_b to produce a SnapshotComparison."""
         if snapshot_a.root != snapshot_b.root:
             raise UnexpectedLitterError(
                 f"Comparing a snapshot of {snapshot_a.root} vs one of {snapshot_b.root}"
             )
         common_paths: frozenset[PathSnapshot] = snapshot_a.paths.intersection(
             snapshot_b.paths
         )
-        only_in_a: frozenset[PathSnapshot] = snapshot_a.paths - common_paths
-        only_in_b: frozenset[PathSnapshot] = snapshot_b.paths - common_paths
         return SnapshotComparison(
-            only_a=(path for path in only_in_a if not self._should_be_ignored(path)),
-            only_b=(path for path in only_in_b if not self._should_be_ignored(path)),
+            only_a=snapshot_a.paths - common_paths,
+            only_b=snapshot_b.paths - common_paths,
         )
```

### Comparing `pytest-litter-0.0.2/src/pytest_litter.egg-info/PKG-INFO` & `pytest-litter-0.0.3/src/pytest_litter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-litter
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pytest plugin which verifies that tests do not modify file trees.
 Author: Anton Vikström
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pytest-litter-0.0.2/src/pytest_litter.egg-info/SOURCES.txt` & `pytest-litter-0.0.3/src/pytest_litter.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 src/pytest_litter.egg-info/requires.txt
 src/pytest_litter.egg-info/top_level.txt
 src/pytest_litter/plugin/__init__.py
 src/pytest_litter/plugin/plugin.py
 src/pytest_litter/plugin/utils.py
 tests/test_plugin.py
 tests/test_snapshots.py
-tests/pytester/pytest.ini
-tests/pytester/pytester_tests.py
+tests/suite/pytest.ini
+tests/suite/suite_tests.py
 tests/system_test/system_test.sh
```

### Comparing `pytest-litter-0.0.2/tests/system_test/system_test.sh` & `pytest-litter-0.0.3/tests/system_test/system_test.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env bash
 
 echo "Preparing system test..."
 WORK_DIR=$(mktemp --directory)
 ROOT_DIR="$(git rev-parse --show-toplevel)"
-TEST_DIR="${ROOT_DIR}/tests/pytester"
+TEST_DIR="${ROOT_DIR}/tests/suite"
 cp "${TEST_DIR}"/* "${WORK_DIR}"
 pushd "${WORK_DIR}" &> /dev/null || exit 1
 VENV="${WORK_DIR}/venv"
 python3 -m venv "${VENV}"
 . "${VENV}/bin/activate"
 "${VENV}/bin/python3" -m pip install --quiet --upgrade pip
 "${VENV}/bin/python3" -m pip install --quiet --editable "${ROOT_DIR}" || exit 1
```

### Comparing `pytest-litter-0.0.2/tests/test_plugin.py` & `pytest-litter-0.0.3/tests/test_plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -90,106 +90,133 @@
         paths_deleted=(path_a,),
     )
 
 
 @pytest.mark.parametrize("matches", [False, True])
 def test_run_snapshot_comparison(
     monkeypatch: "MonkeyPatch",
+    tmp_path: Path,
     matches: bool,
 ) -> None:
     test_name = "test_fake"
-    mock_snapshot_old = Mock(spec=snapshots.TreeSnapshot, root=Path("fake"))
+    mock_factory = Mock(spec=snapshots.TreeSnapshotFactory)
+    mock_snapshot_new = Mock(spec=snapshots.TreeSnapshot)
+    mock_factory.create_snapshot.return_value = mock_snapshot_new
+    mock_snapshot_old = Mock(spec=snapshots.TreeSnapshot, root=tmp_path)
     mock_comparator = Mock(spec=snapshots.SnapshotComparator)
     mock_comparator.compare.return_value = Mock(
         spec=snapshots.SnapshotComparison, matches=matches
     )
     mock_config = Mock(
         spec=pytest.Config,
         stash={
             utils.SNAPSHOT_KEY: mock_snapshot_old,
+            utils.SNAPSHOT_FACTORY_KEY: mock_factory,
             utils.COMPARATOR_KEY: mock_comparator,
         },
     )
-    mock_snapshot_cls = Mock(spec=snapshots.TreeSnapshot)
-    monkeypatch.setattr(
-        "pytest_litter.plugin.utils.TreeSnapshot",
-        mock_snapshot_cls,
-    )
     mock_cb = Mock()
 
     def fake_cb(tc: str, comparison: snapshots.SnapshotComparison) -> None:
         mock_cb(tc, comparison)
 
     utils.run_snapshot_comparison(
         test_name=test_name,
         config=mock_config,
         mismatch_cb=fake_cb,
     )
 
-    mock_snapshot_cls.assert_called_once_with(root=mock_snapshot_old.root)
-    assert mock_config.stash[utils.SNAPSHOT_KEY] is mock_snapshot_cls.return_value
+    mock_factory.create_snapshot.assert_called_once_with(root=mock_snapshot_old.root)
     mock_comparator.compare.assert_called_once_with(
         mock_snapshot_old,
-        mock_snapshot_cls.return_value,
+        mock_snapshot_new,
     )
+    assert mock_config.stash[utils.SNAPSHOT_KEY] is mock_snapshot_new
     if matches:
         mock_cb.assert_not_called()
     else:
         mock_cb.assert_called_once_with(test_name, mock_comparator.compare.return_value)
 
 
 @pytest.mark.parametrize("basetemp", [None, Path("tmp")])
 def test_pytest_configure(monkeypatch: "MonkeyPatch", basetemp: Optional[Path]) -> None:
-    mock_snapshot_cls = Mock(spec=snapshots.TreeSnapshot)
+    mock_snapshot_factory_cls = Mock(spec=snapshots.TreeSnapshotFactory)
     monkeypatch.setattr(
-        "pytest_litter.plugin.plugin.TreeSnapshot",
-        mock_snapshot_cls,
+        "pytest_litter.plugin.plugin.TreeSnapshotFactory",
+        mock_snapshot_factory_cls,
     )
     mock_comparator_cls = Mock(spec=snapshots.SnapshotComparator)
     monkeypatch.setattr(
         "pytest_litter.plugin.plugin.SnapshotComparator",
         mock_comparator_cls,
     )
     mock_config = Mock(
         spec=pytest.Config,
         rootpath=Path("rootpath"),
         stash={},
         getoption=Mock(spec=pytest.Config.getoption, return_value=basetemp),
     )
+    mock_litter_config_cls = Mock(spec=snapshots.LitterConfig)
+    monkeypatch.setattr(
+        "pytest_litter.plugin.plugin.LitterConfig", mock_litter_config_cls
+    )
     mock_dir_ignore_spec = Mock(spec=snapshots.DirectoryIgnoreSpec)
     monkeypatch.setattr(
         "pytest_litter.plugin.plugin.DirectoryIgnoreSpec",
         mock_dir_ignore_spec,
     )
-    mock_regex_ignore_spec = Mock(spec=snapshots.RegexIgnoreSpec)
+    mock_name_ignore_spec = Mock(spec=snapshots.NameIgnoreSpec)
     monkeypatch.setattr(
-        "pytest_litter.plugin.plugin.RegexIgnoreSpec",
-        mock_regex_ignore_spec,
+        "pytest_litter.plugin.plugin.NameIgnoreSpec",
+        mock_name_ignore_spec,
     )
     expected_ignore_specs = []
     if basetemp is not None:
         expected_ignore_specs.append(mock_dir_ignore_spec.return_value)
-    expected_ignore_specs.append(mock_regex_ignore_spec.return_value)
+    expected_ignore_specs.append(mock_name_ignore_spec.return_value)
+    expected_ignore_specs.append(mock_name_ignore_spec.return_value)
+    expected_ignore_specs.append(mock_name_ignore_spec.return_value)
+    expected_ignore_specs.append(mock_name_ignore_spec.return_value)
 
     plugin.pytest_configure(mock_config)
 
     mock_config.getoption.assert_called_once_with("basetemp", None)
-    assert mock_config.stash[utils.SNAPSHOT_KEY] is mock_snapshot_cls.return_value
-    mock_snapshot_cls.assert_called_once_with(root=mock_config.rootpath)
-    assert mock_config.stash[utils.COMPARATOR_KEY] is mock_comparator_cls.return_value
-    mock_comparator_cls.assert_called_once_with(
+    mock_litter_config_cls.assert_called_once_with(
         ignore_specs=expected_ignore_specs,
     )
+    mock_snapshot_factory_cls.assert_called_once_with(
+        config=mock_litter_config_cls.return_value
+    )
+    mock_snapshot_factory_cls.return_value.create_snapshot.assert_called_once_with(
+        root=mock_config.rootpath
+    )
+    assert (
+        mock_config.stash[utils.SNAPSHOT_FACTORY_KEY]
+        is mock_snapshot_factory_cls.return_value
+    )
+    assert (
+        mock_config.stash[utils.SNAPSHOT_KEY]
+        is mock_snapshot_factory_cls.return_value.create_snapshot.return_value
+    )
+    assert mock_config.stash[utils.COMPARATOR_KEY] is mock_comparator_cls.return_value
+
     if basetemp is not None:
         mock_dir_ignore_spec.assert_has_calls(
             [call(directory=mock_config.rootpath / basetemp)]
         )
     else:
         mock_dir_ignore_spec.assert_not_called()
-    mock_regex_ignore_spec.assert_has_calls([call(regex=r".*/__pycache__.*")])
+    mock_name_ignore_spec.assert_has_calls(
+        [
+            call(name="__pycache__"),
+            call(name="venv"),
+            call(name=".venv"),
+            call(name=".pytest_cache"),
+        ]
+    )
 
 
 def test_pytest_runtest_call(monkeypatch: "MonkeyPatch") -> None:
     mock_raise_test_error = Mock(spec=utils.raise_test_error_from_comparison)
     monkeypatch.setattr(
         "pytest_litter.plugin.plugin.raise_test_error_from_comparison",
         mock_raise_test_error,
@@ -214,10 +241,10 @@
 
 
 @pytest.mark.integration_test
 def test_plugin_with_pytester(pytester: pytest.Pytester) -> None:
     # pytester uses basetemp internally, so the case without basetemp
     # cannot be tested using pytester.
     pytester.copy_example("pytest.ini")
-    pytester.copy_example("pytester_tests.py")
+    pytester.copy_example("suite_tests.py")
     result: pytest.RunResult = pytester.runpytest()
     result.assert_outcomes(passed=2, xfailed=2)
```

### Comparing `pytest-litter-0.0.2/tests/test_snapshots.py` & `pytest-litter-0.0.3/tests/test_snapshots.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 """Tests for the snapshots module."""
 import re
 from collections.abc import Hashable, Iterable
 from pathlib import Path
-from typing import Union
+from typing import Optional, Union
 
 import pytest
 
 from pytest_litter import snapshots
 
 
+@pytest.fixture(name="empty_config")
+def fixture_empty_config() -> snapshots.LitterConfig:
+    return snapshots.LitterConfig()
+
+
+@pytest.fixture(name="snapshot_factory")
+def fixture_snapshot_factory(
+    empty_config: snapshots.LitterConfig,
+) -> snapshots.TreeSnapshotFactory:
+    return snapshots.TreeSnapshotFactory(config=empty_config)
+
+
 @pytest.fixture(name="tmp_tree_root")
 def fixture_tmp_tree_root(tmp_path: Path) -> Path:
     root = tmp_path
     subdir_a = root / "a"
     subdir_a_1 = subdir_a / "a_1"
     subdir_b = root / "b"
     subdir_a_1.mkdir(parents=True, exist_ok=True)
@@ -23,22 +35,22 @@
     b_file.touch()
     a_1_file = subdir_a_1 / "a_1_file"
     a_1_file.touch()
     return root
 
 
 @pytest.fixture(name="tree_paths")
-def fixture_tree_paths(tmp_tree_root: Path) -> list[snapshots.PathSnapshot]:
+def fixture_tree_paths(tmp_tree_root: Path) -> list[Path]:
     return [
-        snapshots.PathSnapshot(path=tmp_tree_root / "a"),
-        snapshots.PathSnapshot(path=tmp_tree_root / "a" / "a_file"),
-        snapshots.PathSnapshot(path=tmp_tree_root / "b"),
-        snapshots.PathSnapshot(path=tmp_tree_root / "b" / "b_file"),
-        snapshots.PathSnapshot(path=tmp_tree_root / "a" / "a_1"),
-        snapshots.PathSnapshot(path=tmp_tree_root / "a" / "a_1" / "a_1_file"),
+        tmp_tree_root / "a",
+        tmp_tree_root / "a" / "a_file",
+        tmp_tree_root / "b",
+        tmp_tree_root / "b" / "b_file",
+        tmp_tree_root / "a" / "a_1",
+        tmp_tree_root / "a" / "a_1" / "a_1_file",
     ]
 
 
 def test_path_snapshot(tmp_tree_root: Path) -> None:
     input_path = tmp_tree_root / "a"
     snapshot = snapshots.PathSnapshot(path=input_path)
     assert str(snapshot) == str(input_path)
@@ -48,23 +60,24 @@
     assert snapshot != input_path
     assert snapshot.path == input_path
 
 
 def test_tree_snapshot__bad_root(tmp_path: Path) -> None:
     input_path = tmp_path / "fake_file"
     with pytest.raises(snapshots.UnexpectedLitterError):
-        _ = snapshots.TreeSnapshot(root=input_path)
+        # paths are irrelevant here
+        _ = snapshots.TreeSnapshot(root=input_path, paths=[])
 
 
-def test_tree_snapshot(
-    tmp_tree_root: Path, tree_paths: list[snapshots.PathSnapshot]
-) -> None:
-    snapshot = snapshots.TreeSnapshot(root=tmp_tree_root)
+def test_tree_snapshot(tmp_tree_root: Path, tree_paths: list[Path]) -> None:
+    snapshot = snapshots.TreeSnapshot(root=tmp_tree_root, paths=tree_paths)
     assert snapshot.root == tmp_tree_root
-    assert snapshot.paths == frozenset(tree_paths)
+    assert snapshot.paths == frozenset(
+        snapshots.PathSnapshot(path) for path in tree_paths
+    )
 
 
 @pytest.mark.parametrize(
     "only_a, only_b, expected_match",
     [
         ([], [], True),
         ((), (), True),
@@ -101,15 +114,15 @@
         (Path("subdir"), snapshots.PathSnapshot(path=Path("subdir/subsub/b")), True),
     ],
 )
 def test_directory_ignore_spec(
     directory: Path, path: snapshots.PathSnapshot, expected_match: bool
 ) -> None:
     ignore_spec = snapshots.DirectoryIgnoreSpec(directory=directory)
-    assert ignore_spec.matches(path=path) == expected_match
+    assert ignore_spec.matches(path=path.path) == expected_match
 
 
 @pytest.mark.parametrize(
     "regex, path, expected_match",
     [
         (r"sub\w+/a", snapshots.PathSnapshot(path=Path("subdir/a")), True),
         (r"sub\w+/a", snapshots.PathSnapshot(path=Path("subdir/b")), False),
@@ -119,67 +132,116 @@
 )
 def test_regex_ignore_spec(
     regex: Union[str, re.Pattern[str]],
     path: snapshots.PathSnapshot,
     expected_match: bool,
 ) -> None:
     ignore_spec = snapshots.RegexIgnoreSpec(regex=regex)
-    assert ignore_spec.matches(path=path) == expected_match
+    assert ignore_spec.matches(path=path.path) == expected_match
 
 
-def test_snapshot_comparator__same(tmp_tree_root: Path) -> None:
-    snapshot = snapshots.TreeSnapshot(root=tmp_tree_root)
-    comparison = snapshots.SnapshotComparator().compare(snapshot, snapshot)
+def test_snapshot_comparator__same(
+    empty_config: snapshots.LitterConfig, tmp_tree_root: Path, tree_paths: list[Path]
+) -> None:
+    snapshot = snapshots.TreeSnapshot(root=tmp_tree_root, paths=tree_paths)
+    comparison = snapshots.SnapshotComparator(config=empty_config).compare(
+        snapshot, snapshot
+    )
     assert comparison.matches
     assert not comparison.only_a
     assert not comparison.only_b
 
 
-def test_snapshot_comparator__only_b(tmp_tree_root: Path) -> None:
-    snapshot_a = snapshots.TreeSnapshot(root=tmp_tree_root)
+def test_snapshot_comparator__only_b(
+    empty_config: snapshots.LitterConfig, tmp_tree_root: Path, tree_paths: list[Path]
+) -> None:
+    snapshot_a = snapshots.TreeSnapshot(root=tmp_tree_root, paths=tree_paths)
     new_file = tmp_tree_root / "new_file"
-    new_file.touch()
-    snapshot_b = snapshots.TreeSnapshot(root=tmp_tree_root)
-    comparison = snapshots.SnapshotComparator().compare(snapshot_a, snapshot_b)
+    tree_paths.append(new_file)
+    snapshot_b = snapshots.TreeSnapshot(root=tmp_tree_root, paths=tree_paths)
+    comparison = snapshots.SnapshotComparator(config=empty_config).compare(
+        snapshot_a, snapshot_b
+    )
     assert not comparison.matches
     assert not comparison.only_a
     assert comparison.only_b == frozenset((snapshots.PathSnapshot(path=new_file),))
 
 
-def test_snapshot_comparator__only_a(tmp_tree_root: Path) -> None:
-    snapshot_b = snapshots.TreeSnapshot(root=tmp_tree_root)
+def test_snapshot_comparator__only_a(
+    empty_config: snapshots.LitterConfig, tmp_tree_root: Path, tree_paths: list[Path]
+) -> None:
+    snapshot_b = snapshots.TreeSnapshot(root=tmp_tree_root, paths=tree_paths)
     new_file = tmp_tree_root / "new_file"
-    new_file.touch()
-    snapshot_a = snapshots.TreeSnapshot(root=tmp_tree_root)
-    comparison = snapshots.SnapshotComparator().compare(snapshot_a, snapshot_b)
+    tree_paths.append(new_file)
+    snapshot_a = snapshots.TreeSnapshot(root=tmp_tree_root, paths=tree_paths)
+    comparison = snapshots.SnapshotComparator(config=empty_config).compare(
+        snapshot_a, snapshot_b
+    )
     assert not comparison.matches
     assert comparison.only_a == frozenset((snapshots.PathSnapshot(path=new_file),))
     assert not comparison.only_b
 
 
+def test_snapshot_comparator__incompatible_snapshots(
+    empty_config: snapshots.LitterConfig, tmp_tree_root: Path
+) -> None:
+    # TreeSnapshot paths are incorrect, but that is irrelevant for this test.
+    snapshot_a = snapshots.TreeSnapshot(root=tmp_tree_root, paths=[])
+    snapshot_b = snapshots.TreeSnapshot(root=tmp_tree_root / "a", paths=[])
+    comparator = snapshots.SnapshotComparator(config=empty_config)
+    with pytest.raises(snapshots.UnexpectedLitterError):
+        _ = comparator.compare(snapshot_a, snapshot_b)
+
+
+@pytest.mark.parametrize(
+    "ignore_specs", [None, [], [snapshots.RegexIgnoreSpec(regex=r".*")]]
+)
+def test_litter_config(ignore_specs: Optional[Iterable[snapshots.IgnoreSpec]]) -> None:
+    config = snapshots.LitterConfig(ignore_specs=ignore_specs)
+    assert config.ignore_specs == frozenset(ignore_specs or [])
+
+
+class _FakeIgnoreSpec(snapshots.IgnoreSpec):
+    def matches(self, path: Path) -> bool:
+        return "a" in path.parts
+
+
 @pytest.mark.parametrize(
-    "ignore_spec",
+    "config, expected_paths",
     [
-        snapshots.RegexIgnoreSpec(regex=r".*/new_file\.\w+"),
+        (
+            snapshots.LitterConfig(),
+            [
+                Path("a"),
+                Path("a/a_file"),
+                Path("a/a_1"),
+                Path("a/a_1/a_1_file"),
+                Path("b"),
+                Path("b/b_file"),
+            ],
+        ),
+        (
+            snapshots.LitterConfig(ignore_specs=[_FakeIgnoreSpec()]),
+            [Path("b"), Path("b/b_file")],
+        ),
     ],
 )
-def test_snapshot_comparator__only_b__ignored(
-    tmp_tree_root: Path, ignore_spec: snapshots.IgnoreSpec
+def test_create_snapshot(
+    config: snapshots.LitterConfig, expected_paths: list[Path], tmp_tree_root: Path
 ) -> None:
-    snapshot_a = snapshots.TreeSnapshot(root=tmp_tree_root)
-    (tmp_tree_root / "new_file.txt").touch()
-    (tmp_tree_root / "new_file.yml").touch()
-    snapshot_b = snapshots.TreeSnapshot(root=tmp_tree_root)
-    comparison = snapshots.SnapshotComparator(ignore_specs=[ignore_spec]).compare(
-        snapshot_a, snapshot_b
-    )
-    assert comparison.matches
-    assert not comparison.only_a
-    assert not comparison.only_b
+    factory = snapshots.TreeSnapshotFactory(config=config)
+    snapshot: snapshots.TreeSnapshot = factory.create_snapshot(root=tmp_tree_root)
+    assert {str(p) for p in snapshot.paths} == {
+        str(tmp_tree_root / path) for path in expected_paths
+    }
 
 
-def test_snapshot_comparator__incompatible_snapshots(tmp_tree_root: Path) -> None:
-    snapshot_a = snapshots.TreeSnapshot(root=tmp_tree_root)
-    snapshot_b = snapshots.TreeSnapshot(root=tmp_tree_root / "a")
-    comparator = snapshots.SnapshotComparator()
-    with pytest.raises(snapshots.UnexpectedLitterError):
-        _ = comparator.compare(snapshot_a, snapshot_b)
+@pytest.mark.parametrize(
+    "name, path, expected_match",
+    [
+        ("c", Path("a/b/c"), True),
+        ("c", Path("a/b"), False),
+        ("a", Path("a/b"), True),
+    ],
+)
+def test_name_ignore_spec(name: str, path: Path, expected_match: bool) -> None:
+    assert snapshots.NameIgnoreSpec(name=name).matches(path=path) == expected_match
```

