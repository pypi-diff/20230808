# Comparing `tmp/layout2svg-0.1.4.tar.gz` & `tmp/layout2svg-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layout2svg-0.1.4.tar", max compression
+gzip compressed data, was "layout2svg-0.1.5.tar", max compression
```

## Comparing `layout2svg-0.1.4.tar` & `layout2svg-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    17643 2023-08-08 04:37:18.515466 layout2svg-0.1.4/LICENSE
--rw-r--r--   0        0        0     1060 2023-08-08 04:58:13.665917 layout2svg-0.1.4/README.md
--rw-r--r--   0        0        0      145 2023-08-08 04:55:38.682088 layout2svg-0.1.4/layout2svg/__init__.py
--rw-r--r--   0        0        0     2221 2023-08-08 04:08:56.505191 layout2svg-0.1.4/layout2svg/data.py
--rw-r--r--   0        0        0     7593 2023-08-08 04:08:56.529512 layout2svg-0.1.4/layout2svg/layout2svg.py
--rw-r--r--   0        0        0      992 2023-08-08 04:58:18.575629 layout2svg-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2038 2023-08-08 04:59:59.731802 layout2svg-0.1.4/setup.py
--rw-r--r--   0        0        0     1935 2023-08-08 04:59:59.732009 layout2svg-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    17643 2023-08-08 04:37:18.515466 layout2svg-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1060 2023-08-08 04:58:13.665917 layout2svg-0.1.5/README.md
+-rw-r--r--   0        0        0      145 2023-08-08 04:55:38.682088 layout2svg-0.1.5/layout2svg/__init__.py
+-rw-r--r--   0        0        0     4576 2023-08-08 04:55:09.191985 layout2svg-0.1.5/layout2svg/cli.py
+-rw-r--r--   0        0        0     2221 2023-08-08 04:08:56.505191 layout2svg-0.1.5/layout2svg/data.py
+-rw-r--r--   0        0        0     7593 2023-08-08 04:08:56.529512 layout2svg-0.1.5/layout2svg/layout2svg.py
+-rw-r--r--   0        0        0      992 2023-08-08 05:11:58.435312 layout2svg-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2038 2023-08-08 05:12:24.760113 layout2svg-0.1.5/setup.py
+-rw-r--r--   0        0        0     1935 2023-08-08 05:12:24.760316 layout2svg-0.1.5/PKG-INFO
```

### Comparing `layout2svg-0.1.4/LICENSE` & `layout2svg-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `layout2svg-0.1.4/README.md` & `layout2svg-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `layout2svg-0.1.4/layout2svg/data.py` & `layout2svg-0.1.5/layout2svg/data.py`

 * *Files identical despite different names*

### Comparing `layout2svg-0.1.4/layout2svg/layout2svg.py` & `layout2svg-0.1.5/layout2svg/layout2svg.py`

 * *Files identical despite different names*

### Comparing `layout2svg-0.1.4/pyproject.toml` & `layout2svg-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "layout2svg"
-version = "0.1.4"
+version = "0.1.5"
 description = "A package to convert IC layouts (GDS2 and OASIS) to SVG."
 authors = ["dasdias <das.dias6@gmail.com>"]
 repository = "https://github.com/das-dias/layout2svg"
 readme = "README.md"
 license = "GPLv2"
 keywords = ["layout", "svg", "gds2", "oasis"]
 
@@ -20,15 +20,15 @@
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 pytest-cov = "^4.1.0"
 black = "^23.7.0"
 
 [tool.poetry.scripts]
-layout2svg = "bin.layout2svg:main"
+layout2svg = "layout2svg.cli:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.autohooks]
 mode = "pipenv"
```

### Comparing `layout2svg-0.1.4/setup.py` & `layout2svg-0.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,19 +13,19 @@
  'docopt>=0.6.2,<0.7.0',
  'gdstk>=0.9.42,<0.10.0',
  'klayout>=0.28.10,<0.29.0',
  'loguru>=0.7.0,<0.8.0',
  'lxml>=4.9.3,<5.0.0']
 
 entry_points = \
-{'console_scripts': ['layout2svg = bin.layout2svg:main']}
+{'console_scripts': ['layout2svg = layout2svg.cli:main']}
 
 setup_kwargs = {
     'name': 'layout2svg',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'A package to convert IC layouts (GDS2 and OASIS) to SVG.',
     'long_description': '<h1 align=center> layout2svg </h1>\n\n<div align=justify>\n<p> This is a simple tool to convert an integrated circuit layout saved in OASIS / GDSII file format to a .SVG image file. The tool supports direct export of the SVG file into the Inkscape desktop app. This tool was written with the goal of rendering any layout in a desktop or web application. </p>\n</div>\n\n<h2 align=center> Installation </h2>\n\n<h3 align=center> MacOS, Linux, Windows </h3>\n\n```bash\npip install layout2svg\n```\n\n<h2 align=center> Usage - Command Line Interface </h2>\n\n```bash\nlayout2svg -i <input_file_path [.gds/.oas]> -o <output_file_path [.svg]>\n```\n\n<h2 align=center> Examples </h2>\n\n<p>\nRunning the example with the mock layerstack file and layout provided in the <a href="tests/data/">examples</a>, by running the following command:\n</p>\n\n```bash\nlayout2svg -i examples/crossed_metal.gds -t examples/mock_layers.lys.yml -o examples/crossed_metal.svg\n```\n\n<p>\ncan generate the following SVG image:\n</p>\n\n<p align=center>\n\n\n<img src="tests/data/crossed_metal.png" width=400/>\n\n\n</p>\n',
     'author': 'dasdias',
     'author_email': 'das.dias6@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/das-dias/layout2svg',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['layout2svg'] package_data = \ {'': ['*']} install_requires = \
 ['PyYAML>=6.0.1,<7.0.0', 'colour>=0.1.5,<0.2.0', 'docopt>=0.6.2,<0.7.0',
 'gdstk>=0.9.42,<0.10.0', 'klayout>=0.28.10,<0.29.0', 'loguru>=0.7.0,<0.8.0',
 'lxml>=4.9.3,<5.0.0'] entry_points = \ {'console_scripts': ['layout2svg =
-bin.layout2svg:main']} setup_kwargs = { 'name': 'layout2svg', 'version':
-'0.1.4', 'description': 'A package to convert IC layouts (GDS2 and OASIS) to
+layout2svg.cli:main']} setup_kwargs = { 'name': 'layout2svg', 'version':
+'0.1.5', 'description': 'A package to convert IC layouts (GDS2 and OASIS) to
 SVG.', 'long_description': '
                            ****** layout2svg ******
 \n\n
 \n
 This is a simple tool to convert an integrated circuit layout saved in OASIS /
 GDSII file format to a .SVG image file. The tool supports direct export of the
 SVG file into the Inkscape desktop app. This tool was written with the goal of
```

### Comparing `layout2svg-0.1.4/PKG-INFO` & `layout2svg-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layout2svg
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package to convert IC layouts (GDS2 and OASIS) to SVG.
 Home-page: https://github.com/das-dias/layout2svg
 License: GPLv2
 Keywords: layout,svg,gds2,oasis
 Author: dasdias
 Author-email: das.dias6@gmail.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: layout2svg Version: 0.1.4 Summary: A package to
+Metadata-Version: 2.1 Name: layout2svg Version: 0.1.5 Summary: A package to
 convert IC layouts (GDS2 and OASIS) to SVG. Home-page: https://github.com/das-
 dias/layout2svg License: GPLv2 Keywords: layout,svg,gds2,oasis Author: dasdias
 Author-email: das.dias6@gmail.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: Other/Proprietary License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.9 Requires-Dist: PyYAML (>=6.0.1,<7.0.0) Requires-Dist:
 colour (>=0.1.5,<0.2.0) Requires-Dist: docopt (>=0.6.2,<0.7.0) Requires-Dist:
```

