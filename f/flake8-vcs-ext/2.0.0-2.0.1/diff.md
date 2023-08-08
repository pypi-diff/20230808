# Comparing `tmp/flake8_vcs_ext-2.0.0.tar.gz` & `tmp/flake8_vcs_ext-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_vcs_ext-2.0.0.tar", max compression
+gzip compressed data, was "flake8_vcs_ext-2.0.1.tar", max compression
```

## Comparing `flake8_vcs_ext-2.0.0.tar` & `flake8_vcs_ext-2.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    18092 2023-08-04 18:17:14.172707 flake8_vcs_ext-2.0.0/LICENSE
--rw-r--r--   0        0        0      335 2023-08-04 18:17:14.172707 flake8_vcs_ext-2.0.0/README.md
--rw-r--r--   0        0        0     6990 2023-08-04 18:17:14.172707 flake8_vcs_ext-2.0.0/flake8_vcs_ext.py
--rw-r--r--   0        0        0     1207 2023-08-04 18:17:14.172707 flake8_vcs_ext-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 flake8_vcs_ext-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-08-08 18:26:19.808612 flake8_vcs_ext-2.0.1/LICENSE
+-rw-r--r--   0        0        0      335 2023-08-08 18:26:19.808612 flake8_vcs_ext-2.0.1/README.md
+-rw-r--r--   0        0        0     6985 2023-08-08 18:26:19.808612 flake8_vcs_ext-2.0.1/flake8_vcs_ext.py
+-rw-r--r--   0        0        0     1369 2023-08-08 18:26:19.808612 flake8_vcs_ext-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 flake8_vcs_ext-2.0.1/PKG-INFO
```

### Comparing `flake8_vcs_ext-2.0.0/LICENSE` & `flake8_vcs_ext-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_vcs_ext-2.0.0/flake8_vcs_ext.py` & `flake8_vcs_ext-2.0.1/flake8_vcs_ext.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 		return None
 
 class Plugin:
 
 	def __init__(self, tree: ast.Module) -> None:
 		self.tree = tree
 
-	def __iter__(self) -> Generator[Tuple[int, int, str, Type[Any]], None, None]:
+	def run(self) -> Generator[Tuple[int, int, str, Type[Any]], None, None]:
 		# иначе TypeError: 'Plugin' object is not iterable. Вместо __iter__
 		# должен быть run согласно документации и примерам flake8
 		determinator = MultilineDeterminator(self.tree)
 		indents = determinator.getMultilinesIndents()
 		correct_indent = determinator.getCorrectIndent()
 		if indents:
 			checker = IndentChecker(correct_indent, indents)
```

### Comparing `flake8_vcs_ext-2.0.0/pyproject.toml` & `flake8_vcs_ext-2.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 [build-system]
-requires = ["poetry-core"]
+requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.setuptools_scm]
+
 [tool.poetry]
 name = "flake8_vcs_ext"
-version = "2.0.0"
+version = "2.0.1"
 description = "Плагин flake8 с проверкой на дополнительные стандарты кода, принятые на проекте VCS"
 authors = ["Debianov <regdeb@mail.ru>"]
 readme = "README.md"
 license = "GPL-2.0 license"
 classifiers = [
 	"Framework :: Flake8",
+	"Environment :: Console",
 	"Intended Audience :: Developers",
+	"License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
+	"Programming Language :: Python",
+	"Programming Language :: Python :: 3",
 	"Topic :: Software Development :: Libraries :: Python Modules",
 	"Topic :: Software Development :: Quality Assurance",
-	"Operating System :: OS Independent",
 ]
 
 include = ["pyproject.toml", "flake8_vcs_ext.py", "LICENCE", "README.md"]
 
 [tool.poetry.urls]
 "Repository" = "https://github.com/GREEN-Corporation/vcs-style-flake8-extension"
```

### Comparing `flake8_vcs_ext-2.0.0/PKG-INFO` & `flake8_vcs_ext-2.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: flake8-vcs-ext
-Version: 2.0.0
+Version: 2.0.1
 Summary: Плагин flake8 с проверкой на дополнительные стандарты кода, принятые на проекте VCS
 License: GPL-2.0 license
 Author: Debianov
 Author-email: regdeb@mail.ru
 Requires-Python: >=3.10,<4.0
+Classifier: Environment :: Console
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: flake8-isort (>=6.0.0,<7.0.0)
```

