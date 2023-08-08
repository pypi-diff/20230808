# Comparing `tmp/pyeasysql-3.2.4.tar.gz` & `tmp/pyeasysql-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeasysql-3.2.4.tar", last modified: Wed Aug  2 12:11:14 2023, max compression
+gzip compressed data, was "pyeasysql-3.2.5.tar", last modified: Tue Aug  8 13:32:17 2023, max compression
```

## Comparing `pyeasysql-3.2.4.tar` & `pyeasysql-3.2.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 12:11:14.582393 pyeasysql-3.2.4/
-drwxrwxrwx   0        0        0        0 2023-08-02 12:11:14.565863 pyeasysql-3.2.4/EasySQL/
--rw-rw-rw-   0        0        0     3662 2023-07-24 11:39:55.000000 pyeasysql-3.2.4/EasySQL/ABC.py
--rw-rw-rw-   0        0        0     2887 2021-06-27 12:24:21.000000 pyeasysql-3.2.4/EasySQL/Characters.py
--rw-rw-rw-   0        0        0    15360 2023-07-28 07:59:44.000000 pyeasysql-3.2.4/EasySQL/Classes.py
--rw-rw-rw-   0        0        0     6202 2023-08-02 12:10:47.000000 pyeasysql-3.2.4/EasySQL/Commands.py
--rw-rw-rw-   0        0        0      945 2023-07-25 08:49:05.000000 pyeasysql-3.2.4/EasySQL/Constraints.py
--rw-rw-rw-   0        0        0      305 2023-07-11 12:44:34.000000 pyeasysql-3.2.4/EasySQL/Decorators.py
--rw-rw-rw-   0        0        0     2097 2023-07-09 09:35:55.000000 pyeasysql-3.2.4/EasySQL/EasyInstances.py
--rw-rw-rw-   0        0        0      757 2023-06-08 19:41:42.000000 pyeasysql-3.2.4/EasySQL/Exceptions.py
--rw-rw-rw-   0        0        0      457 2021-04-04 16:17:30.000000 pyeasysql-3.2.4/EasySQL/Logging.py
--rw-rw-rw-   0        0        0     3081 2023-08-02 12:00:29.000000 pyeasysql-3.2.4/EasySQL/Types.py
--rw-rw-rw-   0        0        0     2496 2022-04-15 06:15:51.000000 pyeasysql-3.2.4/EasySQL/Where.py
--rw-rw-rw-   0        0        0      298 2023-07-24 15:21:11.000000 pyeasysql-3.2.4/EasySQL/__init__.py
--rw-rw-rw-   0        0        0     1085 2023-07-23 15:33:54.000000 pyeasysql-3.2.4/LICENSE.md
--rw-rw-rw-   0        0        0     6084 2023-08-02 12:11:14.581381 pyeasysql-3.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     5412 2023-07-24 15:30:12.000000 pyeasysql-3.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 12:11:14.577953 pyeasysql-3.2.4/pyeasysql.egg-info/
--rw-rw-rw-   0        0        0     6084 2023-08-02 12:11:14.000000 pyeasysql-3.2.4/pyeasysql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-08-02 12:11:14.000000 pyeasysql-3.2.4/pyeasysql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 12:11:14.000000 pyeasysql-3.2.4/pyeasysql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-02 12:11:14.000000 pyeasysql-3.2.4/pyeasysql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 12:11:14.000000 pyeasysql-3.2.4/pyeasysql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      717 2023-08-02 12:11:01.000000 pyeasysql-3.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-02 12:11:14.582393 pyeasysql-3.2.4/setup.cfg
--rw-rw-rw-   0        0        0      831 2023-07-24 16:25:04.000000 pyeasysql-3.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 13:32:17.034457 pyeasysql-3.2.5/
+drwxrwxrwx   0        0        0        0 2023-08-08 13:32:17.013654 pyeasysql-3.2.5/EasySQL/
+-rw-rw-rw-   0        0        0     3662 2023-07-24 11:39:55.000000 pyeasysql-3.2.5/EasySQL/ABC.py
+-rw-rw-rw-   0        0        0     2887 2021-06-27 12:24:21.000000 pyeasysql-3.2.5/EasySQL/Characters.py
+-rw-rw-rw-   0        0        0    15476 2023-08-08 13:15:52.000000 pyeasysql-3.2.5/EasySQL/Classes.py
+-rw-rw-rw-   0        0        0     6202 2023-08-02 12:10:47.000000 pyeasysql-3.2.5/EasySQL/Commands.py
+-rw-rw-rw-   0        0        0      945 2023-07-25 08:49:05.000000 pyeasysql-3.2.5/EasySQL/Constraints.py
+-rw-rw-rw-   0        0        0      305 2023-07-11 12:44:34.000000 pyeasysql-3.2.5/EasySQL/Decorators.py
+-rw-rw-rw-   0        0        0     2097 2023-07-09 09:35:55.000000 pyeasysql-3.2.5/EasySQL/EasyInstances.py
+-rw-rw-rw-   0        0        0      757 2023-06-08 19:41:42.000000 pyeasysql-3.2.5/EasySQL/Exceptions.py
+-rw-rw-rw-   0        0        0     1063 2023-08-08 13:31:59.000000 pyeasysql-3.2.5/EasySQL/Logging.py
+-rw-rw-rw-   0        0        0     3081 2023-08-02 12:00:29.000000 pyeasysql-3.2.5/EasySQL/Types.py
+-rw-rw-rw-   0        0        0     2496 2022-04-15 06:15:51.000000 pyeasysql-3.2.5/EasySQL/Where.py
+-rw-rw-rw-   0        0        0      298 2023-07-24 15:21:11.000000 pyeasysql-3.2.5/EasySQL/__init__.py
+-rw-rw-rw-   0        0        0     1085 2023-07-23 15:33:54.000000 pyeasysql-3.2.5/LICENSE.md
+-rw-rw-rw-   0        0        0     6103 2023-08-08 13:32:17.033458 pyeasysql-3.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5431 2023-08-07 11:41:17.000000 pyeasysql-3.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 13:32:17.030167 pyeasysql-3.2.5/pyeasysql.egg-info/
+-rw-rw-rw-   0        0        0     6103 2023-08-08 13:32:16.000000 pyeasysql-3.2.5/pyeasysql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-08-08 13:32:16.000000 pyeasysql-3.2.5/pyeasysql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 13:32:16.000000 pyeasysql-3.2.5/pyeasysql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-08 13:32:16.000000 pyeasysql-3.2.5/pyeasysql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-08 13:32:16.000000 pyeasysql-3.2.5/pyeasysql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      717 2023-08-08 13:15:52.000000 pyeasysql-3.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 13:32:17.035467 pyeasysql-3.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      831 2023-07-24 16:25:04.000000 pyeasysql-3.2.5/setup.py
```

### Comparing `pyeasysql-3.2.4/EasySQL/ABC.py` & `pyeasysql-3.2.5/EasySQL/ABC.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.4/EasySQL/Characters.py` & `pyeasysql-3.2.5/EasySQL/Characters.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.4/EasySQL/Classes.py` & `pyeasysql-3.2.5/EasySQL/Classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from itertools import zip_longest
 from time import sleep
 from typing import Optional, Union, Any, Sequence, TypeVar, Tuple, List
 
 import mysql.connector
-from deprecated.classic import deprecated
 
 from .ABC import SQLType, CHARSET, SQLConstraints
+from .Constraints import NOT_NULL, Unique, UNIQUE, PRIMARY
 from .Exceptions import DatabaseConnectionException
 from .Logging import logger
-from .Constraints import NOT_NULL, Unique, UNIQUE, PRIMARY
 from .Where import Where
 
 __all__ = ['EasyDatabase', 'EasyTable', 'EasyColumn', 'EasyForeignColumn']
 
 
 def _safe_pop(d: dict, k):
     try:
@@ -84,21 +83,22 @@
         if not isinstance(column.table, EasyTable):
             return TypeError('Version 3: To use this method, The table of column must be set')
 
         tags = (NOT_NULL, ) if NOT_NULL in tags else ()
         name = f'{column.name} of {column.table.name}' if name is None else name
         return EasyForeignColumn(name, column.table, column, *tags, default=default)
 
-    def __init__(self, name: str, table: 'EasyTable', reference: Union[EasyColumn, str], *tags: SQLConstraints, default: Any = None):
+    def __init__(self, name: str, table: 'EasyTable', reference: Union[EasyColumn, str], *tags: SQLConstraints, default: Any = None, cascade: bool = True):
         column = table.get_column(reference)
         if column is None:
             raise ValueError(f'Unable to find `{reference}` in the table')
 
         self.refer_table = table
         self.refer_column = column
+        self.cascade = cascade
 
         tags = (NOT_NULL,) if NOT_NULL in tags else ()
         super().__init__(name, column.sql_type, *tags, default=default)
 
     def __repr__(self):
         return f'<EasyForeignColumn "{self.name}" reference={self.refer_table.name}({self.refer_column.name})>'
 
@@ -308,14 +308,16 @@
                 command = ', '.join([column.get_sql() for column in self._columns])
                 if len(self.PRIMARY) > 0:
                     command += f", PRIMARY KEY({', '.join(column.name for column in self.PRIMARY)})"
 
                 for column in self._columns:
                     if isinstance(column, EasyForeignColumn):
                         command += f", FOREIGN KEY ({column.name}) REFERENCES {column.refer_table.name}({column.refer_column.name})"
+                        if column.cascade:
+                            command += " ON DELETE CASCADE"
 
                 for unique in self.UNIQUES:
                     command += f", {unique.value}"
 
                 command = f"CREATE TABLE {self._name} ({command});"
                 self._database.execute(command)
             else:
```

### Comparing `pyeasysql-3.2.4/EasySQL/Commands.py` & `pyeasysql-3.2.5/EasySQL/Commands.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.4/EasySQL/Constraints.py` & `pyeasysql-3.2.5/EasySQL/Constraints.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.4/EasySQL/EasyInstances.py` & `pyeasysql-3.2.5/EasySQL/EasyInstances.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.4/EasySQL/Exceptions.py` & `pyeasysql-3.2.5/EasySQL/Exceptions.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.4/EasySQL/Types.py` & `pyeasysql-3.2.5/EasySQL/Types.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.4/EasySQL/Where.py` & `pyeasysql-3.2.5/EasySQL/Where.py`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.4/LICENSE.md` & `pyeasysql-3.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyeasysql-3.2.4/PKG-INFO` & `pyeasysql-3.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeasysql
-Version: 3.2.4
+Version: 3.2.5
 Summary: SQL Database management without even a SQL line
 Home-page: https://github.com/AGM-Studio/easysql
 Author: Ashenguard
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/easysql
 Project-URL: Bug Tracker, https://github.com/agm-studio/easysql/issues
 Classifier: Programming Language :: Python :: 3
@@ -115,15 +115,15 @@
 # MyTable.delete() -> raise EasySQL.DatabaseSafetyException
 # Turn the safety off with following command.
 MyDatabase.remove_safety(confirm=True)
 # Now there will be no error, it will clean the all data that's why we had safety lock
 MyTable.delete()
 ```
 
-[![AdFoc.us Banner](https://adfoc.us/images/banners/728x90-2.gif)](https://adfoc.us/?refid=497244)
+[![Advertisement Banner](https://2captcha.com/referral-banners/2captcha/08.gif)](https://2captcha.com/?from=19092307)
 
 ## Extras & Features
 1. Need unsigned types? EasySQL has them.
 > `BIGINT.UNSIGNED`, `INT.UNSIGNED`, `MEDIUMINT.UNSIGNED`, `SMALLINT.UNSIGNED`
 2. Afraid of unsigned or signed values? EasySQL will check them for you!
 > Raises `ValueError` if you are out of bound
 3. Multiple primary keys? EasySQL will take care of it.
```

### Comparing `pyeasysql-3.2.4/README.md` & `pyeasysql-3.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 # MyTable.delete() -> raise EasySQL.DatabaseSafetyException
 # Turn the safety off with following command.
 MyDatabase.remove_safety(confirm=True)
 # Now there will be no error, it will clean the all data that's why we had safety lock
 MyTable.delete()
 ```
 
-[![AdFoc.us Banner](https://adfoc.us/images/banners/728x90-2.gif)](https://adfoc.us/?refid=497244)
+[![Advertisement Banner](https://2captcha.com/referral-banners/2captcha/08.gif)](https://2captcha.com/?from=19092307)
 
 ## Extras & Features
 1. Need unsigned types? EasySQL has them.
 > `BIGINT.UNSIGNED`, `INT.UNSIGNED`, `MEDIUMINT.UNSIGNED`, `SMALLINT.UNSIGNED`
 2. Afraid of unsigned or signed values? EasySQL will check them for you!
 > Raises `ValueError` if you are out of bound
 3. Multiple primary keys? EasySQL will take care of it.
```

### Comparing `pyeasysql-3.2.4/pyeasysql.egg-info/PKG-INFO` & `pyeasysql-3.2.5/pyeasysql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeasysql
-Version: 3.2.4
+Version: 3.2.5
 Summary: SQL Database management without even a SQL line
 Home-page: https://github.com/AGM-Studio/easysql
 Author: Ashenguard
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/easysql
 Project-URL: Bug Tracker, https://github.com/agm-studio/easysql/issues
 Classifier: Programming Language :: Python :: 3
@@ -115,15 +115,15 @@
 # MyTable.delete() -> raise EasySQL.DatabaseSafetyException
 # Turn the safety off with following command.
 MyDatabase.remove_safety(confirm=True)
 # Now there will be no error, it will clean the all data that's why we had safety lock
 MyTable.delete()
 ```
 
-[![AdFoc.us Banner](https://adfoc.us/images/banners/728x90-2.gif)](https://adfoc.us/?refid=497244)
+[![Advertisement Banner](https://2captcha.com/referral-banners/2captcha/08.gif)](https://2captcha.com/?from=19092307)
 
 ## Extras & Features
 1. Need unsigned types? EasySQL has them.
 > `BIGINT.UNSIGNED`, `INT.UNSIGNED`, `MEDIUMINT.UNSIGNED`, `SMALLINT.UNSIGNED`
 2. Afraid of unsigned or signed values? EasySQL will check them for you!
 > Raises `ValueError` if you are out of bound
 3. Multiple primary keys? EasySQL will take care of it.
```

### Comparing `pyeasysql-3.2.4/pyproject.toml` & `pyeasysql-3.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyeasysql"
-version = "3.2.4"
+version = "3.2.5"
 authors = [
   { name="Ashenguard", email="ashenguard@agmstudio.xyz" },
 ]
 description = "SQL Database management without even a SQL line"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `pyeasysql-3.2.4/setup.py` & `pyeasysql-3.2.5/setup.py`

 * *Files identical despite different names*

