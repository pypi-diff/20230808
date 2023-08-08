# Comparing `tmp/graphpro-0.3.6.tar.gz` & `tmp/graphpro-0.4.0.tar.gz`

## Comparing `graphpro-0.3.6.tar` & `graphpro-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,19 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 graphpro-0.3.6/pytest.ini
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 graphpro-0.3.6/requirements.txt
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 graphpro-0.3.6/.github/workflows/python-app.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 graphpro-0.3.6/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 graphpro-0.3.6/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 graphpro-0.3.6/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 graphpro-0.3.6/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 graphpro-0.3.6/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 graphpro-0.3.6/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 graphpro-0.3.6/src/graphpro/__init__.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 graphpro-0.3.6/src/graphpro/graph.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 graphpro-0.3.6/src/graphpro/graphgen.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 graphpro-0.3.6/src/graphpro/model.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 graphpro-0.3.6/src/graphpro/util/residues.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 graphpro-0.3.6/test/graphpro/graph_test.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 graphpro-0.3.6/test/graphpro/graphgen_test.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 graphpro-0.3.6/test/graphpro/model_test.py
--rw-r--r--   0        0        0   280989 2020-02-02 00:00:00.000000 graphpro-0.3.6/test/testdata/5htc.pdb
--rw-r--r--   0        0        0  3998279 2020-02-02 00:00:00.000000 graphpro-0.3.6/test/testdata/hetnam.pdb
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 graphpro-0.3.6/.gitignore
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 graphpro-0.3.6/README.md
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 graphpro-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 graphpro-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 graphpro-0.4.0/pytest.ini
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 graphpro-0.4.0/requirements.txt
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 graphpro-0.4.0/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 graphpro-0.4.0/src/graphpro/__init__.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 graphpro-0.4.0/src/graphpro/collection.py
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 graphpro-0.4.0/src/graphpro/graph.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 graphpro-0.4.0/src/graphpro/graphgen.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 graphpro-0.4.0/src/graphpro/model.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 graphpro-0.4.0/src/graphpro/util/residues.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 graphpro-0.4.0/test/graphpro/collection_test.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 graphpro-0.4.0/test/graphpro/graph_test.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 graphpro-0.4.0/test/graphpro/graphgen_test.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 graphpro-0.4.0/test/graphpro/model_test.py
+-rw-r--r--   0        0        0   280989 2020-02-02 00:00:00.000000 graphpro-0.4.0/test/testdata/5htc.pdb
+-rw-r--r--   0        0        0  3998279 2020-02-02 00:00:00.000000 graphpro-0.4.0/test/testdata/hetnam.pdb
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 graphpro-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 graphpro-0.4.0/README.md
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 graphpro-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 graphpro-0.4.0/PKG-INFO
```

### Comparing `graphpro-0.3.6/.github/workflows/python-app.yml` & `graphpro-0.4.0/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.6/src/graphpro/graph.py` & `graphpro-0.4.0/src/graphpro/graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 
         self.name = name
         self.distances = distances
         self.positions = positions
         self._n_attr = {i: {"resid": res_attr['resid'], "resname": one_letter_res(res_attr['resname'])} for i, res_attr in enumerate(res_map)}
         self._resid_to_node = {res_attr['resid']: i for i, res_attr in enumerate(res_map)} 
 
+    def __eq__(self, other):
+        """Compare two graphs for equality"""
+        #TODO: may need to compare more than the distances
+        return (self.distances == other.distances).any()
+
     def node_attr(self, node_id: int):
         return self._n_attr.get(node_id)
     
     def node_attr_add(self, node_id: int, attribute_name: str, attribute: any):
         """Adds a specific attribute to a noode in the graph"""
         attrs = self.node_attr(node_id)
         if attrs:
```

### Comparing `graphpro-0.3.6/src/graphpro/graphgen.py` & `graphpro-0.4.0/src/graphpro/graphgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         pass
 
 
 class ContactMap(RepresentationMethod):
     def __init__(self, cutoff, chain=None):
         self.cutoff = cutoff
         self.chain = chain
-    
+   
     def generate(self, ag, name: str):
         ca_position = ag.c_alphas_positions(self.chain)
         dist = distance.squareform(distance.pdist(ca_position))
         dist[dist > self.cutoff] = 0
         return Graph(name, dist, ca_position, ag.c_alphas_residues(self.chain))
```

### Comparing `graphpro-0.3.6/src/graphpro/model.py` & `graphpro-0.4.0/src/graphpro/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,20 +19,20 @@
         return self.u.atoms.n_atoms
 
     def _c_alphas(self, chain=None):
         chain_sel = ''
         if chain != None:
             chain_sel = f'chainid {chain} and '
         atoms = self.u.select_atoms(chain_sel + 'name CA')
-        
+       
         # select only residues with large occupancy
         atoms_filtered = [ag[ag.occupancies.tolist().index(max(ag.occupancies))] for ag in atoms.groupby('resnums').values()] 
         if len(atoms_filtered) == 0:
             return atoms
-        elif len(atoms_filtered) == 1:
+        if len(atoms_filtered) == 1:
             return atoms
         else:
             return reduce(lambda a,b: a+b, atoms_filtered)
 
     def c_alphas_positions(self, chain = None):
          return self._c_alphas(chain).positions
```

### Comparing `graphpro-0.3.6/test/graphpro/graph_test.py` & `graphpro-0.4.0/test/graphpro/graph_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import os
+
 import MDAnalysis as mda
 import numpy as np
 import networkx as nx
-import os
+
 
 from graphpro import md_analisys
 from graphpro.graph import Graph
 from graphpro.graphgen import ContactMap
 
 DISTANCES = np.array([[4,2],[2,4]])
 POSITIONS_3D = np.array([[1,2,3], [-1,-2,-3]])
```

### Comparing `graphpro-0.3.6/test/graphpro/graphgen_test.py` & `graphpro-0.4.0/test/graphpro/graphgen_test.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.6/test/testdata/5htc.pdb` & `graphpro-0.4.0/test/testdata/5htc.pdb`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.6/test/testdata/hetnam.pdb` & `graphpro-0.4.0/test/testdata/hetnam.pdb`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.6/pyproject.toml` & `graphpro-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "graphpro"
-version = "0.3.6"
+version = "0.4.0"
 authors = [
   { name="Pegerto Fernandez", email="pegerto@gmail.com" },
 ]
 description = "A python module to handle graph protein data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

