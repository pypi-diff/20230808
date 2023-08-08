# Comparing `tmp/intellifire4py-3.1.5.tar.gz` & `tmp/intellifire4py-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intellifire4py-3.1.5.tar", max compression
+gzip compressed data, was "intellifire4py-3.1.6.tar", max compression
```

## Comparing `intellifire4py-3.1.5.tar` & `intellifire4py-3.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2023-03-28 22:12:43.745071 intellifire4py-3.1.5/LICENSE
--rw-r--r--   0        0        0     2488 2023-03-28 22:12:43.745071 intellifire4py-3.1.5/README.md
--rw-r--r--   0        0        0     3158 2023-03-28 22:12:57.585276 intellifire4py-3.1.5/pyproject.toml
--rw-r--r--   0        0        0      638 2023-03-28 22:12:43.745071 intellifire4py-3.1.5/src/intellifire4py/__init__.py
--rw-r--r--   0        0        0    15311 2023-03-28 22:12:43.745071 intellifire4py-3.1.5/src/intellifire4py/cloud_api.py
--rw-r--r--   0        0        0     6607 2023-03-28 22:12:43.745071 intellifire4py-3.1.5/src/intellifire4py/const.py
--rw-r--r--   0        0        0     5053 2023-03-28 22:12:43.745071 intellifire4py-3.1.5/src/intellifire4py/control.py
--rw-r--r--   0        0        0      500 2023-03-28 22:12:43.745071 intellifire4py-3.1.5/src/intellifire4py/exceptions.py
--rw-r--r--   0        0        0    18622 2023-03-28 22:12:43.745071 intellifire4py-3.1.5/src/intellifire4py/local_api.py
--rw-r--r--   0        0        0     5871 2023-03-28 22:12:43.745071 intellifire4py-3.1.5/src/intellifire4py/model.py
--rw-r--r--   0        0        0        0 2023-03-28 22:12:43.745071 intellifire4py-3.1.5/src/intellifire4py/py.typed
--rw-r--r--   0        0        0     1113 2023-03-28 22:12:43.745071 intellifire4py-3.1.5/src/intellifire4py/read.py
--rw-r--r--   0        0        0     5151 2023-03-28 22:12:43.745071 intellifire4py-3.1.5/src/intellifire4py/udp.py
--rw-r--r--   0        0        0      579 2023-03-28 22:12:43.745071 intellifire4py-3.1.5/src/intellifire4py/utils.py
--rw-r--r--   0        0        0     3467 1970-01-01 00:00:00.000000 intellifire4py-3.1.5/setup.py
--rw-r--r--   0        0        0     3376 1970-01-01 00:00:00.000000 intellifire4py-3.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-08 20:58:39.427574 intellifire4py-3.1.6/LICENSE
+-rw-r--r--   0        0        0     2488 2023-08-08 20:58:39.427574 intellifire4py-3.1.6/README.md
+-rw-r--r--   0        0        0     3161 2023-08-08 20:58:53.491863 intellifire4py-3.1.6/pyproject.toml
+-rw-r--r--   0        0        0      638 2023-08-08 20:58:39.427574 intellifire4py-3.1.6/src/intellifire4py/__init__.py
+-rw-r--r--   0        0        0    15311 2023-08-08 20:58:39.427574 intellifire4py-3.1.6/src/intellifire4py/cloud_api.py
+-rw-r--r--   0        0        0     6607 2023-08-08 20:58:39.431575 intellifire4py-3.1.6/src/intellifire4py/const.py
+-rw-r--r--   0        0        0     5053 2023-08-08 20:58:39.431575 intellifire4py-3.1.6/src/intellifire4py/control.py
+-rw-r--r--   0        0        0      500 2023-08-08 20:58:39.431575 intellifire4py-3.1.6/src/intellifire4py/exceptions.py
+-rw-r--r--   0        0        0    18622 2023-08-08 20:58:39.431575 intellifire4py-3.1.6/src/intellifire4py/local_api.py
+-rw-r--r--   0        0        0     5871 2023-08-08 20:58:39.431575 intellifire4py-3.1.6/src/intellifire4py/model.py
+-rw-r--r--   0        0        0        0 2023-08-08 20:58:39.431575 intellifire4py-3.1.6/src/intellifire4py/py.typed
+-rw-r--r--   0        0        0     1113 2023-08-08 20:58:39.431575 intellifire4py-3.1.6/src/intellifire4py/read.py
+-rw-r--r--   0        0        0     5151 2023-08-08 20:58:39.431575 intellifire4py-3.1.6/src/intellifire4py/udp.py
+-rw-r--r--   0        0        0      579 2023-08-08 20:58:39.431575 intellifire4py-3.1.6/src/intellifire4py/utils.py
+-rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 intellifire4py-3.1.6/setup.py
+-rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 intellifire4py-3.1.6/PKG-INFO
```

### Comparing `intellifire4py-3.1.5/LICENSE` & `intellifire4py-3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `intellifire4py-3.1.5/README.md` & `intellifire4py-3.1.6/README.md`

 * *Files identical despite different names*

### Comparing `intellifire4py-3.1.5/pyproject.toml` & `intellifire4py-3.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "intellifire4py"
-version = "3.1.5"
+version = "3.1.6"
 description = "Intellifire4Py"
 authors = ["Jeff Stein <jeffstein@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jeeftor/intellifire4py"
 repository = "https://github.com/jeeftor/intellifire4py"
 documentation = "https://intellifire4py.readthedocs.io"
 classifiers = ["Development Status :: 5 - Production/Stable"]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/jeeftor/intellifire4py/releases"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic = "^1.10.2"
-aenum = "^3.1.11"
-httpx = "^0.23.0"
+pydantic = ">=1.10.2"
+aenum = ">=3.1.11"
+httpx = ">=0.23.0"
 # Rich is needed
 rich = "10.16.2"
 
 
 [tool.poetry.dev-dependencies] # rich <11.0.0,>=10.1.0, but you have rich 12.6.0.
 # mycroftapi 2.0 has requirement websocket-client==0.44.0, but you have websocket-client 1.5.1.
 # ibm-watson 5.2.2 has requirement websocket-client==1.1.0, but you have websocket-client 1.5.1.
```

### Comparing `intellifire4py-3.1.5/src/intellifire4py/__init__.py` & `intellifire4py-3.1.6/src/intellifire4py/__init__.py`

 * *Files identical despite different names*

### Comparing `intellifire4py-3.1.5/src/intellifire4py/cloud_api.py` & `intellifire4py-3.1.6/src/intellifire4py/cloud_api.py`

 * *Files identical despite different names*

### Comparing `intellifire4py-3.1.5/src/intellifire4py/const.py` & `intellifire4py-3.1.6/src/intellifire4py/const.py`

 * *Files identical despite different names*

### Comparing `intellifire4py-3.1.5/src/intellifire4py/control.py` & `intellifire4py-3.1.6/src/intellifire4py/control.py`

 * *Files identical despite different names*

### Comparing `intellifire4py-3.1.5/src/intellifire4py/local_api.py` & `intellifire4py-3.1.6/src/intellifire4py/local_api.py`

 * *Files identical despite different names*

### Comparing `intellifire4py-3.1.5/src/intellifire4py/model.py` & `intellifire4py-3.1.6/src/intellifire4py/model.py`

 * *Files identical despite different names*

### Comparing `intellifire4py-3.1.5/src/intellifire4py/read.py` & `intellifire4py-3.1.6/src/intellifire4py/read.py`

 * *Files identical despite different names*

### Comparing `intellifire4py-3.1.5/src/intellifire4py/udp.py` & `intellifire4py-3.1.6/src/intellifire4py/udp.py`

 * *Files identical despite different names*

### Comparing `intellifire4py-3.1.5/src/intellifire4py/utils.py` & `intellifire4py-3.1.6/src/intellifire4py/utils.py`

 * *Files identical despite different names*

### Comparing `intellifire4py-3.1.5/setup.py` & `intellifire4py-3.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,22 @@
 packages = \
 ['intellifire4py']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['aenum>=3.1.11,<4.0.0',
- 'httpx>=0.23.0,<0.24.0',
- 'pydantic>=1.10.2,<2.0.0',
- 'rich==10.16.2']
+['aenum>=3.1.11', 'httpx>=0.23.0', 'pydantic>=1.10.2', 'rich==10.16.2']
 
 entry_points = \
 {'console_scripts': ['intellifire4py = intellifire4py.__main__:main']}
 
 setup_kwargs = {
     'name': 'intellifire4py',
-    'version': '3.1.5',
+    'version': '3.1.6',
     'description': 'Intellifire4Py',
     'long_description': "# Intellifire4Py\n\n[![PyPI](https://img.shields.io/pypi/v/intellifire4py.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/intellifire4py.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/intellifire4py)][python version]\n[![License](https://img.shields.io/pypi/l/intellifire4py)][license]\n\n[![Read the documentation at https://intellifire4py.readthedocs.io/](https://img.shields.io/readthedocs/intellifire4py/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/jeeftor/intellifire4py/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/jeeftor/intellifire4py/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/intellifire4py/\n[status]: https://pypi.org/project/intellifire4py/\n[python version]: https://pypi.org/project/intellifire4py\n[read the docs]: https://intellifire4py.readthedocs.io/\n[tests]: https://github.com/jeeftor/intellifire4py/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/jeeftor/intellifire4py\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- TODO\n\n## Requirements\n\n- TODO\n\n## Installation\n\nYou can install _Intellifire4Py_ via [pip] from [PyPI]:\n\n```console\n$ pip install intellifire4py\n```\n\n## Usage\n\nPlease see the [API Reference] for details.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Intellifire4Py_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/jeeftor/intellifire4py/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/jeeftor/intellifire4py/blob/main/LICENSE\n[contributor guide]: https://github.com/jeeftor/intellifire4py/blob/main/CONTRIBUTING.md\n[command-line reference]: https://intellifire4py.readthedocs.io/en/latest/usage.html\n",
     'author': 'Jeff Stein',
     'author_email': 'jeffstein@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jeeftor/intellifire4py',
```

### Comparing `intellifire4py-3.1.5/PKG-INFO` & `intellifire4py-3.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: intellifire4py
-Version: 3.1.5
+Version: 3.1.6
 Summary: Intellifire4Py
 Home-page: https://github.com/jeeftor/intellifire4py
 License: MIT
 Author: Jeff Stein
 Author-email: jeffstein@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: aenum (>=3.1.11,<4.0.0)
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: aenum (>=3.1.11)
+Requires-Dist: httpx (>=0.23.0)
+Requires-Dist: pydantic (>=1.10.2)
 Requires-Dist: rich (==10.16.2)
 Project-URL: Changelog, https://github.com/jeeftor/intellifire4py/releases
 Project-URL: Documentation, https://intellifire4py.readthedocs.io
 Project-URL: Repository, https://github.com/jeeftor/intellifire4py
 Description-Content-Type: text/markdown
 
 # Intellifire4Py
```

