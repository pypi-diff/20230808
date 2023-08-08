# Comparing `tmp/ldif-4.2.0.tar.gz` & `tmp/ldif-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldif-4.2.0.tar", max compression
+gzip compressed data, was "ldif-4.2.1.tar", max compression
```

## Comparing `ldif-4.2.0.tar` & `ldif-4.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1399 2020-11-16 18:16:35.000000 ldif-4.2.0/LICENSE
--rw-r--r--   0        0        0     2012 2021-04-22 07:20:35.000000 ldif-4.2.0/README.md
--rw-r--r--   0        0        0     1334 2023-03-29 08:39:27.287024 ldif-4.2.0/pyproject.toml
--rw-r--r--   0        0        0    13072 2021-02-16 10:27:47.000000 ldif-4.2.0/src/ldif.py
--rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 ldif-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1399 2020-11-16 18:16:35.000000 ldif-4.2.1/LICENSE
+-rw-r--r--   0        0        0     2054 2023-03-29 08:42:39.861991 ldif-4.2.1/README.md
+-rw-r--r--   0        0        0     1396 2023-08-08 12:55:17.098442 ldif-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0    13070 2023-08-08 12:53:58.679688 ldif-4.2.1/src/ldif.py
+-rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 ldif-4.2.1/PKG-INFO
```

### Comparing `ldif-4.2.0/LICENSE` & `ldif-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ldif-4.2.0/README.md` & `ldif-4.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -56,7 +56,12 @@
 There is no way of knowing the encoding of this data. To handle this,
 there are two modes:
 
 By default, the `LDIFParser` will try to interpret all values as UTF-8
 and leave only the ones that fail to decode as bytes. But you can also
 pass an `encoding` of `None` to the constructor, in which case the
 parser will not try to do any conversion and return bytes directly.
+
+
+## Changelog
+
+See [here](./CHANGES.rst)
```

### Comparing `ldif-4.2.0/pyproject.toml` & `ldif-4.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ldif"
-version = "4.2.0"
+version = "4.2.1"
 description = "generate and parse LDIF data (see RFC 2849)."
 license = "BSD"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "License :: OSI Approved :: BSD License",
@@ -34,14 +34,17 @@
 
 # Doc
 sphinx = "*"
 sphinx-rtd-theme = "*"
 restructuredtext_lint = "*"
 recommonmark = "*"
 
+[tool.poetry.group.dev.dependencies]
+docformatter = "^1.6.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `ldif-4.2.0/src/ldif.py` & `ldif-4.2.1/src/ldif.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,17 +174,16 @@
                 self._output_file.write(b"-" + self._line_sep)
 
     def unparse(self, dn: str, record: Union[list, dict]):
         """Write an entry or change record to the output file.
 
         :type dn: string
         :param dn: distinguished name
-
         :type record: Union[Dict[string, List[string]], List[Tuple]]
-        :param record: Either a dictionary holding  an entry or a list of
+        :param record: Either a dictionary holding an entry or a list of
             additions (2-tuple) or modifications (3-tuple).
         """
         self._unparse_attr("dn", dn)
         if isinstance(record, dict):
             self._unparse_entry_record(record)
         elif isinstance(record, list):
             self._unparse_change_record(record)
```

### Comparing `ldif-4.2.0/PKG-INFO` & `ldif-4.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldif
-Version: 4.2.0
+Version: 4.2.1
 Summary: generate and parse LDIF data (see RFC 2849).
 Home-page: https://github.com/abilian/ldif
 License: BSD
 Author: Abilian SAS
 Author-email: dev@abilian.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -81,7 +81,12 @@
 there are two modes:
 
 By default, the `LDIFParser` will try to interpret all values as UTF-8
 and leave only the ones that fail to decode as bytes. But you can also
 pass an `encoding` of `None` to the constructor, in which case the
 parser will not try to do any conversion and return bytes directly.
 
+
+## Changelog
+
+See [here](./CHANGES.rst)
+
```

