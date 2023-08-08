# Comparing `tmp/layout3mesh-0.1.0.tar.gz` & `tmp/layout3mesh-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layout3mesh-0.1.0.tar", max compression
+gzip compressed data, was "layout3mesh-0.1.1.tar", max compression
```

## Comparing `layout3mesh-0.1.0.tar` & `layout3mesh-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    17643 2023-08-08 13:15:32.980643 layout3mesh-0.1.0/LICENSE
--rw-r--r--   0        0        0     1135 2023-08-08 20:25:05.680601 layout3mesh-0.1.0/README.md
--rw-r--r--   0        0        0      151 2023-08-08 17:51:33.516801 layout3mesh-0.1.0/layout3mesh/__init__.py
--rw-r--r--   0        0        0     4564 2023-08-08 17:49:08.085697 layout3mesh-0.1.0/layout3mesh/cli.py
--rw-r--r--   0        0        0     2285 2023-08-08 18:42:42.239242 layout3mesh-0.1.0/layout3mesh/data.py
--rw-r--r--   0        0        0    10329 2023-08-08 20:21:37.260046 layout3mesh-0.1.0/layout3mesh/layout3mesh.py
--rw-r--r--   0        0        0     1003 2023-08-08 19:09:24.216676 layout3mesh-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2106 2023-08-08 20:27:22.793391 layout3mesh-0.1.0/setup.py
--rw-r--r--   0        0        0     1994 2023-08-08 20:27:22.793608 layout3mesh-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    17643 2023-08-08 13:15:32.980643 layout3mesh-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1184 2023-08-08 20:47:02.346832 layout3mesh-0.1.1/README.md
+-rw-r--r--   0        0        0      151 2023-08-08 17:51:33.516801 layout3mesh-0.1.1/layout3mesh/__init__.py
+-rw-r--r--   0        0        0     4565 2023-08-08 20:44:52.589329 layout3mesh-0.1.1/layout3mesh/cli.py
+-rw-r--r--   0        0        0     2285 2023-08-08 18:42:42.239242 layout3mesh-0.1.1/layout3mesh/data.py
+-rw-r--r--   0        0        0    10328 2023-08-08 20:43:10.750836 layout3mesh-0.1.1/layout3mesh/layout3mesh.py
+-rw-r--r--   0        0        0     1041 2023-08-08 20:31:18.715654 layout3mesh-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2208 2023-08-08 20:47:12.847072 layout3mesh-0.1.1/setup.py
+-rw-r--r--   0        0        0     2121 2023-08-08 20:47:12.847298 layout3mesh-0.1.1/PKG-INFO
```

### Comparing `layout3mesh-0.1.0/LICENSE` & `layout3mesh-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `layout3mesh-0.1.0/README.md` & `layout3mesh-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align=center> layout3mesh </h1>
 
 <div align=justify>
-<p> This is a simple tool to convert an integrated circuit layout saved in OASIS / GDSII file format to a mesh 3D image file. The tool supports direct export of the 3D mesh file into the Blender desktop app. This tool was written with the goal of rendering any layout in 3D inside a desktop or web application using WebGL. </p>
+<p> This is a simple tool to convert an integrated circuit layout saved in OASIS / GDSII file format to a mesh 3D image file. The tool doesn't support direct export of the 3D mesh file into the Blender desktop app just yet - but I am working on a solution. This tool was written with the goal of rendering any layout in 3D inside a desktop or web application using WebGL. </p>
 </div>
 
 <h2 align=center> Installation </h2>
 
 <h3 align=center> MacOS, Linux, Windows </h3>
 
 ```bash
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                            ****** layout3mesh ******
 This is a simple tool to convert an integrated circuit layout saved in OASIS /
-GDSII file format to a mesh 3D image file. The tool supports direct export of
-the 3D mesh file into the Blender desktop app. This tool was written with the
-goal of rendering any layout in 3D inside a desktop or web application using
-WebGL.
+GDSII file format to a mesh 3D image file. The tool doesn't support direct
+export of the 3D mesh file into the Blender desktop app just yet - but I am
+working on a solution. This tool was written with the goal of rendering any
+layout in 3D inside a desktop or web application using WebGL.
                            ***** Installation *****
                         **** MacOS, Linux, Windows ****
 ```bash pip install layout3mesh ```
                   ***** Usage - Command Line Interface *****
 ```bash layout3mesh -i
 .gds/.oas]> -o
 .gltf]> -t
```

### Comparing `layout3mesh-0.1.0/layout3mesh/cli.py` & `layout3mesh-0.1.1/layout3mesh/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             if verbose:
                 logger.error(f"Could not render to 3D Object: {e}")
             sys.exit("Failed: Could not render to output file.")
         if verbose:
             logger.success("Rendered to 3D Object: ", out_file)
     if render_to_blender:
         cmd = [BLENDER_BIN]
-        with tempfile.NamedTemporaryFile(suffix=".gltf") as f:
+        with tempfile.NamedTemporaryFile(suffix=".blend") as f:
             try:
                 render_to_mesh(layout, layerstack, topcell=topcell_name, out=f.name)
             except Exception as e:
                 if verbose:
                     logger.error("Could not render to temporary file: ")
                     logger.exception(e)
                 sys.exit("Failed: Could not render to Blender.")
```

### Comparing `layout3mesh-0.1.0/layout3mesh/data.py` & `layout3mesh-0.1.1/layout3mesh/data.py`

 * *Files identical despite different names*

### Comparing `layout3mesh-0.1.0/layout3mesh/layout3mesh.py` & `layout3mesh-0.1.1/layout3mesh/layout3mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 _LAYOUT_FILE_EXTENSIONS = [".oas", ".oasis", ".gds", ".gdsii"]
 
 _LAYERSTACK_FILE_EXTENSIONS = [".yaml", ".yml", ".ymls"]
 
 _OUT_FILE_EXTENSIONS = [".gltf", ".glb", ".obj", ".stl", ".ply", ".urdf"]
 
-
 def load_layout(fp: str) -> Optional[gdstk.Library]:
     """Load a layout from a GDSII file.
     Args:
         fp: Path to the GDSII file.
     Returns:
         The top cell of the layout.
     """
```

### Comparing `layout3mesh-0.1.0/pyproject.toml` & `layout3mesh-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "layout3mesh"
-version = "0.1.0"
+version = "0.1.1"
 description = "A tool to generate 3D meshes from 2D integrated circuit layouts"
 authors = ["dasdias <das.dias6@gmail.com>"]
 repository = "https://github.com/das-dias/layout3mesh"
 readme = "README.md"
 license = "GPLv2"
 keywords = ["layout", "3D-mesh", "gds2", "oasis"]
 
@@ -12,22 +12,24 @@
 python = ">=3.9,<3.13"
 trimesh = "^3.23.1"
 shapely = "^2.0.1"
 PyYAML = "^6.0.1"
 gdstk = "^0.9.42"
 mapbox-earcut = "^1.0.1"
 scipy = "^1.11.1"
+loguru = "^0.7.0"
+docopt = "^0.6.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 pytest-cov = "^4.1.0"
 black = "^23.7.0"
 
 [tool.poetry.scripts]
-layout2svg = "layout2svg.cli:main"
+layout3mesh = "layout3mesh.cli:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.autohooks]
 mode = "pipenv"
```

### Comparing `layout3mesh-0.1.0/setup.py` & `layout3mesh-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 ['layout3mesh']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=6.0.1,<7.0.0',
+ 'docopt>=0.6.2,<0.7.0',
  'gdstk>=0.9.42,<0.10.0',
+ 'loguru>=0.7.0,<0.8.0',
  'mapbox-earcut>=1.0.1,<2.0.0',
  'scipy>=1.11.1,<2.0.0',
  'shapely>=2.0.1,<3.0.0',
  'trimesh>=3.23.1,<4.0.0']
 
 entry_points = \
-{'console_scripts': ['layout2svg = layout2svg.cli:main']}
+{'console_scripts': ['layout3mesh = layout3mesh.cli:main']}
 
 setup_kwargs = {
     'name': 'layout3mesh',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A tool to generate 3D meshes from 2D integrated circuit layouts',
-    'long_description': '<h1 align=center> layout3mesh </h1>\n\n<div align=justify>\n<p> This is a simple tool to convert an integrated circuit layout saved in OASIS / GDSII file format to a mesh 3D image file. The tool supports direct export of the 3D mesh file into the Blender desktop app. This tool was written with the goal of rendering any layout in 3D inside a desktop or web application using WebGL. </p>\n</div>\n\n<h2 align=center> Installation </h2>\n\n<h3 align=center> MacOS, Linux, Windows </h3>\n\n```bash\npip install layout3mesh\n```\n\n<h2 align=center> Usage - Command Line Interface </h2>\n\n```bash\nlayout3mesh -i <input_file_path [.gds/.oas]> -o <output_file_path [.gltf]> -t <layerstack_file_path [.ymls]>\n```\n\n<h2 align=center> Examples </h2>\n\n<p>\nRunning the example with the mock layerstack file and layout provided in the <a href="tests/data/">examples</a>, by running the following command:\n</p>\n\n```bash\nlayout3mesh -i ./tests/data/crossed_metal.gds -t ./tests/data/mock_layers.ymls -o ./tests/data/crossed_metal.gltf\n```\n\n<p>\ncan generate the following 3D image:\n</p>\n\n<p align=center>\n\n\n<img src="tests/data/crossed_metal.gif" width=70%/>\n\n</p>\n',
+    'long_description': '<h1 align=center> layout3mesh </h1>\n\n<div align=justify>\n<p> This is a simple tool to convert an integrated circuit layout saved in OASIS / GDSII file format to a mesh 3D image file. The tool doesn\'t support direct export of the 3D mesh file into the Blender desktop app just yet - but I am working on a solution. This tool was written with the goal of rendering any layout in 3D inside a desktop or web application using WebGL. </p>\n</div>\n\n<h2 align=center> Installation </h2>\n\n<h3 align=center> MacOS, Linux, Windows </h3>\n\n```bash\npip install layout3mesh\n```\n\n<h2 align=center> Usage - Command Line Interface </h2>\n\n```bash\nlayout3mesh -i <input_file_path [.gds/.oas]> -o <output_file_path [.gltf]> -t <layerstack_file_path [.ymls]>\n```\n\n<h2 align=center> Examples </h2>\n\n<p>\nRunning the example with the mock layerstack file and layout provided in the <a href="tests/data/">examples</a>, by running the following command:\n</p>\n\n```bash\nlayout3mesh -i ./tests/data/crossed_metal.gds -t ./tests/data/mock_layers.ymls -o ./tests/data/crossed_metal.gltf\n```\n\n<p>\ncan generate the following 3D image:\n</p>\n\n<p align=center>\n\n\n<img src="tests/data/crossed_metal.gif" width=70%/>\n\n</p>\n',
     'author': 'dasdias',
     'author_email': 'das.dias6@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/das-dias/layout3mesh',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['layout3mesh'] package_data = \ {'': ['*']} install_requires = \
-['PyYAML>=6.0.1,<7.0.0', 'gdstk>=0.9.42,<0.10.0', 'mapbox-
-earcut>=1.0.1,<2.0.0', 'scipy>=1.11.1,<2.0.0', 'shapely>=2.0.1,<3.0.0',
-'trimesh>=3.23.1,<4.0.0'] entry_points = \ {'console_scripts': ['layout2svg =
-layout2svg.cli:main']} setup_kwargs = { 'name': 'layout3mesh', 'version':
-'0.1.0', 'description': 'A tool to generate 3D meshes from 2D integrated
-circuit layouts', 'long_description': '
+['PyYAML>=6.0.1,<7.0.0', 'docopt>=0.6.2,<0.7.0', 'gdstk>=0.9.42,<0.10.0',
+'loguru>=0.7.0,<0.8.0', 'mapbox-earcut>=1.0.1,<2.0.0', 'scipy>=1.11.1,<2.0.0',
+'shapely>=2.0.1,<3.0.0', 'trimesh>=3.23.1,<4.0.0'] entry_points = \
+{'console_scripts': ['layout3mesh = layout3mesh.cli:main']} setup_kwargs =
+{ 'name': 'layout3mesh', 'version': '0.1.1', 'description': 'A tool to generate
+3D meshes from 2D integrated circuit layouts', 'long_description': '
                            ****** layout3mesh ******
 \n\n
 \n
 This is a simple tool to convert an integrated circuit layout saved in OASIS /
-GDSII file format to a mesh 3D image file. The tool supports direct export of
-the 3D mesh file into the Blender desktop app. This tool was written with the
-goal of rendering any layout in 3D inside a desktop or web application using
-WebGL.
+GDSII file format to a mesh 3D image file. The tool doesn\'t support direct
+export of the 3D mesh file into the Blender desktop app just yet - but I am
+working on a solution. This tool was written with the goal of rendering any
+layout in 3D inside a desktop or web application using WebGL.
 \n
 \n\n
                            ***** Installation *****
 \n\n
                         **** MacOS, Linux, Windows ****
 \n\n```bash\npip install layout3mesh\n```\n\n
                   ***** Usage - Command Line Interface *****
```

### Comparing `layout3mesh-0.1.0/PKG-INFO` & `layout3mesh-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: layout3mesh
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool to generate 3D meshes from 2D integrated circuit layouts
 Home-page: https://github.com/das-dias/layout3mesh
 License: GPLv2
 Keywords: layout,3D-mesh,gds2,oasis
 Author: dasdias
 Author-email: das.dias6@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
+Requires-Dist: docopt (>=0.6.2,<0.7.0)
 Requires-Dist: gdstk (>=0.9.42,<0.10.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: mapbox-earcut (>=1.0.1,<2.0.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: shapely (>=2.0.1,<3.0.0)
 Requires-Dist: trimesh (>=3.23.1,<4.0.0)
 Project-URL: Repository, https://github.com/das-dias/layout3mesh
 Description-Content-Type: text/markdown
 
 <h1 align=center> layout3mesh </h1>
 
 <div align=justify>
-<p> This is a simple tool to convert an integrated circuit layout saved in OASIS / GDSII file format to a mesh 3D image file. The tool supports direct export of the 3D mesh file into the Blender desktop app. This tool was written with the goal of rendering any layout in 3D inside a desktop or web application using WebGL. </p>
+<p> This is a simple tool to convert an integrated circuit layout saved in OASIS / GDSII file format to a mesh 3D image file. The tool doesn't support direct export of the 3D mesh file into the Blender desktop app just yet - but I am working on a solution. This tool was written with the goal of rendering any layout in 3D inside a desktop or web application using WebGL. </p>
 </div>
 
 <h2 align=center> Installation </h2>
 
 <h3 align=center> MacOS, Linux, Windows </h3>
 
 ```bash
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: layout3mesh Version: 0.1.0 Summary: A tool to
+Metadata-Version: 2.1 Name: layout3mesh Version: 0.1.1 Summary: A tool to
 generate 3D meshes from 2D integrated circuit layouts Home-page: https://
 github.com/das-dias/layout3mesh License: GPLv2 Keywords: layout,3D-
 mesh,gds2,oasis Author: dasdias Author-email: das.dias6@gmail.com Requires-
 Python: >=3.9,<3.13 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: PyYAML (>=6.0.1,<7.0.0) Requires-Dist: gdstk (>=0.9.42,<0.10.0)
+Requires-Dist: PyYAML (>=6.0.1,<7.0.0) Requires-Dist: docopt (>=0.6.2,<0.7.0)
+Requires-Dist: gdstk (>=0.9.42,<0.10.0) Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: mapbox-earcut (>=1.0.1,<2.0.0) Requires-Dist: scipy
 (>=1.11.1,<2.0.0) Requires-Dist: shapely (>=2.0.1,<3.0.0) Requires-Dist:
 trimesh (>=3.23.1,<4.0.0) Project-URL: Repository, https://github.com/das-dias/
 layout3mesh Description-Content-Type: text/markdown
                            ****** layout3mesh ******
 This is a simple tool to convert an integrated circuit layout saved in OASIS /
-GDSII file format to a mesh 3D image file. The tool supports direct export of
-the 3D mesh file into the Blender desktop app. This tool was written with the
-goal of rendering any layout in 3D inside a desktop or web application using
-WebGL.
+GDSII file format to a mesh 3D image file. The tool doesn't support direct
+export of the 3D mesh file into the Blender desktop app just yet - but I am
+working on a solution. This tool was written with the goal of rendering any
+layout in 3D inside a desktop or web application using WebGL.
                            ***** Installation *****
                         **** MacOS, Linux, Windows ****
 ```bash pip install layout3mesh ```
                   ***** Usage - Command Line Interface *****
 ```bash layout3mesh -i
 .gds/.oas]> -o
 .gltf]> -t
```

