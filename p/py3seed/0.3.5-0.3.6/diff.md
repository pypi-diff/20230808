# Comparing `tmp/py3seed-0.3.5.tar.gz` & `tmp/py3seed-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.3.5.tar", last modified: Sat Aug  5 08:11:26 2023, max compression
+gzip compressed data, was "py3seed-0.3.6.tar", last modified: Tue Aug  8 12:57:59 2023, max compression
```

## Comparing `py3seed-0.3.5.tar` & `py3seed-0.3.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-05 08:11:26.360540 py3seed-0.3.5/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.3.5/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-05 08:11:26.360674 py3seed-0.3.5/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.3.5/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.3.5/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-08-05 08:11:26.361331 py3seed-0.3.5/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.3.5/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-05 08:11:26.338875 py3seed-0.3.5/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-05 08:11:26.353262 py3seed-0.3.5/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.3.5/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.3.5/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.3.5/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.3.5/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-05 08:11:26.356293 py3seed-0.3.5/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.3.5/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    22814 2023-08-05 06:24:39.000000 py3seed-0.3.5/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.3.5/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.3.5/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.3.5/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.3.5/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-31 04:55:20.000000 py3seed-0.3.5/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.3.5/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    15080 2023-08-05 08:05:06.000000 py3seed-0.3.5/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.3.5/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-05 08:11:26.355361 py3seed-0.3.5/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-05 08:11:26.000000 py3seed-0.3.5/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-08-05 08:11:26.000000 py3seed-0.3.5/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-08-05 08:11:26.000000 py3seed-0.3.5/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-08-05 08:11:26.000000 py3seed-0.3.5/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-08-05 08:11:26.000000 py3seed-0.3.5/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-08-05 08:11:26.000000 py3seed-0.3.5/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-05 08:11:26.360021 py3seed-0.3.5/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.3.5/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6832 2023-08-05 08:10:59.000000 py3seed-0.3.5/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.3.5/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.3.5/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.3.5/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-08 12:57:59.417404 py3seed-0.3.6/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.3.6/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-08 12:57:59.417533 py3seed-0.3.6/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.3.6/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.3.6/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-08-08 12:57:59.418160 py3seed-0.3.6/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.3.6/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-08 12:57:59.391421 py3seed-0.3.6/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-08 12:57:59.406749 py3seed-0.3.6/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.3.6/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.3.6/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.3.6/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     8042 2023-08-08 12:56:48.000000 py3seed-0.3.6/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-08 12:57:59.412673 py3seed-0.3.6/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.3.6/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    22814 2023-08-05 06:24:39.000000 py3seed-0.3.6/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.3.6/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.3.6/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.3.6/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.3.6/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-31 04:55:20.000000 py3seed-0.3.6/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.3.6/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    15080 2023-08-05 08:05:06.000000 py3seed-0.3.6/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.3.6/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-08 12:57:59.411718 py3seed-0.3.6/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-08 12:57:59.000000 py3seed-0.3.6/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-08-08 12:57:59.000000 py3seed-0.3.6/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-08-08 12:57:59.000000 py3seed-0.3.6/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-08-08 12:57:59.000000 py3seed-0.3.6/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-08-08 12:57:59.000000 py3seed-0.3.6/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-08-08 12:57:59.000000 py3seed-0.3.6/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-08 12:57:59.416819 py3seed-0.3.6/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     4144 2023-08-08 12:56:48.000000 py3seed-0.3.6/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6832 2023-08-05 08:10:59.000000 py3seed-0.3.6/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.3.6/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.3.6/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.3.6/tests/test_mongosupport.py
```

### Comparing `py3seed-0.3.5/LICENSE` & `py3seed-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/PKG-INFO` & `py3seed-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.3.5
+Version: 0.3.6
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.3.5/setup.cfg` & `py3seed-0.3.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.3.5
+version = 0.3.6
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.3.5/src/py3seed/__init__.py` & `py3seed-0.3.6/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/src/py3seed/__main__.py` & `py3seed-0.3.6/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/src/py3seed/admin.py` & `py3seed-0.3.6/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/src/py3seed/cachesupport.py` & `py3seed-0.3.6/src/py3seed/cachesupport.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,24 +71,34 @@
         :param filter_: in mongodb's format, e.g, {name:xxx} or {id:{$in:[]}}
         """
         collection = cls.get_collection(**kwargs)
         records = [record for record in collection if cls.match_record(record, filter_)]
         # sort, [(field, order)], order ASCENDING = 1, order DESCENDING = -1
         if 'sort' in kwargs:
             sort = kwargs['sort']
+            # Do not support multi key sorting
             if len(sort) > 1:
                 raise NotImplementedError(f'UNSUPPORTED sort: {sort}')
             #
             field, order = sort[0]
             records.sort(key=lambda x: x.get(field), reverse=(True if order == -1 else False))
         # pagination
         if 'skip' in kwargs:
             records = records[kwargs['skip']:kwargs['skip'] + kwargs['limit']]
         #
-        return [cls(r) for r in records]
+        ret = [cls(r) for r in records]
+        # projection, [field], used to specify a subset of fields that should be included in the result documents
+        if 'projection' in kwargs:
+            projection = kwargs['projection']
+            if cls.__id_name__ not in projection:
+                projection.insert(0, cls.__id_name__)
+            #
+            ret = list(map(lambda x: {k: getattr(x, k) for k in projection}, ret))
+        #
+        return ret
 
     @classmethod
     def count(cls, filter_=None, **kwargs):
         """ Count reconds. """
         collection = cls.get_collection(**kwargs)
         records = [record for record in collection if cls.match_record(record, filter_)]
         return len(records)
```

### Comparing `py3seed-0.3.5/src/py3seed/commands/gen.py` & `py3seed-0.3.6/src/py3seed/commands/gen.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/src/py3seed/error.py` & `py3seed-0.3.6/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/src/py3seed/inflection.py` & `py3seed-0.3.6/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/src/py3seed/log.py` & `py3seed-0.3.6/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/src/py3seed/merge3.py` & `py3seed-0.3.6/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/src/py3seed/model.py` & `py3seed-0.3.6/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/src/py3seed/mongosupport.py` & `py3seed-0.3.6/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/src/py3seed/utils.py` & `py3seed-0.3.6/src/py3seed/utils.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/src/py3seed/websupport.py` & `py3seed-0.3.6/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.3.6/src/py3seed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.3.5
+Version: 0.3.6
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.3.5/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.3.6/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/tests/test_cachesupport.py` & `py3seed-0.3.6/tests/test_cachesupport.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,14 +86,16 @@
     user2.name = 'user2'
     user2.save()
     assert user2.id == 2
     assert len(team1.members) == 2
 
     # Q
     assert CUser.find_by_ids([1, 2])[1].name == user2.name
+    # projection
+    assert CUser.find({'name': 'user2'}, projection=['name'])[0] == {'id': 2, 'name': 'user2'}
 
     # D
     assert user2.delete()
     assert CUser.find_one(2) is None
     assert len(CUser.find({'name': 'user2'})) == 0
     assert CUser.count() == 1
```

### Comparing `py3seed-0.3.5/tests/test_gen.py` & `py3seed-0.3.6/tests/test_gen.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/tests/test_merge3.py` & `py3seed-0.3.6/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/tests/test_model.py` & `py3seed-0.3.6/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.5/tests/test_mongosupport.py` & `py3seed-0.3.6/tests/test_mongosupport.py`

 * *Files identical despite different names*

