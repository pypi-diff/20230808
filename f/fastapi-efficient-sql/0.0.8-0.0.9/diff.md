# Comparing `tmp/fastapi-efficient-sql-0.0.8.tar.gz` & `tmp/fastapi_efficient_sql-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fastapi-efficient-sql-0.0.8.tar", last modified: Tue Feb 14 10:01:12 2023, max compression
+gzip compressed data, was "fastapi_efficient_sql-0.0.9.tar", max compression
```

## Comparing `fastapi-efficient-sql-0.0.8.tar` & `fastapi_efficient_sql-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,16 @@
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-02-14 10:01:12.000000 fastapi-efficient-sql-0.0.8/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1064 2022-12-08 03:28:17.000000 fastapi-efficient-sql-0.0.8/LICENSE
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5897 2023-02-14 10:01:12.000000 fastapi-efficient-sql-0.0.8/PKG-INFO
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5374 2023-02-02 03:01:17.000000 fastapi-efficient-sql-0.0.8/README.md
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-02-14 10:01:12.000000 fastapi-efficient-sql-0.0.8/fastapi_efficient_sql.egg-info/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5897 2023-02-14 10:01:12.000000 fastapi-efficient-sql-0.0.8/fastapi_efficient_sql.egg-info/PKG-INFO
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      753 2023-02-14 10:01:12.000000 fastapi-efficient-sql-0.0.8/fastapi_efficient_sql.egg-info/SOURCES.txt
--rw-rw-r--   0 bryan     (1000) bryan     (1000)        1 2023-02-14 10:01:12.000000 fastapi-efficient-sql-0.0.8/fastapi_efficient_sql.egg-info/dependency_links.txt
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       13 2023-02-14 10:01:12.000000 fastapi-efficient-sql-0.0.8/fastapi_efficient_sql.egg-info/requires.txt
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       19 2023-02-14 10:01:12.000000 fastapi-efficient-sql-0.0.8/fastapi_efficient_sql.egg-info/top_level.txt
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-02-14 10:01:12.000000 fastapi-efficient-sql-0.0.8/fastapi_esql/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1373 2023-02-14 09:35:39.000000 fastapi-efficient-sql-0.0.8/fastapi_esql/__init__.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-02-14 10:01:12.000000 fastapi-efficient-sql-0.0.8/fastapi_esql/const/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       52 2022-12-08 03:28:17.000000 fastapi-efficient-sql-0.0.8/fastapi_esql/const/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       86 2022-12-08 03:28:17.000000 fastapi-efficient-sql-0.0.8/fastapi_esql/const/error.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-02-14 10:01:12.000000 fastapi-efficient-sql-0.0.8/fastapi_esql/orm/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      107 2022-12-08 03:28:17.000000 fastapi-efficient-sql-0.0.8/fastapi_esql/orm/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1215 2023-01-18 03:57:26.000000 fastapi-efficient-sql-0.0.8/fastapi_esql/orm/base_app.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4609 2023-02-01 09:23:08.000000 fastapi-efficient-sql-0.0.8/fastapi_esql/orm/base_manager.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      751 2022-12-08 03:28:17.000000 fastapi-efficient-sql-0.0.8/fastapi_esql/orm/base_model.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-02-14 10:01:12.000000 fastapi-efficient-sql-0.0.8/fastapi_esql/utils/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      149 2022-12-08 03:28:17.000000 fastapi-efficient-sql-0.0.8/fastapi_esql/utils/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1165 2023-02-01 12:15:50.000000 fastapi-efficient-sql-0.0.8/fastapi_esql/utils/cursor_handler.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      792 2023-02-02 02:30:32.000000 fastapi-efficient-sql-0.0.8/fastapi_esql/utils/decorator.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      375 2023-01-18 03:58:54.000000 fastapi-efficient-sql-0.0.8/fastapi_esql/utils/metaclass.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    10306 2023-02-14 09:36:32.000000 fastapi-efficient-sql-0.0.8/fastapi_esql/utils/sqlizer.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       38 2023-02-14 10:01:12.000000 fastapi-efficient-sql-0.0.8/setup.cfg
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1269 2022-12-08 03:28:17.000000 fastapi-efficient-sql-0.0.8/setup.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-02-14 10:01:12.000000 fastapi-efficient-sql-0.0.8/tests/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1050 2023-02-01 09:22:05.000000 fastapi-efficient-sql-0.0.8/tests/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1007 2023-02-01 12:35:02.000000 fastapi-efficient-sql-0.0.8/tests/test_cursor_handler.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      413 2023-02-02 02:58:04.000000 fastapi-efficient-sql-0.0.8/tests/test_decorator.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      413 2023-02-01 02:31:29.000000 fastapi-efficient-sql-0.0.8/tests/test_metaclass.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      945 2023-02-03 07:42:44.000000 fastapi-efficient-sql-0.0.8/tests/test_orm.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12657 2023-02-01 12:34:12.000000 fastapi-efficient-sql-0.0.8/tests/test_sqlizer.py
+-rw-r--r--   0        0        0     1069 2023-08-07 14:42:18.384919 fastapi_efficient_sql-0.0.9/LICENSE
+-rw-r--r--   0        0        0     5495 2023-08-08 13:43:13.602061 fastapi_efficient_sql-0.0.9/README.md
+-rw-r--r--   0        0        0     1373 2023-08-08 14:04:43.411967 fastapi_efficient_sql-0.0.9/fastapi_esql/__init__.py
+-rw-r--r--   0        0        0       52 2023-08-04 13:31:04.611216 fastapi_efficient_sql-0.0.9/fastapi_esql/const/__init__.py
+-rw-r--r--   0        0        0       86 2023-08-04 13:31:04.611216 fastapi_efficient_sql-0.0.9/fastapi_esql/const/error.py
+-rw-r--r--   0        0        0      107 2023-08-04 13:31:04.611216 fastapi_efficient_sql-0.0.9/fastapi_esql/orm/__init__.py
+-rw-r--r--   0        0        0     1215 2023-08-04 13:31:04.611216 fastapi_efficient_sql-0.0.9/fastapi_esql/orm/base_app.py
+-rw-r--r--   0        0        0     5393 2023-08-08 13:43:13.602061 fastapi_efficient_sql-0.0.9/fastapi_esql/orm/base_manager.py
+-rw-r--r--   0        0        0      751 2023-08-04 13:31:04.611216 fastapi_efficient_sql-0.0.9/fastapi_esql/orm/base_model.py
+-rw-r--r--   0        0        0      149 2023-08-04 13:31:04.611216 fastapi_efficient_sql-0.0.9/fastapi_esql/utils/__init__.py
+-rw-r--r--   0        0        0     1578 2023-08-08 13:43:13.602061 fastapi_efficient_sql-0.0.9/fastapi_esql/utils/cursor_handler.py
+-rw-r--r--   0        0        0      792 2023-08-04 13:31:04.611216 fastapi_efficient_sql-0.0.9/fastapi_esql/utils/decorator.py
+-rw-r--r--   0        0        0      375 2023-08-04 13:31:04.611216 fastapi_efficient_sql-0.0.9/fastapi_esql/utils/metaclass.py
+-rw-r--r--   0        0        0    10860 2023-08-08 13:43:13.602061 fastapi_efficient_sql-0.0.9/fastapi_esql/utils/sqlizer.py
+-rw-r--r--   0        0        0      680 2023-08-08 14:18:24.591910 fastapi_efficient_sql-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6278 1970-01-01 00:00:00.000000 fastapi_efficient_sql-0.0.9/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fastapi-efficient-sql-0.0.8/LICENSE` & `fastapi_efficient_sql-0.0.9/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 BryanLee
+Copyright (c) 2022-2023 BryanLee
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `fastapi-efficient-sql-0.0.8/PKG-INFO` & `fastapi_efficient_sql-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,14 @@
-Metadata-Version: 2.1
-Name: fastapi-efficient-sql
-Version: 0.0.8
-Summary: Generate bulk DML SQL and execute them based on tortoise-orm and mysql8.0+, and integrated with fastapi.
-Home-page: https://github.com/NightMarcher/fastapi-efficient-sql
-Author: BryanLee
-Author-email: bryanlee@126.com
-License: MIT
-Keywords: sql,fastapi,tortoise-orm,mysql8,bulk-operation
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # fastapi-efficient-sql
 
 Installed as package by `pip install fastapi-efficient-sql`
 
-Install developing requirements by `pipenv install --skip-lock --dev` or `pip install -r requirements-dev.txt`
+Install developing requirements by `pyenv local 3.7.9`, `poetry env use 3.7.9`, `poetry shell` and `pip install -r requirements-dev.txt`
+
+Run demo service by `python -m examples.service`
 
 Run unittest by `pytest -sv`
 
 ## Some preparations before using efficient sql
 ```python
 from fastapi_esql import AppMetaclass, BaseManager, BaseModel
 
@@ -58,21 +46,22 @@
         "extend ->> '$.last_login.start_datetime' start_datetime",
         "CAST(extend ->> '$.last_login.online_sec' AS SIGNED) online_sec"
     ],
     wheres=f"id IN ({','.join(map(str, aids))}) AND gender=1",  # These 4 types of `wheres` are equal
     # wheres=Q(Q(id__in=aids), Q(gender=1), join_type="AND"),
     # wheres={"id__in": aids, "gender": 1},
     # wheres=[Q(id__in=aids), Q(gender=1)],
+    index="PRIMARY",
 )
 ```
 Generate sql and execute
 ```sql
     SELECT
       id, extend ->> '$.last_login.ipv4' ipv4, extend ->> '$.last_login.start_datetime' start_datetime, CAST(extend ->> '$.last_login.online_sec' AS SIGNED) online_sec
-    FROM account
+    FROM account FORCE INDEX (`PRIMARY`)
     WHERE id IN (1,2,3) AND gender=1
 ```
 
 **complex example**
 ```python
 await AccountMgr.select_custom_fields(
     fields=[
```

### Comparing `fastapi-efficient-sql-0.0.8/README.md` & `fastapi_efficient_sql-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,33 @@
+Metadata-Version: 2.1
+Name: fastapi-efficient-sql
+Version: 0.0.9
+Summary: Generate bulk DML SQL and execute them based on Tortoise ORM and mysql8.0+, and integrated with FastAPI.
+Home-page: https://github.com/NightMarcher/fastapi-efficient-sql
+License: MIT
+Keywords: sql,fastapi,tortoise-orm,mysql8,bulk-operation
+Author: BryanLee
+Author-email: bryanlee@126.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
 # fastapi-efficient-sql
 
 Installed as package by `pip install fastapi-efficient-sql`
 
-Install developing requirements by `pipenv install --skip-lock --dev` or `pip install -r requirements-dev.txt`
+Install developing requirements by `pyenv local 3.7.9`, `poetry env use 3.7.9`, `poetry shell` and `pip install -r requirements-dev.txt`
+
+Run demo service by `python -m examples.service`
 
 Run unittest by `pytest -sv`
 
 ## Some preparations before using efficient sql
 ```python
 from fastapi_esql import AppMetaclass, BaseManager, BaseModel
 
@@ -44,21 +65,22 @@
         "extend ->> '$.last_login.start_datetime' start_datetime",
         "CAST(extend ->> '$.last_login.online_sec' AS SIGNED) online_sec"
     ],
     wheres=f"id IN ({','.join(map(str, aids))}) AND gender=1",  # These 4 types of `wheres` are equal
     # wheres=Q(Q(id__in=aids), Q(gender=1), join_type="AND"),
     # wheres={"id__in": aids, "gender": 1},
     # wheres=[Q(id__in=aids), Q(gender=1)],
+    index="PRIMARY",
 )
 ```
 Generate sql and execute
 ```sql
     SELECT
       id, extend ->> '$.last_login.ipv4' ipv4, extend ->> '$.last_login.start_datetime' start_datetime, CAST(extend ->> '$.last_login.online_sec' AS SIGNED) online_sec
-    FROM account
+    FROM account FORCE INDEX (`PRIMARY`)
     WHERE id IN (1,2,3) AND gender=1
 ```
 
 **complex example**
 ```python
 await AccountMgr.select_custom_fields(
     fields=[
@@ -179,7 +201,8 @@
           VALUES
           ROW(7, False, 1),
           ROW(15, True, 0)
         ) AS fly_table (id, active, gender)
     ) tmp ON account.id=tmp.id
     SET account.active=tmp.active, account.gender=tmp.gender
 ```
+
```

### Comparing `fastapi-efficient-sql-0.0.8/fastapi_esql/__init__.py` & `fastapi_efficient_sql-0.0.9/fastapi_esql/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Cases,
     RawSQL,
     SQLizer,
     Singleton,
     timing,
 )
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 __all__ = [
     "QsParsingError",
     "WrongParamsError",
     "AppMetaclass",
     "BaseManager",
     "BaseModel",
```

### Comparing `fastapi-efficient-sql-0.0.8/fastapi_esql/orm/base_app.py` & `fastapi_efficient_sql-0.0.9/fastapi_esql/orm/base_app.py`

 * *Files identical despite different names*

### Comparing `fastapi-efficient-sql-0.0.8/fastapi_esql/orm/base_manager.py` & `fastapi_efficient_sql-0.0.9/fastapi_esql/orm/base_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -59,36 +59,64 @@
             return False
 
     @classmethod
     async def select_custom_fields(
         cls,
         fields: List[str],
         wheres: Union[str, Q, Dict[str, Any], List[Q]],
+        index: Optional[str] = None,
         groups: Optional[List[str]] = None,
         having: Optional[str] = None,
         orders: Optional[List[str]] = None,
         offset: Optional[int] = None,
-        limit: int = 0,
+        limit: Optional[int] = None,
         conn: Optional[BaseDBAsyncClient] = None,
     ):
         sql = SQLizer.select_custom_fields(
             cls.table,
             fields,
             wheres,
+            index,
             groups,
             having,
             orders,
             offset,
             limit,
             cls.model,
         )
         conn = conn or cls.ro_conn
         return await CursorHandler.fetch_dicts(sql, conn, logger)
 
     @classmethod
+    async def select_one_record(
+        cls,
+        fields: List[str],
+        wheres: Union[str, Q, Dict[str, Any], List[Q]],
+        index: Optional[str] = None,
+        groups: Optional[List[str]] = None,
+        having: Optional[str] = None,
+        orders: Optional[List[str]] = None,
+        conn: Optional[BaseDBAsyncClient] = None,
+    ):
+        sql = SQLizer.select_custom_fields(
+            cls.table,
+            fields,
+            wheres,
+            index,
+            groups,
+            having,
+            orders,
+            0,
+            1,
+            cls.model,
+        )
+        conn = conn or cls.ro_conn
+        return await CursorHandler.fetch_one(sql, conn, logger)
+
+    @classmethod
     async def update_json_field(
         cls,
         json_field: str,
         wheres: Union[str, Q, Dict[str, Any], List[Q]],
         merge_dict: Optional[Dict[str, Any]] = None,
         path_value_dict: Optional[Dict[str, Any]] = None,
         remove_paths: Optional[List[str]] = None,
```

### Comparing `fastapi-efficient-sql-0.0.8/fastapi_esql/orm/base_model.py` & `fastapi_efficient_sql-0.0.9/fastapi_esql/orm/base_model.py`

 * *Files identical despite different names*

### Comparing `fastapi-efficient-sql-0.0.8/fastapi_esql/utils/cursor_handler.py` & `fastapi_efficient_sql-0.0.9/fastapi_esql/utils/cursor_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,30 @@
         try:
             return await conn.execute_query_dict(sql)
         except Exception as e:
             logger.exception(f"{e} SQL=>{sql}")
             return None
 
     @classmethod
+    async def fetch_one(
+        cls,
+        sql: str,
+        conn: BaseDBAsyncClient,
+        logger: Logger,
+    ) -> Optional[Dict[str, Any]]:
+        try:
+            dicts = await conn.execute_query_dict(sql)
+            if dicts:
+                return dicts[0]
+            return {}
+        except Exception as e:
+            logger.exception(f"{e} SQL=>{sql}")
+            return None
+
+    @classmethod
     async def sum_row_cnt(
         cls,
         sql: str,
         conn: BaseDBAsyncClient,
         logger: Logger,
     ) -> Optional[int]:
         try:
```

### Comparing `fastapi-efficient-sql-0.0.8/fastapi_esql/utils/decorator.py` & `fastapi_efficient_sql-0.0.9/fastapi_esql/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `fastapi-efficient-sql-0.0.8/fastapi_esql/utils/sqlizer.py` & `fastapi_efficient_sql-0.0.9/fastapi_esql/utils/sqlizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,29 +46,29 @@
     @classmethod
     def resolve_wheres(
         cls,
         wheres: Union[str, Q, Dict[str, Any], List[Q]],
         model: Optional[Model] = None,
     ) -> str:
         if not model and not isinstance(wheres, str):
-            raise WrongParamsError("Parameter `wheres` only support str type if no model passed")
+            raise WrongParamsError("Parameter `wheres` only supports str if no model exists")
 
         if isinstance(wheres, str):
             return wheres
         elif isinstance(wheres, Q):
             qs = [wheres]
         elif isinstance(wheres, dict):
             qs = [Q(**{key: value}) for (key, value) in wheres.items()]
         elif isinstance(wheres, list):
             qs = [q for q in wheres if isinstance(q, Q)]
         else:
-            raise WrongParamsError("Parameter `wheres` only supports str, dict and list type")
+            raise WrongParamsError("Parameter `wheres` only support str, Q, Dict[str, Any] and List[Q]")
 
         if not qs:
-            raise QsParsingError("Parsing `wheres` for qs failed!")
+            raise QsParsingError("Parsing `wheres` for QuerySet failed")
 
         modifier = QueryModifier()
         for q in qs:
             # NOTE Method `Q.resolve` changed since version 0.18.0
             # https://github.com/tortoise/tortoise-orm/commit/37178e175bc12bc4767b93142dab0209f9240c55
             if tortoise_version >= "0.18.0":
                 modifier &= q.resolve(model, model._meta.basetable)
@@ -110,41 +110,43 @@
 
     @classmethod
     def select_custom_fields(
         cls,
         table: str,
         fields: List[str],
         wheres: Union[str, Q, Dict[str, Any], List[Q]],
+        index: Optional[str] = None,
         groups: Optional[List[str]] = None,
         having: Optional[str] = None,
         orders: Optional[List[str]] = None,
         offset: Optional[int] = None,
-        limit: int = 0,
+        limit: Optional[int] = None,
         model: Optional[Model] = None,
     ) -> Optional[str]:
         if not all([table, fields, wheres]):
-            raise WrongParamsError("Please check your params")
+            raise WrongParamsError("Parameters `table`, `fields`, `wheres` are required")
         if having and not groups:
-            raise WrongParamsError("Parameter `groups` shoud be no empty when `having` isn't")
+            raise WrongParamsError("Parameter `groups` shoud not be empty if `having` exists")
 
         group_by = f"    GROUP BY {', '.join(groups)}" if groups else ""
         having_ = f"    HAVING {having}" if having else ""
         order_by = f"    ORDER BY {cls.resolve_orders(orders)}" if orders else ""
         offset_ = "" if offset is None else f"{offset}, "
         limit_ = f"    LIMIT {offset_}{limit}" if limit else ""
         extras = [group_by, having_, order_by, limit_]
 
         sql = """
     SELECT
       {}
-    FROM {}
+    FROM {}{}
     WHERE {}
 {}""".format(
         ", ".join(fields),
         table,
+        f" FORCE INDEX (`{index}`)" if index else "",
         cls.resolve_wheres(wheres, model),
         "\n".join(i for i in extras if i),
     )
         logger.debug(sql)
         return sql
 
     @classmethod
@@ -156,17 +158,19 @@
         merge_dict: Optional[Dict[str, Any]] = None,
         path_value_dict: Optional[Dict[str, Any]] = None,
         remove_paths: Optional[List[str]] = None,
         json_type: type = dict,
         model: Optional[Model] = None,
     ) -> Optional[str]:
         if not all([table, json_field, wheres]):
-            raise WrongParamsError("Please check your params")
+            raise WrongParamsError("Parameters `table`, `json_field`, `wheres` are required")
         if not any([merge_dict, path_value_dict, remove_paths]):
-            raise WrongParamsError("Please check your params")
+            raise WrongParamsError(
+                "At least one no empty parameter is required between `merge_dict`, `path_value_dict` and `remove_paths`"
+            )
 
         json_obj = f"COALESCE({json_field}, '{json_type()}')"
         if remove_paths:
             rps = ", ".join(f"'{p}'" for p in remove_paths)
             json_obj = f"JSON_REMOVE({json_obj}, {rps})"
         if path_value_dict:
             pvs = [
@@ -191,15 +195,15 @@
         table: str,
         dicts: List[Dict[str, Any]],
         insert_fields: List[str],
         upsert_fields: List[str],
         using_values: bool = False,
     ) -> Optional[str]:
         if not all([table, dicts, insert_fields, upsert_fields]):
-            raise WrongParamsError("Please check your params")
+            raise WrongParamsError("Parameters `table`, `dicts`, `insert_fields`, `upsert_fields` are required")
 
         values = [
             f"      ({', '.join(cls.sqlize_value(d.get(f)) for f in insert_fields)})"
             for d in dicts
         ]
         # NOTE Beginning with MySQL 8.0.19, it is possible to use an alias for the row
         # https://dev.mysql.com/doc/refman/8.0/en/insert-on-duplicate.html
@@ -232,16 +236,18 @@
         table: str,
         wheres: Union[str, Q, Dict[str, Any], List[Q]],
         remain_fields: List[str],
         assign_field_dict: Dict[str, Any],
         to_table: Optional[str] = None,
         model: Optional[Model] = None,
     ) -> Optional[str]:
-        if not all([table, wheres] or not any([remain_fields, assign_field_dict])):
-            raise WrongParamsError("Please check your params")
+        if not all([table, wheres]):
+            raise WrongParamsError("Parameters `table`, `wheres` are required")
+        if not any([remain_fields, assign_field_dict]):
+            raise WrongParamsError("At least one no empty parameter is required between `remain_fields` and `assign_field_dict`")
 
         fields = [*remain_fields]
         assign_fields = []
         for k, v in assign_field_dict.items():
             fields.append(k)
             assign_fields.append(f"{cls.sqlize_value(v)} {k}")
 
@@ -259,15 +265,15 @@
     def build_fly_table(
         cls,
         dicts: List[Dict[str, Any]],
         fields: List[str],
         using_values: bool = True,
     ) -> Optional[str]:
         if not all([dicts, fields]):
-            raise WrongParamsError("Please check your params")
+            raise WrongParamsError("Parameters `dicts`, `fields` are required")
 
         if using_values:
             rows = [
                 f"          ROW({', '.join(cls.sqlize_value(d.get(f)) for f in fields)})"
                 for d in dicts
             ]
             values = "VALUES\n" + ",\n".join(rows)
@@ -293,15 +299,15 @@
         table: str,
         dicts: List[Dict[str, Any]],
         join_fields: List[str],
         update_fields: List[str],
         using_values: bool = True,
     ) -> Optional[str]:
         if not all([table, dicts, join_fields, update_fields]):
-            raise WrongParamsError("Please check your params")
+            raise WrongParamsError("Parameters `table`, `dicts`, `join_fields`, `update_fields` are required")
 
         joins = [f"{table}.{jf}=tmp.{jf}" for jf in join_fields]
         updates = [f"{table}.{uf}=tmp.{uf}" for uf in update_fields]
 
         sql = f"""
     UPDATE {table}
     JOIN ({SQLizer.build_fly_table(dicts, join_fields + update_fields, using_values)}
```

