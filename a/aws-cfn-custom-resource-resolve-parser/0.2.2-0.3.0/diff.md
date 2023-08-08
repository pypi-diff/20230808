# Comparing `tmp/aws_cfn_custom_resource_resolve_parser-0.2.2.tar.gz` & `tmp/aws_cfn_custom_resource_resolve_parser-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_cfn_custom_resource_resolve_parser-0.2.2.tar", max compression
+gzip compressed data, was "aws_cfn_custom_resource_resolve_parser-0.3.0.tar", max compression
```

## Comparing `aws_cfn_custom_resource_resolve_parser-0.2.2.tar` & `aws_cfn_custom_resource_resolve_parser-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    16725 2023-04-24 10:02:59.281226 aws_cfn_custom_resource_resolve_parser-0.2.2/LICENSE
--rw-r--r--   0        0        0     1934 2023-04-24 10:02:59.282226 aws_cfn_custom_resource_resolve_parser-0.2.2/README.rst
--rw-r--r--   0        0        0     4347 2023-04-24 10:15:33.641432 aws_cfn_custom_resource_resolve_parser-0.2.2/aws_cfn_custom_resource_resolve_parser/__init__.py
--rw-r--r--   0        0        0     1808 2023-04-24 10:15:33.641432 aws_cfn_custom_resource_resolve_parser-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 aws_cfn_custom_resource_resolve_parser-0.2.2/setup.py
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 aws_cfn_custom_resource_resolve_parser-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-04-24 10:02:59.281226 aws_cfn_custom_resource_resolve_parser-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1934 2023-04-24 10:02:59.282226 aws_cfn_custom_resource_resolve_parser-0.3.0/README.rst
+-rw-r--r--   0        0        0     4131 2023-08-08 05:47:30.239427 aws_cfn_custom_resource_resolve_parser-0.3.0/aws_cfn_custom_resource_resolve_parser/__init__.py
+-rw-r--r--   0        0        0     1797 2023-08-08 05:47:30.239427 aws_cfn_custom_resource_resolve_parser-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 aws_cfn_custom_resource_resolve_parser-0.3.0/PKG-INFO
```

### Comparing `aws_cfn_custom_resource_resolve_parser-0.2.2/LICENSE` & `aws_cfn_custom_resource_resolve_parser-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_cfn_custom_resource_resolve_parser-0.2.2/README.rst` & `aws_cfn_custom_resource_resolve_parser-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `aws_cfn_custom_resource_resolve_parser-0.2.2/aws_cfn_custom_resource_resolve_parser/__init__.py` & `aws_cfn_custom_resource_resolve_parser-0.3.0/aws_cfn_custom_resource_resolve_parser/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #  -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MPL-2.0
 # Copyright 2020-2021 John Mille<john@ews-network.net>
 
 """Top-level package for AWS CFN Custom resource Resolve parser."""
 
+from __future__ import annotations
+
 import base64
 import json
 import re
 
 from boto3.session import Session
 from botocore.exceptions import ClientError
 
 __author__ = """John Preston"""
 __email__ = "john@ews-network.net"
-__version__ = "0.2.2"
+__version__ = "0.3.0"
 
 
 SECRET_ARN_REGEXP = re.compile(
     r"(?:{{resolve:secretsmanager:)"
     r"(?P<arn>arn:(?P<partition>aws(?:-[a-z]+)?):secretsmanager:(?P<region>[a-z0-9-]+):"
     r"(?P<account_id>\d{12}):"
     r"(?:secret:(?P<secret_id>[a-z0-9A-Z-_./]+)))"
@@ -26,94 +28,82 @@
 
 SECRET_NAME_REGEXP = re.compile(
     r"(?:{{resolve:secretsmanager:)(?P<name>[a-z0-9A-Z-_./]+)"
     r"(?P<extra>(?::SecretString:(?P<secret_key>[a-z0-9A-Z-_./]+))(?:(::)(?P<version>[a-z0-9A-Z-]+)?)?)?(?:}})"
 )
 
 
-def keyisset(key, obj):
-    """
-    Function to verify the key is present and contains something in the object
-
-    :param str key:
-    :param dict obj:
-    :rtype: bool
-    """
-    if obj and isinstance(obj, dict) and key in obj.keys() and obj[key]:
+def keypresent(key: str, obj: dict) -> bool:
+    if obj and isinstance(obj, dict) and key in obj.keys():
         return True
     return False
 
 
-def keypresent(key, obj):
-    """
-    Function to verify the key is present in the object
-
-    :param str key:
-    :param dict obj:
-    :rtype: bool
-    """
-    if obj and isinstance(obj, dict) and key in obj.keys():
+def keyisset(key: str, obj: dict) -> bool:
+    if keypresent(key, obj) and obj[key]:
         return True
     return False
 
 
-def parse_secret_resolve_string(resolve_str):
+def parse_secret_resolve_string(resolve_str: str) -> tuple:
     """
-    Function to parse the resolve string and return the parts of it of interest
-
-    :param str resolve_str:
-    :return: tuple of the secret, key and stage.
-    :rtype: tuple
+    Parse the resolve string to find the secret
+    Returns key and stage if found/defined.
     """
-    secret = None
     key = None
     stage = None
     if SECRET_ARN_REGEXP.match(resolve_str):
         parts = SECRET_ARN_REGEXP.match(resolve_str)
         secret = parts.group("arn")
         if not secret:
             raise ValueError("Unable to find the secret ARN in", resolve_str)
         key = parts.group("secret_key")
         stage = parts.group("version")
     elif SECRET_NAME_REGEXP.match(resolve_str):
         parts = SECRET_NAME_REGEXP.match(resolve_str)
         secret = parts.group("name")
+        if not secret:
+            raise ValueError("Unable to find the secret name in", resolve_str)
     else:
         raise ValueError(
             "Unable to define secret ARN nor secret name from", resolve_str
         )
     if parts:
         key = parts.group("secret_key")
         stage = parts.group("version")
 
     return secret, key, stage
 
 
-def retrieve_secret(secret, key=None, stage=None, client=None, session=None):
-    """
-    Function to retrieve the secret. If key is provided, attempts to return only the key value.
-    If stage is provided, retrieves the secret for given stage.
+def retrieve_secret(
+    secret: str, key: str = None, stage: str = None, session: Session = None
+) -> str:
+    """
+    Function to retrieve the secret value.
+    If key is provided, returns the key value. Fails if key does not exist.
+    If stage is provided, retrieves the secret for given stage. Fails if stage does not exist.
 
     :param str secret:
     :param str key:
     :param str stage:
     :param boto3.client client:
     :param boto3.session.Session session:
     :return: The secret string or specific key of
     :raises: KeyError  if the key is provided but not present in secret
     :raises: ClientError in case of an error with boto3
     :raises: ResourceNotFoundException,ResourceNotFoundException if specific issue with secret retrieval
     """
-    if not client and session:
-        client = session.client("secretsmanager")
-    elif not client and not session:
-        client = Session().client("secretsmanager")
+    if session is None or not isinstance(session, Session):
+        session = Session()
+    if stage is None:
+        stage = "AWSCURRENT"
+    client = session.client("secretsmanager")
     try:
         get_secret_value_response = client.get_secret_value(
-            SecretId=secret, VersionStage="AWSCURRENT" if not stage else stage
+            SecretId=secret, VersionStage=stage
         )
         if keyisset("SecretString", get_secret_value_response):
             res = json.loads(get_secret_value_response["SecretString"])
         else:
             res = json.loads(
                 base64.b64decode(get_secret_value_response["SecretBinary"])
             )
@@ -127,16 +117,10 @@
         raise
     except ClientError as error:
         print(error)
         raise
 
 
 def handle(resolve_str):
-    """
-    Main function.
-
-    :param resolve_str:
-    :return:
-    """
-    parts = parse_secret_resolve_string(resolve_str)
-    secret = retrieve_secret(parts[0], parts[1], parts[2])
+    secret_name, key, version = parse_secret_resolve_string(resolve_str)
+    secret = retrieve_secret(secret_name, key, version)
     return secret
```

### Comparing `aws_cfn_custom_resource_resolve_parser-0.2.2/pyproject.toml` & `aws_cfn_custom_resource_resolve_parser-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws_cfn_custom_resource_resolve_parser"
-version = "0.2.2"
+version = "0.3.0"
 description = "AWS CFN Custom Resource parser for dynamic values"
 authors = ["John Preston <john@ews-network.net>"]
 license = "MPL-2.0"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
@@ -16,29 +16,29 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-boto3 = "^1.26"
+boto3 = "^1.28"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
-isort = "^5.12.0"
-placebo = "^0.10.0"
+black = "^23.7"
+isort = "^5.12"
+placebo = "^0.10"
 pytest = "^7.3.1"
 coverage = "^7.2.3"
 Sphinx = "^6.2.0"
 sphinx-material = "^0.0.35"
 pre-commit = "^3.2.2"
 tbump = "^6.9.0"
 
 [build-system]
-requires = ["poetry-core>=1.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
 
 [tool.isort]
 profile = "black"
@@ -49,15 +49,15 @@
 known_first_party = "kelvin"
 
 
 [tool.tbump]
 github_url = "https://github.com/EWS-Network/aws_cfn_custom_resource_resolve_parser"
 
 [tool.tbump.version]
-current = "0.2.2"
+current = "0.3.0"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `aws_cfn_custom_resource_resolve_parser-0.2.2/PKG-INFO` & `aws_cfn_custom_resource_resolve_parser-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cfn-custom-resource-resolve-parser
-Version: 0.2.2
+Version: 0.3.0
 Summary: AWS CFN Custom Resource parser for dynamic values
 License: MPL-2.0
 Author: John Preston
 Author-email: john@ews-network.net
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -14,19 +14,15 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: boto3 (>=1.26,<2.0)
+Requires-Dist: boto3 (>=1.28,<2.0)
 Description-Content-Type: text/x-rst
 
 ======================================
 AWS CFN Custom resource Resolve parser
 ======================================
```

