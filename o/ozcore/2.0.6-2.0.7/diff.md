# Comparing `tmp/ozcore-2.0.6.tar.gz` & `tmp/ozcore-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ozcore-2.0.6.tar", max compression
+gzip compressed data, was "ozcore-2.0.7.tar", max compression
```

## Comparing `ozcore-2.0.6.tar` & `ozcore-2.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35149 2023-03-30 03:51:59.899426 ozcore-2.0.6/LICENSE
--rw-r--r--   0        0        0     1756 2023-03-30 03:51:59.899426 ozcore-2.0.6/README.rst
--rw-r--r--   0        0        0      126 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/__init__.py
--rw-r--r--   0        0        0    18664 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/_version.py
--rw-r--r--   0        0        0      533 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/__init__.py
--rw-r--r--   0        0        0      242 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/aggrid/__init__.py
--rw-r--r--   0        0        0     3614 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/aggrid/aggrid.py
--rw-r--r--   0        0        0       54 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/data/__init__.py
--rw-r--r--   0        0        0      102 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/data/csv/__init__.py
--rw-r--r--   0        0        0     4095 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/data/csv/base.py
--rw-r--r--   0        0        0     5065 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/data/csv/process.py
--rw-r--r--   0        0        0      158 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/data/sqlite/__init__.py
--rw-r--r--   0        0        0     8670 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/data/sqlite/orm.py
--rw-r--r--   0        0        0     5897 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/data/sqlite/sqlite.py
--rw-r--r--   0        0        0      712 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/df/__init__.py
--rw-r--r--   0        0        0     7550 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/df/dataframe.py
--rw-r--r--   0        0        0     9551 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/df/dummy.py
--rw-r--r--   0        0        0     1638 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/df/pareto_ranking.py
--rw-r--r--   0        0        0      224 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/path/__init__.py
--rw-r--r--   0        0        0     7310 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/path/folders.py
--rw-r--r--   0        0        0     3318 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/path/tmp_folders.py
--rw-r--r--   0        0        0      580 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/utils/__import_check.py
--rw-r--r--   0        0        0     1041 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/utils/__init__.py
--rw-r--r--   0        0        0     2398 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/utils/helper.py
--rw-r--r--   0        0        0      819 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/utils/html_markdown.py
--rw-r--r--   0        0        0     1791 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/utils/jupyter.py
--rw-r--r--   0        0        0     4124 2023-03-30 03:51:59.903426 ozcore-2.0.6/ozcore/core/utils/zipper.py
--rw-r--r--   0        0        0     2989 2023-03-30 03:53:00.276013 ozcore-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     3914 1970-01-01 00:00:00.000000 ozcore-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-08 13:49:21.364262 ozcore-2.0.7/LICENSE
+-rw-r--r--   0        0        0     1756 2023-08-08 13:49:21.364262 ozcore-2.0.7/README.rst
+-rw-r--r--   0        0        0      126 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/__init__.py
+-rw-r--r--   0        0        0    18664 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/_version.py
+-rw-r--r--   0        0        0      522 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/__init__.py
+-rw-r--r--   0        0        0      242 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/aggrid/__init__.py
+-rw-r--r--   0        0        0     3614 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/aggrid/aggrid.py
+-rw-r--r--   0        0        0       54 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/data/__init__.py
+-rw-r--r--   0        0        0      102 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/data/csv/__init__.py
+-rw-r--r--   0        0        0     4095 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/data/csv/base.py
+-rw-r--r--   0        0        0     5065 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/data/csv/process.py
+-rw-r--r--   0        0        0      158 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/data/sqlite/__init__.py
+-rw-r--r--   0        0        0     8855 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/data/sqlite/orm.py
+-rw-r--r--   0        0        0     5747 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/data/sqlite/sqlite.py
+-rw-r--r--   0        0        0      712 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/df/__init__.py
+-rw-r--r--   0        0        0     7550 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/df/dataframe.py
+-rw-r--r--   0        0        0     9551 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/df/dummy.py
+-rw-r--r--   0        0        0     1638 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/df/pareto_ranking.py
+-rw-r--r--   0        0        0      224 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/path/__init__.py
+-rw-r--r--   0        0        0     7310 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/path/folders.py
+-rw-r--r--   0        0        0     3318 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/path/tmp_folders.py
+-rw-r--r--   0        0        0      580 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/utils/__import_check.py
+-rw-r--r--   0        0        0     1041 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/utils/__init__.py
+-rw-r--r--   0        0        0     2398 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/utils/helper.py
+-rw-r--r--   0        0        0      819 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/utils/html_markdown.py
+-rw-r--r--   0        0        0     1791 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/utils/jupyter.py
+-rw-r--r--   0        0        0     4124 2023-08-08 13:49:21.368263 ozcore-2.0.7/ozcore/core/utils/zipper.py
+-rw-r--r--   0        0        0     2898 2023-08-08 13:50:36.884870 ozcore-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4164 1970-01-01 00:00:00.000000 ozcore-2.0.7/PKG-INFO
```

### Comparing `ozcore-2.0.6/LICENSE` & `ozcore-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/README.rst` & `ozcore-2.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/ozcore/_version.py` & `ozcore-2.0.7/ozcore/_version.py`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/ozcore/core/__init__.py` & `ozcore-2.0.7/ozcore/core/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 note:
     in order not to duplicate variables, some of the modules are called with dunder method 
 
 """
 # check_module
 from .utils import check_modules
 
-# # iöport modules
-from ozcore.core import df, utils, aggrid, path, data
+# # import modules
+from . import df, utils, aggrid, path, data
 
 # path module::Folder
 folder = path.folder
 
 # if aggrid module is available
 try:
     # view - aggric
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ozcore-2.0.6/ozcore/core/aggrid/aggrid.py` & `ozcore-2.0.7/ozcore/core/aggrid/aggrid.py`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/ozcore/core/data/csv/base.py` & `ozcore-2.0.7/ozcore/core/data/csv/base.py`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/ozcore/core/data/csv/process.py` & `ozcore-2.0.7/ozcore/core/data/csv/process.py`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/ozcore/core/data/sqlite/orm.py` & `ozcore-2.0.7/ozcore/core/data/sqlite/orm.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,19 +42,19 @@
             msg = f"{table_name} does not exists in this database!"
             logging.error(msg)
             raise Exception(msg)
         elif self.column_exists(table_name, col):
             msg = f"{col} already exists in {table_name}!"
             logging.error(msg)
             raise Exception(msg)
-        elif not isinstance(type_, sa.sql.visitors.VisitableType):
-            # sa.sql.visitors.VisitableType checks if the type_ argument is an Sqlalchemy type
-            msg = f"{type(type_)} is not an Sqlalchemy type!"
-            logging.error(msg)
-            raise Exception(msg)
+        # elif not isinstance(type_, sa.sql.visitors.Visitable):
+        #     # sa.sql.visitors.VisitableType checks if the type_ argument is an Sqlalchemy type
+        #     msg = f"{type(type_)} is not an Sqlalchemy type!"
+        #     logging.error(msg)
+        #     raise Exception(msg)
 
         with self.engine.connect() as conn:
             ctx = alembic.runtime.migration.MigrationContext.configure(conn)
             op = alembic.operations.Operations(ctx)
             if not isinstance(col, sa.sql.schema.Column):
                 col = sa.Column(col, type_=type_)
             else:
@@ -126,18 +126,18 @@
             raise Exception("No engine found!")
         elif not self.table_exists(table_name):
             logging.error(f"{table_name} does not exists in this database!")
             return False
         elif not self.column_exists(table_name, col):
             logging.error(f"{col} does not exists in {table_name}!")
             return False
-        elif not isinstance(type_, sa.sql.visitors.VisitableType):
-            # sa.sql.visitors.VisitableType checks if the type_ argument is an Sqlalchemy type
-            logging.error(f"{type(type_)} is not an Sqlalchemy type!")
-            return False
+        # elif not isinstance(type_, sa.sql.visitors.Visitable):
+        #     # sa.sql.visitors.VisitableType checks if the type_ argument is an Sqlalchemy type
+        #     logging.error(f"{type(type_)} is not an Sqlalchemy type!")
+        #     return False
 
         with self.engine.connect() as conn:
             ctx = alembic.runtime.migration.MigrationContext.configure(conn)
             op = alembic.operations.Operations(ctx)
             with op.batch_alter_table(table_name) as batch_op:
                 # sqlite has no drop column operation
                 # alembic solves this issue with batch_alter_table
@@ -155,16 +155,17 @@
         """
         if isinstance(table_name, sa.sql.schema.Table):
             table_name = table_name.name
 
         if not self.table_exists(table_name):
             logging.error(f"{table_name} does not exists in this database!")
             return False
-
-        return sa.Table(table_name, self.metadata)
+        metadata = sa.MetaData()
+        metadata.reflect(self.engine)
+        return sa.Table(table_name, metadata)
 
     def sa_column(self, table_name: str, column_name: str):
         """
         Sqalchemy Column object of a given table
 
         parameters:
             table_name: str
@@ -196,17 +197,20 @@
             compare_val: mixed, a value to compare in compare_column
             val: mixed, the new value of the record
         """
 
         tbl = self.sa_table(table_name)
         col = self.sa_column(tbl, column_name)
 
-        tbl.update().where(tbl.c[compare_column] == compare_val).values(
-            {column_name: val}
-        ).execute()
+        with self.engine.connect() as conn:
+            expr = tbl.update().where(tbl.c[compare_column] == compare_val).values(
+                {column_name: val}
+            )
+            conn.execute(expr)
+            conn.commit()
 
     def sa_update_a_column(self, table_name, column_name, compare_column, source_df):
         """
         update a column's records based on a given df_slice
 
         parameters:
             table_name: str or Sqlalchemy Table object
```

### Comparing `ozcore-2.0.6/ozcore/core/data/sqlite/sqlite.py` & `ozcore-2.0.7/ozcore/core/data/sqlite/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,37 +106,27 @@
             engine = self.create_engine(engine)
 
         self.engine = engine
         if return_engine:
             return engine
 
     @property
-    def metadata(self):
-        """
-        returns sqlalchemy metadata of the current engine
-
-        """
-        metadata = sa.MetaData(self.engine)
-        metadata.reflect(self.engine)
-        return metadata
-
-    @property
     def tables(self):
         """
         enum tables in a database
 
         returns:
             a table name from Enum
             also, assigns table names as a list in self.tables_list
 
         usage::
 
             core.sql.tables.table_name
         """
-        tables = self.engine.table_names()
+        tables = sa.inspect(self.engine).get_table_names()
         en = enum.IntEnum("tables", tables)
         self.tables_list = [e.name for e in en]
         return en
 
     def columns(self, table_name):
         """
         enum columns in a table
@@ -149,18 +139,19 @@
             also assigns this query to self.columns_list as a dict
         """
         engine = self.engine
 
         if isinstance(table_name, enum.Enum):
             table_name = table_name.name
 
-        if not engine.has_table(table_name):
+        if not self.table_exists(table_name):
             raise Exception("table name not found in the database!")
-
-        cols = [col for col in sa.Table(table_name, self.metadata).columns]
+        metadata = sa.MetaData()
+        metadata.reflect(engine)
+        cols = [col for col in sa.Table(table_name, metadata).columns]
         names = [e.name for e in cols]
         dic = dict(e for e in zip(names, cols))
 
         en = enum.Enum("columns", dic)
         self.columns_list[table_name] = [e.name for e in en]
         return en
 
@@ -227,15 +218,15 @@
 
         if not isinstance(engine, sa.engine.Engine):
             raise Exception("Engine must be set!")
 
         if isinstance(table_name, enum.Enum):
             table_name = table_name.name
 
-        if not engine.has_table(table_name):
+        if not self.table_exists(table_name):
             raise Exception("table name not found in the database!")
 
         sql = "SELECT * from " + table_name
 
         if isinstance(limit, int):
             sql += " LIMIT " + str(limit)
```

### Comparing `ozcore-2.0.6/ozcore/core/df/__init__.py` & `ozcore-2.0.7/ozcore/core/df/__init__.py`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/ozcore/core/df/dataframe.py` & `ozcore-2.0.7/ozcore/core/df/dataframe.py`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/ozcore/core/df/dummy.py` & `ozcore-2.0.7/ozcore/core/df/dummy.py`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/ozcore/core/df/pareto_ranking.py` & `ozcore-2.0.7/ozcore/core/df/pareto_ranking.py`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/ozcore/core/path/folders.py` & `ozcore-2.0.7/ozcore/core/path/folders.py`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/ozcore/core/path/tmp_folders.py` & `ozcore-2.0.7/ozcore/core/path/tmp_folders.py`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/ozcore/core/utils/__import_check.py` & `ozcore-2.0.7/ozcore/core/utils/__import_check.py`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/ozcore/core/utils/__init__.py` & `ozcore-2.0.7/ozcore/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/ozcore/core/utils/helper.py` & `ozcore-2.0.7/ozcore/core/utils/helper.py`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/ozcore/core/utils/html_markdown.py` & `ozcore-2.0.7/ozcore/core/utils/html_markdown.py`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/ozcore/core/utils/jupyter.py` & `ozcore-2.0.7/ozcore/core/utils/jupyter.py`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/ozcore/core/utils/zipper.py` & `ozcore-2.0.7/ozcore/core/utils/zipper.py`

 * *Files identical despite different names*

### Comparing `ozcore-2.0.6/PKG-INFO` & `ozcore-2.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ozcore
-Version: 2.0.6
+Version: 2.0.7
 Summary: My core.
 Home-page: https://ozcore.readthedocs.io/
 License: GPL-3.0-or-later
 Author: Ozgur Kalan
 Author-email: ozgurkalan@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,35 +13,40 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
-Requires-Dist: alembic (>=1.10.2,<2.0.0)
+Requires-Dist: alembic (>=1.11.2,<2.0.0)
+Requires-Dist: duckdb (>=0.8.1,<0.9.0) ; extra == "all"
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0) ; extra == "all"
-Requires-Dist: faker (>=18.3.1,<19.0.0) ; extra == "all"
+Requires-Dist: faker (>=19.3.0,<20.0.0) ; extra == "all"
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0) ; extra == "all"
 Requires-Dist: html5lib (>=1.1,<2.0) ; extra == "all"
-Requires-Dist: ipyaggrid (>=0.3.2,<0.4.0) ; extra == "all"
+Requires-Dist: ibis-framework (>=6.1.0,<7.0.0) ; extra == "all"
+Requires-Dist: ipyaggrid (>=0.4.1,<0.5.0) ; extra == "all"
 Requires-Dist: ipykernel (>=6.22.0,<7.0.0) ; extra == "all"
-Requires-Dist: ipython (>=8.11.0,<9.0.0) ; extra == "all"
+Requires-Dist: ipython (>=8.14.0,<9.0.0) ; extra == "all"
 Requires-Dist: ipywidgets (>=8.0.6,<9.0.0) ; extra == "all"
+Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: jupyter-contrib-nbextensions (>=0.7.0,<0.8.0) ; extra == "all"
+Requires-Dist: jupyterlab (>=4.0.4,<5.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0) ; extra == "all"
-Requires-Dist: markdown2 (>=2.4.8,<3.0.0) ; extra == "all"
+Requires-Dist: markdown2 (>=2.4.10,<3.0.0) ; extra == "all"
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0) ; extra == "all"
 Requires-Dist: nbformat (>=5.8.0,<6.0.0) ; extra == "all"
-Requires-Dist: notebook (>=6.5.3,<7.0.0) ; extra == "all"
+Requires-Dist: notebook (>=7.0.2,<8.0.0) ; extra == "all"
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0) ; extra == "all"
+Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0) ; extra == "all"
 Requires-Dist: seaborn (>=0.12.2,<0.13.0) ; extra == "all"
-Requires-Dist: sqlalchemy (==1.4.46)
+Requires-Dist: sqlalchemy (>=2.0.19,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0) ; extra == "all"
 Requires-Dist: typeguard (>=3.0.2,<4.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/ozgurkalan/OzCore
 Description-Content-Type: text/x-rst
 
 ======
```

