# Comparing `tmp/rdfdf-0.1.6.tar.gz` & `tmp/rdfdf-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfdf-0.1.6.tar", max compression
+gzip compressed data, was "rdfdf-0.1.7.tar", max compression
```

## Comparing `rdfdf-0.1.6.tar` & `rdfdf-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-05-08 07:12:58.000000 rdfdf-0.1.6/LICENSE
--rw-r--r--   0        0        0     8674 2023-06-29 06:45:26.524130 rdfdf-0.1.6/README.md
--rw-r--r--   0        0        0      459 2023-07-05 06:32:54.665184 rdfdf-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 10:17:54.081795 rdfdf-0.1.6/rdfdf/__init__.py
--rw-r--r--   0        0        0      918 2023-05-15 09:40:40.000000 rdfdf-0.1.6/rdfdf/examples/example_1.py
--rw-r--r--   0        0        0     1154 2023-05-15 09:40:40.000000 rdfdf-0.1.6/rdfdf/examples/example_2.py
--rw-r--r--   0        0        0     1517 2023-05-15 09:40:40.000000 rdfdf-0.1.6/rdfdf/examples/example_3.py
--rw-r--r--   0        0        0     1373 2023-05-15 09:40:40.000000 rdfdf-0.1.6/rdfdf/examples/example_4.py
--rw-r--r--   0        0        0        0 2023-05-23 08:11:06.000000 rdfdf-0.1.6/rdfdf/helpers/__init__.py
--rw-r--r--   0        0        0     1323 2023-06-20 14:36:07.751495 rdfdf-0.1.6/rdfdf/helpers/importers.py
--rw-r--r--   0        0        0      969 2023-05-22 07:07:02.000000 rdfdf-0.1.6/rdfdf/helpers/rdfdf_utils.py
--rw-r--r--   0        0        0     4201 2023-07-05 06:32:04.361342 rdfdf-0.1.6/rdfdf/rdfdf.py
--rw-r--r--   0        0        0     9231 1970-01-01 00:00:00.000000 rdfdf-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-08 07:12:58.000000 rdfdf-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5569 2023-07-06 09:06:07.378355 rdfdf-0.1.7/README.md
+-rw-r--r--   0        0        0      459 2023-08-08 13:53:47.363555 rdfdf-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 10:17:54.081795 rdfdf-0.1.7/rdfdf/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:11:06.000000 rdfdf-0.1.7/rdfdf/helpers/__init__.py
+-rw-r--r--   0        0        0     1323 2023-06-20 14:36:07.751495 rdfdf-0.1.7/rdfdf/helpers/importers.py
+-rw-r--r--   0        0        0     1010 2023-07-05 09:33:18.189851 rdfdf-0.1.7/rdfdf/helpers/rdfdf_utils.py
+-rw-r--r--   0        0        0     3933 2023-07-06 08:36:25.219082 rdfdf-0.1.7/rdfdf/rdfdf.py
+-rw-r--r--   0        0        0      328 2023-07-05 08:35:59.657869 rdfdf-0.1.7/rdfdf/rdfdf_types.py
+-rw-r--r--   0        0        0     6126 1970-01-01 00:00:00.000000 rdfdf-0.1.7/PKG-INFO
```

### Comparing `rdfdf-0.1.6/LICENSE` & `rdfdf-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.6/rdfdf/helpers/importers.py` & `rdfdf-0.1.7/rdfdf/helpers/importers.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.6/rdfdf/helpers/rdfdf_utils.py` & `rdfdf-0.1.7/rdfdf/helpers/rdfdf_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import hashlib
 import inspect
 import functools
 import types
 
+## todo: try to fix closure problem + move to LispKit
 def anaphoric(**anaphors):
     """Decorator for making bindings defined in **anaphors available in a decorated function.
-    
+
     Example:
-    
+
     @anaphoric(x=1, y=2, z=3)
     def foo():
         return x, y, z
 
     foo() # -> (1, 2, 3)
 
     For anaphoric references see https://en.wikipedia.org/wiki/Anaphoric_macro.
@@ -29,12 +30,11 @@
 
             return _f(*args, **kwargs)
         return _wrapper
     return _decor
 
 
 def genhash(string: str) -> str:
-    """Hash generator for language encoding.
-    """
+    """Hash generator for language encoding."""
     # _hash = hashlib.md5(string.encode("UTF-8"))
     _hash = hashlib.sha1(string.encode("UTF-8"))
     return _hash.hexdigest()[:8]
```

### Comparing `rdfdf-0.1.6/rdfdf/rdfdf.py` & `rdfdf-0.1.7/rdfdf/rdfdf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,131 +1,122 @@
-from collections.abc import Callable, Mapping, Iterable
-from typing import Generator
+"""rdfdf - Functionality for rule-based Dataframe to Graph conversion."""
+
+import functools
+
+from collections.abc import Iterable, Callable
+from typing import Generator, Optional
 
 import pandas as pd
-from rdflib import Graph, Literal, URIRef, Namespace
+from rdflib import Graph, URIRef, Namespace
 
-_TripleObject = URIRef | Literal
-_FieldRules = Mapping[str, tuple[URIRef, Callable[[str], _TripleObject]]]
-_TripleType = tuple[URIRef, URIRef, _TripleObject]
+from rdfdf.rdfdf_types import _RulesMapping
 
 
 class DFGraphConverter:
     """Rule-based pandas.DataFrame to rdflib.Graph converter.
 
-    DFGraphConverter iterates over a dataframe and constructs RDF triples by constructing a generator of subgraphs ('field graphs');
+    DFGraphConverter iterates over a dataframe and constructs RDF triples
+    by constructing a generator of subgraphs ('field graphs');
     subgraphs are then merged with an rdflib.Graph component.
 
-    For basic usage examples see https://gitlab.com/lupl/rdfdf.
+    For basic usage examples see https://github.com/lu-pl/rdfdf.
     """
 
     store: dict = dict()
 
     def __init__(self,
                  dataframe: pd.DataFrame,
                  *,
                  subject_column: str,
-                 subject_rule: Callable[[str], URIRef] | Namespace = None,
-                 column_rules: Mapping[str, Callable[[], Graph | None]],
-                 graph: Graph = None):
-
+                 subject_rule: Optional[
+                     Callable[[str], URIRef] | Namespace
+                 ] = None,
+                 column_rules: _RulesMapping,
+                 graph: Optional[Graph] = None):
+        """Initialize a DFGraphConverter instance."""
         self._df = dataframe
         self._subject_column = subject_column
         self._subject_rule = subject_rule
         self._column_rules = column_rules
         # bug fix: this allows also empty but namespaced graphs
         self._graph = Graph() if graph is None else graph
 
     def _apply_subject_rule(self, row: pd.Series) -> URIRef:
-        """Applies subject_rule to the subject_column of a pd.Series row;
-        conveniently allows to also pass an rdflib.Namespace (or generally Sequence types) as subject_rule.
-        """
+        """Apply subject_rule to the subject_column of a pd.Series row.
 
+        Conveniently allows to also pass an rdflib.Namespace
+        (or generally Sequence types) as subject_rule.
+        """
         try:
             # call
             _sub_uri = self._subject_rule(row[self._subject_column])
         except TypeError:
             # getitem
             _sub_uri = self._subject_rule[row[self._subject_column]]
 
         return _sub_uri
 
     def _generate_graphs(self) -> Generator[Graph, None, None]:
-        """Loops over the table rows of the provided DataFrame;
-        generates and returns a Generator of graph objects for merging.
-        """
+        """Loop over the table rows of the provided DataFrame.
 
+        Generates and returns a Generator of graph objects for merging.
+        """
         for _, row in self._df.iterrows():
 
             _subject = (
                 self._apply_subject_rule(row)
                 if self._subject_rule
                 else row[self._subject_column]
             )
 
             for field, rule in self._column_rules.items():
                 _object = row[field]
 
-                ## old
-                # make bindings meaningful in rule callables
-                # rule = anaphoric(
-                #     __subject__=_subject,
-                #     __object__=_object,
-                #     __store__=self.store
-                # )(rule)
-
-                ## new
                 field_rule_result = rule(
                     _subject,
                     _object,
                     self.store
                 )
 
                 # yield only rdflib.Graph instances
                 if isinstance(field_rule_result, Graph):
                     yield field_rule_result
                 continue
 
-    def _merge_to_graph_component(self,
-                                  graphs: Iterable[Graph]) -> Graph:
-        """Loops over a graphs generator and merges every field_graph to the self._graph component.
-        Returns the modified self._graph component.
-        """
+    def _merge_to_graph_component(self, graphs: Iterable[Graph]) -> Graph:
+        """Merge subgraphs to main graph.
 
+        Loops over a graphs generator and merges every field_graph with the
+        self._graph component. Returns the modified self._graph component.
+        """
         # warning: this is not BNode-safe (yet)!!!
-        # how to do BNode-safe graph merging?
+        # todo: how to do BNode-safe graph merging?
         for graph in graphs:
             self._graph += graph
 
         return self._graph
 
     @property
     def graph(self):
-        """Getter for the internal graph component.
-        """
+        """Getter for the internal graph component."""
         return self._graph
 
     def to_graph(self) -> Graph:
-        """rdflib.Graph.adds triples from _generate_triples and returns the graph component."""
+        """Add triples from _generate_triples and return the graph component."""
         # generate subgraphs
         _graphs_generator = self._generate_graphs()
 
         # merge subgraphs to graph component
         self._merge_to_graph_component(_graphs_generator)
 
         return self._graph
 
+    @functools.wraps(Graph.serialize)
     def serialize(self, *args, **kwargs):
-        """Proxy for rdflib.Graph.serialize.
-        """
+        """Serialize triples from graph component.
 
+        Proxy for rdflib.Graph.serialize.
+        """
         if not self._graph:
             self.to_graph
 
         return self._graph.serialize(*args, **kwargs)
-
-
-# todo
-class GraphDFConverter:
-    """Rule-based rdflib.Graph to pandas.DataFrame converter.
-    """
-    ...
```

