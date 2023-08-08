# Comparing `tmp/databeakers-0.1.0.tar.gz` & `tmp/databeakers-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databeakers-0.1.0.tar", max compression
+gzip compressed data, was "databeakers-0.1.2.tar", max compression
```

## Comparing `databeakers-0.1.0.tar` & `databeakers-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    32337 2023-07-26 19:53:05.541419 databeakers-0.1.0/LICENSE
--rw-r--r--   0        0        0     3470 2023-07-26 19:53:05.541623 databeakers-0.1.0/README.md
--rw-r--r--   0        0        0      681 2023-08-03 06:18:01.633516 databeakers-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       39 2023-07-26 19:53:05.541992 databeakers-0.1.0/src/databeakers/__init__.py
--rw-r--r--   0        0        0     3942 2023-07-26 19:53:05.542135 databeakers-0.1.0/src/databeakers/beakers.py
--rw-r--r--   0        0        0     3333 2023-08-03 06:19:06.993854 databeakers-0.1.0/src/databeakers/cli.py
--rw-r--r--   0        0        0      160 2023-07-26 19:53:05.542411 databeakers-0.1.0/src/databeakers/exceptions.py
--rw-r--r--   0        0        0     1070 2023-07-26 19:53:05.542662 databeakers-0.1.0/src/databeakers/http.py
--rw-r--r--   0        0        0     1547 2023-08-03 06:24:32.984044 databeakers-0.1.0/src/databeakers/models.py
--rw-r--r--   0        0        0    18108 2023-08-03 06:24:04.432792 databeakers-0.1.0/src/databeakers/pipeline.py
--rw-r--r--   0        0        0      588 2023-07-26 19:53:05.543259 databeakers-0.1.0/src/databeakers/record.py
--rw-r--r--   0        0        0     4452 1970-01-01 00:00:00.000000 databeakers-0.1.0/setup.py
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 databeakers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    32337 2023-07-19 03:19:38.035740 databeakers-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3470 2023-07-20 04:18:52.572124 databeakers-0.1.2/README.md
+-rw-r--r--   0        0        0      685 2023-08-08 19:55:54.589044 databeakers-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-08-03 18:36:28.538645 databeakers-0.1.2/src/databeakers/__init__.py
+-rw-r--r--   0        0        0     3942 2023-08-03 18:36:28.538977 databeakers-0.1.2/src/databeakers/beakers.py
+-rw-r--r--   0        0        0     5826 2023-08-08 03:10:38.098834 databeakers-0.1.2/src/databeakers/cli.py
+-rw-r--r--   0        0        0      160 2023-08-03 18:36:28.539534 databeakers-0.1.2/src/databeakers/exceptions.py
+-rw-r--r--   0        0        0     1160 2023-08-06 01:11:09.820423 databeakers-0.1.2/src/databeakers/http.py
+-rw-r--r--   0        0        0     1547 2023-08-03 18:36:28.539922 databeakers-0.1.2/src/databeakers/models.py
+-rw-r--r--   0        0        0    17568 2023-08-06 00:46:52.969614 databeakers-0.1.2/src/databeakers/pipeline.py
+-rw-r--r--   0        0        0      668 2023-08-03 18:36:28.540154 databeakers-0.1.2/src/databeakers/record.py
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 databeakers-0.1.2/PKG-INFO
```

### Comparing `databeakers-0.1.0/LICENSE` & `databeakers-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `databeakers-0.1.0/README.md` & `databeakers-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `databeakers-0.1.0/pyproject.toml` & `databeakers-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "databeakers"
-version = "0.1.0"
+version = "0.1.2"
 description = ""
 authors = ["James Turk <dev@jamesturk.net>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
-bkr = 'beakers.cli:app'
+bkr = 'databeakers.cli:app'
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 #scrapeghost = {path = "../scrapeghost", develop = true}
 scrapelib = "^2.1.0"
 httpx = "^0.24.0"
```

### Comparing `databeakers-0.1.0/src/databeakers/beakers.py` & `databeakers-0.1.2/src/databeakers/beakers.py`

 * *Files identical despite different names*

### Comparing `databeakers-0.1.0/src/databeakers/models.py` & `databeakers-0.1.2/src/databeakers/models.py`

 * *Files identical despite different names*

### Comparing `databeakers-0.1.0/src/databeakers/pipeline.py` & `databeakers-0.1.2/src/databeakers/pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 from pydantic import BaseModel
 from structlog import get_logger
 
 from .beakers import Beaker, SqliteBeaker, TempBeaker
 from .record import Record
 from .exceptions import ItemNotFound, SeedError
 
+# !!! Note:
+# by convention, a variable ending with _b is a beaker name
+# & a variable ending with _beaker is a beaker instance
+# _beaker_name is sometimes used to be explicit, and is also a name
+
 log = get_logger()
 
 
 class Pipeline:
     def __init__(self, name: str, db_name: str = "beakers.db", *, num_workers: int = 1):
         self.name = name
         self.num_workers = num_workers
@@ -62,15 +67,18 @@
         *,
         name: str | None = None,
         edge_type: EdgeType = EdgeType.transform,
         error_map: dict[tuple, str] | None = None,
         whole_record: bool = False,
     ) -> None:
         if name is None:
-            name = func.__name__ if func.__name__ != "<lambda>" else "λ"
+            if hasattr(func, "__name__"):
+                name = "λ" if func.__name__ == "<lambda>" else func.__name__
+            else:
+                name = repr(func)
         edge = Edge(
             name=name,
             edge_type=edge_type,
             func=func,
             error_map=error_map or {},
             whole_record=whole_record,
         )
@@ -203,17 +211,19 @@
         log.info("run", pipeline=self)
 
         # go through each node in forward order
         if run_mode == RunMode.waterfall:
             return self._run_waterfall(start_beaker, end_beaker, report)
         elif run_mode == RunMode.river:
             return self._run_river(start_beaker, end_beaker, report)
+        else:
+            raise ValueError(f"Unknown run mode {run_mode}")
 
     def _run_waterfall(
-        self, start_beaker: str, end_beaker: str, report: RunReport
+        self, start_beaker: str | None, end_beaker: str | None, report: RunReport
     ) -> RunReport:
         started = False if start_beaker else True
         for node in networkx.topological_sort(self.graph):
             # only process nodes between start and end
             if not started:
                 if node == start_beaker:
                     started = True
@@ -241,60 +251,64 @@
         for beaker_name, beaker in self.beakers.items():
             try:
                 rec[beaker_name] = beaker.get_item(id)
             except ItemNotFound:
                 pass
         return rec
 
+    def _all_upstream(self, to_beaker: Beaker, edge: Edge):
+        all_upstream = to_beaker.id_set()
+        for error_b in edge.error_map.values():
+            all_upstream |= self.beakers[error_b].id_set()
+        return all_upstream
+
     def _run_node_waterfall(self, node: str) -> dict[str, int]:
         """
         Run a single node in a waterfall run, returning a report of items dispatched.
         """
         loop = asyncio.new_event_loop()
         # store count of dispatched items
         node_report: dict[str, int] = defaultdict(int)
 
-        # convert coroutine to function if needed
-        # if inspect.iscoroutinefunction(edge.func):
-        #     def e_func(x: BaseModel) -> BaseModel:
-        #         return loop.run_until_complete(edge.func(x))
-
         # get outbound edges
         edges = self.graph.out_edges(node, data=True)
         for from_b, to_b, e in edges:
             from_beaker = self.beakers[from_b]
             to_beaker = self.beakers[to_b]
             edge = e["edge"]
-            already_processed = from_beaker.id_set() & to_beaker.id_set()
+            all_upstream = self._all_upstream(to_beaker, edge)
+            already_processed = from_beaker.id_set() & all_upstream
             node_report["_already_processed"] += len(already_processed)
 
             log.info(
                 "processing edge",
                 from_b=from_beaker.name,
                 to_b=to_beaker.name,
                 edge=edge.name,
                 to_process=len(from_beaker) - len(already_processed),
                 already_processed=len(already_processed),
             )
             partial_result = loop.run_until_complete(
-                self._run_edge_async(from_beaker, to_beaker, edge, already_processed)
+                self._run_edge_waterfall(
+                    from_beaker, to_beaker, edge, already_processed
+                )
             )
             for k, v in partial_result.items():
                 node_report[k] += v
 
         return node_report
 
-    async def _run_edge_async(
+    async def _run_edge_waterfall(
         self,
         from_beaker: Beaker,
         to_beaker: Beaker,
         edge: Edge,
         already_processed: set[str],
     ) -> dict[str, int]:
-        queue = asyncio.Queue()
+        queue: asyncio.Queue[tuple[str, Record]] = asyncio.Queue()
         node_report: dict[str, int] = defaultdict(int)
 
         # enqueue all items
         for id, item in from_beaker.items():
             if id in already_processed:
                 continue
             queue.put_nowait((id, item))
@@ -309,30 +323,22 @@
                 except RuntimeError:
                     # queue closed
                     return
                 log.info("task accepted", worker=name, id=id, item=item, edge=edge.name)
 
                 try:
                     with self.db:
-                        result_loc = await self._process_item(edge, to_beaker, id, item)
+                        result_loc = await self._run_edge_func(
+                            from_beaker.name, edge, to_beaker, id, item=item
+                        )
                     node_report[result_loc] += 1
                 except Exception:
                     # uncaught exception, log and re-raise
                     result_loc = "UNCAUGHT_EXCEPTION"
                     raise
-                except asyncio.CancelledError:
-                    # task cancelled, return quietly
-                    log.info(
-                        "task cancelled",
-                        worker=name,
-                        id=id,
-                        item=item,
-                        sent_to=result_loc,
-                    )
-                    return
                 finally:
                     queue.task_done()
                     log.info(
                         "task done", worker=name, id=id, item=item, sent_to=result_loc
                     )
 
         workers = [
@@ -353,39 +359,72 @@
                 w.cancel()
             else:
                 to_raise = w.exception()
         if to_raise:
             raise to_raise
         return node_report
 
-    async def _process_item(self, edge, to_beaker, id, item) -> str:
+    def _run_river(self, start_b, end_b, report: RunReport) -> RunReport:
+        loop = asyncio.new_event_loop()
+        if not start_b:
+            start_b = list(networkx.topological_sort(self.graph))[0]
+        start_beaker = self.beakers[start_b]
+        report.nodes = defaultdict(lambda: defaultdict(int))
+
+        for id in start_beaker.id_set():
+            record = self._get_full_record(id)
+            log.info("river record", id=id, record=record)
+            for from_b, to_b in loop.run_until_complete(
+                self._run_one_item_river(record, start_b, end_b)
+            ):
+                report.nodes[from_b][to_b] += 1
+
+        return report
+
+    async def _run_edge_func(
+        self,
+        cur_b: str,
+        edge: Edge,
+        to_beaker: Beaker,
+        id: str,
+        *,
+        item: BaseModel | None = None,
+        record: Record | None = None,
+    ):
         """
-        Process a single item, returning the name of the beaker it was dispatched to.
+        Used in river and waterfall runs, logic around an edge function
+        hardly varies between them.
 
-        Returns: name of destination beaker (for reporting)
+        One key difference is that in waterfall runs, record
+        is always None, so will be fetched using _get_full_record.
+
+        Returns: result_beaker_name
         """
         try:
             if edge.whole_record:
-                record = self._get_full_record(id)
+                if record is None:
+                    record = self._get_full_record(id)
                 result = edge.func(record)
             else:
+                if item is None and record:
+                    item = record[cur_b]
                 result = edge.func(item)
-            match edge.edge_type:
-                case EdgeType.transform:
-                    # transform: add result to to_beaker (if not None)
-                    if result is not None:
-                        to_beaker.add_item(result, id)
-                        return to_beaker.name
-                case EdgeType.conditional:
-                    # conditional: add item to to_beaker if e_func returns truthy
-                    if result:
-                        to_beaker.add_item(item, id)
-                        return to_beaker.name
+            if inspect.isawaitable(result):
+                result = await result
+            if record:
+                record[to_beaker.name] = result
         except Exception as e:
-            log.info("exception", exception=repr(e), id=id, item=item)
+            log.info(
+                "exception",
+                exception=repr(e),
+                edge=edge,
+                id=id,
+                item=item,
+                record=record,
+            )
             for (
                 error_types,
                 error_beaker_name,
             ) in edge.error_map.items():
                 if isinstance(e, error_types):
                     error_beaker = self.beakers[error_beaker_name]
                     error_beaker.add_item(
@@ -397,30 +436,37 @@
                         id,
                     )
                     return error_beaker.name
             else:
                 # no error handler, re-raise
                 raise
 
-    def _run_river(self, start_b, end_b, report: RunReport) -> RunReport:
-        loop = asyncio.new_event_loop()
-        if not start_b:
-            start_b = list(networkx.topological_sort(self.graph))[0]
-        start_beaker = self.beakers[start_b]
-        report.nodes = defaultdict(lambda: defaultdict(int))
-
-        for id in start_beaker.id_set():
-            record = self._get_full_record(id)
-            log.info("river record", id=id, record=record)
-            for from_b, to_b in loop.run_until_complete(self._run_one_item(record, start_b, end_b)):
-                report.nodes[from_b][to_b] += 1
-
-        return report
-
-    async def _run_one_item(self, record: Record, cur_b: str, end_b: str) -> list[tuple[str, str]]:
+        # propagate result to downstream beakers
+        match edge.edge_type:
+            case EdgeType.transform:
+                # transform: add result to to_beaker (if not None)
+                if result is not None:
+                    to_beaker.add_item(result, id)
+                    to_beaker_name = to_beaker.name
+                else:
+                    to_beaker_name = "_none"
+            case EdgeType.conditional:
+                # conditional: add item to to_beaker if e_func returns truthy
+                if result:
+                    to_beaker.add_item(item, id)
+                    to_beaker_name = to_beaker.name
+                else:
+                    to_beaker_name = "_none"
+            case _:
+                raise ValueError(f"Unknown edge type {edge.edge_type}")
+        return to_beaker_name
+
+    async def _run_one_item_river(
+        self, record: Record, cur_b: str, end_b: str
+    ) -> list[tuple[str, str]]:
         """
         Run a single item through a single beaker.
 
         Calls itself recursively to fan out to downstream beakers.
 
         Return list of (from, to) pairs.
         """
@@ -429,72 +475,32 @@
         from_to = []
 
         # fan an item out to all downstream beakers
         for _, to_b, e in self.graph.out_edges(cur_b, data=True):
             edge = e["edge"]
             to_beaker = self.beakers[to_b]
 
-            # TODO: better way to do this
-            if record.id in to_beaker.id_set():
+            # TODO: cache this upstream set?
+            if record.id in self._all_upstream(to_beaker, edge):
                 from_to.append((cur_b, "_already_processed"))
                 # already processed this item, nothing to do
                 continue
 
             if to_b == end_b:
                 stop_early = True
 
-            try:
-                if edge.whole_record:
-                    result = edge.func(record)
-                else:
-                    result = edge.func(record[cur_b])
-                match edge.edge_type:
-                    case EdgeType.transform:
-                        if result is not None:
-                            to_beaker.add_item(result, record.id)
-                            from_to.append((cur_b, to_b))
-                            # update record to include the result
-                            record[to_b] = result
-                            subtasks.append(
-                                asyncio.create_task(self._run_one_item(record, to_b, end_b))
-                            )
-                    case EdgeType.conditional:
-                        if result:
-                            to_beaker.add_item(record[cur_b], record.id)
-                            from_to.append((cur_b, to_b))
-                            subtasks.append(
-                                asyncio.create_task(self._run_one_item(record, to_b, end_b))
-                            )
-            except Exception as e:
-                log.info("exception", exception=repr(e), record=record)
-                for (
-                    error_types,
-                    error_beaker_name,
-                ) in edge.error_map.items():
-                    if isinstance(e, error_types):
-                        error_beaker = self.beakers[error_beaker_name]
-                        error_beaker.add_item(
-                            ErrorType(
-                                item=record[cur_b],
-                                exception=str(e),
-                                exc_type=str(type(e)),
-                            ),
-                            record.id,
-                        )
-                        from_to.append((cur_b, error_beaker_name))
-                        subtasks.append(
-                            asyncio.create_task(
-                                self._run_one_item(record, error_beaker_name, end_b)
-                            )
-                        )
-                        break
-                else:
-                    # no error handler, re-raise
-                    raise
+            result_beaker = await self._run_edge_func(
+                cur_b, edge, to_beaker, record.id, record=record
+            )
+            from_to.append((cur_b, result_beaker))
+            subtasks.append(self._run_one_item_river(record, result_beaker, end_b))
 
+        log.info(
+            "river subtasks", cur_b=cur_b, subtasks=len(subtasks), stop_early=stop_early
+        )
         if subtasks and not stop_early:
             results = await asyncio.gather(*subtasks, return_exceptions=True)
             for r in results:
                 if isinstance(r, Exception):
                     raise r
                 else:
                     from_to.extend(r)
```

### Comparing `databeakers-0.1.0/src/databeakers/record.py` & `databeakers-0.1.2/src/databeakers/record.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,7 +14,10 @@
         return self._data[name]
 
     def __setitem__(self, name: str, value: BaseModel) -> None:
         if name not in self._data and name not in self._reserved_names:
             self._data[name] = value
         else:
             raise AttributeError(f"DataObject attribute {name} already exists")
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}({self.id})"
```

### Comparing `databeakers-0.1.0/setup.py` & `databeakers-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,88 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: databeakers
+Version: 0.1.2
+Summary: 
+Author: James Turk
+Author-email: dev@jamesturk.net
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: networkx (>=3.1,<4.0)
+Requires-Dist: pydantic (>=2.0.2,<3.0.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: scrapelib (>=2.1.0,<3.0.0)
+Requires-Dist: structlog (>=23.1.0,<24.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# beakers
 
-packages = \
-['databeakers']
+beakers is an experimental lightweight declarative ETL framework for Python
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['httpx>=0.24.0,<0.25.0',
- 'networkx>=3.1,<4.0',
- 'pydantic>=2.0.2,<3.0.0',
- 'rich>=13.4.2,<14.0.0',
- 'scrapelib>=2.1.0,<3.0.0',
- 'structlog>=23.1.0,<24.0.0',
- 'typer>=0.9.0,<0.10.0']
-
-entry_points = \
-{'console_scripts': ['bkr = beakers.cli:app']}
-
-setup_kwargs = {
-    'name': 'databeakers',
-    'version': '0.1.0',
-    'description': '',
-    'long_description': '# beakers\n\nbeakers is an experimental lightweight declarative ETL framework for Python\n\nRight now this is an experiment to explore some ideas around ETL.\n\nIt is still very experimental with no stability guarantees. \nIf you\'re interested in poking around, thoughts and feedback are welcome, please reach out before contributing code though as a lot is still in flux.\n\n## (Intended) Features\n\n- [x] Declarative ETL graph comprised of Python functions & Pydantic models\n- [x] Developer-friendly CLI for running processes\n- [x] Synchronous mode for ease of debugging or simple pipelines\n- [x] Data checkpoints stored in local database for intermediate caching & resuming interrupted runs\n- [ ] Asynchronous task execution\n- [ ] Support for multiple backends (sqlite, postgres, etc)\n- [ ] Robust error handling, including retries\n\n## Guiding Principles\n\n* **Lightweight** - Writing a single python file should be enough to get started. It should be as easy to use as a script in that sense.\n* **Data-centric** - Looking at the definition should make it clear what data exists at what step. \n* **Modern Python** - Take full advantage of recent additions to Python, including type hints, `asyncio`, and libraries like `pydantic`.\n* **Developer Experience** - The focus should be on the developer experience, a nice CLI, helpful error messages.\n\n## Anti-Principles\n\nUnlike most tools in this space, this is not a complete "enterprise grade" ETL solution.\n\nIt isn\'t a perfect analogy by any means but beakers strives to be to `luigi` what `flask` is to `Django`. \nIf you are building your entire business around ETL, it makes sense to invest in the infrastructure & tooling to make that work.\nMaybe structuring your code around beakers will make it easier to migrate to one of those tools than if you had written a bespoke script.\nPlus, beakers is Python, so you can always start by running it from within a bigger framework.\n\n## Concepts\n\nLike most ETL tools, beakers is built around a directed acyclic graph (DAG).\n\nThe nodes on this graph are known as "beakers", and the edges are often called "transforms".\n\n(Note: These names aren\'t final, suggestions welcome.)\n\n### Beakers\n\nEach node in the graph is called a "beaker". A beaker is a container for some data.\n\nEach beaker has a name and a type.\nThe name is used to refer to the beaker elsewhere in the graph.\nThe type, represented by a `pydantic` model, defines the structure of the data. By leveraging `pydantic` we get a lot of nice features for free, like validation and serialization.\n\n### Transform\n\nEdges in the graph represent dataflow between beakers. Each edge has a concept of a "source beaker" and a "destination beaker".\n\n These come in two main flavors:\n\n* **Transforms** - A transform places new data in the destination beaker based on data already in the source beaker.\nAn example of this might be a transform that takes a list of URLs and downloads the HTML for each one, placing the results in a new beaker.\n\n* **Filter** - A filter can be used to stop the flow of data from one beaker to another based on some criteria.\n\n### Seed\n\nA concept somewhat unique to beakers is the "seed". A seed is a function that returns initial data for a beaker.\n\nThis is useful for things like starting the graph with a list of URLs to scrape, or a list of images to process.\n\nA beaker can have any number of seeds, for example one might have a short list of URLs to use for testing, and another that reads from a database.',
-    'author': 'James Turk',
-    'author_email': 'dev@jamesturk.net',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+Right now this is an experiment to explore some ideas around ETL.
 
+It is still very experimental with no stability guarantees. 
+If you're interested in poking around, thoughts and feedback are welcome, please reach out before contributing code though as a lot is still in flux.
 
-setup(**setup_kwargs)
+## (Intended) Features
+
+- [x] Declarative ETL graph comprised of Python functions & Pydantic models
+- [x] Developer-friendly CLI for running processes
+- [x] Synchronous mode for ease of debugging or simple pipelines
+- [x] Data checkpoints stored in local database for intermediate caching & resuming interrupted runs
+- [ ] Asynchronous task execution
+- [ ] Support for multiple backends (sqlite, postgres, etc)
+- [ ] Robust error handling, including retries
+
+## Guiding Principles
+
+* **Lightweight** - Writing a single python file should be enough to get started. It should be as easy to use as a script in that sense.
+* **Data-centric** - Looking at the definition should make it clear what data exists at what step. 
+* **Modern Python** - Take full advantage of recent additions to Python, including type hints, `asyncio`, and libraries like `pydantic`.
+* **Developer Experience** - The focus should be on the developer experience, a nice CLI, helpful error messages.
+
+## Anti-Principles
+
+Unlike most tools in this space, this is not a complete "enterprise grade" ETL solution.
+
+It isn't a perfect analogy by any means but beakers strives to be to `luigi` what `flask` is to `Django`. 
+If you are building your entire business around ETL, it makes sense to invest in the infrastructure & tooling to make that work.
+Maybe structuring your code around beakers will make it easier to migrate to one of those tools than if you had written a bespoke script.
+Plus, beakers is Python, so you can always start by running it from within a bigger framework.
+
+## Concepts
+
+Like most ETL tools, beakers is built around a directed acyclic graph (DAG).
+
+The nodes on this graph are known as "beakers", and the edges are often called "transforms".
+
+(Note: These names aren't final, suggestions welcome.)
+
+### Beakers
+
+Each node in the graph is called a "beaker". A beaker is a container for some data.
+
+Each beaker has a name and a type.
+The name is used to refer to the beaker elsewhere in the graph.
+The type, represented by a `pydantic` model, defines the structure of the data. By leveraging `pydantic` we get a lot of nice features for free, like validation and serialization.
+
+### Transform
+
+Edges in the graph represent dataflow between beakers. Each edge has a concept of a "source beaker" and a "destination beaker".
+
+ These come in two main flavors:
+
+* **Transforms** - A transform places new data in the destination beaker based on data already in the source beaker.
+An example of this might be a transform that takes a list of URLs and downloads the HTML for each one, placing the results in a new beaker.
+
+* **Filter** - A filter can be used to stop the flow of data from one beaker to another based on some criteria.
+
+### Seed
+
+A concept somewhat unique to beakers is the "seed". A seed is a function that returns initial data for a beaker.
+
+This is useful for things like starting the graph with a list of URLs to scrape, or a list of images to process.
+
+A beaker can have any number of seeds, for example one might have a short list of URLs to use for testing, and another that reads from a database.
```

