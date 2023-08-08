# Comparing `tmp/pankmer-0.15.1.tar.gz` & `tmp/pankmer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+gzip compressed data, was "pankmer-0.9.0.tar", last modified: Sat Feb  4 08:39:36 2023, max compression
```

## Comparing `pankmer-0.15.1.tar` & `pankmer-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 pankmer-0.15.1/rust/Cargo.toml
--rw-r--r--   0      501       20     2636 2023-08-07 22:20:33.000000 pankmer-0.15.1/rust/src/adj_matrix.rs
--rw-r--r--   0      501       20     3544 2023-07-14 17:37:45.000000 pankmer-0.15.1/rust/src/decompose_kmers.rs
--rw-r--r--   0      501       20    14136 2023-08-07 22:20:33.000000 pankmer-0.15.1/rust/src/get_kmers.rs
--rw-r--r--   0      501       20     4070 2023-08-07 22:20:33.000000 pankmer-0.15.1/rust/src/helpers.rs
--rw-r--r--   0      501       20     9199 2023-07-27 20:42:27.000000 pankmer-0.15.1/rust/src/lib.rs
--rw-r--r--   0      501       20     3946 2023-07-27 20:25:40.000000 pankmer-0.15.1/rust/src/measure.rs
--rw-r--r--   0      501       20     2667 2023-07-14 17:37:45.000000 pankmer-0.15.1/rust/src/mem_blocks.rs
--rw-r--r--   0      501       20     4779 2023-07-27 20:42:27.000000 pankmer-0.15.1/rust/src/metadata.rs
--rw-r--r--   0      501       20    14813 2023-08-07 22:20:33.000000 pankmer-0.15.1/rust/src/pkidx.rs
--rw-r--r--   0      501       20    11767 2023-08-07 22:20:33.000000 pankmer-0.15.1/rust/src/subset_index.rs
--rw-r--r--   0      501       20     1160 2023-08-08 02:53:42.000000 pankmer-0.15.1/pyproject.toml
--rw-r--r--   0      501       20    32404 2023-08-08 02:39:19.000000 pankmer-0.15.1/rust/Cargo.lock
--rw-r--r--   0      501       20     1313 2023-07-27 20:25:40.000000 pankmer-0.15.1/src/pankmer/parse_genomes_input.py
--rw-r--r--   0      501       20     8227 2023-08-07 22:20:33.000000 pankmer-0.15.1/src/pankmer/tree.py
--rw-r--r--   0      501       20     6157 2023-07-27 20:42:27.000000 pankmer-0.15.1/src/pankmer/collect.py
--rw-r--r--   0      501       20       58 2023-06-01 18:28:18.000000 pankmer-0.15.1/src/pankmer/version.py
--rw-r--r--   0      501       20      583 2023-07-27 20:42:27.000000 pankmer-0.15.1/src/pankmer/env.py
--rw-r--r--   0      501       20     3699 2023-08-07 22:20:33.000000 pankmer-0.15.1/src/pankmer/clustermap.py
--rw-r--r--   0      501       20    18607 2023-08-07 22:20:33.000000 pankmer-0.15.1/src/pankmer/anchor.py
--rw-r--r--   0      501       20      214 2023-06-01 18:28:18.000000 pankmer-0.15.1/src/pankmer/get_lower_bound.py
--rw-r--r--   0      501       20     6288 2023-07-27 20:42:27.000000 pankmer-0.15.1/src/pankmer/download.py
--rw-r--r--   0      501       20    33386 2023-07-27 20:42:27.000000 pankmer-0.15.1/src/pankmer/datasets.py
--rw-r--r--   0      501       20      337 2023-08-08 02:53:42.000000 pankmer-0.15.1/src/pankmer/__init__.py
--rw-r--r--   0      501       20     1683 2023-07-27 20:42:27.000000 pankmer-0.15.1/src/pankmer/adjacency_matrix.py
--rw-r--r--   0      501       20     1801 2023-07-27 20:42:27.000000 pankmer-0.15.1/src/pankmer/upset.py
--rw-r--r--   0      501       20      603 2023-07-27 20:25:40.000000 pankmer-0.15.1/src/pankmer/subset.py
--rw-r--r--   0      501       20      947 2023-07-14 17:37:45.000000 pankmer-0.15.1/src/pankmer/gzip_agnostic_open.py
--rw-r--r--   0      501       20     3278 2023-08-07 22:20:33.000000 pankmer-0.15.1/src/pankmer/anchormap.py
--rw-r--r--   0      501       20      772 2023-07-27 20:42:27.000000 pankmer-0.15.1/src/pankmer/count.py
--rw-r--r--   0      501       20     2617 2023-07-27 20:25:40.000000 pankmer-0.15.1/src/pankmer/dryrun.py
--rw-r--r--   0      501       20    63455 2023-08-08 02:53:42.000000 pankmer-0.15.1/src/pankmer/pankmer.py
--rw-r--r--   0      501       20     8366 2023-08-07 22:20:33.000000 pankmer-0.15.1/README.md
--rw-r--r--   0        0        0     9377 1970-01-01 00:00:00.000000 pankmer-0.15.1/PKG-INFO
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-02-04 08:39:36.228165 pankmer-0.9.0/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1582 2023-02-04 07:58:07.000000 pankmer-0.9.0/LICENSE
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5077 2023-02-04 08:39:36.227417 pankmer-0.9.0/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4331 2023-02-04 07:49:14.000000 pankmer-0.9.0/README.md
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-02-04 08:39:36.187702 pankmer-0.9.0/pankmer.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5077 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      638 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       49 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       68 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        8 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/top_level.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1174 2023-02-04 08:27:05.000000 pankmer-0.9.0/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-02-04 08:39:36.228268 pankmer-0.9.0/setup.cfg
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      450 2023-01-16 17:12:04.000000 pankmer-0.9.0/setup.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-02-04 08:39:36.180795 pankmer-0.9.0/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-02-04 08:39:36.218482 pankmer-0.9.0/src/pankmer/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      257 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1832 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/adjacency_matrix.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3009 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/clustermap.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      907 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/count.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1493 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/download.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    17939 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/env.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      213 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/get_lower_bound.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      364 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/gzip_agnostic_open.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    13154 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/index.pyx
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    46421 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/pankmer.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      355 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/populate.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    17507 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/reg_coverage.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6062 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/tree.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       81 2023-02-04 08:26:57.000000 pankmer-0.9.0/src/pankmer/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-02-04 08:39:36.224115 pankmer-0.9.0/test/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4278 2023-01-16 17:12:04.000000 pankmer-0.9.0/test/test_compiled.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6969 2023-02-04 07:49:15.000000 pankmer-0.9.0/test/test_slow.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2255 2023-01-16 17:12:04.000000 pankmer-0.9.0/test/test_tree.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pankmer-0.15.1/pyproject.toml` & `pankmer-0.9.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 [build-system]
-requires = ["maturin>=1.1,<2.0"]
-build-backend = "maturin"
+requires = ["setuptools", "wheel", "Cython", "numpy"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "pankmer"
-version = "0.15.1" # Don't forget to match with Cargo.toml and docs/source/conf.py
+version = "0.9.0" # Don't forget to match with version.py and docs/source/conf.py
 authors = [
   { name="Anthony Aylward", email="aaylward@salk.edu" },
   { name="Semar Petrus" },
   { name="Allen Mamerto" },
   { name="Nolan Hartwick" },
 ]
 description = "Generate a PanGenome given a set of genomes"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.8,<3.11"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: BSD License",
 ]
 dependencies = [
-    "biopython",
+    "biopython<=1.79",
     "gff2bed",
     "newick",
+    "pandas",
     "pyfaidx",
     "scipy",
     "seaborn",
-    "urllib3",
-    "upsetplot",
-    "pybedtools",
-    "more-itertools"
+    "urllib3"
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/salk-tm/pankmer"
 "Documentation" = "https://salk-tm.gitlab.io/pankmer"
 
 [project.scripts]
 pankmer = "pankmer.pankmer:main"
 
-[tool.maturin]
-module-name = "pankmer.index"
+[tool.setuptools]
+package-dir = {pankmer="src/pankmer"}
```

### Comparing `pankmer-0.15.1/src/pankmer/tree.py` & `pankmer-0.9.0/src/pankmer/tree.py`

 * *Files 24% similar despite different names*

```diff
@@ -65,75 +65,14 @@
 
     mat = adj_matrix.to_numpy()
     kmers_per_col = get_kmers_per_col(mat)
     overlap = mat / np.minimum(kmers_per_col, np.transpose(kmers_per_col))
     return pd.DataFrame(overlap, index=adj_matrix.index, columns=adj_matrix.columns)
 
 
-def adj_to_qv(adj_matrix, k=31):
-    """Convert a raw adjacency matrix to QV values
-    
-    Parameters
-    ----------
-    adj_matrix
-        pandas data frame containing the adjacency matrix
-    
-    Returns
-    -------
-    DataFrame
-        pandas data framed containing the QV matrix
-    """
-
-    mat = adj_matrix.to_numpy()
-    kmers_per_col = get_kmers_per_col(mat)
-    qv = -10*np.log10(1 - (mat / kmers_per_col)**(1/k) + np.identity(len(adj_matrix.index)))
-    return pd.DataFrame(qv, index=adj_matrix.index, columns=adj_matrix.columns)
-
-
-def adj_to_qv_symmetric(adj_matrix, k=31):
-    """Convert a raw adjacency matrix to symmetric QV values
-    
-    Parameters
-    ----------
-    adj_matrix
-        pandas data frame containing the adjacency matrix
-    
-    Returns
-    -------
-    DataFrame
-        pandas data framed containing the symmetric QV matrix
-    """
-
-    mat = adj_matrix.to_numpy()
-    kmers_per_col = get_kmers_per_col(mat)
-    qv_sym = -10*np.log10(1 - (mat / (kmers_per_col + np.transpose(kmers_per_col) - mat))**(1/k) + np.identity(len(adj_matrix.index)))
-    return pd.DataFrame(qv_sym, index=adj_matrix.index, columns=adj_matrix.columns)
-
-
-def adj_to_ani(adj_matrix, k=31):
-    """Convert a raw adjacency matrix to average nucleotide identity (ANI) values
-    
-    Parameters
-    ----------
-    adj_matrix
-        pandas data frame containing the adjacency matrix
-    
-    Returns
-    -------
-    DataFrame
-        pandas data framed containing the ANI matrix
-    """
-
-    mat = adj_matrix.to_numpy()
-    kmers_per_col = get_kmers_per_col(mat)
-    jaccard = mat / (kmers_per_col + np.transpose(kmers_per_col) - mat)
-    ani = 1 +  1 / k * np.log(2 * jaccard / (1 + jaccard))
-    return pd.DataFrame(ani, index=adj_matrix.index, columns=adj_matrix.columns)
-
-
 def compute_linkage_matrix(adj_matrix, method='complete', optimal_ordering=True):
     """Compute a linkage matrix defining a hierarchical clustering
     
     Parameters
     ---------
     adj_matrix
         pandas data frame containing the adjacency matrix
@@ -219,38 +158,28 @@
     adj_matrix
         a pandas data frame containing an adjacency matrix
     newick : bool
         if True, print a NEWICK-formatted tree. Otherwise, print a linkage
         matrix
     metric : str
         similarity metric to use for clustering. must be "intersection",
-        "jaccard", "overlap", "qv" or "qv_symmetric"
+        "jaccard", or "overlap"
     method : str
         linkage algorithm for hierarchical clustering. See
         `scipy.cluster.hierarchy.linkage` for details.
     optimal_ordering : bool
         If True, the linkage matrix will be reordered so that the distance
         between successive leaves is minimal. See
         `scipy.cluster.hierarchy.linkage`
-    transformed_matrix
-        path to write jaccard/overlap matrix, or None
     """
     
     if metric == 'jaccard':
         adj_matrix = adj_to_jaccard(adj_matrix)
     elif metric == 'overlap':
         adj_matrix = adj_to_overlap(adj_matrix)
-    elif metric == 'qv':
-        adj_matrix = adj_to_qv(adj_matrix)
-    elif metric == 'qv_symmetric':
-        adj_matrix = adj_to_qv_symmetric(adj_matrix)
-    elif metric == 'ani':
-        adj_matrix = adj_to_ani(adj_matrix)
-    else:
-        raise RuntimeError('invalid metric')
     if transformed_matrix:
         with open(transformed_matrix, 'w') as f:
             adj_matrix.to_csv(f)
     linkage_matrix = compute_linkage_matrix(adj_matrix, method=method,
                                      optimal_ordering=optimal_ordering)
     df = linkage_df(linkage_matrix)
     if newick:
```

### Comparing `pankmer-0.15.1/src/pankmer/clustermap.py` & `pankmer-0.9.0/src/pankmer/clustermap.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import pandas as pd
 import seaborn as sns
-from pankmer.tree import (adj_to_jaccard, adj_to_overlap, compute_linkage_matrix,
-                          adj_to_qv, adj_to_qv_symmetric, adj_to_ani)
+from pankmer.tree import adj_to_jaccard, adj_to_overlap, compute_linkage_matrix
 
 def clustermap(adj_matrix, output: str, cmap: str = 'mako_r',
                width: float = 7.0, height: float = 7.0,
                metric='intersection', method='complete',
                optimal_ordering: bool = True, square: bool = True,
-               heatmap_tick_pos='right', cbar_tick_pos='left',
-               dendrogram_ratio: float = 0.2, dendrogram_spacer:float = 0.1):
+               heatmap_tick_pos='right', cbar_tick_pos='left'):
     """Plot a clustered heatmap of genome similarity values
 
     Parameters
     ----------
     adj_matrix : DataFrame
         a Pandas data frame representing the adjacency matrix
     output : str
@@ -20,51 +18,39 @@
     cmap : str
         color map for the heatmap
     width : float
         width of the plot in inches
     height : float
         height of the plot in inches
     metric : str
-        similarity metric to use for clustering. must be "intersection",
-        "jaccard", "overlap", "qv" or "qv_symmetric"
+        similarity metric to use, chosen from "intersection", "jaccard", or
+        "overlap"
     method : str
         linkage algorithm for hierarchical clustering. See
         `scipy.cluster.hierarchy.linkage` for details.
     optimal_ordering : bool
         If True, the linkage matrix will be reordered so that the distance
         between successive leaves is minimal. See
         `scipy.cluster.hierarchy.linkage`
     square : bool
         If True, the heatmap will be drawn square. This may force the figure
         dimensions to be altered slightly
     cbar_tick_pos : str
         Position of color bar ticks. Must be "left" or "right" [left]
-    dendrogram_ratio : float
-        Fraction of plot width used for dendrogram [0.2]
-    dendrogram_spacer : float
-        Fraction of plot width used as spacer between dendrogram and heatmap [0.1]
     """
     
     if metric == 'jaccard':
         adj_matrix = adj_to_jaccard(adj_matrix)
     elif metric == 'overlap':
         adj_matrix = adj_to_overlap(adj_matrix)
-    elif metric == 'qv':
-        adj_matrix = adj_to_qv(adj_matrix)
-    elif metric == 'qv_symmetric':
-        adj_matrix = adj_to_qv_symmetric(adj_matrix)
-    elif metric == 'ani':
-        adj_matrix = adj_to_ani(adj_matrix)
-    else:
-        raise RuntimeError('invalid metric')
     linkage = compute_linkage_matrix(adj_matrix, method=method,
                                      optimal_ordering=optimal_ordering)
     ax = sns.clustermap(adj_matrix, cmap=cmap, figsize=(width, height),
                         row_linkage=linkage, col_linkage=linkage,
-                        xticklabels=False, dendrogram_ratio=(dendrogram_ratio,0))
+                        xticklabels=False, dendrogram_ratio=(.2,0))
     if square:
         ax.ax_heatmap.set_aspect("equal")
     ax.ax_col_dendrogram.set_visible(False)
     ax_hm_pos = ax.ax_heatmap.get_position()
     ax_row_pos = ax.ax_row_dendrogram.get_position()
     match heatmap_tick_pos:
         case 'left':
@@ -72,11 +58,11 @@
                                         ax_hm_pos.width, ax_hm_pos.height])
         case 'right':
             ax.ax_heatmap.set_position([ax_hm_pos.x0-.1, ax_hm_pos.y0,
                                         ax_hm_pos.width, ax_hm_pos.height])
     ax.ax_heatmap.yaxis.set_ticks_position(heatmap_tick_pos)
     ax.ax_heatmap.set_yticklabels(ax.ax_heatmap.get_yticklabels(), rotation=0)
     ax.ax_row_dendrogram.set_position([ax_row_pos.x0, ax_hm_pos.y0, 
-                                       ax_row_pos.width-dendrogram_spacer, ax_hm_pos.height])
+                                       ax_row_pos.width-.1, ax_hm_pos.height])
     ax.ax_cbar.set_position([.97, ax_hm_pos.y0, .03, ax_hm_pos.height])
     ax.ax_cbar.yaxis.set_ticks_position(cbar_tick_pos)
     ax.savefig(output)
```

### Comparing `pankmer-0.15.1/src/pankmer/anchor.py` & `pankmer-0.9.0/src/pankmer/reg_coverage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #===============================================================================
-# anchor.py
+# reg_coverage.py
 #===============================================================================
 
-"""High-level functions for genome anchoring analysis"""
+"""High-level functions for k-mer coverage analysis"""
 
 
 
 # Imports ======================================================================
 
 import gzip
 import matplotlib.pyplot as plt
@@ -112,35 +112,35 @@
     """
 
     parsed_features = gff2bed.parse(gff, type=type)
     return {attr_vals[attr]: (seqid, start, end)
         for seqid, start, end, _, attr_vals in parsed_features}
 
 
-def generate_anchoring_values(chrom, start, end, *anchor_dicts, summary_func=mean):
+def generate_coverage_values(chrom, start, end, *regcov_dicts, summary_func=mean):
     for position, *values in zip(range(start, end + 1),
-        *(next(iter(anchor_dict[chrom].values())) for anchor_dict in anchor_dicts)):
+        *(next(iter(regcov_dict[chrom].values())) for regcov_dict in regcov_dicts)):
         yield chrom, position-1, position, *(summary_func(v) for v in values)
 
 
-def anchor_region(*pk_results, ref, coords, summary_func=mean, output_file=None,
+def reg_coverage(*pk_results, ref, coords, summary_func=mean, output_file=None,
                  bgzip: bool = False, genes=None, flank: int = 0,
                  processes: int = 1):
-    """Generate k-mer conservation levels across the input region
+    """Generate k-mer coverage levels across the input region
 
     Parameters
     ----------
     pk_results
         a PKResults object
     ref: str
         path to a reference genome in BGZIP compressed FASTA format
     coords: str
         genomic coordinates formatted as ctg:start-end
     summary_func
-        function for summarizing the conservation of a kmer across genomes
+        function for summarizing the coverage value of a kmer across genomes
         in the index. The default is statistics.mean
     output_file
         filename or file object to write to
     bgzip: bool
         if True, output_file will be block compressed
     genes: str
         path to gff3 file containing gnes
@@ -159,32 +159,32 @@
         contig, start, end = attr_to_coords(genes)[coords]
     else:
         contig, start, end = parse_coords(coords)
     start -= flank
     end += flank
     for result in pk_results:
         result.threads = processes
-    anchor_dicts = (result.get_collapsed_regional_scores(ref, {contig: [[start, end]]})
+    regcov_dicts = (result.get_collapsed_regional_scores(ref, {contig: [[start, end]]})
                     for result in  pk_results)
     if output_file:
         with (output_file if isinstance(output_file, (BgzfWriter, IOBase))
               else (BgzfWriter if bgzip else open)(output_file, 'wb')) as f:
-            for cg, st, ed, *vs in generate_anchoring_values(
-                contig, start, end, *anchor_dicts, summary_func=summary_func
+            for cg, st, ed, *vs in generate_coverage_values(
+                contig, start, end, *regcov_dicts, summary_func=summary_func
             ):
                 f.write(('\t'.join(str(x) for x in (cg, st, ed, *vs))+'\n').encode())
-    return generate_anchoring_values(contig, start, end, *anchor_dicts,
+    return generate_coverage_values(contig, start, end, *regcov_dicts,
                                         summary_func=summary_func)
 
 
 def check_for_bgzip(reference: str):
     try:
         BgzfReader(reference)
     except ValueError:
-        raise RuntimeError('Input FASTA must be BGZIP compressed')
+        raise RuntimeError('Input FASTA must be BGZIP compressed')        
 
 
 def get_chromosome_sizes_from_ref(reference: str):
     """Extract chromosome sizes from reference FASTA
 
     Parameters
     ----------
@@ -197,25 +197,25 @@
         name and size of each chromosome
     """
     return pd.DataFrame(((k, len(v)) for k, v in Fasta(reference).items()),
                         columns=('name', 'size'))
 
 
 
-def generate_plotting_data(anchoring_values, groups, size, scale: float = 1,
+def generate_plotting_data(coverage_values, groups, size, scale: float = 1,
                            shift: float = 0, bin_size: int = 0,
                            single_chrom: bool = False):
     """Construct rows of preprocessed data for the plotting data frame. Data
     are binned by rounding to the nearest bin coordinate, while bin coordinates
     are determined by the bin size parameter.
 
     Parameters
     ----------
-    anchoring values
-        iterable of iterables listing anchoring values
+    coverage values
+        iterable of iterables listing coverage values
     groups
         iterable of group names
     size
         chromosome size in bp
     scale
         ratio of chromosome size to mean chromosome size
     shift
@@ -224,70 +224,69 @@
     bin_size
         set bin size. The input <int> is converted to the bin size by the
         formula: 10^(<int>+6) bp. The default value is 0, i.e. 1-megabase bins.
 
     Yields
     ------
     tuple
-        bin coordinate, value, and group ID of an anchoring data point
+        bin coordinate, value, and group ID of a coverage data point
     """
 
     yield from ((chrom, min(round(int(pos), -6-bin_size), size)/size*scale + shift,
                 float(cov), group, f'{group}' if single_chrom else f'{group}_{chrom}')
         for chrom, _, pos, cov, group
-        in (list(vals)+[g] for cv, g in zip(anchoring_values, groups) for vals in cv))
+        in (list(vals)+[g] for cv, g in zip(coverage_values, groups) for vals in cv))
 
 
 def collapse_plotting_data(rows):
     yield from ((c, x, mean(r[2] for r in rws), g, n)
                 for (c, x, g, n), rws in groupby(rows, key=itemgetter(0,1,3,4)))
 
 
-def anchor_dicts_tuple(*pk_results, ref, chromosomes):
+def regcov_dicts_tuple(*pk_results, ref, chromosomes):
     return tuple(result.get_collapsed_regional_scores(ref, {c: [] for c in chromosomes})
                     for result in  pk_results)
 
 
-def anchor_genome_df(*anchor_dicts, sizes, chromosomes: list,
+def genome_coverage_df(*regcov_dicts, sizes, chromosomes: list,
                        summary_func=mean, groups=None,
                        legend_title: str = 'Group', bin_size: int = 0,
                        x_label: str = 'Chromosome'):
     sizes.index = sizes.name
     sizes = sizes.loc[chromosomes, 'size']
     scales = sizes / sizes.mean()
     shifts = pd.Series(accumulate(chain((0,),scales[:-1])), index=scales.index)
     return pd.DataFrame(
         chain.from_iterable((collapse_plotting_data(generate_plotting_data(
-                (generate_anchoring_values(chrom, 0,
+                (generate_coverage_values(chrom, 0,
                     sizes[chrom], rd, summary_func=summary_func)
-                    for rd in anchor_dicts),
+                    for rd in regcov_dicts),
                 groups, size, scale=scale, shift=shift, bin_size=bin_size,
                 single_chrom=(len(chromosomes)==1)))
             for chrom, size, scale, shift
             in zip(chromosomes, sizes, scales, shifts))),
-        columns=('SeqID', x_label, 'K-mer conserv (%)', legend_title,
+        columns=('SeqID', x_label, 'K-mer coverage (%)', legend_title,
                  f'{legend_title}_chrom'))
 
 
-def anchor_genome_plot(plotting_data, output: str,
+def genome_coverage_plot(plotting_data, output: str,
                          groups=None, loci=None, sizes=None,
                          title: str = 'Coverage', x_label: str = 'Chromosome',
                          legend: bool = False,
                          legend_title: str = 'Group', legend_loc: str = 'best',
                          width: float = 7.0, height: float = 3.0,
                          color_palette=COLOR_PALETTE, alpha: float = 0.5,
-                         linewidth: int = 3, xtlabel_rotation: int = 0,
-                         xtlabel_ha: str = 'center'):
-    """Generate a plot of average k-mer conservation values in bins, from a DF
-    generated by anchor_genome_df
+                         linewidth: int = 3):
+    """Generate a plot of average k-mer coverage values in bins, from a DF
+    generated by genome_coverage_df
 
     Parameters
     ----------
     plotting_data
-        pandas DataFrame as generated by anchor_genome_df
+        pandas DataFrame as generated by genome_coverage_df
     output : str
         path to destination file for the plot
     groups
         iterable of group names
     loci
         list of strings indicating loci in form "contig:pos:name"
     sizes
@@ -309,94 +308,78 @@
         height of the plot in inches
     color_palette
         color palette for plot lines
     alpha : float
         alpha value for plot lines
     linewidth : float
         width value for plot lines
-    xtlabel_rotation : int
-        rotation for x-axis tick labels
-    xtlabel_ha : str
-        horizontal alignment for x-axis tick labels (left, center, right)
     """
 
     chromosomes = plotting_data.loc[:,'SeqID'].unique()
-    if legend:
-        data_groups = plotting_data.loc[:,legend_title].unique()
-        if groups is None:
-            groups = data_groups
-        else:
-            groups_dict = dict(zip(data_groups, groups))
-            plotting_data[legend_title] = tuple(groups_dict[x] for x in plotting_data[legend_title])
-            plotting_data[f'{legend_title}_chrom'] = tuple(groups_dict[x] for x in plotting_data[f'{legend_title}_chrom'])
     palette = tuple(islice(cycle(color_palette[:len(groups)]),
                                  len(chromosomes) * len(groups)))
     shifts = plotting_data.loc[:,['SeqID', x_label]].groupby('SeqID').min()
-    if sizes is not None:
-        sizes.index = sizes.name
-        sizes = sizes.loc[chromosomes, 'size']
     if loci is not None:
         if sizes is None:
             raise RuntimeError('loci argument requires sizes argument')
+        sizes.index = sizes.name
+        sizes = sizes.loc[chromosomes, 'size']
         scales = sizes / sizes.mean()
         loci_parsed = tuple(
             (int(p)/sizes[c] * scales[c] + shifts.loc[c, x_label], n)
             for c, p, n in (l.split(':') for l in loci))
         loci_x = tuple(l[0] for l in loci_parsed)
         ticks_labels = sorted(loci_parsed + tuple(zip(shifts[x_label],
                                                       chromosomes)))
         xticks = tuple(tl[0] for tl in ticks_labels)
         xlabels = tuple(tl[1] for tl in ticks_labels)
     else:
         xticks = shifts[x_label]
         xlabels = chromosomes
-    ax = sns.lineplot(x=x_label, y='K-mer conserv (%)',
-                      hue=f'{legend_title}_chrom', data=plotting_data, errorbar=None,
-                      linewidth=linewidth,
-                      palette=palette,
-                      alpha=alpha,
+    ax = sns.lineplot(x=x_label, y='K-mer coverage (%)',
+                      hue=f'{legend_title}_chrom', data=plotting_data, ci=None,
+                      linewidth=linewidth, palette=palette, alpha=alpha,
                       legend='auto' if legend else False)
     ax.set_title(title)
     if (loci is not None) and (sizes is not None):
-        ax.vlines(x=loci_x, ymin=min(plotting_data['K-mer conserv (%)']),
-                  ymax=max(plotting_data['K-mer conserv (%)']),
+        ax.vlines(x=loci_x, ymin=min(plotting_data['K-mer coverage (%)']),
+                  ymax=max(plotting_data['K-mer coverage (%)']),
                   colors='gray',
                   linestyles='dashed')
-    if (len(chromosomes) == 1) and (sizes is not None):
+    if len(chromosomes) == 1:
         xticks = ax.get_xticks()[1:-1]
-        xlabels=tuple(f"{x*sizes.loc[chromosomes[0]]/1e6:.1f}" for x in xticks)
+        xlabels=tuple(f"{x*sizes.loc[chromosomes[0], 'size']/1e6:.1f}" for x in xticks)
     ax.set_xticks(xticks)
-    ax.set_xticklabels(xlabels, rotation=xtlabel_rotation, ha=xtlabel_ha)
+    ax.set_xticklabels(xlabels, ha='left')
     if legend:
         if legend_loc == 'outside':
             leg = ax.legend(bbox_to_anchor=(1.02, 1), loc='upper left',
                             borderaxespad=0, title=legend_title)
         else:
             leg = ax.legend(loc=legend_loc, title=legend_title)
         for line in leg.get_lines():
             line.set_linewidth(linewidth)
             line.set_alpha(alpha)
     fig = ax.get_figure()
-    fig.set_figwidth(width)
     fig.set_figheight(height)
+    fig.set_figwidth(width)
     fig.tight_layout()
     fig.savefig(output)
     fig.clf()
 
 
-def anchor_genome(*pk_results, output: str, ref: str, chromosomes: list,
+def genome_coverage(*pk_results, output: str, ref: str, chromosomes: list,
                     output_table=None, summary_func=mean, groups=None, loci=None,
-                    title: str = 'Genome anchoring', x_label: str = 'Chromosome',
+                    title: str = 'Coverage', x_label: str = 'Chromosome',
                     legend: bool = False, legend_title='Group', legend_loc='best',
                     bin_size: int = 0, width: float = 7.0, height: float = 3.0,
                     color_palette=COLOR_PALETTE, alpha: float = 0.5,
-                    linewidth: int = 3, processes: int = 1,
-                    xtlabel_rotation: int = 0, xtlabel_ha: str = 'center'):
+                    linewidth: int = 3, processes: int = 1):
 
-    """Generate a plot of average k-mer conservation values in bins across the
+    """Generate a plot of average k-mer coverage values in bins across the
     input genome
 
     Parameters
     ----------
     pk_results
         a PKResults object
     output : str
@@ -404,15 +387,15 @@
     ref : str
         path to the input reference genome in BGZIP compressed FASTA format
     chromosomes : list
         list of chromosomes to include in the plot
     output_table
         path to write TSV table containing underlying plotting data
     summary_func
-        function for summarizing the conservation of a kmer across genomes
+        function for summarizing the coverage value of a kmer across genomes
         in the index. The default is statistics.mean
     groups
         iterable of group names
     title : str
         title of the plot
     x_label : str
         x-axis label
@@ -434,49 +417,44 @@
         color palette for plot lines
     alpha : float
         alpha value for plot lines
     linewidth : float
         width value for plot lines
     processes: int
         number of processes to use
-    xtlabel_rotation : int
-        rotation for x-axis tick labels
-    xtlabel_ha : str
-        horizontal alignment for x-axis tick labels (left, center, right)
     """
 
     check_for_bgzip(ref)
     if not groups:
         groups = list(range(len(pk_results)))
     for result in pk_results:
         result.threads = processes
-    anchor_dicts = anchor_dicts_tuple(*pk_results, ref=ref,
+    regcov_dicts = regcov_dicts_tuple(*pk_results, ref=ref,
         chromosomes=chromosomes)
     sizes = get_chromosome_sizes_from_ref(ref)
-    plotting_data = anchor_genome_df(*anchor_dicts, sizes=sizes,
+    plotting_data = genome_coverage_df(*regcov_dicts, sizes=sizes,
         chromosomes=chromosomes, summary_func=summary_func, groups=groups,
         legend_title=legend_title, bin_size=bin_size, x_label=x_label)
     if output_table:
         plotting_data.to_csv(output_table, sep='\t', index=False)
-    anchor_genome_plot(plotting_data, output=output,
+    genome_coverage_plot(plotting_data, output=output,
         groups=groups, loci=loci, sizes=sizes, title=title, x_label=x_label,
         legend=legend, legend_title=legend_title, legend_loc=legend_loc,
         width=width, height=height, color_palette=color_palette, alpha=alpha,
-        linewidth=linewidth, xtlabel_rotation=xtlabel_rotation,
-        xtlabel_ha=xtlabel_ha)
+        linewidth=linewidth)
 
 
-def anchor_heatmap(pk_results, refs, features, output, n_features=None, width=7, height=7):
+def coverage_heatmap(pk_results, refs, features, output, n_features=None, width=7, height=7):
     if not output.endswith('.png'):
         raise RuntimeError('output file path must end with .png')
     results = tuple(pk_results.get_collapsed_regional_scores(ref, gff_to_dict(gff, n_features=n_features))
         for ref, gff in zip(refs, features))
     dfs = tuple(pd.DataFrame({os.path.basename(ref.replace('.fasta', '').replace('.gz', '')):
-            tuple(sum(v) for values in anchor_dict.values() for v in values)}).transpose()
-        for ref, anchor_dict in zip(refs, results))
+            tuple(sum(v) for values in regcov_dict.values() for v in values)}).transpose()
+        for ref, regcov_dict in zip(refs, results))
     vmin = min(df.values.min() for df in dfs)
     vmax = max(df.values.max() for df in dfs)
     sns.set_context('paper')
     fig, axs = plt.subplots(nrows=len(dfs))
     fig.set_figwidth(width)
     fig.set_figheight(height)
     def round(n, k):
```

### Comparing `pankmer-0.15.1/src/pankmer/adjacency_matrix.py` & `pankmer-0.9.0/src/pankmer/adjacency_matrix.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,25 +22,28 @@
 #     return df
 
 def get_adjacency_matrix(results):
     """Generate an adjacency matrix from a PKResults object
     
     Parameters
     ----------
-    results : PKResults
+    results
         a PKResults object
     
     Returns
     -------
     DataFrame
         an adjacency matrix    
     """
 
     score_counts = {}
     for _, score in results:
         score_counts[score] = score_counts.get(score, 0) + 1
     mat = np.zeros((results.number_of_genomes,
                     results.number_of_genomes), dtype=int)
     for score, count in score_counts.items():
-        score_multi = np.array(results.decode_score(score), dtype=int) * count
+        score_arr = results.decode_score(score)
+        score_multi = np.array(score_arr) * count
         mat = add_score_mat_np(score_multi, mat)
-    return pd.DataFrame(mat, index=results.genomes, columns=results.genomes)
+    genome_names = tuple(str(os.path.basename(g)).replace('.fasta.gz', '').replace('.fa.gz', '')
+                         for g in results.genomes)
+    return pd.DataFrame(mat, index=genome_names, columns=genome_names)
```

### Comparing `pankmer-0.15.1/src/pankmer/count.py` & `pankmer-0.9.0/src/pankmer/count.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import pandas as pd
-from collections import Counter
 
 def count_kmers(*pk_results, names=None):
     """Count total and diagnostic K-mers in one or more indexes
 
     Parameters
     ----------
     pk_results
         a PKResults object
     names
         an iterable of the names for each input index
 
     Returns
     -------
     DataFrame
-        table of K-mer counts for each index
+        table of total and diagnostic K-mer counts for each index
     """
-    names = names or range(len(pk_results))
-    max_score = max(pkr.number_of_genomes for pkr in pk_results)
-    kmer_counts = pd.DataFrame(0, columns=names, index=range(1, max_score+1))
-    for pkr, name in zip(pk_results, names):
-        for s, c in  Counter(sum(pkr.decode_score(score)) for _, score in pkr).items():
-            kmer_counts.loc[s, name] = c
+
+    kmer_counts = pd.DataFrame(columns=('index', 'total', 'diagnostic'))
+    for pkr, name in zip(pk_results, names or range(len(pk_results))):
+        total_count, diagnostic_count = 0, 0
+        for _, score in pkr:
+            total_count += 1
+            if sum(score) < pkr.number_of_genomes:
+                diagnostic_count += 1
+        kmer_counts = pd.concat((kmer_counts, pd.DataFrame(
+            ((name, total_count, diagnostic_count),),
+            columns=('index', 'total', 'diagnostic'))))
     return kmer_counts
```

### Comparing `pankmer-0.15.1/src/pankmer/pankmer.py` & `pankmer-0.9.0/src/pankmer/pankmer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,62 @@
 #!/usr/bin/env python
 import argparse
-import gzip
-import io
-from os.path import join, isfile, isdir, basename, dirname, exists, commonprefix
-import seaborn as sns
-from os import mkdir, listdir
+from os.path import join, isfile, isdir, basename
+import os
 import sys
 import time
+import gzip
 from multiprocessing import Pool
 import pandas as pd
+import io
 import math
 import json
 from Bio import SeqIO
 import numpy as np
 import shutil
 import tarfile
-from operator import itemgetter
-from itertools import chain
-from more_itertools import batched
 
 # from pankmer.index import (print_err, genome_name, break_seq, get_kmers,
 #                    score_byte_to_blist, kmer_byte_to_blist, kmer_byte_to_long)
-from pankmer.index import (kmer_size, break_seq, print_err, score_byte_to_blist,
-                           run_index, measure_genomes)
+from pankmer.index import (print_err, break_seq, get_kmers, score_byte_to_blist,
+                           run_index)
 from pankmer.env import EXAMPLE_DATA_DIR
 from pankmer.download import download_example
 from pankmer.count import count_kmers
-from pankmer.collect import COL_COLOR_PALETTE, collect
-from pankmer.upset import upset
-from pankmer.subset import subset
 from pankmer.adjacency_matrix import get_adjacency_matrix
-from pankmer.tree import (tree, adj_to_jaccard, adj_to_overlap, adj_to_qv,
-                          adj_to_qv_symmetric, adj_to_ani)
+from pankmer.tree import tree
 from pankmer.clustermap import clustermap
-from pankmer.anchor import (COLOR_PALETTE, anchor_region, anchor_genome,
-                                  anchor_genome_plot, anchor_heatmap)
-from pankmer.anchormap import anchormap
-from pankmer.dryrun import dryrun
+from pankmer.reg_coverage import (COLOR_PALETTE, reg_coverage, genome_coverage,
+                                  genome_coverage_plot, coverage_heatmap)
 from pankmer.version import __version__
 from pankmer.gzip_agnostic_open import gzip_agnostic_open
 from pankmer.get_lower_bound import get_lower_bound
-from pankmer.parse_genomes_input import parse_genomes_input, remove_seq_ext
-
-#===============================================================================
-KMER_MAX = 2**64 - 1
 
-#===============================================================================
 
-def retrieve_metadata(metadata_path):
+def retreive_metadata(metadata_path):
     if isinstance(metadata_path, tarfile.ExFileObject):
         metadata = json.load(metadata_path)
     else:
         with open(metadata_path, 'rt') as infile:
             metadata = json.load(infile)
     genomes = {}
     for pos in range(len(metadata['genomes'])):
         genome = metadata['genomes'][str(pos)]
         size = metadata['genome_sizes'][genome]
         genomes[genome] = size
-    return metadata['kmer_size'], genomes, metadata['positions'], metadata['mem_blocks']
+    return metadata['kmer_size'], genomes, metadata['positions']
 
 
 def get_positional_kmers(fasta_path, upper, lower, contig_header='id'):
     kmers_dict = {}
     with gzip_agnostic_open(fasta_path, 'rt') as infile:
         for record in SeqIO.parse(infile, 'fasta'):
             names = {'id': record.id, 'description': record.description}
             seq_byte = bytes(str(record.seq).upper(), 'ascii')
-            kmers_dict[names[contig_header]] = break_seq(seq_byte, upper, lower, KMER_MAX)
+            kmers_dict[names[contig_header]] = break_seq(seq_byte, upper, lower)
     return kmers_dict
 
 
 def get_sorted_kmer_scores(args: list) -> dict:
     index_path, kmers = args
     results = PKResults(index_path)
     lower = min(list(kmers.keys()))
@@ -85,15 +70,16 @@
         results.seek_kmer(initial_lower_bound)
         results.seek_score(initial_lower_bound)
     for kmer_bit, score_bit in results:
         if kmer_bit > ub_bit:
             break
         kmer  = results.decode_kmer(kmer_bit)
         if kmer in kmers:
-            kmers[kmer] = results.decode_score(score_bit)
+            score = results.decode_score(score_bit)
+            kmers[kmer] = score
     return kmers
 
 
 class PKIterator:
     def __init__(self, results):
         self._results = results
     
@@ -104,63 +90,59 @@
             self._results.reset_iter()
             raise StopIteration
         return kmer, score
 
 
 class PKResults:
     def __init__(self, results_dir: str, threads: int = 1):
-        index_files = ['metadata.json', 'kmers.bgz', 'scores.bgz']
-        self.input_is_tar = False
+        index_files = ['metadata.json', 'kmers.b.gz', 'scores.b.gz']
         if isfile(results_dir) and tarfile.is_tarfile(results_dir):
             self.input_is_tar = True
             self.tar = tarfile.open(results_dir)
             found_files = {basename(tarinfo.name) for tarinfo in self.tar
                             if tarinfo.isreg()}
             for file in index_files:
                 if file not in found_files:
                     raise ValueError(f"{file} is not found in index!")
             kmers_filename, metadata_filename, scores_filename = sorted(
                 tarinfo.name for tarinfo in self.tar if tarinfo.isreg())
-            kmer_size, genomes, positions, mem_blocks = retrieve_metadata(
+            kmer_size, genomes, positions = retreive_metadata(
                 self.tar.extractfile(metadata_filename))
-            self.number_of_genomes = len(genomes)
             self.kmers_stream = gzip.open(self.tar.extractfile(kmers_filename), 'rb')
             self.scores_stream = gzip.open(self.tar.extractfile(scores_filename), 'rb')
         elif isdir(results_dir):
             for file in index_files:
                 file_path = join(results_dir, file)
                 if not isfile(file_path):
                     raise ValueError(f"{file} is not found in results directory!")
-            kmer_size, genomes, positions, mem_blocks = retrieve_metadata(join(results_dir, 'metadata.json'))
-            self.number_of_genomes = len(genomes)
-            self.kmers_stream = gzip.open(join(results_dir, 'kmers.bgz'), 'rb')
-            self.scores_stream = gzip.open(join(results_dir, 'scores.bgz'), 'rb')
+            kmer_size, genomes, positions = retreive_metadata(join(results_dir, 'metadata.json'))
+            self.kmers_stream = gzip.open(join(results_dir, 'kmers.b.gz'), 'rb')
+            self.scores_stream = gzip.open(join(results_dir, 'scores.b.gz'), 'rb')
         else:
             raise ValueError(f"{results_dir} is not a valid directory!")
         self.results_dir = results_dir
         self.kmer_size = kmer_size
         self.genomes = genomes
+        self.number_of_genomes = len(genomes)
         self.positions = positions
-        self.kmer_bitsize = math.ceil(kmer_size*2/8)
+        self.kmer_bitsize = math.ceil(((kmer_size*2))/8)
         self.score_bitsize = math.ceil(len(genomes)/8)
         self.threads = threads
-        self.mem_blocks = mem_blocks
         self.kmer_buffer = io.BufferedReader(self.kmers_stream)
         self.score_buffer = io.BufferedReader(self.scores_stream)
         
     def __iter__(self) -> PKIterator:
         """ Object iterator
 
         Returns
         -------
         PKIterator
             returns a kmer and a score in bytes
         """        
         return PKIterator(self)
-
         
     def get_kmer_byte(self) -> bytes:
         """read bytes in size of one kmer from kmers file
 
         Returns
         -------
         bytes
@@ -174,15 +156,15 @@
     def get_score_byte(self) -> bytes:
         """read bytes in size of one score from scores file
 
         Returns
         -------
         bytes
             bytes represting what samples have a Kmer
-        """
+        """        
         score_byte = self.score_buffer.read(self.score_bitsize)
         if not score_byte:
             return None
         return score_byte
     
     def seek_kmer(self, kmer_num : int):
         """Move Kmer file pointer past a number of Kmers
@@ -268,15 +250,15 @@
         -------
         int
             Python integer representing canonical Kmer
         """        
         upper = (1<<(self.kmer_size*2))-1
         lower = 0
         kmer_byte = bytes(kmer.upper(), 'ascii')
-        kmer_list = break_seq(kmer_byte, upper, lower, KMER_MAX)
+        kmer_list = break_seq(kmer_byte, upper, lower)
         if len(kmer_list) > 1:
             raise ValueError(f"encode_kmer should be used for one Kmer of size {self.kmer_size} only! "
                              f"Please use get_sequence_kmerbits for a sequence larger than that.")
         return kmer_list[0]
     
     def get_sequence_kmerbits(self, seq : str, upper : int = None, lower : int = None) -> list:
         """Get canonical Kmers making up the sequence
@@ -292,15 +274,15 @@
             list of Python integers representing the canonical Kmers
         """        
         if upper == None:
             upper = (1<<(self.kmer_size*2))-1
         if lower == None:
             lower = 0
         seq_byte = bytes(str(seq).upper(), 'ascii')
-        kmer_bits = break_seq(seq_byte, upper, lower, KMER_MAX)
+        kmer_bits = break_seq(seq_byte, upper, lower)
         
         return kmer_bits
     
     def get_kmer_scores(self, kmers : dict = None) -> dict:
         """Retrieve scores of Kmer in the Kmers dictionary.
         if no dictionary is supplied then retrieve all scores.
 
@@ -321,15 +303,15 @@
             for kmer, score in self:
                 kmers[kmer] = score
         else:
             # get only scores in kmers
             for kmer, score in self:
                 kmer_int = self.decode_kmer(kmer)
                 if kmer_int in kmers:
-                    kmers[kmer_int] = score
+                    kmers[kmer_int] = self.decode_score(score)
         return kmers
     
     def get_sequence_score(self, seq : str, kmers : dict = None) -> list:
         """Retrieve scores of canonical Kmers in the sequence
 
         Parameters
         ----------
@@ -712,260 +694,91 @@
 #             else:
 #                 scores_counts[score] = 1
 #             score = score_buffer.read(score_bitsize)
 
 #     return scores_counts
 
 
-def index_wrapper(outdir: str,  genomes_input=None, genomes_input_paired=None,
-                  split_memory: int = 1, threads: int = 1,
-                  index: str = '', fraction: float = 1.0, gzip_level: int = 6,
-                  k=kmer_size()):
-    if basename(outdir).endswith('.tar'):
-        output_is_tar = True
-        outdir = join(dirname(outdir), basename(outdir)[:-4])
-    else:
-        output_is_tar = False
-    if genomes_input is None and genomes_input_paired is None:
-        raise RuntimeError('genomes must be provided')
-    print_err('Recording genome sizes')
-    if genomes_input is not None:
-        genomes_input, genomes, input_is_tar = parse_genomes_input(genomes_input)
-        genomes_dict = measure_genomes(genomes, str(genomes_input[0]) if input_is_tar else '')
-    else:
-        genomes_dict, genomes, input_is_tar = {}, [], False
-    if genomes_input_paired is not None:
-        genomes_input_paired, genomes_paired, _= parse_genomes_input(genomes_input_paired)
-        genomes_dict_paired = {commonprefix([g0, g1]): s0+s1
-                               for ((g0, s0), (g1, s1))
-                               in batched(sorted(measure_genomes(genomes_paired, '').items()), 2)}
-    else:
-        genomes_dict_paired, genomes_paired = {}, []
-
-    # Make the output directory if it doesn't exist
-    if not exists(outdir):
-        mkdir(outdir)
-
-    total_seq_bp = sum(chain(genomes_dict.values(), genomes_dict_paired.values()))
-    if total_seq_bp == 0:
-        raise RuntimeError('No sequence in input')
-    print_err(f'{total_seq_bp} bp of sequence total')
-    print_err(f'Using {split_memory} memory blocks')
-    positions_dictionary, mem_blocks = run_index(
-            (str(genomes_input[0] if genomes_input else '') if input_is_tar else ''),
-            (genomes if genomes else []),
-            (genomes_paired if genomes_paired else []),
-            str(outdir),
-            split_memory=split_memory, threads=threads,
-            index=index,
-            input_is_tar=input_is_tar,
-            fraction=fraction,
-            gzip_level=gzip_level, kmersize=k)
-    
-    # if index:
-    #     genomes, genomes_dict = update_genomes(index, genomes, genomes_dict)
+def get_kmers_wrapper(seq, upper, lower):
+    seq_byte = bytes(str(seq).upper(), 'ascii')
+    kmers = break_seq(seq_byte, upper, lower)
+    return kmers
 
-    print_err("Saving metadata.")
-    metadata_dict = {'kmer_size': kmer_size(),
-        'version': __version__,
-        'genomes': {c: remove_seq_ext(basename(g))
-                    for c, g in enumerate(chain(genomes,
-                        (commonprefix([g0, g1])
-                         for g0, g1 in batched(genomes_paired, 2))))},
-        'genome_sizes': {remove_seq_ext(basename(g)): s
-                         for g, s in chain(genomes_dict.items(),
-                                           genomes_dict_paired.items())},
-        'positions': dict(sorted(positions_dictionary.items(), key=itemgetter(1))),
-        'mem_blocks': mem_blocks,
-        'fraction_cutoff': [fraction, int(fraction*KMER_MAX)]
-    }
-    with open(f'{outdir}/metadata.json', 'w') as outfile:
-        json.dump(metadata_dict, outfile)
-    if output_is_tar:
-        with tarfile.open(f'{outdir}.tar', 'w') as tar:
-            tar.add(outdir)
-        shutil.rmtree(outdir)
 
-def run_index_wrapper(args):
+def index_wrapper(args):
     if args.time:
         start = time.time()
-    # index = args.index
-    index_wrapper(args.output,
-        genomes_input=args.genomes,
-        genomes_input_paired=args.genomes_paired,
-        split_memory=args.split_memory,
-        threads=args.threads, index='',
-        k=kmer_size(),
-        fraction=1-10**(-1*args.qual/(10*kmer_size())) if args.qual else args.fraction,
-        gzip_level=args.gzip_level)
+    genomes_input = args.genomes
+    output = args.output
+    split_memory = args.split_memory
+    threads = args.threads
+    index = args.index
+    run_index(genomes_input, output,
+        split_memory=split_memory, threads=threads, index=index)
     if args.time:
         stop = time.time()
         print(f'Indexed in {(stop - start) / 60:.2f} minutes')
 
 
 def run_count(args):
     kmer_counts = count_kmers(*(PKResults(i) for i in args.index), names=args.index)
-    kmer_counts.to_csv(sys.stdout, sep='\t')
-
-
-def run_collect(args):
-    sat_df = collect(PKResults(args.index), args.output, title=args.title,
-                        width=args.width, height=args.height,
-                        palette=args.color_palette, alpha=args.alpha,
-                        linewidth=args.linewidth, conf=args.conf,
-                        contours=args.contours, legend_loc=args.legend_loc)
-    if args.table:
-        sat_df.to_csv(args.table, sep='\t', index=False)
-
-
-def run_upset(args):
-    if args.time:
-        start = time.time()
-    upset(PKResults(args.input), args.output, args.genomes,
-          vertical=args.vertical,
-          show_counts=args.show_counts,
-          min_subset_size=args.min_subset_size,
-          max_subset_size=args.max_subset_size,
-          exclusive=args.exclusive,
-          table=args.table)
-    if args.time:
-        stop = time.time()
-        print(f'UpSet plot generated in {(stop - start) / 60:.2f} minutes')
-
-
-def run_subset(args):
-    if args.time:
-        start = time.time()
-    subset(PKResults(args.input), args.output, args.genomes,
-          exclusive=args.exclusive, gzip_level=args.gzip_level)
-    if args.time:
-        stop = time.time()
-        print(f'subset index generated in {(stop - start) / 60:.2f} minutes')
+    kmer_counts.to_csv(sys.stdout, sep='\t', index=False)
 
 
 def run_adjacency_matrix(args):
     if args.time:
         start = time.time()
-    if args.output.endswith('.csv'):
-        separator = ','
-    elif args.output.endswith('.tsv'):
-        separator = '\t'
-    else:
-        raise RuntimeError('output must end with .csv or .tsv')
     results = PKResults(args.input_dir)
+    output = args.output
     df = get_adjacency_matrix(results)
-    df.to_csv(args.output, sep=separator)
+    df.to_csv(output)
     if args.time:
         stop = time.time()
         print(f'Matrix generated in {(stop - start) / 60:.2f} minutes')
 
 
 def run_tree(args):
-    if str(args.input).endswith('.csv'):
-        adj_matrix = pd.read_csv(args.input, index_col=0)
-    elif str(args.input).endswith('.tsv'):
-        adj_matrix = pd.read_table(args.input, index_col=0)
-    else:
-        raise RuntimeError('input must end with .csv or .tsv')
+    adj_matrix = pd.read_csv(args.input, index_col=0)
     tree(adj_matrix, newick=args.newick, metric=args.metric, method=args.method,
          transformed_matrix=args.transformed_matrix)
 
 
 def run_clustermap(args):
-    if str(args.input).endswith('.csv'):
-        adj_matrix = pd.read_csv(args.input, index_col=0)
-    elif str(args.input).endswith('.tsv'):
-        adj_matrix = pd.read_table(args.input, index_col=0)
-    else:
-        raise RuntimeError('input must end with .csv or .tsv')
+    adj_matrix = pd.read_csv(args.input, index_col=0)
     clustermap(adj_matrix, args.output, cmap=args.colormap, width=args.width,
-        height=args.height, metric=args.metric, method=args.method,
-        heatmap_tick_pos=args.heatmap_ticks,
-        cbar_tick_pos=args.cbar_ticks, dendrogram_ratio=args.dend_ratio,
-        dendrogram_spacer=args.dend_spacer)
-
-
-def run_similarity(args):
-    if str(args.input).endswith('.csv'):
-        adj_matrix = pd.read_csv(args.input, index_col=0)
-    elif str(args.input).endswith('.tsv'):
-        adj_matrix = pd.read_table(args.input, index_col=0)
-    else:
-        raise RuntimeError('input must end with .csv or .tsv')
-    if args.output.endswith('.csv'):
-        separator = ','
-    elif args.output.endswith('.tsv'):
-        separator = '\t'
-    else:
-        raise RuntimeError('output must end with .csv or .tsv')
-    if args.metric == 'jaccard':
-        df = adj_to_jaccard(adj_matrix)
-    elif args.metric == 'overlap':
-        df = adj_to_overlap(adj_matrix)
-    elif args.metric == 'qv':
-        df = adj_to_qv(adj_matrix)
-    elif args.metric == 'qv_symmetric':
-        df = adj_to_qv_symmetric(adj_matrix)
-    elif args.metric == 'ani':
-        df = adj_to_ani(adj_matrix)
-    else:
-        raise RuntimeError('invalid metric')
-    df.to_csv(args.output, sep=separator)
-
-
-def run_distance(args):
-    if str(args.input).endswith('.csv'):
-        adj_matrix = pd.read_csv(args.input, index_col=0)
-    elif str(args.input).endswith('.tsv'):
-        adj_matrix = pd.read_table(args.input, index_col=0)
-    else:
-        raise RuntimeError('input must end with .csv or .tsv')
-    if args.output.endswith('.csv'):
-        separator = ','
-    elif args.output.endswith('.tsv'):
-        separator = '\t'
-    else:
-        raise RuntimeError('output must end with .csv or .tsv')
-    if args.metric == 'jaccard':
-        df = 1 - adj_to_jaccard(adj_matrix)
-    elif args.metric == 'overlap':
-        df = 1 - adj_to_overlap(adj_matrix)
-    elif args.metric == 'ani':
-        df = 1 - adj_to_ani(adj_matrix)
-    else:
-        raise RuntimeError('invalid metric')
-    df.to_csv(args.output, sep=separator)
-
+               height=args.height, metric=args.metric, method=args.method,
+               heatmap_tick_pos=args.heatmap_ticks,
+               cbar_tick_pos=args.cbar_ticks)
 
 
-def run_anchor_region(args):
+def run_regcoverage(args):
     if args.output:
-        anchor_region(*(PKResults(i) for i in args.index), ref=args.ref,
+        reg_coverage(*(PKResults(i) for i in args.index), ref=args.ref,
             coords=args.coords, output_file=args.output, bgzip=args.bgzip,
             genes=args.genes, flank=args.flank, processes=args.processes)
     else:
-        for chrom, start, end, *values in anchor_region(
+        for chrom, start, end, *values in reg_coverage(
             *(PKResults(i) for i in args.index), ref=args.ref,
                 coords=args.coords, genes=args.genes, flank=args.flank,
                 processes=args.processes):
             print(chrom, start, end, *values, sep='\t')
 
 
-def run_anchor_genome(args):
-    anchor_genome(*(PKResults(i) for i in args.index), output=args.output,
+def run_genome_coverage(args):
+    genome_coverage(*(PKResults(i) for i in args.index), output=args.output,
         ref=args.ref, chromosomes=args.chromosomes, output_table=args.table,
         groups=args.groups, title=args.title, x_label=args.x_label,
         legend=args.legend,
         legend_title=args.legend_title, legend_loc=args.legend_loc,
         bin_size=args.bin_size, width=args.width, height=args.height,
         color_palette=args.color_palette, alpha=args.alpha,
         linewidth=args.linewidth, processes=args.processes)
 
 
-def run_anchor_genome_plot(args):
+def run_genome_coverage_plot(args):
     plotting_data=pd.read_table(args.table)
     x_label = args.x_label if args.x_label else plotting_data.columns[1]
     legend_title = args.legend_title if args.legend_title else plotting_data.columns[3]
     columns = (
         plotting_data.columns[0],
         x_label,
         plotting_data.columns[2],
@@ -974,238 +787,125 @@
     )
     plotting_data.columns = columns
     if args.chromsizes:
         sizes = pd.read_table(args.chromsizes, header=None)
         sizes.columns = 'name', 'size'
     else:
         sizes = None
-    anchor_genome_plot(plotting_data, output=args.output,
+    genome_coverage_plot(plotting_data, output=args.output,
         groups=args.groups, loci=args.loci, sizes=sizes,
         title=args.title, x_label=x_label, legend=args.legend,
         legend_title=legend_title,
         legend_loc=args.legend_loc, width=args.width, height=args.height,
         color_palette=args.color_palette, alpha=args.alpha,
         linewidth=args.linewidth)
 
 
-def run_anchormap(args):
-    anchormap(PKResults(args.index), args.output, args.anchors, args.anno,
-              threads=args.threads)
-
-
-def run_anchor_heatmap(args):
-    anchor_heatmap(PKResults(args.index), args.refs, args.features,
+def run_coverage_heatmap(args):
+    coverage_heatmap(PKResults(args.index), args.refs, args.features,
         args.output, n_features=args.n_features, width=args.width,
         height=args.height)
 
 
-def run_dryrun(args):
-    metadata_dict = dryrun(genomes_input=args.genomes,
-                           genomes_input_paired=args.genomes_paired,
-                           split_memory=args.split_memory, threads=args.threads)
-    json.dump(metadata_dict, sys.stdout)
-
-
 def run_download_example(args):
-    download_example(args.dir, args.species, args.n_samples)
+    download_example(args.dir, args.bacterial, args.n_samples)
 
 
 def main():
     parser = argparse.ArgumentParser(
         add_help=True)
-    parser.add_argument('--version', action='version',
-                    version='%(prog)s {version}'.format(version=__version__))
+    parser.add_argument('--version', action='store_true',
+        help='print version number')
     subparsers = parser.add_subparsers(dest='func')
     index_parser = subparsers.add_parser('index',
         help='generate k-mer index')
     index_parser.add_argument(
-        '-g', '--genomes', metavar='<genome[s]{.fa,.fq,.tar,/}>',
-        nargs='+',
-        help='paths to input genomes, directories, or tar archive')
-    index_parser.add_argument(
-        '-p', '--genomes-paired', metavar='<genome[s]{.fa,.fq,/}>',
-        nargs='+',
-        help='paths to input genomes or directories (paired)')
+        '-g', '--genomes', metavar='<genomes[.tar]>', type=str, action='store',
+        dest='genomes', required=True,
+        help='directory containig input genomes')
     index_parser.add_argument(
-        '-o', '--output', metavar='<output[.tar]>',
-        required=True,
+        '-o', '--output', metavar='<output[.tar]>', type=str, action='store',
+        dest='output', required=True,
         help='output directory or tarfile that will contain the k-mer index')
     index_parser.add_argument(
-        '--split-memory', metavar='<int>', type=int, default=1,
-        help='split indexing into multiple rounds to reduce memory usage')
+        '--split-memory', metavar='<int>', action='store',
+        dest='split_memory', type=int, help=(
+        'Parallel.'
+        'This splits the indexing into multiple rounds; reducing memory.'
+        ), default=1)
     index_parser.add_argument(
-        '-t', '--threads', metavar='<int>',
-        type=int, help=('Number of threads to use [1]'), default=1)
-    fraction_group = index_parser.add_mutually_exclusive_group()
-    fraction_group.add_argument(
-        '--fraction', metavar='<float>', type=float, default=1.0, help=(
-        'Fraction of k-mers to use. By default all k-mers are kept.'))
-    fraction_group.add_argument(
-        '-q', '--qual', metavar='<int>', type=int, help=(
-        'Completeness of index, in terms of bases, expressed as a Phred quality score. '
-        'e.g. --qual 30 means approx 1 in 1000 bases will be missed, which is '
-        'equivalent to --fraction 0.2. By default no bases are missed.'))
+        '-t', '--threads', metavar='<int>', action='store',
+        dest='threads', type=int, help=('Number of threads to use'), default=1)
     index_parser.add_argument(
-        '--gzip-level', choices=range(1,10), type=int, default=6,
-        help='gzip compression level [6]')
-    # index_parser.add_argument(
-    #     '-i', '--index', metavar='<index[.tar]>',
-    #     dest='index', required=False, default='',
-    #     help=('Path to existing index to update.')
-    # )
+        '-i', '--index', metavar='<index[.tar]>', type=str, action='store',
+        dest='index', required=False, default=None,
+        help=('Path to existing index to update.')
+    )
     index_parser.add_argument(
         '--time', action='store_true',
         help='Report the time required to execute'
     )
-    index_parser.set_defaults(func=run_index_wrapper)
+    index_parser.set_defaults(func=index_wrapper)
 
     count_parser = subparsers.add_parser('count',
         help='count k-mers in one or more indexes')
     count_parser.add_argument(
         '-i', '--index', metavar='<index[.tar]>', type=str, action='store',
         dest='index', required=True, nargs='+', help='a k-mer index')
     count_parser.set_defaults(func=run_count)
 
-    collect_parser = subparsers.add_parser('collect',
-        help='calculate k-mer collection curve')
-    collect_parser.add_argument(
-        '-i', '--index', metavar='<index[.tar]>', type=str, action='store',
-        required=True, help='a k-mer index')
-    collect_parser.add_argument(
-        '-o', '--output', metavar='<output.{pdf,png,svg}>', type=str,
-        action='store', dest='output',
-        help='destination file for plot')
-    collect_parser.add_argument(
-        '-t', '--table', metavar='<output-table.tsv>',
-        help='output TSV file containing plotted data')
-    collect_parser.add_argument('--title', metavar='<"Plot title">',
-        help='set the title for the plot')
-    collect_parser.add_argument('--width', metavar='<float>', type=float,
-        default=4.0, help='set width of figure in inches [4]')
-    collect_parser.add_argument('--height', metavar='<float>', type=float,
-        default=3.0, help='set height of figure in inches [3]')
-    collect_parser.add_argument('--color-palette', metavar='<#color>', nargs='+',
-        default=COL_COLOR_PALETTE, help='color palette to use')
-    collect_parser.add_argument('--alpha', metavar='<float>', type=float,
-        default=1.0, help='transparency value for lines [1.0]')
-    collect_parser.add_argument('--linewidth', metavar='<int>', type=int,
-        default=3, help='line width for plot [3]')
-    conf_or_cont = collect_parser.add_mutually_exclusive_group()
-    conf_or_cont.add_argument('--conf', action='store_true',
-        help='calculate confidence intervals for collection curves')
-    conf_or_cont.add_argument('--contours', metavar='<int>', type=int,
-        nargs='+', help='set contours for collection curves (in percent)')
-    collect_parser.add_argument('--legend-loc',
-        choices=('best', 'upper left', 'upper right', 'lower left',
-                 'lower right', 'outside'),
-        default='best', help='location of legend [best]')
-    collect_parser.set_defaults(func=run_collect)
-
-    upset_parser = subparsers.add_parser('upset', help='generate upset plot')
-    upset_parser.add_argument(
-        '-i', '--input', metavar='<index[.tar]>',
-        required=True, help='a k-mer index')
-    upset_parser.add_argument(
-        '-o', '--output', metavar='<output.{pdf,png,svg}>', required=True,
-        help='destination file for upset plot')
-    upset_parser.add_argument(
-        '-g', '--genomes', metavar='<genome>', required=True, nargs='+',
-        help='list of genomes to include')
-    upset_parser.add_argument(
-        '-v', '--vertical', action='store_true',
-        help='draw the plot vertically')
-    upset_parser.add_argument(
-        '-x', '--exclusive', action='store_true',
-        help='exclude k-mers that occur in genomes other than the input set')
-    upset_parser.add_argument(
-        '-t', '--table', metavar='<table.tsv[.gz]>',
-        help='write (optionally compressed) table of values in tsv format')
-    upset_parser.add_argument(
-        '--show-counts', action='store_true',
-        help='show counts for each subset')
-    upset_parser.add_argument(
-        '--min-subset-size', metavar='<int>', type=int,
-        help='show only subsets larger than a minimum size')
-    upset_parser.add_argument(
-        '--max-subset-size', metavar='<int>', type=int,
-        help='show only subsets smaller than a maximum size')
-    upset_parser.add_argument(
-        '--time', action='store_true',
-        help='report the time required to execute')
-    upset_parser.set_defaults(func=run_upset)
-
-    subset_parser = subparsers.add_parser('subset', help='subset an index')
-    subset_parser.add_argument(
-        '-i', '--input', metavar='<input-index[.tar]>',
-        required=True, help='a k-mer index')
-    subset_parser.add_argument(
-        '-o', '--output', metavar='<output-index[.tar]>', required=True,
-        help='destination file for subset index')
-    subset_parser.add_argument(
-        '-g', '--genomes', metavar='<genome>', required=True, nargs='+',
-        help='list of genomes to include ')
-    subset_parser.add_argument(
-        '-x', '--exclusive', action='store_true',
-        help='exclude k-mers that occur in genomes other than the input set')
-    subset_parser.add_argument(
-        '--gzip-level',  choices=range(1,10), type=int, default=6,
-        help='gzip compression level [6]')
-    subset_parser.add_argument(
-        '--time', action='store_true',
-        help='report the time required to execute')
-    subset_parser.set_defaults(func=run_subset)
-
     adjmat_parser = subparsers.add_parser('adj-matrix',
         help='generate adjacency matrix')
     adjmat_parser.add_argument(
-        '-i', '--input', metavar='<index[.tar]>',
+        '-i', '--input', metavar='<index[.tar]>', type=str, action='store',
         dest='input_dir', required=True, help='a k-mer index')
     adjmat_parser.add_argument(
-        '-o', '--output', metavar='<adjmatrix.{csv,tsv}>',
+        '-o', '--output', metavar='<adjmatrix.csv>', type=str, action='store',
         dest='output', required=True,
         help='destination file for adjacency matrix')
     adjmat_parser.add_argument(
         '--time', action='store_true',
-        help='Report the time required to execute')
+        help='Report the time required to execute'
+    )
     adjmat_parser.set_defaults(func=run_adjacency_matrix)
 
     tree_parser = subparsers.add_parser('tree',
         help='generate a heirarchical clustering tree from an adjacency matrix')
     tree_parser.add_argument(
-        '-i', '--input', metavar='<adjmatrix.{csv,tsv}>',
+        '-i', '--input', metavar='<adjmatrix.csv>', type=str, action='store',
         dest='input', required=True, help='adjacency matrix file')
     tree_parser.add_argument(
         '-n', '--newick', action='store_true', dest='newick',
         help='output tree in NEWICK format'
     )
     tree_parser.add_argument(
-        '--metric', choices=('intersection', 'jaccard', 'overlap', 'qv', 'qv_symmetric', 'ani'),
+        '--metric', choices=('intersection', 'jaccard', 'overlap'),
         type=str, action='store', dest='metric', default='intersection',
         help='similarity metric [intersection]')
     tree_parser.add_argument(
         '--method', choices=('single', 'complete', 'average', 'weighted', 'centroid'),
         type=str, action='store', dest='method', default='complete',
         help='clustering method [complete]')
     tree_parser.add_argument(
-        '--transformed-matrix', metavar='<matrix.{csv,tsv}>',
+        '--transformed-matrix', metavar='<matrix.csv>',
         help='Write similarity transformed matrix to file')
     tree_parser.set_defaults(func=run_tree)
 
     clustermap_parser = subparsers.add_parser('clustermap',
         help='plot a clustered heatmap from the adjacency matrix')
     clustermap_parser.add_argument(
-        '-i', '--input', metavar='<adjmatrix.{csv,tsv}>', type=str, action='store',
+        '-i', '--input', metavar='<adjmatrix.csv>', type=str, action='store',
         dest='input', required=True,
         help='adjacency matrix file')
     clustermap_parser.add_argument(
         '-o', '--output', metavar='<adjmatrix.{pdf,png,svg}>', type=str, action='store',
         dest='output', required=True,
         help='destination file for plot')
     clustermap_parser.add_argument(
-        '--metric', choices=('intersection', 'jaccard', 'overlap', 'qv', 'qv_symmetric', 'ani'),
+        '--metric', choices=('intersection', 'jaccard', 'overlap'),
         type=str, action='store', dest='metric', default='intersection',
         help='similarity metric [intersection]')
     clustermap_parser.add_argument(
         '--method', choices=('single', 'complete', 'average', 'weighted', 'centroid'),
         type=str, action='store', dest='method', default='complete',
         help='clustering method [complete]')
     clustermap_parser.add_argument(
@@ -1222,243 +922,179 @@
         '--heatmap-ticks', choices=('left', 'right'),
         default='left',
         help='Position of heatmap ticks. Must be "left" or "right" [left]')
     clustermap_parser.add_argument(
         '--cbar-ticks', choices=('left', 'right'),
         default='left',
         help='Position of color bar ticks. Must be "left" or "right" [left]')
-    clustermap_parser.add_argument(
-        '--dend-ratio', metavar='<float>', type=float, default=0.2,
-        help='Fraction of plot width used for dendrogram [0.2]')
-    clustermap_parser.add_argument(
-        '--dend-spacer', metavar='<float>', type=float, default=0.1,
-        help='Fraction of plot width used as spacer between dendrogram and heatmap [0.1]')
     clustermap_parser.set_defaults(func=run_clustermap)
 
-    similarity_parser = subparsers.add_parser('similarity',
-        help='generate a similarity matrix from an adjacency matrix')
-    similarity_parser.add_argument(
-        '-i', '--input', metavar='<adjmatrix.{csv,tsv}>',
-        required=True, help='adjacency matrix file')
-    similarity_parser.add_argument(
-        '-o', '--output', metavar='<simmatrix.{csv,tsv}>',
-        required=True, help='similarity matrix file')
-    similarity_parser.add_argument(
-        '--metric', choices=('jaccard', 'overlap', 'qv', 'qv_symmetric', 'ani'),
-        dest='metric', default='jaccard', help='similarity metric [jaccard]')
-    similarity_parser.set_defaults(func=run_similarity)
-
-    distance_parser = subparsers.add_parser('distance',
-        help='generate a distance matrix from an adjacency matrix')
-    distance_parser.add_argument(
-        '-i', '--input', metavar='<adjmatrix.{csv,tsv}>',
-        required=True, help='adjacency matrix file')
-    distance_parser.add_argument(
-        '-o', '--output', metavar='<distmatrix.{csv,tsv}>',
-        required=True, help='distance matrix file')
-    distance_parser.add_argument(
-        '--metric', choices=('jaccard', 'overlap', 'ani'),
-        dest='metric', default='jaccard', help='distance metric [jaccard]')
-    distance_parser.set_defaults(func=run_distance)
-
-    anchor_reg_parser = subparsers.add_parser('anchor-region',
-        help='anchor k-mers in a region')
-    anchor_reg_parser.add_argument(
+    regcov_parser = subparsers.add_parser('reg-coverage',
+        help='generate regional coverage')
+    regcov_parser.add_argument(
         '-i', '--index', metavar='<index[.tar]>', type=str, action='store',
         dest='index', required=True, nargs='+', help='index')
-    anchor_reg_parser.add_argument(
+    regcov_parser.add_argument(
         '-r', '--reference', metavar='<reference.fa.gz>', type=str, action='store',
         dest='ref', required=True, help='reference')
-    anchor_reg_parser.add_argument(
+    regcov_parser.add_argument(
         '-c', '--coords', metavar='<chr:start-end>', type=str, action='store',
         dest='coords', required=True, help='genomic coordinates')
-    anchor_reg_parser.add_argument(
+    regcov_parser.add_argument(
         '-o', '--output', metavar='<output.bdg[.gz]>', type=str,
         dest='output', help='write to file instead of standard output')
-    anchor_reg_parser.add_argument(
+    regcov_parser.add_argument(
         '-b', '--bgzip', action='store_true',
         dest='bgzip', help='block compress the output file')
-    anchor_reg_parser.add_argument(
+    regcov_parser.add_argument(
         '-g', '--genes', metavar='<genes.gff3[.gz]>', type=str,
         dest='genes', help='gff file of gene coordinates')
-    anchor_reg_parser.add_argument(
+    regcov_parser.set_defaults(func=run_regcoverage)
+    regcov_parser.add_argument(
         '-f', '--flank', metavar='<int>', type=int, default=0,
         dest='flank', help='size of flanking regions')
-    anchor_reg_parser.add_argument(
+    regcov_parser.add_argument(
         '-p', '--processes', metavar='<int>', type=int, default=1,
         dest='processes', help='number of processes to use')
-    anchor_reg_parser.set_defaults(func=run_anchor_region)
+    regcov_parser.set_defaults(func=run_regcoverage)
 
-    anchor_genome_parser = subparsers.add_parser('anchor-genome',
-        help='anchor k-mers in a genome')
-    anchor_genome_parser.add_argument(
+    genomecov_parser = subparsers.add_parser('genome-coverage',
+        help='generate genomic coverage')
+    genomecov_parser.add_argument(
         '-i', '--index', metavar='<index[.tar]>', type=str, action='store',
         dest='index', required=True, nargs='+', help='index')
-    anchor_genome_parser.add_argument(
+    genomecov_parser.add_argument(
         '-o', '--output', metavar='<output.{pdf,png,svg}>', type=str,
         action='store', dest='output', required=True,
         help='destination file for plot')
-    anchor_genome_parser.add_argument(
+    genomecov_parser.add_argument(
         '-r', '--reference', metavar='<reference.fa.gz>', type=str,
         action='store', dest='ref', required=True,
         help='reference in BGZIP compressed FASTA format')
-    anchor_genome_parser.add_argument(
+    genomecov_parser.add_argument(
         '-c', '--chromosomes', metavar='<chrX>', type=str, action='store',
         dest='chromosomes', required=True, nargs='+',
         help='chromosomes to include')
-    anchor_genome_parser.add_argument(
+    genomecov_parser.add_argument(
         '-t', '--table', metavar='<output-table.tsv>',
         help='output TSV file containing plotted data')
-    anchor_genome_parser.add_argument('--groups', metavar='<"Group">', nargs='+',
+    genomecov_parser.add_argument('--groups', metavar='<"Group">', nargs='+',
         help='list of groups for provided indexes [0]')
-    anchor_genome_parser.add_argument('--title', metavar='<"Plot title">',
+    genomecov_parser.add_argument('--title', metavar='<"Plot title">',
         default='Coverage', help='set the title for the plot')
-    anchor_genome_parser.add_argument('--x-label', metavar='<"Label">',
+    genomecov_parser.add_argument('--x-label', metavar='<"Label">',
         default='Chromosome', help='set the x-axis label for the plot')
-    anchor_genome_parser.add_argument('--legend', action='store_true',
+    genomecov_parser.add_argument('--legend', action='store_true',
         help='include a legend with the plot')
-    anchor_genome_parser.add_argument('--legend-title', metavar='<"Title">',
+    genomecov_parser.add_argument('--legend-title', metavar='<"Title">',
         default='Group', help='title of legend')
-    anchor_genome_parser.add_argument('--legend-loc',
+    genomecov_parser.add_argument('--legend-loc',
         choices=('best', 'upper left', 'upper right', 'lower left',
                  'lower right', 'outside'),
         default='best', help='location of legend [best]')
-    anchor_genome_parser.add_argument('--bin-size', metavar='<int>', type=int, default=0,
+    genomecov_parser.add_argument('--bin-size', metavar='<int>', type=int, default=0,
         choices=(-2,-1,0,1,2),
         help=('Set bin size. The input <int> is converted to the bin size by '
               'the formula: 10^(<int>+6) bp. The default value is 0, i.e. '
               '1-megabase bins. [0]'))
-    anchor_genome_parser.add_argument('--width', metavar='<float>', type=float,
+    genomecov_parser.add_argument('--width', metavar='<float>', type=float,
         default=7.0, help='set width of figure in inches [7]')
-    anchor_genome_parser.add_argument('--height', metavar='<float>', type=float,
-        default=3.0, help='set height of figure in inches [3]')
-    anchor_genome_parser.add_argument('--color-palette', metavar='<#color>', nargs='+',
+    genomecov_parser.add_argument('--height', metavar='<float>', type=float,
+        default=3.0, help='set width of figure in inches [3]')
+    genomecov_parser.add_argument('--color-palette', metavar='<#color>', nargs='+',
         default=COLOR_PALETTE, help='color palette to use')
-    anchor_genome_parser.add_argument('--alpha', metavar='<float>', type=float,
+    genomecov_parser.add_argument('--alpha', metavar='<float>', type=float,
         default=0.5, help='transparency value for lines [0.5]')
-    anchor_genome_parser.add_argument('--linewidth', metavar='<int>', type=int,
+    genomecov_parser.add_argument('--linewidth', metavar='<int>', type=int,
         default=3, help='line width for plot [3]')
-    anchor_genome_parser.add_argument('--processes', metavar='<int>', type=int,
+    genomecov_parser.add_argument('--processes', metavar='<int>', type=int,
         default=1, help='number of processes to use')
-    anchor_genome_parser.set_defaults(func=run_anchor_genome)
+    genomecov_parser.set_defaults(func=run_genome_coverage)
 
-    agplot_parser = subparsers.add_parser('anchor-plot',
-        help='generate a plot from genome anchoring results')
-    agplot_parser.add_argument(
+    gcplot_parser = subparsers.add_parser('gcplot',
+        help='generate a plot from genomic coverage results')
+    gcplot_parser.add_argument(
         '-t', '--table', metavar='<genomecov.tsv>', type=str, action='store',
         dest='table', required=True, help='genomic coverage results')
-    agplot_parser.add_argument(
+    gcplot_parser.add_argument(
         '-o', '--output', metavar='<output.{pdf,png,svg}>', type=str,
         action='store', dest='output', required=True,
         help='destination file for plot')
-    agplot_parser.add_argument('--groups', metavar='<"Group">', nargs='+',
-        help='list of groups for provided indexes')
-    agplot_parser.add_argument('--loci', metavar='<"chr:pos:name">', nargs='+',
-        help='list of loci to mark on plot')
-    agplot_parser.add_argument('--chromsizes', metavar='<file.chrom.sizes>',
+    gcplot_parser.add_argument('--groups', metavar='<"Group">', nargs='+',
+        help='list of groups for provided indexes [0]')
+    gcplot_parser.add_argument('--loci', metavar='<"chr:pos:name">', nargs='+',
+        help='list of loci to mark on plot [0]')
+    gcplot_parser.add_argument('--chromsizes', metavar='<file.chrom.sizes>',
         help='chromsizes file of the reference used to generate the table')
-    agplot_parser.add_argument('--title', metavar='<"Plot title">',
+    gcplot_parser.add_argument('--title', metavar='<"Plot title">',
         help='set the title for the plot')
-    agplot_parser.add_argument('--x-label', metavar='<"Label">',
+    gcplot_parser.add_argument('--x-label', metavar='<"Label">',
         help='set x-axis label for the plot')
-    agplot_parser.add_argument('--legend', action='store_true',
+    gcplot_parser.add_argument('--legend', action='store_true',
         help='include a legend with the plot')
-    agplot_parser.add_argument('--legend-title', metavar='<"Title">',
+    gcplot_parser.add_argument('--legend-title', metavar='<"Title">',
         help='title of legend')
-    agplot_parser.add_argument('--legend-loc',
+    gcplot_parser.add_argument('--legend-loc',
         choices=('best', 'upper left', 'upper right', 'lower left',
                  'lower right', 'outside'),
         default='best', help='location of legend [best]')
-    agplot_parser.add_argument('--width', metavar='<float>', type=float,
+    gcplot_parser.add_argument('--width', metavar='<float>', type=float,
         default=7.0, help='set width of figure in inches [7]')
-    agplot_parser.add_argument('--height', metavar='<float>', type=float,
-        default=3.0, help='set height of figure in inches [3]')
-    agplot_parser.add_argument('--color-palette', metavar='<#color>', nargs='+',
+    gcplot_parser.add_argument('--height', metavar='<float>', type=float,
+        default=3.0, help='set width of figure in inches [3]')
+    gcplot_parser.add_argument('--color-palette', metavar='<#color>', nargs='+',
         default=COLOR_PALETTE, help='color palette to use')
-    agplot_parser.add_argument('--alpha', metavar='<float>', type=float,
+    gcplot_parser.add_argument('--alpha', metavar='<float>', type=float,
         default=0.5, help='transparency value for lines [0.5]')
-    agplot_parser.add_argument('--linewidth', metavar='<int>', type=int,
+    gcplot_parser.add_argument('--linewidth', metavar='<int>', type=int,
         default=3, help='line width for plot [3]')
-    agplot_parser.set_defaults(func=run_anchor_genome_plot)
+    gcplot_parser.set_defaults(func=run_genome_coverage_plot)
 
-    anchor_hm_parser = subparsers.add_parser('anchor-heatmap',
-        help='draw anchor heatmap')
-    anchor_hm_parser.add_argument(
+    covhm_parser = subparsers.add_parser('cov-heatmap',
+        help='draw coverage heatmap')
+    covhm_parser.add_argument(
         '-i', '--index', metavar='<index[.tar]>', type=str, action='store',
         dest='index', required=True, help='index')
-    anchor_hm_parser.add_argument(
+    covhm_parser.add_argument(
         '-r', '--refs', metavar='<reference.fa.gz>', type=str, action='store',
         dest='refs', required=True, nargs='+', help='references')
-    anchor_hm_parser.add_argument(
+    covhm_parser.add_argument(
         '-f', '--features', metavar='<features.gff3>', type=str, action='store',
         dest='features', required=True, nargs='+',
         help='GFF files defining features (such as genes)')
-    anchor_hm_parser.add_argument(
+    covhm_parser.add_argument(
         '-o', '--output', metavar='<output.{pdf,png,svg}>', type=str, action='store',
         dest='output', required=True, help='output file (must end with ".png")')
-    anchor_hm_parser.add_argument(
+    covhm_parser.add_argument(
         '--n-features', metavar='<int>', type=int, action='store',
         dest='n_features',
         help='use to limit plotting to the first n features for each genome')
-    anchor_hm_parser.add_argument(
+    covhm_parser.add_argument(
         '--width', metavar='<float>', type=float, action='store',
         dest='width', default=7, help='width of plot in inches', )
-    anchor_hm_parser.add_argument(
+    covhm_parser.add_argument(
         '--height', metavar='<float>', type=float, action='store',
         dest='height', default=7, help='height of plot in inches', )
-    anchor_hm_parser.set_defaults(func=run_anchor_heatmap)
-
-    anchormap_parser = subparsers.add_parser('anchormap',
-        help='export an anchormap for downstream visualization')
-    anchormap_parser.add_argument(
-        '-i', '--index', metavar='<index[.tar]>', required=True, help='index')
-    anchormap_parser.add_argument(
-        '-o', '--output', metavar='<anchormap_dir/>', required=True,
-        help='output directory for the anchormap')
-    anchormap_parser.add_argument('--anchors', metavar='<anchor.fasta[.gz]>',
-                                  required=True, nargs='+',
-                                  help='the anchor genomes')
-    anchormap_parser.add_argument('--anno', metavar='<anno.gff[.gz]>',
-                                  required=True, nargs='+', help='annotations')
-    anchormap_parser.add_argument(
-        '-t', '--threads', metavar='<int>',
-        type=int, help='Number of threads to use', default=1)
-    anchormap_parser.set_defaults(func=run_anchormap)
-
-    dryrun_parser = subparsers.add_parser('dryrun',
-        help='perform a dry run of indexing and print metadata')
-    dryrun_parser.add_argument(
-        '-g', '--genomes', metavar='<genome[s]{.fa,.fq,.tar,/}>',
-        nargs='+',
-        help='input genomes')
-    dryrun_parser.add_argument(
-        '-p', '--genomes-paired', metavar='<genome[s]{.fa,.fq,.tar,/}>',
-        nargs='+',
-        help='input genomes (paired)')
-    dryrun_parser.add_argument(
-        '--split-memory', metavar='<int>',
-        type=int, help=(
-        'Parallel.'
-        'This splits the indexing into multiple rounds; reducing memory.'
-        ), default=1)
-    dryrun_parser.add_argument(
-        '-t', '--threads', metavar='<int>',
-        type=int, help=('Number of threads to use'), default=1)
-    dryrun_parser.set_defaults(func=run_dryrun)
+    covhm_parser.set_defaults(func=run_coverage_heatmap)
 
     download_parser = subparsers.add_parser('download-example',
         help='download an example dataset')
     download_parser.add_argument(
         '-d', '--dir', metavar='<dir/>', type=str, action='store',
         dest='dir', default=EXAMPLE_DATA_DIR,
         help='destination directory for example data')
     download_parser.add_argument(
-        '-s', '--species', choices=('Spolyrhiza', 'Slycopersicum', 'Zmays', 'Hsapiens', 'Bsubtilis', 'Athaliana'),
-        help=('download publicly available genomes. Species: max_samples. '
-              'Spolyrhiza: 3, Slycopersicum: 46, Zmays: 54, Hsapiens: 94, Bsubtilis: 164, Athaliana: 1135'))
+        '-b', '--bacterial', action='store_true', dest='bacterial',
+        help='if True, download bacterial genomes')
     download_parser.add_argument(
-        '-n', '--n-samples', metavar='<int>', type=int, default=1, action='store', dest='n_samples',
-        help='number of samples to download, must be less than species max [1]')
+        '-n', '--n-samples', metavar='<int>', type=int, action='store', dest='n_samples',
+        help='number of bacterial samples to download, max 164 [1]')
     download_parser.set_defaults(func=run_download_example)
 
     args = parser.parse_args()
+    if args.version:
+        print(__version__)
+        sys.exit()
     args.func(args)
+
+if __name__ == "__main__":
+    main()
```

