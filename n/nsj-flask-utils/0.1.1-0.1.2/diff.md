# Comparing `tmp/nsj_flask_utils-0.1.1.tar.gz` & `tmp/nsj_flask_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_flask_utils-0.1.1.tar", max compression
+gzip compressed data, was "nsj_flask_utils-0.1.2.tar", max compression
```

## Comparing `nsj_flask_utils-0.1.1.tar` & `nsj_flask_utils-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       72 2023-08-04 20:16:13.230462 nsj_flask_utils-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-08-04 19:16:54.719394 nsj_flask_utils-0.1.1/nsj_flask_utils/__init__.py
--rw-r--r--   0        0        0       53 2023-08-04 20:08:10.746192 nsj_flask_utils-0.1.1/nsj_flask_utils/daos/__init__.py
--rw-r--r--   0        0        0     3153 2023-08-04 19:58:22.274631 nsj_flask_utils-0.1.1/nsj_flask_utils/daos/base_dao.py
--rw-r--r--   0        0        0       53 2023-08-04 20:08:26.739234 nsj_flask_utils-0.1.1/nsj_flask_utils/dtos/__init__.py
--rw-r--r--   0        0        0      212 2023-08-04 18:49:58.954112 nsj_flask_utils-0.1.1/nsj_flask_utils/dtos/base_dto.py
--rw-r--r--   0        0        0      629 2023-08-04 19:15:17.291078 nsj_flask_utils-0.1.1/nsj_flask_utils/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 19:42:03.906006 nsj_flask_utils-0.1.1/nsj_flask_utils/py.typed
--rw-r--r--   0        0        0        0 2023-08-04 18:34:53.078783 nsj_flask_utils-0.1.1/nsj_flask_utils/service/__init__.py
--rw-r--r--   0        0        0     3077 2023-08-04 20:14:05.516126 nsj_flask_utils-0.1.1/nsj_flask_utils/service/base_service.py
--rw-r--r--   0        0        0      212 2023-08-04 20:01:49.619187 nsj_flask_utils-0.1.1/nsj_flask_utils/utils/__init__.py
--rw-r--r--   0        0        0     1059 2023-08-04 19:16:06.086236 nsj_flask_utils-0.1.1/nsj_flask_utils/utils/error_handlers.py
--rw-r--r--   0        0        0      147 2023-07-06 20:22:50.549765 nsj_flask_utils-0.1.1/nsj_flask_utils/utils/filter_params.py
--rw-r--r--   0        0        0      434 2023-08-04 19:57:27.085483 nsj_flask_utils-0.1.1/nsj_flask_utils/utils/json.py
--rw-r--r--   0        0        0     1051 2023-08-04 19:04:40.476273 nsj_flask_utils-0.1.1/nsj_flask_utils/utils/pagination_params.py
--rw-r--r--   0        0        0     2953 2023-08-04 19:59:57.791888 nsj_flask_utils-0.1.1/nsj_flask_utils/utils/request_args.py
--rw-r--r--   0        0        0      508 2023-08-07 19:43:59.133159 nsj_flask_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 nsj_flask_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-08-04 20:16:13.230462 nsj_flask_utils-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-08-04 19:16:54.719394 nsj_flask_utils-0.1.2/nsj_flask_utils/__init__.py
+-rw-r--r--   0        0        0       53 2023-08-04 20:08:10.746192 nsj_flask_utils-0.1.2/nsj_flask_utils/daos/__init__.py
+-rw-r--r--   0        0        0     4238 2023-08-08 12:45:07.643448 nsj_flask_utils-0.1.2/nsj_flask_utils/daos/base_dao.py
+-rw-r--r--   0        0        0       53 2023-08-04 20:08:26.739234 nsj_flask_utils-0.1.2/nsj_flask_utils/dtos/__init__.py
+-rw-r--r--   0        0        0      233 2023-08-08 12:49:50.743121 nsj_flask_utils-0.1.2/nsj_flask_utils/dtos/base_dto.py
+-rw-r--r--   0        0        0      629 2023-08-04 19:15:17.291078 nsj_flask_utils-0.1.2/nsj_flask_utils/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 19:42:03.906006 nsj_flask_utils-0.1.2/nsj_flask_utils/py.typed
+-rw-r--r--   0        0        0        0 2023-08-04 18:34:53.078783 nsj_flask_utils-0.1.2/nsj_flask_utils/service/__init__.py
+-rw-r--r--   0        0        0     3153 2023-08-08 12:48:48.643974 nsj_flask_utils-0.1.2/nsj_flask_utils/service/base_service.py
+-rw-r--r--   0        0        0      212 2023-08-04 20:01:49.619187 nsj_flask_utils-0.1.2/nsj_flask_utils/utils/__init__.py
+-rw-r--r--   0        0        0     1059 2023-08-04 19:16:06.086236 nsj_flask_utils-0.1.2/nsj_flask_utils/utils/error_handlers.py
+-rw-r--r--   0        0        0      147 2023-07-06 20:22:50.549765 nsj_flask_utils-0.1.2/nsj_flask_utils/utils/filter_params.py
+-rw-r--r--   0        0        0      434 2023-08-04 19:57:27.085483 nsj_flask_utils-0.1.2/nsj_flask_utils/utils/json.py
+-rw-r--r--   0        0        0     1051 2023-08-04 19:04:40.476273 nsj_flask_utils-0.1.2/nsj_flask_utils/utils/pagination_params.py
+-rw-r--r--   0        0        0     3155 2023-08-08 12:43:29.667218 nsj_flask_utils-0.1.2/nsj_flask_utils/utils/request_args.py
+-rw-r--r--   0        0        0      508 2023-08-08 12:51:32.553362 nsj_flask_utils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 nsj_flask_utils-0.1.2/PKG-INFO
```

### Comparing `nsj_flask_utils-0.1.1/nsj_flask_utils/exceptions/__init__.py` & `nsj_flask_utils-0.1.2/nsj_flask_utils/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_utils-0.1.1/nsj_flask_utils/service/base_service.py` & `nsj_flask_utils-0.1.2/nsj_flask_utils/service/base_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from nsj_flask_utils.utils import RequestArgs
 from nsj_flask_utils.daos  import BaseDAO
 from nsj_flask_utils.dtos  import BaseDTO
 
 TDTO = TypeVar('TDTO', bound=BaseDTO)
 TDAO = TypeVar('TDAO', bound=BaseDAO)
 
+
 class BaseService(Generic[TDAO, TDTO]):
     _dao_cls: type[TDAO]
     _dto_cls: type[TDTO]
 
     _dao: TDAO
     _dto: type[TDTO]
 
@@ -33,67 +34,69 @@
         elif self._dto_cls:
             self._dto = self._dto_cls
         else:
             raise Exception('DTO not defined')
         pass
 
     def list(self, req_args: RequestArgs) -> list[TDTO]:
-        filter_params = req_args.get_filter_params()
-        pagination_params = req_args.get_pagination_params()
-        rs: list[TDTO] = self._dao.list(pagination_params, filter_params)
-        return rs
+        return self._dao.list(req_args)
 
     def create(self, dto: TDTO) -> TDTO:
         return self._dao.create(dto)
 
-    def get(self, id: Any) -> TDTO:
+    def get_or_none(self, id: Any) -> TDTO | None:
+        return self._dao.get(id)
+
+    def get_or_raise(self, id: Any
+                         , exception: type[Exception] = NotFound) -> TDTO:
         rs = self._dao.get(id)
         if not rs:
-            raise NotFound("Not found")
+            raise exception("Not found")
         return rs
 
     def update(self, id: Any, dto: TDTO) -> TDTO:
-        original = self.get(id)
+        original = self.get_or_raise(id)
         atualizado = original.model_copy(
             update=dto.model_dump(exclude_unset=True)
         )
         self._dao.update(atualizado)
         return atualizado
 
     def delete(self, id: Any) -> TDTO:
-        self.get(id)
+        self.get_or_raise(id)
         return self._dao.delete(id)
 
     def paginate_response(self, req_args: RequestArgs
                               , data    : List[TDTO]
                               , exclude : set[str] | None = None
                               , include : set[str] | None = None) -> dict[str, Any]:
-        rows_total = self._dao.get_rows_total()
+        rows_total = self._dao.get_rows_total(req_args)
         pagination_params = req_args.get_pagination_params()
         current_page = int(pagination_params["page"])
         total_pages = math.ceil(rows_total / int(pagination_params["limit"]))
 
+        next_page: int | None = None
         if current_page < total_pages:
             next_page = current_page + 1
-        else:
-            next_page = None
+            pass
 
-        if current_page == 1:
-            prev_page = None
-        else:
+        prev_page: int | None = None
+        if current_page != 1:
             prev_page = current_page - 1
+            pass
 
         if include:
             ndata = [model.model_dump(include=include) for model in data]
         elif exclude:
             ndata = [model.model_dump(exclude=exclude) for model in data]
         else:
             ndata = [model.model_dump() for model in data]
 
         response = {
+            "total": rows_total,
             "next_page": next_page,
             "current_page": current_page,
             "total_pages": total_pages,
             "prev_page": prev_page,
             "data": ndata,
         }
```

### Comparing `nsj_flask_utils-0.1.1/nsj_flask_utils/utils/error_handlers.py` & `nsj_flask_utils-0.1.2/nsj_flask_utils/utils/error_handlers.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_utils-0.1.1/nsj_flask_utils/utils/pagination_params.py` & `nsj_flask_utils-0.1.2/nsj_flask_utils/utils/pagination_params.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_utils-0.1.1/nsj_flask_utils/utils/request_args.py` & `nsj_flask_utils-0.1.2/nsj_flask_utils/utils/request_args.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,28 @@
 
 from nsj_flask_utils.dtos.base_dto import BaseDTO
 from nsj_flask_utils.exceptions    import HTTP400
 
 from .filter_params     import FilterParams
 from .pagination_params import PaginationParams, PaginationDTO
 
+
 class RequestArgs:
     filter_params: FilterParams
     pagi_params  : PaginationParams
+    group_by     : str | None
+
+    def __init__(self, dto_cls : type[BaseDTO]
+                     , args    : MultiDict[str, str]
+                     , group_by: bool = False) -> None:
+        self.group_by = None
+        if group_by:
+            self.group_by = args.pop('group_by', None)
+            pass
 
-    def __init__(self, dto_cls: type[BaseDTO]
-                     , args   : MultiDict[str, str]) -> None:
         (obj_fields, pagi_dto) = self._validate(dto_cls, args)
         self.filter_params = FilterParams(obj_fields)
         self.pagi_params   = PaginationParams(
             dto_cls, pagi_dto
         )
         pass
```

### Comparing `nsj_flask_utils-0.1.1/PKG-INFO` & `nsj_flask_utils-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-flask-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utils for Flask
 License: MIT
 Author: Vinicius Teshima
 Author-email: viniciusteshima@nasajon.com.br
 Requires-Python: ==3.11.4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

