# Comparing `tmp/ldif-4.2.1.tar.gz` & `tmp/ldif-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldif-4.2.1.tar", max compression
+gzip compressed data, was "ldif-4.2.2.tar", max compression
```

## Comparing `ldif-4.2.1.tar` & `ldif-4.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1399 2020-11-16 18:16:35.000000 ldif-4.2.1/LICENSE
--rw-r--r--   0        0        0     2054 2023-03-29 08:42:39.861991 ldif-4.2.1/README.md
--rw-r--r--   0        0        0     1396 2023-08-08 12:55:17.098442 ldif-4.2.1/pyproject.toml
--rw-r--r--   0        0        0    13070 2023-08-08 12:53:58.679688 ldif-4.2.1/src/ldif.py
--rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 ldif-4.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1399 2020-11-16 18:16:35.000000 ldif-4.2.2/LICENSE
+-rw-r--r--   0        0        0     2054 2023-03-29 08:42:39.861991 ldif-4.2.2/README.md
+-rw-r--r--   0        0        0     1396 2023-08-08 13:28:43.440126 ldif-4.2.2/pyproject.toml
+-rw-r--r--   0        0        0    13165 2023-08-08 13:28:11.029352 ldif-4.2.2/src/ldif.py
+-rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 ldif-4.2.2/PKG-INFO
```

### Comparing `ldif-4.2.1/LICENSE` & `ldif-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ldif-4.2.1/README.md` & `ldif-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ldif-4.2.1/pyproject.toml` & `ldif-4.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ldif"
-version = "4.2.1"
+version = "4.2.2"
 description = "generate and parse LDIF data (see RFC 2849)."
 license = "BSD"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "License :: OSI Approved :: BSD License",
```

### Comparing `ldif-4.2.1/src/ldif.py` & `ldif-4.2.2/src/ldif.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,14 +162,16 @@
                 raise ValueError("Subsequent modlist item of wrong length")
 
             if mod_len == 2:
                 mod_type, mod_vals = mod
             elif mod_len == 3:
                 mod_op, mod_type, mod_vals = mod
                 self._unparse_attr(MOD_OPS[mod_op], mod_type)
+            else:
+                raise ValueError(f"modlist item of wrong length: {mod_len}")
 
             for mod_val in mod_vals:
                 self._unparse_attr(mod_type, mod_val)
 
             if mod_len == 3:
                 self._output_file.write(b"-" + self._line_sep)
```

### Comparing `ldif-4.2.1/PKG-INFO` & `ldif-4.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldif
-Version: 4.2.1
+Version: 4.2.2
 Summary: generate and parse LDIF data (see RFC 2849).
 Home-page: https://github.com/abilian/ldif
 License: BSD
 Author: Abilian SAS
 Author-email: dev@abilian.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

