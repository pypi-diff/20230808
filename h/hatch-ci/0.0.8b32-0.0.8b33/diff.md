# Comparing `tmp/hatch_ci-0.0.8b32.tar.gz` & `tmp/hatch_ci-0.0.8b33.tar.gz`

## Comparing `hatch_ci-0.0.8b32.tar` & `hatch_ci-0.0.8b33.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/.gitattributes
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/.pre-commit-config.yaml
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/Makefile
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/.github/workflows/beta.yml
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/.github/workflows/master.yml
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/.github/workflows/tags.yml
--rw-r--r--   0        0        0    28053 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage.xml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/coverage_html.js
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html
--rw-r--r--   0        0        0    44736 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html
--rw-r--r--   0        0        0    85102 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html
--rw-r--r--   0        0        0    49009 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html
--rw-r--r--   0        0        0   129332 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html
--rw-r--r--   0        0        0    23045 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/favicon_32.png
--rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/keybd_open.png
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/style.css
--rw-r--r--   0        0        0    20682 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/junit/junit.html
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/junit/junit.xml
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/index.html
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/mypy-html.css
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html
--rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html
--rw-r--r--   0        0        0    45457 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html
--rw-r--r--   0        0        0    30121 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html
--rw-r--r--   0        0        0    75063 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html
--rw-r--r--   0        0        0    11219 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/src/hatch_ci/__init__.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/src/hatch_ci/cli.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/src/hatch_ci/common.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/src/hatch_ci/hooks.py
--rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/src/hatch_ci/scm.py
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/src/hatch_ci/script.py
--rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/src/hatch_ci/tools.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/src/hatch_ci/version_hook.py
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/tests/conftest.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/tests/requirements.txt
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/tests/test_scm.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/tests/test_tools.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/LICENSE.txt
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/README.md
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/pyproject.toml
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b32/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/.gitattributes
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/Makefile
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/.github/workflows/beta.yml
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/.github/workflows/master.yml
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/.github/workflows/tags.yml
+-rw-r--r--   0        0        0    28003 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage.xml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/coverage_html.js
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html
+-rw-r--r--   0        0        0    44532 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html
+-rw-r--r--   0        0        0    84967 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html
+-rw-r--r--   0        0        0    49464 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html
+-rw-r--r--   0        0        0   129332 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html
+-rw-r--r--   0        0        0    23045 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/favicon_32.png
+-rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/keybd_open.png
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/style.css
+-rw-r--r--   0        0        0    24054 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/junit/junit.html
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/junit/junit.xml
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/index.html
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/mypy-html.css
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html
+-rw-r--r--   0        0        0    23800 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html
+-rw-r--r--   0        0        0    45457 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html
+-rw-r--r--   0        0        0    30121 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html
+-rw-r--r--   0        0        0    75099 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html
+-rw-r--r--   0        0        0    11219 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/src/hatch_ci/__init__.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/src/hatch_ci/cli.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/src/hatch_ci/common.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/src/hatch_ci/hooks.py
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/src/hatch_ci/scm.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/src/hatch_ci/script.py
+-rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/src/hatch_ci/tools.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/src/hatch_ci/version_hook.py
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/tests/conftest.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/tests/requirements.txt
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/tests/test_scm.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/tests/test_script.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/tests/test_tools.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/LICENSE.txt
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/README.md
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/pyproject.toml
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 hatch_ci-0.0.8b33/PKG-INFO
```

### Comparing `hatch_ci-0.0.8b32/Makefile` & `hatch_ci-0.0.8b33/Makefile`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/.github/workflows/beta.yml` & `hatch_ci-0.0.8b33/.github/workflows/beta.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/.github/workflows/master.yml` & `hatch_ci-0.0.8b33/.github/workflows/master.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/.github/workflows/tags.yml` & `hatch_ci-0.0.8b33/.github/workflows/tags.yml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage.xml` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage.xml`

 * *Files 2% similar despite different names*

#### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage.xml` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage.xml`

```diff
@@ -1,75 +1,75 @@
 <?xml version="1.0" encoding="utf-8"?>
-<coverage version="7.2.7" timestamp="1691439205054" lines-valid="572" lines-covered="340" line-rate="0.5944" branches-valid="202" branches-covered="117" branch-rate="0.5792" complexity="0">
+<coverage version="7.2.7" timestamp="1691439619630" lines-valid="572" lines-covered="435" line-rate="0.7605" branches-valid="206" branches-covered="138" branch-rate="0.6699" complexity="0">
   <!-- Generated by coverage.py: https://coverage.readthedocs.io/en/7.2.7 -->
   <!-- Based on https://raw.githubusercontent.com/cobertura/web/master/htdocs/xml/coverage-04.dtd -->
   <sources>
     <source>/home/runner/work/hatch-ci/hatch-ci</source>
   </sources>
   <packages>
-    <package name="src.hatch_ci" line-rate="0.5944" branch-rate="0.5792" complexity="0">
+    <package name="src.hatch_ci" line-rate="0.7605" branch-rate="0.6699" complexity="0">
       <classes>
         <class name="__init__.py" filename="src/hatch_ci/__init__.py" complexity="0" line-rate="1" branch-rate="1">
           <methods/>
           <lines>
             <line number="1" hits="1"/>
             <line number="2" hits="1"/>
           </lines>
         </class>
-        <class name="cli.py" filename="src/hatch_ci/cli.py" complexity="0" line-rate="0" branch-rate="0">
+        <class name="cli.py" filename="src/hatch_ci/cli.py" complexity="0" line-rate="0.3194" branch-rate="0">
           <methods/>
           <lines>
-            <line number="1" hits="0"/>
-            <line number="3" hits="0"/>
-            <line number="4" hits="0"/>
-            <line number="5" hits="0"/>
-            <line number="6" hits="0"/>
-            <line number="7" hits="0"/>
-            <line number="9" hits="0"/>
-            <line number="12" hits="0"/>
-            <line number="13" hits="0"/>
+            <line number="1" hits="1"/>
+            <line number="3" hits="1"/>
+            <line number="4" hits="1"/>
+            <line number="5" hits="1"/>
+            <line number="6" hits="1"/>
+            <line number="7" hits="1"/>
+            <line number="9" hits="1"/>
+            <line number="12" hits="1"/>
+            <line number="13" hits="1"/>
             <line number="14" hits="0"/>
-            <line number="17" hits="0"/>
-            <line number="18" hits="0"/>
-            <line number="19" hits="0"/>
+            <line number="17" hits="1"/>
+            <line number="18" hits="1"/>
+            <line number="19" hits="1"/>
             <line number="20" hits="0"/>
             <line number="21" hits="0"/>
             <line number="22" hits="0"/>
             <line number="23" hits="0"/>
-            <line number="25" hits="0"/>
+            <line number="25" hits="1"/>
             <line number="32" hits="0"/>
             <line number="33" hits="0"/>
             <line number="34" hits="0"/>
             <line number="35" hits="0"/>
-            <line number="37" hits="0"/>
+            <line number="37" hits="1"/>
             <line number="38" hits="0"/>
             <line number="39" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="40,41"/>
             <line number="40" hits="0"/>
             <line number="41" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="42,43"/>
             <line number="42" hits="0"/>
             <line number="43" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="44,46"/>
             <line number="44" hits="0"/>
             <line number="45" hits="0"/>
             <line number="46" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="47,49"/>
             <line number="47" hits="0"/>
             <line number="48" hits="0"/>
             <line number="49" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="exit,exit"/>
-            <line number="52" hits="0"/>
+            <line number="52" hits="1"/>
             <line number="61" hits="0"/>
             <line number="62" hits="0"/>
-            <line number="65" hits="0"/>
+            <line number="65" hits="1"/>
             <line number="68" hits="0"/>
             <line number="75" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="78,79"/>
             <line number="78" hits="0"/>
             <line number="79" hits="0"/>
-            <line number="82" hits="0"/>
-            <line number="88" hits="0"/>
-            <line number="89" hits="0"/>
-            <line number="90" hits="0"/>
-            <line number="91" hits="0"/>
+            <line number="82" hits="1"/>
+            <line number="88" hits="1"/>
+            <line number="89" hits="1"/>
+            <line number="90" hits="1"/>
+            <line number="91" hits="1"/>
             <line number="92" hits="0"/>
             <line number="94" hits="0"/>
             <line number="98" hits="0"/>
             <line number="100" hits="0"/>
             <line number="101" hits="0"/>
             <line number="106" hits="0"/>
             <line number="107" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="108,110"/>
@@ -84,16 +84,16 @@
             <line number="125" hits="0"/>
             <line number="127" hits="0"/>
             <line number="128" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="129,131"/>
             <line number="129" hits="0"/>
             <line number="130" hits="0"/>
             <line number="131" hits="0"/>
             <line number="132" hits="0"/>
-            <line number="134" hits="0"/>
-            <line number="136" hits="0"/>
+            <line number="134" hits="1"/>
+            <line number="136" hits="1"/>
           </lines>
         </class>
         <class name="common.py" filename="src/hatch_ci/common.py" complexity="0" line-rate="0" branch-rate="1">
           <methods/>
           <lines>
             <line number="1" hits="0"/>
           </lines>
@@ -104,15 +104,15 @@
             <line number="1" hits="0"/>
             <line number="3" hits="0"/>
             <line number="6" hits="0"/>
             <line number="7" hits="0"/>
             <line number="8" hits="0"/>
           </lines>
         </class>
-        <class name="scm.py" filename="src/hatch_ci/scm.py" complexity="0" line-rate="0.8333" branch-rate="0.7692">
+        <class name="scm.py" filename="src/hatch_ci/scm.py" complexity="0" line-rate="0.9259" branch-rate="0.8077">
           <methods/>
           <lines>
             <line number="3" hits="1"/>
             <line number="5" hits="1"/>
             <line number="6" hits="1"/>
             <line number="7" hits="1"/>
             <line number="8" hits="1"/>
@@ -128,16 +128,16 @@
             <line number="27" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="28" hits="1"/>
             <line number="29" hits="1"/>
             <line number="31" hits="1"/>
             <line number="33" hits="1"/>
             <line number="34" hits="1"/>
             <line number="37" hits="1"/>
-            <line number="38" hits="0"/>
-            <line number="39" hits="0"/>
+            <line number="38" hits="1"/>
+            <line number="39" hits="1"/>
             <line number="42" hits="1"/>
             <line number="43" hits="1"/>
             <line number="46" hits="1"/>
             <line number="47" hits="1"/>
             <line number="50" hits="1"/>
             <line number="51" hits="1"/>
             <line number="54" hits="1" branch="true" condition-coverage="100% (2/2)"/>
@@ -149,15 +149,15 @@
             <line number="62" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="63" hits="1"/>
             <line number="64" hits="1"/>
             <line number="66" hits="1"/>
             <line number="67" hits="1"/>
             <line number="69" hits="1"/>
             <line number="70" hits="1"/>
-            <line number="71" hits="0"/>
+            <line number="71" hits="1"/>
             <line number="74" hits="1"/>
             <line number="75" hits="1"/>
             <line number="76" hits="1"/>
             <line number="77" hits="1"/>
             <line number="78" hits="1"/>
             <line number="80" hits="1"/>
             <line number="81" hits="1"/>
@@ -179,42 +179,42 @@
             <line number="107" hits="1"/>
             <line number="109" hits="1"/>
             <line number="110" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="111" hits="1"/>
             <line number="114" hits="1"/>
             <line number="115" hits="1"/>
             <line number="116" hits="1"/>
-            <line number="117" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="118,119"/>
-            <line number="118" hits="0"/>
-            <line number="119" hits="0"/>
-            <line number="121" hits="0"/>
+            <line number="117" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="118" hits="1"/>
+            <line number="119" hits="1"/>
+            <line number="121" hits="1"/>
             <line number="122" hits="0"/>
-            <line number="124" hits="0"/>
+            <line number="124" hits="1"/>
             <line number="125" hits="0"/>
-            <line number="127" hits="0"/>
-            <line number="128" hits="0"/>
-            <line number="136" hits="0"/>
+            <line number="127" hits="1"/>
+            <line number="128" hits="1"/>
+            <line number="136" hits="1"/>
             <line number="138" hits="1"/>
             <line number="139" hits="1"/>
             <line number="140" hits="1"/>
             <line number="142" hits="1"/>
             <line number="143" hits="1"/>
             <line number="144" hits="1"/>
             <line number="145" hits="1"/>
             <line number="146" hits="1"/>
-            <line number="147" hits="0"/>
-            <line number="148" hits="0"/>
+            <line number="147" hits="1"/>
+            <line number="148" hits="1"/>
             <line number="149" hits="1"/>
             <line number="151" hits="1"/>
             <line number="158" hits="1"/>
             <line number="165" hits="1"/>
             <line number="166" hits="1"/>
             <line number="167" hits="1"/>
-            <line number="168" hits="0"/>
-            <line number="169" hits="0"/>
+            <line number="168" hits="1"/>
+            <line number="169" hits="1"/>
             <line number="170" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="171" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="172" hits="1"/>
             <line number="173" hits="1"/>
             <line number="174" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="175"/>
             <line number="175" hits="0"/>
             <line number="176" hits="1"/>
@@ -271,86 +271,86 @@
             <line number="262" hits="1"/>
             <line number="263" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="264"/>
             <line number="264" hits="0"/>
             <line number="265" hits="1"/>
             <line number="266" hits="0"/>
           </lines>
         </class>
-        <class name="script.py" filename="src/hatch_ci/script.py" complexity="0" line-rate="0" branch-rate="0">
+        <class name="script.py" filename="src/hatch_ci/script.py" complexity="0" line-rate="0.8636" branch-rate="0.75">
           <methods/>
           <lines>
-            <line number="12" hits="0"/>
-            <line number="14" hits="0"/>
-            <line number="15" hits="0"/>
-            <line number="16" hits="0"/>
-            <line number="17" hits="0"/>
-            <line number="18" hits="0"/>
-            <line number="20" hits="0"/>
-            <line number="22" hits="0"/>
-            <line number="25" hits="0"/>
-            <line number="26" hits="0"/>
-            <line number="27" hits="0"/>
-            <line number="34" hits="0"/>
-            <line number="35" hits="0"/>
-            <line number="38" hits="0"/>
-            <line number="41" hits="0"/>
-            <line number="42" hits="0"/>
-            <line number="43" hits="0"/>
-            <line number="44" hits="0"/>
-            <line number="45" hits="0"/>
-            <line number="50" hits="0"/>
-            <line number="51" hits="0"/>
-            <line number="52" hits="0"/>
+            <line number="12" hits="1"/>
+            <line number="14" hits="1"/>
+            <line number="15" hits="1"/>
+            <line number="16" hits="1"/>
+            <line number="17" hits="1"/>
+            <line number="18" hits="1"/>
+            <line number="20" hits="1"/>
+            <line number="22" hits="1"/>
+            <line number="25" hits="1"/>
+            <line number="26" hits="1"/>
+            <line number="27" hits="1"/>
+            <line number="34" hits="1"/>
+            <line number="35" hits="1"/>
+            <line number="38" hits="1"/>
+            <line number="41" hits="1"/>
+            <line number="42" hits="1"/>
+            <line number="43" hits="1"/>
+            <line number="44" hits="1"/>
+            <line number="45" hits="1"/>
+            <line number="50" hits="1"/>
+            <line number="51" hits="1"/>
+            <line number="52" hits="1"/>
             <line number="53" hits="0"/>
-            <line number="54" hits="0"/>
-            <line number="55" hits="0"/>
+            <line number="54" hits="1"/>
+            <line number="55" hits="1"/>
             <line number="64" hits="0"/>
-            <line number="67" hits="0"/>
-            <line number="68" hits="0"/>
-            <line number="70" hits="0"/>
-            <line number="76" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="77,78"/>
+            <line number="67" hits="1"/>
+            <line number="68" hits="1"/>
+            <line number="70" hits="1"/>
+            <line number="76" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="77"/>
             <line number="77" hits="0"/>
-            <line number="78" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="79,81"/>
-            <line number="79" hits="0"/>
-            <line number="81" hits="0"/>
-            <line number="82" hits="0"/>
-            <line number="83" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="84,87"/>
+            <line number="78" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="79" hits="1"/>
+            <line number="81" hits="1"/>
+            <line number="82" hits="1"/>
+            <line number="83" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="84"/>
             <line number="84" hits="0"/>
-            <line number="87" hits="0"/>
-            <line number="89" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="90,115"/>
-            <line number="90" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="91,95"/>
+            <line number="87" hits="1"/>
+            <line number="89" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="90" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="91"/>
             <line number="91" hits="0"/>
-            <line number="95" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="96,99"/>
-            <line number="96" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="97,98"/>
-            <line number="97" hits="0"/>
-            <line number="98" hits="0"/>
-            <line number="99" hits="0"/>
-            <line number="100" hits="0"/>
-            <line number="101" hits="0"/>
-            <line number="115" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="117,165"/>
-            <line number="117" hits="0"/>
-            <line number="118" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="119,125"/>
-            <line number="119" hits="0"/>
+            <line number="95" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="96" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="97" hits="1"/>
+            <line number="98" hits="1"/>
+            <line number="99" hits="1"/>
+            <line number="100" hits="1"/>
+            <line number="101" hits="1"/>
+            <line number="115" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="165"/>
+            <line number="117" hits="1"/>
+            <line number="118" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="119" hits="1"/>
             <line number="124" hits="0"/>
-            <line number="125" hits="0"/>
-            <line number="126" hits="0" branch="true" condition-coverage="0% (0/2)" missing-branches="127,130"/>
+            <line number="125" hits="1"/>
+            <line number="126" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="127"/>
             <line number="127" hits="0"/>
-            <line number="130" hits="0"/>
-            <line number="133" hits="0"/>
-            <line number="136" hits="0"/>
-            <line number="137" hits="0"/>
-            <line number="140" hits="0"/>
-            <line number="141" hits="0"/>
-            <line number="144" hits="0"/>
-            <line number="148" hits="0"/>
+            <line number="130" hits="1"/>
+            <line number="133" hits="1"/>
+            <line number="136" hits="1"/>
+            <line number="137" hits="1"/>
+            <line number="140" hits="1"/>
+            <line number="141" hits="1"/>
+            <line number="144" hits="1"/>
+            <line number="148" hits="1"/>
             <line number="165" hits="0"/>
             <line number="166" hits="0"/>
           </lines>
         </class>
-        <class name="tools.py" filename="src/hatch_ci/tools.py" complexity="0" line-rate="0.9062" branch-rate="0.7857">
+        <class name="tools.py" filename="src/hatch_ci/tools.py" complexity="0" line-rate="0.9062" branch-rate="0.7941">
           <methods/>
           <lines>
             <line number="3" hits="1"/>
             <line number="5" hits="1"/>
             <line number="6" hits="1"/>
             <line number="7" hits="1"/>
             <line number="8" hits="1"/>
@@ -482,15 +482,15 @@
             <line number="223" hits="1"/>
             <line number="224" hits="1"/>
             <line number="225" hits="1"/>
             <line number="226" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="227" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="228" hits="1"/>
             <line number="229" hits="1"/>
-            <line number="231" hits="1"/>
+            <line number="231" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="232" hits="1"/>
             <line number="233" hits="1"/>
             <line number="236" hits="1"/>
             <line number="251" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="252" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="253" hits="1"/>
             <line number="254" hits="1"/>
@@ -563,15 +563,15 @@
             <line number="415" hits="1"/>
             <line number="416" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="417" hits="1"/>
             <line number="418" hits="1"/>
             <line number="419" hits="1"/>
             <line number="421" hits="1" branch="true" condition-coverage="50% (1/2)" missing-branches="429"/>
             <line number="422" hits="1"/>
-            <line number="423" hits="1"/>
+            <line number="423" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="424" hits="1"/>
             <line number="425" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="426" hits="1"/>
             <line number="427" hits="1"/>
             <line number="429" hits="1"/>
           </lines>
         </class>
```

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/coverage_html.js` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/coverage_html.js`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/d_7005a4ce5d73f943___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -89,13 +89,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 2 statements   2 run 0 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 20:13 +0000
+at 2023-08-07 20:20 +0000
 
 
 1__version__ = "0.0.8" 
 2__hash__ = "" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 20:13 +0000
+at 2023-08-07 20:20 +0000
```

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/d_7005a4ce5d73f943_cli_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/hatch_ci/cli.py: 0%</title>
+    <title>Coverage for src/hatch_ci/cli.py: 26%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/hatch_ci/cli.py</b>:
-            <span class="pc_cov">0%</span>
+            <span class="pc_cov">26%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -52,105 +52,105 @@
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
             <span class="text">72 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">72<span class="text"> missing</span></button>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">23<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">49<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
             <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">0<span class="text"> partial</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
             <button type="button" class="button_next_file" data-shortcut="]"/>
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="mis show_mis"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">from</span> <span class="nam">__future__</span> <span class="key">import</span> <span class="nam">annotations</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">from</span> <span class="nam">__future__</span> <span class="key">import</span> <span class="nam">annotations</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">argparse</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">functools</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">logging</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">Callable</span><span class="op">,</span> <span class="nam">Protocol</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">argparse</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">functools</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">logging</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">Callable</span><span class="op">,</span> <span class="nam">Protocol</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="op">.</span> <span class="key">import</span> <span class="nam">tools</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="op">.</span> <span class="key">import</span> <span class="nam">tools</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">class</span> <span class="nam">ErrorFn</span><span class="op">(</span><span class="nam">Protocol</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="key">def</span> <span class="nam">__call__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">message</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">explain</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">,</span> <span class="nam">hint</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">class</span> <span class="nam">ErrorFn</span><span class="op">(</span><span class="nam">Protocol</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="key">def</span> <span class="nam">__call__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">message</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">explain</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">,</span> <span class="nam">hint</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">        <span class="op">...</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">class</span> <span class="nam">AbortExecutionError</span><span class="op">(</span><span class="nam">Exception</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="op">@</span><span class="nam">staticmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="key">def</span> <span class="nam">_strip</span><span class="op">(</span><span class="nam">txt</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">class</span> <span class="nam">AbortExecutionError</span><span class="op">(</span><span class="nam">Exception</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="op">@</span><span class="nam">staticmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="key">def</span> <span class="nam">_strip</span><span class="op">(</span><span class="nam">txt</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">txt</span> <span class="op">=</span> <span class="nam">txt</span> <span class="key">or</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">        <span class="nam">txt</span> <span class="op">=</span> <span class="nam">txt</span><span class="op">[</span><span class="num">1</span><span class="op">:</span><span class="op">]</span> <span class="key">if</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span> <span class="key">else</span> <span class="nam">txt</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="nam">txt</span> <span class="op">=</span> <span class="nam">tools</span><span class="op">.</span><span class="nam">indent</span><span class="op">(</span><span class="nam">txt</span><span class="op">,</span> <span class="nam">pre</span><span class="op">=</span><span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="key">return</span> <span class="nam">txt</span><span class="op">[</span><span class="op">:</span><span class="op">-</span><span class="num">1</span><span class="op">]</span> <span class="key">if</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">endswith</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span> <span class="key">else</span> <span class="nam">txt</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="nam">message</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">        <span class="nam">explain</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="nam">hint</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">usage</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">message</span> <span class="op">=</span> <span class="nam">message</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">explain</span> <span class="op">=</span> <span class="nam">explain</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">hint</span> <span class="op">=</span> <span class="nam">hint</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">usage</span> <span class="op">=</span> <span class="nam">usage</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">        <span class="nam">out</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">usage</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">            <span class="nam">out</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">usage</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">message</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">            <span class="nam">out</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_strip</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">message</span><span class="op">)</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">explain</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">            <span class="nam">out</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="str">"reason:"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">            <span class="nam">out</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="nam">tools</span><span class="op">.</span><span class="nam">indent</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">explain</span><span class="op">)</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">hint</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">            <span class="nam">out</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="str">"hint:"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">            <span class="nam">out</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="nam">tools</span><span class="op">.</span><span class="nam">indent</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">hint</span><span class="op">)</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="key">return</span> <span class="str">"\n"</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="op">(</span><span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="key">not</span> <span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">else</span> <span class="nam">line</span><span class="op">)</span> <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">out</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="key">def</span> <span class="nam">_add_arguments</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="key">def</span> <span class="nam">_add_arguments</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="nam">parser</span><span class="op">:</span> <span class="nam">argparse</span><span class="op">.</span><span class="nam">ArgumentParser</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="str">"""parses args from the command line</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t"><span class="str">        args: command line arguments or None to pull from sys.argv</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">        doc: text to use in cli description</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span><span class="str">"-n"</span><span class="op">,</span> <span class="str">"--dry-run"</span><span class="op">,</span> <span class="nam">dest</span><span class="op">=</span><span class="str">"dryrun"</span><span class="op">,</span> <span class="nam">action</span><span class="op">=</span><span class="str">"store_true"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span><span class="str">"-v"</span><span class="op">,</span> <span class="str">"--verbose"</span><span class="op">,</span> <span class="nam">action</span><span class="op">=</span><span class="str">"store_true"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t"><span class="key">def</span> <span class="nam">_process_options</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t"><span class="key">def</span> <span class="nam">_process_options</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="nam">options</span><span class="op">:</span> <span class="nam">argparse</span><span class="op">.</span><span class="nam">Namespace</span><span class="op">,</span> <span class="nam">errorfn</span><span class="op">:</span> <span class="nam">ErrorFn</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">argparse</span><span class="op">.</span><span class="nam">Namespace</span> <span class="op">|</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">    <span class="nam">logging</span><span class="op">.</span><span class="nam">basicConfig</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="nam">format</span><span class="op">=</span><span class="str">"%(levelname)s:%(name)s:(dry-run) %(message)s"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="key">if</span> <span class="nam">options</span><span class="op">.</span><span class="nam">dryrun</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="key">else</span> <span class="str">"%(levelname)s:%(name)s:%(message)s"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="nam">level</span><span class="op">=</span><span class="nam">logging</span><span class="op">.</span><span class="nam">DEBUG</span> <span class="key">if</span> <span class="nam">options</span><span class="op">.</span><span class="nam">verbose</span> <span class="key">else</span> <span class="nam">logging</span><span class="op">.</span><span class="nam">INFO</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
@@ -159,24 +159,24 @@
     <p class="mis show_mis"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">    <span class="key">for</span> <span class="nam">d</span> <span class="key">in</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="str">"verbose"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">    <span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">        <span class="nam">delattr</span><span class="op">(</span><span class="nam">options</span><span class="op">,</span> <span class="nam">d</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="key">return</span> <span class="nam">options</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t"><span class="key">def</span> <span class="nam">cli</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t"><span class="key">def</span> <span class="nam">cli</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="nam">add_arguments</span><span class="op">:</span> <span class="nam">Callable</span><span class="op">[</span><span class="op">[</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">ArgumentParser</span><span class="op">]</span><span class="op">,</span> <span class="key">None</span><span class="op">]</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">    <span class="nam">process_options</span><span class="op">:</span> <span class="nam">Callable</span><span class="op">[</span><span class="op">[</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">Namespace</span><span class="op">,</span> <span class="nam">ErrorFn</span><span class="op">]</span><span class="op">,</span> <span class="nam">argparse</span><span class="op">.</span><span class="nam">Namespace</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">    <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="nam">doc</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t"><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">    <span class="op">@</span><span class="nam">functools</span><span class="op">.</span><span class="nam">wraps</span><span class="op">(</span><span class="nam">cli</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="key">def</span> <span class="nam">_fn</span><span class="op">(</span><span class="nam">main</span><span class="op">:</span> <span class="nam">Callable</span><span class="op">[</span><span class="op">[</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">Namespace</span><span class="op">]</span><span class="op">,</span> <span class="nam">Any</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="op">@</span><span class="nam">functools</span><span class="op">.</span><span class="nam">wraps</span><span class="op">(</span><span class="nam">main</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="key">def</span> <span class="nam">_fn1</span><span class="op">(</span><span class="nam">args</span><span class="op">:</span> <span class="key">None</span> <span class="op">|</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">    <span class="op">@</span><span class="nam">functools</span><span class="op">.</span><span class="nam">wraps</span><span class="op">(</span><span class="nam">cli</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="key">def</span> <span class="nam">_fn</span><span class="op">(</span><span class="nam">main</span><span class="op">:</span> <span class="nam">Callable</span><span class="op">[</span><span class="op">[</span><span class="nam">argparse</span><span class="op">.</span><span class="nam">Namespace</span><span class="op">]</span><span class="op">,</span> <span class="nam">Any</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="op">@</span><span class="nam">functools</span><span class="op">.</span><span class="nam">wraps</span><span class="op">(</span><span class="nam">main</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="key">def</span> <span class="nam">_fn1</span><span class="op">(</span><span class="nam">args</span><span class="op">:</span> <span class="key">None</span> <span class="op">|</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">            <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">                <span class="key">class</span> <span class="nam">ParserFormatter</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">                    <span class="nam">argparse</span><span class="op">.</span><span class="nam">ArgumentDefaultsHelpFormatter</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">                    <span class="nam">argparse</span><span class="op">.</span><span class="nam">RawDescriptionHelpFormatter</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">                <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">                    <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
@@ -211,25 +211,25 @@
     <p class="mis show_mis"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">                <span class="key">return</span> <span class="nam">main</span><span class="op">(</span><span class="nam">options</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">            <span class="key">except</span> <span class="nam">AbortExecutionError</span> <span class="key">as</span> <span class="nam">err</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">                <span class="nam">print</span><span class="op">(</span><span class="nam">str</span><span class="op">(</span><span class="nam">err</span><span class="op">)</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>  <span class="com"># noqa: T201</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">                <span class="key">raise</span> <span class="nam">SystemExit</span><span class="op">(</span><span class="num">2</span><span class="op">)</span> <span class="key">from</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">            <span class="key">except</span> <span class="nam">Exception</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">                <span class="key">raise</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">        <span class="key">return</span> <span class="nam">_fn1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">        <span class="key">return</span> <span class="nam">_fn1</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">    <span class="key">return</span> <span class="nam">_fn</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">    <span class="key">return</span> <span class="nam">_fn</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 
-****** Coverage for src/hatch_ci/cli.py: 0% ******
+****** Coverage for src/hatch_ci/cli.py: 26% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x p   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 72 statements   0 run 72 missing 0 excluded 0 partial *****
+***** 72 statements   23 run 49 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 20:13 +0000
+at 2023-08-07 20:20 +0000
 
 
 1from __future__ import annotations 
 2 
 3import argparse 
 4import functools 
 5import logging 
@@ -151,8 +151,8 @@
 132 raise 
 133 
 134 return _fn1 
 135 
 136 return _fn 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 20:13 +0000
+at 2023-08-07 20:20 +0000
```

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/d_7005a4ce5d73f943_common_py.html`

 * *Files 9% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -88,13 +88,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,14 +7,14 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 1 statements   0 run 1 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 20:13 +0000
+at 2023-08-07 20:20 +0000
 
 
 1PLUGIN_NAME = "ci" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 20:13 +0000
+at 2023-08-07 20:20 +0000
```

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/d_7005a4ce5d73f943_hooks_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -95,13 +95,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_common_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,21 +7,21 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 5 statements   0 run 5 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 20:13 +0000
+at 2023-08-07 20:20 +0000
 
 
 1from hatchling.plugin import hookimpl 
 2 
 3from hatch_ci.version_hook import CIVersionSource 
 4 
 5 
 6@hookimpl 
 7def hatch_register_version_source(): 
 8 return CIVersionSource 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 20:13 +0000
+at 2023-08-07 20:20 +0000
```

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/d_7005a4ce5d73f943_scm_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/hatch_ci/scm.py: 82%</title>
+    <title>Coverage for src/hatch_ci/scm.py: 90%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/hatch_ci/scm.py</b>:
-            <span class="pc_cov">82%</span>
+            <span class="pc_cov">90%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -52,26 +52,26 @@
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
             <span class="text">162 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">135<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">27<span class="text"> missing</span></button>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">150<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">12<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
             <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">8<span class="text"> partial</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -115,16 +115,16 @@
     <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="nam">last_eol</span> <span class="op">=</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="nam">result</span> <span class="op">=</span> <span class="nam">pre</span> <span class="op">+</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">"\n"</span><span class="op">,</span> <span class="str">"\n"</span> <span class="op">+</span> <span class="nam">pre</span><span class="op">)</span> <span class="op">+</span> <span class="nam">last_eol</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span> <span class="key">if</span> <span class="nam">result</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span> <span class="key">else</span> <span class="nam">result</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t"><span class="key">def</span> <span class="nam">shorthand</span><span class="op">(</span><span class="nam">txt</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="nam">tag</span> <span class="op">=</span> <span class="str">"refs/heads/"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="key">return</span> <span class="nam">txt</span><span class="op">[</span><span class="nam">len</span><span class="op">(</span><span class="nam">tag</span><span class="op">)</span> <span class="op">:</span><span class="op">]</span> <span class="key">if</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="nam">tag</span><span class="op">)</span> <span class="key">else</span> <span class="nam">txt</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="nam">tag</span> <span class="op">=</span> <span class="str">"refs/heads/"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="key">return</span> <span class="nam">txt</span><span class="op">[</span><span class="nam">len</span><span class="op">(</span><span class="nam">tag</span><span class="op">)</span> <span class="op">:</span><span class="op">]</span> <span class="key">if</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="nam">tag</span><span class="op">)</span> <span class="key">else</span> <span class="nam">txt</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="key">class</span> <span class="nam">NA</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="key">class</span> <span class="nam">GitError</span><span class="op">(</span><span class="nam">Exception</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
@@ -148,15 +148,15 @@
     <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">        <span class="nam">hex</span><span class="op">:</span> <span class="nam">str</span>  <span class="com"># noqa: A003</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="nam">target</span><span class="op">:</span> <span class="nam">GitRepoHeadHex</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">    <span class="op">@</span><span class="nam">property</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="key">def</span> <span class="nam">shorthand</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="key">return</span> <span class="nam">shorthand</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="key">return</span> <span class="nam">shorthand</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t"><span class="key">class</span> <span class="nam">GitRepoBase</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">workdir</span><span class="op">:</span> <span class="nam">Path</span> <span class="op">|</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">exe</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"git"</span><span class="op">,</span> <span class="nam">gitdir</span><span class="op">:</span> <span class="nam">Path</span> <span class="op">|</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">""</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">workdir</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">workdir</span><span class="op">)</span><span class="op">.</span><span class="nam">absolute</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">exe</span> <span class="op">=</span> <span class="nam">exe</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">gitdir</span> <span class="op">=</span> <span class="nam">Path</span><span class="op">(</span><span class="nam">gitdir</span> <span class="key">or</span> <span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">workdir</span> <span class="op">/</span> <span class="str">".git"</span><span class="op">)</span><span class="op">)</span><span class="op">.</span><span class="nam">absolute</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
@@ -194,46 +194,46 @@
     <p class="run"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span><span class="str">"\n"</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="op">[</span><span class="nam">line</span><span class="op">.</span><span class="nam">rstrip</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">lines</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span><span class="op">]</span><span class="op">)</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">buf</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">        <span class="key">return</span> <span class="nam">buf</span><span class="op">.</span><span class="nam">getvalue</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t"><span class="key">class</span> <span class="nam">GitRepo</span><span class="op">(</span><span class="nam">GitRepoBase</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">    <span class="op">@</span><span class="nam">property</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">    <span class="key">def</span> <span class="nam">config</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">        <span class="op">@</span><span class="nam">dc</span><span class="op">.</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="key">class</span> <span class="nam">X</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">            <span class="nam">repo</span><span class="op">:</span> <span class="nam">GitRepo</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">        <span class="op">@</span><span class="nam">dc</span><span class="op">.</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="key">class</span> <span class="nam">X</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">            <span class="nam">repo</span><span class="op">:</span> <span class="nam">GitRepo</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">            <span class="key">def</span> <span class="nam">__getitem__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">item</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">            <span class="key">def</span> <span class="nam">__getitem__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">item</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">                <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"config"</span><span class="op">,</span> <span class="nam">item</span><span class="op">]</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">            <span class="key">def</span> <span class="nam">__setitem__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">item</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">value</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">            <span class="key">def</span> <span class="nam">__setitem__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">item</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">value</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"config"</span><span class="op">,</span> <span class="nam">item</span><span class="op">,</span> <span class="nam">str</span><span class="op">(</span><span class="nam">value</span><span class="op">)</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">            <span class="key">def</span> <span class="nam">__contains__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">item</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">                <span class="key">return</span> <span class="nam">item</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">            <span class="key">def</span> <span class="nam">__contains__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">item</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">                <span class="key">return</span> <span class="nam">item</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">                    <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">                        <span class="str">"config"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">                        <span class="str">"--list"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">                        <span class="str">"--name-only"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">                    <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">                <span class="op">)</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="key">return</span> <span class="nam">X</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="key">return</span> <span class="nam">X</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">    <span class="key">def</span> <span class="nam">revert</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">paths</span><span class="op">:</span> <span class="nam">ListOfArgs</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="nam">sources</span> <span class="op">=</span> <span class="nam">to_list_of_paths</span><span class="op">(</span><span class="nam">paths</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">workdir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">        <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"checkout"</span><span class="op">,</span> <span class="op">*</span><span class="nam">sources</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">    <span class="op">@</span><span class="nam">property</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">    <span class="key">def</span> <span class="nam">head</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="nam">name</span> <span class="op">=</span> <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"symbolic-ref"</span><span class="op">,</span> <span class="str">"HEAD"</span><span class="op">]</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">            <span class="nam">txt</span> <span class="op">=</span> <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"rev-parse"</span><span class="op">,</span> <span class="nam">name</span><span class="op">]</span><span class="op">)</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">        <span class="key">except</span> <span class="nam">subprocess</span><span class="op">.</span><span class="nam">CalledProcessError</span> <span class="key">as</span> <span class="nam">exc</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">            <span class="key">raise</span> <span class="nam">GitError</span><span class="op">(</span><span class="str">f"no branch '{name}'"</span><span class="op">)</span> <span class="key">from</span> <span class="nam">exc</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">        <span class="key">except</span> <span class="nam">subprocess</span><span class="op">.</span><span class="nam">CalledProcessError</span> <span class="key">as</span> <span class="nam">exc</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">            <span class="key">raise</span> <span class="nam">GitError</span><span class="op">(</span><span class="str">f"no branch '{name}'"</span><span class="op">)</span> <span class="key">from</span> <span class="nam">exc</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">        <span class="key">return</span> <span class="nam">GitRepoHead</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="nam">name</span><span class="op">,</span> <span class="nam">target</span><span class="op">=</span><span class="nam">GitRepoHead</span><span class="op">.</span><span class="nam">GitRepoHeadHex</span><span class="op">(</span><span class="nam">txt</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">    <span class="key">def</span> <span class="nam">status</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">        <span class="nam">untracked_files</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"all"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">        <span class="nam">ignored</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">int</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
@@ -245,16 +245,16 @@
     <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">            <span class="str">"D "</span><span class="op">:</span> <span class="num">4</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">            <span class="str">" M"</span><span class="op">:</span> <span class="num">256</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">            <span class="str">"A "</span><span class="op">:</span> <span class="num">1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">        <span class="nam">result</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">            <span class="nam">txt</span> <span class="op">=</span> <span class="nam">self</span><span class="op">(</span><span class="op">[</span><span class="str">"status"</span><span class="op">,</span> <span class="str">"--porcelain"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">        <span class="key">except</span> <span class="nam">subprocess</span><span class="op">.</span><span class="nam">CalledProcessError</span> <span class="key">as</span> <span class="nam">exc</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">            <span class="key">raise</span> <span class="nam">GitError</span><span class="op">(</span><span class="str">"invalid repo"</span><span class="op">)</span> <span class="key">from</span> <span class="nam">exc</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">        <span class="key">except</span> <span class="nam">subprocess</span><span class="op">.</span><span class="nam">CalledProcessError</span> <span class="key">as</span> <span class="nam">exc</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">            <span class="key">raise</span> <span class="nam">GitError</span><span class="op">(</span><span class="str">"invalid repo"</span><span class="op">)</span> <span class="key">from</span> <span class="nam">exc</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">        <span class="key">for</span> <span class="nam">line</span> <span class="key">in</span> <span class="nam">txt</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"\n"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">line</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">                <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">            <span class="nam">tag</span><span class="op">,</span> <span class="nam">filename</span> <span class="op">=</span> <span class="nam">line</span><span class="op">[</span><span class="op">:</span><span class="num">2</span><span class="op">]</span><span class="op">,</span> <span class="nam">line</span><span class="op">[</span><span class="num">3</span><span class="op">:</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="par run show_par"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">            <span class="key">if</span> <span class="nam">tag</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">mapper</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">174&#x202F;&#x219B;&#x202F;175</span><span class="annotate long">line 174 didn't jump to line 175, because the condition on line 174 was never true</span></span></p>
     <p class="mis show_mis"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">                <span class="key">raise</span> <span class="nam">GitError</span><span class="op">(</span><span class="str">f"cannot map git status for '{tag}'"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">mapper</span><span class="op">[</span><span class="nam">tag</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
@@ -353,13 +353,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_hooks_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 
-****** Coverage for src/hatch_ci/scm.py: 82% ******
+****** Coverage for src/hatch_ci/scm.py: 90% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x p   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 162 statements   135 run 27 missing 0 excluded 8 partial *****
+***** 162 statements   150 run 12 missing 0 excluded 8 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 20:13 +0000
+at 2023-08-07 20:20 +0000
 
 
 1# see https://pypi.org/project/setuptools-github 
 2# copy of setuptools_github.scm 
 3from __future__ import annotations 
 4 
 5import dataclasses as dc 
@@ -287,8 +287,8 @@
 263 if str(cur) == cur.root: 263&#x202F;&#x219B;&#x202F;264line 263 didn't jump
 to line 264, because the condition on line 263 was never true
 264 break 
 265 cur = cur.parent 
 266 return None 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 20:13 +0000
+at 2023-08-07 20:20 +0000
```

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/d_7005a4ce5d73f943_script_py.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/hatch_ci/script.py: 0%</title>
+    <title>Coverage for src/hatch_ci/script.py: 84%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/hatch_ci/script.py</b>:
-            <span class="pc_cov">0%</span>
+            <span class="pc_cov">84%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -52,26 +52,26 @@
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
             <span class="text">66 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">66<span class="text"> missing</span></button>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">57<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">9<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">2<span class="text"> excluded</span></button>
-            <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">0<span class="text"> partial</span></button>
+            <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">5<span class="text"> partial</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -89,151 +89,151 @@
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="str">     hatch-ci make-beta ./src/package_name/__init__.py</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="str">Or will release the beta branch and will move inot the next minor</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="str">    hatch-ci {major|minor|micro} ./src/package_name/__init__.py</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">__future__</span> <span class="key">import</span> <span class="nam">annotations</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">__future__</span> <span class="key">import</span> <span class="nam">annotations</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">import</span> <span class="nam">argparse</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">import</span> <span class="nam">logging</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">import</span> <span class="nam">re</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">import</span> <span class="nam">argparse</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">import</span> <span class="nam">logging</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">import</span> <span class="nam">re</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="key">from</span> <span class="nam">pathlib</span> <span class="key">import</span> <span class="nam">Path</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="key">from</span> <span class="op">.</span> <span class="key">import</span> <span class="nam">cli</span><span class="op">,</span> <span class="nam">scm</span><span class="op">,</span> <span class="nam">tools</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="key">from</span> <span class="op">.</span> <span class="key">import</span> <span class="nam">cli</span><span class="op">,</span> <span class="nam">scm</span><span class="op">,</span> <span class="nam">tools</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="nam">log</span> <span class="op">=</span> <span class="nam">logging</span><span class="op">.</span><span class="nam">getLogger</span><span class="op">(</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="nam">log</span> <span class="op">=</span> <span class="nam">logging</span><span class="op">.</span><span class="nam">getLogger</span><span class="op">(</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="key">def</span> <span class="nam">add_arguments</span><span class="op">(</span><span class="nam">parser</span><span class="op">:</span> <span class="nam">argparse</span><span class="op">.</span><span class="nam">ArgumentParser</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span><span class="str">"--master"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"the 'master' branch"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="key">def</span> <span class="nam">add_arguments</span><span class="op">(</span><span class="nam">parser</span><span class="op">:</span> <span class="nam">argparse</span><span class="op">.</span><span class="nam">ArgumentParser</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span><span class="str">"--master"</span><span class="op">,</span> <span class="nam">help</span><span class="op">=</span><span class="str">"the 'master' branch"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">        <span class="str">"-w"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="str">"--workdir"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">help</span><span class="op">=</span><span class="str">"git working dir"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="nam">default</span><span class="op">=</span><span class="nam">Path</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="nam">type</span><span class="op">=</span><span class="nam">Path</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span><span class="str">"mode"</span><span class="op">,</span> <span class="nam">choices</span><span class="op">=</span><span class="op">[</span><span class="str">"micro"</span><span class="op">,</span> <span class="str">"minor"</span><span class="op">,</span> <span class="str">"major"</span><span class="op">,</span> <span class="str">"make-beta"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span><span class="str">"initfile"</span><span class="op">,</span> <span class="nam">metavar</span><span class="op">=</span><span class="str">"__init__.py"</span><span class="op">,</span> <span class="nam">type</span><span class="op">=</span><span class="nam">Path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span><span class="str">"mode"</span><span class="op">,</span> <span class="nam">choices</span><span class="op">=</span><span class="op">[</span><span class="str">"micro"</span><span class="op">,</span> <span class="str">"minor"</span><span class="op">,</span> <span class="str">"major"</span><span class="op">,</span> <span class="str">"make-beta"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">parser</span><span class="op">.</span><span class="nam">add_argument</span><span class="op">(</span><span class="str">"initfile"</span><span class="op">,</span> <span class="nam">metavar</span><span class="op">=</span><span class="str">"__init__.py"</span><span class="op">,</span> <span class="nam">type</span><span class="op">=</span><span class="nam">Path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="key">def</span> <span class="nam">process_options</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="key">def</span> <span class="nam">process_options</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="nam">options</span><span class="op">:</span> <span class="nam">argparse</span><span class="op">.</span><span class="nam">Namespace</span><span class="op">,</span> <span class="nam">error</span><span class="op">:</span> <span class="nam">cli</span><span class="op">.</span><span class="nam">ErrorFn</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">argparse</span><span class="op">.</span><span class="nam">Namespace</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span> <span class="op">=</span> <span class="nam">repo</span> <span class="op">=</span> <span class="nam">scm</span><span class="op">.</span><span class="nam">GitRepo</span><span class="op">(</span><span class="nam">options</span><span class="op">.</span><span class="nam">workdir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="nam">repo</span><span class="op">.</span><span class="nam">status</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="key">except</span> <span class="nam">scm</span><span class="op">.</span><span class="nam">GitError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">        <span class="nam">error</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span> <span class="op">=</span> <span class="nam">repo</span> <span class="op">=</span> <span class="nam">scm</span><span class="op">.</span><span class="nam">GitRepo</span><span class="op">(</span><span class="nam">options</span><span class="op">.</span><span class="nam">workdir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="nam">repo</span><span class="op">.</span><span class="nam">status</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="key">except</span> <span class="nam">scm</span><span class="op">.</span><span class="nam">GitError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">        <span class="nam">error</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">            <span class="str">"no git directory"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">            <span class="str">"It looks the repository is not a git repo"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">            <span class="nam">hint</span><span class="op">=</span><span class="str">"init the git directory"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="nam">log</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"working dir set to '%s'"</span><span class="op">,</span> <span class="nam">options</span><span class="op">.</span><span class="nam">workdir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="nam">branch</span> <span class="op">=</span> <span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">shorthand</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="nam">log</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"working dir set to '%s'"</span><span class="op">,</span> <span class="nam">options</span><span class="op">.</span><span class="nam">workdir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="nam">branch</span> <span class="op">=</span> <span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">shorthand</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="nam">log</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"current branch set to '%s'"</span><span class="op">,</span> <span class="nam">branch</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="key">except</span> <span class="nam">scm</span><span class="op">.</span><span class="nam">GitError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="nam">error</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="key">except</span> <span class="nam">scm</span><span class="op">.</span><span class="nam">GitError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="nam">error</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">            <span class="str">"invalid git repository"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">            <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t"><span class="str">              It looks the repository doesn't have any branch,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">              you should:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="str">                git checkout --orphan &lt;branch-name></span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t"><span class="str">              """</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">            <span class="nam">hint</span><span class="op">=</span><span class="str">"create a git branch"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="key">return</span> <span class="nam">options</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t"><span class="op">@</span><span class="nam">cli</span><span class="op">.</span><span class="nam">cli</span><span class="op">(</span><span class="nam">add_arguments</span><span class="op">,</span> <span class="nam">process_options</span><span class="op">,</span> <span class="nam">__doc__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t"><span class="key">def</span> <span class="nam">main</span><span class="op">(</span><span class="nam">options</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t"><span class="op">@</span><span class="nam">cli</span><span class="op">.</span><span class="nam">cli</span><span class="op">(</span><span class="nam">add_arguments</span><span class="op">,</span> <span class="nam">process_options</span><span class="op">,</span> <span class="nam">__doc__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t"><span class="key">def</span> <span class="nam">main</span><span class="op">(</span><span class="nam">options</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">    <span class="com"># master branch</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="nam">master</span> <span class="op">=</span> <span class="nam">options</span><span class="op">.</span><span class="nam">master</span> <span class="key">or</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="nam">master</span> <span class="op">=</span> <span class="nam">options</span><span class="op">.</span><span class="nam">master</span> <span class="key">or</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">config</span><span class="op">[</span><span class="str">"init.defaultbranch"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="key">if</span> <span class="str">"init.defaultbranch"</span> <span class="key">in</span> <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">config</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="key">else</span> <span class="str">"master"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">    <span class="key">if</span> <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">status</span><span class="op">(</span><span class="nam">untracked_files</span><span class="op">=</span><span class="str">"no"</span><span class="op">,</span> <span class="nam">ignored</span><span class="op">=</span><span class="key">False</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">    <span class="key">if</span> <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">status</span><span class="op">(</span><span class="nam">untracked_files</span><span class="op">=</span><span class="str">"no"</span><span class="op">,</span> <span class="nam">ignored</span><span class="op">=</span><span class="key">False</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">76&#x202F;&#x219B;&#x202F;77</span><span class="annotate long">line 76 didn't jump to line 77, because the condition on line 76 was never true</span></span></p>
     <p class="mis show_mis"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span><span class="str">f"modified files in {options.repo.workdir}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">options</span><span class="op">.</span><span class="nam">initfile</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span><span class="str">f"cannot find version file {options.initfile}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">options</span><span class="op">.</span><span class="nam">initfile</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span><span class="str">f"cannot find version file {options.initfile}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="nam">version</span> <span class="op">=</span> <span class="nam">tools</span><span class="op">.</span><span class="nam">get_module_var</span><span class="op">(</span><span class="nam">options</span><span class="op">.</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">    <span class="nam">log</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"got version %s for branch '%s'"</span><span class="op">,</span> <span class="nam">version</span><span class="op">,</span> <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">shorthand</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">version</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="nam">version</span> <span class="op">=</span> <span class="nam">tools</span><span class="op">.</span><span class="nam">get_module_var</span><span class="op">(</span><span class="nam">options</span><span class="op">.</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">    <span class="nam">log</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"got version %s for branch '%s'"</span><span class="op">,</span> <span class="nam">version</span><span class="op">,</span> <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">shorthand</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">version</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">83&#x202F;&#x219B;&#x202F;84</span><span class="annotate long">line 83 didn't jump to line 84, because the condition on line 83 was never true</span></span></p>
     <p class="mis show_mis"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="key">raise</span> <span class="nam">tools</span><span class="op">.</span><span class="nam">InvalidVersionError</span><span class="op">(</span><span class="str">f"cannot find a version in {options.initfile}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="com"># fetching all remotes</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">    <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"fetch"</span><span class="op">,</span> <span class="str">"--all"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">    <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"fetch"</span><span class="op">,</span> <span class="str">"--all"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="key">if</span> <span class="nam">options</span><span class="op">.</span><span class="nam">mode</span> <span class="op">==</span> <span class="str">"make-beta"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="key">if</span> <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">name</span> <span class="op">!=</span> <span class="str">f"refs/heads/{master}"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="key">if</span> <span class="nam">options</span><span class="op">.</span><span class="nam">mode</span> <span class="op">==</span> <span class="str">"make-beta"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="key">if</span> <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">name</span> <span class="op">!=</span> <span class="str">f"refs/heads/{master}"</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">90&#x202F;&#x219B;&#x202F;91</span><span class="annotate long">line 90 didn't jump to line 91, because the condition on line 90 was never true</span></span></p>
     <p class="mis show_mis"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">                <span class="str">f"wrong branch '{options.repo.head.name}', expected '{master}'"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="key">for</span> <span class="nam">branch</span> <span class="key">in</span> <span class="op">[</span><span class="op">*</span><span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">branches</span><span class="op">.</span><span class="nam">local</span><span class="op">,</span> <span class="op">*</span><span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">branches</span><span class="op">.</span><span class="nam">remote</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">branch</span><span class="op">.</span><span class="nam">endswith</span><span class="op">(</span><span class="str">f"beta/{version}"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">                <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span><span class="str">f"branch '{branch}' already present"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">        <span class="nam">log</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"creating branch '%s'"</span><span class="op">,</span> <span class="str">f"/beta/{version}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">branch</span><span class="op">(</span><span class="str">f"beta/{version}"</span><span class="op">,</span> <span class="nam">master</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span>  <span class="com"># noqa: T201</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="key">for</span> <span class="nam">branch</span> <span class="key">in</span> <span class="op">[</span><span class="op">*</span><span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">branches</span><span class="op">.</span><span class="nam">local</span><span class="op">,</span> <span class="op">*</span><span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">branches</span><span class="op">.</span><span class="nam">remote</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">branch</span><span class="op">.</span><span class="nam">endswith</span><span class="op">(</span><span class="str">f"beta/{version}"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">                <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span><span class="str">f"branch '{branch}' already present"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">        <span class="nam">log</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"creating branch '%s'"</span><span class="op">,</span> <span class="str">f"/beta/{version}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">branch</span><span class="op">(</span><span class="str">f"beta/{version}"</span><span class="op">,</span> <span class="nam">master</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span>  <span class="com"># noqa: T201</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">            <span class="nam">tools</span><span class="op">.</span><span class="nam">indent</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">                <span class="str">f"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t"><span class="str">        The release branch beta/{version} has been created.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t"><span class="str">        To complete the release:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="str">            git push origin beta/{version}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t"><span class="str">        To revert this beta branch:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t"><span class="str">            git branch -D beta/{version}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">            <span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">            <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">    <span class="key">elif</span> <span class="nam">options</span><span class="op">.</span><span class="nam">mode</span> <span class="key">in</span> <span class="op">{</span><span class="str">"micro"</span><span class="op">,</span> <span class="str">"minor"</span><span class="op">,</span> <span class="str">"major"</span><span class="op">}</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">    <span class="key">elif</span> <span class="nam">options</span><span class="op">.</span><span class="nam">mode</span> <span class="key">in</span> <span class="op">{</span><span class="str">"micro"</span><span class="op">,</span> <span class="str">"minor"</span><span class="op">,</span> <span class="str">"major"</span><span class="op">}</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">115&#x202F;&#x219B;&#x202F;165</span><span class="annotate long">line 115 didn't jump to line 165, because the condition on line 115 was never false</span></span></p>
     <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">        <span class="com"># we need to be in the beta/N.M.O branch</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">        <span class="nam">expr</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">compile</span><span class="op">(</span><span class="str">r"refs/heads/beta/(?P&lt;beta>\d+([.]\d+)*)$"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="op">(</span><span class="nam">match</span> <span class="op">:=</span> <span class="nam">expr</span><span class="op">.</span><span class="nam">search</span><span class="op">(</span><span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">name</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">        <span class="nam">expr</span> <span class="op">=</span> <span class="nam">re</span><span class="op">.</span><span class="nam">compile</span><span class="op">(</span><span class="str">r"refs/heads/beta/(?P&lt;beta>\d+([.]\d+)*)$"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="op">(</span><span class="nam">match</span> <span class="op">:=</span> <span class="nam">expr</span><span class="op">.</span><span class="nam">search</span><span class="op">(</span><span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">head</span><span class="op">.</span><span class="nam">name</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">                <span class="str">f"wrong branch '{options.repo.head.shorthand}'"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">                <span class="str">f"expected to be in 'beta/{version}' branch"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">                <span class="str">f"git checkout beta/{version}"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">            <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="nam">local</span> <span class="op">=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"beta"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">        <span class="key">if</span> <span class="nam">local</span> <span class="op">!=</span> <span class="nam">version</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="nam">local</span> <span class="op">=</span> <span class="nam">match</span><span class="op">.</span><span class="nam">group</span><span class="op">(</span><span class="str">"beta"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">        <span class="key">if</span> <span class="nam">local</span> <span class="op">!=</span> <span class="nam">version</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">126&#x202F;&#x219B;&#x202F;127</span><span class="annotate long">line 126 didn't jump to line 127, because the condition on line 126 was never true</span></span></p>
     <p class="mis show_mis"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span><span class="str">f"wrong version file {version=} != {local}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">        <span class="com"># create an empty commit to mark the release</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"commit"</span><span class="op">,</span> <span class="str">"--allow-empty"</span><span class="op">,</span> <span class="str">"-m"</span><span class="op">,</span> <span class="str">f"released {version}"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"commit"</span><span class="op">,</span> <span class="str">"--allow-empty"</span><span class="op">,</span> <span class="str">"-m"</span><span class="op">,</span> <span class="str">f"released {version}"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">        <span class="com"># tag</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"tag"</span><span class="op">,</span> <span class="str">"-a"</span><span class="op">,</span> <span class="str">f"release/{version}"</span><span class="op">,</span> <span class="str">"-m"</span><span class="op">,</span> <span class="str">f"released {version}"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"tag"</span><span class="op">,</span> <span class="str">"-a"</span><span class="op">,</span> <span class="str">f"release/{version}"</span><span class="op">,</span> <span class="str">"-m"</span><span class="op">,</span> <span class="str">f"released {version}"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">        <span class="com"># switch to master (and incorporate the commit message)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"checkout"</span><span class="op">,</span> <span class="nam">master</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"merge"</span><span class="op">,</span> <span class="str">f"beta/{version}"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"checkout"</span><span class="op">,</span> <span class="nam">master</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">(</span><span class="op">[</span><span class="str">"merge"</span><span class="op">,</span> <span class="str">f"beta/{version}"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="com"># bump version</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">        <span class="nam">new_version</span> <span class="op">=</span> <span class="nam">tools</span><span class="op">.</span><span class="nam">bump_version</span><span class="op">(</span><span class="nam">version</span><span class="op">,</span> <span class="nam">options</span><span class="op">.</span><span class="nam">mode</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">        <span class="nam">tools</span><span class="op">.</span><span class="nam">set_module_var</span><span class="op">(</span><span class="nam">options</span><span class="op">.</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">new_version</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">        <span class="nam">new_version</span> <span class="op">=</span> <span class="nam">tools</span><span class="op">.</span><span class="nam">bump_version</span><span class="op">(</span><span class="nam">version</span><span class="op">,</span> <span class="nam">options</span><span class="op">.</span><span class="nam">mode</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">        <span class="nam">tools</span><span class="op">.</span><span class="nam">set_module_var</span><span class="op">(</span><span class="nam">options</span><span class="op">.</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">"__version__"</span><span class="op">,</span> <span class="nam">new_version</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">        <span class="com"># commit</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">repo</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">initfile</span><span class="op">,</span> <span class="str">f"version bump {version} -> {new_version}"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span>  <span class="com"># noqa: T201</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span>  <span class="com"># noqa: T201</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">            <span class="nam">tools</span><span class="op">.</span><span class="nam">indent</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">                <span class="str">f"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t"><span class="str">        The release is almost complete.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t"><span class="str">        To complete the release:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t"><span class="str">            git push origin release/{version}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t"><span class="str">            git push origin master</span>&nbsp;</span><span class="r"></span></p>
@@ -257,13 +257,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_scm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 
-****** Coverage for src/hatch_ci/script.py: 0% ******
+****** Coverage for src/hatch_ci/script.py: 84% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x p   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 66 statements   0 run 66 missing 2 excluded 0 partial *****
+***** 66 statements   57 run 9 missing 2 excluded 5 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 20:13 +0000
+at 2023-08-07 20:20 +0000
 
 
 1"""create a beta branch or release a beta branch 
 2 
 3This script will either create a new beta branch: 
 4 
 5 hatch-ci make-beta ./src/package_name/__init__.py 
@@ -86,31 +86,36 @@
 69 # master branch 
 70 master = options.master or ( 
 71 options.repo.config["init.defaultbranch"] 
 72 if "init.defaultbranch" in options.repo.config 
 73 else "master" 
 74 ) 
 75 
-76 if options.repo.status(untracked_files="no", ignored=False): 
+76 if options.repo.status(untracked_files="no", ignored=False):
+ 76&#x202F;&#x219B;&#x202F;77line 76 didn't jump to line 77, because the
+condition on line 76 was never true
 77 options.error(f"modified files in {options.repo.workdir}") 
 78 if not options.initfile.exists(): 
 79 options.error(f"cannot find version file {options.initfile}") 
 80 
 81 version = tools.get_module_var(options.initfile, "__version__") 
 82 log.info("got version %s for branch '%s'", version,
 options.repo.head.shorthand) 
-83 if not version: 
+83 if not version: 83&#x202F;&#x219B;&#x202F;84line 83 didn't jump to line 84,
+because the condition on line 83 was never true
 84 raise tools.InvalidVersionError(f"cannot find a version in
 {options.initfile}") 
 85 
 86 # fetching all remotes 
 87 options.repo(["fetch", "--all"]) 
 88 
 89 if options.mode == "make-beta": 
-90 if options.repo.head.name != f"refs/heads/{master}": 
+90 if options.repo.head.name != f"refs/heads/{master}":
+ 90&#x202F;&#x219B;&#x202F;91line 90 didn't jump to line 91, because the
+condition on line 90 was never true
 91 options.error( 
 92 f"wrong branch '{options.repo.head.name}', expected '{master}'" 
 93 ) 
 94 
 95 for branch in [*options.repo.branches.local, *options.repo.branches.remote]:
  
 96 if not branch.endswith(f"beta/{version}"): 
@@ -128,26 +133,29 @@
 108 
 109 To revert this beta branch: 
 110 git branch -D beta/{version} 
 111 """ 
 112 ), 
 113 file=sys.stderr, 
 114 ) 
-115 elif options.mode in {"micro", "minor", "major"}: 
+115 elif options.mode in {"micro", "minor", "major"}:
+ 115&#x202F;&#x219B;&#x202F;165line 115 didn't jump to line 165, because the
+condition on line 115 was never false
 116 # we need to be in the beta/N.M.O branch 
 117 expr = re.compile(r"refs/heads/beta/(?P<beta>\d+([.]\d+)*)$") 
 118 if not (match := expr.search(options.repo.head.name)): 
 119 options.error( 
 120 f"wrong branch '{options.repo.head.shorthand}'", 
 121 f"expected to be in 'beta/{version}' branch", 
 122 f"git checkout beta/{version}", 
 123 ) 
 124 return 
 125 local = match.group("beta") 
-126 if local != version: 
+126 if local != version: 126&#x202F;&#x219B;&#x202F;127line 126 didn't jump to
+line 127, because the condition on line 126 was never true
 127 options.error(f"wrong version file {version=} != {local}") 
 128 
 129 # create an empty commit to mark the release 
 130 options.repo(["commit", "--allow-empty", "-m", f"released {version}"]) 
 131 
 132 # tag 
 133 options.repo(["tag", "-a", f"release/{version}", "-m", f"released
@@ -187,8 +195,8 @@
 166 raise RuntimeError(f"unsupported mode {options.mode=}") 
 167 
 168 
 169if __name__ == "__main__": 
 170 main() 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 20:13 +0000
+at 2023-08-07 20:20 +0000
```

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/d_7005a4ce5d73f943_tools_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -516,13 +516,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_script_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 224 statements   203 run 21 missing 0 excluded 11 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 20:13 +0000
+at 2023-08-07 20:20 +0000
 
 
 1# see https://pypi.org/project/setuptools-github 
 2# copy of setuptools_github.tools 
 3from __future__ import annotations 
 4 
 5import ast 
@@ -460,8 +460,8 @@
 425 for key, value in sorted((gdata or {}).items()): 
 426 value = f"'{value}'" if isinstance(value, str) else value 
 427 print(f"{key} = {value}", file=fp) 
 428 
 429 return data 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 20:13 +0000
+at 2023-08-07 20:20 +0000
```

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/d_7005a4ce5d73f943_version_hook_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -150,13 +150,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_tools_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 40 statements   0 run 40 missing 0 excluded 0 partial *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 20:13 +0000
+at 2023-08-07 20:20 +0000
 
 
 1from __future__ import annotations 
 2 
 3from typing import Any 
 4 
 5from hatchling.version.source.plugin.interface import VersionSourceInterface 
@@ -75,8 +75,8 @@
 59 ) 
 60 gdata = tools.process( 
 61 version_file, getenv("GITHUB_DUMP"), paths=paths, fixers=fixers 
 62 )[0] 
 63 return {"version": gdata["version"]} 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-08-07 20:13 +0000
+at 2023-08-07 20:20 +0000
```

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/favicon_32.png` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/favicon_32.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/index.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">59%</span>
+            <span class="pc_cov">74%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -43,15 +43,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -73,19 +73,19 @@
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_cli_py.html">src/hatch_ci/cli.py</a></td>
                 <td>72</td>
-                <td>72</td>
+                <td>49</td>
                 <td>0</td>
                 <td>18</td>
                 <td>0</td>
-                <td class="right" data-ratio="0 90">0%</td>
+                <td class="right" data-ratio="23 90">26%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_common_py.html">src/hatch_ci/common.py</a></td>
                 <td>1</td>
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
@@ -100,37 +100,37 @@
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 5">0%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_scm_py.html">src/hatch_ci/scm.py</a></td>
                 <td>162</td>
-                <td>27</td>
+                <td>12</td>
                 <td>0</td>
                 <td>52</td>
                 <td>8</td>
-                <td class="right" data-ratio="175 214">82%</td>
+                <td class="right" data-ratio="192 214">90%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_script_py.html">src/hatch_ci/script.py</a></td>
                 <td>66</td>
-                <td>66</td>
+                <td>9</td>
                 <td>2</td>
                 <td>20</td>
-                <td>0</td>
-                <td class="right" data-ratio="0 86">0%</td>
+                <td>5</td>
+                <td class="right" data-ratio="72 86">84%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_tools_py.html">src/hatch_ci/tools.py</a></td>
                 <td>224</td>
                 <td>21</td>
                 <td>0</td>
-                <td>98</td>
+                <td>102</td>
                 <td>11</td>
-                <td class="right" data-ratio="280 322">87%</td>
+                <td class="right" data-ratio="284 326">87%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_7005a4ce5d73f943_version_hook_py.html">src/hatch_ci/version_hook.py</a></td>
                 <td>40</td>
                 <td>40</td>
                 <td>0</td>
                 <td>14</td>
@@ -138,31 +138,31 @@
                 <td class="right" data-ratio="0 54">0%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td>572</td>
-                <td>232</td>
+                <td>137</td>
                 <td>2</td>
-                <td>202</td>
-                <td>19</td>
-                <td class="right" data-ratio="457 774">59%</td>
+                <td>206</td>
+                <td>24</td>
+                <td class="right" data-ratio="573 778">74%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-08-07 20:13 +0000
+            created at 2023-08-07 20:20 +0000
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_7005a4ce5d73f943_version_hook_py.html"/>
         <a id="nextFileLink" class="nav" href="d_7005a4ce5d73f943___init___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
 
-****** Coverage report: 59% ******
+****** Coverage report: 74% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-08-07 20:13 +0000
+coverage.py_v7.2.7, created at 2023-08-07 20:20 +0000
 
 Module                   statements missing excluded branches partial coverage
 src/hatch_ci/__init__.py 2          0       0        0        0       100%
-src/hatch_ci/cli.py      72         72      0        18       0       0%
+src/hatch_ci/cli.py      72         49      0        18       0       26%
 src/hatch_ci/common.py   1          1       0        0        0       0%
 src/hatch_ci/hooks.py    5          5       0        0        0       0%
-src/hatch_ci/scm.py      162        27      0        52       8       82%
-src/hatch_ci/script.py   66         66      2        20       0       0%
-src/hatch_ci/tools.py    224        21      0        98       11      87%
+src/hatch_ci/scm.py      162        12      0        52       8       90%
+src/hatch_ci/script.py   66         9       2        20       5       84%
+src/hatch_ci/tools.py    224        21      0        102      11      87%
 src/hatch_ci/            40         40      0        14       0       0%
 version_hook.py
-Total                    572        232     2        202      19      59%
+Total                    572        137     2        206      24      74%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-08-07 20:13 +0000
+coverage.py_v7.2.7, created at 2023-08-07 20:20 +0000
  ____
```

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/keybd_closed.png` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/keybd_open.png` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/keybd_open.png`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/status.json` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/status.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8667350589225589%*

 * *Differences: {"'files'": "{'d_7005a4ce5d73f943_cli_py': {'hash': 'a989fa299dc72d46ef5e594b93d5eb9d', 'index': "*

 * *            "{'nums': {insert: [(4, 49)], delete: [4]}}}, 'd_7005a4ce5d73f943_scm_py': {'hash': "*

 * *            "'ebfd36e2744eca065edf28598195d83a', 'index': {'nums': {insert: [(4, 12), (7, 10)], "*

 * *            "delete: [7, 4]}}}, 'd_7005a4ce5d73f943_script_py': {'hash': "*

 * *            "'f497cb12d07bcee92e3d49b6c7edb999', 'index': {'nums': {insert: [(4, 9), (6, 5), (7, "*

 * *            "5)], delete: [6, 5, 4]}}}, 'd_ […]*

```diff
@@ -14,23 +14,23 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/hatch_ci/__init__.py"
             }
         },
         "d_7005a4ce5d73f943_cli_py": {
-            "hash": "6434bcdee8d64d6b0c51317462cce110",
+            "hash": "a989fa299dc72d46ef5e594b93d5eb9d",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_cli_py.html",
                 "nums": [
                     0,
                     1,
                     72,
                     0,
-                    72,
+                    49,
                     18,
                     0,
                     18
                 ],
                 "relative_filename": "src/hatch_ci/cli.py"
             }
         },
@@ -65,58 +65,58 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/hatch_ci/hooks.py"
             }
         },
         "d_7005a4ce5d73f943_scm_py": {
-            "hash": "b208d1663706f031c634592ef10b4313",
+            "hash": "ebfd36e2744eca065edf28598195d83a",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_scm_py.html",
                 "nums": [
                     0,
                     1,
                     162,
                     0,
-                    27,
+                    12,
                     52,
                     8,
-                    12
+                    10
                 ],
                 "relative_filename": "src/hatch_ci/scm.py"
             }
         },
         "d_7005a4ce5d73f943_script_py": {
-            "hash": "8ee62da09a4cade164014211a2cdbea5",
+            "hash": "f497cb12d07bcee92e3d49b6c7edb999",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_script_py.html",
                 "nums": [
                     0,
                     1,
                     66,
                     2,
-                    66,
+                    9,
                     20,
-                    0,
-                    20
+                    5,
+                    5
                 ],
                 "relative_filename": "src/hatch_ci/script.py"
             }
         },
         "d_7005a4ce5d73f943_tools_py": {
-            "hash": "85d900cb995532ebb0a96d363886ec40",
+            "hash": "04f98b024bfde5286f870968087dae0f",
             "index": {
                 "html_filename": "d_7005a4ce5d73f943_tools_py.html",
                 "nums": [
                     0,
                     1,
                     224,
                     0,
                     21,
-                    98,
+                    102,
                     11,
                     21
                 ],
                 "relative_filename": "src/hatch_ci/tools.py"
             }
         },
         "d_7005a4ce5d73f943_version_hook_py": {
@@ -134,10 +134,10 @@
                     14
                 ],
                 "relative_filename": "src/hatch_ci/version_hook.py"
             }
         }
     },
     "format": 2,
-    "globals": "67047f35a6135996fb3c824e7903a7a4",
+    "globals": "e79ff11124a8fae1d4c0dc0f92821e1e",
     "version": "7.2.7"
 }
```

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/coverage/style.css` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/coverage/style.css`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/junit/junit.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/junit/junit.html`

 * *Files 11% similar despite different names*

```diff
@@ -435,62 +435,138 @@
     const rows = findAll('.results-table-row').filter(isAllRowsHidden);
     const allRowsHidden = rows.length == 0 ? true : false;
     const notFoundMessage = document.getElementById('not-found-message');
     notFoundMessage.hidden = !allRowsHidden;
 }
 </script>
     <h1>junit.html</h1>
-    <p>Report generated on 07-Aug-2023 at 20:13:25 by <a href="https://pypi.python.org/pypi/pytest-html">pytest-html</a> v3.2.0</p>
+    <p>Report generated on 07-Aug-2023 at 20:20:19 by <a href="https://pypi.python.org/pypi/pytest-html">pytest-html</a> v3.2.0</p>
     <h2>Summary</h2>
-    <p>16 tests ran in 1.49 seconds. </p>
-    <p class="filter" hidden="true">(Un)check the boxes to filter the results.</p><input checked="true" class="filter" data-test-result="passed" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="passed">16 passed</span>, <input checked="true" class="filter" data-test-result="skipped" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="skipped">0 skipped</span>, <input checked="true" class="filter" data-test-result="failed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="failed">0 failed</span>, <input checked="true" class="filter" data-test-result="error" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="error">0 errors</span>, <input checked="true" class="filter" data-test-result="xfailed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xfailed">0 expected failures</span>, <input checked="true" class="filter" data-test-result="xpassed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xpassed">0 unexpected passes</span>
+    <p>20 tests ran in 1.17 seconds. </p>
+    <p class="filter" hidden="true">(Un)check the boxes to filter the results.</p><input checked="true" class="filter" data-test-result="passed" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="passed">20 passed</span>, <input checked="true" class="filter" data-test-result="skipped" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="skipped">0 skipped</span>, <input checked="true" class="filter" data-test-result="failed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="failed">0 failed</span>, <input checked="true" class="filter" data-test-result="error" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="error">0 errors</span>, <input checked="true" class="filter" data-test-result="xfailed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xfailed">0 expected failures</span>, <input checked="true" class="filter" data-test-result="xpassed" disabled="true" hidden="true" name="filter_checkbox" onChange="filterTable(this)" type="checkbox"/><span class="xpassed">0 unexpected passes</span>
     <h2>Results</h2>
     <table id="results-table">
       <thead id="results-table-head">
         <tr>
           <th class="sortable result initial-sort" col="result">Result</th>
           <th class="sortable" col="name">Test</th>
           <th class="sortable" col="duration">Duration</th>
           <th class="sortable links" col="links">Links</th></tr>
         <tr hidden="true" id="not-found-message">
           <th colspan="4">No results found. Try to check the filters</th></tr></thead>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_scm.py::test_lookup</td>
-          <td class="col-duration">0.04</td>
+          <td class="col-duration">0.02</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_scm.py::test_handle_remote_and_local_repos</td>
-          <td class="col-duration">0.32</td>
+          <td class="col-duration">0.18</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.3&#x27;
 Switched to a new branch &#x27;beta/0.0.4&#x27;
 Switched to branch &#x27;master&#x27;
 Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-repo1&#x27;...
 done.
 Switched to a new branch &#x27;beta/0.0.2&#x27;
-Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/0C95EU&#x27;...
+Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/VX4USL&#x27;...
 done.
 Switched to a new branch &#x27;beta/0.0.1&#x27;
 fatal: a branch named &#x27;master&#x27; already exists
 From /tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/test_check_version-repo1
  * [new branch]      beta/0.0.2 -&gt; repo1/beta/0.0.2
  * [new branch]      master     -&gt; repo1/master
 <br/></div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
+          <td class="col-name">tests/test_script.py::test_add_arguments</td>
+          <td class="col-duration">0.00</td>
+          <td class="col-links"></td></tr>
+        <tr>
+          <td class="extra" colspan="4">
+            <div class="empty log">No log output captured.</div></td></tr></tbody>
+      <tbody class="passed results-table-row">
+        <tr>
+          <td class="col-result">Passed</td>
+          <td class="col-name">tests/test_script.py::test_process_options</td>
+          <td class="col-duration">0.01</td>
+          <td class="col-links"></td></tr>
+        <tr>
+          <td class="extra" colspan="4">
+            <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>fatal: not a git repository: &#x27;/tmp/pytest-of-runner/pytest-0/test_process_options0/.git&#x27;
+hint: Using &#x27;master&#x27; as the name for the initial branch. This default branch name
+hint: is subject to change. To configure the initial branch name to use in all
+hint: of your new repositories, which will suppress this warning, call:
+hint: 
+hint: 	git config --global init.defaultBranch &lt;name&gt;
+hint: 
+hint: Names commonly chosen instead of &#x27;master&#x27; are &#x27;main&#x27;, &#x27;trunk&#x27; and
+hint: &#x27;development&#x27;. The just-created branch can be renamed via this command:
+hint: 
+hint: 	git branch -m &lt;name&gt;
+fatal: ambiguous argument &#x27;refs/heads/master&#x27;: unknown revision or path not in the working tree.
+Use &#x27;--&#x27; to separate paths from revisions, like this:
+&#x27;git &lt;command&gt; [&lt;revision&gt;...] -- [&lt;file&gt;...]&#x27;
+<br/></div></td></tr></tbody>
+      <tbody class="passed results-table-row">
+        <tr>
+          <td class="col-result">Passed</td>
+          <td class="col-name">tests/test_script.py::test_main_make_beta</td>
+          <td class="col-duration">0.08</td>
+          <td class="col-links"></td></tr>
+        <tr>
+          <td class="extra" colspan="4">
+            <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.0&#x27;
+  
+  The release branch beta/0.0.0 has been created.
+  
+  To complete the release:
+      git push origin beta/0.0.0
+  
+  To revert this beta branch:
+      git branch -D beta/0.0.0
+
+Switched to branch &#x27;master&#x27;
+<br/></div></td></tr></tbody>
+      <tbody class="passed results-table-row">
+        <tr>
+          <td class="col-result">Passed</td>
+          <td class="col-name">tests/test_script.py::test_main_make_release</td>
+          <td class="col-duration">0.09</td>
+          <td class="col-links"></td></tr>
+        <tr>
+          <td class="extra" colspan="4">
+            <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.0&#x27;
+Switched to branch &#x27;master&#x27;
+Switched to branch &#x27;beta/0.0.0&#x27;
+Switched to branch &#x27;master&#x27;
+  
+  The release is almost complete.
+  
+  To complete the release:
+      git push origin release/0.0.0
+      git push origin master
+  
+  To revert this release:
+      git reset --hard HEAD~1
+      git tag -d release/0.0.0
+
+<br/></div></td></tr></tbody>
+      <tbody class="passed results-table-row">
+        <tr>
+          <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_abort_exception</td>
           <td class="col-duration">0.00</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
@@ -574,47 +650,47 @@
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_update_version_master</td>
-          <td class="col-duration">0.06</td>
+          <td class="col-duration">0.03</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="empty log">No log output captured.</div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_update_version_beta</td>
-          <td class="col-duration">0.14</td>
+          <td class="col-duration">0.07</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.4&#x27;
 Updated 1 path from the index
 Updated 1 path from the index
 Switched to a new branch &#x27;beta/0.0.2&#x27;
 <br/></div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_update_version_release</td>
-          <td class="col-duration">0.08</td>
+          <td class="col-duration">0.04</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Switched to a new branch &#x27;beta/0.0.3&#x27;
 Updated 1 path from the index
 <br/></div></td></tr></tbody>
       <tbody class="passed results-table-row">
         <tr>
           <td class="col-result">Passed</td>
           <td class="col-name">tests/test_tools.py::test_process</td>
-          <td class="col-duration">0.17</td>
+          <td class="col-duration">0.10</td>
           <td class="col-links"></td></tr>
         <tr>
           <td class="extra" colspan="4">
             <div class="log"> ------------------------------Captured stderr call------------------------------ <br/>Updated 1 path from the index
 Switched to a new branch &#x27;beta/1.2.3&#x27;
 <br/></div></td></tr></tbody></table></body></html>
```

#### html2text {}

```diff
@@ -1,32 +1,64 @@
 ****** junit.html ******
-Report generated on 07-Aug-2023 at 20:13:25 by pytest-html v3.2.0
+Report generated on 07-Aug-2023 at 20:20:19 by pytest-html v3.2.0
 ***** Summary *****
-16 tests ran in 1.49 seconds.
+20 tests ran in 1.17 seconds.
 (Un)check the boxes to filter the results.
-*16 passed, *0 skipped, *0 failed, *0 errors, *0 expected failures, *0
+*20 passed, *0 skipped, *0 failed, *0 errors, *0 expected failures, *0
 unexpected passes
 ***** Results *****
 Result Test                                                  Duration Links
 No results found. Try to check the filters
-Passed tests/test_scm.py::test_lookup                        0.04
+Passed tests/test_scm.py::test_lookup                        0.02
 No log output captured.
-Passed tests/test_scm.py::test_handle_remote_and_local_repos 0.32
+Passed tests/test_scm.py::test_handle_remote_and_local_repos 0.18
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.3&#x27; Switched to a new branch
 &#x27;beta/0.0.4&#x27; Switched to branch &#x27;master&#x27; Cloning into
 &#x27;/tmp/pytest-of-runner/pytest-0/test_handle_remote_and_local_r0/
 test_check_version-repo1&#x27;... done. Switched to a new branch &#x27;beta/
 0.0.2&#x27; Cloning into &#x27;/tmp/pytest-of-runner/pytest-0/
-test_handle_remote_and_local_r0/0C95EU&#x27;... done. Switched to a new
+test_handle_remote_and_local_r0/VX4USL&#x27;... done. Switched to a new
 branch &#x27;beta/0.0.1&#x27; fatal: a branch named &#x27;master&#x27;
 already exists From /tmp/pytest-of-runner/pytest-0/
 test_handle_remote_and_local_r0/test_check_version-repo1 * [new branch]
 beta/0.0.2 -> repo1/beta/0.0.2 * [new branch] master -> repo1/master
+Passed tests/test_script.py::test_add_arguments              0.00
+No log output captured.
+Passed tests/test_script.py::test_process_options            0.01
+------------------------------Captured stderr call--------------------------
+----
+fatal: not a git repository: &#x27;/tmp/pytest-of-runner/pytest-0/
+test_process_options0/.git&#x27; hint: Using &#x27;master&#x27; as the name
+for the initial branch. This default branch name hint: is subject to change.
+To configure the initial branch name to use in all hint: of your new
+repositories, which will suppress this warning, call: hint: hint: git config
+--global init.defaultBranch <name> hint: hint: Names commonly chosen instead
+of &#x27;master&#x27; are &#x27;main&#x27;, &#x27;trunk&#x27; and hint:
+&#x27;development&#x27;. The just-created branch can be renamed via this
+command: hint: hint: git branch -m <name> fatal: ambiguous argument
+&#x27;refs/heads/master&#x27;: unknown revision or path not in the working
+tree. Use &#x27;--&#x27; to separate paths from revisions, like this:
+&#x27;git <command> [<revision>...] -- [<file>...]&#x27;
+Passed tests/test_script.py::test_main_make_beta             0.08
+------------------------------Captured stderr call--------------------------
+----
+Switched to a new branch &#x27;beta/0.0.0&#x27; The release branch beta/
+0.0.0 has been created. To complete the release: git push origin beta/0.0.0
+To revert this beta branch: git branch -D beta/0.0.0 Switched to branch
+&#x27;master&#x27;
+Passed tests/test_script.py::test_main_make_release          0.09
+------------------------------Captured stderr call--------------------------
+----
+Switched to a new branch &#x27;beta/0.0.0&#x27; Switched to branch
+&#x27;master&#x27; Switched to branch &#x27;beta/0.0.0&#x27; Switched to
+branch &#x27;master&#x27; The release is almost complete. To complete the
+release: git push origin release/0.0.0 git push origin master To revert this
+release: git reset --hard HEAD~1 git tag -d release/0.0.0
 Passed tests/test_tools.py::test_abort_exception             0.00
 No log output captured.
 Passed tests/test_tools.py::test_urmtree                     0.00
 No log output captured.
 Passed tests/test_tools.py::test_indent                      0.00
 No log output captured.
 Passed tests/test_tools.py::test_list_of_paths               0.00
@@ -39,25 +71,25 @@
 No log output captured.
 Passed tests/test_tools.py::test_set_module_var              0.00
 No log output captured.
 Passed tests/test_tools.py::test_set_module_var_empty_file   0.00
 No log output captured.
 Passed tests/test_tools.py::test_bump_version                0.00
 No log output captured.
-Passed tests/test_tools.py::test_update_version_master       0.06
+Passed tests/test_tools.py::test_update_version_master       0.03
 No log output captured.
-Passed tests/test_tools.py::test_update_version_beta         0.14
+Passed tests/test_tools.py::test_update_version_beta         0.07
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.4&#x27; Updated 1 path from the
 index Updated 1 path from the index Switched to a new branch &#x27;beta/
 0.0.2&#x27;
-Passed tests/test_tools.py::test_update_version_release      0.08
+Passed tests/test_tools.py::test_update_version_release      0.04
 ------------------------------Captured stderr call--------------------------
 ----
 Switched to a new branch &#x27;beta/0.0.3&#x27; Updated 1 path from the
 index
-Passed tests/test_tools.py::test_process                     0.17
+Passed tests/test_tools.py::test_process                     0.10
 ------------------------------Captured stderr call--------------------------
 ----
 Updated 1 path from the index Switched to a new branch &#x27;beta/
 1.2.3&#x27;
```

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/junit/junit.xml` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/junit/junit.xml`

 * *Files 5% similar despite different names*

#### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/junit/junit.xml` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/junit/junit.xml`

```diff
@@ -1,21 +1,25 @@
 <?xml version="1.0" encoding="utf-8"?>
 <testsuites>
-  <testsuite name="pytest" errors="0" failures="0" skipped="0" tests="16" time="1.468" timestamp="2023-08-07T20:13:23.703498" hostname="fv-az563-119">
-    <testcase classname="tests.test_scm" name="test_lookup" time="0.046"/>
-    <testcase classname="tests.test_scm" name="test_handle_remote_and_local_repos" time="0.329"/>
-    <testcase classname="tests.test_tools" name="test_abort_exception" time="0.002"/>
-    <testcase classname="tests.test_tools" name="test_urmtree" time="0.002"/>
+  <testsuite name="pytest" errors="0" failures="0" skipped="0" tests="20" time="1.165" timestamp="2023-08-07T20:20:18.551384" hostname="fv-az248-184">
+    <testcase classname="tests.test_scm" name="test_lookup" time="0.024"/>
+    <testcase classname="tests.test_scm" name="test_handle_remote_and_local_repos" time="0.185"/>
+    <testcase classname="tests.test_script" name="test_add_arguments" time="0.001"/>
+    <testcase classname="tests.test_script" name="test_process_options" time="0.017"/>
+    <testcase classname="tests.test_script" name="test_main_make_beta" time="0.086"/>
+    <testcase classname="tests.test_script" name="test_main_make_release" time="0.090"/>
+    <testcase classname="tests.test_tools" name="test_abort_exception" time="0.001"/>
+    <testcase classname="tests.test_tools" name="test_urmtree" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_indent" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_list_of_paths" time="0.001"/>
     <testcase classname="tests.test_tools" name="test_lstrip" time="0.001"/>
-    <testcase classname="tests.test_tools" name="test_apply_fixers" time="0.004"/>
-    <testcase classname="tests.test_tools" name="test_get_module_var" time="0.003"/>
-    <testcase classname="tests.test_tools" name="test_set_module_var" time="0.007"/>
-    <testcase classname="tests.test_tools" name="test_set_module_var_empty_file" time="0.003"/>
+    <testcase classname="tests.test_tools" name="test_apply_fixers" time="0.003"/>
+    <testcase classname="tests.test_tools" name="test_get_module_var" time="0.002"/>
+    <testcase classname="tests.test_tools" name="test_set_module_var" time="0.003"/>
+    <testcase classname="tests.test_tools" name="test_set_module_var_empty_file" time="0.002"/>
     <testcase classname="tests.test_tools" name="test_bump_version" time="0.001"/>
-    <testcase classname="tests.test_tools" name="test_update_version_master" time="0.065"/>
-    <testcase classname="tests.test_tools" name="test_update_version_beta" time="0.142"/>
-    <testcase classname="tests.test_tools" name="test_update_version_release" time="0.083"/>
-    <testcase classname="tests.test_tools" name="test_process" time="0.173"/>
+    <testcase classname="tests.test_tools" name="test_update_version_master" time="0.038"/>
+    <testcase classname="tests.test_tools" name="test_update_version_beta" time="0.078"/>
+    <testcase classname="tests.test_tools" name="test_update_version_release" time="0.048"/>
+    <testcase classname="tests.test_tools" name="test_process" time="0.107"/>
   </testsuite>
 </testsuites>
```

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/index.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 <thead><tr class="summary">
 <th class="summary">File</th>
 <th class="summary">Imprecision</th>
 <th class="summary">Lines</th>
 </tr></thead>
 <tfoot><tr class="summary summary-quality-1">
 <th class="summary summary-filename">Total</th>
-<th class="summary summary-precision">18.88% imprecise</th>
+<th class="summary summary-precision">18.98% imprecise</th>
 <th class="summary summary-lines">1075 LOC</th>
 </tr></tfoot>
 <tbody>
 <tr class="summary summary-quality-0">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/__init__.py.html">hatch_ci</a></td>
 <td class="summary summary-precision">0.00% imprecise</td>
 <td class="summary summary-lines">2 LOC</td>
@@ -46,15 +46,15 @@
 <tr class="summary summary-quality-2">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/script.py.html">hatch_ci.script</a></td>
 <td class="summary summary-precision">26.47% imprecise</td>
 <td class="summary summary-lines">170 LOC</td>
 </tr>
 <tr class="summary summary-quality-2">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/tools.py.html">hatch_ci.tools</a></td>
-<td class="summary summary-precision">20.28% imprecise</td>
+<td class="summary summary-precision">20.51% imprecise</td>
 <td class="summary summary-lines">429 LOC</td>
 </tr>
 <tr class="summary summary-quality-2">
 <td class="summary summary-filename"><a href="html/src/hatch_ci/version_hook.py.html">hatch_ci.version_hook</a></td>
 <td class="summary summary-precision">26.98% imprecise</td>
 <td class="summary summary-lines">63 LOC</td>
 </tr>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 
 ****** Mypy Type Check Coverage Summary ******
               Summary from index
 File                  Imprecision      Lines
-Total                 18.88% imprecise 1075 LOC
+Total                 18.98% imprecise 1075 LOC
 hatch_ci              0.00% imprecise  2 LOC
 hatch_ci.cli          19.85% imprecise 136 LOC
 hatch_ci.common       0.00% imprecise  1 LOC
 hatch_ci.hooks        37.50% imprecise 8 LOC
 hatch_ci.scm          9.02% imprecise  266 LOC
 hatch_ci.script       26.47% imprecise 170 LOC
-hatch_ci.tools        20.28% imprecise 429 LOC
+hatch_ci.tools        20.51% imprecise 429 LOC
 hatch_ci.version_hook 26.98% imprecise 63 LOC
```

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/mypy-html.css` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/mypy-html.css`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/html/src/hatch_ci/__init__.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/html/src/hatch_ci/cli.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/html/src/hatch_ci/common.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/html/src/hatch_ci/hooks.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/html/src/hatch_ci/scm.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/html/src/hatch_ci/script.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/html/src/hatch_ci/tools.py.html`

 * *Files 0% similar despite different names*

```diff
@@ -620,17 +620,18 @@
 <span class="line-any" title="No Anys on this line!">                        continue</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x2)
 Explicit (x6)">                    if not isinstance(subnode.value, (ast.Num, ast.Str, ast.Constant)):</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x1)">                        raise ValidationError(</span>
 <span class="line-any" title="Any Types on this line: 
-Unannotated (x10)
-Explicit (x2)">                            f"cannot extract non Constant variable "</span>
-<span class="line-empty" title="No Anys on this line!">                            f"{target.id} ({type(subnode.value)})"</span>
+Unannotated (x8)">                            f"cannot extract non Constant variable "</span>
+<span class="line-any" title="Any Types on this line: 
+Unannotated (x2)
+Explicit (x2)">                            f"{target.id} ({type(subnode.value)})"</span>
 <span class="line-empty" title="No Anys on this line!">                        )</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x2)
 Explicit (x2)">                    if isinstance(subnode.value, ast.Str):</span>
 <span class="line-any" title="Any Types on this line: 
 Unannotated (x2)">                        value = subnode.value.s</span>
 <span class="line-any" title="Any Types on this line: 
@@ -848,17 +849,18 @@
 <span class="line-precise" title="No Anys on this line!">        match1 = expr1.search(current or "")</span>
 <span class="line-precise" title="No Anys on this line!">        if not match1:</span>
 <span class="line-precise" title="No Anys on this line!">            raise InvalidVersionError(f"cannot parse current version '{current}'")</span>
 <span class="line-imprecise" title="Any Types on this line: 
 Explicit (x7)">        if match1.group("version") != match.group("version"):</span>
 <span class="line-precise" title="No Anys on this line!">            raise InvalidVersionError(</span>
 <span class="line-any" title="Any Types on this line: 
-Explicit (x6)
-Omitted Generics (x4)">                f"building package for {current} from '{gdata['ref']}' "</span>
-<span class="line-empty" title="No Anys on this line!">                f"branch ({match.groupdict()} mismatch {match1.groupdict()})"</span>
+Explicit (x4)">                f"building package for {current} from '{gdata['ref']}' "</span>
+<span class="line-precise" title="Any Types on this line: 
+Explicit (x2)
+Omitted Generics (x4)">                f"branch ({match.groupdict()} mismatch {match1.groupdict()})"</span>
 <span class="line-empty" title="No Anys on this line!">            )</span>
 <span class="line-imprecise" title="Any Types on this line: 
 Explicit (x4)">        if match.group("what") == "beta":</span>
 <span class="line-any" title="Any Types on this line: 
 Explicit (x5)">            result["version"] = f"{match1.group('version')}b{gdata['run_number']}"</span>
 <span class="line-precise" title="No Anys on this line!">            result["workflow"] = "beta"</span>
 <span class="line-empty" title="No Anys on this line!">        else:</span>
```

### Comparing `hatch_ci-0.0.8b32/build/qa-3.8-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html` & `hatch_ci-0.0.8b33/build/qa-3.10-ubuntu-latest/mypy/html/src/hatch_ci/version_hook.py.html`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/src/hatch_ci/cli.py` & `hatch_ci-0.0.8b33/src/hatch_ci/cli.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/src/hatch_ci/scm.py` & `hatch_ci-0.0.8b33/src/hatch_ci/scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/src/hatch_ci/script.py` & `hatch_ci-0.0.8b33/src/hatch_ci/script.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/src/hatch_ci/tools.py` & `hatch_ci-0.0.8b33/src/hatch_ci/tools.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/src/hatch_ci/version_hook.py` & `hatch_ci-0.0.8b33/src/hatch_ci/version_hook.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/tests/conftest.py` & `hatch_ci-0.0.8b33/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/tests/test_scm.py` & `hatch_ci-0.0.8b33/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/tests/test_tools.py` & `hatch_ci-0.0.8b33/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/LICENSE.txt` & `hatch_ci-0.0.8b33/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/README.md` & `hatch_ci-0.0.8b33/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
-[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/5789474090)
+[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/5789534498)
 [![codecov](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.0.8/graph/badge.svg?token=521FB9K5KT)](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.0.8)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
```

### Comparing `hatch_ci-0.0.8b32/pyproject.toml` & `hatch_ci-0.0.8b33/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_ci-0.0.8b32/PKG-INFO` & `hatch_ci-0.0.8b33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-ci
-Version: 0.0.8b32
+Version: 0.0.8b33
 Summary: Hatch plugin for ci system versioning
 Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
 Project-URL: Source, https://github.com/cav71/hatch-ci
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 License-File: LICENSE.txt
 Keywords: git,hatch,plugin,scm,version
@@ -24,15 +24,15 @@
 
 # hatch-ci
 
 [![PyPI version](https://img.shields.io/pypi/v/hatch-ci.svg?color=blue)](https://pypi.org/project/hatch-ci)
 [![Python versions](https://img.shields.io/pypi/pyversions/hatch-ci.svg)](https://pypi.org/project/hatch-ci)
 [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/)
 
-[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/5789474090)
+[![Build](https://github.com/cav71/hatch-ci/actions/workflows/beta.yml/badge.svg)](https://github.com/cav71/hatch-ci/actions/runs/5789534498)
 [![codecov](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.0.8/graph/badge.svg?token=521FB9K5KT)](https://codecov.io/gh/cav71/hatch-ci/branch/beta%2F0.0.8)
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](Black)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
```

