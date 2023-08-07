# Comparing `tmp/diffusion_curvature-0.0.1.tar.gz` & `tmp/diffusion_curvature-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffusion_curvature-0.0.1.tar", last modified: Thu Aug  3 18:20:09 2023, max compression
+gzip compressed data, was "diffusion_curvature-0.0.2.tar", last modified: Mon Aug  7 22:55:18 2023, max compression
```

## Comparing `diffusion_curvature-0.0.1.tar` & `diffusion_curvature-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxr-x   0 piriac    (1000) piriac    (1000)        0 2023-08-03 18:20:09.582289 diffusion_curvature-0.0.1/
--rw-rw-r--   0 piriac    (1000) piriac    (1000)     1211 2023-08-02 18:37:17.000000 diffusion_curvature-0.0.1/LICENSE
--rw-rw-r--   0 piriac    (1000) piriac    (1000)      111 2023-04-27 10:12:58.000000 diffusion_curvature-0.0.1/MANIFEST.in
--rw-rw-r--   0 piriac    (1000) piriac    (1000)     4250 2023-08-03 18:20:09.582289 diffusion_curvature-0.0.1/PKG-INFO
--rw-rw-r--   0 piriac    (1000) piriac    (1000)     3462 2023-08-02 21:19:00.000000 diffusion_curvature-0.0.1/README.md
-drwxrwxr-x   0 piriac    (1000) piriac    (1000)        0 2023-08-03 18:20:09.582289 diffusion_curvature-0.0.1/diffusion_curvature/
--rw-rw-r--   0 piriac    (1000) piriac    (1000)       22 2023-08-02 21:42:58.000000 diffusion_curvature-0.0.1/diffusion_curvature/__init__.py
--rw-rw-r--   0 piriac    (1000) piriac    (1000)     9437 2023-08-02 21:43:51.000000 diffusion_curvature-0.0.1/diffusion_curvature/_modidx.py
--rw-rw-r--   0 piriac    (1000) piriac    (1000)      142 2023-08-02 18:39:06.000000 diffusion_curvature-0.0.1/diffusion_curvature/core.py
--rw-rw-r--   0 piriac    (1000) piriac    (1000)     7810 2023-08-02 21:42:58.000000 diffusion_curvature-0.0.1/diffusion_curvature/datasets.py
--rw-rw-r--   0 piriac    (1000) piriac    (1000)      760 2023-08-02 21:42:58.000000 diffusion_curvature-0.0.1/diffusion_curvature/distances.py
--rw-rw-r--   0 piriac    (1000) piriac    (1000)     8073 2023-08-02 21:42:58.000000 diffusion_curvature-0.0.1/diffusion_curvature/graphtools.py
--rw-rw-r--   0 piriac    (1000) piriac    (1000)     5648 2023-08-02 21:42:58.000000 diffusion_curvature-0.0.1/diffusion_curvature/kernels.py
-drwxrwxr-x   0 piriac    (1000) piriac    (1000)        0 2023-08-03 18:20:09.582289 diffusion_curvature-0.0.1/diffusion_curvature.egg-info/
--rw-rw-r--   0 piriac    (1000) piriac    (1000)     4250 2023-08-03 18:20:09.000000 diffusion_curvature-0.0.1/diffusion_curvature.egg-info/PKG-INFO
--rw-rw-r--   0 piriac    (1000) piriac    (1000)      574 2023-08-03 18:20:09.000000 diffusion_curvature-0.0.1/diffusion_curvature.egg-info/SOURCES.txt
--rw-rw-r--   0 piriac    (1000) piriac    (1000)        1 2023-08-03 18:20:09.000000 diffusion_curvature-0.0.1/diffusion_curvature.egg-info/dependency_links.txt
--rw-rw-r--   0 piriac    (1000) piriac    (1000)       60 2023-08-03 18:20:09.000000 diffusion_curvature-0.0.1/diffusion_curvature.egg-info/entry_points.txt
--rw-rw-r--   0 piriac    (1000) piriac    (1000)        1 2023-08-02 21:07:25.000000 diffusion_curvature-0.0.1/diffusion_curvature.egg-info/not-zip-safe
--rw-rw-r--   0 piriac    (1000) piriac    (1000)      140 2023-08-03 18:20:09.000000 diffusion_curvature-0.0.1/diffusion_curvature.egg-info/requires.txt
--rw-rw-r--   0 piriac    (1000) piriac    (1000)       20 2023-08-03 18:20:09.000000 diffusion_curvature-0.0.1/diffusion_curvature.egg-info/top_level.txt
--rw-rw-r--   0 piriac    (1000) piriac    (1000)      840 2023-08-02 21:34:31.000000 diffusion_curvature-0.0.1/settings.ini
--rw-rw-r--   0 piriac    (1000) piriac    (1000)       38 2023-08-03 18:20:09.582289 diffusion_curvature-0.0.1/setup.cfg
--rw-rw-r--   0 piriac    (1000) piriac    (1000)     2596 2023-04-27 10:12:58.000000 diffusion_curvature-0.0.1/setup.py
+drwxrwxr-x   0 piriac    (1000) piriac    (1000)        0 2023-08-07 22:55:18.335328 diffusion_curvature-0.0.2/
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)     1211 2023-08-02 18:37:17.000000 diffusion_curvature-0.0.2/LICENSE
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)      111 2023-04-27 10:12:58.000000 diffusion_curvature-0.0.2/MANIFEST.in
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)     7554 2023-08-07 22:55:18.331328 diffusion_curvature-0.0.2/PKG-INFO
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)     6766 2023-08-07 22:43:36.000000 diffusion_curvature-0.0.2/README.md
+drwxrwxr-x   0 piriac    (1000) piriac    (1000)        0 2023-08-07 22:55:18.331328 diffusion_curvature-0.0.2/diffusion_curvature/
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)       22 2023-08-07 22:55:12.000000 diffusion_curvature-0.0.2/diffusion_curvature/__init__.py
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)    14304 2023-08-07 22:55:12.000000 diffusion_curvature-0.0.2/diffusion_curvature/_modidx.py
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)      142 2023-08-02 18:39:06.000000 diffusion_curvature-0.0.2/diffusion_curvature/core.py
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)     7810 2023-08-07 22:55:12.000000 diffusion_curvature-0.0.2/diffusion_curvature/datasets.py
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)      760 2023-08-07 22:55:12.000000 diffusion_curvature-0.0.2/diffusion_curvature/distances.py
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)     8218 2023-08-07 22:55:12.000000 diffusion_curvature-0.0.2/diffusion_curvature/graphtools.py
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)     5648 2023-08-07 22:55:12.000000 diffusion_curvature-0.0.2/diffusion_curvature/kernels.py
+-rw-r--r--   0 piriac    (1000) piriac    (1000)     5364 2023-08-07 22:55:12.000000 diffusion_curvature-0.0.2/diffusion_curvature/manifold_graph.py
+drwxrwxr-x   0 piriac    (1000) piriac    (1000)        0 2023-08-07 22:55:18.331328 diffusion_curvature-0.0.2/diffusion_curvature.egg-info/
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)     7554 2023-08-07 22:55:18.000000 diffusion_curvature-0.0.2/diffusion_curvature.egg-info/PKG-INFO
+-rw-r--r--   0 piriac    (1000) piriac    (1000)      444 2023-01-07 23:16:45.000000 diffusion_curvature-0.0.2/diffusion_curvature.egg-info/SOURCES.sync-conflict-20230806-204323-NXPHTTX.txt
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)      771 2023-08-07 22:55:18.000000 diffusion_curvature-0.0.2/diffusion_curvature.egg-info/SOURCES.txt
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)        1 2023-08-07 22:55:18.000000 diffusion_curvature-0.0.2/diffusion_curvature.egg-info/dependency_links.txt
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)       60 2023-08-07 22:55:18.000000 diffusion_curvature-0.0.2/diffusion_curvature.egg-info/entry_points.txt
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)        1 2023-08-02 21:07:25.000000 diffusion_curvature-0.0.2/diffusion_curvature.egg-info/not-zip-safe
+-rw-r--r--   0 piriac    (1000) piriac    (1000)        7 2023-01-07 23:16:45.000000 diffusion_curvature-0.0.2/diffusion_curvature.egg-info/requires.sync-conflict-20230806-200642-NXPHTTX.txt
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)      140 2023-08-07 22:55:18.000000 diffusion_curvature-0.0.2/diffusion_curvature.egg-info/requires.txt
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)       20 2023-08-07 22:55:18.000000 diffusion_curvature-0.0.2/diffusion_curvature.egg-info/top_level.txt
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)     1085 2023-08-07 22:55:12.000000 diffusion_curvature-0.0.2/settings.ini
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)       38 2023-08-07 22:55:18.335328 diffusion_curvature-0.0.2/setup.cfg
+-rw-rw-r--   0 piriac    (1000) piriac    (1000)     2596 2023-04-27 10:12:58.000000 diffusion_curvature-0.0.2/setup.py
```

### Comparing `diffusion_curvature-0.0.1/LICENSE` & `diffusion_curvature-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `diffusion_curvature-0.0.1/diffusion_curvature/datasets.py` & `diffusion_curvature-0.0.2/diffusion_curvature/datasets.py`

 * *Files identical despite different names*

### Comparing `diffusion_curvature-0.0.1/diffusion_curvature/distances.py` & `diffusion_curvature-0.0.2/diffusion_curvature/distances.py`

 * *Files identical despite different names*

### Comparing `diffusion_curvature-0.0.1/diffusion_curvature/graphtools.py` & `diffusion_curvature-0.0.2/diffusion_curvature/graphtools.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,49 +15,52 @@
 from .distances import *
 import skdim
 class DiffusionCurvature():
     def __init__(
     self,
     t:int, # Number of diffusion steps to use when measuring curvature. TODO: Heuristics
     distance_type = "PHATE",
+    dimest = None, # Dimensionality estimator to use. If None, defaults to KNN with default params
     use_entropy:bool = False, # If true, uses KL Divergence instead of Wasserstein Distances. Faster, seems empirically as good, but less proven.
     **kwargs
     ):
         store_attr()
+        if self.dimest is None:
+            self.dimest = skdim.id.KNN()
 
 # %% ../nbs/Core (graphtools).ipynb 12
 @patch
 def power_diffusion_matrix(self:DiffusionCurvature, G:graphtools.api.Graph, t=None):
         # Raises the diffusion matrix of G to t and stores the result in G.Pt
         if not t:
             t = self.t
         if type(G.P) == np.ndarray:
             G.Pt = np.linalg.matrix_power(G.P, t)
         elif type(G.P) == scipy.sparse.csr_matrix:
             if 'n_landmark' in G.get_params().keys():
-                # the graph was built with landmarking. We'll power the diffusion matrix that way
+                # the graph was built with landmarking we'll power the diffusion matrix that way
                 G.Pt = scipy.sparse.csr_matrix(
                     G.transitions @ np.linalg.matrix_power(G.landmark_op,t) @ G.transitions.T
                 )
             else:
                 G.Pt = G.P ** t
         else:
             raise NotImplementedError("Unknown Matrix Type")
         return G
 
-# %% ../nbs/Core (graphtools).ipynb 17
+# %% ../nbs/Core (graphtools).ipynb 18
 @patch
 def distances(self:DiffusionCurvature, G):
         if self.distance_type == "PHATE":
             G = phate_distances(G)
         else:
            raise NotImplementedError(f"No distance with name {self.distance_type}")
         return G
 
-# %% ../nbs/Core (graphtools).ipynb 22
+# %% ../nbs/Core (graphtools).ipynb 23
 @patch
 def wasserstein_spread_of_diffusion(self:DiffusionCurvature, G:graphtools.graphs.DataGraph, idx = None):
         """
         Returns how "spread out" each diffusion is, with wasserstein distance"
         Presumes that the manifold distances have been separately calculated
         If idx is passed, only computes wsd at that index
         """
@@ -71,23 +74,23 @@
         else:
             Pt = G.Pt.toarray()
         if idx is None:
             return np.sum(G.D * Pt, axis=1)
         else:
             return np.sum(G.D[idx]* Pt[idx])
 
-# %% ../nbs/Core (graphtools).ipynb 26
+# %% ../nbs/Core (graphtools).ipynb 27
 def get_graph_type(G):
     tt = str(type(G)).split('.')[-1][:3].lower()
     # TODO: Support for MNN graphs
     if tt == 'mnn': raise NotImplementedError("MNN Graphs require manual indices. These are not yet supported by our graph flattener.")
     if tt in ['knn']: return tt
     else: return 'exact'
 
-# %% ../nbs/Core (graphtools).ipynb 31
+# %% ../nbs/Core (graphtools).ipynb 32
 @patch
 def flattened_facsimile_of_graph(self:DiffusionCurvature, G:graphtools.graphs.DataGraph, dimension):
         """
         Constructs a flat graph, hewn from uniform random noise of the supplied dimension.
         Calculates the powered diffusion matrix on this graph.
         """
         noise = np.concatenate([np.zeros((1,dimension)), 2*np.random.rand(G.K.shape[0]-1,dimension)-1])
@@ -120,15 +123,15 @@
             n_jobs = found_keys['n_jobs'],
             graphtype = get_graph_type(G),
         )
         G_flat = self.power_diffusion_matrix(G_flat, t = self.t)
         # TODO: This is a tad wasteful. We only need the center diffusion powered.
         return G_flat
 
-# %% ../nbs/Core (graphtools).ipynb 34
+# %% ../nbs/Core (graphtools).ipynb 35
 @patch
 def entropy_of_diffusion(self:DiffusionCurvature, G:graphtools.graphs.DataGraph, idx=None):
         """
         Returns the pointwise entropy of diffusion from the powered diffusion matrix in the inpiut 
         """
         assert G.Pt is not None
         # TODO: Entropy may be compatible with scipy.sparse matrices
@@ -137,55 +140,52 @@
         else:
             Pt = G.Pt.toarray()
         if idx is None:
             return entropy(Pt, axis=1)
         else:
             return entropy(Pt[idx])
 
-# %% ../nbs/Core (graphtools).ipynb 36
+# %% ../nbs/Core (graphtools).ipynb 38
 @patch
 def curvature(self:DiffusionCurvature, 
     G:graphtools.graphs.DataGraph, # A graphtools graph to compute the curvature of
     t=None,  # The number of steps within the random walks. Corresponds to how local/global the curvature estimate is.
-    dimension:int = None,  # If supplied, the global manifold dimension. If not supplied, estimates the local dimension of each point.
+    dimension = None,  # If supplied, the intrinsic dimension of the manifold, either a list of the intrinsic dimension per point or an int of the global intrinsic dimension. If not supplied, estimates the local dimension of each point on the manifold using the estimator passed to DiffusionCurvature.
     ):
     """
     Computes diffusion curvature of input graph. Stores it in G.ks
     """
     if t is None:
         t = self.t
     G = self.power_diffusion_matrix(G,t)
     G = self.distances(G)
     spreads_on_manifold = self.wasserstein_spread_of_diffusion(G) if not self.use_entropy else self.entropy_of_diffusion(G)
     # Create flattened version of manifold and compute stuff
-    if dimension is not None:
-        # dimension was supplied as an int. There's a single global dimension. Our life is easy.
-        G_flat = self.flattened_facsimile_of_graph(G, dimension=dimension)
-        G_flat = self.power_diffusion_matrix(G_flat,t)
-        G_flat = self.distances(G_flat)
-        spreads_on_flat = self.wasserstein_spread_of_diffusion(G_flat, idx=0) if not self.use_entropy else self.entropy_of_diffusion(G, idx=0)
-        G.ks = 1 - (spreads_on_manifold/spreads_on_flat)
-    else:
-        # compute local dimension of each point, 
-        # TODO: Currently this requires underlying points.
+    if dimension is None: # The dimension wasn't supplied; we'll estimate it pointwise
         print("estimating local dimension of each point... may take a while")
-        ldims = skdim.id.DANCo().fit_pw(G.data,
+        ldims = self.dimest.fit_pw(G.data,
                             n_neighbors = 100,
                             n_jobs = 1)
-        dims_per_point = np.round(ldims.dimension_pw_)
-        unique_dims = set(dims_per_point)
-        unique_flats = {}
-        for d in unique_dims:
-            G_flat = self.flattened_facsimile_of_graph(G, dimension=d)
-            G_flat = self.power_diffusion_matrix(G_flat,t)
-            G_flat = self.distances(G_flat)
-            unique_flats[d] = self.wasserstein_spread_of_diffusion(G_flat, idx=0) if not self.use_entropy else self.entropy_of_diffusion(G, idx=0)
-        divided_pts = np.array([spreads_on_manifold/unique_flats[localdim] for localdim in dims_per_point])
-        G.ks = 1 - divided_pts
+        dims_per_point = np.round(ldims.dimension_pw_).astype(int)
+    else: # the dimension *was* supplied, but it may be either a single global dimension or a local dimension for each point
+        if isinstance(dimension, int):
+            dims_per_point = np.ones(G.P.shape[0], dtype=int)*dimension
+        else:
+            dims_per_point = dimension
+    # TODO: Currently this requires underlying points.
+    unique_dims = set(dims_per_point)
+    unique_flats = {}
+    for d in unique_dims:
+        G_flat = self.flattened_facsimile_of_graph(G, dimension=d)
+        G_flat = self.power_diffusion_matrix(G_flat,t)
+        G_flat = self.distances(G_flat)
+        unique_flats[d] = self.wasserstein_spread_of_diffusion(G_flat, idx=0) if not self.use_entropy else self.entropy_of_diffusion(G, idx=0)
+    divided_pts = np.array([spreads_on_manifold[idx]/unique_flats[localdim] for idx, localdim in enumerate(dims_per_point)])
+    G.ks = 1 - divided_pts
     return G
 
-# %% ../nbs/Core (graphtools).ipynb 39
+# %% ../nbs/Core (graphtools).ipynb 45
 from .kernels import plot_3d
 def plot_manifold_curvature(G, title = None):
     X = G.data
     ks = G.ks
     plot_3d(X, ks, colorbar=True, title=title)
```

### Comparing `diffusion_curvature-0.0.1/diffusion_curvature/kernels.py` & `diffusion_curvature-0.0.2/diffusion_curvature/kernels.py`

 * *Files identical despite different names*

### Comparing `diffusion_curvature-0.0.1/diffusion_curvature.egg-info/SOURCES.txt` & `diffusion_curvature-0.0.2/diffusion_curvature.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 diffusion_curvature/__init__.py
 diffusion_curvature/_modidx.py
 diffusion_curvature/core.py
 diffusion_curvature/datasets.py
 diffusion_curvature/distances.py
 diffusion_curvature/graphtools.py
 diffusion_curvature/kernels.py
+diffusion_curvature/manifold_graph.py
 diffusion_curvature.egg-info/PKG-INFO
+diffusion_curvature.egg-info/SOURCES.sync-conflict-20230806-204323-NXPHTTX.txt
 diffusion_curvature.egg-info/SOURCES.txt
 diffusion_curvature.egg-info/dependency_links.txt
 diffusion_curvature.egg-info/entry_points.txt
 diffusion_curvature.egg-info/not-zip-safe
+diffusion_curvature.egg-info/requires.sync-conflict-20230806-200642-NXPHTTX.txt
 diffusion_curvature.egg-info/requires.txt
 diffusion_curvature.egg-info/top_level.txt
```

### Comparing `diffusion_curvature-0.0.1/settings.ini` & `diffusion_curvature-0.0.2/settings.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 [DEFAULT]
 repo = diffusion_curvature
-lib_name = %(repo)s
-version = 0.0.1
+lib_name = diffusion_curvature
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = diffusion_curvature
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
 branch = main
 custom_sidebar = False
-doc_host = https://%(user)s.github.io
-doc_baseurl = /%(repo)s
-git_url = https://github.com/%(user)s/%(repo)s
-title = %(lib_name)s
+doc_host = https://professorwug.github.io
+doc_baseurl = /diffusion_curvature
+git_url = https://github.com/professorwug/diffusion_curvature
+title = diffusion_curvature
 audience = Developers
 author = Kincaid
 author_email = dev@riddle.press
-copyright = 2023 onwards, %(author)s
+copyright = 2023 onwards, Kincaid
 description = Fast, pointwise graph curvature
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = professorwug
-requirements = numpy pandas scikit-learn scipy sympy numba tqdm rich typer matplotlib plotly nbdev>=2.3.12 pyyaml graphtools scikit-dimension 
+requirements = numpy pandas scikit-learn scipy sympy numba tqdm rich typer matplotlib plotly nbdev>=2.3.12 pyyaml graphtools scikit-dimension
+conda_requirements = 
+pip_requirements = 
+conda_user = riddlelabs
 dev_requirements = nbdev
+readme_nb = index.ipynb
+allowed_metadata_keys = 
+allowed_cell_metadata_keys = 
+jupyter_hooks = True
+clean_ids = True
+clear_all = False
```

### Comparing `diffusion_curvature-0.0.1/setup.py` & `diffusion_curvature-0.0.2/setup.py`

 * *Files identical despite different names*

