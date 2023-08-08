# Comparing `tmp/zephyrcore-4.0.tar.gz` & `tmp/zephyrcore-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zephyrcore-4.0.tar", last modified: Tue Aug  8 18:41:07 2023, max compression
+gzip compressed data, was "zephyrcore-5.0.tar", last modified: Tue Aug  8 19:12:47 2023, max compression
```

## Comparing `zephyrcore-4.0.tar` & `zephyrcore-5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:41:07.900601 zephyrcore-4.0/
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     1241 2023-08-08 18:41:07.900601 zephyrcore-4.0/PKG-INFO
--rw-rw-r--   0 rayan     (1000) rayan     (1000)      985 2023-07-17 12:37:36.000000 zephyrcore-4.0/README.md
--rw-rw-r--   0 rayan     (1000) rayan     (1000)       38 2023-08-08 18:41:07.900601 zephyrcore-4.0/setup.cfg
--rw-rw-r--   0 rayan     (1000) rayan     (1000)      761 2023-08-08 18:40:41.000000 zephyrcore-4.0/setup.py
-drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:41:07.900601 zephyrcore-4.0/zephyrcore/
-drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:41:07.900601 zephyrcore-4.0/zephyrcore/src/
-drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:41:07.900601 zephyrcore-4.0/zephyrcore/src/zephyrcore/
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     1910 2023-07-31 17:35:09.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore/actions.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     5820 2023-08-08 12:42:10.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore/constants.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)    20585 2023-08-08 12:52:21.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore/create_test_cycles.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     6549 2023-08-08 12:42:10.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore/json_treatment.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     1496 2023-08-08 18:38:16.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore/logger.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     2047 2023-08-03 15:43:40.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore/update_test_case.py
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     3225 2023-08-08 12:42:10.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore/utils.py
-drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 18:41:07.900601 zephyrcore-4.0/zephyrcore/src/zephyrcore.egg-info/
--rw-rw-r--   0 rayan     (1000) rayan     (1000)     1241 2023-08-08 18:41:07.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore.egg-info/PKG-INFO
--rw-rw-r--   0 rayan     (1000) rayan     (1000)      547 2023-08-08 18:41:07.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore.egg-info/SOURCES.txt
--rw-rw-r--   0 rayan     (1000) rayan     (1000)        1 2023-08-08 18:41:07.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore.egg-info/dependency_links.txt
--rw-rw-r--   0 rayan     (1000) rayan     (1000)       30 2023-08-08 18:41:07.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore.egg-info/requires.txt
--rw-rw-r--   0 rayan     (1000) rayan     (1000)       11 2023-08-08 18:41:07.000000 zephyrcore-4.0/zephyrcore/src/zephyrcore.egg-info/top_level.txt
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 19:12:47.589311 zephyrcore-5.0/
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     1241 2023-08-08 19:12:47.589311 zephyrcore-5.0/PKG-INFO
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)      985 2023-07-17 12:37:36.000000 zephyrcore-5.0/README.md
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)       38 2023-08-08 19:12:47.589311 zephyrcore-5.0/setup.cfg
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)      761 2023-08-08 19:12:33.000000 zephyrcore-5.0/setup.py
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 19:12:47.589311 zephyrcore-5.0/zephyrcore/
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 19:12:47.589311 zephyrcore-5.0/zephyrcore/src/
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 19:12:47.589311 zephyrcore-5.0/zephyrcore/src/zephyrcore/
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     1910 2023-07-31 17:35:09.000000 zephyrcore-5.0/zephyrcore/src/zephyrcore/actions.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     5820 2023-08-08 12:42:10.000000 zephyrcore-5.0/zephyrcore/src/zephyrcore/constants.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)    21057 2023-08-08 19:12:24.000000 zephyrcore-5.0/zephyrcore/src/zephyrcore/create_test_cycles.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     6632 2023-08-08 19:12:24.000000 zephyrcore-5.0/zephyrcore/src/zephyrcore/json_treatment.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     1496 2023-08-08 18:38:16.000000 zephyrcore-5.0/zephyrcore/src/zephyrcore/logger.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     2047 2023-08-03 15:43:40.000000 zephyrcore-5.0/zephyrcore/src/zephyrcore/update_test_case.py
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     3225 2023-08-08 12:42:10.000000 zephyrcore-5.0/zephyrcore/src/zephyrcore/utils.py
+drwxrwxr-x   0 rayan     (1000) rayan     (1000)        0 2023-08-08 19:12:47.589311 zephyrcore-5.0/zephyrcore/src/zephyrcore.egg-info/
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)     1241 2023-08-08 19:12:47.000000 zephyrcore-5.0/zephyrcore/src/zephyrcore.egg-info/PKG-INFO
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)      547 2023-08-08 19:12:47.000000 zephyrcore-5.0/zephyrcore/src/zephyrcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)        1 2023-08-08 19:12:47.000000 zephyrcore-5.0/zephyrcore/src/zephyrcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)       30 2023-08-08 19:12:47.000000 zephyrcore-5.0/zephyrcore/src/zephyrcore.egg-info/requires.txt
+-rw-rw-r--   0 rayan     (1000) rayan     (1000)       11 2023-08-08 19:12:47.000000 zephyrcore-5.0/zephyrcore/src/zephyrcore.egg-info/top_level.txt
```

### Comparing `zephyrcore-4.0/PKG-INFO` & `zephyrcore-5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zephyrcore
-Version: 4.0
+Version: 5.0
 Summary: Python Distribution Utilities
 Home-page: https://www.python.org/sigs/distutils-sig/
 Author: QM Core Team
 Author-email: business.agility@ab-inbev.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `zephyrcore-4.0/README.md` & `zephyrcore-5.0/README.md`

 * *Files identical despite different names*

### Comparing `zephyrcore-4.0/setup.py` & `zephyrcore-5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 import setuptools
 
 setuptools.setup(name='zephyrcore',
-                 version='4.0',
+                 version='5.0',
                  description='Python Distribution Utilities',
                  author='QM Core Team',
                  author_email='business.agility@ab-inbev.com',
                  long_description=open('README.md').read(),
                  long_description_content_type='text/markdown',
                  url='https://www.python.org/sigs/distutils-sig/',
                  packages=setuptools.find_packages(),
```

### Comparing `zephyrcore-4.0/zephyrcore/src/zephyrcore/actions.py` & `zephyrcore-5.0/zephyrcore/src/zephyrcore/actions.py`

 * *Files identical despite different names*

### Comparing `zephyrcore-4.0/zephyrcore/src/zephyrcore/constants.py` & `zephyrcore-5.0/zephyrcore/src/zephyrcore/constants.py`

 * *Files identical despite different names*

### Comparing `zephyrcore-4.0/zephyrcore/src/zephyrcore/create_test_cycles.py` & `zephyrcore-5.0/zephyrcore/src/zephyrcore/create_test_cycles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from pathlib import PurePosixPath
 import requests
 import re
-from constants import (FOLDERS_URL, MAX_FOLDER_RESULTS, Environment, _QM_SUB_FOLDER_MAP,
-                       _QM_AUTOMATED_TEST_CYCLE_FOLDER_MAP, _JIRA_VERSION_URL, _JIRA_ACCOUNT_URL,
-                       _QM_TEST_CYCLE_TITLE_VERSION_PATTERN, _TEST_COMPONENT_CYCLE_NAME_PATTERN,
-                       _TEST_CYCLE_NAME_PATTERN, _TEST_CYCLE_URL_PATTERN, _TEST_CYCLE_URL, _QM_JIRA_VERSION_PATTERN,
-                       _BUG_KEY_PATTERN, _JIRA_ISSUE_URL, _PLATFORM_FIELD, _ENVIRONMENT_FIELD, _ZONES_FIELD,
-                       _ZONE_NAME_MAP, TEST_EXECUTION_ISSUE_URL, _QM_ENVIRONMENT_NAME_MAP,
-                       TEST_EXECUTION_URL)
-from actions import get_headers, get_current_date_test_cycle_name, parse_description, get_hyperlink, get_current_date
+from zephyrcore.src.zephyrcore.constants import (FOLDERS_URL, MAX_FOLDER_RESULTS, Environment, _QM_SUB_FOLDER_MAP,
+                                                 _QM_AUTOMATED_TEST_CYCLE_FOLDER_MAP, _JIRA_VERSION_URL,
+                                                 _JIRA_ACCOUNT_URL,
+                                                 _QM_TEST_CYCLE_TITLE_VERSION_PATTERN,
+                                                 _TEST_COMPONENT_CYCLE_NAME_PATTERN,
+                                                 _TEST_CYCLE_NAME_PATTERN, _TEST_CYCLE_URL_PATTERN, _TEST_CYCLE_URL,
+                                                 _QM_JIRA_VERSION_PATTERN,
+                                                 _BUG_KEY_PATTERN, _JIRA_ISSUE_URL, _PLATFORM_FIELD, _ENVIRONMENT_FIELD,
+                                                 _ZONES_FIELD,
+                                                 _ZONE_NAME_MAP, TEST_EXECUTION_ISSUE_URL, _QM_ENVIRONMENT_NAME_MAP,
+                                                 TEST_EXECUTION_URL)
+from zephyrcore.src.zephyrcore.actions import get_headers, get_current_date_test_cycle_name, parse_description, \
+    get_hyperlink, get_current_date
 import json
-from logger import logger
+from zephyrcore.src.zephyrcore.logger import logger
 from packaging.version import parse
-import utils
+from zephyrcore.src.zephyrcore import utils
 
 _MOBILE_PLATFORMS = ['android', 'ios']
 _JIRA_BASE_URL = 'https://ab-inbev.atlassian.net'
 
 # QM specific data
 _QM_PROJECT = 'BEESQM'
 
@@ -352,15 +357,15 @@
                 self._testcase = self._json_data[start]['testTag']
                 self._platform = self._json_data[start]['customFields']['platform']
                 self._test_tag = self._json_data[start]['testTag']
                 self._test_execution_status = self._json_data[start]['statusName']
 
                 # Test execution time treatment
                 hours, minutes, seconds = self._json_data[start]['executionTime'].split(':')
-                total_milliseconds = (float(hours)*3600 + float(minutes)*60 + float(seconds))*1000
+                total_milliseconds = (float(hours) * 3600 + float(minutes) * 60 + float(seconds)) * 1000
                 self._test_execution_duration = total_milliseconds
 
                 self._zone = self._json_data[start]['customFields']['zone']
                 self._component_test_case = self._json_data[start]['testComponent'] if \
                     self._json_data[start]['testComponentKey'] else None
                 self._test_cycle = self._test_cycles_dict[
                     self._component_test_case] if self._create_zephyr_cycle_per_component else \
@@ -392,8 +397,7 @@
                                                          data=json.dumps(test_execution_data)).json()
                 except Exception as e:
                     logger.error('Zephyr error -> Error to the create test cycle on zephyr!'
                                  f'Test Cycle: {self._test_cycle["key"]}\n'
                                  f'Test: {self._test_case}')
                     logger.debug(e)
                 self._add_issues_to_test_execution()
-
```

### Comparing `zephyrcore-4.0/zephyrcore/src/zephyrcore/json_treatment.py` & `zephyrcore-5.0/zephyrcore/src/zephyrcore/json_treatment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 import re
-from constants import TEST_CASE_URL, TEST_CASE_KEY_PATTERN
+from zephyrcore.src.zephyrcore.constants import TEST_CASE_URL, TEST_CASE_KEY_PATTERN
 import json
 import os
 from atlassian import Jira
-from logger import logger
-import utils
+from zephyrcore.src.zephyrcore.logger import logger
+from zephyrcore.src.zephyrcore import utils
 
 _MOBILE_PLATFORMS = ['android', 'ios']
 _JIRA_BASE_URL = 'https://ab-inbev.atlassian.net'
 
 # QM specific data
 _QM_PROJECT = 'BEESQM'
```

### Comparing `zephyrcore-4.0/zephyrcore/src/zephyrcore/logger.py` & `zephyrcore-5.0/zephyrcore/src/zephyrcore/logger.py`

 * *Files identical despite different names*

### Comparing `zephyrcore-4.0/zephyrcore/src/zephyrcore/update_test_case.py` & `zephyrcore-5.0/zephyrcore/src/zephyrcore/update_test_case.py`

 * *Files identical despite different names*

### Comparing `zephyrcore-4.0/zephyrcore/src/zephyrcore/utils.py` & `zephyrcore-5.0/zephyrcore/src/zephyrcore/utils.py`

 * *Files identical despite different names*

### Comparing `zephyrcore-4.0/zephyrcore/src/zephyrcore.egg-info/PKG-INFO` & `zephyrcore-5.0/zephyrcore/src/zephyrcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zephyrcore
-Version: 4.0
+Version: 5.0
 Summary: Python Distribution Utilities
 Home-page: https://www.python.org/sigs/distutils-sig/
 Author: QM Core Team
 Author-email: business.agility@ab-inbev.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `zephyrcore-4.0/zephyrcore/src/zephyrcore.egg-info/SOURCES.txt` & `zephyrcore-5.0/zephyrcore/src/zephyrcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

