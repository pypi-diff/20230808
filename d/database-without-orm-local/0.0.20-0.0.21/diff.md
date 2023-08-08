# Comparing `tmp/database-without-orm-local-0.0.20.tar.gz` & `tmp/database-without-orm-local-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-without-orm-local-0.0.20.tar", last modified: Tue Aug  8 14:03:44 2023, max compression
+gzip compressed data, was "database-without-orm-local-0.0.21.tar", last modified: Tue Aug  8 17:21:59 2023, max compression
```

## Comparing `database-without-orm-local-0.0.20.tar` & `database-without-orm-local-0.0.21.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:03:44.162594 database-without-orm-local-0.0.20/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:03:14.000000 database-without-orm-local-0.0.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-08 14:03:44.162594 database-without-orm-local-0.0.20/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:03:44.162594 database-without-orm-local-0.0.20/circles_local_database_python/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 14:03:14.000000 database-without-orm-local-0.0.20/circles_local_database_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-08-08 14:03:14.000000 database-without-orm-local-0.0.20/circles_local_database_python/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-08 14:03:14.000000 database-without-orm-local-0.0.20/circles_local_database_python/connection_cursor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:03:44.162594 database-without-orm-local-0.0.20/database_without_orm_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-08 14:03:44.000000 database-without-orm-local-0.0.20/database_without_orm_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-08 14:03:44.000000 database-without-orm-local-0.0.20/database_without_orm_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:03:44.000000 database-without-orm-local-0.0.20/database_without_orm_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 14:03:44.000000 database-without-orm-local-0.0.20/database_without_orm_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-08 14:03:14.000000 database-without-orm-local-0.0.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 14:03:44.162594 database-without-orm-local-0.0.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-08 14:03:14.000000 database-without-orm-local-0.0.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:21:59.288058 database-without-orm-local-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:21:28.000000 database-without-orm-local-0.0.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-08 17:21:59.288058 database-without-orm-local-0.0.21/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:21:59.288058 database-without-orm-local-0.0.21/circles_local_database_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 17:21:28.000000 database-without-orm-local-0.0.21/circles_local_database_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-08-08 17:21:28.000000 database-without-orm-local-0.0.21/circles_local_database_python/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-08 17:21:28.000000 database-without-orm-local-0.0.21/circles_local_database_python/connection_cursor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:21:59.288058 database-without-orm-local-0.0.21/database_without_orm_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-08 17:21:59.000000 database-without-orm-local-0.0.21/database_without_orm_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-08 17:21:59.000000 database-without-orm-local-0.0.21/database_without_orm_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 17:21:59.000000 database-without-orm-local-0.0.21/database_without_orm_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 17:21:59.000000 database-without-orm-local-0.0.21/database_without_orm_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-08 17:21:28.000000 database-without-orm-local-0.0.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 17:21:59.288058 database-without-orm-local-0.0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-08 17:21:28.000000 database-without-orm-local-0.0.21/setup.py
```

### Comparing `database-without-orm-local-0.0.20/circles_local_database_python/connection.py` & `database-without-orm-local-0.0.21/circles_local_database_python/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         
         # Checking if RDS_HOSTNAME, RDS_USERNAME, and RDS_PASSWORD are set
         if not all([os.getenv("RDS_HOSTNAME"), os.getenv("RDS_USERNAME"), os.getenv("RDS_PASSWORD")]):
             print("Error: Add RDS_HOSTNAME, RDS_USERNAME and RDS_PASSWORD to .env")
             raise Exception("Environment variables not set.")
         
         self.host = host or os.getenv("RDS_HOSTNAME")
-        self.database = os.getenv("RDS_DB") or database
+        self.database = os.getenv("RDS_DATABASE") or database
         self.user = user or os.getenv("RDS_USERNAME")
         self.password = password or os.getenv("RDS_PASSWORD")
         
         # Checking RDS_HOSTNAME suffix
         if not (self.host.endswith("circ.zone") or self.host.endswith("circlez.ai")):
             print(f"Warning: Your RDS_HOSTNAME={self.host} which is not what is expected")
```

### Comparing `database-without-orm-local-0.0.20/circles_local_database_python/connection_cursor.py` & `database-without-orm-local-0.0.21/circles_local_database_python/connection_cursor.py`

 * *Files identical despite different names*

### Comparing `database-without-orm-local-0.0.20/pyproject.toml` & `database-without-orm-local-0.0.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database-without-orm-local-0.0.20/setup.py` & `database-without-orm-local-0.0.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 # used by python -m build
 setuptools.setup(
     name='database-without-orm-local',
-    version='0.0.20',  # https://pypi.org/project/database-without-orm-local/
+    version='0.0.21',  # https://pypi.org/project/database-without-orm-local/
     author="Circles",
     author_email="info@circles.life",
     description="Circles Local Database without ORM Python PyPI Package",
     long_description="This is a package for sharing common Database methods",
     long_description_content_type="text/markdown",
     url="https://github.com/javatechy/dokr",
     packages=setuptools.find_packages(),
```

