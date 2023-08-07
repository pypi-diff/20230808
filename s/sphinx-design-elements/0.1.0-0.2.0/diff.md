# Comparing `tmp/sphinx-design-elements-0.1.0.tar.gz` & `tmp/sphinx-design-elements-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-design-elements-0.1.0.tar", last modified: Wed Jul 19 20:42:44 2023, max compression
+gzip compressed data, was "sphinx-design-elements-0.2.0.tar", last modified: Mon Aug  7 22:13:17 2023, max compression
```

## Comparing `sphinx-design-elements-0.1.0.tar` & `sphinx-design-elements-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-07-19 20:42:44.644276 sphinx-design-elements-0.1.0/
--rw-r--r--   0 amo        (501) staff       (20)      225 2023-07-19 19:40:43.000000 sphinx-design-elements-0.1.0/CHANGES.md
--rw-r--r--   0 amo        (501) staff       (20)     1099 2023-07-16 18:50:11.000000 sphinx-design-elements-0.1.0/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)      134 2023-07-18 20:19:29.000000 sphinx-design-elements-0.1.0/MANIFEST.in
--rw-r--r--   0 amo        (501) staff       (20)     5285 2023-07-19 20:42:44.644051 sphinx-design-elements-0.1.0/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     2144 2023-07-19 20:41:30.000000 sphinx-design-elements-0.1.0/README.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-07-19 20:42:44.635131 sphinx-design-elements-0.1.0/docs/
--rw-r--r--   0 amo        (501) staff       (20)      258 2023-07-18 20:19:29.000000 sphinx-design-elements-0.1.0/docs/backlog.md
--rw-r--r--   0 amo        (501) staff       (20)      225 2023-07-19 19:40:43.000000 sphinx-design-elements-0.1.0/docs/changes.md
--rw-r--r--   0 amo        (501) staff       (20)     1350 2023-07-19 20:41:30.000000 sphinx-design-elements-0.1.0/docs/css_classes.md
--rw-r--r--   0 amo        (501) staff       (20)     2114 2023-07-19 19:40:43.000000 sphinx-design-elements-0.1.0/docs/get_started.md
--rw-r--r--   0 amo        (501) staff       (20)     3867 2023-07-19 20:41:30.000000 sphinx-design-elements-0.1.0/docs/gridtable.md
--rw-r--r--   0 amo        (501) staff       (20)     3532 2023-07-19 20:41:30.000000 sphinx-design-elements-0.1.0/docs/index.md
--rw-r--r--   0 amo        (501) staff       (20)     2943 2023-07-19 20:41:30.000000 sphinx-design-elements-0.1.0/docs/infocard.md
--rw-r--r--   0 amo        (501) staff       (20)      165 2023-07-18 20:38:40.000000 sphinx-design-elements-0.1.0/docs/project.md
--rw-r--r--   0 amo        (501) staff       (20)     2144 2023-07-19 20:41:30.000000 sphinx-design-elements-0.1.0/docs/readme.md
--rw-r--r--   0 amo        (501) staff       (20)     1605 2023-07-19 19:40:43.000000 sphinx-design-elements-0.1.0/docs/sandbox.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-07-19 20:42:44.635620 sphinx-design-elements-0.1.0/docs/snippets/
--rw-r--r--   0 amo        (501) staff       (20)       73 2023-07-18 22:10:25.000000 sphinx-design-elements-0.1.0/docs/snippets/index.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-07-19 20:42:44.637202 sphinx-design-elements-0.1.0/docs/snippets/myst/
--rw-r--r--   0 amo        (501) staff       (20)      327 2023-07-18 22:10:25.000000 sphinx-design-elements-0.1.0/docs/snippets/myst/gridtable.md
--rw-r--r--   0 amo        (501) staff       (20)      427 2023-07-19 17:40:51.000000 sphinx-design-elements-0.1.0/docs/snippets/myst/infocard.md
--rw-r--r--   0 amo        (501) staff       (20)       33 2023-07-18 22:13:22.000000 sphinx-design-elements-0.1.0/docs/snippets/myst/tag.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-07-19 20:42:44.639174 sphinx-design-elements-0.1.0/docs/snippets/rst/
--rw-r--r--   0 amo        (501) staff       (20)      373 2023-07-18 22:10:25.000000 sphinx-design-elements-0.1.0/docs/snippets/rst/gridtable.rst
--rw-r--r--   0 amo        (501) staff       (20)      515 2023-07-19 17:40:51.000000 sphinx-design-elements-0.1.0/docs/snippets/rst/infocard.rst
--rw-r--r--   0 amo        (501) staff       (20)       33 2023-07-18 22:13:22.000000 sphinx-design-elements-0.1.0/docs/snippets/rst/tag.rst
--rw-r--r--   0 amo        (501) staff       (20)     2832 2023-07-19 19:40:43.000000 sphinx-design-elements-0.1.0/docs/tag.md
--rw-r--r--   0 amo        (501) staff       (20)     4962 2023-07-19 20:37:12.000000 sphinx-design-elements-0.1.0/pyproject.toml
--rw-r--r--   0 amo        (501) staff       (20)       38 2023-07-19 20:42:44.644339 sphinx-design-elements-0.1.0/setup.cfg
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-07-19 20:42:44.641741 sphinx-design-elements-0.1.0/sphinx_design_elements/
--rw-r--r--   0 amo        (501) staff       (20)      433 2023-07-18 20:19:29.000000 sphinx-design-elements-0.1.0/sphinx_design_elements/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-07-19 20:42:44.643518 sphinx-design-elements-0.1.0/sphinx_design_elements/compiled/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-07-18 20:19:29.000000 sphinx-design-elements-0.1.0/sphinx_design_elements/compiled/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)      965 2023-07-19 20:41:30.000000 sphinx-design-elements-0.1.0/sphinx_design_elements/compiled/style.css
--rw-r--r--   0 amo        (501) staff       (20)     2149 2023-07-18 22:13:22.000000 sphinx-design-elements-0.1.0/sphinx_design_elements/extension.py
--rw-r--r--   0 amo        (501) staff       (20)     4960 2023-07-18 22:10:25.000000 sphinx-design-elements-0.1.0/sphinx_design_elements/gridtable.py
--rw-r--r--   0 amo        (501) staff       (20)     3751 2023-07-19 17:40:51.000000 sphinx-design-elements-0.1.0/sphinx_design_elements/infocard.py
--rw-r--r--   0 amo        (501) staff       (20)     2006 2023-07-18 22:13:22.000000 sphinx-design-elements-0.1.0/sphinx_design_elements/tag.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-07-19 20:42:44.643112 sphinx-design-elements-0.1.0/sphinx_design_elements.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)     5285 2023-07-19 20:42:44.000000 sphinx-design-elements-0.1.0/sphinx_design_elements.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)      923 2023-07-19 20:42:44.000000 sphinx-design-elements-0.1.0/sphinx_design_elements.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2023-07-19 20:42:44.000000 sphinx-design-elements-0.1.0/sphinx_design_elements.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)      339 2023-07-19 20:42:44.000000 sphinx-design-elements-0.1.0/sphinx_design_elements.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       29 2023-07-19 20:42:44.000000 sphinx-design-elements-0.1.0/sphinx_design_elements.egg-info/top_level.txt
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-08-07 22:13:17.499284 sphinx-design-elements-0.2.0/
+-rw-r--r--   0 amo        (501) staff       (20)      368 2023-08-07 22:12:35.000000 sphinx-design-elements-0.2.0/CHANGES.md
+-rw-r--r--   0 amo        (501) staff       (20)     1099 2023-07-16 18:50:11.000000 sphinx-design-elements-0.2.0/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)      134 2023-07-18 20:19:29.000000 sphinx-design-elements-0.2.0/MANIFEST.in
+-rw-r--r--   0 amo        (501) staff       (20)     5285 2023-08-07 22:13:17.499029 sphinx-design-elements-0.2.0/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     2144 2023-07-19 20:41:30.000000 sphinx-design-elements-0.2.0/README.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-08-07 22:13:17.490375 sphinx-design-elements-0.2.0/docs/
+-rw-r--r--   0 amo        (501) staff       (20)      258 2023-07-18 20:19:29.000000 sphinx-design-elements-0.2.0/docs/backlog.md
+-rw-r--r--   0 amo        (501) staff       (20)      368 2023-08-07 22:12:35.000000 sphinx-design-elements-0.2.0/docs/changes.md
+-rw-r--r--   0 amo        (501) staff       (20)     1350 2023-07-19 20:41:30.000000 sphinx-design-elements-0.2.0/docs/css_classes.md
+-rw-r--r--   0 amo        (501) staff       (20)     1212 2023-08-07 22:02:30.000000 sphinx-design-elements-0.2.0/docs/dropdown-group.md
+-rw-r--r--   0 amo        (501) staff       (20)     2114 2023-08-07 22:02:29.000000 sphinx-design-elements-0.2.0/docs/get_started.md
+-rw-r--r--   0 amo        (501) staff       (20)     3867 2023-07-19 20:41:30.000000 sphinx-design-elements-0.2.0/docs/gridtable.md
+-rw-r--r--   0 amo        (501) staff       (20)     3566 2023-08-07 22:11:04.000000 sphinx-design-elements-0.2.0/docs/index.md
+-rw-r--r--   0 amo        (501) staff       (20)     2943 2023-07-19 20:41:30.000000 sphinx-design-elements-0.2.0/docs/infocard.md
+-rw-r--r--   0 amo        (501) staff       (20)      165 2023-07-18 20:38:40.000000 sphinx-design-elements-0.2.0/docs/project.md
+-rw-r--r--   0 amo        (501) staff       (20)     2144 2023-07-19 20:41:30.000000 sphinx-design-elements-0.2.0/docs/readme.md
+-rw-r--r--   0 amo        (501) staff       (20)     1815 2023-07-19 20:49:36.000000 sphinx-design-elements-0.2.0/docs/sandbox.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-08-07 22:13:17.490905 sphinx-design-elements-0.2.0/docs/snippets/
+-rw-r--r--   0 amo        (501) staff       (20)       73 2023-07-18 22:10:25.000000 sphinx-design-elements-0.2.0/docs/snippets/index.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-08-07 22:13:17.492670 sphinx-design-elements-0.2.0/docs/snippets/myst/
+-rw-r--r--   0 amo        (501) staff       (20)      129 2023-08-07 22:02:30.000000 sphinx-design-elements-0.2.0/docs/snippets/myst/dropdown-group.md
+-rw-r--r--   0 amo        (501) staff       (20)      327 2023-07-18 22:10:25.000000 sphinx-design-elements-0.2.0/docs/snippets/myst/gridtable.md
+-rw-r--r--   0 amo        (501) staff       (20)      427 2023-07-19 17:40:51.000000 sphinx-design-elements-0.2.0/docs/snippets/myst/infocard.md
+-rw-r--r--   0 amo        (501) staff       (20)       33 2023-07-18 22:13:22.000000 sphinx-design-elements-0.2.0/docs/snippets/myst/tag.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-08-07 22:13:17.494615 sphinx-design-elements-0.2.0/docs/snippets/rst/
+-rw-r--r--   0 amo        (501) staff       (20)      140 2023-08-07 22:02:30.000000 sphinx-design-elements-0.2.0/docs/snippets/rst/dropdown-group.rst
+-rw-r--r--   0 amo        (501) staff       (20)      373 2023-07-18 22:10:25.000000 sphinx-design-elements-0.2.0/docs/snippets/rst/gridtable.rst
+-rw-r--r--   0 amo        (501) staff       (20)      515 2023-07-19 17:40:51.000000 sphinx-design-elements-0.2.0/docs/snippets/rst/infocard.rst
+-rw-r--r--   0 amo        (501) staff       (20)       33 2023-07-18 22:13:22.000000 sphinx-design-elements-0.2.0/docs/snippets/rst/tag.rst
+-rw-r--r--   0 amo        (501) staff       (20)     2832 2023-07-19 19:40:43.000000 sphinx-design-elements-0.2.0/docs/tag.md
+-rw-r--r--   0 amo        (501) staff       (20)     4908 2023-08-07 22:02:30.000000 sphinx-design-elements-0.2.0/pyproject.toml
+-rw-r--r--   0 amo        (501) staff       (20)       38 2023-08-07 22:13:17.499360 sphinx-design-elements-0.2.0/setup.cfg
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-08-07 22:13:17.496732 sphinx-design-elements-0.2.0/sphinx_design_elements/
+-rw-r--r--   0 amo        (501) staff       (20)      433 2023-07-18 20:19:29.000000 sphinx-design-elements-0.2.0/sphinx_design_elements/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-08-07 22:13:17.498679 sphinx-design-elements-0.2.0/sphinx_design_elements/compiled/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-07-18 20:19:29.000000 sphinx-design-elements-0.2.0/sphinx_design_elements/compiled/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)      965 2023-08-07 22:02:29.000000 sphinx-design-elements-0.2.0/sphinx_design_elements/compiled/style.css
+-rw-r--r--   0 amo        (501) staff       (20)      927 2023-08-07 22:02:30.000000 sphinx-design-elements-0.2.0/sphinx_design_elements/dropdown_group.py
+-rw-r--r--   0 amo        (501) staff       (20)     2228 2023-08-07 22:02:30.000000 sphinx-design-elements-0.2.0/sphinx_design_elements/extension.py
+-rw-r--r--   0 amo        (501) staff       (20)     4960 2023-07-18 22:10:25.000000 sphinx-design-elements-0.2.0/sphinx_design_elements/gridtable.py
+-rw-r--r--   0 amo        (501) staff       (20)     3751 2023-07-19 17:40:51.000000 sphinx-design-elements-0.2.0/sphinx_design_elements/infocard.py
+-rw-r--r--   0 amo        (501) staff       (20)     2006 2023-07-18 22:13:22.000000 sphinx-design-elements-0.2.0/sphinx_design_elements/tag.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-08-07 22:13:17.498217 sphinx-design-elements-0.2.0/sphinx_design_elements.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)     5285 2023-08-07 22:13:17.000000 sphinx-design-elements-0.2.0/sphinx_design_elements.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     1061 2023-08-07 22:13:17.000000 sphinx-design-elements-0.2.0/sphinx_design_elements.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2023-08-07 22:13:17.000000 sphinx-design-elements-0.2.0/sphinx_design_elements.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)      300 2023-08-07 22:13:17.000000 sphinx-design-elements-0.2.0/sphinx_design_elements.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)       29 2023-08-07 22:13:17.000000 sphinx-design-elements-0.2.0/sphinx_design_elements.egg-info/top_level.txt
```

### Comparing `sphinx-design-elements-0.1.0/LICENSE` & `sphinx-design-elements-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.1.0/PKG-INFO` & `sphinx-design-elements-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-design-elements
-Version: 0.1.0
+Version: 0.2.0
 Summary: A collection of composite web elements based on components from sphinx-design.
 Author-email: Andreas Motl <andreas.motl@panodata.org>
 License: MIT License Copyright (c) 2023 Andreas Motl
         
         Permission is hereby granted, free
         of charge, to any person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the Software without
```

### Comparing `sphinx-design-elements-0.1.0/README.md` & `sphinx-design-elements-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.1.0/docs/css_classes.md` & `sphinx-design-elements-0.2.0/docs/css_classes.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.1.0/docs/get_started.md` & `sphinx-design-elements-0.2.0/docs/get_started.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.1.0/docs/gridtable.md` & `sphinx-design-elements-0.2.0/docs/gridtable.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.1.0/docs/index.md` & `sphinx-design-elements-0.2.0/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 ---
 sd_hide_title: true
 ---
 
-# sphinx-design
+(index)=
+
+# sphinx-design-elements
 
 ::::::{div} landing-title
 :style: "padding: 0.6rem 0.1rem 0.1rem 0; background-image: linear-gradient(315deg, #992d3b 0%, #303545 84%); clip-path: polygon(0px 0px, 100% 0%, 100% calc(100% - 1.5rem), 0% 100%); -webkit-clip-path: polygon(0px 0px, 100% 0%, 100% calc(100% - 1.5rem), 0% 100%);"
 
 ::::{grid}
 :reverse:
 :gutter: 2 3 3 3
@@ -81,14 +83,15 @@
 ```
 
 ```{toctree}
 :caption: Styling
 :hidden:
 
 css_classes
+dropdown-group
 ```
 
 ```{toctree}
 :caption: Development
 :hidden:
 
 project
```

### Comparing `sphinx-design-elements-0.1.0/docs/infocard.md` & `sphinx-design-elements-0.2.0/docs/infocard.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.1.0/docs/readme.md` & `sphinx-design-elements-0.2.0/docs/readme.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.1.0/docs/sandbox.md` & `sphinx-design-elements-0.2.0/docs/sandbox.md`

 * *Files 7% similar despite different names*

```diff
@@ -46,11 +46,27 @@
 
 ## Edit source code
 
 In order to edit or inspect the CSS stylesheet rules, head over to
 [`compiled/style.css`]. For editing or inspecting the directive- and
 role-implementations, see [`gridtable.py`], [`infocard.py`], and [`tag.py`].
 
+
+## Releasing
+
+```shell
+# Install a few more prerequisites.
+pip install --editable=.[release]
+
+# Designate a new version.
+git tag v0.1.0
+git push --tags
+
+# Build package, and publish to PyPI.
+poe release
+```
+
+
 [`compiled/style.css`]: https://github.com/panodata/sphinx-design-elements/blob/main/sphinx_design_elements/compiled/style.css
 [`gridtable.py`]: https://github.com/panodata/sphinx-design-elements/blob/main/sphinx_design_elements/gridtable.py
 [`infocard.py`]: https://github.com/panodata/sphinx-design-elements/blob/main/sphinx_design_elements/infocard.py
 [`tag.py`]: https://github.com/panodata/sphinx-design-elements/blob/main/sphinx_design_elements/tag.py
```

### Comparing `sphinx-design-elements-0.1.0/docs/snippets/rst/infocard.rst` & `sphinx-design-elements-0.2.0/docs/snippets/rst/infocard.rst`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.1.0/docs/tag.md` & `sphinx-design-elements-0.2.0/docs/tag.md`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.1.0/pyproject.toml` & `sphinx-design-elements-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -57,26 +57,26 @@
 [project.optional-dependencies]
 develop = [
   "black<24",
   "docutils-stubs",
   "mypy==1.4.1",
   "poethepoet<0.22",
   "pyproject-fmt<0.14",
-  "ruff==0.0.278",
+  "ruff==0.0.282",
   "validate-pyproject<0.14",
 ]
 docs = [
   "furo",
   "myst-parser[linkify]<3,>=0.18",
   "sphinx-autobuild",
   "sphinx-copybutton",
 ]
 release = [
   "build<1",
-  'minibump<1; python_version >= "3.10"',
+  "keyring",
   "twine<5",
 ]
 test = [
   "pytest<8",
   "pytest-cov<5",
   "pytest-regressions<3",
 ]
@@ -214,13 +214,12 @@
   { cmd = "ruff ." },
   { cmd = "black --check ." },
   { cmd = "validate-pyproject pyproject.toml" },
   { cmd = "mypy" },
 ]
 
 release = [
-  { cmd = "minibump bump --relax minor" },
   { cmd = "python -m build" },
-  { cmd = "twine upload dist/*" },
+  { cmd = "twine upload dist/*.tar.gz dist/*.whl" },
 ]
 
 test = { cmd = "pytest" }
```

### Comparing `sphinx-design-elements-0.1.0/sphinx_design_elements/compiled/style.css` & `sphinx-design-elements-0.2.0/sphinx_design_elements/compiled/style.css`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.1.0/sphinx_design_elements/extension.py` & `sphinx-design-elements-0.2.0/sphinx_design_elements/extension.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from docutils import nodes
 from sphinx.application import Sphinx
 from sphinx.environment import BuildEnvironment
 from sphinx_design.extension import depart_container, visit_container
 
 from . import compiled as static_module
+from .dropdown_group import setup_dropdown_group
 from .gridtable import setup_gridtable
 from .infocard import setup_infocard
 from .tag import setup_tags
 
 
 def setup_extension(app: Sphinx) -> None:
     """Set up the sphinx extension."""
@@ -21,14 +22,15 @@
     # we override container html visitors, to stop the default behaviour
     # of adding the `container` class to all nodes.container
     app.add_node(nodes.container, override=True, html=(visit_container, depart_container))
 
     setup_gridtable(app)
     setup_infocard(app)
     setup_tags(app)
+    setup_dropdown_group(app)
 
 
 def update_css_js(app: Sphinx):
     """Copy the CSS to the build directory."""
     # reset changed identifier
     app.env.settings["sphinx_design_elements_css_changed"] = False
     # setup up new static path in output dir
```

### Comparing `sphinx-design-elements-0.1.0/sphinx_design_elements/gridtable.py` & `sphinx-design-elements-0.2.0/sphinx_design_elements/gridtable.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.1.0/sphinx_design_elements/infocard.py` & `sphinx-design-elements-0.2.0/sphinx_design_elements/infocard.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.1.0/sphinx_design_elements/tag.py` & `sphinx-design-elements-0.2.0/sphinx_design_elements/tag.py`

 * *Files identical despite different names*

### Comparing `sphinx-design-elements-0.1.0/sphinx_design_elements.egg-info/PKG-INFO` & `sphinx-design-elements-0.2.0/sphinx_design_elements.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-design-elements
-Version: 0.1.0
+Version: 0.2.0
 Summary: A collection of composite web elements based on components from sphinx-design.
 Author-email: Andreas Motl <andreas.motl@panodata.org>
 License: MIT License Copyright (c) 2023 Andreas Motl
         
         Permission is hereby granted, free
         of charge, to any person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the Software without
```

### Comparing `sphinx-design-elements-0.1.0/sphinx_design_elements.egg-info/SOURCES.txt` & `sphinx-design-elements-0.2.0/sphinx_design_elements.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,30 +2,34 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 docs/backlog.md
 docs/changes.md
 docs/css_classes.md
+docs/dropdown-group.md
 docs/get_started.md
 docs/gridtable.md
 docs/index.md
 docs/infocard.md
 docs/project.md
 docs/readme.md
 docs/sandbox.md
 docs/tag.md
 docs/snippets/index.md
+docs/snippets/myst/dropdown-group.md
 docs/snippets/myst/gridtable.md
 docs/snippets/myst/infocard.md
 docs/snippets/myst/tag.md
+docs/snippets/rst/dropdown-group.rst
 docs/snippets/rst/gridtable.rst
 docs/snippets/rst/infocard.rst
 docs/snippets/rst/tag.rst
 sphinx_design_elements/__init__.py
+sphinx_design_elements/dropdown_group.py
 sphinx_design_elements/extension.py
 sphinx_design_elements/gridtable.py
 sphinx_design_elements/infocard.py
 sphinx_design_elements/tag.py
 sphinx_design_elements.egg-info/PKG-INFO
 sphinx_design_elements.egg-info/SOURCES.txt
 sphinx_design_elements.egg-info/dependency_links.txt
```

