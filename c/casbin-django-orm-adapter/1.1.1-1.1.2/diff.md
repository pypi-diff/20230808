# Comparing `tmp/casbin-django-orm-adapter-1.1.1.tar.gz` & `tmp/casbin-django-orm-adapter-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin-django-orm-adapter-1.1.1.tar", last modified: Wed Aug  2 06:09:29 2023, max compression
+gzip compressed data, was "casbin-django-orm-adapter-1.1.2.tar", last modified: Tue Aug  8 06:33:21 2023, max compression
```

## Comparing `casbin-django-orm-adapter-1.1.1.tar` & `casbin-django-orm-adapter-1.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:09:29.799650 casbin-django-orm-adapter-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-08-02 06:09:29.799650 casbin-django-orm-adapter-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:09:29.795650 casbin-django-orm-adapter-1.1.1/casbin_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/casbin_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/casbin_adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/casbin_adapter/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/casbin_adapter/enforcer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:09:29.795650 casbin-django-orm-adapter-1.1.1/casbin_adapter/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/casbin_adapter/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/casbin_adapter/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/casbin_adapter/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/casbin_adapter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:09:29.799650 casbin-django-orm-adapter-1.1.1/casbin_django_orm_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-08-02 06:09:29.000000 casbin-django-orm-adapter-1.1.1/casbin_django_orm_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-02 06:09:29.000000 casbin-django-orm-adapter-1.1.1/casbin_django_orm_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 06:09:29.000000 casbin-django-orm-adapter-1.1.1/casbin_django_orm_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 06:09:29.000000 casbin-django-orm-adapter-1.1.1/casbin_django_orm_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 06:09:29.000000 casbin-django-orm-adapter-1.1.1/casbin_django_orm_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 06:09:29.799650 casbin-django-orm-adapter-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:09:29.799650 casbin-django-orm-adapter-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-08-02 06:09:02.000000 casbin-django-orm-adapter-1.1.1/tests/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:33:21.207105 casbin-django-orm-adapter-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 06:32:47.000000 casbin-django-orm-adapter-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-08-08 06:33:21.207105 casbin-django-orm-adapter-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-08-08 06:32:47.000000 casbin-django-orm-adapter-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:33:21.207105 casbin-django-orm-adapter-1.1.2/casbin_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 06:32:47.000000 casbin-django-orm-adapter-1.1.2/casbin_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-08-08 06:32:47.000000 casbin-django-orm-adapter-1.1.2/casbin_adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-08 06:32:47.000000 casbin-django-orm-adapter-1.1.2/casbin_adapter/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-08 06:32:47.000000 casbin-django-orm-adapter-1.1.2/casbin_adapter/enforcer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:33:21.207105 casbin-django-orm-adapter-1.1.2/casbin_adapter/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-08 06:32:47.000000 casbin-django-orm-adapter-1.1.2/casbin_adapter/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 06:32:47.000000 casbin-django-orm-adapter-1.1.2/casbin_adapter/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-08 06:32:47.000000 casbin-django-orm-adapter-1.1.2/casbin_adapter/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-08 06:32:47.000000 casbin-django-orm-adapter-1.1.2/casbin_adapter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:33:21.207105 casbin-django-orm-adapter-1.1.2/casbin_django_orm_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-08-08 06:33:21.000000 casbin-django-orm-adapter-1.1.2/casbin_django_orm_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-08 06:33:21.000000 casbin-django-orm-adapter-1.1.2/casbin_django_orm_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 06:33:21.000000 casbin-django-orm-adapter-1.1.2/casbin_django_orm_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 06:33:21.000000 casbin-django-orm-adapter-1.1.2/casbin_django_orm_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-08 06:33:21.000000 casbin-django-orm-adapter-1.1.2/casbin_django_orm_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 06:32:47.000000 casbin-django-orm-adapter-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-08 06:33:21.207105 casbin-django-orm-adapter-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-08 06:32:47.000000 casbin-django-orm-adapter-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:33:21.207105 casbin-django-orm-adapter-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-08-08 06:32:47.000000 casbin-django-orm-adapter-1.1.2/tests/test_adapter.py
```

### Comparing `casbin-django-orm-adapter-1.1.1/LICENSE` & `casbin-django-orm-adapter-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.1.1/PKG-INFO` & `casbin-django-orm-adapter-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin-django-orm-adapter
-Version: 1.1.1
+Version: 1.1.2
 Summary: Django's ORM adapter for PyCasbin
 Home-page: https://github.com/pycasbin/django-orm-adapter
 Author: Yang Luo
 Author-email: hsluoyz@qq.com
 License: Apache 2.0
 Keywords: casbin,adapter,storage-driver,django,orm,django-orm,access-control,authorization
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `casbin-django-orm-adapter-1.1.1/README.md` & `casbin-django-orm-adapter-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.1.1/casbin_adapter/adapter.py` & `casbin-django-orm-adapter-1.1.2/casbin_adapter/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             line.v4 = rule[4]
         if len(rule) > 5:
             line.v5 = rule[5]
         return line
 
     def save_policy(self, model):
         """saves all policy rules to the storage."""
-        # See https://casbin.org/docs/en/adapters#autosave
+        # See https://casbin.org/docs/adapters/#autosave
         # for why this is deleting all rules
         CasbinRule.objects.using(self.db_alias).all().delete()
 
         lines = []
         for sec in ["p", "g"]:
             if sec not in model.model.keys():
                 continue
```

### Comparing `casbin-django-orm-adapter-1.1.1/casbin_adapter/enforcer.py` & `casbin-django-orm-adapter-1.1.2/casbin_adapter/enforcer.py`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.1.1/casbin_adapter/migrations/0001_initial.py` & `casbin-django-orm-adapter-1.1.2/casbin_adapter/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.1.1/casbin_adapter/models.py` & `casbin-django-orm-adapter-1.1.2/casbin_adapter/models.py`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.1.1/casbin_django_orm_adapter.egg-info/PKG-INFO` & `casbin-django-orm-adapter-1.1.2/casbin_django_orm_adapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin-django-orm-adapter
-Version: 1.1.1
+Version: 1.1.2
 Summary: Django's ORM adapter for PyCasbin
 Home-page: https://github.com/pycasbin/django-orm-adapter
 Author: Yang Luo
 Author-email: hsluoyz@qq.com
 License: Apache 2.0
 Keywords: casbin,adapter,storage-driver,django,orm,django-orm,access-control,authorization
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `casbin-django-orm-adapter-1.1.1/casbin_django_orm_adapter.egg-info/SOURCES.txt` & `casbin-django-orm-adapter-1.1.2/casbin_django_orm_adapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.1.1/setup.py` & `casbin-django-orm-adapter-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.1.1/tests/test_adapter.py` & `casbin-django-orm-adapter-1.1.2/tests/test_adapter.py`

 * *Files identical despite different names*

