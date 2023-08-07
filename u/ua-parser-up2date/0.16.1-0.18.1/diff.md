# Comparing `tmp/ua-parser-up2date-0.16.1.tar.gz` & `tmp/ua-parser-up2date-0.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ua-parser-up2date-0.16.1.tar", last modified: Sat Dec 17 03:05:50 2022, max compression
+gzip compressed data, was "ua-parser-up2date-0.18.1.tar", last modified: Mon Aug  7 22:48:03 2023, max compression
```

## Comparing `ua-parser-up2date-0.16.1.tar` & `ua-parser-up2date-0.18.1.tar`

### file list

```diff
@@ -1,19 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-17 03:05:50.678843 ua-parser-up2date-0.16.1/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-17 03:05:39.000000 ua-parser-up2date-0.16.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2022-12-17 03:05:50.678843 ua-parser-up2date-0.16.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2022-12-17 03:05:39.000000 ua-parser-up2date-0.16.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2022-12-17 03:05:39.000000 ua-parser-up2date-0.16.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-17 03:05:50.678843 ua-parser-up2date-0.16.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2022-12-17 03:05:39.000000 ua-parser-up2date-0.16.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-17 03:05:50.678843 ua-parser-up2date-0.16.1/ua_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2022-12-17 03:05:39.000000 ua-parser-up2date-0.16.1/ua_parser/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-17 03:05:39.000000 ua-parser-up2date-0.16.1/ua_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   163945 2022-12-17 03:05:50.000000 ua-parser-up2date-0.16.1/ua_parser/_regexes.py
--rw-r--r--   0 runner    (1001) docker     (123)    19619 2022-12-17 03:05:39.000000 ua-parser-up2date-0.16.1/ua_parser/user_agent_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2022-12-17 03:05:39.000000 ua-parser-up2date-0.16.1/ua_parser/user_agent_parser_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-17 03:05:50.678843 ua-parser-up2date-0.16.1/ua_parser_up2date.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2022-12-17 03:05:48.000000 ua-parser-up2date-0.16.1/ua_parser_up2date.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2022-12-17 03:05:48.000000 ua-parser-up2date-0.16.1/ua_parser_up2date.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-17 03:05:48.000000 ua-parser-up2date-0.16.1/ua_parser_up2date.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-17 03:05:48.000000 ua-parser-up2date-0.16.1/ua_parser_up2date.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-17 03:05:48.000000 ua-parser-up2date-0.16.1/ua_parser_up2date.egg-info/top_level.txt
+drwxr-xr-x   0 robd       (501) staff       (20)        0 2023-08-07 22:48:03.615710 ua-parser-up2date-0.18.1/
+-rw-r--r--   0 robd       (501) staff       (20)    11358 2023-08-07 22:37:18.000000 ua-parser-up2date-0.18.1/LICENSE
+-rw-r--r--   0 robd       (501) staff       (20)      146 2023-08-07 22:37:18.000000 ua-parser-up2date-0.18.1/MANIFEST.in
+-rw-r--r--   0 robd       (501) staff       (20)     5401 2023-08-07 22:48:03.615826 ua-parser-up2date-0.18.1/PKG-INFO
+-rw-r--r--   0 robd       (501) staff       (20)     4123 2023-08-07 22:37:18.000000 ua-parser-up2date-0.18.1/README.rst
+-rw-r--r--   0 robd       (501) staff       (20)     1566 2023-08-07 22:48:00.000000 ua-parser-up2date-0.18.1/pyproject.toml
+-rw-r--r--   0 robd       (501) staff       (20)      148 2023-08-07 22:48:03.616152 ua-parser-up2date-0.18.1/setup.cfg
+-rw-r--r--   0 robd       (501) staff       (20)     4751 2023-08-07 22:38:05.000000 ua-parser-up2date-0.18.1/setup.py
+drwxr-xr-x   0 robd       (501) staff       (20)        0 2023-08-07 22:48:03.595932 ua-parser-up2date-0.18.1/src/
+drwxr-xr-x   0 robd       (501) staff       (20)        0 2023-08-07 22:48:03.597385 ua-parser-up2date-0.18.1/src/ua_parser/
+-rw-r--r--   0 robd       (501) staff       (20)       21 2023-08-07 22:37:18.000000 ua-parser-up2date-0.18.1/src/ua_parser/__init__.py
+-rw-r--r--   0 robd       (501) staff       (20)    15513 2023-08-07 22:37:18.000000 ua-parser-up2date-0.18.1/src/ua_parser/user_agent_parser.py
+drwxr-xr-x   0 robd       (501) staff       (20)        0 2023-08-07 22:48:03.597924 ua-parser-up2date-0.18.1/src/ua_parser_up2date.egg-info/
+-rw-r--r--   0 robd       (501) staff       (20)     5401 2023-08-07 22:48:03.000000 ua-parser-up2date-0.18.1/src/ua_parser_up2date.egg-info/PKG-INFO
+-rw-r--r--   0 robd       (501) staff       (20)     1106 2023-08-07 22:48:03.000000 ua-parser-up2date-0.18.1/src/ua_parser_up2date.egg-info/SOURCES.txt
+-rw-r--r--   0 robd       (501) staff       (20)        1 2023-08-07 22:48:03.000000 ua-parser-up2date-0.18.1/src/ua_parser_up2date.egg-info/dependency_links.txt
+-rw-r--r--   0 robd       (501) staff       (20)       15 2023-08-07 22:48:03.000000 ua-parser-up2date-0.18.1/src/ua_parser_up2date.egg-info/requires.txt
+-rw-r--r--   0 robd       (501) staff       (20)       10 2023-08-07 22:48:03.000000 ua-parser-up2date-0.18.1/src/ua_parser_up2date.egg-info/top_level.txt
+drwxr-xr-x   0 robd       (501) staff       (20)        0 2023-08-07 22:48:03.598031 ua-parser-up2date-0.18.1/tests/
+-rw-r--r--   0 robd       (501) staff       (20)     8761 2023-08-07 22:37:18.000000 ua-parser-up2date-0.18.1/tests/test_legacy.py
+drwxr-xr-x   0 robd       (501) staff       (20)        0 2023-08-07 22:48:03.598930 ua-parser-up2date-0.18.1/uap-core/
+drwxr-xr-x   0 robd       (501) staff       (20)        0 2023-08-07 22:48:03.596160 ua-parser-up2date-0.18.1/uap-core/.github/
+drwxr-xr-x   0 robd       (501) staff       (20)        0 2023-08-07 22:48:03.599490 ua-parser-up2date-0.18.1/uap-core/.github/workflows/
+-rw-r--r--   0 robd       (501) staff       (20)      800 2023-08-07 22:40:19.000000 ua-parser-up2date-0.18.1/uap-core/.github/workflows/ci.yml
+-rw-r--r--   0 robd       (501) staff       (20)     1094 2023-08-07 22:36:30.000000 ua-parser-up2date-0.18.1/uap-core/CONTRIBUTING.md
+-rw-r--r--   0 robd       (501) staff       (20)      608 2023-08-07 22:36:30.000000 ua-parser-up2date-0.18.1/uap-core/LICENSE
+-rw-r--r--   0 robd       (501) staff       (20)     2585 2023-08-07 22:36:30.000000 ua-parser-up2date-0.18.1/uap-core/README.md
+drwxr-xr-x   0 robd       (501) staff       (20)        0 2023-08-07 22:48:03.599648 ua-parser-up2date-0.18.1/uap-core/docs/
+-rw-r--r--   0 robd       (501) staff       (20)     9862 2023-08-07 22:36:30.000000 ua-parser-up2date-0.18.1/uap-core/docs/specification.md
+-rw-r--r--   0 robd       (501) staff       (20)      965 2023-08-07 22:40:19.000000 ua-parser-up2date-0.18.1/uap-core/package.json
+-rw-r--r--   0 robd       (501) staff       (20)   205558 2023-08-07 22:40:19.000000 ua-parser-up2date-0.18.1/uap-core/regexes.yaml
+drwxr-xr-x   0 robd       (501) staff       (20)        0 2023-08-07 22:48:03.607404 ua-parser-up2date-0.18.1/uap-core/test_resources/
+-rw-r--r--   0 robd       (501) staff       (20)     5235 2023-08-07 22:36:30.000000 ua-parser-up2date-0.18.1/uap-core/test_resources/additional_os_tests.yaml
+-rwxr-xr-x   0 robd       (501) staff       (20)    27693 2023-08-07 22:36:30.000000 ua-parser-up2date-0.18.1/uap-core/test_resources/firefox_user_agent_strings.txt
+-rw-r--r--   0 robd       (501) staff       (20)    46613 2023-08-07 22:40:19.000000 ua-parser-up2date-0.18.1/uap-core/test_resources/firefox_user_agent_strings.yaml
+-rw-r--r--   0 robd       (501) staff       (20)    38168 2023-08-07 22:36:30.000000 ua-parser-up2date-0.18.1/uap-core/test_resources/opera_mini_user_agent_strings.yaml
+-rwxr-xr-x   0 robd       (501) staff       (20)  2057377 2023-08-07 22:36:30.000000 ua-parser-up2date-0.18.1/uap-core/test_resources/pgts_browser_list-orig.yaml
+-rwxr-xr-x   0 robd       (501) staff       (20)  1111221 2023-08-07 22:36:30.000000 ua-parser-up2date-0.18.1/uap-core/test_resources/pgts_browser_list.txt
+-rwxr-xr-x   0 robd       (501) staff       (20)  2027004 2023-08-07 22:36:30.000000 ua-parser-up2date-0.18.1/uap-core/test_resources/pgts_browser_list.yaml
+-rwxr-xr-x   0 robd       (501) staff       (20)    20017 2023-08-07 22:36:30.000000 ua-parser-up2date-0.18.1/uap-core/test_resources/podcasting_user_agent_strings.yaml
+-rwxr-xr-x   0 robd       (501) staff       (20)     1372 2023-08-07 22:36:30.000000 ua-parser-up2date-0.18.1/uap-core/test_resources/transform-pgts_browser_list.pl
+drwxr-xr-x   0 robd       (501) staff       (20)        0 2023-08-07 22:48:03.614901 ua-parser-up2date-0.18.1/uap-core/tests/
+-rw-r--r--   0 robd       (501) staff       (20)  3294090 2023-08-07 22:40:19.000000 ua-parser-up2date-0.18.1/uap-core/tests/test_device.yaml
+-rw-r--r--   0 robd       (501) staff       (20)    87251 2023-08-07 22:40:19.000000 ua-parser-up2date-0.18.1/uap-core/tests/test_os.yaml
+-rw-r--r--   0 robd       (501) staff       (20)   244650 2023-08-07 22:40:19.000000 ua-parser-up2date-0.18.1/uap-core/tests/test_ua.yaml
```

### Comparing `ua-parser-up2date-0.16.1/PKG-INFO` & `ua-parser-up2date-0.18.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ua-parser-up2date
-Version: 0.16.1
-Summary: Python port of Browserscope's user agent parser that is kept up to date!
-Home-page: https://github.com/robd003/uap-python
-Author: PBS
-Author-email: no-reply@pbs.org
+Version: 0.18.1
+Summary: Python port of Browserscope's user agent parser
+Author-email: Stephen Lamm <slamm@google.com>, PBS <no-reply@pbs.org>, Selwin Ong <selwin.ong@gmail.com>, Matt Robenolt <matt@ydekproductions.com>, Lindsey Simon <lsimon@commoner.com>
+Maintainer-email: masklinn <uap@masklinn.net>
 License: Apache 2.0
-Classifier: Development Status :: 5 - Production/Stable
+Project-URL: repository, https://github.com/robd003/uap-python-up2date
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -18,14 +18,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+Provides-Extra: yaml
+License-File: LICENSE
 
 uap-python
 ==========
 
 An **up to date** python implementation of the UA Parser (https://github.com/ua-parser,
 formerly https://github.com/tobie/ua-parser)
 
@@ -138,12 +140,7 @@
     >>> from ua_parser import user_agent_parser
     >>> import pprint
     >>> pp = pprint.PrettyPrinter(indent=4)
     >>> ua_string = 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2272.104 Safari/537.36'
     >>> parsed_string = user_agent_parser.ParseDevice(ua_string)
     >>> pp.pprint(parsed_string)
     {'brand': 'Apple', 'family': 'Mac', 'model': 'Mac'}
-
-Copyright
----------
-
-Copyright 2008 Google Inc. See ua\_parser/LICENSE for more information
```

### Comparing `ua-parser-up2date-0.16.1/README.rst` & `ua-parser-up2date-0.18.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -113,12 +113,7 @@
     >>> from ua_parser import user_agent_parser
     >>> import pprint
     >>> pp = pprint.PrettyPrinter(indent=4)
     >>> ua_string = 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2272.104 Safari/537.36'
     >>> parsed_string = user_agent_parser.ParseDevice(ua_string)
     >>> pp.pprint(parsed_string)
     {'brand': 'Apple', 'family': 'Mac', 'model': 'Mac'}
-
-Copyright
----------
-
-Copyright 2008 Google Inc. See ua\_parser/LICENSE for more information
```

### Comparing `ua-parser-up2date-0.16.1/ua_parser/LICENSE` & `ua-parser-up2date-0.18.1/uap-core/LICENSE`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-Copyright 2008 Google Inc.
+Apache License, Version 2.0
+===========================
 
-Licensed under the Apache License, Version 2.0 (the 'License')
+Copyright 2009 Google Inc.
+
+Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an 'AS IS' BASIS,
+distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
```

### Comparing `ua-parser-up2date-0.16.1/ua_parser/user_agent_parser.py` & `ua-parser-up2date-0.18.1/src/ua_parser/user_agent_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,56 @@
-# Copyright 2009 Google Inc.
-#
-# Licensed under the Apache License, Version 2.0 (the 'License')
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#         http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an 'AS IS' BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-"""Python implementation of the UA parser."""
-
-from __future__ import absolute_import
-
 import os
 import re
-import sys
 import warnings
-
-__author__ = "Lindsey Simon <elsigh@gmail.com>"
+from typing import *
 
 
 class UserAgentParser(object):
     def __init__(
         self, pattern, family_replacement=None, v1_replacement=None, v2_replacement=None
     ):
         """Initialize UserAgentParser.
 
         Args:
           pattern: a regular expression string
           family_replacement: a string to override the matched family (optional)
           v1_replacement: a string to override the matched v1 (optional)
           v2_replacement: a string to override the matched v2 (optional)
         """
-        self.pattern = pattern
-        self.user_agent_re = re.compile(self.pattern)
+        self.user_agent_re = re.compile(pattern)
         self.family_replacement = family_replacement
         self.v1_replacement = v1_replacement
         self.v2_replacement = v2_replacement
 
-    def MatchSpans(self, user_agent_string):
-        match_spans = []
-        match = self.user_agent_re.search(user_agent_string)
-        if match:
-            match_spans = [
-                match.span(group_index) for group_index in range(1, match.lastindex + 1)
-            ]
-        return match_spans
-
-    def Parse(self, user_agent_string):
+    def Parse(
+        self, user_agent_string: str
+    ) -> Tuple[Optional[str], Optional[str], Optional[str], Optional[str],]:
         family, v1, v2, v3 = None, None, None, None
         match = self.user_agent_re.search(user_agent_string)
         if match:
             if self.family_replacement:
                 if re.search(r"\$1", self.family_replacement):
-                    family = re.sub(r"\$1", match.group(1), self.family_replacement)
+                    family = re.sub(r"\$1", match[1], self.family_replacement)
                 else:
                     family = self.family_replacement
             else:
-                family = match.group(1)
+                family = match[1]
 
             if self.v1_replacement:
                 v1 = self.v1_replacement
             elif match.lastindex and match.lastindex >= 2:
-                v1 = match.group(2) or None
+                v1 = match[2] or None
 
             if self.v2_replacement:
                 v2 = self.v2_replacement
             elif match.lastindex and match.lastindex >= 3:
-                v2 = match.group(3) or None
+                v2 = match[3] or None
 
             if match.lastindex and match.lastindex >= 4:
-                v3 = match.group(4) or None
+                v3 = match[4] or None
 
         return family, v1, v2, v3
 
 
 class OSParser(object):
     def __init__(
         self,
@@ -95,76 +67,71 @@
           pattern: a regular expression string
           os_replacement: a string to override the matched os (optional)
           os_v1_replacement: a string to override the matched v1 (optional)
           os_v2_replacement: a string to override the matched v2 (optional)
           os_v3_replacement: a string to override the matched v3 (optional)
           os_v4_replacement: a string to override the matched v4 (optional)
         """
-        self.pattern = pattern
-        self.user_agent_re = re.compile(self.pattern)
+        self.user_agent_re = re.compile(pattern)
         self.os_replacement = os_replacement
         self.os_v1_replacement = os_v1_replacement
         self.os_v2_replacement = os_v2_replacement
         self.os_v3_replacement = os_v3_replacement
         self.os_v4_replacement = os_v4_replacement
 
-    def MatchSpans(self, user_agent_string):
-        match_spans = []
-        match = self.user_agent_re.search(user_agent_string)
-        if match:
-            match_spans = [
-                match.span(group_index) for group_index in range(1, match.lastindex + 1)
-            ]
-        return match_spans
-
-    def Parse(self, user_agent_string):
+    def Parse(
+        self, user_agent_string: str
+    ) -> Tuple[
+        Optional[str],
+        Optional[str],
+        Optional[str],
+        Optional[str],
+        Optional[str],
+    ]:
         os, os_v1, os_v2, os_v3, os_v4 = None, None, None, None, None
         match = self.user_agent_re.search(user_agent_string)
         if match:
             if self.os_replacement:
                 os = MultiReplace(self.os_replacement, match)
             elif match.lastindex:
-                os = match.group(1)
+                os = match[1]
 
             if self.os_v1_replacement:
                 os_v1 = MultiReplace(self.os_v1_replacement, match)
             elif match.lastindex and match.lastindex >= 2:
-                os_v1 = match.group(2)
+                os_v1 = match[2]
 
             if self.os_v2_replacement:
                 os_v2 = MultiReplace(self.os_v2_replacement, match)
             elif match.lastindex and match.lastindex >= 3:
-                os_v2 = match.group(3)
+                os_v2 = match[3]
 
             if self.os_v3_replacement:
                 os_v3 = MultiReplace(self.os_v3_replacement, match)
             elif match.lastindex and match.lastindex >= 4:
-                os_v3 = match.group(4)
+                os_v3 = match[4]
 
             if self.os_v4_replacement:
                 os_v4 = MultiReplace(self.os_v4_replacement, match)
             elif match.lastindex and match.lastindex >= 5:
-                os_v4 = match.group(5)
+                os_v4 = match[5]
 
         return os, os_v1, os_v2, os_v3, os_v4
 
 
 def MultiReplace(string, match):
     def _repl(m):
-        index = int(m.group(1)) - 1
+        index = int(m[1]) - 1
         group = match.groups()
         if index < len(group):
             return group[index]
         return ""
 
-    _string = re.sub(r"\$(\d)", _repl, string)
-    _string = re.sub(r"^\s+|\s+$", "", _string)
-    if _string == "":
-        return None
-    return _string
+    _string = re.sub(r"\$(\d)", _repl, string).strip()
+    return _string or None
 
 
 class DeviceParser(object):
     def __init__(
         self,
         pattern,
         regex_flag=None,
@@ -174,210 +141,179 @@
     ):
         """Initialize UserAgentParser.
 
         Args:
           pattern: a regular expression string
           device_replacement: a string to override the matched device (optional)
         """
-        self.pattern = pattern
-        if regex_flag == "i":
-            self.user_agent_re = re.compile(self.pattern, re.IGNORECASE)
-        else:
-            self.user_agent_re = re.compile(self.pattern)
+        self.user_agent_re = re.compile(
+            pattern, re.IGNORECASE if regex_flag == "i" else 0
+        )
         self.device_replacement = device_replacement
         self.brand_replacement = brand_replacement
         self.model_replacement = model_replacement
 
-    def MatchSpans(self, user_agent_string):
-        match_spans = []
-        match = self.user_agent_re.search(user_agent_string)
-        if match:
-            match_spans = [
-                match.span(group_index) for group_index in range(1, match.lastindex + 1)
-            ]
-        return match_spans
-
-    def Parse(self, user_agent_string):
+    def Parse(
+        self, user_agent_string: str
+    ) -> Tuple[Optional[str], Optional[str], Optional[str],]:
         device, brand, model = None, None, None
         match = self.user_agent_re.search(user_agent_string)
         if match:
             if self.device_replacement:
                 device = MultiReplace(self.device_replacement, match)
             else:
-                device = match.group(1)
+                device = match[1]
 
             if self.brand_replacement:
                 brand = MultiReplace(self.brand_replacement, match)
 
             if self.model_replacement:
                 model = MultiReplace(self.model_replacement, match)
             elif len(match.groups()) > 0:
-                model = match.group(1)
+                model = match[1]
 
         return device, brand, model
 
 
 MAX_CACHE_SIZE = 200
-_PARSE_CACHE = {}
+_PARSE_CACHE: Dict[str, Dict[str, Any]] = {}
 
-_UA_TYPES = str
-if sys.version_info < (3,):
-    _UA_TYPES = (str, unicode)
 
+def _lookup(ua: str):
+    if not isinstance(ua, str):
+        raise TypeError(f"Expected user agent to be a string, got {ua!r}")
 
-def _lookup(ua, args):
-    if not isinstance(ua, _UA_TYPES):
-        raise TypeError("Expected user agent to be a string, got %r" % ua)
-
-    key = (ua, tuple(sorted(args.items())))
-    entry = _PARSE_CACHE.get(key)
+    entry = _PARSE_CACHE.get(ua)
     if entry is not None:
         return entry
 
     if len(_PARSE_CACHE) >= MAX_CACHE_SIZE:
         _PARSE_CACHE.clear()
 
-    v = _PARSE_CACHE[key] = {"string": ua}
+    v = _PARSE_CACHE[ua] = {"string": ua}
     return v
 
 
-def _cached(ua, args, key, fn):
-    entry = _lookup(ua, args)
+def _cached(ua, key, fn):
+    entry = _lookup(ua)
     r = entry.get(key)
     if not r:
-        r = entry[key] = fn(ua, args)
+        r = entry[key] = fn(ua)
     return r
 
 
-def Parse(user_agent_string, **jsParseBits):
+def Parse(user_agent_string: str, **_jsParseBits):
     """Parse all the things
     Args:
       user_agent_string: the full user agent string
     Returns:
       A dictionary containing all parsed bits
     """
-    entry = _lookup(user_agent_string, jsParseBits)
+    if _jsParseBits:
+        warnings.warn(
+            "javascript overrides are not used anymore",
+            category=DeprecationWarning,
+            stacklevel=2,
+        )
+
+    entry = _lookup(user_agent_string)
     # entry is complete, return directly
     if len(entry) == 4:
         return entry
 
     # entry is partially or entirely empty
     if "user_agent" not in entry:
-        entry["user_agent"] = _ParseUserAgent(user_agent_string, jsParseBits)
+        entry["user_agent"] = _ParseUserAgent(user_agent_string)
     if "os" not in entry:
-        entry["os"] = _ParseOS(user_agent_string, jsParseBits)
+        entry["os"] = _ParseOS(user_agent_string)
     if "device" not in entry:
-        entry["device"] = _ParseDevice(user_agent_string, jsParseBits)
+        entry["device"] = _ParseDevice(user_agent_string)
 
     return entry
 
 
-def ParseUserAgent(user_agent_string, **jsParseBits):
+def ParseUserAgent(user_agent_string, **_jsParseBits):
     """Parses the user-agent string for user agent (browser) info.
     Args:
       user_agent_string: The full user-agent string.
     Returns:
       A dictionary containing parsed bits.
     """
-    return _cached(user_agent_string, jsParseBits, "user_agent", _ParseUserAgent)
-
-
-def _ParseUserAgent(user_agent_string, jsParseBits):
-    if jsParseBits:
+    if _jsParseBits:
         warnings.warn(
-            "javascript overrides are deprecated and will be removed next release",
+            "javascript overrides are not used anymore",
             category=DeprecationWarning,
             stacklevel=2,
         )
-    if (
-        "js_user_agent_family" in jsParseBits
-        and jsParseBits["js_user_agent_family"] != ""
-    ):
-        family = jsParseBits["js_user_agent_family"]
-        v1 = jsParseBits.get("js_user_agent_v1") or None
-        v2 = jsParseBits.get("js_user_agent_v2") or None
-        v3 = jsParseBits.get("js_user_agent_v3") or None
-    else:
-        for uaParser in USER_AGENT_PARSERS:
-            family, v1, v2, v3 = uaParser.Parse(user_agent_string)
-            if family:
-                break
+    return _cached(user_agent_string, "user_agent", _ParseUserAgent)
 
-    # Override for Chrome Frame IFF Chrome is enabled.
-    if "js_user_agent_string" in jsParseBits:
-        js_user_agent_string = jsParseBits["js_user_agent_string"]
-        if (
-            js_user_agent_string
-            and js_user_agent_string.find("Chrome/") > -1
-            and user_agent_string.find("chromeframe") > -1
-        ):
-            jsOverride = {}
-            jsOverride = ParseUserAgent(js_user_agent_string)
-            family = "Chrome Frame (%s %s)" % (family, v1)
-            v1 = jsOverride["major"]
-            v2 = jsOverride["minor"]
-            v3 = jsOverride["patch"]
+
+def _ParseUserAgent(user_agent_string):
+    for uaParser in USER_AGENT_PARSERS:
+        family, v1, v2, v3 = uaParser.Parse(user_agent_string)
+        if family:
+            break
 
     family = family or "Other"
     return {
         "family": family,
         "major": v1 or None,
         "minor": v2 or None,
         "patch": v3 or None,
     }
 
 
-def ParseOS(user_agent_string, **jsParseBits):
+def ParseOS(user_agent_string, **_jsParseBits):
     """Parses the user-agent string for operating system info
     Args:
       user_agent_string: The full user-agent string.
     Returns:
       A dictionary containing parsed bits.
     """
-    return _cached(user_agent_string, jsParseBits, "os", _ParseOS)
-
-
-def _ParseOS(user_agent_string, jsParseBits):
-    if jsParseBits:
+    if _jsParseBits:
         warnings.warn(
-            "javascript overrides are deprecated and will be removed next release",
+            "javascript overrides are not used anymore",
             category=DeprecationWarning,
             stacklevel=2,
         )
+    return _cached(user_agent_string, "os", _ParseOS)
+
+
+def _ParseOS(user_agent_string):
     for osParser in OS_PARSERS:
         os, os_v1, os_v2, os_v3, os_v4 = osParser.Parse(user_agent_string)
         if os:
             break
     os = os or "Other"
     return {
         "family": os,
         "major": os_v1,
         "minor": os_v2,
         "patch": os_v3,
         "patch_minor": os_v4,
     }
 
 
-def ParseDevice(user_agent_string, **jsParseBits):
+def ParseDevice(user_agent_string, **_jsParseBits):
     """Parses the user-agent string for device info.
     Args:
         user_agent_string: The full user-agent string.
     Returns:
         A dictionary containing parsed bits.
     """
-    return _cached(user_agent_string, jsParseBits, "device", _ParseDevice)
-
-
-def _ParseDevice(user_agent_string, jsParseBits):
-    if jsParseBits:
+    if _jsParseBits:
         warnings.warn(
-            "javascript overrides are deprecated and will be removed next release",
+            "javascript overrides are not used anymore",
             category=DeprecationWarning,
             stacklevel=2,
         )
+    return _cached(user_agent_string, "device", _ParseDevice)
+
+
+def _ParseDevice(user_agent_string):
     for deviceParser in DEVICE_PARSERS:
         device, brand, model = deviceParser.Parse(user_agent_string)
         if device:
             break
 
     if device is None:
         device = "Other"
@@ -385,49 +321,48 @@
     return {"family": device, "brand": brand, "model": model}
 
 
 def PrettyUserAgent(family, v1=None, v2=None, v3=None):
     """Pretty user agent string."""
     if v3:
         if v3[0].isdigit():
-            return "%s %s.%s.%s" % (family, v1, v2, v3)
+            return f"{family} {v1}.{v2}.{v3}"
         else:
-            return "%s %s.%s%s" % (family, v1, v2, v3)
+            return f"{family} {v1}.{v2}{v3}"
     elif v2:
-        return "%s %s.%s" % (family, v1, v2)
+        return f"{family} {v1}.{v2}"
     elif v1:
-        return "%s %s" % (family, v1)
+        return f"{family} {v1}"
     return family
 
 
 def PrettyOS(os, os_v1=None, os_v2=None, os_v3=None, os_v4=None):
     """Pretty os string."""
     if os_v4:
-        return "%s %s.%s.%s.%s" % (os, os_v1, os_v2, os_v3, os_v4)
+        return f"{os} {os_v1}.{os_v2}.{os_v3}.{os_v4}"
     if os_v3:
         if os_v3[0].isdigit():
-            return "%s %s.%s.%s" % (os, os_v1, os_v2, os_v3)
+            return f"{os} {os_v1}.{os_v2}.{os_v3}"
         else:
-            return "%s %s.%s%s" % (os, os_v1, os_v2, os_v3)
+            return f"{os} {os_v1}.{os_v2}{os_v3}"
     elif os_v2:
-        return "%s %s.%s" % (os, os_v1, os_v2)
+        return f"{os} {os_v1}.{os_v2}"
     elif os_v1:
-        return "%s %s" % (os, os_v1)
+        return f"{os} {os_v1}"
     return os
 
 
 def ParseWithJSOverrides(
     user_agent_string,
     js_user_agent_string=None,
     js_user_agent_family=None,
     js_user_agent_v1=None,
     js_user_agent_v2=None,
     js_user_agent_v3=None,
 ):
-    """backwards compatible. use one of the other Parse methods instead!"""
     warnings.warn(
         "Use Parse (or a specialised parser)", DeprecationWarning, stacklevel=2
     )
 
     # Override via JS properties.
     if js_user_agent_family is not None and js_user_agent_family != "":
         family = js_user_agent_family
@@ -458,61 +393,37 @@
         v2 = ua_dict["minor"]
         v3 = ua_dict["patch"]
 
     return family or "Other", v1, v2, v3
 
 
 def Pretty(family, v1=None, v2=None, v3=None):
-    """backwards compatible. use PrettyUserAgent instead!"""
     warnings.warn("Use PrettyUserAgent", DeprecationWarning, stacklevel=2)
     if v3:
         if v3[0].isdigit():
-            return "%s %s.%s.%s" % (family, v1, v2, v3)
+            return f"{family} {v1}.{v2}.{v3}"
         else:
-            return "%s %s.%s%s" % (family, v1, v2, v3)
+            return f"{family} {v1}.{v2}{v3}"
     elif v2:
-        return "%s %s.%s" % (family, v1, v2)
+        return f"{family} {v1}.{v2}"
     elif v1:
-        return "%s %s" % (family, v1)
+        return f"{family} {v1}"
     return family
 
 
 def GetFilters(
     user_agent_string,
     js_user_agent_string=None,
     js_user_agent_family=None,
     js_user_agent_v1=None,
     js_user_agent_v2=None,
     js_user_agent_v3=None,
 ):
-    """Return the optional arguments that should be saved and used to query.
-
-    js_user_agent_string is always returned if it is present. We really only need
-    it for Chrome Frame. However, I added it in the generally case to find other
-    cases when it is different. When the recording of js_user_agent_string was
-    added, we created new records for all new user agents.
-
-    Since we only added js_document_mode for the IE 9 preview case, it did not
-    cause new user agent records the way js_user_agent_string did.
+    warnings.warn("No use case anymore", DeprecationWarning, stacklevel=2)
 
-    js_document_mode has since been removed in favor of individual property
-    overrides.
-
-    Args:
-      user_agent_string: The full user-agent string.
-      js_user_agent_string: JavaScript ua string from client-side
-      js_user_agent_family: This is an override for the family name to deal
-          with the fact that IE platform preview (for instance) cannot be
-          distinguished by user_agent_string, but only in javascript.
-      js_user_agent_v1: v1 override - see above.
-      js_user_agent_v2: v1 override - see above.
-      js_user_agent_v3: v1 override - see above.
-    Returns:
-      {js_user_agent_string: '[...]', js_family_name: '[...]', etc...}
-    """
     filters = {}
     filterdict = {
         "js_user_agent_string": js_user_agent_string,
         "js_user_agent_family": js_user_agent_family,
         "js_user_agent_v1": js_user_agent_v1,
         "js_user_agent_v2": js_user_agent_v2,
         "js_user_agent_v3": js_user_agent_v3,
@@ -531,15 +442,15 @@
     import yaml
 
     try:
         # Try and use libyaml bindings if available since faster,
         # pyyaml doesn't do it by default (yaml/pyyaml#436)
         from yaml import CSafeLoader as SafeLoader
     except ImportError:
-        from yaml import SafeLoader
+        from yaml import SafeLoader  #  type: ignore
 
     with open(UA_PARSER_YAML, "rb") as fp:
         regexes = yaml.load(fp, Loader=SafeLoader)
 
     USER_AGENT_PARSERS = []
     for _ua_parser in regexes["user_agent_parsers"]:
         _regex = _ua_parser["regex"]
```

### Comparing `ua-parser-up2date-0.16.1/ua_parser_up2date.egg-info/PKG-INFO` & `ua-parser-up2date-0.18.1/src/ua_parser_up2date.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ua-parser-up2date
-Version: 0.16.1
-Summary: Python port of Browserscope's user agent parser that is kept up to date!
-Home-page: https://github.com/robd003/uap-python
-Author: PBS
-Author-email: no-reply@pbs.org
+Version: 0.18.1
+Summary: Python port of Browserscope's user agent parser
+Author-email: Stephen Lamm <slamm@google.com>, PBS <no-reply@pbs.org>, Selwin Ong <selwin.ong@gmail.com>, Matt Robenolt <matt@ydekproductions.com>, Lindsey Simon <lsimon@commoner.com>
+Maintainer-email: masklinn <uap@masklinn.net>
 License: Apache 2.0
-Classifier: Development Status :: 5 - Production/Stable
+Project-URL: repository, https://github.com/robd003/uap-python-up2date
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -18,14 +18,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+Provides-Extra: yaml
+License-File: LICENSE
 
 uap-python
 ==========
 
 An **up to date** python implementation of the UA Parser (https://github.com/ua-parser,
 formerly https://github.com/tobie/ua-parser)
 
@@ -138,12 +140,7 @@
     >>> from ua_parser import user_agent_parser
     >>> import pprint
     >>> pp = pprint.PrettyPrinter(indent=4)
     >>> ua_string = 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2272.104 Safari/537.36'
     >>> parsed_string = user_agent_parser.ParseDevice(ua_string)
     >>> pp.pprint(parsed_string)
     {'brand': 'Apple', 'family': 'Mac', 'model': 'Mac'}
-
-Copyright
----------
-
-Copyright 2008 Google Inc. See ua\_parser/LICENSE for more information
```

