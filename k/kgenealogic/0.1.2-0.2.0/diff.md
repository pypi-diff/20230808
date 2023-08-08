# Comparing `tmp/kgenealogic-0.1.2.tar.gz` & `tmp/kgenealogic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgenealogic-0.1.2.tar", max compression
+gzip compressed data, was "kgenealogic-0.2.0.tar", max compression
```

## Comparing `kgenealogic-0.1.2.tar` & `kgenealogic-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-05-22 13:59:12.365697 kgenealogic-0.1.2/LICENSE
--rw-r--r--   0        0        0     3163 2023-08-04 23:23:25.016985 kgenealogic-0.1.2/README.md
--rw-r--r--   0        0        0      295 2023-08-04 23:06:44.187647 kgenealogic-0.1.2/kgenealogic/__init__.py
--rw-r--r--   0        0        0      165 2023-08-04 23:06:51.483712 kgenealogic-0.1.2/kgenealogic/__main__.py
--rw-r--r--   0        0        0     7082 2023-08-04 23:05:48.491160 kgenealogic-0.1.2/kgenealogic/cache.py
--rw-r--r--   0        0        0    10188 2023-08-04 23:06:05.387307 kgenealogic-0.1.2/kgenealogic/cli.py
--rw-r--r--   0        0        0    11818 2023-08-05 23:08:22.473767 kgenealogic-0.1.2/kgenealogic/cluster.py
--rw-r--r--   0        0        0     4891 2023-08-04 23:06:17.307412 kgenealogic-0.1.2/kgenealogic/data.py
--rw-r--r--   0        0        0     4619 2023-08-05 23:05:24.307721 kgenealogic-0.1.2/kgenealogic/files.py
--rw-r--r--   0        0        0   703233 2023-07-28 20:38:53.281601 kgenealogic-0.1.2/kgenealogic/genetmap.csv
--rw-r--r--   0        0        0     3701 2023-07-31 17:22:39.081516 kgenealogic-0.1.2/kgenealogic/schema.py
--rw-r--r--   0        0        0      458 2023-08-06 01:42:25.425994 kgenealogic-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3960 1970-01-01 00:00:00.000000 kgenealogic-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1146 2023-08-07 15:15:15.356183 kgenealogic-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3041 2023-08-06 13:24:46.820586 kgenealogic-0.2.0/README.md
+-rw-r--r--   0        0        0     1012 2023-08-06 13:33:38.425795 kgenealogic-0.2.0/examples/config.yaml
+-rw-r--r--   0        0        0      237 2023-08-06 22:59:13.648864 kgenealogic-0.2.0/kgenealogic/__init__.py
+-rw-r--r--   0        0        0      165 2023-08-04 23:06:51.483712 kgenealogic-0.2.0/kgenealogic/__main__.py
+-rw-r--r--   0        0        0     8615 2023-08-08 01:41:02.229394 kgenealogic-0.2.0/kgenealogic/cli.py
+-rw-r--r--   0        0        0    17927 2023-08-08 02:29:50.834421 kgenealogic-0.2.0/kgenealogic/cluster.py
+-rw-r--r--   0        0        0     8621 2023-08-07 19:18:26.667793 kgenealogic-0.2.0/kgenealogic/data.py
+-rw-r--r--   0        0        0     5934 2023-08-07 19:26:46.108208 kgenealogic-0.2.0/kgenealogic/files.py
+-rw-r--r--   0        0        0   703233 2023-07-28 20:38:53.281601 kgenealogic-0.2.0/kgenealogic/genetmap.csv
+-rw-r--r--   0        0        0     5054 2023-08-07 15:52:52.763714 kgenealogic-0.2.0/kgenealogic/schema.py
+-rw-r--r--   0        0        0      483 2023-08-07 21:38:19.121153 kgenealogic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3838 1970-01-01 00:00:00.000000 kgenealogic-0.2.0/PKG-INFO
```

### Comparing `kgenealogic-0.1.2/README.md` & `kgenealogic-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 
 ## Usage
 
 ```
 python3 -m kgenealogic init [-p <project-file>]
 python3 -m kgenealogic add [-p <project-file>] ... # files to import
-python3 -m kgenealogic build [-p <project-file>] ... # build crossover probability model and find negative triangulations
 python3 -m kgenealogic cluster [-p <project-file>] [-o <out-file>] <config-file>
 
 python3 -m kgenealogic --help # general help
 python3 -m kgenealogic <command> --help # help for <command>, e.g. init/add/build/cluster
 ```
 
 ## Algorithms
```

### Comparing `kgenealogic-0.1.2/kgenealogic/cli.py` & `kgenealogic-0.2.0/kgenealogic/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -88,36 +88,14 @@
                 raise typer.Exit(code=1)
             data = kg_files.read_ged_triangles(path, source)
             kg.import_triangles(engine, data)
         else:
             typer.echo(f"Unrecognized file type: {path}", err=True)
 
 @app.command()
-def build(
-    project: PROJECT_OPTION = DEFAULT_PROJECT,
-    force:  Annotated[bool, typer.Option(help="Force re-build, even if already built")] = False
-):
-    """
-    Process all added data files in preparation for clustering.
-
-    - Uses all segments with provided lengths in order to build a model of crossover probability, to
-    impute cM lengths of derived segments
-
-    - Finds all "negative" triangles, where two target kits have overlapping matching segments on a
-    common source kit, but the segment does not appear as a triangulation for the three kits
-    """
-    engine = sql.create_engine(f"sqlite:///{project}")
-    if not force:
-        if kg.is_cache_valid(engine):
-            typer.echo("Project is already built. Use --force to re-build", err=True)
-            raise typer.Abort()
-
-    kg.build_cache(engine)
-
-@app.command()
 def cluster(
     config: Annotated[Path, typer.Argument(
         file_okay=True,
         dir_okay=False,
         readable=True,
         resolve_path=True,
         help=f"The configuration file describing how to cluster kits",
@@ -139,19 +117,21 @@
     A config file in (strict) YAML format must be provided. An example of such a file is
     distributed with this package. The valid keys for this config file are:
 
     - include: Kit numbers to be included are specified as a list. Each list entry can be either
       (1) just the kit number to be included, as a string, or (2) a mapping indicating a kit number
       and some of its matches to be included. In the second format, the valid keys are
 
-      -- id: the (base) kit number as a string (required)
-      -- matches (optional, floating point): if this is given, it is interpreted as the minimum
+      --- id: the (base) kit number as a string (required)
+
+      --- matches (optional, floating point): if this is given, it is interpreted as the minimum
       length in cM of a match so that if kit2 matches the base kit anywhere with this length, then
       kit2 will also be included
-      -- triangles (optional, floating point): if this is given, it is interpreted as the minimum
+
+      --- triangles (optional, floating point): if this is given, it is interpreted as the minimum
       length in cM of a triangle so that if kit2 participates in a triangle the base kit anywhere
       with this length, with any third kit, then kit2 will also be included.
 
       Seeds are automatically included.
 
     - exclude: Kit numbers to be excluded are specified as a list. E.g., known duplicate kits can
       be specified here, or individuals that are known to not respect the desired tree structure.
@@ -160,85 +140,72 @@
 
     - min_length: Minimum segment length to be considered, in cM. Optional, defaults to 7cM
 
     - tree: A tree giving the desired family structure to be produced, along with any kits known to reside at
       each node of the of the tree. The more accurate seeds are available, the more reliable and
       useful the results will be. This root node of the tree is specified with the "tree" key. At
       each node of the tree, you can optionally specify any of:
+
       1. a "kits" key, associated with a list of kit numbers known to reside at that node of the
       tree. See below for additional options.
+
       2. a "paternal" key, formatted as a node of the tree, specifying the paternal branch
-      2. a "maternal" key, formatted as a node of the tree, specifying the maternal branch
+
+      3. a "maternal" key, formatted as a node of the tree, specifying the maternal branch
       The tree key is required
 
     Entries of each "kits" list of the tree can be specified in one of two ways:
 
     - just the kit number as a string
+
     - a mapping with the following keys:
-      -- id: the kit number as a string (required)
-      -- autox: whether to classify kits that match this kit on the X chromosome as necessarily
+
+      --- id: the kit number as a string (required)
+
+      --- autox: whether to classify kits that match this kit on the X chromosome as necessarily
       maternal (optional, boolean). If the kit corresponds to a male child of the parents
       represented by the paternal and maternal branches of this node of the tree, it makes sense to
       use a value of true. Otherwise omit the key or set it to false (the default)
-      -- negative: whether to use negative triangulations for this node, if available (option,
+
+      --- negative: whether to use negative triangulations for this node, if available (option,
       boolean, default false)
-      -- float: whether to keep the kit at this node of the tree, or attempt to float it into the
+
+      --- float: whether to keep the kit at this node of the tree, or attempt to float it into the
       branches (optional, boolean). If float is false, this seed will be kept at this node of the
       tree - this is desired when the kit is known to be a descendant of the parents represented by
       the maternal and paternal branches at this node. If float is true, this seed will be pushed
       out as far as possible into the branches - this is desired when the kit's relation to the
       root is partially but not completely known (e.g., the kit is some relative of the maternal
       grandfather, but nothing more is known). If float is not set, the default behavior is to
       treat it as false if triangulations are available, and otherwise treat it as true.
 
-    For example:
+    An example configuration file is available in the "examples" directory included with the source
+    of this package.
 
-    exclude: # these kits will be excluded from the clustering
-      - T000001
-      - T000002
-    min_length: 8.5
-    tree:
-      kits:
-        - # me (male)
-          id: T000003
-          autox: true
-          float: false
-          negative: true
-        - # my sister's son
-          id: T000004
-          float: false
-      paternal:
-        kits:
-          - T000004 # my father's grand-niece
-        paternal:
-          kits:
-            - T000005 # a distant cousin on my paternal grandfather's side
-        maternal:
-          # I don't know any relatives of my paternal grandmother, but I'd like any that are
-          # discovered to be present in the output
-      maternal:
-        kits:
-          - T000006 # a relative of my mother, but not my father, with no other information
 
     This will produce an output file separating my maternal and paternal relatives, with the
     paternal relatives further split into paternal grandfather and paternal grandmother relatives.
     The output file will be a CSV file with several columns:
+
     - kit, specifying the kit number
+
     - ahnentafel, the ahnentafel number of the most distant relative of the root to which the kit
       is determiend to be related
+
+    - seed, the ahnentafel number of the node at which this kit was listed as a seed, if any
+
     - label<n>, where n varies from 0 to depth of the tree minus 1. This is 'M' if the kit is put
       on the maternal side at that depth, and P if it is put on the paternal side. The list of
       these labels is equivalent to the value in the ahnentafel field
+
     - confidence<n>, a number between 0 and 1 indicating a rough confidence with which the kit is
-      given label<n>. These numbers should not be interpreted as probabilities. A value of 1
+      given label<n>. These numbers should NOT be interpreted as probabilities. A value of 1
       indicates that all of the kit's matches have labels consistent with the kit's label at this
       depth.
+
     """
 
     engine = sql.create_engine(f"sqlite:///{project}")
-    if not kg.is_cache_valid(engine):
-        typer.echo("Project is not yet built. First run kgenealogic build", err=True)
-        raise typer.Abort()
     config = kg_files.read_cluster_config(config)
     clusters = kg.cluster_data(engine, config)
     kg_files.write_clusters(clusters, outfile)
```

### Comparing `kgenealogic-0.1.2/kgenealogic/files.py` & `kgenealogic-0.2.0/kgenealogic/files.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,21 +13,23 @@
     'B37End': 'end',
     'Segment cM': 'length',
     'MatchedName': 'name',
     'Matched Sex': 'sex',
     'MatchedEmail': 'email',
 }
 def is_ged_matches(path):
+    """Check if file at path is a valid GEDmatch pairwise matches file."""
     try:
         csv = pd.read_csv(path, dtype=str)
     except:
         return False
     return set(GED_MATCH_COLS.keys()).issubset(csv.columns)
 
 def read_ged_matches(path):
+    """Load GEDmatch pairwise matches file into pandas dataframe."""
     dtype = defaultdict(lambda: str)
     dtype['B37Start'] = int
     dtype['B37End'] = int
     matches = pd.read_csv(path, dtype=dtype)
     return matches[GED_MATCH_COLS.keys()].rename(columns=GED_MATCH_COLS)
 
 GED_TRIANGLE_COLS = {
@@ -39,29 +41,41 @@
     'Kit2 Email': 'email3',
     'Chr': 'chromosome',
     'B37 Start': 'start',
     'B37 End': 'end',
     'cM': 'length',
 }
 def is_ged_triangles(path):
+    """Check if file at path is a valid GEDmatch triangulation file."""
     try:
         csv = pd.read_csv(path, dtype=str)
     except:
         return False
     return set(GED_TRIANGLE_COLS.keys()).issubset(csv.columns)
 
 def read_ged_triangles(path, primary_kit):
+    """Load GEDmatch triangulation file into pandas dataframe.
+
+    Args:
+        path: path to the file
+        primary_kit: the kit from which the triangulations were generated
+
+    Returns:
+        A pandas dataframe in the format expected by data.import_triangles.
+        Specifically, primary_kit will appear as kit1 in the dataframe
+    """
     dtype = defaultdict(lambda: str)
     dtype['B37 Start'] = int
     dtype['B37 End'] = int
     tri = pd.read_csv(path, dtype=dtype)
     tri = tri[GED_TRIANGLE_COLS.keys()].rename(columns=GED_TRIANGLE_COLS)
     tri['kit1'] = primary_kit
     return tri
 
+# StrictYAML schemas used for cluster config files
 CLUSTER_KIT_SCHEMA = yaml.Str() | yaml.Map({
     'id': yaml.Str(),
     yaml.Optional('autox', default=False): yaml.Bool(),
     yaml.Optional('float', default=None, drop_if_none=False): yaml.EmptyNone() | yaml.Bool(),
     yaml.Optional('negative', default=None, drop_if_none=False): yaml.EmptyNone() | yaml.Bool(),
 })
 CLUSTER_INCLUDE_SCHEMA = yaml.Str() | yaml.Map({
@@ -87,14 +101,23 @@
     include: list[dict[str, typing.Any]]
     exclude: list[str]
     min_length: float
     tree: dict[str, typing.Any]
     seeds: set[str]
 
 def validate_config_tree(config, seeds):
+    """Recursively validate the StrictYAML tree schema and extract all seeds.
+
+    Seeds that appear in the config file as strings are expanded to dictionaries with default
+    values for the keys.
+
+    Args:
+        config: the StrictYAML document at the current node of the tree
+        seeds: the list of all encountered seeds
+    """
     expanded_kits = []
     for k in config.data.get('kits', []):
         if type(k)==str:
             expanded_kits.append(dict(id=k, autox=False, float=None, negative=False))
         else:
             expanded_kits.append(k)
     config['kits']=expanded_kits
@@ -102,14 +125,24 @@
 
     for branch in ('maternal', 'paternal'):
         if branch in config.data:
             config[branch].revalidate(yaml.EmptyDict() | CLUSTER_TREE_SCHEMA)
             validate_config_tree(config[branch], seeds)
 
 def read_cluster_config(path):
+    """Parse a clustering config file in StrictYAML format.
+
+    The schema is given above in code, and is documented in the cluster CLI command.
+
+    Args:
+        path: path to the cluster config file
+
+    Returns:
+        A ClusterConfig object representing the contents of the config file
+    """
     with open(path) as f:
         config_yaml = f.read()
     parsed = yaml.load(config_yaml, CLUSTER_CONFIG_SCHEMA)
     seeds = []
     validate_config_tree(parsed['tree'], seeds)
     exclude = parsed.data.get('exclude', [])
 
@@ -139,8 +172,9 @@
         min_length=parsed.data.get('min_length', 7.),
         tree=parsed['tree'].data,
         seeds=unique_seeds,
     )
     return result
 
 def write_clusters(clusters, path):
+    """Write out the results of clustering to a CSV file."""
     clusters.to_csv(path, index=False)
```

### Comparing `kgenealogic-0.1.2/kgenealogic/genetmap.csv` & `kgenealogic-0.2.0/kgenealogic/genetmap.csv`

 * *Files identical despite different names*

### Comparing `kgenealogic-0.1.2/PKG-INFO` & `kgenealogic-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgenealogic
-Version: 0.1.2
+Version: 0.2.0
 Summary: Genetic genealogy tool for tree structure inference
 License: MIT
 Author: John Wilmes
 Author-email: jw@johnwilmes.name
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -42,15 +42,14 @@
 
 
 ## Usage
 
 ```
 python3 -m kgenealogic init [-p <project-file>]
 python3 -m kgenealogic add [-p <project-file>] ... # files to import
-python3 -m kgenealogic build [-p <project-file>] ... # build crossover probability model and find negative triangulations
 python3 -m kgenealogic cluster [-p <project-file>] [-o <out-file>] <config-file>
 
 python3 -m kgenealogic --help # general help
 python3 -m kgenealogic <command> --help # help for <command>, e.g. init/add/build/cluster
 ```
 
 ## Algorithms
```

