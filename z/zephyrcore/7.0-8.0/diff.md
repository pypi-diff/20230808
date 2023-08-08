# Comparing `tmp/zephyrcore-7.0.tar.gz` & `tmp/zephyrcore-8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zephyrcore-7.0.tar", last modified: Tue Aug  8 19:20:21 2023, max compression
+gzip compressed data, was "zephyrcore-8.0.tar", last modified: Tue Aug  8 19:37:08 2023, max compression
```

## Comparing `zephyrcore-7.0.tar` & `zephyrcore-8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 19:20:21.534904 zephyrcore-7.0/
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     1241 2023-08-08 19:20:21.534904 zephyrcore-7.0/PKG-INFO
--rw-rw-r--   0 rayan     (1000) rayan     (1000)      985 2023-07-17 12:37:36.000000 zephyrcore-7.0/README.md
--rw-rw-r--   0 rayan     (1000) rayan     (1000)       38 2023-08-08 19:20:21.534904 zephyrcore-7.0/setup.cfg
--rw-rw-r--   0 rayan     (1000) rayan     (1000)      761 2023-08-08 19:20:19.000000 zephyrcore-7.0/setup.py
-drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 19:20:21.534904 zephyrcore-7.0/zephyrcore/
-drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 19:20:21.534904 zephyrcore-7.0/zephyrcore/src/
-drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 19:20:21.534904 zephyrcore-7.0/zephyrcore/src/zephyrcore/
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     1910 2023-07-31 17:35:09.000000 zephyrcore-7.0/zephyrcore/src/zephyrcore/actions.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     5820 2023-08-08 12:42:10.000000 zephyrcore-7.0/zephyrcore/src/zephyrcore/constants.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)    20997 2023-08-08 19:18:28.000000 zephyrcore-7.0/zephyrcore/src/zephyrcore/create_test_cycles.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     6587 2023-08-08 19:20:05.000000 zephyrcore-7.0/zephyrcore/src/zephyrcore/json_treatment.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     1496 2023-08-08 18:38:16.000000 zephyrcore-7.0/zephyrcore/src/zephyrcore/logger.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     2047 2023-08-03 15:43:40.000000 zephyrcore-7.0/zephyrcore/src/zephyrcore/update_test_case.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     3225 2023-08-08 12:42:10.000000 zephyrcore-7.0/zephyrcore/src/zephyrcore/utils.py
-drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 19:20:21.534904 zephyrcore-7.0/zephyrcore/src/zephyrcore.egg-info/
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     1241 2023-08-08 19:20:21.000000 zephyrcore-7.0/zephyrcore/src/zephyrcore.egg-info/PKG-INFO
--rw-rw-r--   0 rayan     (1000) rayan     (1000)      547 2023-08-08 19:20:21.000000 zephyrcore-7.0/zephyrcore/src/zephyrcore.egg-info/SOURCES.txt
--rw-rw-r--   0 rayan     (1000) rayan     (1000)        1 2023-08-08 19:20:21.000000 zephyrcore-7.0/zephyrcore/src/zephyrcore.egg-info/dependency_links.txt
--rw-rw-r--   0 rayan     (1000) rayan     (1000)       30 2023-08-08 19:20:21.000000 zephyrcore-7.0/zephyrcore/src/zephyrcore.egg-info/requires.txt
--rw-rw-r--   0 rayan     (1000) rayan     (1000)       11 2023-08-08 19:20:21.000000 zephyrcore-7.0/zephyrcore/src/zephyrcore.egg-info/top_level.txt
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 19:37:08.099013 zephyrcore-8.0/
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     1241 2023-08-08 19:37:08.099013 zephyrcore-8.0/PKG-INFO
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)      985 2023-07-17 12:37:36.000000 zephyrcore-8.0/README.md
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)       38 2023-08-08 19:37:08.099013 zephyrcore-8.0/setup.cfg
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)      761 2023-08-08 19:37:05.000000 zephyrcore-8.0/setup.py
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 19:37:08.095013 zephyrcore-8.0/zephyrcore/
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 19:37:08.095013 zephyrcore-8.0/zephyrcore/src/
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 19:37:08.095013 zephyrcore-8.0/zephyrcore/src/zephyrcore/
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     1910 2023-07-31 17:35:09.000000 zephyrcore-8.0/zephyrcore/src/zephyrcore/actions.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     5820 2023-08-08 12:42:10.000000 zephyrcore-8.0/zephyrcore/src/zephyrcore/constants.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)    20875 2023-08-08 19:37:05.000000 zephyrcore-8.0/zephyrcore/src/zephyrcore/create_test_cycles.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     6593 2023-08-08 19:37:05.000000 zephyrcore-8.0/zephyrcore/src/zephyrcore/json_treatment.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     1496 2023-08-08 18:38:16.000000 zephyrcore-8.0/zephyrcore/src/zephyrcore/logger.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     2047 2023-08-03 15:43:40.000000 zephyrcore-8.0/zephyrcore/src/zephyrcore/update_test_case.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     3225 2023-08-08 12:42:10.000000 zephyrcore-8.0/zephyrcore/src/zephyrcore/utils.py
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 19:37:08.099013 zephyrcore-8.0/zephyrcore/src/zephyrcore.egg-info/
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     1241 2023-08-08 19:37:08.000000 zephyrcore-8.0/zephyrcore/src/zephyrcore.egg-info/PKG-INFO
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)      547 2023-08-08 19:37:08.000000 zephyrcore-8.0/zephyrcore/src/zephyrcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)        1 2023-08-08 19:37:08.000000 zephyrcore-8.0/zephyrcore/src/zephyrcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)       30 2023-08-08 19:37:08.000000 zephyrcore-8.0/zephyrcore/src/zephyrcore.egg-info/requires.txt
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)       11 2023-08-08 19:37:08.000000 zephyrcore-8.0/zephyrcore/src/zephyrcore.egg-info/top_level.txt
```

### Comparing `zephyrcore-7.0/PKG-INFO` & `zephyrcore-8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zephyrcore
-Version: 7.0
+Version: 8.0
 Summary: Python Distribution Utilities
 Home-page: https://www.python.org/sigs/distutils-sig/
 Author: QM Core Team
 Author-email: business.agility@ab-inbev.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `zephyrcore-7.0/README.md` & `zephyrcore-8.0/README.md`

 * *Files identical despite different names*

### Comparing `zephyrcore-7.0/setup.py` & `zephyrcore-8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 import setuptools
 
 setuptools.setup(name='zephyrcore',
-                 version='7.0',
+                 version='8.0',
                  description='Python Distribution Utilities',
                  author='QM Core Team',
                  author_email='business.agility@ab-inbev.com',
                  long_description=open('README.md').read(),
                  long_description_content_type='text/markdown',
                  url='https://www.python.org/sigs/distutils-sig/',
                  packages=setuptools.find_packages(),
```

### Comparing `zephyrcore-7.0/zephyrcore/src/zephyrcore/actions.py` & `zephyrcore-8.0/zephyrcore/src/zephyrcore/actions.py`

 * *Files identical despite different names*

### Comparing `zephyrcore-7.0/zephyrcore/src/zephyrcore/constants.py` & `zephyrcore-8.0/zephyrcore/src/zephyrcore/constants.py`

 * *Files identical despite different names*

### Comparing `zephyrcore-7.0/zephyrcore/src/zephyrcore/create_test_cycles.py` & `zephyrcore-8.0/zephyrcore/src/zephyrcore/create_test_cycles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from pathlib import PurePosixPath
 import requests
 import re
-from zephyrcore.constants import (FOLDERS_URL, MAX_FOLDER_RESULTS, Environment, _QM_SUB_FOLDER_MAP,
-                                                 _QM_AUTOMATED_TEST_CYCLE_FOLDER_MAP, _JIRA_VERSION_URL,
-                                                 _JIRA_ACCOUNT_URL,
-                                                 _QM_TEST_CYCLE_TITLE_VERSION_PATTERN,
-                                                 _TEST_COMPONENT_CYCLE_NAME_PATTERN,
-                                                 _TEST_CYCLE_NAME_PATTERN, _TEST_CYCLE_URL_PATTERN, _TEST_CYCLE_URL,
-                                                 _QM_JIRA_VERSION_PATTERN,
-                                                 _BUG_KEY_PATTERN, _JIRA_ISSUE_URL, _PLATFORM_FIELD, _ENVIRONMENT_FIELD,
-                                                 _ZONES_FIELD,
-                                                 _ZONE_NAME_MAP, TEST_EXECUTION_ISSUE_URL, _QM_ENVIRONMENT_NAME_MAP,
-                                                 TEST_EXECUTION_URL)
-from zephyrcore.actions import get_headers, get_current_date_test_cycle_name, parse_description, \
+from ..zephyrcore.constants import (FOLDERS_URL, MAX_FOLDER_RESULTS, Environment, _QM_SUB_FOLDER_MAP,
+                                    _QM_AUTOMATED_TEST_CYCLE_FOLDER_MAP, _JIRA_VERSION_URL,
+                                    _JIRA_ACCOUNT_URL,
+                                    _QM_TEST_CYCLE_TITLE_VERSION_PATTERN,
+                                    _TEST_COMPONENT_CYCLE_NAME_PATTERN,
+                                    _TEST_CYCLE_NAME_PATTERN, _TEST_CYCLE_URL_PATTERN, _TEST_CYCLE_URL,
+                                    _QM_JIRA_VERSION_PATTERN,
+                                    _BUG_KEY_PATTERN, _JIRA_ISSUE_URL, _PLATFORM_FIELD, _ENVIRONMENT_FIELD,
+                                    _ZONES_FIELD,
+                                    _ZONE_NAME_MAP, TEST_EXECUTION_ISSUE_URL, _QM_ENVIRONMENT_NAME_MAP,
+                                    TEST_EXECUTION_URL)
+from ..zephyrcore.actions import get_headers, get_current_date_test_cycle_name, parse_description, \
     get_hyperlink, get_current_date
 import json
-from zephyrcore.logger import logger
+from ..zephyrcore.logger import logger
 from packaging.version import parse
-from zephyrcore import utils
+from ..zephyrcore import utils
 
 _MOBILE_PLATFORMS = ['android', 'ios']
 _JIRA_BASE_URL = 'https://ab-inbev.atlassian.net'
 
 # QM specific data
 _QM_PROJECT = 'BEESQM'
```

### Comparing `zephyrcore-7.0/zephyrcore/src/zephyrcore/json_treatment.py` & `zephyrcore-8.0/zephyrcore/src/zephyrcore/json_treatment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 import re
-from zephyrcore.constants import TEST_CASE_URL, TEST_CASE_KEY_PATTERN
+from ..zephyrcore.constants import TEST_CASE_URL, TEST_CASE_KEY_PATTERN
 import json
 import os
 from atlassian import Jira
-from zephyrcore.logger import logger
-from zephyrcore import utils
+from ..zephyrcore.logger import logger
+from ..zephyrcore import utils
 
 _MOBILE_PLATFORMS = ['android', 'ios']
 _JIRA_BASE_URL = 'https://ab-inbev.atlassian.net'
 
 # QM specific data
 _QM_PROJECT = 'BEESQM'
```

### Comparing `zephyrcore-7.0/zephyrcore/src/zephyrcore/logger.py` & `zephyrcore-8.0/zephyrcore/src/zephyrcore/logger.py`

 * *Files identical despite different names*

### Comparing `zephyrcore-7.0/zephyrcore/src/zephyrcore/update_test_case.py` & `zephyrcore-8.0/zephyrcore/src/zephyrcore/update_test_case.py`

 * *Files identical despite different names*

### Comparing `zephyrcore-7.0/zephyrcore/src/zephyrcore/utils.py` & `zephyrcore-8.0/zephyrcore/src/zephyrcore/utils.py`

 * *Files identical despite different names*

### Comparing `zephyrcore-7.0/zephyrcore/src/zephyrcore.egg-info/PKG-INFO` & `zephyrcore-8.0/zephyrcore/src/zephyrcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zephyrcore
-Version: 7.0
+Version: 8.0
 Summary: Python Distribution Utilities
 Home-page: https://www.python.org/sigs/distutils-sig/
 Author: QM Core Team
 Author-email: business.agility@ab-inbev.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `zephyrcore-7.0/zephyrcore/src/zephyrcore.egg-info/SOURCES.txt` & `zephyrcore-8.0/zephyrcore/src/zephyrcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

