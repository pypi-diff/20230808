# Comparing `tmp/noteable_origami-1.0.0a3.tar.gz` & `tmp/noteable_origami-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noteable_origami-1.0.0a3.tar", max compression
+gzip compressed data, was "noteable_origami-1.0.0a4.tar", max compression
```

## Comparing `noteable_origami-1.0.0a3.tar` & `noteable_origami-1.0.0a4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1516 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/LICENSE
--rw-r--r--   0        0        0     4615 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/README.md
--rw-r--r--   0        0        0       82 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/clients/__init__.py
--rw-r--r--   0        0        0    14644 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/clients/api.py
--rw-r--r--   0        0        0        0 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/clients/cache.py
--rw-r--r--   0        0        0    42382 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/clients/rtu.py
--rw-r--r--   0        0        0        0 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/api/__init__.py
--rw-r--r--   0        0        0      238 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/api/base.py
--rw-r--r--   0        0        0      649 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/api/datasources.py
--rw-r--r--   0        0        0      924 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/api/files.py
--rw-r--r--   0        0        0      659 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/api/outputs.py
--rw-r--r--   0        0        0      475 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/api/projects.py
--rw-r--r--   0        0        0      437 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/api/spaces.py
--rw-r--r--   0        0        0      681 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/api/users.py
--rw-r--r--   0        0        0        0 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/__init__.py
--rw-r--r--   0        0        0      803 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/base.py
--rw-r--r--   0        0        0      953 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/delta_types/cell_contents.py
--rw-r--r--   0        0        0     1120 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/delta_types/cell_execute.py
--rw-r--r--   0        0        0     1222 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/delta_types/cell_metadata.py
--rw-r--r--   0        0        0      703 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/delta_types/cell_output_collection.py
--rw-r--r--   0        0        0     1115 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/delta_types/nb_cells.py
--rw-r--r--   0        0        0      588 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/delta_types/nb_metadata.py
--rw-r--r--   0        0        0      850 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/discriminators.py
--rw-r--r--   0        0        0      451 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/kernels.py
--rw-r--r--   0        0        0     5018 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/notebook.py
--rw-r--r--   0        0        0        0 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/rtu/__init__.py
--rw-r--r--   0        0        0     1520 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/rtu/base.py
--rw-r--r--   0        0        0        0 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/rtu/channels/__init__.py
--rw-r--r--   0        0        0     7730 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/rtu/channels/files.py
--rw-r--r--   0        0        0     2508 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/rtu/channels/kernels.py
--rw-r--r--   0        0        0     2640 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/rtu/channels/system.py
--rw-r--r--   0        0        0     1210 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/rtu/discriminators.py
--rw-r--r--   0        0        0     1073 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/rtu/errors.py
--rw-r--r--   0        0        0        0 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/notebook/__init__.py
--rw-r--r--   0        0        0    11988 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/notebook/builder.py
--rw-r--r--   0        0        0     2715 2023-08-01 21:50:00.599425 noteable_origami-1.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     5924 1970-01-01 00:00:00.000000 noteable_origami-1.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1516 2023-08-08 15:56:18.300319 noteable_origami-1.0.0a4/LICENSE
+-rw-r--r--   0        0        0     4615 2023-08-08 15:56:18.300319 noteable_origami-1.0.0a4/README.md
+-rw-r--r--   0        0        0       82 2023-08-08 15:56:18.300319 noteable_origami-1.0.0a4/origami/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/clients/__init__.py
+-rw-r--r--   0        0        0    14837 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/clients/api.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/clients/cache.py
+-rw-r--r--   0        0        0    43381 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/clients/rtu.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/api/__init__.py
+-rw-r--r--   0        0        0      238 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/api/base.py
+-rw-r--r--   0        0        0      649 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/api/datasources.py
+-rw-r--r--   0        0        0      924 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/api/files.py
+-rw-r--r--   0        0        0      659 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/api/outputs.py
+-rw-r--r--   0        0        0      475 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/api/projects.py
+-rw-r--r--   0        0        0      437 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/api/spaces.py
+-rw-r--r--   0        0        0      681 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/api/users.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/deltas/__init__.py
+-rw-r--r--   0        0        0      803 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/deltas/base.py
+-rw-r--r--   0        0        0      953 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/deltas/delta_types/cell_contents.py
+-rw-r--r--   0        0        0     1120 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/deltas/delta_types/cell_execute.py
+-rw-r--r--   0        0        0     1222 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/deltas/delta_types/cell_metadata.py
+-rw-r--r--   0        0        0      703 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/deltas/delta_types/cell_output_collection.py
+-rw-r--r--   0        0        0     1115 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/deltas/delta_types/nb_cells.py
+-rw-r--r--   0        0        0      588 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/deltas/delta_types/nb_metadata.py
+-rw-r--r--   0        0        0      850 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/deltas/discriminators.py
+-rw-r--r--   0        0        0      451 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/kernels.py
+-rw-r--r--   0        0        0     5018 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/notebook.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/rtu/__init__.py
+-rw-r--r--   0        0        0     1520 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/rtu/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/rtu/channels/__init__.py
+-rw-r--r--   0        0        0     7730 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/rtu/channels/files.py
+-rw-r--r--   0        0        0     2508 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/rtu/channels/kernels.py
+-rw-r--r--   0        0        0     2640 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/rtu/channels/system.py
+-rw-r--r--   0        0        0     1210 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/rtu/discriminators.py
+-rw-r--r--   0        0        0     1073 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/models/rtu/errors.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/notebook/__init__.py
+-rw-r--r--   0        0        0    11988 2023-08-08 15:56:18.304319 noteable_origami-1.0.0a4/origami/notebook/builder.py
+-rw-r--r--   0        0        0     2715 2023-08-08 15:56:18.308320 noteable_origami-1.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     5924 1970-01-01 00:00:00.000000 noteable_origami-1.0.0a4/PKG-INFO
```

### Comparing `noteable_origami-1.0.0a3/LICENSE` & `noteable_origami-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/README.md` & `noteable_origami-1.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/clients/api.py` & `noteable_origami-1.0.0a4/origami/clients/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,17 @@
 
         self.client = httpx.AsyncClient(
             base_url=self.api_base_url,
             headers=self.headers,
             transport=transport,
             timeout=timeout,
         )
-
+        # Hack until Gate changes out rtu_client_type from enum to str
+        if rtu_client_type not in ['origami', 'origamist', 'planar_ally', 'geas']:
+            rtu_client_type = 'unknown'
         self.rtu_client_type = rtu_client_type  # Only used when generating an RTUClient
 
     def add_tags_and_contextvars(self, **tags):
         """Hook for Apps to override so they can set structlog contextvars or ddtrace tags etc"""
         pass
 
     async def user_info(self) -> User:
```

### Comparing `noteable_origami-1.0.0a3/origami/clients/rtu.py` & `noteable_origami-1.0.0a4/origami/clients/rtu.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from typing import Awaitable, Callable, Dict, List, Literal, Optional, Type
 
 import orjson
 from pydantic import BaseModel, parse_obj_as
 from sending.backends.websocket import WebsocketManager
 from websockets.client import WebSocketClientProtocol
 
+from origami.models.deltas.delta_types.cell_contents import CellContentsReplace, CellContentsUpdate
 from origami.models.deltas.delta_types.cell_execute import (
     CellExecute,
     CellExecuteAfter,
     CellExecuteAll,
     CellExecuteBefore,
 )
 from origami.models.deltas.delta_types.cell_metadata import CellMetadataReplace, CellMetadataUpdate
@@ -818,14 +819,38 @@
             await self.new_delta_request(delta)
         else:
             raise ValueError(f"Unknown cell type {cell_type}")
         # Grab updated cell post-squashing
         _, cell = self.builder.get_cell(cell_id)
         return cell
 
+    async def update_cell_content(self, cell_id: str, patch: str) -> NotebookCell:
+        """
+        Update cell content with a diff-match-patch patch string
+        """
+        delta = CellContentsUpdate(
+            file_id=self.file_id, resource_id=cell_id, properties={'patch': patch}
+        )
+        await self.new_delta_request(delta)
+        # Grab updated cell post-squashing
+        _, cell = self.builder.get_cell(cell_id)
+        return cell
+
+    async def replace_cell_content(self, cell_id: str, source: str) -> NotebookCell:
+        """
+        Replace cell content with a string
+        """
+        delta = CellContentsReplace(
+            file_id=self.file_id, resource_id=cell_id, properties={'source': source}
+        )
+        await self.new_delta_request(delta)
+        # Grab updated cell post-squashing
+        _, cell = self.builder.get_cell(cell_id)
+        return cell
+
     async def queue_execution(
         self,
         cell_id: Optional[str] = None,
         before_id: Optional[str] = None,
         after_id: Optional[str] = None,
         run_all: bool = False,
     ) -> Dict[asyncio.Future[CodeCell], str]:
```

### Comparing `noteable_origami-1.0.0a3/origami/models/api/datasources.py` & `noteable_origami-1.0.0a4/origami/models/api/datasources.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/api/files.py` & `noteable_origami-1.0.0a4/origami/models/api/files.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/api/outputs.py` & `noteable_origami-1.0.0a4/origami/models/api/outputs.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/api/users.py` & `noteable_origami-1.0.0a4/origami/models/api/users.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/deltas/base.py` & `noteable_origami-1.0.0a4/origami/models/deltas/base.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/deltas/delta_types/cell_contents.py` & `noteable_origami-1.0.0a4/origami/models/deltas/delta_types/cell_contents.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/deltas/delta_types/cell_execute.py` & `noteable_origami-1.0.0a4/origami/models/deltas/delta_types/cell_execute.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/deltas/delta_types/cell_metadata.py` & `noteable_origami-1.0.0a4/origami/models/deltas/delta_types/cell_metadata.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/deltas/delta_types/cell_output_collection.py` & `noteable_origami-1.0.0a4/origami/models/deltas/delta_types/cell_output_collection.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/deltas/delta_types/nb_cells.py` & `noteable_origami-1.0.0a4/origami/models/deltas/delta_types/nb_cells.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/deltas/delta_types/nb_metadata.py` & `noteable_origami-1.0.0a4/origami/models/deltas/delta_types/nb_metadata.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/deltas/discriminators.py` & `noteable_origami-1.0.0a4/origami/models/deltas/discriminators.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/notebook.py` & `noteable_origami-1.0.0a4/origami/models/notebook.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/rtu/base.py` & `noteable_origami-1.0.0a4/origami/models/rtu/base.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/rtu/channels/files.py` & `noteable_origami-1.0.0a4/origami/models/rtu/channels/files.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/rtu/channels/kernels.py` & `noteable_origami-1.0.0a4/origami/models/rtu/channels/kernels.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/rtu/channels/system.py` & `noteable_origami-1.0.0a4/origami/models/rtu/channels/system.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/rtu/discriminators.py` & `noteable_origami-1.0.0a4/origami/models/rtu/discriminators.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/models/rtu/errors.py` & `noteable_origami-1.0.0a4/origami/models/rtu/errors.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/origami/notebook/builder.py` & `noteable_origami-1.0.0a4/origami/notebook/builder.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a3/pyproject.toml` & `noteable_origami-1.0.0a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.poetry]
 name = "noteable-origami"
-version = "1.0.0-alpha.3"
+version = "1.0.0-alpha.4"
 description = "The Noteable API interface"
 authors = ["Matt Seal <matt@noteable.io>"]
 maintainers = ["Matt Seal <matt@noteable.io>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/noteable-io/origami"
 # old setup.cfg had a bdist_wheel option.
```

### Comparing `noteable_origami-1.0.0a3/PKG-INFO` & `noteable_origami-1.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noteable-origami
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: The Noteable API interface
 Home-page: https://github.com/noteable-io/origami
 License: BSD-3-Clause
 Keywords: notebook,api,noteable
 Author: Matt Seal
 Author-email: matt@noteable.io
 Maintainer: Matt Seal
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: noteable-origami Version: 1.0.0a3 Summary: The
+Metadata-Version: 2.1 Name: noteable-origami Version: 1.0.0a4 Summary: The
 Noteable API interface Home-page: https://github.com/noteable-io/origami
 License: BSD-3-Clause Keywords: notebook,api,noteable Author: Matt Seal Author-
 email: matt@noteable.io Maintainer: Matt Seal Maintainer-email:
 matt@noteable.io Requires-Python: >=3.8,<4.0 Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

