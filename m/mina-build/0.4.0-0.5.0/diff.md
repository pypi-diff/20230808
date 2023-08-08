# Comparing `tmp/mina-build-0.4.0.tar.gz` & `tmp/mina_build-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mina-build-0.4.0.tar", last modified: Wed Jun 14 12:10:04 2023, max compression
+gzip compressed data, was "mina_build-0.5.0.tar", last modified: Tue Aug  8 08:17:20 2023, max compression
```

## Comparing `mina-build-0.4.0.tar` & `mina_build-0.5.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      381 2023-06-14 12:09:44.821847 mina-build-0.4.0/README.build.md
--rw-r--r--   0        0        0    11045 2023-06-14 12:09:44.821847 mina-build-0.4.0/mina/backend/__init__.py
--rw-r--r--   0        0        0     1499 2023-06-14 12:09:44.821847 mina-build-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 mina-build-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      381 2023-08-08 08:16:49.431067 mina_build-0.5.0/README.build.md
+-rw-r--r--   0        0        0    11409 2023-08-08 08:16:49.431067 mina_build-0.5.0/mina/backend/__init__.py
+-rw-r--r--   0        0        0     1654 2023-08-08 08:17:20.647318 mina_build-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 mina_build-0.5.0/PKG-INFO
```

### Comparing `mina-build-0.4.0/mina/backend/__init__.py` & `mina_build-0.5.0/mina/backend/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from __future__ import annotations
 
 import functools
 import os
 from pathlib import Path
-from typing import Any, Dict, Mapping, Optional
+from typing import Any, Dict, Mapping, Optional, cast
 
 try:
     import tomllib as tomli  # type: ignore
 except ImportError:
     try:
         from pdm.backend._vendor import tomli
     except ImportError:
-        import tomli
+        import tomli  # type: ignore
 
 from pdm.backend._vendor.packaging.requirements import Requirement
 from pdm.backend import \
     get_requires_for_build_sdist as get_requires_for_build_sdist
 from pdm.backend import \
     get_requires_for_build_wheel as get_requires_for_build_wheel
-from pdm.backend import \
-    prepare_metadata_for_build_wheel as prepare_metadata_for_build_wheel
 from pdm.backend.base import Builder
 from pdm.backend.config import Metadata, BuildConfig
 
 
 @functools.lru_cache(None)
 def _get_config_root():
     cwd = Path.cwd()
@@ -34,15 +32,15 @@
 def _get_root_project():
     return _get_config_root().get("project", {})
 
 
 @functools.lru_cache(None)
 def _get_tool_mina() -> dict[str, Any]:
     return _get_config_root().get("tool", {}).get("mina", {})
-
+   
 
 @functools.lru_cache(None)
 def _get_package(package: str) -> Dict[str, Any]:
     return _get_tool_mina().get("packages", {}).get(package, {})
 
 
 def _has_package(package: str) -> bool:
@@ -69,46 +67,46 @@
         if "override" in pkg:
             return pkg["override"]
     return _using_override_global()
 
 
 def _patch_dep(pkg_project: dict[str, Any]):
     if "dependencies" in pkg_project:
-        optional_dependencies: list[str] = []
+        dependencies: list[str] = []
 
-        optional_deps: list[str] = pkg_project["dependencies"]
+        deps = cast(list[str], pkg_project["dependencies"])
         workspace_deps_origin: list[str] = _get_root_project().get("dependencies", [])
         workspace_deps_convert = [Requirement(i) for i in workspace_deps_origin]
         workspace_deps_map = {
             i.name: i for i in workspace_deps_convert if i.name is not None
         }
 
-        for dep in optional_deps:
+        for dep in deps:
             req = Requirement(dep)
             if req.name is None:
                 raise ValueError(f"'{dep}' is not a valid requirement")
             if req.name not in workspace_deps_map:
                 raise ValueError(f"{req.name} is not defined in project requirements")
-            optional_dependencies.append(str(workspace_deps_map[req.name]))
+            dependencies.append(str(workspace_deps_map[req.name]))
 
-        pkg_project["dependencies"] = optional_dependencies
+        pkg_project["dependencies"] = dependencies
 
     if "optional-dependencies" in pkg_project:
         optional_dependencies: dict[str, list[str]] = {}
 
-        deps: dict[str, list[str]] = pkg_project["optional-dependencies"]
+        optional_dep_groups: dict[str, list[str]] = pkg_project["optional-dependencies"]
 
         # workspace don't use optional dep: it must contains ALL deps mina required.
         workspace_deps_origin: list[str] = _get_root_project().get("dependencies", [])
         workspace_deps_convert = [Requirement(i) for i in workspace_deps_origin]
         workspace_deps_map = {
             i.name: i for i in workspace_deps_convert if i.name is not None
         }
 
-        for group, optional_deps in deps.items():
+        for group, optional_deps in optional_dep_groups.items():
             group_deps = []
             for dep in optional_deps:
                 req = Requirement(dep)
                 if req.name is None:
                     raise ValueError(f"'{dep}' is not a valid requirement")
                 if req.name not in workspace_deps_map:
                     raise ValueError(
@@ -116,26 +114,41 @@
                     )
                 group_deps.append(str(workspace_deps_map[req.name]))
             optional_dependencies[group] = group_deps
 
         pkg_project["optional-dependencies"] = optional_dependencies
 
 
+def _get_standalone_config(pkg: str):
+    config_file = Path.cwd() / ".mina" / f"{pkg}.toml"
+    if not config_file.exists():
+        return
+    
+    return tomli.loads(config_file.read_text())
+
+
 def _patch_pdm_config(package: str):
     cwd = Path.cwd()
     config = Builder(cwd).config
 
-    package_conf = (
-        config.data.get("tool", {})
-        .get("mina", {})
-        .get("packages", {})
-        .get(package, None)
-    )
-    if package_conf is None:
-        raise ValueError(f"No package named '{package}'")
+    package_conf = _get_standalone_config(package)
+    if package_conf is not None:
+        package_conf.setdefault("includes", []).append(
+            str(Path.cwd() / ".mina" / f"{package}.toml")
+        )
+    else:
+        package_conf = (
+            config.data.get("tool", {})
+            .get("mina", {})
+            .get("packages", {})
+            .get(package, None)
+        )
+        if package_conf is None:
+            raise ValueError(f"No package named '{package}'")
+
     package_project = package_conf.get("project", {})
 
     _patch_dep(package_project)
 
     pdm_settings = config.data.get("tool", {}).get("pdm", {}).get("build", {})
 
     # dev-dependencies is unnecessary for a pkg(for workspace), so it will be ignored by mina.
```

### Comparing `mina-build-0.4.0/pyproject.toml` & `mina_build-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 [project]
 name = "mina-build"
-version = "0.4.0"
+version = "0.5.0"
 description = "build backend for Mina Package Structure"
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
 dependencies = [
     "pdm-backend>=2.1.0",
     "tomli>=1.1.0; python_version < \"3.11\"",
+    "editables>=0.5",
 ]
 requires-python = ">=3.9"
 readme = "README.build.md"
 
 [project.license]
 text = "MIT"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "black>=22.3.0",
     "isort>=5.10.1",
     "devtools>=0.8.0",
 ]
 
+[tool.pdm.build]
+includes = [
+    "mina/backend",
+]
+
 [tool.mina]
 enabled = true
 override-global = false
 
 [tool.mina.packages.backend]
 override = false
 includes = [
     "mina/backend",
 ]
 raw-dependencies = []
 
 [tool.mina.packages.backend.project]
 name = "mina-build"
-version = "0.4.0"
+version = "0.5.0"
 description = "build backend for Mina Package Structure"
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
 dependencies = [
-    "pdm-backend",
-    "tomli",
+    "pdm-backend>=2.1.0",
+    "tomli>=1.1.0; python_version < \"3.11\"",
+    "editables>=0.5",
 ]
 requires-python = ">=3.9"
 readme = "README.build.md"
 
 [tool.mina.packages.backend.project.license]
 text = "MIT"
 
@@ -56,15 +63,15 @@
 ]
 excludes = [
     "mina/backend",
 ]
 
 [tool.mina.packages.cli-pdm.project]
 name = "pdm-mina"
-version = "0.2.2"
+version = "0.3.0"
 dependencies = [
     "pdm",
     "mina-build",
     "tomli",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
@@ -74,9 +81,10 @@
 
 [tool.mina.packages.cli-pdm.project.entry-points.pdm]
 mina = "mina.plugin:ensure_pdm"
 
 [build-system]
 requires = [
     "mina-build>=0.2.6",
+    "editables",
 ]
 build-backend = "mina.backend"
```

### Comparing `mina-build-0.4.0/PKG-INFO` & `mina_build-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: mina-build
-Version: 0.4.0
+Version: 0.5.0
 Summary: build backend for Mina Package Structure
+Author-Email: GreyElaina <GreyElaina@outlook.com>
 License: MIT
-Author-email: GreyElaina <GreyElaina@outlook.com>
 Requires-Python: >=3.9
+Requires-Dist: pdm-backend>=2.1.0
+Requires-Dist: tomli>=1.1.0; python_version < "3.11"
+Requires-Dist: editables>=0.5
 Description-Content-Type: text/markdown
 
 # PEP-517 implementation for Mina Package Structure
 
 `mina-build` 是 `Mina Package Structure` 的具体实现, 基于 `pdm-backend` 的现有建构.
 
 你需要在 `pyproject.toml` 内将 `tool.mina.enabled` 设为 `true` 才能使用 Mina 的相关功能,
 否则 `mina-build` 的行为与 `pdm-backend` 一致.
 
-若是需要关于 `Mina` 的更多信息, 请参阅其他的文稿.
+若是需要关于 `Mina` 的更多信息, 请参阅其他的文稿.
```

