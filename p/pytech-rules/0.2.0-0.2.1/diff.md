# Comparing `tmp/pytech_rules-0.2.0.tar.gz` & `tmp/pytech_rules-0.2.1.tar.gz`

## Comparing `pytech_rules-0.2.0.tar` & `pytech_rules-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytech_rules-0.2.0/pytech/rules/__init__.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 pytech_rules-0.2.0/pytech/rules/conversions.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 pytech_rules-0.2.0/pytech/rules/rules.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pytech_rules-0.2.0/.gitignore
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pytech_rules-0.2.0/LICENCE
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pytech_rules-0.2.0/README.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 pytech_rules-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pytech_rules-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytech_rules-0.2.1/pytech/rules/__init__.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 pytech_rules-0.2.1/pytech/rules/conversions.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 pytech_rules-0.2.1/pytech/rules/rules.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pytech_rules-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 pytech_rules-0.2.1/LICENCE
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pytech_rules-0.2.1/README.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 pytech_rules-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pytech_rules-0.2.1/PKG-INFO
```

### Comparing `pytech_rules-0.2.0/pytech/rules/conversions.py` & `pytech_rules-0.2.1/pytech/rules/conversions.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,14 +43,24 @@
 
     :param list_of_elements: a list of elements
     :return: the last element of the list
     """
     return list_of_elements[-1]
 
 
+def make_false(*_) -> bool:
+    """
+    A function that always returns False.
+
+    :param _: any number of values
+    :return: False
+    """
+    return False
+
+
 def no_conversion(n: any) -> any:
     """
     A function that returns the param as is.
     :param n: the value to return
     :return: the given param
     """
     return n
```

### Comparing `pytech_rules-0.2.0/pytech/rules/rules.py` & `pytech_rules-0.2.1/pytech/rules/rules.py`

 * *Files identical despite different names*

### Comparing `pytech_rules-0.2.0/LICENCE` & `pytech_rules-0.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `pytech_rules-0.2.0/pyproject.toml` & `pytech_rules-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytech-rules"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name = "Alessandro Grandi", email = "alessandro.grandi@pytech.it" },
 ]
 description = "PyTech Rules Project"
 readme = "README.md"
 dependencies = []
 requires-python = ">=3"
```

### Comparing `pytech_rules-0.2.0/PKG-INFO` & `pytech_rules-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytech-rules
-Version: 0.2.0
+Version: 0.2.1
 Summary: PyTech Rules Project
 Project-URL: Homepage, https://gitlab.com/pytech-srl/resources/pytech-rules/
 Project-URL: Bug Tracker, https://gitlab.com/pytech-srl/resources/pytech-rules/-/issues
 Project-URL: Documentation, https://pytech-srl.gitlab.io/resources/pytech-rules/
 Author-email: Alessandro Grandi <alessandro.grandi@pytech.it>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
```

