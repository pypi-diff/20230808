# Comparing `tmp/lodkit-0.1.1.tar.gz` & `tmp/lodkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lodkit-0.1.1.tar", max compression
+gzip compressed data, was "lodkit-0.1.2.tar", max compression
```

## Comparing `lodkit-0.1.1.tar` & `lodkit-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-06-05 13:34:34.817840 lodkit-0.1.1/LICENSE
--rw-r--r--   0        0        0     2877 2023-07-06 06:20:51.465671 lodkit-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-05 13:34:34.821173 lodkit-0.1.1/lodkit/__init__.py
--rw-r--r--   0        0        0     3138 2023-07-06 06:20:51.465671 lodkit-0.1.1/lodkit/connections.py
--rw-r--r--   0        0        0     1335 2023-07-06 06:20:59.159038 lodkit-0.1.1/lodkit/graph.py
--rw-r--r--   0        0        0     1274 2023-06-06 08:39:54.017219 lodkit-0.1.1/lodkit/importer.py
--rw-r--r--   0        0        0     2914 2023-07-06 06:20:59.159038 lodkit-0.1.1/lodkit/reasoners.py
--rw-r--r--   0        0        0      280 2023-07-06 06:20:59.159038 lodkit-0.1.1/lodkit/types.py
--rw-r--r--   0        0        0      397 2023-07-06 06:22:18.586045 lodkit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 lodkit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-05 13:34:34.817840 lodkit-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2943 2023-07-06 06:41:11.800179 lodkit-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 13:34:34.821173 lodkit-0.1.2/lodkit/__init__.py
+-rw-r--r--   0        0        0     3138 2023-07-06 06:20:51.465671 lodkit-0.1.2/lodkit/connections.py
+-rw-r--r--   0        0        0     1414 2023-07-06 06:52:44.256063 lodkit-0.1.2/lodkit/graph.py
+-rw-r--r--   0        0        0     1274 2023-06-06 08:39:54.017219 lodkit-0.1.2/lodkit/importer.py
+-rw-r--r--   0        0        0     2914 2023-07-06 06:20:59.159038 lodkit-0.1.2/lodkit/reasoners.py
+-rw-r--r--   0        0        0      581 2023-07-31 08:01:11.868389 lodkit-0.1.2/lodkit/types.py
+-rw-r--r--   0        0        0      396 2023-08-08 13:55:28.223747 lodkit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3501 1970-01-01 00:00:00.000000 lodkit-0.1.2/PKG-INFO
```

### Comparing `lodkit-0.1.1/LICENSE` & `lodkit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lodkit-0.1.1/README.md` & `lodkit-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,41 +6,47 @@
 LODKit is a collection of Linked Open Data related Python functionalities. 
 
 LODkit (includes|will include)
 - a custom `rdflib.Graph` subclass that is capable of 
   - RDFS and OWL-RL inferencing 
   - Bnode-safe graph merging [todo]
 - a custom importer for loading RDF files as if they where Python modules
+- LOD-specific type definitions
 - [...]
 
 ## Examples
 
 ### lodkit.Graph
 `lodkit.Graph` is an `rdflib.Graph` subclass that is cabable of RFDS and OWL-RL inferencing.
 
 The default plugin for inferencing is the [owlrl](https://github.com/RDFLib/OWL-RL/) native Python inferencing engine. The deductive closure type used for `lodkit.Graph` is [RDFS_OWLRL_Semantics](https://owl-rl.readthedocs.io/en/latest/CombinedClosure.html) which allows for RDFS *and* OWL-RL reasoning.
 
 ```python
-from lodkit import Graph
+from lodkit.graph import Graph
+
 from rdflib import Namespace
+from rdflib.namespace import OWL
 
 ex = Namespace("http://example.org/")
 
 graph = Graph()
 graph.add((ex.subj, ex.pred, ex.obj))
 graph.add((ex.inverse, OWL.inverseOf, ex.pred))
 
+
 len(graph)                              # 2
 (ex.obj, ex.inverse, ex.subj) in graph  # False
 
-graph.inference(reasoner="owlrl") 
+graph.inference(reasoner="owlrl")
 
 len(graph)                              # 359
-(ex.obj, ex.inverse, ex.subj) in graph  # True
+(ex.obj, ex.inverse, ex.subj) in graph
 ```
+
+
 The `reasoner` parameter of `lodkit.Graph.inference` (so far) also takes 
 - "rdfs" for owlrl's [RDFS deductive closure type](https://owl-rl.readthedocs.io/en/latest/RDFSClosure.html#owlrl.RDFSClosure.RDFS_Semantics), 
 - "reasonable" for the [reasonable](https://github.com/gtfierro/reasonable) inference engine and 
 - "allegro" for the [Allegrograph reasoner](https://franz.com/agraph/support/documentation/current/materializer.html) (using the RDFS++ *and* OWL-RL). 
 
 Also the `reasoner` parameter takes `Reasoner` objects directly, see [reasoners.py](https://github.com/lu-pl/lodkit/blob/main/lodkit/reasoners.py).
```

### Comparing `lodkit-0.1.1/lodkit/connections.py` & `lodkit-0.1.2/lodkit/connections.py`

 * *Files identical despite different names*

### Comparing `lodkit-0.1.1/lodkit/graph.py` & `lodkit-0.1.2/lodkit/graph.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """An rdflib.Graph subclass with plugin-based inferencing capability."""
 
-from typing import Optional
+from typing import Optional, Literal
 import rdflib
 
 from lodkit import reasoners
 
 
 _Reasoner = reasoners.Reasoner
-_ReasonerReference = _Reasoner | str
+_ReasonerLiterals = Literal[*reasoners.reasoners.keys()]
+_ReasonerReference = _Reasoner | _ReasonerLiterals
 
 
 class Graph(rdflib.Graph):
     """Subclass of rdflib.Graph with inferencing capability."""
 
     def __init__(self,
                  reasoner: Optional[_ReasonerReference] = None,
@@ -30,14 +31,13 @@
             return reasoner
 
         raise Exception("Reasoner not seizable.")
 
     def inference(self,
                   reasoner: Optional[_ReasonerReference] = None) -> rdflib.Graph:
         """Perform inferencing according to an InferencePlugin."""
-
         # get an actual Reasoner
         _reasoner_reference: _ReasonerReference = reasoner or self.reasoner
         _reasoner: _Reasoner = self._resolve_reasoner(_reasoner_reference)
 
         # call the reasoner
         return _reasoner.inference(self)
```

### Comparing `lodkit-0.1.1/lodkit/importer.py` & `lodkit-0.1.2/lodkit/importer.py`

 * *Files identical despite different names*

### Comparing `lodkit-0.1.1/lodkit/reasoners.py` & `lodkit-0.1.2/lodkit/reasoners.py`

 * *Files identical despite different names*

### Comparing `lodkit-0.1.1/PKG-INFO` & `lodkit-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: lodkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Lukas Plank
 Author-email: lupl@tuta.io
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: agraph-python (>=102.0.0,<103.0.0)
 Requires-Dist: docker (>=6.1.3,<7.0.0)
 Requires-Dist: owlrl (>=6.0.2,<7.0.0)
 Requires-Dist: pycurl (>=7.45.2,<8.0.0)
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
-Requires-Dist: rdflib (>=6.3.2,<7.0.0)
+Requires-Dist: rdflib (==7.0.0)
 Requires-Dist: reasonable (>=0.2.2,<0.3.0)
 Description-Content-Type: text/markdown
 
 ![<img src="lodkit.png" width=50% height=50%>](./lodkit.png)
 
 # LODKit
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
@@ -24,41 +24,47 @@
 LODKit is a collection of Linked Open Data related Python functionalities. 
 
 LODkit (includes|will include)
 - a custom `rdflib.Graph` subclass that is capable of 
   - RDFS and OWL-RL inferencing 
   - Bnode-safe graph merging [todo]
 - a custom importer for loading RDF files as if they where Python modules
+- LOD-specific type definitions
 - [...]
 
 ## Examples
 
 ### lodkit.Graph
 `lodkit.Graph` is an `rdflib.Graph` subclass that is cabable of RFDS and OWL-RL inferencing.
 
 The default plugin for inferencing is the [owlrl](https://github.com/RDFLib/OWL-RL/) native Python inferencing engine. The deductive closure type used for `lodkit.Graph` is [RDFS_OWLRL_Semantics](https://owl-rl.readthedocs.io/en/latest/CombinedClosure.html) which allows for RDFS *and* OWL-RL reasoning.
 
 ```python
-from lodkit import Graph
+from lodkit.graph import Graph
+
 from rdflib import Namespace
+from rdflib.namespace import OWL
 
 ex = Namespace("http://example.org/")
 
 graph = Graph()
 graph.add((ex.subj, ex.pred, ex.obj))
 graph.add((ex.inverse, OWL.inverseOf, ex.pred))
 
+
 len(graph)                              # 2
 (ex.obj, ex.inverse, ex.subj) in graph  # False
 
-graph.inference(reasoner="owlrl") 
+graph.inference(reasoner="owlrl")
 
 len(graph)                              # 359
-(ex.obj, ex.inverse, ex.subj) in graph  # True
+(ex.obj, ex.inverse, ex.subj) in graph
 ```
+
+
 The `reasoner` parameter of `lodkit.Graph.inference` (so far) also takes 
 - "rdfs" for owlrl's [RDFS deductive closure type](https://owl-rl.readthedocs.io/en/latest/RDFSClosure.html#owlrl.RDFSClosure.RDFS_Semantics), 
 - "reasonable" for the [reasonable](https://github.com/gtfierro/reasonable) inference engine and 
 - "allegro" for the [Allegrograph reasoner](https://franz.com/agraph/support/documentation/current/materializer.html) (using the RDFS++ *and* OWL-RL). 
 
 Also the `reasoner` parameter takes `Reasoner` objects directly, see [reasoners.py](https://github.com/lu-pl/lodkit/blob/main/lodkit/reasoners.py).
```

