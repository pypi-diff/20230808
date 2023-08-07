# Comparing `tmp/angola-0.15.0.tar.gz` & `tmp/angola-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.15.0.tar", last modified: Thu Aug  3 08:07:44 2023, max compression
+gzip compressed data, was "angola-0.16.0.tar", last modified: Mon Aug  7 22:25:44 2023, max compression
```

## Comparing `angola-0.15.0.tar` & `angola-0.16.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-08-03 08:07:44.283976 angola-0.15.0/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.15.0/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.15.0/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-08-03 08:07:44.284049 angola-0.15.0/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.15.0/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-08-03 08:07:44.284298 angola-0.15.0/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      793 2023-08-03 07:57:57.000000 angola-0.15.0/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-08-03 08:07:44.277460 angola-0.15.0/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-08-03 08:07:44.281396 angola-0.15.0/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.15.0/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    51001 2023-06-28 16:10:18.000000 angola-0.15.0/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.15.0/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.15.0/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    18665 2023-08-03 08:03:16.000000 angola-0.15.0/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    20084 2023-06-23 04:30:25.000000 angola-0.15.0/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-08-03 08:07:44.282535 angola-0.15.0/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-08-03 08:07:44.000000 angola-0.15.0/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-08-03 08:07:44.000000 angola-0.15.0/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-08-03 08:07:44.000000 angola-0.15.0/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       53 2023-08-03 08:07:44.000000 angola-0.15.0/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-08-03 08:07:44.000000 angola-0.15.0/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-08-03 08:07:44.283864 angola-0.15.0/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.15.0/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.15.0/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.15.0/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     4810 2023-06-30 07:41:06.000000 angola-0.15.0/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.15.0/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-08-07 22:25:44.016766 angola-0.16.0/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.16.0/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.16.0/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-08-07 22:25:44.016839 angola-0.16.0/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.16.0/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-08-07 22:25:44.017098 angola-0.16.0/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      793 2023-08-07 20:44:31.000000 angola-0.16.0/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-08-07 22:25:44.007227 angola-0.16.0/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-08-07 22:25:44.013515 angola-0.16.0/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.16.0/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    51288 2023-08-07 20:43:14.000000 angola-0.16.0/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.16.0/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.16.0/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18678 2023-08-03 20:55:02.000000 angola-0.16.0/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    20084 2023-06-23 04:30:25.000000 angola-0.16.0/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-08-07 22:25:44.014828 angola-0.16.0/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-08-07 22:25:44.000000 angola-0.16.0/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-08-07 22:25:44.000000 angola-0.16.0/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-08-07 22:25:44.000000 angola-0.16.0/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       53 2023-08-07 22:25:44.000000 angola-0.16.0/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-08-07 22:25:44.000000 angola-0.16.0/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-08-07 22:25:44.016662 angola-0.16.0/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.16.0/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.16.0/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.16.0/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     4810 2023-06-30 07:41:06.000000 angola-0.16.0/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.16.0/tests/test_query.py
```

### Comparing `angola-0.15.0/LICENSE` & `angola-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `angola-0.15.0/PKG-INFO` & `angola-0.16.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.15.0
+Version: 0.16.0
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.15.0/README.md` & `angola-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `angola-0.15.0/setup.py` & `angola-0.16.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.15.0"
+VERSION = "0.16.0"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
```

### Comparing `angola-0.15.0/src/angola/database.py` & `angola-0.16.0/src/angola/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -776,14 +776,24 @@
         """
         _dbname = dbname or self.dbname
         sys_db = self.select_db("_system")
         if not sys_db.db.has_database(_dbname):
             sys_db.db.create_database(_dbname)
         return self.select_db(_dbname)
 
+    def delete_db(self, dbname:str) -> bool:
+        """
+        To delete a database 
+
+        """
+        sys_db = self.select_db("_system")
+        if sys_db.db.has_database(dbname):
+            return sys_db.db.delete_database(name=dbname, ignore_missing=True)
+        return False
+
     def select_db(self, dbname:str, collection_prefix:str=None, default_indexes:dict=None) -> "Database":
         """
         Select a different DB using the same connection
 
         Params:
             dbname:str - The dbname to check
             collection_prefix
```

### Comparing `angola-0.15.0/src/angola/dict_mutator.py` & `angola-0.16.0/src/angola/dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.15.0/src/angola/dict_query.py` & `angola-0.16.0/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.15.0/src/angola/lib.py` & `angola-0.16.0/src/angola/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,16 +81,16 @@
     pattern = re.compile(r"^[a-zA-Z\_\$][a-zA-Z0-9\_\-\$]*$")
     return bool(pattern.match(name)) 
 
 
 
 def gen_xid() -> str:
     """
-    XID - To be used as id. 
-    Return CUID2 - 16 chars
+    XID - To generate a random unique ID. 
+    Return CUID2. 16 chars
     """
     l = 16
     return cuid2.Cuid(length=l).generate()
 
 def gen_key() -> str:
     """
     To be used as random key
```

### Comparing `angola-0.15.0/src/angola/lib_xql.py` & `angola-0.16.0/src/angola/lib_xql.py`

 * *Files identical despite different names*

### Comparing `angola-0.15.0/src/angola.egg-info/PKG-INFO` & `angola-0.16.0/src/angola.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.15.0
+Version: 0.16.0
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.15.0/tests/test_database.py` & `angola-0.16.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.15.0/tests/test_dict_mutator.py` & `angola-0.16.0/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.15.0/tests/test_lib.py` & `angola-0.16.0/tests/test_lib.py`

 * *Files identical despite different names*

