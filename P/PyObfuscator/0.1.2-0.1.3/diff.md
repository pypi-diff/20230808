# Comparing `tmp/PyObfuscator-0.1.2.tar.gz` & `tmp/PyObfuscator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyObfuscator-0.1.2.tar", last modified: Sun Jul  2 17:55:32 2023, max compression
+gzip compressed data, was "PyObfuscator-0.1.3.tar", last modified: Tue Aug  8 06:36:57 2023, max compression
```

## Comparing `PyObfuscator-0.1.2.tar` & `PyObfuscator-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-02 17:55:32.056936 PyObfuscator-0.1.2/
--rw-r--r--   0 kali      (1000) kali      (1000)    35821 2023-07-02 09:32:18.000000 PyObfuscator-0.1.2/LICENSE.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       72 2023-07-02 09:32:18.000000 PyObfuscator-0.1.2/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     8902 2023-07-02 17:55:32.056936 PyObfuscator-0.1.2/PKG-INFO
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-02 17:55:32.056936 PyObfuscator-0.1.2/PyObfuscator.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     8902 2023-07-02 17:55:31.000000 PyObfuscator-0.1.2/PyObfuscator.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      520 2023-07-02 17:55:31.000000 PyObfuscator-0.1.2/PyObfuscator.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-02 17:55:31.000000 PyObfuscator-0.1.2/PyObfuscator.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-07-02 17:55:31.000000 PyObfuscator-0.1.2/PyObfuscator.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-02 17:55:31.000000 PyObfuscator-0.1.2/PyObfuscator.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    40617 2023-07-02 17:42:10.000000 PyObfuscator-0.1.2/PyObfuscator.py
--rw-r--r--   0 kali      (1000) kali      (1000)     7804 2023-07-02 09:32:18.000000 PyObfuscator-0.1.2/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-02 17:55:32.056936 PyObfuscator-0.1.2/examples/
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-02 09:32:18.000000 PyObfuscator-0.1.2/examples/other.py
--rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-07-02 09:32:18.000000 PyObfuscator-0.1.2/examples/other2.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3220 2023-07-02 17:34:38.000000 PyObfuscator-0.1.2/examples/test.py
--rw-r--r--   0 kali      (1000) kali      (1000)      380 2023-07-02 09:32:18.000000 PyObfuscator-0.1.2/examples/test_import.py
--rw-r--r--   0 kali      (1000) kali      (1000)    14243 2023-07-02 17:44:28.000000 PyObfuscator-0.1.2/examples/test_import_level2.py
--rw-r--r--   0 kali      (1000) kali      (1000)    15561 2023-07-02 17:41:22.000000 PyObfuscator-0.1.2/examples/test_level1.py
--rw-r--r--   0 kali      (1000) kali      (1000)    88954 2023-07-02 17:35:40.000000 PyObfuscator-0.1.2/examples/test_level2.py
--rw-r--r--   0 kali      (1000) kali      (1000)    54463 2023-07-02 17:35:46.000000 PyObfuscator-0.1.2/examples/test_level3.py
--rw-r--r--   0 kali      (1000) kali      (1000)   250704 2023-07-02 17:35:52.000000 PyObfuscator-0.1.2/examples/test_level4.py
--rw-r--r--   0 kali      (1000) kali      (1000)   316806 2023-07-02 17:35:58.000000 PyObfuscator-0.1.2/examples/test_level5.py
--rw-r--r--   0 kali      (1000) kali      (1000)  1270388 2023-07-02 17:36:04.000000 PyObfuscator-0.1.2/examples/test_level6.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-02 17:55:32.056936 PyObfuscator-0.1.2/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1633 2023-07-02 09:32:18.000000 PyObfuscator-0.1.2/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-02 17:55:32.056936 PyObfuscator-0.1.2/tests/
--rw-r--r--   0 kali      (1000) kali      (1000)    43367 2023-07-02 09:32:18.000000 PyObfuscator-0.1.2/tests/TestPyObfuscator.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-08 06:36:57.552733 PyObfuscator-0.1.3/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35821 2023-07-02 18:03:50.000000 PyObfuscator-0.1.3/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       72 2023-07-02 18:03:50.000000 PyObfuscator-0.1.3/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     8902 2023-08-08 06:36:57.552733 PyObfuscator-0.1.3/PKG-INFO
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-08 06:36:57.548731 PyObfuscator-0.1.3/PyObfuscator.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     8902 2023-08-08 06:36:57.000000 PyObfuscator-0.1.3/PyObfuscator.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      520 2023-08-08 06:36:57.000000 PyObfuscator-0.1.3/PyObfuscator.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-08-08 06:36:57.000000 PyObfuscator-0.1.3/PyObfuscator.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-08-08 06:36:57.000000 PyObfuscator-0.1.3/PyObfuscator.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-08-08 06:36:57.000000 PyObfuscator-0.1.3/PyObfuscator.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    40876 2023-08-08 06:32:00.000000 PyObfuscator-0.1.3/PyObfuscator.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7804 2023-07-02 18:03:50.000000 PyObfuscator-0.1.3/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-08 06:36:57.552733 PyObfuscator-0.1.3/examples/
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-02 18:03:50.000000 PyObfuscator-0.1.3/examples/other.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-07-02 18:03:50.000000 PyObfuscator-0.1.3/examples/other2.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3220 2023-07-02 18:03:50.000000 PyObfuscator-0.1.3/examples/test.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      380 2023-07-02 18:03:50.000000 PyObfuscator-0.1.3/examples/test_import.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    14243 2023-07-02 18:03:50.000000 PyObfuscator-0.1.3/examples/test_import_level2.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    15561 2023-07-02 18:03:50.000000 PyObfuscator-0.1.3/examples/test_level1.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    88954 2023-07-02 18:03:50.000000 PyObfuscator-0.1.3/examples/test_level2.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    54463 2023-07-02 18:03:50.000000 PyObfuscator-0.1.3/examples/test_level3.py
+-rw-r--r--   0 kali      (1000) kali      (1000)   250704 2023-07-02 18:03:50.000000 PyObfuscator-0.1.3/examples/test_level4.py
+-rw-r--r--   0 kali      (1000) kali      (1000)   316806 2023-07-02 18:03:50.000000 PyObfuscator-0.1.3/examples/test_level5.py
+-rw-r--r--   0 kali      (1000) kali      (1000)  1270388 2023-07-02 18:03:50.000000 PyObfuscator-0.1.3/examples/test_level6.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-08-08 06:36:57.552733 PyObfuscator-0.1.3/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1633 2023-07-02 18:03:50.000000 PyObfuscator-0.1.3/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-08 06:36:57.552733 PyObfuscator-0.1.3/tests/
+-rw-r--r--   0 kali      (1000) kali      (1000)    43367 2023-07-02 18:03:50.000000 PyObfuscator-0.1.3/tests/TestPyObfuscator.py
```

### Comparing `PyObfuscator-0.1.2/LICENSE.txt` & `PyObfuscator-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyObfuscator-0.1.2/PKG-INFO` & `PyObfuscator-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyObfuscator
-Version: 0.1.2
+Version: 0.1.3
 Summary: This module obfuscates python code.
 Home-page: https://github.com/mauricelambert/PyObfuscator/
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `PyObfuscator-0.1.2/PyObfuscator.egg-info/PKG-INFO` & `PyObfuscator-0.1.3/PyObfuscator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyObfuscator
-Version: 0.1.2
+Version: 0.1.3
 Summary: This module obfuscates python code.
 Home-page: https://github.com/mauricelambert/PyObfuscator/
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `PyObfuscator-0.1.2/PyObfuscator.egg-info/SOURCES.txt` & `PyObfuscator-0.1.3/PyObfuscator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyObfuscator-0.1.2/PyObfuscator.py` & `PyObfuscator-0.1.3/PyObfuscator.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     -----------------------------------------------
     TOTAL                         400      1    99%
 
 """
 
 default_dir = dir()
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = "This module obfuscates python code."
 license = "GPL-3.0 License"
 __url__ = "https://github.com/mauricelambert/PyObfuscator/"
@@ -669,17 +669,21 @@
 
         targets = []
         values = []
 
         for element in elements:
             alias = getattr(element, "asname", None) or element.name
 
-            code = None
+            code = (
+                None
+                if "." not in module
+                else f'myimport("{module}", "{element.name}")'
+            )
             for name in module.split(".")[1:]:
-                code = f'getattr(myimport("{module}", "{element.name}"), "{name}")'
+                code = f'getattr({code}, "{name}")'
 
             if is_from_import:
                 code = f"""getattr({code if code else f'myimport("{module}", "{element.name}")'}, "{element.name}")"""
 
             targets.append(NameAst(id=alias, ctx=Store()))
             values.append(parse(code).body[0].value)
 
@@ -731,30 +735,41 @@
             value = ord(car)
             temp_value = randint(value, value * value)
             return f"chr({temp_value} - {temp_value - value})"
 
         functions = (to_hex, to_octal, to_chr, to_chrbin, to_chradd, to_chrsub)
         string_repr = repr(string)
         code = self.code
-        debug('Hard coded string obfuscation: ' + string_repr)
+        debug("Hard coded string obfuscation: " + string_repr)
         while string_repr in code:
-            code = code.replace(string_repr, ' + '.join(choice(functions)(car) for car in string), 1)
+            code = code.replace(
+                string_repr,
+                " + ".join(choice(functions)(car) for car in string),
+                1,
+            )
         self.code = code
         return code
 
     def int_call_obfuscation(self) -> str:
         """
         This method obfuscates int calls for int obfuscation.
         """
 
         code = self.code
         for match in finditer(r"\('0o[0-7]+', 8\)", code):
             string = match.group()
-            debug('Int call obfuscation: ' + repr(string))
-            _8 = choice(('ord("\\x08")', oct(8), bin(8), (lambda x: f"{x} - {x - 8}")(randint(8, 256 * 256))))
+            debug("Int call obfuscation: " + repr(string))
+            _8 = choice(
+                (
+                    'ord("\\x08")',
+                    oct(8),
+                    bin(8),
+                    (lambda x: f"{x} - {x - 8}")(randint(8, 256 * 256)),
+                )
+            )
             value = string.split("'")[1]
             self.code = code.replace(string, f"('{value}', {_8})", 1)
             code = self.string_obfuscation(value)
 
         self.code = code
         return code
 
@@ -779,16 +794,16 @@
         astcode = self.visit(astcode)
 
         attributes_obfuscator = AttributeObfuscation(self)
         astcode = attributes_obfuscator.visit(astcode)
 
         self.code = unparse(astcode)
 
-        self.string_obfuscation('decode')
-        self.code = self.string_obfuscation('utf-8')
+        self.string_obfuscation("decode")
+        self.code = self.string_obfuscation("utf-8")
         self.code = self.int_call_obfuscation()
 
         code = self.add_builtins()
         code = self.gzip(code)
         code = self.xor_code(code)
         code = self.base85(code)
         self.code = self.hexadecimal(code)
@@ -882,17 +897,15 @@
             debug(f"Integer obfuscation for {astcode.value!r}")
             astcode = self.generic_visit(astcode)
             return Call(
                 func=NameAst(
                     id=self.default_names["int"].obfuscation, ctx=Load()
                 ),
                 args=[
-                    Constant(
-                        value=oct(astcode.value)
-                    ),
+                    Constant(value=oct(astcode.value)),
                     Constant(value=8),
                 ],
                 keywords=[],
             )
         else:
             info(
                 f"In format string {astcode.value!r} this constant type can't be obfuscated."
```

### Comparing `PyObfuscator-0.1.2/README.md` & `PyObfuscator-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `PyObfuscator-0.1.2/examples/test.py` & `PyObfuscator-0.1.3/examples/test.py`

 * *Files identical despite different names*

### Comparing `PyObfuscator-0.1.2/examples/test_import_level2.py` & `PyObfuscator-0.1.3/examples/test_import_level2.py`

 * *Files identical despite different names*

### Comparing `PyObfuscator-0.1.2/examples/test_level1.py` & `PyObfuscator-0.1.3/examples/test_level1.py`

 * *Files identical despite different names*

### Comparing `PyObfuscator-0.1.2/examples/test_level2.py` & `PyObfuscator-0.1.3/examples/test_level2.py`

 * *Files identical despite different names*

### Comparing `PyObfuscator-0.1.2/examples/test_level3.py` & `PyObfuscator-0.1.3/examples/test_level3.py`

 * *Files identical despite different names*

### Comparing `PyObfuscator-0.1.2/examples/test_level4.py` & `PyObfuscator-0.1.3/examples/test_level4.py`

 * *Files identical despite different names*

### Comparing `PyObfuscator-0.1.2/examples/test_level5.py` & `PyObfuscator-0.1.3/examples/test_level5.py`

 * *Files identical despite different names*

### Comparing `PyObfuscator-0.1.2/examples/test_level6.py` & `PyObfuscator-0.1.3/examples/test_level6.py`

 * *Files identical despite different names*

### Comparing `PyObfuscator-0.1.2/setup.py` & `PyObfuscator-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `PyObfuscator-0.1.2/tests/TestPyObfuscator.py` & `PyObfuscator-0.1.3/tests/TestPyObfuscator.py`

 * *Files identical despite different names*

