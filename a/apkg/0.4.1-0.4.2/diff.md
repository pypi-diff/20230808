# Comparing `tmp/apkg-0.4.1.tar.gz` & `tmp/apkg-0.4.2.tar.gz`

## Comparing `apkg-0.4.1.tar` & `apkg-0.4.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.4.1/CHANGELOG.md -> docs/news.md
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 apkg-0.4.1/requirements.txt
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 apkg-0.4.1/setup.cfg
--rwxr-xr-x   0        0        0      627 2020-02-02 00:00:00.000000 apkg-0.4.1/setup.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/__init__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/__main__.py
--rw-r--r--   0        0        0     8023 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/adistro.py
--rw-r--r--   0        0        0     5531 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/cache.py
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/cli.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/compat.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/ex.py
--rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/log.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/parse.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/pkgstyle.py
--rw-r--r--   0        0        0     8101 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/pkgtemplate.py
--rw-r--r--   0        0        0    12761 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/pkgtest.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/project.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/terminal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/__init__.py
--rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/build.py
--rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/build_dep.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/clean.py
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/compat.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/get_archive.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/info.py
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/install.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/make_archive.py
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/srcpkg.py
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/status.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/system_setup.py
--rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/test.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/commands/test_dep.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/pkgstyles/__init__.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/pkgstyles/arch.py
--rw-r--r--   0        0        0    10446 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/pkgstyles/deb.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/pkgstyles/nix.py
--rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/pkgstyles/rpm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/util/__init__.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/util/archive.py
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/util/common.py
--rw-r--r--   0        0        0     8794 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/util/git.py
--rw-r--r--   0        0        0     7775 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/util/run.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/util/shutil35.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/util/test.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 apkg-0.4.1/apkg/util/upstreamversion.py
--rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 apkg-0.4.1/scripts/make-archive.sh
--rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 apkg-0.4.1/scripts/upstream-version.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 apkg-0.4.1/.gitignore
--rw-r--r--   0        0        0    35427 2020-02-02 00:00:00.000000 apkg-0.4.1/COPYING
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 apkg-0.4.1/README.md
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 apkg-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 apkg-0.4.1/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.4.2/CHANGELOG.md -> docs/news.md
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 apkg-0.4.2/requirements.txt
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 apkg-0.4.2/setup.cfg
+-rwxr-xr-x   0        0        0      627 2020-02-02 00:00:00.000000 apkg-0.4.2/setup.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/__init__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/__main__.py
+-rw-r--r--   0        0        0     8023 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/adistro.py
+-rw-r--r--   0        0        0     5531 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/cache.py
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/cli.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/compat.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/ex.py
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/log.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/parse.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/pkgstyle.py
+-rw-r--r--   0        0        0     8101 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/pkgtemplate.py
+-rw-r--r--   0        0        0    12761 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/pkgtest.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/project.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/terminal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/__init__.py
+-rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/build.py
+-rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/build_dep.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/clean.py
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/compat.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/get_archive.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/info.py
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/install.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/make_archive.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/srcpkg.py
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/status.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/system_setup.py
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/test.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/commands/test_dep.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/pkgstyles/__init__.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/pkgstyles/arch.py
+-rw-r--r--   0        0        0    10446 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/pkgstyles/deb.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/pkgstyles/nix.py
+-rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/pkgstyles/rpm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/util/__init__.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/util/archive.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/util/common.py
+-rw-r--r--   0        0        0     8794 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/util/git.py
+-rw-r--r--   0        0        0     7775 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/util/run.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/util/shutil35.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/util/test.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 apkg-0.4.2/apkg/util/upstreamversion.py
+-rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 apkg-0.4.2/scripts/make-archive.sh
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 apkg-0.4.2/scripts/upstream-version.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 apkg-0.4.2/.gitignore
+-rw-r--r--   0        0        0    35427 2020-02-02 00:00:00.000000 apkg-0.4.2/COPYING
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 apkg-0.4.2/README.md
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 apkg-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 apkg-0.4.2/PKG-INFO
```

### Comparing `apkg-0.4.1/setup.cfg` & `apkg-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/setup.py` & `apkg-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/adistro.py` & `apkg-0.4.2/apkg/adistro.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/cache.py` & `apkg-0.4.2/apkg/cache.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/cli.py` & `apkg-0.4.2/apkg/cli.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/compat.py` & `apkg-0.4.2/apkg/compat.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/ex.py` & `apkg-0.4.2/apkg/ex.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/log.py` & `apkg-0.4.2/apkg/log.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/parse.py` & `apkg-0.4.2/apkg/parse.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/pkgstyle.py` & `apkg-0.4.2/apkg/pkgstyle.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/pkgtemplate.py` & `apkg-0.4.2/apkg/pkgtemplate.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/pkgtest.py` & `apkg-0.4.2/apkg/pkgtest.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/project.py` & `apkg-0.4.2/apkg/project.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/terminal.py` & `apkg-0.4.2/apkg/terminal.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/commands/build.py` & `apkg-0.4.2/apkg/commands/build.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/commands/build_dep.py` & `apkg-0.4.2/apkg/commands/build_dep.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/commands/clean.py` & `apkg-0.4.2/apkg/commands/clean.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/commands/compat.py` & `apkg-0.4.2/apkg/commands/compat.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/commands/get_archive.py` & `apkg-0.4.2/apkg/commands/get_archive.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/commands/info.py` & `apkg-0.4.2/apkg/commands/info.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/commands/install.py` & `apkg-0.4.2/apkg/commands/install.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/commands/make_archive.py` & `apkg-0.4.2/apkg/commands/make_archive.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/commands/srcpkg.py` & `apkg-0.4.2/apkg/commands/srcpkg.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/commands/status.py` & `apkg-0.4.2/apkg/commands/status.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/commands/system_setup.py` & `apkg-0.4.2/apkg/commands/system_setup.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/commands/test.py` & `apkg-0.4.2/apkg/commands/test.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/commands/test_dep.py` & `apkg-0.4.2/apkg/commands/test_dep.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/pkgstyles/arch.py` & `apkg-0.4.2/apkg/pkgstyles/arch.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/pkgstyles/deb.py` & `apkg-0.4.2/apkg/pkgstyles/deb.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/pkgstyles/nix.py` & `apkg-0.4.2/apkg/pkgstyles/nix.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/pkgstyles/rpm.py` & `apkg-0.4.2/apkg/pkgstyles/rpm.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/util/archive.py` & `apkg-0.4.2/apkg/util/archive.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/util/common.py` & `apkg-0.4.2/apkg/util/common.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/util/git.py` & `apkg-0.4.2/apkg/util/git.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/util/run.py` & `apkg-0.4.2/apkg/util/run.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/util/shutil35.py` & `apkg-0.4.2/apkg/util/shutil35.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/util/test.py` & `apkg-0.4.2/apkg/util/test.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/apkg/util/upstreamversion.py` & `apkg-0.4.2/apkg/util/upstreamversion.py`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/scripts/make-archive.sh` & `apkg-0.4.2/scripts/make-archive.sh`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/COPYING` & `apkg-0.4.2/COPYING`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/README.md` & `apkg-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `apkg-0.4.1/pyproject.toml` & `apkg-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "beautifulsoup4",
     "blessed",
+    "cached_property",
     "click",
     "distro",
     "jinja2",
     "packaging",
     "requests",
     "toml",
 ]
```

### Comparing `apkg-0.4.1/PKG-INFO` & `apkg-0.4.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkg
-Version: 0.4.1
+Version: 0.4.2
 Summary: cross-distro upstream packaging automation tool
 Project-URL: Documentation, https://gitlab.nic.cz/packaging/apkg/-/blob/master/README.md
 Project-URL: Issues, https://gitlab.nic.cz/packaging/apkg/-/issues
 Project-URL: Source, https://gitlab.nic.cz/packaging/apkg
 Author-email: Jakub Ružička <jakub.ruzicka@nic.cz>
 License: MIT
 License-File: COPYING
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: beautifulsoup4
 Requires-Dist: blessed
+Requires-Dist: cached-property
 Requires-Dist: click
 Requires-Dist: distro
 Requires-Dist: jinja2
 Requires-Dist: packaging
 Requires-Dist: requests
 Requires-Dist: toml
 Description-Content-Type: text/markdown
```

