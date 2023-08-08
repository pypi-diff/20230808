# Comparing `tmp/OpenGeode_Inspector-3.0.9-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/OpenGeode_Inspector-3.0.9rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 360237 bytes, number of entries: 8
--rw-r--r--  2.0 unx       71 b- defN 23-Aug-08 01:06 opengeode_inspector/__init__.py
--rw-r--r--  2.0 unx      262 b- defN 23-Aug-08 01:06 opengeode_inspector/inspector.py
--rwxr-xr-x  2.0 unx   622208 b- defN 23-Aug-08 01:07 opengeode_inspector/lib64/libOpenGeode-Inspector_inspector.so
--rwxr-xr-x  2.0 unx   541536 b- defN 23-Aug-08 01:07 opengeode_inspector/lib64/opengeode_inspector_py_inspector.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx     5345 b- defN 23-Aug-08 01:07 OpenGeode_Inspector-3.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx      103 b- defN 23-Aug-08 01:07 OpenGeode_Inspector-3.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Aug-08 01:07 OpenGeode_Inspector-3.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      789 b- defN 23-Aug-08 01:07 OpenGeode_Inspector-3.0.9.dist-info/RECORD
-8 files, 1170334 bytes uncompressed, 358829 bytes compressed:  69.3%
+Zip file size: 266862 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      175 b- defN 23-Aug-07 10:24 opengeode_inspector/__init__.py
+-rw-rw-rw-  2.0 fat      271 b- defN 23-Aug-07 10:24 opengeode_inspector/inspector.py
+-rw-rw-rw-  2.0 fat   444416 b- defN 23-Aug-07 10:25 opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll
+-rw-rw-rw-  2.0 fat   451584 b- defN 23-Aug-07 10:25 opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     5488 b- defN 23-Aug-07 10:25 OpenGeode_Inspector-3.0.9rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-07 10:25 OpenGeode_Inspector-3.0.9rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Aug-07 10:25 OpenGeode_Inspector-3.0.9rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      784 b- defN 23-Aug-07 10:25 OpenGeode_Inspector-3.0.9rc1.dist-info/RECORD
+8 files, 902838 bytes uncompressed, 265466 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: opengeode_inspector/__init__.py
 Comment: 
 
 Filename: opengeode_inspector/inspector.py
 Comment: 
 
-Filename: opengeode_inspector/lib64/libOpenGeode-Inspector_inspector.so
+Filename: opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll
 Comment: 
 
-Filename: opengeode_inspector/lib64/opengeode_inspector_py_inspector.cpython-39-x86_64-linux-gnu.so
+Filename: opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd
 Comment: 
 
-Filename: OpenGeode_Inspector-3.0.9.dist-info/METADATA
+Filename: OpenGeode_Inspector-3.0.9rc1.dist-info/METADATA
 Comment: 
 
-Filename: OpenGeode_Inspector-3.0.9.dist-info/WHEEL
+Filename: OpenGeode_Inspector-3.0.9rc1.dist-info/WHEEL
 Comment: 
 
-Filename: OpenGeode_Inspector-3.0.9.dist-info/top_level.txt
+Filename: OpenGeode_Inspector-3.0.9rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: OpenGeode_Inspector-3.0.9.dist-info/RECORD
+Filename: OpenGeode_Inspector-3.0.9rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opengeode_inspector/__init__.py

```diff
@@ -1,3 +1,6 @@
-## Copyright (c) 2019 - 2023 Geode-solutions
-
-from .inspector import *
+## Copyright (c) 2019 - 2023 Geode-solutions
+
+import os, pathlib
+os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
+
+from .inspector import *
```

## opengeode_inspector/inspector.py

```diff
@@ -1,11 +1,11 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import opengeode_io
-import opengeode_geosciences
-import opengeode_geosciencesio
-
-from .lib64.opengeode_inspector_py_inspector import *
-InspectorInspectorLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import opengeode_io
+import opengeode_geosciences
+import opengeode_geosciencesio
+
+from .bin.opengeode_inspector_py_inspector import *
+InspectorInspectorLibrary.initialize()
```

## Comparing `OpenGeode_Inspector-3.0.9.dist-info/METADATA` & `OpenGeode_Inspector-3.0.9rc1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,113 +1,116 @@
-Metadata-Version: 2.1
-Name: OpenGeode-Inspector
-Version: 3.0.9
-Summary: Open source framework for inspecting the validity of geometric models
-Home-page: https://github.com/Geode-solutions/OpenGeode-Inspector
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: MIT
-Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core (==14.*,>=14.4.7)
-Requires-Dist: opengeode-geosciences (==7.*,>=7.1.5)
-Requires-Dist: opengeode-geosciencesio (==4.*,>=4.2.2)
-Requires-Dist: opengeode-io (==6.*,>=6.0.11)
-
-<h1 align="center">OpenGeode-Inspector<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">OpenGeode module for inspecting meshes and models</h3>
-
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/OpenGeode-ModuleTemplate/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/OpenGeode-ModuleTemplate/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/OpenGeode-ModuleTemplate/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/OpenGeode-ModuleTemplate.svg" alt="Version">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
-  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
-  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
-  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
-  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
-  <a href="https://opengeode-slack-invite.herokuapp.com">
-    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
-  </a>
-  <a href="https://doi.org/10.5281/zenodo.3610370">
-    <img src="https://zenodo.org/badge/DOI/10.5281/zenodo.3610370.svg" alt="DOI">
-  </a>
-
----
-
-## Introduction
-
-OpenGeode-Inspector is a module of [OpenGeode] providing ways of inspecting your meshes and models and verifying their validity.
-
-[OpenGeode]: https://github.com/Geode-solutions/OpenGeode
-
-## Documentation
-
-Go check out the online documentation at [docs.geode-solutions.com].
-
-[docs.geode-solutions.com] https://docs.geode-solutions.com
-
-Installing OpenGeode-Inspector is done:
-
- * either by compiling the C++ source.
- * or by installing the python library using the pip command ```pip install opengeode-inspector```.
-
-## Usage
-
-To use OpenGeode-Inspector, several options are available:
-
- * If you installed and compiled the C++ source code, you can use the executable binaries to apply an inspection of your meshes/models and toggle on/off the various checks directly.
- * or use the API functions (check the tests to see how it is done) if you want to go further or use the resulting errors to repair your meshes/models.
- * If you installed the python library, you can add ```import opengeode_inspector``` in your Python script to use the available API functions. Check [this documentation page](https://docs.geode-solutions.com/how-to-use-binding) for more details. Examples are also procured in the ```examples``` folder.
- * You can inspect your models without any installation, by using the API of the [Geode-solutions free tools](https://geode-solutions.com/tools).
-
-The available checks for each mesh type are:
- * PointSet:
-   * Colocation of vertices
- * EdgedCurve:
-   * Colocation of vertices
-   * Degeneration of edges
- * SurfaceMesh:
-   * Adjacency of polygons
-   * Colocation of vertices
-   * Degeneration of edges
-   * Degeneration of polygons
-   * Intersection of triangles (for triangulated surfaces)
-   * Manifold of vertices
-   * Manifold of edges
- * SolidMesh:
-   * Adjacency of polyhedra
-   * Colocation of vertices
-   * Degeneration of edges
-   * Degeneration of polyhedra
-   * Manifold of vertices
-   * Manifold of edges
-   * Manifold of facets
-The available checks for each model type are:
- * Section:
-   * Validity of the topology
-   * Checks on each component mesh: all the previous mesh checks depending on the component mesh type
-   * Checks on the validity of the unique vertices (linking to vertices, colocation of unique vertices points, un-colocation of points with same unique vertices)
-   * Intersection of the component mesh surfaces between each other
- * BRep:
-   * Validity of the topology
-   * Checks on each component mesh: all the previous mesh checks depending on the component mesh type
-   * Checks on the validity of the unique vertices (linking to vertices, colocation of unique vertices points, un-colocation of points with same unique vertices)
-   * Intersection of the component mesh surfaces between each other
-
-## Questions
-For questions and support please use the official [slack](https://opengeode-slack-invite.herokuapp.com) and go to the channel #inspector. The issue list of this repo is exclusively for bug reports and feature requests. 
-
-
-## License
-
-[MIT](https://opensource.org/licenses/MIT)
-
-Copyright (c) 2019 - 2023, Geode-solutions
+Metadata-Version: 2.1
+Name: OpenGeode-Inspector
+Version: 3.0.9rc1
+Summary: Open source framework for inspecting the validity of geometric models
+Home-page: https://github.com/Geode-solutions/OpenGeode-Inspector
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: MIT
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+Requires-Dist: opengeode-core ==14.*,>=14.4.7rc1
+Requires-Dist: opengeode-geosciences ==7.*,>=7.1.5rc1
+Requires-Dist: opengeode-geosciencesio ==4.*,>=4.2.2rc1
+Requires-Dist: opengeode-io ==6.*,>=6.0.11rc1
+
+<h1 align="center">OpenGeode-Inspector<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">OpenGeode module for inspecting meshes and models</h3>
+
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/OpenGeode-ModuleTemplate/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/OpenGeode-ModuleTemplate/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/OpenGeode-ModuleTemplate/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/OpenGeode-ModuleTemplate.svg" alt="Version">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
+  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
+  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
+  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
+  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
+  <a href="https://opengeode-slack-invite.herokuapp.com">
+    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
+  </a>
+  <a href="https://doi.org/10.5281/zenodo.3610370">
+    <img src="https://zenodo.org/badge/DOI/10.5281/zenodo.3610370.svg" alt="DOI">
+  </a>
+
+---
+
+## Introduction
+
+OpenGeode-Inspector is a module of [OpenGeode] providing ways of inspecting your meshes and models and verifying their validity.
+
+[OpenGeode]: https://github.com/Geode-solutions/OpenGeode
+
+## Documentation
+
+Go check out the online documentation at [docs.geode-solutions.com].
+
+[docs.geode-solutions.com] https://docs.geode-solutions.com
+
+Installing OpenGeode-Inspector is done:
+
+ * either by compiling the C++ source.
+ * or by installing the python library using the pip command ```pip install opengeode-inspector```.
+
+## Usage
+
+To use OpenGeode-Inspector, several options are available:
+
+ * If you installed and compiled the C++ source code, you can use the executable binaries to apply an inspection of your meshes/models and toggle on/off the various checks directly.
+ * or use the API functions (check the tests to see how it is done) if you want to go further or use the resulting errors to repair your meshes/models.
+ * If you installed the python library, you can add ```import opengeode_inspector``` in your Python script to use the available API functions. Check [this documentation page](https://docs.geode-solutions.com/how-to-use-binding) for more details. Examples are also procured in the ```examples``` folder.
+ * You can inspect your models without any installation, by using the API of the [Geode-solutions free tools](https://geode-solutions.com/tools).
+
+The available checks for each mesh type are:
+ * PointSet:
+   * Colocation of vertices
+ * EdgedCurve:
+   * Colocation of vertices
+   * Degeneration of edges
+ * SurfaceMesh:
+   * Adjacency of polygons
+   * Colocation of vertices
+   * Degeneration of edges
+   * Degeneration of polygons
+   * Intersection of triangles (for triangulated surfaces)
+   * Manifold of vertices
+   * Manifold of edges
+ * SolidMesh:
+   * Adjacency of polyhedra
+   * Colocation of vertices
+   * Degeneration of edges
+   * Degeneration of polyhedra
+   * Manifold of vertices
+   * Manifold of edges
+   * Manifold of facets
+The available checks for each model type are:
+ * Section:
+   * Validity of the topology
+   * Checks on each component mesh: all the previous mesh checks depending on the component mesh type
+   * Checks on the validity of the unique vertices (linking to vertices, colocation of unique vertices points, un-colocation of points with same unique vertices)
+   * Intersection of the component mesh surfaces between each other
+ * BRep:
+   * Validity of the topology
+   * Checks on each component mesh: all the previous mesh checks depending on the component mesh type
+   * Checks on the validity of the unique vertices (linking to vertices, colocation of unique vertices points, un-colocation of points with same unique vertices)
+   * Intersection of the component mesh surfaces between each other
+
+## Questions
+For questions and support please use the official [slack](https://opengeode-slack-invite.herokuapp.com) and go to the channel #inspector. The issue list of this repo is exclusively for bug reports and feature requests. 
+
+
+## License
+
+[MIT](https://opensource.org/licenses/MIT)
+
+Copyright (c) 2019 - 2023, Geode-solutions
+
+
```

### html2text {}

```diff
@@ -1,14 +1,15 @@
-Metadata-Version: 2.1 Name: OpenGeode-Inspector Version: 3.0.9 Summary: Open
+Metadata-Version: 2.1 Name: OpenGeode-Inspector Version: 3.0.9rc1 Summary: Open
 source framework for inspecting the validity of geometric models Home-page:
 https://github.com/Geode-solutions/OpenGeode-Inspector Author: Geode-solutions
-Author-email: contact@geode-solutions.com License: MIT Description-Content-
-Type: text/markdown Requires-Dist: opengeode-core (==14.*,>=14.4.7) Requires-
-Dist: opengeode-geosciences (==7.*,>=7.1.5) Requires-Dist: opengeode-
-geosciencesio (==4.*,>=4.2.2) Requires-Dist: opengeode-io (==6.*,>=6.0.11)
+Author-email: contact@geode-solutions.com License: MIT Platform: UNKNOWN
+Description-Content-Type: text/markdown Requires-Dist: opengeode-core
+==14.*,>=14.4.7rc1 Requires-Dist: opengeode-geosciences ==7.*,>=7.1.5rc1
+Requires-Dist: opengeode-geosciencesio ==4.*,>=4.2.2rc1 Requires-Dist:
+opengeode-io ==6.*,>=6.0.11rc1
               ****** OpenGeode-Inspectorby Geode-solutions ******
           **** OpenGeode module for inspecting meshes and models ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
       [Language] [License] [Semantic-release] [Slack_invite] [DOI] --- ##
  Introduction OpenGeode-Inspector is a module of [OpenGeode] providing ways of
  inspecting your meshes and models and verifying their validity. [OpenGeode]:
```

