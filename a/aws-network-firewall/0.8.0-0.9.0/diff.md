# Comparing `tmp/aws_network_firewall-0.8.0.tar.gz` & `tmp/aws_network_firewall-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_network_firewall-0.8.0.tar", max compression
+gzip compressed data, was "aws_network_firewall-0.9.0.tar", max compression
```

## Comparing `aws_network_firewall-0.8.0.tar` & `aws_network_firewall-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,32 @@
--rw-r--r--   0        0        0    11335 2023-08-07 13:46:42.178762 aws_network_firewall-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0      800 2023-08-07 13:46:42.178762 aws_network_firewall-0.8.0/README.md
--rw-r--r--   0        0        0       22 2023-08-07 13:46:43.358822 aws_network_firewall-0.8.0/aws_network_firewall/__init__.py
--rw-r--r--   0        0        0     1776 2023-08-07 13:46:42.178762 aws_network_firewall-0.8.0/aws_network_firewall/account.py
--rw-r--r--   0        0        0      175 2023-08-07 13:46:42.178762 aws_network_firewall-0.8.0/aws_network_firewall/cidr_range.py
--rw-r--r--   0        0        0      387 2023-08-07 13:46:42.178762 aws_network_firewall-0.8.0/aws_network_firewall/cidr_ranges.py
--rw-r--r--   0        0        0      505 2023-08-07 13:46:42.178762 aws_network_firewall-0.8.0/aws_network_firewall/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 13:46:42.178762 aws_network_firewall-0.8.0/aws_network_firewall/cli/commands/__init__.py
--rw-r--r--   0        0        0     1365 2023-08-07 13:46:42.178762 aws_network_firewall-0.8.0/aws_network_firewall/cli/commands/check.py
--rw-r--r--   0        0        0      374 2023-08-07 13:46:42.178762 aws_network_firewall-0.8.0/aws_network_firewall/cli/commands/docs.py
--rw-r--r--   0        0        0     1191 2023-08-07 13:46:42.178762 aws_network_firewall-0.8.0/aws_network_firewall/cli/commands/update.py
--rw-r--r--   0        0        0      744 2023-08-07 13:46:42.178762 aws_network_firewall-0.8.0/aws_network_firewall/cli/handler.py
--rw-r--r--   0        0        0      352 2023-08-07 13:46:42.178762 aws_network_firewall-0.8.0/aws_network_firewall/destination.py
--rw-r--r--   0        0        0     1130 2023-08-07 13:46:42.178762 aws_network_firewall-0.8.0/aws_network_firewall/documentation_generator.py
--rw-r--r--   0        0        0     7161 2023-08-07 13:46:42.182762 aws_network_firewall-0.8.0/aws_network_firewall/rule.py
--rw-r--r--   0        0        0      708 2023-08-07 13:46:42.182762 aws_network_firewall-0.8.0/aws_network_firewall/rule_set.py
--rw-r--r--   0        0        0     2043 2023-08-07 13:46:42.182762 aws_network_firewall-0.8.0/aws_network_firewall/schemas/__init__.py
--rw-r--r--   0        0        0     2773 2023-08-07 13:46:42.182762 aws_network_firewall-0.8.0/aws_network_firewall/schemas/environment.yaml
--rw-r--r--   0        0        0      211 2023-08-07 13:46:42.182762 aws_network_firewall-0.8.0/aws_network_firewall/source.py
--rw-r--r--   0        0        0      210 2023-08-07 13:46:42.182762 aws_network_firewall-0.8.0/aws_network_firewall/suricata/__init__.py
--rw-r--r--   0        0        0      457 2023-08-07 13:46:42.182762 aws_network_firewall-0.8.0/aws_network_firewall/suricata/host.py
--rw-r--r--   0        0        0      473 2023-08-07 13:46:42.182762 aws_network_firewall-0.8.0/aws_network_firewall/suricata/option.py
--rw-r--r--   0        0        0     1215 2023-08-07 13:46:42.182762 aws_network_firewall-0.8.0/aws_network_firewall/suricata/rule.py
--rw-r--r--   0        0        0     1202 2023-08-07 13:46:43.358822 aws_network_firewall-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0      800 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/README.md
+-rw-r--r--   0        0        0       22 2023-08-08 06:52:00.854097 aws_network_firewall-0.9.0/aws_network_firewall/__init__.py
+-rw-r--r--   0        0        0     1776 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/account.py
+-rw-r--r--   0        0        0      175 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/cidr_range.py
+-rw-r--r--   0        0        0      387 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/cidr_ranges.py
+-rw-r--r--   0        0        0      505 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1365 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/cli/commands/check.py
+-rw-r--r--   0        0        0      374 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/cli/commands/docs.py
+-rw-r--r--   0        0        0     1191 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/cli/commands/update.py
+-rw-r--r--   0        0        0      744 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/cli/handler.py
+-rw-r--r--   0        0        0     1140 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/destination.py
+-rw-r--r--   0        0        0     1130 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/documentation_generator.py
+-rw-r--r--   0        0        0        0 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/engines/__init__.py
+-rw-r--r--   0        0        0     1172 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/engines/abstract.py
+-rw-r--r--   0        0        0      829 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/engines/default_rule.py
+-rw-r--r--   0        0        0     1050 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/engines/dns_rule.py
+-rw-r--r--   0        0        0      826 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/engines/icmp_rule.py
+-rw-r--r--   0        0        0      784 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/engines/prefix_list.py
+-rw-r--r--   0        0        0     3873 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/engines/tls_rule.py
+-rw-r--r--   0        0        0     2277 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/rule.py
+-rw-r--r--   0        0        0      708 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/rule_set.py
+-rw-r--r--   0        0        0     2043 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/schemas/__init__.py
+-rw-r--r--   0        0        0     2773 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/schemas/environment.yaml
+-rw-r--r--   0        0        0      211 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/source.py
+-rw-r--r--   0        0        0      210 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/suricata/__init__.py
+-rw-r--r--   0        0        0      457 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/suricata/host.py
+-rw-r--r--   0        0        0      473 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/suricata/option.py
+-rw-r--r--   0        0        0     1215 2023-08-08 06:52:00.046093 aws_network_firewall-0.9.0/aws_network_firewall/suricata/rule.py
+-rw-r--r--   0        0        0     1235 2023-08-08 06:52:00.854097 aws_network_firewall-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.9.0/PKG-INFO
```

### Comparing `aws_network_firewall-0.8.0/LICENSE.txt` & `aws_network_firewall-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.8.0/README.md` & `aws_network_firewall-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.8.0/aws_network_firewall/account.py` & `aws_network_firewall-0.9.0/aws_network_firewall/account.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.8.0/aws_network_firewall/cli/commands/check.py` & `aws_network_firewall-0.9.0/aws_network_firewall/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.8.0/aws_network_firewall/cli/commands/update.py` & `aws_network_firewall-0.9.0/aws_network_firewall/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.8.0/aws_network_firewall/cli/handler.py` & `aws_network_firewall-0.9.0/aws_network_firewall/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.8.0/aws_network_firewall/documentation_generator.py` & `aws_network_firewall-0.9.0/aws_network_firewall/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.8.0/aws_network_firewall/rule_set.py` & `aws_network_firewall-0.9.0/aws_network_firewall/rule_set.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.8.0/aws_network_firewall/schemas/__init__.py` & `aws_network_firewall-0.9.0/aws_network_firewall/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.8.0/aws_network_firewall/schemas/environment.yaml` & `aws_network_firewall-0.9.0/aws_network_firewall/schemas/environment.yaml`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.8.0/aws_network_firewall/suricata/rule.py` & `aws_network_firewall-0.9.0/aws_network_firewall/suricata/rule.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.8.0/pyproject.toml` & `aws_network_firewall-0.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-network-firewall"
-version = "0.8.0"
+version = "0.9.0"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_network_firewall"}]
 
 [tool.poetry.group.dev.dependencies]
@@ -46,13 +46,14 @@
 branch = true
 source = ["aws_network_firewall"]
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 98
 exclude_lines = [
-    "if __name__ == .__main__.:"
+    "if __name__ == .__main__.:",
+    "raise NotImplementedError"
 ]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aws_network_firewall-0.8.0/PKG-INFO` & `aws_network_firewall-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-network-firewall
-Version: 0.8.0
+Version: 0.9.0
 Summary: 
 License: MIT
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

