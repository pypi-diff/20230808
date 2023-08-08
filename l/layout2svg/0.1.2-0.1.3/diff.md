# Comparing `tmp/layout2svg-0.1.2.tar.gz` & `tmp/layout2svg-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layout2svg-0.1.2.tar", max compression
+gzip compressed data, was "layout2svg-0.1.3.tar", max compression
```

## Comparing `layout2svg-0.1.2.tar` & `layout2svg-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    17643 2023-08-08 04:37:18.515466 layout2svg-0.1.2/LICENSE
--rw-r--r--   0        0        0     1067 2023-08-08 04:15:47.839675 layout2svg-0.1.2/README.md
--rw-r--r--   0        0        0       22 2023-08-08 02:48:25.552267 layout2svg-0.1.2/layout2svg/__init__.py
--rw-r--r--   0        0        0     2221 2023-08-08 04:08:56.505191 layout2svg-0.1.2/layout2svg/data.py
--rw-r--r--   0        0        0     7593 2023-08-08 04:08:56.529512 layout2svg-0.1.2/layout2svg/layout2svg.py
--rw-r--r--   0        0        0      992 2023-08-08 04:40:23.366528 layout2svg-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2041 2023-08-08 04:40:25.748746 layout2svg-0.1.2/setup.py
--rw-r--r--   0        0        0     1942 2023-08-08 04:40:25.748947 layout2svg-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    17643 2023-08-08 04:37:18.515466 layout2svg-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1065 2023-08-08 04:41:20.175838 layout2svg-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2023-08-08 02:48:25.552267 layout2svg-0.1.3/layout2svg/__init__.py
+-rw-r--r--   0        0        0     2221 2023-08-08 04:08:56.505191 layout2svg-0.1.3/layout2svg/data.py
+-rw-r--r--   0        0        0     7593 2023-08-08 04:08:56.529512 layout2svg-0.1.3/layout2svg/layout2svg.py
+-rw-r--r--   0        0        0      992 2023-08-08 04:41:33.830856 layout2svg-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2039 2023-08-08 04:41:37.607059 layout2svg-0.1.3/setup.py
+-rw-r--r--   0        0        0     1940 2023-08-08 04:41:37.607314 layout2svg-0.1.3/PKG-INFO
```

### Comparing `layout2svg-0.1.2/LICENSE` & `layout2svg-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `layout2svg-0.1.2/README.md` & `layout2svg-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,9 +29,9 @@
 ```
 
 <p>
 can generate the following SVG image:
 </p>
 
 <p align=center>
-<img src="./tests/data/crossed_metal.svg" width=400/>
+<img src="tests/data/crossed_metal.svg" width=400/>
 </p>
```

#### html2text {}

```diff
@@ -12,8 +12,8 @@
 .svg]> ```
                              ***** Examples *****
 Running the example with the mock layerstack file and layout provided in the
 examples directory, by running the following command:
 ```bash layout2svg -i examples/crossed_metal.gds -t examples/
 mock_layers.lys.yml -o examples/crossed_metal.svg ```
 can generate the following SVG image:
-                       [./tests/data/crossed_metal.svg]
+                        [tests/data/crossed_metal.svg]
```

### Comparing `layout2svg-0.1.2/layout2svg/data.py` & `layout2svg-0.1.3/layout2svg/data.py`

 * *Files identical despite different names*

### Comparing `layout2svg-0.1.2/layout2svg/layout2svg.py` & `layout2svg-0.1.3/layout2svg/layout2svg.py`

 * *Files identical despite different names*

### Comparing `layout2svg-0.1.2/pyproject.toml` & `layout2svg-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "layout2svg"
-version = "0.1.2"
+version = "0.1.3"
 description = "A package to convert IC layouts (GDS2 and OASIS) to SVG."
 authors = ["dasdias <das.dias6@gmail.com>"]
 repository = "https://github.com/das-dias/layout2svg"
 readme = "README.md"
 license = "GPLv2"
 keywords = ["layout", "svg", "gds2", "oasis"]
```

### Comparing `layout2svg-0.1.2/setup.py` & `layout2svg-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
  'lxml>=4.9.3,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['layout2svg = bin.layout2svg:main']}
 
 setup_kwargs = {
     'name': 'layout2svg',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'A package to convert IC layouts (GDS2 and OASIS) to SVG.',
-    'long_description': '<h1 align=center> layout2svg </h1>\n\n<div align=justify>\n<p> This is a simple tool to convert an integrated circuit layout saved in OASIS / GDSII file format to a .SVG image file. The tool supports direct export of the SVG file into the Inkscape desktop app. This tool was written with the goal of rendering any layout in a desktop or web application. </p>\n</div>\n\n<h2 align=center> Installation </h2>\n\n<h3 align=center> MacOS, Linux, Windows </h3>\n\n```bash\npip install layout2svg\n```\n\n<h2 align=center> Usage - Command Line Interface </h2>\n\n```bash\nlayout2svg -i <input_file_path [.gds/.oas]> -o <output_file_path [.svg]>\n```\n\n<h2 align=center> Examples </h2>\n\n<p>\nRunning the example with the mock layerstack file and layout provided in the <a href="./examples">examples</a> directory, by running the following command:\n</p>\n\n```bash\nlayout2svg -i examples/crossed_metal.gds -t examples/mock_layers.lys.yml -o examples/crossed_metal.svg\n```\n\n<p>\ncan generate the following SVG image:\n</p>\n\n<p align=center>\n<img src="./tests/data/crossed_metal.svg" width=400/>\n</p>\n',
+    'long_description': '<h1 align=center> layout2svg </h1>\n\n<div align=justify>\n<p> This is a simple tool to convert an integrated circuit layout saved in OASIS / GDSII file format to a .SVG image file. The tool supports direct export of the SVG file into the Inkscape desktop app. This tool was written with the goal of rendering any layout in a desktop or web application. </p>\n</div>\n\n<h2 align=center> Installation </h2>\n\n<h3 align=center> MacOS, Linux, Windows </h3>\n\n```bash\npip install layout2svg\n```\n\n<h2 align=center> Usage - Command Line Interface </h2>\n\n```bash\nlayout2svg -i <input_file_path [.gds/.oas]> -o <output_file_path [.svg]>\n```\n\n<h2 align=center> Examples </h2>\n\n<p>\nRunning the example with the mock layerstack file and layout provided in the <a href="./examples">examples</a> directory, by running the following command:\n</p>\n\n```bash\nlayout2svg -i examples/crossed_metal.gds -t examples/mock_layers.lys.yml -o examples/crossed_metal.svg\n```\n\n<p>\ncan generate the following SVG image:\n</p>\n\n<p align=center>\n<img src="tests/data/crossed_metal.svg" width=400/>\n</p>\n',
     'author': 'dasdias',
     'author_email': 'das.dias6@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/das-dias/layout2svg',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['layout2svg'] package_data = \ {'': ['*']} install_requires = \
 ['PyYAML>=6.0.1,<7.0.0', 'colour>=0.1.5,<0.2.0', 'docopt>=0.6.2,<0.7.0',
 'gdstk>=0.9.42,<0.10.0', 'klayout>=0.28.10,<0.29.0', 'loguru>=0.7.0,<0.8.0',
 'lxml>=4.9.3,<5.0.0'] entry_points = \ {'console_scripts': ['layout2svg =
 bin.layout2svg:main']} setup_kwargs = { 'name': 'layout2svg', 'version':
-'0.1.2', 'description': 'A package to convert IC layouts (GDS2 and OASIS) to
+'0.1.3', 'description': 'A package to convert IC layouts (GDS2 and OASIS) to
 SVG.', 'long_description': '
                            ****** layout2svg ******
 \n\n
 \n
 This is a simple tool to convert an integrated circuit layout saved in OASIS /
 GDSII file format to a .SVG image file. The tool supports direct export of the
 SVG file into the Inkscape desktop app. This tool was written with the goal of
@@ -27,13 +27,13 @@
 \n\n
 \nRunning the example with the mock layerstack file and layout provided in the
 examples directory, by running the following command:\n
 \n\n```bash\nlayout2svg -i examples/crossed_metal.gds -t examples/
 mock_layers.lys.yml -o examples/crossed_metal.svg\n```\n\n
 \ncan generate the following SVG image:\n
 \n\n
-                     \n[./tests/data/crossed_metal.svg]\n
+                      \n[tests/data/crossed_metal.svg]\n
 \n', 'author': 'dasdias', 'author_email': 'das.dias6@gmail.com', 'maintainer':
 None, 'maintainer_email': None, 'url': 'https://github.com/das-dias/
 layout2svg', 'packages': packages, 'package_data': package_data,
 'install_requires': install_requires, 'entry_points': entry_points,
 'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
```

### Comparing `layout2svg-0.1.2/PKG-INFO` & `layout2svg-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layout2svg
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to convert IC layouts (GDS2 and OASIS) to SVG.
 Home-page: https://github.com/das-dias/layout2svg
 License: GPLv2
 Keywords: layout,svg,gds2,oasis
 Author: dasdias
 Author-email: das.dias6@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -53,10 +53,10 @@
 ```
 
 <p>
 can generate the following SVG image:
 </p>
 
 <p align=center>
-<img src="./tests/data/crossed_metal.svg" width=400/>
+<img src="tests/data/crossed_metal.svg" width=400/>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: layout2svg Version: 0.1.2 Summary: A package to
+Metadata-Version: 2.1 Name: layout2svg Version: 0.1.3 Summary: A package to
 convert IC layouts (GDS2 and OASIS) to SVG. Home-page: https://github.com/das-
 dias/layout2svg License: GPLv2 Keywords: layout,svg,gds2,oasis Author: dasdias
 Author-email: das.dias6@gmail.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: Other/Proprietary License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.9 Requires-Dist: PyYAML (>=6.0.1,<7.0.0) Requires-Dist:
 colour (>=0.1.5,<0.2.0) Requires-Dist: docopt (>=0.6.2,<0.7.0) Requires-Dist:
@@ -24,8 +24,8 @@
 .svg]> ```
                              ***** Examples *****
 Running the example with the mock layerstack file and layout provided in the
 examples directory, by running the following command:
 ```bash layout2svg -i examples/crossed_metal.gds -t examples/
 mock_layers.lys.yml -o examples/crossed_metal.svg ```
 can generate the following SVG image:
-                       [./tests/data/crossed_metal.svg]
+                        [tests/data/crossed_metal.svg]
```

