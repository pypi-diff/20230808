# Comparing `tmp/pdm_build_locked-0.1.3.tar.gz` & `tmp/pdm_build_locked-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_build_locked-0.1.3.tar", last modified: Sun Jul 30 13:35:17 2023, max compression
+gzip compressed data, was "pdm_build_locked-0.1.4.tar", last modified: Tue Aug  8 15:18:49 2023, max compression
```

## Comparing `pdm_build_locked-0.1.3.tar` & `pdm_build_locked-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2023-07-30 13:34:58.923403 pdm_build_locked-0.1.3/LICENSE
--rw-r--r--   0        0        0     1017 2023-07-30 13:34:58.923403 pdm_build_locked-0.1.3/README.rst
--rw-r--r--   0        0        0     2052 2023-07-30 13:35:17.375301 pdm_build_locked-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      515 2023-07-30 13:34:58.923403 pdm_build_locked-0.1.3/src/pdm_build_locked/__init__.py
--rw-r--r--   0        0        0     6963 2023-07-30 13:34:58.923403 pdm_build_locked-0.1.3/src/pdm_build_locked/command.py
--rw-r--r--   0        0        0        0 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     2176 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0      200 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/data/invalid/pyproject.toml
--rw-r--r--   0        0        0   117717 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/data/large/pdm.lock
--rw-r--r--   0        0        0     1896 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/data/large/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/data/large/src/large/__init__.py
--rw-r--r--   0        0        0      221 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/data/simple-optional/pyproject.toml
--rw-r--r--   0        0        0      108 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/data/simple/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/unit/__init__.py
--rw-r--r--   0        0        0     7138 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/unit/test_build_locked.py
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 pdm_build_locked-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-08 15:18:26.427735 pdm_build_locked-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1017 2023-08-08 15:18:26.427735 pdm_build_locked-0.1.4/README.rst
+-rw-r--r--   0        0        0     2052 2023-08-08 15:18:49.943911 pdm_build_locked-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      515 2023-08-08 15:18:26.427735 pdm_build_locked-0.1.4/src/pdm_build_locked/__init__.py
+-rw-r--r--   0        0        0     7136 2023-08-08 15:18:26.431735 pdm_build_locked-0.1.4/src/pdm_build_locked/command.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:18:26.431735 pdm_build_locked-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     2176 2023-08-08 15:18:26.431735 pdm_build_locked-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0      200 2023-08-08 15:18:26.431735 pdm_build_locked-0.1.4/tests/data/invalid/pyproject.toml
+-rw-r--r--   0        0        0   117717 2023-08-08 15:18:26.431735 pdm_build_locked-0.1.4/tests/data/large/pdm.lock
+-rw-r--r--   0        0        0     1896 2023-08-08 15:18:26.431735 pdm_build_locked-0.1.4/tests/data/large/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-08 15:18:26.431735 pdm_build_locked-0.1.4/tests/data/large/src/large/__init__.py
+-rw-r--r--   0        0        0      221 2023-08-08 15:18:26.431735 pdm_build_locked-0.1.4/tests/data/simple-optional/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-08-08 15:18:26.431735 pdm_build_locked-0.1.4/tests/data/simple/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-08 15:18:26.431735 pdm_build_locked-0.1.4/tests/unit/__init__.py
+-rw-r--r--   0        0        0     7138 2023-08-08 15:18:26.431735 pdm_build_locked-0.1.4/tests/unit/test_build_locked.py
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 pdm_build_locked-0.1.4/PKG-INFO
```

### Comparing `pdm_build_locked-0.1.3/LICENSE` & `pdm_build_locked-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.3/README.rst` & `pdm_build_locked-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.3/pyproject.toml` & `pdm_build_locked-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3.11",
 ]
 authors = [
     { name = "sigma67", email = "sigma67.github@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.8"
-version = "0.1.3"
+version = "0.1.4"
 
 [project.entry-points.pdm]
 pdm-build-locked = "pdm_build_locked:plugin"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `pdm_build_locked-0.1.3/src/pdm_build_locked/__init__.py` & `pdm_build_locked-0.1.4/src/pdm_build_locked/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.3/src/pdm_build_locked/command.py` & `pdm_build_locked-0.1.4/src/pdm_build_locked/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import subprocess
 from contextlib import suppress
 from typing import Dict, List, Tuple, Union
 
 from pdm.cli import actions
 from pdm.cli.commands.build import Command as BaseCommand
 from pdm.exceptions import PdmException
-from pdm.models.candidates import Candidate
 from pdm.models.requirements import Requirement
 from pdm.project.core import Project
 from pdm.resolver import resolve
+from pdm.resolver.providers import ReusePinProvider
+from pdm.utils import normalize_name
 from resolvelib import BaseReporter
 
 DependencyList = Dict[str, Union[List[str], Dict[str, List[str]]]]
 
 # copied from pdm.models.repository due to TYPECHECKING guard
 CandidateKey = Tuple[str, Union[str, None], Union[str, None], bool]
 
@@ -58,18 +59,15 @@
 
         # retrieve locked dependencies and write to pyproject
         optional_dependencies: Dict[str, List[str]] = {}
 
         ###############################
         # determine locked dependencies
         ###############################
-        # performance optimization: we prepare the data structure here instead of searching inside the loop
-        locked_package_version: Dict[str, Tuple[CandidateKey, Candidate]] = {}
-        for package_key, package in project.locked_repository.packages.items():
-            locked_package_version[str(package.name)] = (package_key, package)
+        project.core.ui.echo("pdm-build-locked - Resolving locked packages from lockfile...")
 
         for group in groups:
             locked_group_name = self._get_locked_group_name(group)
 
             locked_packages = self._get_locked_packages(project, group)
             optional_dependencies[locked_group_name] = locked_packages
 
@@ -80,30 +78,30 @@
         # get reference to optional-dependencies in project.pyproject, or create it if it doesn't exist
         optional = project.pyproject.metadata.get(
             "optional-dependencies", None
         ) or project.pyproject.metadata.setdefault("optional-dependencies", {})
 
         # update target
         optional.update(optional_dependencies)
-        project.pyproject.write()
+        project.pyproject.write(show_message=False)
 
         # to prevent unclean scm status, we need to ignore pyproject.toml during build
         self._git_ignore_pyproject(project, True)
 
         ################
         # build project
         ################
         try:
             super().handle(project, options)
         finally:
             # undo our changes to pyproject.toml even if pdm build crashes
             for group in locked_groups:
                 with suppress(KeyError):
                     project.pyproject.metadata.get("optional-dependencies", {}).pop(group)
-            project.pyproject.write()
+            project.pyproject.write(show_message=False)
             self._git_ignore_pyproject(project, False)
 
     @staticmethod
     def _update_lockfile(project: Project) -> None:
         """
         Update the lockfile if needed
         Reimplementation of pdm install lockfile check and update
@@ -147,18 +145,27 @@
             group: the group to get pinned dependencies for
 
         Returns:
             Set of locked packages
         """
         requirements: Dict[str, Requirement] = project.get_dependencies(group)
 
-        # taken from pdm.actions.resolve_candidates_from_lockfile and adjusted so
-        # that environment markers are not evaluated
-        # -- we want to publish all requirements with markers
-        provider = project.get_provider(strategy="reuse", ignore_compatibility=True)
+        # get a ReusePinProvider - we don't want any calls to the remote repository,
+        # we just want to read from the lockfile
+        locked_repository = project.locked_repository
+        locked_repository.ignore_compatibility = True
+        project.get_provider()
+        # taken from pdm.actions.resolve_candidates_from_lockfile and adjusted
+        provider = ReusePinProvider(
+            locked_repository.all_candidates,
+            (),
+            locked_repository,
+            project.allow_prereleases,
+            {normalize_name(k): v for k, v in project.pyproject.resolution_overrides.items()},
+        )
         resolver = project.core.resolver_class(provider, BaseReporter())  # type: ignore
         reqs = list(requirements.values())
         candidates, *_ = resolve(resolver, reqs, project.environment.python_requires)
 
         return [str(c.req.as_pinned_version(c.version)) for c in candidates.values()]
 
     @staticmethod
```

### Comparing `pdm_build_locked-0.1.3/tests/conftest.py` & `pdm_build_locked-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.3/tests/data/large/pdm.lock` & `pdm_build_locked-0.1.4/tests/data/large/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.3/tests/data/large/pyproject.toml` & `pdm_build_locked-0.1.4/tests/data/large/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.3/tests/unit/test_build_locked.py` & `pdm_build_locked-0.1.4/tests/unit/test_build_locked.py`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.3/PKG-INFO` & `pdm_build_locked-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-build-locked
-Version: 0.1.3
+Version: 0.1.4
 Summary: \
                 pdm-build-locked is a pdm plugin to add locked packages as additional optional dependency groups
                 to the distribution metadata
             
 Keywords: pdm plugin
 Author-Email: sigma67 <sigma67.github@gmail.com>
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

