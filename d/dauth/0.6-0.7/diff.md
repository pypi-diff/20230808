# Comparing `tmp/dauth-0.6.tar.gz` & `tmp/dauth-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dauth-0.6.tar", last modified: Mon Jul 31 08:23:27 2023, max compression
+gzip compressed data, was "dauth-0.7.tar", last modified: Tue Aug  8 17:12:36 2023, max compression
```

## Comparing `dauth-0.6.tar` & `dauth-0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 denvilk    (501) staff       (20)        0 2023-07-31 08:23:27.401097 dauth-0.6/
--rw-r--r--   0 denvilk    (501) staff       (20)     2541 2023-07-31 08:23:27.400995 dauth-0.6/PKG-INFO
--rw-r--r--   0 denvilk    (501) staff       (20)     2405 2023-07-31 08:18:49.000000 dauth-0.6/README.md
--rw-r--r--   0 denvilk    (501) staff       (20)       38 2023-07-31 08:23:27.401125 dauth-0.6/setup.cfg
--rw-r--r--   0 denvilk    (501) staff       (20)      570 2023-07-31 08:23:14.000000 dauth-0.6/setup.py
-drwxr-xr-x   0 denvilk    (501) staff       (20)        0 2023-07-31 08:23:27.399860 dauth-0.6/src/
-drwxr-xr-x   0 denvilk    (501) staff       (20)        0 2023-07-31 08:23:27.400265 dauth-0.6/src/dauth/
--rw-r--r--   0 denvilk    (501) staff       (20)      187 2023-07-31 08:12:43.000000 dauth-0.6/src/dauth/__init__.py
--rw-r--r--   0 denvilk    (501) staff       (20)      770 2023-07-31 08:15:56.000000 dauth-0.6/src/dauth/auth.py
-drwxr-xr-x   0 denvilk    (501) staff       (20)        0 2023-07-31 08:23:27.400856 dauth-0.6/src/dauth.egg-info/
--rw-r--r--   0 denvilk    (501) staff       (20)     2541 2023-07-31 08:23:27.000000 dauth-0.6/src/dauth.egg-info/PKG-INFO
--rw-r--r--   0 denvilk    (501) staff       (20)      190 2023-07-31 08:23:27.000000 dauth-0.6/src/dauth.egg-info/SOURCES.txt
--rw-r--r--   0 denvilk    (501) staff       (20)        1 2023-07-31 08:23:27.000000 dauth-0.6/src/dauth.egg-info/dependency_links.txt
--rw-r--r--   0 denvilk    (501) staff       (20)        6 2023-07-31 08:23:27.000000 dauth-0.6/src/dauth.egg-info/top_level.txt
+drwxr-xr-x   0 denvilk    (501) staff       (20)        0 2023-08-08 17:12:36.749562 dauth-0.7/
+-rw-r--r--   0 denvilk    (501) staff       (20)     2541 2023-08-08 17:12:36.749355 dauth-0.7/PKG-INFO
+-rw-r--r--   0 denvilk    (501) staff       (20)     2405 2023-07-31 08:18:49.000000 dauth-0.7/README.md
+-rw-r--r--   0 denvilk    (501) staff       (20)       38 2023-08-08 17:12:36.749596 dauth-0.7/setup.cfg
+-rw-r--r--   0 denvilk    (501) staff       (20)      570 2023-08-08 17:12:26.000000 dauth-0.7/setup.py
+drwxr-xr-x   0 denvilk    (501) staff       (20)        0 2023-08-08 17:12:36.747724 dauth-0.7/src/
+drwxr-xr-x   0 denvilk    (501) staff       (20)        0 2023-08-08 17:12:36.748330 dauth-0.7/src/dauth/
+-rw-r--r--   0 denvilk    (501) staff       (20)      187 2023-07-31 08:12:43.000000 dauth-0.7/src/dauth/__init__.py
+-rw-r--r--   0 denvilk    (501) staff       (20)      809 2023-08-08 17:04:22.000000 dauth-0.7/src/dauth/auth.py
+drwxr-xr-x   0 denvilk    (501) staff       (20)        0 2023-08-08 17:12:36.749090 dauth-0.7/src/dauth.egg-info/
+-rw-r--r--   0 denvilk    (501) staff       (20)     2541 2023-08-08 17:12:36.000000 dauth-0.7/src/dauth.egg-info/PKG-INFO
+-rw-r--r--   0 denvilk    (501) staff       (20)      190 2023-08-08 17:12:36.000000 dauth-0.7/src/dauth.egg-info/SOURCES.txt
+-rw-r--r--   0 denvilk    (501) staff       (20)        1 2023-08-08 17:12:36.000000 dauth-0.7/src/dauth.egg-info/dependency_links.txt
+-rw-r--r--   0 denvilk    (501) staff       (20)        6 2023-08-08 17:12:36.000000 dauth-0.7/src/dauth.egg-info/top_level.txt
```

### Comparing `dauth-0.6/PKG-INFO` & `dauth-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dauth
-Version: 0.6
+Version: 0.7
 Summary: FastAPI ABAC authorization realization
 Description-Content-Type: text/markdown
 
 # DAuth 
 
 Python FastAPI ABAC Realization.
```

### Comparing `dauth-0.6/README.md` & `dauth-0.7/README.md`

 * *Files identical despite different names*

### Comparing `dauth-0.6/setup.py` & `dauth-0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 print(long_description)
 
 if __name__ == '__main__':
     setup(
         name='dauth',
-        version="0.6",
+        version="0.7",
         package_dir={'': 'src'},
         packages=find_packages('src', include=[
             'dauth*'
         ]),
         description='FastAPI ABAC authorization realization',
         long_description=long_description,
         long_description_content_type='text/markdown',
```

### Comparing `dauth-0.6/src/dauth/auth.py` & `dauth-0.7/src/dauth/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,7 +20,10 @@
         item_id: Union[str, int] = "*",
     ) -> Any:
         '''Function that checks policy'''
         check_callback(subject, resource_type, item_id, method, database, cache)
         return subject
 
     return _check
+
+def AnyUser(*args, **kwargs):
+    pass
```

### Comparing `dauth-0.6/src/dauth.egg-info/PKG-INFO` & `dauth-0.7/src/dauth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dauth
-Version: 0.6
+Version: 0.7
 Summary: FastAPI ABAC authorization realization
 Description-Content-Type: text/markdown
 
 # DAuth 
 
 Python FastAPI ABAC Realization.
```

