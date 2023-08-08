# Comparing `tmp/venv-management-2.0.3.tar.gz` & `tmp/venv-management-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venv-management-2.0.3.tar", last modified: Tue Aug  8 13:13:06 2023, max compression
+gzip compressed data, was "venv-management-2.0.4.tar", last modified: Tue Aug  8 13:13:08 2023, max compression
```

## Comparing `venv-management-2.0.3.tar` & `venv-management-2.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:06.188081 venv-management-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-08 13:12:53.000000 venv-management-2.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-08-08 13:13:06.188081 venv-management-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-08-08 13:12:53.000000 venv-management-2.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-08 13:12:53.000000 venv-management-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-08 13:13:06.188081 venv-management-2.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:06.180081 venv-management-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:06.184081 venv-management-2.0.3/src/venv_management/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-08 13:12:53.000000 venv-management-2.0.3/src/venv_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-08-08 13:12:53.000000 venv-management-2.0.3/src/venv_management/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-08-08 13:12:53.000000 venv-management-2.0.3/src/venv_management/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-08 13:12:53.000000 venv-management-2.0.3/src/venv_management/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:06.184081 venv-management-2.0.3/src/venv_management/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:12:53.000000 venv-management-2.0.3/src/venv_management/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:06.184081 venv-management-2.0.3/src/venv_management/ext/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:12:53.000000 venv-management-2.0.3/src/venv_management/ext/drivers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:06.184081 venv-management-2.0.3/src/venv_management/ext/drivers/pyenv_virtualenv/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 13:12:53.000000 venv-management-2.0.3/src/venv_management/ext/drivers/pyenv_virtualenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-08-08 13:12:53.000000 venv-management-2.0.3/src/venv_management/ext/drivers/pyenv_virtualenv/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:06.184081 venv-management-2.0.3/src/venv_management/ext/drivers/virtualenv_sh/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-08 13:12:53.000000 venv-management-2.0.3/src/venv_management/ext/drivers/virtualenv_sh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-08-08 13:12:53.000000 venv-management-2.0.3/src/venv_management/ext/drivers/virtualenv_sh/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:06.188081 venv-management-2.0.3/src/venv_management/ext/drivers/virtualenvwrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-08 13:12:53.000000 venv-management-2.0.3/src/venv_management/ext/drivers/virtualenvwrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-08-08 13:12:53.000000 venv-management-2.0.3/src/venv_management/ext/drivers/virtualenvwrapper/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-08-08 13:12:53.000000 venv-management-2.0.3/src/venv_management/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-08-08 13:12:53.000000 venv-management-2.0.3/src/venv_management/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-08 13:12:53.000000 venv-management-2.0.3/src/venv_management/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:06.184081 venv-management-2.0.3/src/venv_management.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-08-08 13:13:06.000000 venv-management-2.0.3/src/venv_management.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-08 13:13:06.000000 venv-management-2.0.3/src/venv_management.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:13:06.000000 venv-management-2.0.3/src/venv_management.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-08 13:13:06.000000 venv-management-2.0.3/src/venv_management.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-08 13:13:06.000000 venv-management-2.0.3/src/venv_management.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 13:13:06.000000 venv-management-2.0.3/src/venv_management.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:13:05.000000 venv-management-2.0.3/src/venv_management.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:06.188081 venv-management-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-08 13:12:53.000000 venv-management-2.0.3/tests/test_check_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-08 13:12:53.000000 venv-management-2.0.3/tests/test_discard_virtual_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-08 13:12:53.000000 venv-management-2.0.3/tests/test_ensure_virtual_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-08 13:12:53.000000 venv-management-2.0.3/tests/test_has_virtualenvwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-08 13:12:53.000000 venv-management-2.0.3/tests/test_list_virtual_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-08 13:12:53.000000 venv-management-2.0.3/tests/test_make_virtual_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-08 13:12:53.000000 venv-management-2.0.3/tests/test_remove_virtual_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-08 13:12:53.000000 venv-management-2.0.3/tests/test_resolve_virtual_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-08 13:12:53.000000 venv-management-2.0.3/tests/test_virtual_env_context_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:08.657602 venv-management-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-08 13:12:57.000000 venv-management-2.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-08-08 13:13:08.657602 venv-management-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-08-08 13:12:57.000000 venv-management-2.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-08 13:12:57.000000 venv-management-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-08 13:13:08.657602 venv-management-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:08.645602 venv-management-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:08.649602 venv-management-2.0.4/src/venv_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-08 13:12:57.000000 venv-management-2.0.4/src/venv_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-08-08 13:12:57.000000 venv-management-2.0.4/src/venv_management/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-08-08 13:12:57.000000 venv-management-2.0.4/src/venv_management/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-08 13:12:57.000000 venv-management-2.0.4/src/venv_management/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:08.653602 venv-management-2.0.4/src/venv_management/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:12:57.000000 venv-management-2.0.4/src/venv_management/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:08.653602 venv-management-2.0.4/src/venv_management/ext/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:12:57.000000 venv-management-2.0.4/src/venv_management/ext/drivers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:08.653602 venv-management-2.0.4/src/venv_management/ext/drivers/pyenv_virtualenv/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 13:12:57.000000 venv-management-2.0.4/src/venv_management/ext/drivers/pyenv_virtualenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-08-08 13:12:57.000000 venv-management-2.0.4/src/venv_management/ext/drivers/pyenv_virtualenv/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:08.653602 venv-management-2.0.4/src/venv_management/ext/drivers/virtualenv_sh/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-08 13:12:57.000000 venv-management-2.0.4/src/venv_management/ext/drivers/virtualenv_sh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-08-08 13:12:57.000000 venv-management-2.0.4/src/venv_management/ext/drivers/virtualenv_sh/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:08.657602 venv-management-2.0.4/src/venv_management/ext/drivers/virtualenvwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-08 13:12:57.000000 venv-management-2.0.4/src/venv_management/ext/drivers/virtualenvwrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-08-08 13:12:57.000000 venv-management-2.0.4/src/venv_management/ext/drivers/virtualenvwrapper/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-08-08 13:12:57.000000 venv-management-2.0.4/src/venv_management/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-08-08 13:12:57.000000 venv-management-2.0.4/src/venv_management/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-08 13:12:57.000000 venv-management-2.0.4/src/venv_management/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:08.653602 venv-management-2.0.4/src/venv_management.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-08-08 13:13:08.000000 venv-management-2.0.4/src/venv_management.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-08 13:13:08.000000 venv-management-2.0.4/src/venv_management.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:13:08.000000 venv-management-2.0.4/src/venv_management.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-08 13:13:08.000000 venv-management-2.0.4/src/venv_management.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-08 13:13:08.000000 venv-management-2.0.4/src/venv_management.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 13:13:08.000000 venv-management-2.0.4/src/venv_management.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:13:08.000000 venv-management-2.0.4/src/venv_management.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:08.657602 venv-management-2.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-08 13:12:57.000000 venv-management-2.0.4/tests/test_check_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-08 13:12:57.000000 venv-management-2.0.4/tests/test_discard_virtual_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-08 13:12:57.000000 venv-management-2.0.4/tests/test_ensure_virtual_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-08 13:12:57.000000 venv-management-2.0.4/tests/test_has_virtualenvwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-08 13:12:57.000000 venv-management-2.0.4/tests/test_list_virtual_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-08 13:12:57.000000 venv-management-2.0.4/tests/test_make_virtual_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-08 13:12:57.000000 venv-management-2.0.4/tests/test_remove_virtual_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-08 13:12:57.000000 venv-management-2.0.4/tests/test_resolve_virtual_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-08 13:12:57.000000 venv-management-2.0.4/tests/test_virtual_env_context_manager.py
```

### Comparing `venv-management-2.0.3/LICENSE.txt` & `venv-management-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.3/PKG-INFO` & `venv-management-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-management
-Version: 2.0.3
+Version: 2.0.4
 Summary: A Python package for programmatic creation of Python virtual environments
 Home-page: https://github.com/sixty-north/venv-management
 Author: Sixty North AS
 Author-email: systems+venv_management@sixty-north.com
 License: MIT License
 Keywords: virtual-environment
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `venv-management-2.0.3/README.rst` & `venv-management-2.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.3/setup.cfg` & `venv-management-2.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.3/src/venv_management/__init__.py` & `venv-management-2.0.4/src/venv_management/__init__.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.3/src/venv_management/api.py` & `venv-management-2.0.4/src/venv_management/api.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.3/src/venv_management/driver.py` & `venv-management-2.0.4/src/venv_management/driver.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.3/src/venv_management/ext/drivers/pyenv_virtualenv/driver.py` & `venv-management-2.0.4/src/venv_management/ext/drivers/pyenv_virtualenv/driver.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.3/src/venv_management/ext/drivers/virtualenv_sh/driver.py` & `venv-management-2.0.4/src/venv_management/ext/drivers/virtualenv_sh/driver.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.3/src/venv_management/ext/drivers/virtualenvwrapper/driver.py` & `venv-management-2.0.4/src/venv_management/ext/drivers/virtualenvwrapper/driver.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.3/src/venv_management/extension.py` & `venv-management-2.0.4/src/venv_management/extension.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.3/src/venv_management/utilities.py` & `venv-management-2.0.4/src/venv_management/utilities.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.3/src/venv_management.egg-info/PKG-INFO` & `venv-management-2.0.4/src/venv_management.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-management
-Version: 2.0.3
+Version: 2.0.4
 Summary: A Python package for programmatic creation of Python virtual environments
 Home-page: https://github.com/sixty-north/venv-management
 Author: Sixty North AS
 Author-email: systems+venv_management@sixty-north.com
 License: MIT License
 Keywords: virtual-environment
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `venv-management-2.0.3/src/venv_management.egg-info/SOURCES.txt` & `venv-management-2.0.4/src/venv_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.3/tests/test_discard_virtual_env.py` & `venv-management-2.0.4/tests/test_discard_virtual_env.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.3/tests/test_ensure_virtual_env.py` & `venv-management-2.0.4/tests/test_ensure_virtual_env.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.3/tests/test_make_virtual_env.py` & `venv-management-2.0.4/tests/test_make_virtual_env.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.3/tests/test_remove_virtual_env.py` & `venv-management-2.0.4/tests/test_remove_virtual_env.py`

 * *Files identical despite different names*

### Comparing `venv-management-2.0.3/tests/test_resolve_virtual_env.py` & `venv-management-2.0.4/tests/test_resolve_virtual_env.py`

 * *Files identical despite different names*

