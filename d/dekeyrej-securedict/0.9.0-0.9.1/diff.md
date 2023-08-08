# Comparing `tmp/dekeyrej-securedict-0.9.0.tar.gz` & `tmp/dekeyrej-securedict-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dekeyrej-securedict-0.9.0.tar", last modified: Sun Jul 16 20:10:54 2023, max compression
+gzip compressed data, was "dekeyrej-securedict-0.9.1.tar", last modified: Tue Aug  8 02:35:26 2023, max compression
```

## Comparing `dekeyrej-securedict-0.9.0.tar` & `dekeyrej-securedict-0.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 20:10:54.883452 dekeyrej-securedict-0.9.0/
--rw-rw-rw-   0        0        0     1102 2023-07-16 19:30:57.000000 dekeyrej-securedict-0.9.0/LICENSE
--rw-rw-rw-   0        0        0        0 2023-07-16 19:09:30.000000 dekeyrej-securedict-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1671 2023-07-16 20:10:54.883452 dekeyrej-securedict-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0       81 2023-07-16 20:07:36.000000 dekeyrej-securedict-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 20:10:54.865098 dekeyrej-securedict-0.9.0/dekeyrej_securedict.egg-info/
--rw-rw-rw-   0        0        0     1671 2023-07-16 20:10:54.000000 dekeyrej-securedict-0.9.0/dekeyrej_securedict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-16 20:10:54.000000 dekeyrej-securedict-0.9.0/dekeyrej_securedict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 20:10:54.000000 dekeyrej-securedict-0.9.0/dekeyrej_securedict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-16 20:10:54.000000 dekeyrej-securedict-0.9.0/dekeyrej_securedict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-16 20:10:54.000000 dekeyrej-securedict-0.9.0/dekeyrej_securedict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      659 2023-07-16 20:09:39.000000 dekeyrej-securedict-0.9.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-16 20:10:54.879099 dekeyrej-securedict-0.9.0/securedict/
--rw-rw-rw-   0        0        0       88 2023-07-04 21:17:52.000000 dekeyrej-securedict-0.9.0/securedict/__init__.py
--rw-rw-rw-   0        0        0     2286 2023-07-16 00:08:40.000000 dekeyrej-securedict-0.9.0/securedict/decrypt.py
--rw-rw-rw-   0        0        0     3433 2023-07-05 02:48:02.000000 dekeyrej-securedict-0.9.0/securedict/encrypt.py
--rw-rw-rw-   0        0        0       42 2023-07-16 20:10:54.883452 dekeyrej-securedict-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      385 2023-07-04 21:16:57.000000 dekeyrej-securedict-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 20:10:54.882419 dekeyrej-securedict-0.9.0/tests/
--rw-rw-rw-   0        0        0      565 2023-07-05 02:56:52.000000 dekeyrej-securedict-0.9.0/tests/test_enc_dec.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:35:26.043480 dekeyrej-securedict-0.9.1/
+-rw-rw-rw-   0        0        0     1102 2023-08-08 02:21:14.000000 dekeyrej-securedict-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-08-08 02:21:14.000000 dekeyrej-securedict-0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1690 2023-08-08 02:35:26.042486 dekeyrej-securedict-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      100 2023-08-08 02:34:48.000000 dekeyrej-securedict-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 02:35:26.039486 dekeyrej-securedict-0.9.1/dekeyrej_securedict.egg-info/
+-rw-rw-rw-   0        0        0     1690 2023-08-08 02:35:26.000000 dekeyrej-securedict-0.9.1/dekeyrej_securedict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-08-08 02:35:26.000000 dekeyrej-securedict-0.9.1/dekeyrej_securedict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 02:35:26.000000 dekeyrej-securedict-0.9.1/dekeyrej_securedict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-08-08 02:35:26.000000 dekeyrej-securedict-0.9.1/dekeyrej_securedict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-08 02:35:26.000000 dekeyrej-securedict-0.9.1/dekeyrej_securedict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1162 2023-08-08 02:34:48.000000 dekeyrej-securedict-0.9.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-08 02:35:26.041480 dekeyrej-securedict-0.9.1/securedict/
+-rw-rw-rw-   0        0        0       88 2023-08-08 02:21:14.000000 dekeyrej-securedict-0.9.1/securedict/__init__.py
+-rw-rw-rw-   0        0        0     2286 2023-08-08 02:21:14.000000 dekeyrej-securedict-0.9.1/securedict/decrypt.py
+-rw-rw-rw-   0        0        0     3433 2023-08-08 02:21:14.000000 dekeyrej-securedict-0.9.1/securedict/encrypt.py
+-rw-rw-rw-   0        0        0       42 2023-08-08 02:35:26.043480 dekeyrej-securedict-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      385 2023-08-08 02:34:48.000000 dekeyrej-securedict-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 02:35:26.042486 dekeyrej-securedict-0.9.1/tests/
+-rw-rw-rw-   0        0        0      600 2023-08-08 02:21:14.000000 dekeyrej-securedict-0.9.1/tests/test_enc_dec.py
```

### Comparing `dekeyrej-securedict-0.9.0/LICENSE` & `dekeyrej-securedict-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dekeyrej-securedict-0.9.0/PKG-INFO` & `dekeyrej-securedict-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dekeyrej-securedict
-Version: 0.9.0
+Version: 0.9.1
 Summary: value encryption for secrets
 Author: J.DeKeyrel
 Author-email: "J. DeKeyrel" <noneyabusiness@notemail.com>
 License: The MIT License (MIT)
         Copyright © 2023 <copyright J. DeKeyrel>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -15,8 +15,9 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+{version='0.9.1'}
 encrypts and decrypts python dicts - values are encrpyted, keys are NOT encrypted
```

### Comparing `dekeyrej-securedict-0.9.0/dekeyrej_securedict.egg-info/PKG-INFO` & `dekeyrej-securedict-0.9.1/dekeyrej_securedict.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dekeyrej-securedict
-Version: 0.9.0
+Version: 0.9.1
 Summary: value encryption for secrets
 Author: J.DeKeyrel
 Author-email: "J. DeKeyrel" <noneyabusiness@notemail.com>
 License: The MIT License (MIT)
         Copyright © 2023 <copyright J. DeKeyrel>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -15,8 +15,9 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+{version='0.9.1'}
 encrypts and decrypts python dicts - values are encrpyted, keys are NOT encrypted
```

### Comparing `dekeyrej-securedict-0.9.0/securedict/decrypt.py` & `dekeyrej-securedict-0.9.1/securedict/decrypt.py`

 * *Files identical despite different names*

### Comparing `dekeyrej-securedict-0.9.0/securedict/encrypt.py` & `dekeyrej-securedict-0.9.1/securedict/encrypt.py`

 * *Files identical despite different names*

### Comparing `dekeyrej-securedict-0.9.0/tests/test_enc_dec.py` & `dekeyrej-securedict-0.9.1/tests/test_enc_dec.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,19 +6,20 @@
     secrets = {
         "Key1" : "Value1",
         "Key2" : "Value2",
         "Key3" : "Value3",
     }
 
     ed = EncryptDicts()
-    dd = DecryptDicts()
-
     ed.new_key("testRefKey.txt")
     ed.encrypt_dict(secrets)
     ed.write_dict("encsecrets.py")
     # print(json.dumps(ed._encdict,indent=2))
 
+    assert ed._encdict != secrets
+
+    dd = DecryptDicts()
     dd.read_key_from_file("testRefKey.txt")
     dec = dd.decrypt_dict(ed._encdict)
     # print(json.dumps(dec,indent=2))
 
     assert dec == secrets
```

