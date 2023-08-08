# Comparing `tmp/pyoak-1.0.0.tar.gz` & `tmp/pyoak-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoak-1.0.0.tar", max compression
+gzip compressed data, was "pyoak-1.1.0.tar", max compression
```

## Comparing `pyoak-1.0.0.tar` & `pyoak-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1068 2023-07-30 19:48:44.096164 pyoak-1.0.0/LICENSE
--rw-r--r--   0        0        0     3776 2023-07-30 19:48:44.096164 pyoak-1.0.0/README.md
--rw-r--r--   0        0        0     2683 2023-07-30 19:48:44.096164 pyoak-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      122 2023-07-30 19:48:44.096164 pyoak-1.0.0/src/pyoak/__init__.py
--rw-r--r--   0        0        0     5606 2023-07-30 19:48:44.096164 pyoak-1.0.0/src/pyoak/error.py
--rw-r--r--   0        0        0     1189 2023-07-30 19:48:44.096164 pyoak-1.0.0/src/pyoak/file.py
--rw-r--r--   0        0        0     6409 2023-07-30 19:48:44.096164 pyoak-1.0.0/src/pyoak/helpers.py
--rw-r--r--   0        0        0        0 2023-07-30 19:48:44.096164 pyoak-1.0.0/src/pyoak/match/__init__.py
--rw-r--r--   0        0        0      726 2023-07-30 19:48:44.096164 pyoak-1.0.0/src/pyoak/match/error.py
--rw-r--r--   0        0        0     1110 2023-07-30 19:48:44.096164 pyoak-1.0.0/src/pyoak/match/grammar.py
--rw-r--r--   0        0        0     1612 2023-07-30 19:48:44.096164 pyoak-1.0.0/src/pyoak/match/helpers.py
--rw-r--r--   0        0        0    37790 2023-07-30 19:48:44.096164 pyoak-1.0.0/src/pyoak/match/pattern.py
--rw-r--r--   0        0        0     6036 2023-07-30 19:48:44.096164 pyoak-1.0.0/src/pyoak/match/xpath.py
--rw-r--r--   0        0        0    68459 2023-07-30 19:48:44.096164 pyoak-1.0.0/src/pyoak/node.py
--rw-r--r--   0        0        0    22331 2023-07-30 19:48:44.096164 pyoak-1.0.0/src/pyoak/origin.py
--rw-r--r--   0        0        0        0 2023-07-30 19:48:44.096164 pyoak-1.0.0/src/pyoak/py.typed
--rw-r--r--   0        0        0    13537 2023-07-30 19:48:44.096164 pyoak-1.0.0/src/pyoak/serialize.py
--rw-r--r--   0        0        0     4691 1970-01-01 00:00:00.000000 pyoak-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-08 21:27:53.621445 pyoak-1.1.0/LICENSE
+-rw-r--r--   0        0        0    20693 2023-08-08 21:27:53.621445 pyoak-1.1.0/README.md
+-rw-r--r--   0        0        0     2690 2023-08-08 21:27:53.625445 pyoak-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/__init__.py
+-rw-r--r--   0        0        0     5606 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/error.py
+-rw-r--r--   0        0        0     1189 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/file.py
+-rw-r--r--   0        0        0     6409 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/helpers.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/match/__init__.py
+-rw-r--r--   0        0        0      726 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/match/error.py
+-rw-r--r--   0        0        0     1110 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/match/grammar.py
+-rw-r--r--   0        0        0     1612 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/match/helpers.py
+-rw-r--r--   0        0        0    37790 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/match/pattern.py
+-rw-r--r--   0        0        0     6036 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/match/xpath.py
+-rw-r--r--   0        0        0    70095 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/node.py
+-rw-r--r--   0        0        0    22983 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/origin.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/py.typed
+-rw-r--r--   0        0        0    13537 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/serialize.py
+-rw-r--r--   0        0        0    21611 1970-01-01 00:00:00.000000 pyoak-1.1.0/PKG-INFO
```

### Comparing `pyoak-1.0.0/LICENSE` & `pyoak-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoak-1.0.0/pyproject.toml` & `pyoak-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyoak"
-version = "1.0.0"
+version = "1.1.0"
 homepage = "https://github.com/mishamsk/pyoak"
 description = "Library for building and working with arbitrary ASTs on top dataclasses"
 authors = ["Mike Perlov <mishamsk@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     'Development Status :: 5 - Production/Stable',
@@ -14,21 +14,21 @@
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
 packages = [{ include = "pyoak", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.10"
-rich = "^13.5.0"
+rich = ">=12.5.0, <14"
 mashumaro = ">=3.8.1,<3.9"
-lark = "1.1.5"
-pyyaml = "^6.0.1"
-orjson = "^3.9.2"
-msgpack = "^1.0.5"
-chardet = "^5.1.0"
+lark = "^1.1.5"
+pyyaml = "^6.0.0"
+orjson = "^3.8.7"
+msgpack = "^1.0.4"
+chardet = "^5.0.0"
 
 [tool.poetry.group.dev.dependencies]
 bump2version = "^1.0.1"
 tox = "^4.6.4"
 tox-gh-actions = "^3.1.3"
 
 [tool.poetry.group.pre.dependencies]
```

### Comparing `pyoak-1.0.0/src/pyoak/error.py` & `pyoak-1.1.0/src/pyoak/error.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.0.0/src/pyoak/file.py` & `pyoak-1.1.0/src/pyoak/file.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.0.0/src/pyoak/helpers.py` & `pyoak-1.1.0/src/pyoak/helpers.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.0.0/src/pyoak/match/error.py` & `pyoak-1.1.0/src/pyoak/match/error.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.0.0/src/pyoak/match/grammar.py` & `pyoak-1.1.0/src/pyoak/match/grammar.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.0.0/src/pyoak/match/helpers.py` & `pyoak-1.1.0/src/pyoak/match/helpers.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.0.0/src/pyoak/match/pattern.py` & `pyoak-1.1.0/src/pyoak/match/pattern.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.0.0/src/pyoak/match/xpath.py` & `pyoak-1.1.0/src/pyoak/match/xpath.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.0.0/src/pyoak/node.py` & `pyoak-1.1.0/src/pyoak/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,22 +127,21 @@
     """A base class for all AST Node classes.
 
     Provides the following functions:
         - Maintains a weakref dictionary of all nodes, accessible through the class methods `get` and `get_any`
         - Maintains a parent-child relationship between nodes
         - Methods for replacing attributes or whole nodes
         - Various tree walking methods
-        - Visitor API (visit method)
+        - Visitor API (accept method)
         - Serialization & deserialization
         - rich console API support (for printing)
 
     Notes:
         - Subclasses must be dataclasses
         - Only fields with subclasses of ASTNode or tuples/lists of ASTNode subclasses are considered children
-        - fields starting with "_" are not serialized
 
     Raises:
         ASTNodeError: If there are children with a different parent alredy assigned (every AST node can only have one parent)
 
     """
 
     _nodes: t.ClassVar[weakref.WeakValueDictionary[str, ASTNode]] = weakref.WeakValueDictionary()
@@ -553,26 +552,50 @@
     @classmethod
     def get(
         cls: t.Type[ASTNodeType],
         id: str,
         default: ASTNodeType | None = None,
         strict: bool = True,
     ) -> ASTNodeType | None:
+        """Gets a node of this class type from the AST registry.
+
+        Args:
+            id (str): The id of the node to get
+            default (ASTNodeType | None, optional): The default value to return if the node is not found.
+                Defaults to None.
+            strict (bool, optional): If True, only a node of this class type is returned.
+                Otherwise an instnace if any subclass is allowed. Defaults to True.
+
+        Returns:
+            ASTNodeType | None: The node if found, otherwise the default value
+
+        """
         ret = ASTNode._nodes.get(id, default)
         if ret is None:
             return None
         elif strict and not type(ret) == cls:
             return None
         elif not strict and not isinstance(ret, cls):
             return None
         else:
             return t.cast(ASTNodeType, ret)
 
     @classmethod
     def get_any(cls, id: str, default: ASTNode | None = None) -> ASTNode | None:
+        """Gets a node of any type from the AST registry by id.
+
+        Args:
+            id (str): The id of the node to get
+            default (ASTNode | None, optional): The default value to return if the node is not found.
+                Defaults to None.
+
+        Returns:
+            ASTNode | None: The node if found, otherwise the default value
+
+        """
         return ASTNode._nodes.get(id, default)
 
     def attach(self) -> None:
         """Attaches this node and all of it's detached children to the AST registry.
 
         Raises:
             ASTNodeRegistryCollisionError: If this node's or any of the subtree node id's
@@ -938,14 +961,19 @@
             object.__setattr__(ret, "original_id", self.id)
         else:
             object.__setattr__(ret, "original_id", self.original_id)
 
         return ret
 
     def calculate_xpath(self) -> bool:
+        """Calculates the xpath of this node and all its children.
+
+        This is a legacy method. The use of match.xpath module is preferred.
+
+        """
         if not self.is_attached_root:
             logger.debug("Cannot calculate xpath for a non-root node")
             return False
 
         # Calculate the xpath of this node (root)
         xpath = f"/@root[0]{self.__class__.__name__}"
 
@@ -1000,14 +1028,17 @@
         else:
             return parent_index
 
     @property
     def xpath(self) -> str | None:
         """Returns the last calculated xpath of this node.
 
+        This is the legacy xpath that may be removed in the future.
+        The recommended way of matching nodes by xpath is via the match.xpath module.
+
         To calculate the xpath, use `calculate_xpath` or root node.
 
         Returns None if xpath wasn't calculated.
 
         """
         # Since we are dynamically assigning the parent fields
         # we need to use getattr to make typing happy
@@ -1434,14 +1465,15 @@
             # Always skip children
             if self._is_field_child(f):
                 continue
 
             yield getattr(self, f.name), f
 
     def get_child_nodes(self) -> t.Iterable[ASTNode]:
+        """Returns a generator object which yields all child nodes."""
         for f in fields(self):
             # Skip non-child fields
             if not self._is_field_child(f):
                 continue
 
             objects = self._ensure_iterable(getattr(self, f.name))
             for o in objects:
@@ -1510,19 +1542,14 @@
                 child._rich(tree, f)
 
         return tree
 
     __hash__ = None  # type: ignore # Make sure even frozen dataclasses will not be hashable
 
     def __init_subclass__(cls) -> None:
-        """Register subclasses and enforce hash function by object ID to all ASTNode subclasses.
-
-        Dataclasses by default will remove hashing by ID, but we want it back for ASTNodes.
-
-        """
         cls.__hash__ = None  # type: ignore # Make sure even frozen dataclasses will not be hashable
 
         # Make sure each class uses it's own list of child fields & properties
         # We do not set them until first access due forwared references
         # that may not be resolved yet.
         cls._props = None
         cls._child_fields = None
@@ -1611,14 +1638,19 @@
             as context.
 
     """
 
     def _transform_children(
         self, node: ASTNode
     ) -> t.Mapping[str, ASTNode | None | list[ASTNode] | tuple[ASTNode, ...]]:
+        """Transforms the children of a given node and returns a mapping of field names to changes.
+
+        This mapping can be passed to ASTNode.replace method.
+
+        """
         changes: dict[str, ASTNode | None | list[ASTNode] | tuple[ASTNode, ...]] = {}
         field_names_with_changes = set()
 
         # Iterate over all child nodes and collect changes
         for child, f, index in node.get_child_nodes_with_field():
             fname = f.name
             if index is not None:
@@ -1688,14 +1720,27 @@
             ASTNode | None: The transformed node or None if the node was
             removed.
 
         """
         return self.transform(node)
 
     def transform(self, node: ASTNode) -> ASTNode | None:
+        """Transforms a given node and returns the transformed node or None if the node was removed.
+
+        Args:
+            node (ASTNode): The node to transform
+
+        Returns:
+            ASTNode | None: The transformed node or None if the node was removed.
+
+        Raises:
+            ASTTransformError: If the transformation fails with the original exception
+                as context.
+
+        """
         orig_node: ASTNode | None = None
 
         # If we are transforming an attached tree or subtree
         # we create a fully detached clone, transform it
         # and then replace the original node with the transformed one.
         # but only if transformation was successful.
         if not node.detached:
```

### Comparing `pyoak-1.0.0/src/pyoak/origin.py` & `pyoak-1.1.0/src/pyoak/origin.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,16 +31,14 @@
     @abstractmethod
     def fqn(self) -> str:
         ...
 
 
 # -----------------------------------------------------------------------------
 # --------------------- Source bases & constants ---------------------------
-SourceType = t.TypeVar("SourceType", bound="Source")
-
 SOURCE_OPTIMIZED_SERIALIZATION_KEY = "source_optimized_serialization"
 """Use with (de)serialation functions via `serialization_options` to enable/disable optimized
 serialization of sources.
 
 When enabled, source serializaes as a single integer, which is the index
 of the source in the registry of all sources.
 
@@ -88,33 +86,38 @@
 
     def _serialize(self) -> dict[str, t.Any]:
         if self._get_serialization_options().get(SOURCE_OPTIMIZED_SERIALIZATION_KEY, False):
             return {"idx": Source._sources[self]}
         return super()._serialize()
 
     @classmethod
-    def _deserialize(cls: t.Type[SourceType], data: dict[str, t.Any]) -> SourceType:
-        if cls._get_deserialization_options().get(SOURCE_OPTIMIZED_SERIALIZATION_KEY, False):
-            idx = data.get("idx")
-            if idx is None:
-                raise ValueError("Missing idx in serialized source data")
-            ret: SourceType | None = None
-            for source, source_idx in Source._sources.items():
-                if source_idx == idx:
-                    return t.cast(SourceType, source)
-
-            if ret is None:
-                raise ValueError(
-                    f"Source with idx {idx} not found in registry. Did you forget to load sources?"
-                )
-        # This may return not the object in the registry, but a new instance
-        # if the same source was previously in the registry
-        obj = super()._deserialize(data)
+    def _deserialize(cls, data: dict[str, t.Any]) -> Source:
+        if data == {}:
+            return NoSource()
+
+        # Try to deserialize as optimized serialization
+        idx = data.get("idx")
+
+        if idx is None:
+            # This may return not the object in the registry, but a new instance
+            # if the same source was previously in the registry
+            obj = super()._deserialize(data)
+
+            idx = obj.source_registry_id
+        elif not isinstance(idx, int):
+            raise ValueError(f"Invalid value of idx <{idx}> in a serialized source.")
+
+        ret = Source._source_idx_to_source.get(idx)
+
+        if ret is None:
+            raise ValueError(
+                f"Source with idx {idx} not found in registry. Did you forget to load sources?"
+            )
 
-        return t.cast(SourceType, Source._source_idx_to_source[Source._sources[obj]])
+        return ret
 
     @staticmethod
     def load_serialized_sources(sources: list[dict[str, t.Any]]) -> None:
         """Load serialized sources.
 
         Args:
             data: The list of dictionaries containing the serialized sources.
@@ -146,16 +149,16 @@
     def clear_registry(cls) -> None:
         cls._sources = {}
         cls._source_idx_to_source = {}
 
     @classmethod
     def list_registered_sources(cls, exclude_no_source: bool = False) -> list[Source]:
         ret = list(cls._sources.keys())
-        if exclude_no_source and NoSource() in ret:
-            ret.remove(NoSource())
+        if not exclude_no_source:
+            ret.append(NO_SOURCE)
         return ret
 
     def __str__(self) -> str:
         return f"{self.source_type}@{self.source_uri}"
 
     @property
     def fqn(self) -> str:
@@ -176,15 +179,20 @@
     def get_raw(self) -> str | None:
         return self._raw
 
 
 class Position(DataClassSerializeMixin, FQN):
     """Base class for all position types."""
 
-    pass
+    @classmethod
+    def _deserialize(cls, value: dict[str, t.Any]) -> Position:
+        if value == {}:
+            return NO_POSITION
+
+        return super()._deserialize(value)
 
 
 @dataclass(frozen=True)
 class Origin(DataClassSerializeMixin, FQN):
     """Base class for all origin types."""
 
     source: Source
@@ -193,14 +201,21 @@
     def __post_init__(self) -> None:
         if not isinstance(self.source, Source):
             raise TypeError(f"Expected Source, got {type(self.source)}")
 
         if not isinstance(self.position, Position):
             raise TypeError(f"Expected Position, got {type(self.position)}")
 
+    @classmethod
+    def _deserialize(cls, value: dict[str, t.Any]) -> Origin:
+        if value == {}:
+            return NO_ORIGIN
+
+        return super()._deserialize(value)
+
     def __str__(self) -> str:
         return f"{self.source.source_type}@{self.fqn}"
 
     @property
     def fqn(self) -> str:
         return f"{self.source.fqn}{URI_DELIM}{self.position.fqn}"
 
@@ -222,52 +237,78 @@
     _instance: t.ClassVar[NoSource | None] = None
 
     def __new__(cls, *args: t.Any, **kwargs: t.Any) -> NoSource:
         if cls._instance is None:
             cls._instance = object.__new__(cls, *args, **kwargs)
         return cls._instance
 
+    def __post_init__(self) -> None:
+        # Prevents NoSource from being added to the registry
+        pass
+
+    def _serialize(self) -> dict[str, t.Any]:
+        return {}
+
     def get_raw(self) -> None:
         return None
 
+    @property
+    def source_registry_id(self) -> int:
+        # No Source does not have a "real" registry id
+        return -1
+
+
+NO_SOURCE = NoSource()
+
 
 @dataclass(frozen=True)
 class NoPosition(Position):
     _instance: t.ClassVar[NoPosition | None] = None
 
     def __new__(cls, *args: t.Any, **kwargs: t.Any) -> NoPosition:
         if cls._instance is None:
             cls._instance = object.__new__(cls, *args, **kwargs)
         return cls._instance
 
+    def _serialize(self) -> dict[str, t.Any]:
+        return {}
+
     @property
     def fqn(self) -> str:
         return "NoPosition"
 
 
+NO_POSITION = NoPosition()
+
+
 @dataclass(frozen=True)
 class NoOrigin(Origin):
     source: NoSource = field(default_factory=NoSource, init=False)
     position: NoPosition = field(default_factory=NoPosition, init=False)
 
     _instance: t.ClassVar[NoOrigin | None] = None
 
     def __new__(cls, *args: t.Any, **kwargs: t.Any) -> NoOrigin:
         if cls._instance is None:
             cls._instance = object.__new__(cls, *args, **kwargs)
         return cls._instance
 
+    def _serialize(self) -> dict[str, t.Any]:
+        return {}
+
     @property
     def fqn(self) -> str:
         return "NoOrigin"
 
     def get_raw(self) -> None:
         return None
 
 
+NO_ORIGIN = NoOrigin()
+
 # -----------------------------------------------------------------------------
 # ----------------------------- Source Classess ---------------------------------
 
 
 @dataclass(frozen=True)
 class SourceSet(Source):
     sources: tuple[Source, ...]
```

### Comparing `pyoak-1.0.0/src/pyoak/serialize.py` & `pyoak-1.1.0/src/pyoak/serialize.py`

 * *Files identical despite different names*

