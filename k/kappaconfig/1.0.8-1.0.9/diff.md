# Comparing `tmp/kappaconfig-1.0.8.tar.gz` & `tmp/kappaconfig-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappaconfig-1.0.8.tar", last modified: Mon Jun 13 20:38:11 2022, max compression
+gzip compressed data, was "kappaconfig-1.0.9.tar", last modified: Wed Jun 15 20:19:15 2022, max compression
```

## Comparing `kappaconfig-1.0.8.tar` & `kappaconfig-1.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 20:38:11.386365 kappaconfig-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-06-13 20:38:11.386365 kappaconfig-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3999 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 20:38:11.382365 kappaconfig-1.0.8/kappaconfig/
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-06-13 20:37:56.000000 kappaconfig-1.0.8/kappaconfig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 20:38:11.382365 kappaconfig-1.0.8/kappaconfig/entities/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/entities/grammar_tree_nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1783 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/entities/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 20:38:11.382365 kappaconfig-1.0.8/kappaconfig/functional/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/functional/convert.py
--rw-r--r--   0 runner    (1001) docker     (121)     3547 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/functional/dotlist.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/functional/load.py
--rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/functional/parse_grammar.py
--rw-r--r--   0 runner    (1001) docker     (121)     3788 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/functional/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 20:38:11.382365 kappaconfig-1.0.8/kappaconfig/resolvers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 20:38:11.382365 kappaconfig-1.0.8/kappaconfig/resolvers/collection_resolvers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/collection_resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/collection_resolvers/collection_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/collection_resolvers/missing_value_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)     4296 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/collection_resolvers/template_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/default_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 20:38:11.382365 kappaconfig-1.0.8/kappaconfig/resolvers/post_processors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/post_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/post_processors/post_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/post_processors/remove_nones_post_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/post_processors/remove_vars_post_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)     7548 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 20:38:11.386365 kappaconfig-1.0.8/kappaconfig/resolvers/scalar_resolvers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/scalar_resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/scalar_resolvers/eval_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/scalar_resolvers/interpolation_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/scalar_resolvers/nested_yaml_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/scalar_resolvers/scalar_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/kappaconfig/resolvers/scalar_resolvers/select_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 20:38:11.382365 kappaconfig-1.0.8/kappaconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-06-13 20:38:10.000000 kappaconfig-1.0.8/kappaconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1570 2022-06-13 20:38:11.000000 kappaconfig-1.0.8/kappaconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-13 20:38:10.000000 kappaconfig-1.0.8/kappaconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-06-13 20:38:11.000000 kappaconfig-1.0.8/kappaconfig.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-06-13 20:38:11.386365 kappaconfig-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 20:38:11.386365 kappaconfig-1.0.8/tests_integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/tests_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2699 2022-06-13 20:37:53.000000 kappaconfig-1.0.8/tests_integration/test_complex_yamls.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 20:19:15.385998 kappaconfig-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-06-15 20:19:15.385998 kappaconfig-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3999 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 20:19:15.381998 kappaconfig-1.0.9/kappaconfig/
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2022-06-15 20:18:57.000000 kappaconfig-1.0.9/kappaconfig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 20:19:15.381998 kappaconfig-1.0.9/kappaconfig/entities/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      908 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/entities/grammar_tree_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2195 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/entities/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 20:19:15.381998 kappaconfig-1.0.9/kappaconfig/functional/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/functional/convert.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3611 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/functional/dotlist.py
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/functional/load.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/functional/parse_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3788 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/functional/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 20:19:15.381998 kappaconfig-1.0.9/kappaconfig/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 20:19:15.381998 kappaconfig-1.0.9/kappaconfig/resolvers/collection_resolvers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/collection_resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/collection_resolvers/collection_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/collection_resolvers/missing_value_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4296 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/collection_resolvers/template_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/default_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 20:19:15.385998 kappaconfig-1.0.9/kappaconfig/resolvers/post_processors/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/post_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/post_processors/post_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/post_processors/remove_nones_post_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/post_processors/remove_vars_post_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7548 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 20:19:15.385998 kappaconfig-1.0.9/kappaconfig/resolvers/scalar_resolvers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/scalar_resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/scalar_resolvers/eval_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/scalar_resolvers/interpolation_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/scalar_resolvers/nested_yaml_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/scalar_resolvers/scalar_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (121)      585 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/kappaconfig/resolvers/scalar_resolvers/select_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 20:19:15.381998 kappaconfig-1.0.9/kappaconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-06-15 20:19:14.000000 kappaconfig-1.0.9/kappaconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1570 2022-06-15 20:19:15.000000 kappaconfig-1.0.9/kappaconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-15 20:19:14.000000 kappaconfig-1.0.9/kappaconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-06-15 20:19:15.000000 kappaconfig-1.0.9/kappaconfig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      641 2022-06-15 20:19:15.385998 kappaconfig-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 20:19:15.385998 kappaconfig-1.0.9/tests_integration/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/tests_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2699 2022-06-15 20:18:54.000000 kappaconfig-1.0.9/tests_integration/test_complex_yamls.py
```

### Comparing `kappaconfig-1.0.8/LICENSE` & `kappaconfig-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kappaconfig-1.0.8/PKG-INFO` & `kappaconfig-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappaconfig
-Version: 1.0.8
+Version: 1.0.9
 Summary: flexible yaml configuration framework
 Home-page: https://github.com/BenediktAlkin/KappaConfig
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaConfig
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaConfig/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kappaconfig-1.0.8/README.md` & `kappaconfig-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kappaconfig-1.0.8/kappaconfig/__init__.py` & `kappaconfig-1.0.9/kappaconfig/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 from .resolvers.default_resolver import DefaultResolver
 from .resolvers.resolver import Resolver
 from .resolvers.scalar_resolvers.scalar_resolver import ScalarResolver
 from .resolvers.collection_resolvers.collection_resolver import CollectionResolver
 from .resolvers.post_processors.post_processor import PostProcessor
 
-from .functional.load import from_string, from_file_uri, from_cli, from_primitive
+from .functional.load import from_string, from_file_uri, from_cli
 from .functional.util import merge, mask_in, mask_out
-from .functional.dotlist import from_dotlist, to_dotlist
+from .functional.dotlist import from_dotlist, to_dotlist
+from .functional.convert import from_primitive, to_primitive
```

### Comparing `kappaconfig-1.0.8/kappaconfig/entities/grammar_tree_nodes.py` & `kappaconfig-1.0.9/kappaconfig/entities/grammar_tree_nodes.py`

 * *Files identical despite different names*

### Comparing `kappaconfig-1.0.8/kappaconfig/entities/wrappers.py` & `kappaconfig-1.0.9/kappaconfig/entities/wrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     def __init__(self, value):
         super().__init__()
         self.value = value
 
     def __repr__(self):
         return repr(self.value)
 
+    def __eq__(self, other):
+        return type(self) == type(other) and self.value == other.value
+
 class KCDict(KCObject):
     def __init__(self, **kwargs):
         super().__init__()
         self.dict = kwargs
 
     def __repr__(self):
         return repr(self.dict)
@@ -35,14 +38,17 @@
 
     def items(self):
         return self.dict.items()
 
     def pop(self, key):
         return self.dict.pop(key)
 
+    def __eq__(self, other):
+        return type(self) == type(other) and self.dict == other.dict
+
 
 class KCList(KCObject):
     def __init__(self, *args):
         super().__init__()
         self.list = list(args)
 
     def __repr__(self):
@@ -65,7 +71,16 @@
 
     def __iadd__(self, other):
         if not isinstance(other, KCList):
             from ..errors import unexpected_type_error
             raise unexpected_type_error(KCList, other)
         self.list += other.list
         return self.list
+
+    def __len__(self):
+        return len(self.list)
+
+    def append(self, item):
+        self.list.append(item)
+
+    def __eq__(self, other):
+        return type(self) == type(other) and self.list == other.list
```

### Comparing `kappaconfig-1.0.8/kappaconfig/errors.py` & `kappaconfig-1.0.9/kappaconfig/errors.py`

 * *Files identical despite different names*

### Comparing `kappaconfig-1.0.8/kappaconfig/functional/convert.py` & `kappaconfig-1.0.9/kappaconfig/functional/convert.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,7 +11,21 @@
 def _from_primitive_fn(node, parent_node, parent_accessor, **_):
     if isinstance(node, dict):
         parent_node[parent_accessor] = KCDict(**node)
     elif isinstance(node, list):
         parent_node[parent_accessor] = KCList(*node)
     elif not isinstance(node, (KCDict, KCList, KCScalar)):
         parent_node[parent_accessor] = KCScalar(node)
+
+def to_primitive(root_node):
+    root_node = deepcopy(root_node)
+    wrapped_node = dict(root=root_node)
+    apply(root_node, parent_node=wrapped_node, parent_accessor="root", pre_fn=_to_primitive_fn)
+    return wrapped_node["root"]
+
+def _to_primitive_fn(node, parent_node, parent_accessor, **_):
+    if isinstance(node, KCDict):
+        parent_node[parent_accessor] = dict(**node.dict)
+    elif isinstance(node, KCList):
+        parent_node[parent_accessor] = [*node.list]
+    elif isinstance(node, KCScalar):
+        parent_node[parent_accessor] = node.value
```

### Comparing `kappaconfig-1.0.8/kappaconfig/functional/dotlist.py` & `kappaconfig-1.0.9/kappaconfig/functional/dotlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .util import apply, accessors_to_string, string_to_accessors
-from ..entities.wrappers import KCObject
+from ..entities.wrappers import KCObject, KCList, KCDict, KCScalar
 import yaml
 
 def from_dotlist(dotlist):
-    result = dict(root={})
+    result = dict(root=KCDict())
     for entry in dotlist:
         accessor_value_split = entry.split("=")
         if len(accessor_value_split) != 2:
             from..errors import dotlist_entry_requires_equal_sign_error
             raise dotlist_entry_requires_equal_sign_error()
         accessor_string, value = accessor_value_split
         accessors = string_to_accessors(accessor_string)
@@ -26,37 +26,37 @@
 
             # create missing datastructures
             if isinstance(next_accessor, int):
                 # create list (if it doesn't exist already)
                 if isinstance(cur_accessor, int):
                     prev_node.append([])
                 elif cur_accessor not in prev_node:
-                    prev_node[cur_accessor] = []
+                    prev_node[cur_accessor] = KCList()
             else:
                 # create dict (if it doesn't exist already)
                 if isinstance(cur_accessor, int):
                     prev_node.append({})
                 elif cur_accessor not in prev_node:
-                    prev_node[cur_accessor] = {}
+                    prev_node[cur_accessor] = KCDict()
 
             # progress to next accessor
             prev_node = prev_node[cur_accessor]
 
         # parse value
         parsed_value = yaml.safe_load(value)
 
         # insert current value
         last_accessor = accessors[-1]
         if isinstance(last_accessor, int):
             if len(prev_node) != last_accessor:
                 from ..errors import dotlist_requires_sequential_insert_error
                 raise dotlist_requires_sequential_insert_error()
-            prev_node.append(parsed_value)
+            prev_node.append(KCScalar(parsed_value))
         else:
-            prev_node[last_accessor] = parsed_value
+            prev_node[last_accessor] = KCScalar(parsed_value)
 
     return result["root"]
 
 
 def to_dotlist(root_node):
     if isinstance(root_node, KCObject):
         from ..errors import requires_primitive_node_error
```

### Comparing `kappaconfig-1.0.8/kappaconfig/functional/load.py` & `kappaconfig-1.0.9/kappaconfig/functional/load.py`

 * *Files identical despite different names*

### Comparing `kappaconfig-1.0.8/kappaconfig/functional/parse_grammar.py` & `kappaconfig-1.0.9/kappaconfig/functional/parse_grammar.py`

 * *Files identical despite different names*

### Comparing `kappaconfig-1.0.8/kappaconfig/functional/util.py` & `kappaconfig-1.0.9/kappaconfig/functional/util.py`

 * *Files identical despite different names*

### Comparing `kappaconfig-1.0.8/kappaconfig/resolvers/collection_resolvers/template_resolver.py` & `kappaconfig-1.0.9/kappaconfig/resolvers/collection_resolvers/template_resolver.py`

 * *Files identical despite different names*

### Comparing `kappaconfig-1.0.8/kappaconfig/resolvers/default_resolver.py` & `kappaconfig-1.0.9/kappaconfig/resolvers/default_resolver.py`

 * *Files identical despite different names*

### Comparing `kappaconfig-1.0.8/kappaconfig/resolvers/post_processors/remove_nones_post_processor.py` & `kappaconfig-1.0.9/kappaconfig/resolvers/post_processors/remove_nones_post_processor.py`

 * *Files identical despite different names*

### Comparing `kappaconfig-1.0.8/kappaconfig/resolvers/resolver.py` & `kappaconfig-1.0.9/kappaconfig/resolvers/resolver.py`

 * *Files identical despite different names*

### Comparing `kappaconfig-1.0.8/kappaconfig/resolvers/scalar_resolvers/nested_yaml_resolver.py` & `kappaconfig-1.0.9/kappaconfig/resolvers/scalar_resolvers/nested_yaml_resolver.py`

 * *Files identical despite different names*

### Comparing `kappaconfig-1.0.8/kappaconfig/resolvers/scalar_resolvers/select_resolver.py` & `kappaconfig-1.0.9/kappaconfig/resolvers/scalar_resolvers/select_resolver.py`

 * *Files identical despite different names*

### Comparing `kappaconfig-1.0.8/kappaconfig.egg-info/PKG-INFO` & `kappaconfig-1.0.9/kappaconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappaconfig
-Version: 1.0.8
+Version: 1.0.9
 Summary: flexible yaml configuration framework
 Home-page: https://github.com/BenediktAlkin/KappaConfig
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaConfig
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaConfig/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kappaconfig-1.0.8/kappaconfig.egg-info/SOURCES.txt` & `kappaconfig-1.0.9/kappaconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kappaconfig-1.0.8/setup.cfg` & `kappaconfig-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.0.8
+version = 1.0.9
 name = kappaconfig
 description = flexible yaml configuration framework
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BenediktAlkin/KappaConfig
 project_urls = 
 	Source Code = https://github.com/BenediktAlkin/KappaConfig
```

### Comparing `kappaconfig-1.0.8/tests_integration/test_complex_yamls.py` & `kappaconfig-1.0.9/tests_integration/test_complex_yamls.py`

 * *Files identical despite different names*

