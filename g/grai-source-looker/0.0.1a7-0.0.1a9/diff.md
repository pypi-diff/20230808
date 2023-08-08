# Comparing `tmp/grai_source_looker-0.0.1a7.tar.gz` & `tmp/grai_source_looker-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_looker-0.0.1a7.tar", max compression
+gzip compressed data, was "grai_source_looker-0.0.1a9.tar", max compression
```

## Comparing `grai_source_looker-0.0.1a7.tar` & `grai_source_looker-0.0.1a9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      133 2023-08-04 13:13:12.227156 grai_source_looker-0.0.1a7/README.md
--rw-r--r--   0        0        0     1123 2023-08-04 14:16:48.820507 grai_source_looker-0.0.1a7/pyproject.toml
--rw-r--r--   0        0        0       97 2023-08-04 14:16:53.685911 grai_source_looker-0.0.1a7/src/grai_source_looker/__init__.py
--rw-r--r--   0        0        0    10796 2023-08-04 13:13:12.238817 grai_source_looker-0.0.1a7/src/grai_source_looker/adapters.py
--rw-r--r--   0        0        0       48 2023-08-04 13:13:12.239339 grai_source_looker-0.0.1a7/src/grai_source_looker/api/__init__.py
--rw-r--r--   0        0        0   642045 2023-08-04 13:13:12.242056 grai_source_looker-0.0.1a7/src/grai_source_looker/api/api_models.py
--rw-r--r--   0        0        0     1410 2023-08-04 13:13:12.243796 grai_source_looker-0.0.1a7/src/grai_source_looker/base.py
--rw-r--r--   0        0        0     5832 2023-08-04 14:16:42.225829 grai_source_looker-0.0.1a7/src/grai_source_looker/loader.py
--rw-r--r--   0        0        0     5963 2023-08-04 13:13:12.244847 grai_source_looker-0.0.1a7/src/grai_source_looker/models.py
--rw-r--r--   0        0        0      195 2023-08-04 13:13:12.245077 grai_source_looker-0.0.1a7/src/grai_source_looker/package_definitions.py
--rw-r--r--   0        0        0        0 2023-08-04 13:13:12.245125 grai_source_looker-0.0.1a7/src/grai_source_looker/py.typed
--rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 grai_source_looker-0.0.1a7/PKG-INFO
+-rw-r--r--   0        0        0      133 2023-08-08 08:24:27.097774 grai_source_looker-0.0.1a9/README.md
+-rw-r--r--   0        0        0     1123 2023-08-08 08:54:06.113353 grai_source_looker-0.0.1a9/pyproject.toml
+-rw-r--r--   0        0        0       97 2023-08-08 08:54:09.861236 grai_source_looker-0.0.1a9/src/grai_source_looker/__init__.py
+-rw-r--r--   0        0        0    10349 2023-08-08 08:24:27.103881 grai_source_looker-0.0.1a9/src/grai_source_looker/adapters.py
+-rw-r--r--   0        0        0       48 2023-08-08 08:24:27.104718 grai_source_looker-0.0.1a9/src/grai_source_looker/api/__init__.py
+-rw-r--r--   0        0        0   642045 2023-08-08 08:24:27.106322 grai_source_looker-0.0.1a9/src/grai_source_looker/api/api_models.py
+-rw-r--r--   0        0        0     1504 2023-08-08 13:09:20.363685 grai_source_looker-0.0.1a9/src/grai_source_looker/base.py
+-rw-r--r--   0        0        0     6624 2023-08-08 09:59:03.312118 grai_source_looker-0.0.1a9/src/grai_source_looker/loader.py
+-rw-r--r--   0        0        0     5482 2023-08-08 09:10:14.431787 grai_source_looker-0.0.1a9/src/grai_source_looker/models.py
+-rw-r--r--   0        0        0      195 2023-08-08 08:24:27.108744 grai_source_looker-0.0.1a9/src/grai_source_looker/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:24:27.108766 grai_source_looker-0.0.1a9/src/grai_source_looker/py.typed
+-rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 grai_source_looker-0.0.1a9/PKG-INFO
```

### Comparing `grai_source_looker-0.0.1a7/pyproject.toml` & `grai_source_looker-0.0.1a9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_looker"
-version = "0.0.1a7"
+version = "0.0.1a9"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_looker", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `grai_source_looker-0.0.1a7/src/grai_source_looker/adapters.py` & `grai_source_looker-0.0.1a9/src/grai_source_looker/adapters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Dict, List, Literal, Sequence, TypeVar, Union
 
 from grai_schemas import config as base_config
 from grai_schemas.v1 import SourcedEdgeV1, SourcedNodeV1, SourceV1
 from grai_schemas.v1.metadata.edges import (
+    BaseEdgeMetadataV1,
     ColumnToColumnMetadata,
     EdgeMetadataTypeLabels,
     GenericEdgeMetadataV1,
     TableToColumnMetadata,
     TableToTableMetadata,
 )
 from grai_schemas.v1.metadata.nodes import (
@@ -36,32 +37,32 @@
 
 
 @multimethod
 def build_grai_metadata(current: Any, desired: Any) -> None:
     """
 
     Args:
-        current (Any):
-        desired (Any):
+        current:
+        desired:
 
     Returns:
 
     Raises:
 
     """
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
 
 
 @build_grai_metadata.register
 def build_grai_metadata_from_dashboard(current: Dashboard, version: Literal["v1"] = "v1") -> TableMetadata:
     """
 
     Args:
-        current (Dashboard):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     data = {
@@ -98,16 +99,16 @@
 
 
 @build_grai_metadata.register
 def build_grai_metadata_from_explore(current: Explore, version: Literal["v1"] = "v1") -> TableMetadata:
     """
 
     Args:
-        current (Explore):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     data = {
@@ -121,16 +122,16 @@
 
 
 @build_grai_metadata.register
 def build_grai_metadata_from_dimension(current: Dimension, version: Literal["v1"] = "v1") -> ColumnMetadata:
     """
 
     Args:
-        current (Dimension):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     data = {
@@ -140,20 +141,20 @@
         "tags": [config.metadata_id],
     }
 
     return ColumnMetadata(**data)
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_edge(current: Edge, version: Literal["v1"] = "v1") -> GenericEdgeMetadataV1:
+def build_grai_metadata_from_edge(current: Edge, version: Literal["v1"] = "v1") -> BaseEdgeMetadataV1:
     """
 
     Args:
-        current (Edge):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     data = {"version": version, "tags": [config.metadata_id]}
@@ -175,32 +176,32 @@
 
 
 @multimethod
 def build_app_metadata(current: Any, desired: Any) -> None:
     """
 
     Args:
-        current (Any):
-        desired (Any):
+        current:
+        desired:
 
     Returns:
 
     Raises:
 
     """
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
 
 
 @build_app_metadata.register
 def build_metadata_from_dashboard(current: Dashboard, version: Literal["v1"] = "v1") -> Dict:
     """
 
     Args:
-        current (Dashboard):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     data = {
@@ -212,16 +213,16 @@
 
 
 @build_app_metadata.register
 def build_metadata_from_query(current: Query, version: Literal["v1"] = "v1") -> Dict:
     """
 
     Args:
-        current (Dashboard):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     data = {
@@ -233,16 +234,16 @@
 
 
 @build_app_metadata.register
 def build_metadata_from_explore(current: Explore, version: Literal["v1"] = "v1") -> Dict:
     """
 
     Args:
-        current (Explore):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     data = {
@@ -254,16 +255,16 @@
 
 
 @build_app_metadata.register
 def build_metadata_from_dimension(current: Dimension, version: Literal["v1"] = "v1") -> Dict:
     """
 
     Args:
-        current (Dimension):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     data = {
@@ -275,27 +276,27 @@
 
 
 @build_app_metadata.register
 def build_metadata_from_edge(current: Edge, version: Literal["v1"] = "v1") -> Dict:
     """
 
     Args:
-        current (Edge):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     data = {
         "definition": current.definition,
         "constraint_type": current.constraint_type.name,
     }
-    data |= current.metadata if current.metadata is not None else {}
+    data.update(current.metadata if current.metadata is not None else {})
 
     return data
 
 
 def build_metadata(obj, version):
     """
 
@@ -315,32 +316,33 @@
 
 
 @multimethod
 def adapt_to_client(current: Any, desired: Any):
     """
 
     Args:
-        current (Any):
-        desired (Any):
+        current:
+        desired:
 
     Returns:
 
     Raises:
 
     """
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)}")
 
 
 @adapt_to_client.register
 def adapt_dashboard_to_client(current: Dashboard, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
-        current (Dashboard):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        source:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     spec_dict = {
@@ -354,16 +356,17 @@
 
 
 @adapt_to_client.register
 def adapt_query_to_client(current: Query, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
-        current (Query):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        source:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     spec_dict = {
@@ -377,16 +380,17 @@
 
 
 @adapt_to_client.register
 def adapt_explore_to_client(current: Explore, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
-        current (Explore):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        source:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     spec_dict = {
@@ -400,16 +404,17 @@
 
 
 @adapt_to_client.register
 def adapt_dimension_to_client(current: Dimension, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
-        current (Dimension):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        source:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     spec_dict = {
@@ -422,16 +427,16 @@
     return SourcedNodeV1.from_spec(spec_dict)
 
 
 def make_name(node1: ID, node2: ID) -> str:
     """
 
     Args:
-        node1 (ID):
-        node2 (ID):
+        node1:
+        node2:
 
     Returns:
 
     Raises:
 
     """
     node1_name = f"{node1.namespace}:{node1.full_name}"
@@ -440,16 +445,17 @@
 
 
 @adapt_to_client.register
 def adapt_edge_to_client(current: Edge, source: SourceSpec, version: Literal["v1"]) -> SourcedEdgeV1:
     """
 
     Args:
-        current (Edge):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        source:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     spec_dict = {
```

### Comparing `grai_source_looker-0.0.1a7/src/grai_source_looker/api/api_models.py` & `grai_source_looker-0.0.1a9/src/grai_source_looker/api/api_models.py`

 * *Files identical despite different names*

### Comparing `grai_source_looker-0.0.1a7/src/grai_source_looker/base.py` & `grai_source_looker-0.0.1a9/src/grai_source_looker/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Tuple
+from typing import Dict, List, Optional, Tuple
 
 from grai_client.integrations.base import (
     CombinedNodesAndEdgesMixin,
     GraiIntegrationImplementation,
 )
 from grai_schemas.base import SourcedEdge, SourcedNode
 from grai_schemas.v1.source import SourceV1
@@ -17,23 +17,25 @@
         source: SourceV1,
         version: Optional[str] = None,
         base_url: Optional[str] = None,
         client_id: Optional[str] = None,
         client_secret: Optional[str] = None,
         verify_ssl: Optional[bool] = None,
         namespace: Optional[str] = None,
+        namespaces: Optional[Dict[str, str]] = None,
     ):
         super().__init__(source, version)
 
         self.connector = LookerAPI(
             base_url=base_url,
             client_id=client_id,
             client_secret=client_secret,
             verify_ssl=verify_ssl,
             namespace=namespace,
+            namespaces=namespaces,
         )
 
     def ready(self) -> bool:
         self.connector.get_user()
         return True
 
     def get_nodes_and_edges(self) -> Tuple[List[SourcedNode], List[SourcedEdge]]:
```

### Comparing `grai_source_looker-0.0.1a7/src/grai_source_looker/loader.py` & `grai_source_looker-0.0.1a9/src/grai_source_looker/loader.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,41 @@
-import asyncio
-import json
+from functools import cached_property
 from itertools import chain
 from typing import (
-    Any,
-    Callable,
     Dict,
-    Iterable,
     List,
     Optional,
-    ParamSpec,
-    Sequence,
-    Tuple,
-    TypedDict,
-    TypeVar,
-    Union,
 )
 
 import looker_sdk
-import requests
 from looker_sdk import api_settings
-from pydantic import BaseModel, BaseSettings, Json, SecretStr, validator
+from pydantic import BaseSettings, SecretStr, validator
 
 from grai_source_looker.models import (
     Constraint,
     Dashboard,
     Edge,
     Explore,
     FieldID,
     TableID,
 )
 
-T = TypeVar("T")
-P = ParamSpec("P")
-
 
 class LookerConfig(BaseSettings):
     """ """
 
     base_url: str
     client_id: str
     client_secret: SecretStr
     verify_ssl: bool = True
-    namespace: str = "default"
+    namespace: str = None
+    namespaces: Dict[str, str] = {}
 
     @validator("base_url")
-    def validate_endpoint(cls, value):
+    def validate_base_url(cls, value):
         """
 
         Args:
             value:
 
         Returns:
 
@@ -92,118 +79,136 @@
     def __init__(
         self,
         base_url: Optional[str] = None,
         client_id: Optional[str] = None,
         client_secret: Optional[str] = None,
         verify_ssl: Optional[bool] = None,
         namespace: Optional[str] = None,
+        namespaces: Optional[Dict[str, str]] = None,
     ):
         passthrough_kwargs = {
             "base_url": base_url,
             "client_id": client_id,
             "client_secret": client_secret,
             "verify_ssl": verify_ssl,
             "namespace": namespace,
+            "namespaces": namespaces,
         }
         self.config = LookerConfig(
             **{k: v for k, v in passthrough_kwargs.items() if v is not None}
         )
 
         settings = LookerSettings(self.config)
 
         self.sdk = looker_sdk.init40(config_settings=settings)
 
-    def get_dashboards(self):
-        result = self.sdk.all_dashboards()
+    def get_model_explore(
+        self, lookml_model_name: str, explore_name: str, namespace: str
+    ) -> Explore:
+        return Explore(
+            namespace=namespace,
+            **self.sdk.lookml_model_explore(lookml_model_name, explore_name),
+        )
 
+    @cached_property
+    def dashboards(self) -> List[Dashboard]:
+        result = self.sdk.all_dashboards()
         return [
             Dashboard(namespace=self.config.namespace, **self.sdk.dashboard(item.id))
             for item in result
         ]
 
-    def get_model_explore(self, lookml_model_name: str, explore_name: str):
-        return Explore(
-            namespace=self.config.namespace,
-            **self.sdk.lookml_model_explore(lookml_model_name, explore_name),
+    @cached_property
+    def queries(self) -> List:
+        query_items = (dashboard.get_queries() for dashboard in self.dashboards)
+        return list(chain(*query_items))
+
+    @cached_property
+    def explores(self) -> List:
+        explores = (
+            self.get_model_explore(query.model, query.view, self.config.namespace)
+            for query in self.queries
         )
+        return [explore for explore in explores if explore]
 
     def get_user(self):
         return self.sdk.me()
 
     def get_nodes_and_edges(self):
-        dashboards = self.get_dashboards()
-
-        queries = []
-        edges = []
-
-        for dashboard in dashboards:
-            q = dashboard.get_queries()
-            queries.extend(q)
-            edges.extend(dashboard.get_query_edges())
-
-            for query in q:
-                explore = self.get_model_explore(query.model, query.view)
+        nodes = [*self.dashboards, *self.queries]
+        edges = list(
+            chain.from_iterable(
+                dashboard.get_query_edges() for dashboard in self.dashboards
+            )
+        )
 
-                if not explore:
-                    print("Explore not found")
+        for query in self.queries:
+            # Fetch custom explore namespace or use default
+            explore_namespace = self.config.namespaces.get(
+                query.model, self.config.namespace
+            )
+
+            explore = self.get_model_explore(query.model, query.view, explore_namespace)
+            # TODO: Typing doesn't make sense here. How can `get_model_explore` return false-y without erroring?
+            if not explore:
+                print("Explore not found")
+                continue
+
+            nodes.append(explore)
+
+            for field in query.fields:
+                dynamic_field = query.dynamic_fields_map.get(field, None)
+
+                if dynamic_field:
+                    field = dynamic_field
+
+                field_dimension = (
+                    dimension
+                    for dimension in explore.fields.dimensions
+                    if dimension.name == field
+                )
+
+                if not (dimension := next(field_dimension, False)):
+                    print(f"Dimension not found {field}")
+                    print(query.dynamic_fields)
                     continue
 
-                queries.append(explore)
-
-                for field in query.fields:
-                    dynamic_field = query.dynamic_fields_map.get(field, None)
-
-                    if dynamic_field:
-                        field = dynamic_field
+                dimension.namespace = explore_namespace
+                dimension.table_name = explore.table_name
 
-                    dimension = next(
-                        (
-                            dimension
-                            for dimension in explore.fields.dimensions
-                            if dimension.name == field
-                        ),
-                        None,
-                    )
-
-                    if not dimension:
-                        print(f"Dimension not found {field}")
-                        continue
-
-                    dimension.namespace = self.config.namespace
-                    dimension.table_name = explore.table_name
-
-                    queries.append(dimension)
-
-                    edge = Edge(
-                        constraint_type=Constraint("bt"),
-                        source=TableID(
-                            name=explore.table_name,
-                            namespace=self.config.namespace,
-                        ),
-                        destination=FieldID(
-                            table_name=explore.table_name,
-                            name=dimension.column_name,
-                            namespace=self.config.namespace,
-                        ),
-                    )
-
-                    edges.append(edge)
-
-                    edge = Edge(
-                        constraint_type=Constraint("f"),
-                        source=FieldID(
-                            table_name=explore.table_name,
-                            name=dimension.column_name,
-                            namespace=self.config.namespace,
-                        ),
-                        destination=FieldID(
-                            table_name=dashboard.name,
-                            name=query.title if query.title else query.id,
-                            namespace=self.config.namespace,
-                        ),
-                    )
+                nodes.append(dimension)
 
-                    edges.append(edge)
+                # TODO: Do these reference tables in their storage database or Looker specific constructs?
+                # We may not need to generate these edges if they correspond to the storage media but in that case
+                # we would need to provide a different namespace from the namespace_map
+                edge = Edge(
+                    constraint_type=Constraint("bt"),
+                    source=TableID(
+                        name=explore.table_name,
+                        namespace=explore_namespace,
+                    ),
+                    destination=FieldID(
+                        table_name=explore.table_name,
+                        name=dimension.column_name,
+                        namespace=explore_namespace,
+                    ),
+                )
+
+                edges.append(edge)
+
+                edge = Edge(
+                    constraint_type=Constraint("f"),
+                    source=FieldID(
+                        table_name=explore.table_name,
+                        name=dimension.column_name,
+                        namespace=explore_namespace,
+                    ),
+                    destination=FieldID(
+                        table_name=query.dashboard_name,
+                        name=query.title if query.title else query.id,
+                        namespace=self.config.namespace,
+                    ),
+                )
 
-        dashboards.extend(queries)
+                edges.append(edge)
 
-        return dashboards, edges
+        return nodes, edges
```

### Comparing `grai_source_looker-0.0.1a7/src/grai_source_looker/models.py` & `grai_source_looker-0.0.1a9/src/grai_source_looker/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -123,18 +123,44 @@
     id: int
     title: Optional[str]
     namespace: Optional[str]
     model: str
     view: str
     fields: List[str]
     dynamic_fields: Optional[str]
+    dashboard_name: Optional[str]
 
     @property
     def dynamic_fields_map(self):
-        return {f["measure"]: f["based_on"] for f in json.loads(self.dynamic_fields)}
+        if not self.dynamic_fields:
+            return {}
+
+        result = {}
+
+        try:
+            for f in json.loads(self.dynamic_fields):
+                category = f.get("category")
+
+                if category == "measure":
+                    result[f["measure"]] = f["based_on"]
+                elif category == "dimension":
+                    # result[f["dimension"]] = f["expression"]
+                    pass
+                elif category == "table_calculation":
+                    pass
+                elif not category and f.get("measure") and f.get("based_on"):
+                    result[f["measure"]] = f["based_on"]
+                else:
+                    print("Unknown category: ", f["category"])
+                    print(self.dynamic_fields)
+
+            return result
+        except:
+            print(self.dynamic_fields)
+            raise
 
 
 class ResultMaker(LookerNode):
     id: int
     query: Optional[Query]
     dynamic_fields: Optional[str]
 
@@ -183,81 +209,38 @@
         for element in self.dashboard_elements if self.dashboard_elements else []:
             query = self.get_query(element)
 
             if query:
                 query.title = element.title
                 query.namespace = self.namespace
                 query.dynamic_fields = element.result_maker.dynamic_fields
+                query.dashboard_name = self.name
 
                 queries.append(query)
 
         return queries
 
     def get_query_edges(self):
         """ """
 
         edges = []
 
         for element in self.dashboard_elements if self.dashboard_elements else []:
             query = self.get_query(element)
 
             if query:
-                edges.extend(
-                    [
-                        Edge(
-                            constraint_type=Constraint("bt"),
-                            source=TableID(
-                                name=self.name,
-                                namespace=self.namespace,
-                            ),
-                            destination=FieldID(
-                                table_name=self.name,
-                                name=element.title if element.title else element.id,
-                                namespace=self.namespace,
-                            ),
-                        )
-                    ]
-                )
-
-        return edges
-
-    def get_fields(self):
-        """ """
-
-        fields = []
-
-        for element in self.dashboard_elements if self.dashboard_elements else []:
-            query = self.get_query(element)
-
-            if query:
-                fields.extend([QueryField(namespace=self.namespace, name=field) for field in query.fields])
-
-        return fields
-
-    def get_edges(self):
-        """ """
-
-        edges = []
-
-        for element in self.dashboard_elements if self.dashboard_elements else []:
-            query = self.get_query(element)
-
-            if query:
-                edges.extend(
-                    [
-                        Edge(
-                            constraint_type=Constraint("bt"),
-                            source=TableID(
-                                name=self.name,
-                                namespace=self.namespace,
-                            ),
-                            destination=FieldID(
-                                table_name=self.name,
-                                name=field,
-                                namespace=self.namespace,
-                            ),
-                        )
-                        for field in query.fields
-                    ]
+                edges.append(
+                    Edge(
+                        constraint_type=Constraint("bt"),
+                        source=TableID(
+                            name=self.name,
+                            namespace=self.namespace,
+                        ),
+                        destination=FieldID(
+                            table_name=self.name,
+                            name=element.title if element.title else element.id,
+                            namespace=self.namespace,
+                        ),
+                    )
                 )
 
         return edges
```

### Comparing `grai_source_looker-0.0.1a7/PKG-INFO` & `grai_source_looker-0.0.1a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-looker
-Version: 0.0.1a7
+Version: 0.0.1a9
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.9.13,<4.0.0
 Classifier: License :: Other/Proprietary License
```

