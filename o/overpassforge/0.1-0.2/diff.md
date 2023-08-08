# Comparing `tmp/overpassforge-0.1.tar.gz` & `tmp/overpassforge-0.2.tar.gz`

## Comparing `overpassforge-0.1.tar` & `overpassforge-0.2.tar`

### file list

```diff
@@ -1,24 +1,31 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 overpassforge-0.1/requirements.txt
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 overpassforge-0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 overpassforge-0.1/overpassforge/__init__.py
--rw-r--r--   0        0        0    11637 2020-02-02 00:00:00.000000 overpassforge-0.1/overpassforge/base.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 overpassforge-0.1/overpassforge/builder.py
--rw-r--r--   0        0        0    10622 2020-02-02 00:00:00.000000 overpassforge-0.1/overpassforge/filters.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 overpassforge-0.1/overpassforge/statements.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 overpassforge-0.1/overpassforge/utils.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 overpassforge-0.1/overpassforge/variables.py
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 overpassforge-0.1/overpassforge/visitors.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 overpassforge-0.1/tests/conftest.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 overpassforge-0.1/tests/test_around_filter.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 overpassforge-0.1/tests/test_basic_filters.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 overpassforge-0.1/tests/test_build_query.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 overpassforge-0.1/tests/test_id_filter.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 overpassforge-0.1/tests/test_intersect_filter.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 overpassforge-0.1/tests/test_statements.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 overpassforge-0.1/tests/test_tag_filter.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 overpassforge-0.1/tests/test_visitors.py
--rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 overpassforge-0.1/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 overpassforge-0.1/LICENSE
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 overpassforge-0.1/README.md
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 overpassforge-0.1/pyproject.toml
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 overpassforge-0.1/PKG-INFO
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 overpassforge-0.2/requirements.txt
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 overpassforge-0.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 overpassforge-0.2/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 overpassforge-0.2/docs/make.bat
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 overpassforge-0.2/docs/source/api.rst
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 overpassforge-0.2/docs/source/conf.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 overpassforge-0.2/docs/source/index.rst
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 overpassforge-0.2/docs/source/introduction.rst
+-rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 overpassforge-0.2/docs/source/usage.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 overpassforge-0.2/overpassforge/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 overpassforge-0.2/overpassforge/_utils.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 overpassforge-0.2/overpassforge/_variables.py
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 overpassforge-0.2/overpassforge/_visitors.py
+-rw-r--r--   0        0        0    10601 2020-02-02 00:00:00.000000 overpassforge-0.2/overpassforge/base.py
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 overpassforge-0.2/overpassforge/builder.py
+-rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 overpassforge-0.2/overpassforge/filters.py
+-rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 overpassforge-0.2/overpassforge/statements.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 overpassforge-0.2/tests/conftest.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 overpassforge-0.2/tests/test_around_filter.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 overpassforge-0.2/tests/test_basic_filters.py
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 overpassforge-0.2/tests/test_build_query.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 overpassforge-0.2/tests/test_id_filter.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 overpassforge-0.2/tests/test_intersect_filter.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 overpassforge-0.2/tests/test_statements.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 overpassforge-0.2/tests/test_tag_filter.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 overpassforge-0.2/tests/test_visitors.py
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 overpassforge-0.2/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 overpassforge-0.2/LICENSE
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 overpassforge-0.2/README.md
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 overpassforge-0.2/pyproject.toml
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 overpassforge-0.2/PKG-INFO
```

### Comparing `overpassforge-0.1/.github/workflows/ci.yml` & `overpassforge-0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `overpassforge-0.1/overpassforge/base.py` & `overpassforge-0.2/overpassforge/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,61 +10,65 @@
     Changed,
     User,
     Around,
     Area,
     Pivot,
     Polygon
 )
-from .variables import VariableManager
+from ._variables import VariableManager as _VariableManager
 from datetime import datetime
 
 if TYPE_CHECKING:
-    from .visitors import Visitor
+    from ._visitors import Visitor as _Visitor
     from .statements import Difference, Union, Areas
 
 
 OUT_OPTIONS = ("ids", "skel", "body", "tags", "meta", "noids", "geom", "bb", "center", "asc", "qt", "count")
 
 DATE_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
 
 
 class Statement:
-    """
-    Represents a generic Overpass QL statement.
-    """
+    """Represents a generic Overpass QL statement."""
 
     def __init__(self, label: str | None = None) -> None:
+        """
+        Args:
+            label: A label for this statement which may be used
+                as variable name for the result of this statement at compilation.
+        """
         self.out_options: list[set[str]] = []
         self.label = label
     
-    def accept_pre(self, visitor: Visitor):
-        """
-        Calls the appropriate visitor method when this statement is visited before
+    def _accept_pre(self, visitor: _Visitor):
+        """Calls the appropriate visitor method when this statement is visited before
         visiting it's dependencies.
         """
         visitor.visit_statement_pre(self)
 
-    def accept_post(self, visitor: Visitor):
-        """
-        Calls the appropriate visitor method after having visited this statement's
+    def _accept_post(self, visitor: _Visitor):
+        """Calls the appropriate visitor method after having visited this statement's
         dependencies.
         """
         visitor.visit_statement_post(self)
 
-    def _compile(self, vars: VariableManager, out_var: str | None = None) -> str:
-        """
-        Compiles the statement into its Overpass query string, without eventual
-        outputs.
+    def _compile_core(self, vars: _VariableManager, out_var: str | None = None) -> str:
+        """Compiles the statement into its Overpass query string, without additional
+        output statements.
+
+        Args:
+            vars: The variable manager at compile time
+            out_var: The name of the output variable where to
+                store the result of this statement
         """
         raise NotImplementedError("Must be implemented in subclass.")
     
     @property
-    def dependencies(self) -> list[Statement]:
-        """
-        The list of statements on which this statement depends on.
+    def _dependencies(self) -> list[Statement]:
+        """The list of statements on which this statement depends on (readonly)
         """
         raise NotImplementedError("Must be implemented in subclass.")
     
     def __hash__(self) -> int:
         return id(self)
     
     def __sub__(self, other: Statement) -> Difference:
@@ -76,19 +80,23 @@
         return Union(self, other)
     
     def out(self, *options: str | tuple[float, float, float, float]) -> Statement:
         """
         Indicate that the result of this statement must be outputed.
 
         Args:
-            options: one or a combination of "ids", "skel", "body", "tags",
-            "meta", "noids", "geom", "bb", "center", "asc", "qt", "count" or
-            a bounding box (south,west,north,east)
+            options: None or any combination of "ids", "skel", "body", "tags",
+                "meta", "noids", "geom", "bb", "center", "asc", "qt", "count" or
+                a bounding box (south,west,north,east).
         
-        Returns: itself
+        Returns:
+            This same instance.
+        
+        Raises:
+            ValueError: Invalid output options.
         """
         extract = lambda item: item.strip().split(' ')
         valid_options: set[str] = set()
         for item in options:
             if isinstance(item, str):
                 opts = set(filter(lambda opt: len(opt) > 0, extract(item)))
                 invalid = opts - set(OUT_OPTIONS)
@@ -97,19 +105,26 @@
                 valid_options.update(opts)
             else:
                 valid_options.add(str(item))
         
         self.out_options.append(valid_options)
         return self
     
-    def compile(self, vars: VariableManager, out_var: str | None = None) -> str:
-        """
-        Compiles the statement into its Overpass query string, with its outputs.
+    def _compile(self, vars: _VariableManager, out_var: str | None = None) -> str:
+        """Compiles the statement into its Overpass query string, with its eventual outputs.
+
+        Args:
+            vars: The variable manager at compile time.
+            out_var: The name of the output variable where to store the result
+                of this statement.
+        
+        Returns:
+            The compiled statement string.
         """
-        compiled = self._compile(vars, out_var)
+        compiled = self._compile_core(vars, out_var)
         if len(self.out_options) == 0:
             return compiled
         
         outs = []
         var = vars.get(self)
         for opts in self.out_options:
             out = f".{var} out" if var is not None else "out"
@@ -119,82 +134,16 @@
         return compiled + "\n" + "\n".join(outs)
     
     def __repr__(self) -> str:
         info = self.label if self.label else id(self)
         return f"<{self.__class__.__name__} \'{info}\'>"
 
 
-class RawStatement(Statement):
-    """
-    Represents a generic Overpass QL statement.
-    """
-
-    def __init__(self, raw: str = "", label: str | None = None, **dependencies: Statement) -> None:
-        """
-        Raw Overpass query string. It can be formated to support dependency
-        from other statements (raw or not). Placholders will be replaced
-        by the names of the variables where the dependencies output their
-        results.
-
-        Args:
-            raw (str): A formatable string of the query. Named placeholders
-            (e.g. "{name}") indicating dependency on other statements. An
-            optional special {:out_var} placeholder indicates where the name of
-            the output set must be placed.
-            **dependencies (Statement): the list of named statement on which
-            this statements depends on. The names must match the placeholders
-            in the raw query.
-        
-        Example:
-            ```python
-            >>> foo = Nodes().where(name="Foo")
-            >>> bar = Statement("node.{x}[amenity=\"bar\"]->.{:out_var};", x=foo)
-            >>> baz = Nodes(input_set=bar).within((50.6,7.0,50.8,7.3))
-            >>> print(build(baz))
-                node["name"="Foo"]->.set_0;
-                node.set_0[amenity="bar"]->.set_1;
-                node.set_1(50.6,7.0,50.8,7.3);
-            ```
-        """
-
-        super().__init__()
-
-        self._raw = raw
-        self._dependencies = dependencies
-        if "{}" in raw:
-            raise ValueError("All inserted dependencies must be named.")
-    
-    def _compile(self, vars: VariableManager, out_var: str | None = None) -> str:
-        """
-        Compiles the statement into its Overpass query string, without eventual
-        outputs.
-        """
-        var_names: dict[str, str] = {}
-        for name, stmt in self._dependencies.items():
-            if not vars.is_named(stmt):
-                raise RuntimeError("All inserted sets must use variables.")
-            var_names[name] = vars[stmt]
-        compiled = self._raw
-        if "{:out_var}" in self._raw:
-            compiled = compiled.replace("{:out_var}", out_var or "_")
-        elif out_var is not None:
-            raise RuntimeError("No output variable specified.")
-        return compiled.format(**var_names)
-    
-    @property
-    def dependencies(self) -> list[Statement]:
-        """
-        The list of statements on which this statement depends on.
-        """
-        return list(self._dependencies.values())
-
-
 class QueryStatement(Statement):
-    """
-    Represents a query statement, e.g. node, rel, way... Query statements always
+    """Represents a query statement, e.g. node, rel, way... Query statements always
     return a set that can be used as input to other statements/filters.
     """
 
     _type_specifier: str = "<Unspecified>"
     
     def __init__(self,
         ids: Iterable[int] | int | None = None,
@@ -229,96 +178,117 @@
             self.filters.append(around)
         elif around is not None:
             self.filters.append(Around(around[1], around[0]))
         
         for key, value in tags.items():
             self.filters.append(K(key) == V(value))
     
-    def filter(self, *args: Filter) -> QueryStatement:
-        """
-        Adds filters to the statement/set.
+    def filter(self, *filters: Filter) -> QueryStatement:
+        """Adds filters to the statement/set.
+
+        Args:
+            filters: A list of filters.
         """
-        return self.__class__(filters=[Intersection(self), *args])
+        return self.__class__(filters=[Intersection(self), *filters])
     
     def where(self, **tags: str) -> QueryStatement:
+        """Adds filters "key"="value".
+
+        Args:
+            tags: List of key="value".
         """
-        Adds filters "key"="value" on tags.
-        """
+
         filters: list[Filter] = [Intersection(self)]
         for key, value in tags.items():
             filters.append(K(key) == V(value))
         return self.__class__(filters=filters)
     
-    def within(self, area: tuple[float,float,float,float] | BoundingBox | Polygon | Area | 'Areas') -> QueryStatement:
-        """
-        Filters the elements that are in the specified area.
+    def within(self, area: tuple[float,float,float,float] | BoundingBox | Polygon | Area | Areas) -> QueryStatement:
+        """Filters the elements that are in the specified area.
+
+        Args:
+            area: A bounding box (filter object or as a tuple), polygon filter,
+                area filter or set of areas.
         """
         if isinstance(area, Filter):
             return self.__class__(filters=[Intersection(self), area])
         elif isinstance(area, tuple):
             return self.__class__(filters=[Intersection(self), BoundingBox(*area)])
         else:
             return self.__class__(filters=[Intersection(self), Area(area)])
     
     def intersection(self, *others: Statement) -> QueryStatement:
-        """
-        Returns the statement computing the intersection of
-        this set with the others.
+        """Returns the statement computing the intersection of
+        this statement with the others.
+        
+        Args:
+            others: Other statements to intersect with
         """
         return self.__class__(filters=[Intersection(self, *others)])
     
     def changed_since(self, date: datetime) -> QueryStatement:
-        """
-        Filters the elements that were changed since the specified datetime.
+        """Filters the elements that were changed since the specified datetime.
+
+        Args:
+            date: The lower bound of change dates to consider
         """
         return self.__class__(filters=[Intersection(self), Newer(date)])
     
-    def changed_between(self, lower: datetime, higher: datetime) -> QueryStatement:
-        """
-        Filters the elements that were changed between the two specified dates.
+    def changed_between(self, lower: datetime, upper: datetime) -> QueryStatement:
+        """Filters the elements that were changed between the two specified dates.
+
+        Args:
+            lower (datetime): Lower bound datetime.
+            upper (datetime): Upper bound datetime.
         """
-        return self.__class__(filters=[Intersection(self), Changed(lower, higher)])
+        return self.__class__(filters=[Intersection(self), Changed(lower, upper)])
     
     def last_changed_by(self, *users: str | int) -> QueryStatement:
-        """
-        Filters the elements that last changed by any of the given users.
+        """Filters the elements that last changed by any of the given users.
 
         Args:
-            *users: the list of user names or user ids
+            users: The list of user names or user ids.
         """
         return self.__class__(filters=[Intersection(self), User(*users)])
     
     def outlines_of(self, area: 'Areas') -> QueryStatement:
-        """
-        Filters the elements that are part of the outline of the given area.
+        """Filters the elements that are part of the outline of the given area.
+
+        Args:
+            area: The area to consider to outline of.
         """
         return self.__class__(filters=[Intersection(self), Pivot(area)])
     
     def around(self,
         radius: float,
-        other: Statement | None,
+        other: Statement | None = None,
         lats: Iterable[float] | None = None, 
         lons: Iterable[float] | None = None
     ):
-        """
-        Filters elements that are within a given radius of the elements of another set
+        """Filters elements that are within a given radius of the elements of another set
         or a list of given coordinates (cannot specify both).
+
+        Args:
+            radius: The radius to consider around each element (in meters).
+            other: Another statement.
+            lats: List of latitude of points.
+            lons: List of longitudes of points.
         """
         around = Around(radius, other, lats, lons)
         return self.__class__(filters=[Intersection(self), around])
 
     @property
-    def dependencies(self) -> list[Statement]:
+    def _dependencies(self) -> list[Statement]:
         deps: list[Statement] = []
         for filt in self.filters:
-            deps.extend(filt.dependencies)
+            deps.extend(filt._dependencies)
         return deps
     
-    def _compile(self, vars: VariableManager, out_var: str | None = None) -> str:
-        comp_filter = lambda f: f.compile(vars)
+    def _compile_core(self, vars: _VariableManager, out_var: str | None = None) -> str:
+        comp_filter = lambda f: f._compile(vars)
         res = self._type_specifier + "".join(map(comp_filter, self.filters))
         if out_var is not None:
             return res + f"->.{out_var};"
         return res + ";"
 
 
 class BlockStatement(Statement):
```

### Comparing `overpassforge-0.1/overpassforge/filters.py` & `overpassforge-0.2/overpassforge/filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,98 +1,108 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterable
 from datetime import datetime
-from .variables import VariableManager
-from .utils import partition
+from ._variables import VariableManager as _VariableManager
+from ._utils import partition
 
 if TYPE_CHECKING:
     from .base import Statement
-    from .variables import VariableManager
     from .statements import Areas
 
 
 class Filter:
     """
-    Represents a filter that can be applied on a query statement.
+    Represents a generic filter that can be applied on a query statement.
     """
     def __init__(self, raw: str | None = None) -> None:
         self._raw = raw or ""
 
-    def compile(self, vars: VariableManager) -> str:
+    def _compile(self, vars: _VariableManager) -> str:
         """
         Builds the Overpass string of this filter.
         """
         return self._raw
     
     @property
-    def dependencies(self) -> list[Statement]:
+    def _dependencies(self) -> list[Statement]:
         return []
     
     def __repr__(self) -> str:
         return f"<Filter \"{self._raw}\">"
 
 
 
 class Tag(Filter):
     """
     Represents a tag (key-value pair) filter.
     """
     def __init__(self, comparison: str, case_sensitive=True):
         """
         Args:
-            comparison (str): the comparison expression of the tag filter
-            (e.g. "name"="Foo", !"tourism")
-            case_sensitive (bool): ignore case (if comparison is "name"="Foo"
-            then a tag "name"="fOO" is also valid)
+            comparison: the comparison expression of the tag filter
+                (e.g. "name"="Foo", !"tourism")
+            case_sensitive: ignore case (e.g. if comparison is "name"="Foo"
+                then a tag "name"="fOO" is also valid)
         """
         self.comparison = comparison
         self.case_sensitive = case_sensitive
     
-    def compile(self, vars: VariableManager) -> str:
+    def _compile(self, vars: _VariableManager) -> str:
         ending = "]" if self.case_sensitive else ",i]"
         return f"[{self.comparison}{ending}"
     
     @staticmethod
     def has(key: str):
+        """Returns the filter "has key", i.e. ["key"]"""
         return Tag(f"\"{key}\"")
     
     @staticmethod
     def hasnot(key: str):
+        """Returns the filter "has not key", i.e. [!"key"]"""
         return Tag(f"!\"{key}\"")
+    
+    def __repr__(self) -> str:
+        return f"<Tag {self.comparison}, case_sensitive={self.case_sensitive}>"
 
 class V:
     """
     Represents the value of a tag.
     """
     def __init__(self, expr: str, regex=False):
         """
         Args:
-            expr: the key string
+            expr: the value string
             regex: wether the string is a regex
         """
         self.expr = expr
         self.regex = regex
     
     def __str__(self) -> str:
         if self.regex:
             return f"~\"{self.expr}\""
         return f"=\"{self.expr}\""
 
 class K:
     """
     Represents the key of a tag. Used to build a tag filter expression.
 
-    Exemples:
-    ```python
-        K("amenity") == V("cinema"), K("amenity") == "cinema" -> ["amenity"="restaurant"]
-        K("amenity") != V("bar"), K("amenity") != "bar" -> ["amenity"!="restaurant"]
-        K("name") == V("^Foo$", regex=True) -> ["name"~"^Foo$"]
-        K("name") == V("^Baz$", regex=True) -> ["name"!~"^Baz$"]
-        K("^addr:.*$", regex=True) == V("^Foo$", regex=True) -> [~"^addr:.*$"~"^Foo$"]
-    ```
+    Examples:
+
+    >>> K("amenity") == V("cinema")
+    <Tag "amenity"="cinema", case_sensitive=True>
+    >>> K("amenity") == "cinema"
+    <Tag "amenity"="cinema", case_sensitive=True>
+    >>> K("amenity") != V("bar")
+    <Tag "amenity"!="bar", case_sensitive=True>
+    >>> K("amenity") != "bar"
+    <Tag "amenity"!="bar", case_sensitive=True>
+    >>> K("name") == V("^Foo$", regex=True)
+    <Tag "name"~"^Foo$", case_sensitive=True>
+    >>> K("^addr:.*$", regex=True) == V("^Foo$", regex=True)
+    <Tag ~"^addr:.*$"~"^Foo$", case_sensitive=True>
     """
     def __init__(self, expr: str, regex=False):
         """
         Args:
             expr: the key string
             regex: wether the string is a regex
         """
@@ -119,204 +129,223 @@
     """
     Bounding box filter on a query statement.
     """
 
     def __init__(self, south: float, west: float, north: float, east: float) -> None:
         """
         Args:
-            south, west, north, east (float): bounding box latitudes and longitudes
+            south: Minimum latitude.
+            west: Minimum longitude.
+            north: Maximum latitude.
+            east: Maximum longitude.
         """
         super().__init__()
 
         self.south = south
         self.west = west
         self.north = north
         self.east = east
     
-    def compile(self, vars: VariableManager) -> str:
+    def _compile(self, vars: _VariableManager) -> str:
         return f"({self.south},{self.west},{self.north},{self.east})"
     
     def __repr__(self) -> str:
         return f"<BoundingBox ({self.south},{self.west},{self.north},{self.east})>"
 
 
 class Ids(Filter):
-    """
-    Represents an id filter.
-    """
+    """Represents an id filter."""
 
     def __init__(self, *ids: int) -> None:
         """
         Args:
-            ids (int): the list of OSM ids to filter
+            ids: The list of OSM ids to select.
         """
         super().__init__()
         
         self.ids = ids
     
-    def compile(self, vars: VariableManager) -> str:
+    def _compile(self, vars: _VariableManager) -> str:
         match len(self.ids):
             case 0:
                 return ""
             case 1:
                 return f"({self.ids[0]})"
             case _:
                 return f"(id:{','.join(map(str, self.ids))})"
     
     def __repr__(self) -> str:
         return f"<Ids ({self.ids})>"
 
 
 class Intersection(Filter):
-    """
-    Intersection with other sets.
-    """
-    def __init__(self, *elements: Statement) -> None:
+    """Intersection with other statement results."""
+
+    def __init__(self, *statements: Statement) -> None:
+        """
+        Args:
+            statements: The other statement whose results intersect with.
+        """
+
         super().__init__()
-        self.statements = list(elements)
+        self.statements = list(statements)
     
     @property
-    def dependencies(self) -> list[Statement]:
+    def _dependencies(self) -> list[Statement]:
         return [*self.statements]
     
-    def compile(self, vars: VariableManager) -> str:
+    def _compile(self, vars: _VariableManager) -> str:
         if len(self.statements) == 0:
-            raise RuntimeError("Empty intersection.")
+            raise AttributeError("Empty intersection.")
         names: list[str] = []
         for stmt in self.statements:
             names.append(vars[stmt])
         return "." + ".".join(names)
     
     def __repr__(self) -> str:
         return f"<IntersectsWith {', '.join(map(str, self.statements))}>"
 
 
 class Newer(Filter):
-    """
-    Filter by newer change dates.
-    """
+    """Filter by newer change dates."""
+
     def __init__(self, date: datetime):
+        """
+        Args:
+            date: The oldest when the element has been modified.
+        """
         self.date = date
     
-    def compile(self, vars: VariableManager) -> str:
+    def _compile(self, vars: _VariableManager) -> str:
         from .base import DATE_FORMAT
         return f"(newer:\"{self.date.strftime(DATE_FORMAT)}\")"
     
     def __repr__(self) -> str:
         return f"<Newer {self.date}>"
 
 class Changed(Filter):
-    """
-    Filter that selects elements that have been changed between two given
+    """Filter that selects elements that have been changed between two given
     dates. If only the lower date is given, the second is assumed to be the
     front date of the database.
     """
-    def __init__(self, lower: datetime, higher: datetime | None = None):
+
+    def __init__(self, lower: datetime, upper: datetime | None = None):
+        """
+        Args:
+            lower: Dates' range lower bound.
+            upper: Dates' range upper bound. If not given, it is assumed to be the
+                front date of the database.
+        """
         self.lower = lower
-        self.higher = higher
+        self.upper = upper
     
-    def compile(self, vars: VariableManager) -> str:
+    def _compile(self, vars: _VariableManager) -> str:
         from .base import DATE_FORMAT
-        if self.higher is None:
+        if self.upper is None:
             return f"(changed:\"{self.lower.strftime(DATE_FORMAT)}\")"
-        return f"(changed:\"{self.lower.strftime(DATE_FORMAT)}\",\"{self.higher.strftime(DATE_FORMAT)}\")"
+        return f"(changed:\"{self.lower.strftime(DATE_FORMAT)}\",\"{self.upper.strftime(DATE_FORMAT)}\")"
     
     def __repr__(self) -> str:
-        return f"<Changed {self.lower} - {self.higher}>"
+        return f"<Changed {self.lower} - {self.upper}>"
 
 class User(Filter):
-    """
-    Filter the elements last edited by the specified users.
-    """
+    """Filter the elements last edited by the specified users."""
+
     def __init__(self, *users: int | str) -> None:
         """
         Args:
-            *users: a list of user names or user ids.
+            users: A list of user names or user ids.
+        
+        Raises:
+            ValueError: No used specified.
         """
         if len(users) == 0:
             raise ValueError("Must list at least one user.")
         self.users = users
 
-    def compile(self, vars: VariableManager) -> str:
+    def _compile(self, vars: _VariableManager) -> str:
         ids, names = partition(lambda x: isinstance(x, int), self.users)
         ids = list(map(str, ids))
         names = list(map(lambda x: f"\"{x}\"", names))
         
         compiled = ""
         if len(ids) > 0:
             compiled += f"(uid:{','.join(ids)})"
         if len(names) > 0:
             compiled += f"(user:{','.join(names)})"
         return compiled
 
 
 class Area(Filter):
-    """
-    Filters the elements which are within the given area.
-    """
+    """Filters the elements which are within the given area."""
+
     def __init__(self, input_area: 'Areas') -> None:
+        """
+        Args:
+            input_area: The areas in which the elements must lay in.
+        """
         self.input_area = input_area
     
     @property
-    def dependencies(self) -> list[Statement]:
+    def _dependencies(self) -> list[Statement]:
         return [self.input_area]
     
-    def compile(self, vars: VariableManager) -> str:
+    def _compile(self, vars: _VariableManager) -> str:
         return f"(area.{vars[self.input_area]})"
 
 class Pivot(Filter):
-    """
-    Filters the elements which are part of the outline of the given
-    area.
-    """
+    """Filters the elements which are part of the outline of the given area."""
+
     def __init__(self, input_area: 'Areas') -> None:
+        """
+        Args:
+            input_area: The areas to consider the outlines of.
+        """
         self.input_area = input_area
     
     @property
-    def dependencies(self) -> list[Statement]:
+    def _dependencies(self) -> list[Statement]:
         return [self.input_area]
     
-    def compile(self, vars: VariableManager) -> str:
+    def _compile(self, vars: _VariableManager) -> str:
         return f"(pivot.{vars[self.input_area]})"
 
 
 class Around(Filter):
-    """
-    Filters elements within a certain radius around elements in the
+    """Filters elements within a certain radius around elements in the
     input set.
     """
+
     def __init__(
         self,
         radius: float,
         input_set: Statement | None = None,
         lats: Iterable[float] | None = None,
         lons: Iterable[float] | None = None,
     ):
         """
-        Creates an around filter.
-
         Args:
-            radius (float): the radius in meters around each elements
-            input_set (Statement): the input set of elements around which to filter
-            (cannot be used in combination with lats, lons)
-            lats, lons: latitude and longitudes of points around which to filter
-            (cannot be used in combination with input_set)
+            radius: The radius in meters around each elements.
+            input_set: The input set of elements around which to filter
+                (cannot be used in combination with lats, lons).
+            lats, lons: Latitude and longitudes of points around which to filter
+                (cannot be used in combination with input_set).
         """
         self.radius = radius
         self.input_set = input_set
         self.lats = lats
         self.lons = lons
     
     @property
-    def dependencies(self) -> list[Statement]:
+    def _dependencies(self) -> list[Statement]:
         if self.input_set is None:
             return []
         return [self.input_set]
     
-    def compile(self, vars: VariableManager) -> str:
+    def _compile(self, vars: _VariableManager) -> str:
         if self.input_set is not None and (self.lats is not None or self.lons is not None):
             raise AttributeError("Cannot use both coordinates and input set.")
         
         if self.input_set is not None:
             return f"(around.{vars[self.input_set]}:{self.radius})"
         if self.lats is not None and self.lons is not None:
             latlons = []
@@ -324,25 +353,25 @@
                 latlons.append(str(lat))
                 latlons.append(str(lon))
             return f"(around:{self.radius},{','.join(latlons)})"
         
         raise AttributeError("Input set or coordinates not defined.")
 
 class Polygon(Filter):
-    """
-    Filters all elements that are inside the defined polygon.
-    """
+    """Filters all elements that are inside the defined polygon."""
+
     def __init__(self, lats: Iterable[float], lons: Iterable[float]) -> None:
         """
         Args:
-            lats, lons: the latitudes and longitudes of the points describing the polygon.
+            lats: Latitudes of the points describing the polygon.
+            lons: Longitudes of the points describing the polygon.
         """
         super().__init__()
         self.lats = lats
         self.lons = lons
     
-    def compile(self, vars: VariableManager) -> str:
+    def _compile(self, vars: _VariableManager) -> str:
         latlons = []
         for lat, lon in zip(self.lats, self.lons):
             latlons.append(str(lat))
             latlons.append(str(lon))
         return f"(poly:\"{' '.join(latlons)}\")"
```

### Comparing `overpassforge-0.1/overpassforge/variables.py` & `overpassforge-0.2/overpassforge/_variables.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         self._var_names: dict['Statement', str] = {}
         self._next_id = 0
 
     def get_or_compile(self, stmt: 'Statement', name_format: str = "{}") -> str:
         if stmt in self._var_names:
             return name_format.format(self._var_names[stmt])
         else:
-            return stmt.compile(self)
+            return stmt._compile(self)
 
     def add_statement(self, stmt: 'Statement') -> str:
         if stmt in self._var_names:
             raise RuntimeError(f"Trying to name an already named statement: {stmt}.")
         
         name = f"set_{self._next_id}"
         if stmt.label is not None and stmt.label not in self._var_names.values():
```

### Comparing `overpassforge-0.1/overpassforge/visitors.py` & `overpassforge-0.2/overpassforge/_visitors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
-from .base import Statement, RawStatement
-from .variables import VariableManager
+from .base import Statement
+from .statements import RawStatement
+from ._variables import VariableManager
 from .base import QueryStatement
-from .utils import partition
+from ._utils import partition
 from .filters import Filter, Intersection
 from dataclasses import dataclass
 
 
 class Visitor:
     """
     Base visitor class.
@@ -67,22 +68,22 @@
             self.deps[statement] = Dependency(statement)
         else:
             self.deps[statement].ref_count += 1
 
         # If we are compiling raw statement, all of its
         # dependencies must be stored in variables
         if statement.__class__ is RawStatement:
-            for stmt in statement.dependencies:
+            for stmt in statement._dependencies:
                 if stmt not in self.deps:
                     self.deps[stmt] = Dependency(stmt, 0, True)
             return
         # Dependencies used by filters must always from variables
         if isinstance(statement, QueryStatement):
             for f in statement.filters:
-                for stmt in f.dependencies:
+                for stmt in f._dependencies:
                     if stmt not in self.deps:
                         self.deps[stmt] = Dependency(stmt, 0, True)
 
 
 class DependencySimplifier(Visitor):
     """
     Simplifies chained filter dependencies. For example:
@@ -138,31 +139,31 @@
         self.sequence: list[str] = []
     
     def visit_statement_post(self, statement: Statement):
         # Other statement that can be inlined are automatically
         # handled in each statement's compilation
 
         if statement == self.root:
-            self.sequence.append(statement.compile(self.variables))
+            self.sequence.append(statement._compile(self.variables))
         elif not self.deps[statement].can_inline:
             name_to = self.variables.add_statement(statement)
-            compiled = statement.compile(self.variables, name_to)
+            compiled = statement._compile(self.variables, name_to)
             self.sequence.append(compiled)
 
 
 def traverse_statement(statement: Statement, visitor: Visitor, visited: set[Statement] | None = None):
     """
     Applies on a visitor on the statement's dependency graph in a
     Depth-First Search manner. The graph must not contain cycles.
     If a substatement is referenced more that once it will be pre-visited
     multiple times but post-visited only once.
     """
     if visited is None:
         visited = set()
     
-    statement.accept_pre(visitor)
+    statement._accept_pre(visitor)
     if statement in visited:
         return
     visited.add(statement)
-    for child in statement.dependencies:
+    for child in statement._dependencies:
         traverse_statement(child, visitor, visited)
-    statement.accept_post(visitor)
+    statement._accept_post(visitor)
```

### Comparing `overpassforge-0.1/tests/test_around_filter.py` & `overpassforge-0.2/tests/test_around_filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import pytest
 from overpassforge.filters import Around
 from overpassforge.base import Statement
-from overpassforge.variables import VariableManager
+from overpassforge._variables import VariableManager
 
 def test_too_many_attributes():
     a = Statement()
     vars = VariableManager()
     with pytest.raises(AttributeError):
-        Around(100.0, a, [10.0], [10.0]).compile(vars)
+        Around(100.0, a, [10.0], [10.0])._compile(vars)
 
 def test_no_attributes():
     with pytest.raises(AttributeError):
-        Around(100.0).compile(VariableManager())
+        Around(100.0)._compile(VariableManager())
 
 def test_around_set():
     a = Statement()
     vars = VariableManager()
     name = vars.add_statement(a)
-    assert Around(10.0, a).compile(vars) == f"(around.{name}:10.0)"
+    assert Around(10.0, a)._compile(vars) == f"(around.{name}:10.0)"
 
 def test_around_one_point():
     around = Around(10.0, lats=[42.0], lons=[43.0])
-    assert around.compile(VariableManager()) == f"(around:10.0,42.0,43.0)"
+    assert around._compile(VariableManager()) == f"(around:10.0,42.0,43.0)"
 
 def test_around_many_points():
     around = Around(10.0, lats=[42.0, -21.0], lons=[43.0, 17.5, 31.0])
-    assert around.compile(VariableManager()) == f"(around:10.0,42.0,43.0,-21.0,17.5)"
+    assert around._compile(VariableManager()) == f"(around:10.0,42.0,43.0,-21.0,17.5)"
```

### Comparing `overpassforge-0.1/tests/test_basic_filters.py` & `overpassforge-0.2/tests/test_basic_filters.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from overpassforge.filters import BoundingBox, Newer, Changed, User, Area, Pivot, Polygon
 from overpassforge.statements import Areas
-from overpassforge.variables import VariableManager
+from overpassforge._variables import VariableManager
 from datetime import datetime
 
 def test_bounding_box(no_vars):
-    assert BoundingBox(50.6,7.0,50.8,7.3).compile(no_vars) == "(50.6,7.0,50.8,7.3)"
+    assert BoundingBox(50.6,7.0,50.8,7.3)._compile(no_vars) == "(50.6,7.0,50.8,7.3)"
 
 def test_newer(no_vars):
-    assert Newer(datetime(2012, 9, 14, 7)).compile(no_vars) == "(newer:\"2012-09-14T07:00:00Z\")"
+    assert Newer(datetime(2012, 9, 14, 7))._compile(no_vars) == "(newer:\"2012-09-14T07:00:00Z\")"
 
 def test_changed_one(no_vars):
-    assert Changed(datetime(2012, 9, 14, 7)).compile(no_vars) == "(changed:\"2012-09-14T07:00:00Z\")"
+    assert Changed(datetime(2012, 9, 14, 7))._compile(no_vars) == "(changed:\"2012-09-14T07:00:00Z\")"
 
 def test_changed_two(no_vars):
     c = Changed(datetime(2012, 9, 14, 7), datetime(2012, 9, 14, 7, 1))
-    assert c.compile(no_vars) == "(changed:\"2012-09-14T07:00:00Z\",\"2012-09-14T07:01:00Z\")"
+    assert c._compile(no_vars) == "(changed:\"2012-09-14T07:00:00Z\",\"2012-09-14T07:01:00Z\")"
 
 def test_user_name(no_vars):
-    assert User("Steve").compile(no_vars) == "(user:\"Steve\")"
+    assert User("Steve")._compile(no_vars) == "(user:\"Steve\")"
 
 def test_user_id(no_vars):
-    assert User(1).compile(no_vars) == "(uid:1)"
+    assert User(1)._compile(no_vars) == "(uid:1)"
 
 def test_user_ids_names(no_vars):
-    assert User("Steve",1,2,"Paul",3).compile(no_vars) == "(uid:1,2,3)(user:\"Steve\",\"Paul\")"
+    assert User("Steve",1,2,"Paul",3)._compile(no_vars) == "(uid:1,2,3)(user:\"Steve\",\"Paul\")"
 
 def test_area_filter():
     a = Areas()
     vars = VariableManager()
     name = vars.add_statement(a)
-    assert Area(a).compile(vars) == f"(area.{name})"
+    assert Area(a)._compile(vars) == f"(area.{name})"
 
 def test_pivot_filter():
     a = Areas()
     vars = VariableManager()
     name = vars.add_statement(a)
-    assert Pivot(a).compile(vars) == f"(pivot.{name})"
+    assert Pivot(a)._compile(vars) == f"(pivot.{name})"
 
 def test_polygon_filter(no_vars):
     p = Polygon([50.7,50.7,50.75], [7.1,7.2,7.15])
-    assert p.compile(no_vars) == "(poly:\"50.7 7.1 50.7 7.2 50.75 7.15\")"
+    assert p._compile(no_vars) == "(poly:\"50.7 7.1 50.7 7.2 50.75 7.15\")"
```

### Comparing `overpassforge-0.1/tests/test_build_query.py` & `overpassforge-0.2/tests/test_build_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from overpassforge.builder import build
-from overpassforge.statements import Nodes, Difference, Union, Areas, Ways
-from overpassforge.base import RawStatement
+from overpassforge.statements import RawStatement, Nodes, Difference, Union, Areas, Ways
 
 def test_no_dependencies_1():
     assert build(Nodes().where(amenity="restaurant")) == \
         """node["amenity"="restaurant"];"""
 
 def test_no_dependencies_2():
     a = Nodes(ids=128)
```

### Comparing `overpassforge-0.1/tests/test_intersect_filter.py` & `overpassforge-0.2/tests/test_intersect_filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from overpassforge.filters import Intersection
 from overpassforge.statements import Statement
-from overpassforge.variables import VariableManager
+from overpassforge._variables import VariableManager
 import pytest
 
 def test_one_intersections():
     a = Statement()
     vars = VariableManager()
     name_a = vars.add_statement(a)
-    assert Intersection(a).compile(vars) == f".{name_a}"
+    assert Intersection(a)._compile(vars) == f".{name_a}"
 
 def test_two_intersections():
     a = Statement()
     b = Statement()
     vars = VariableManager()
     name_a = vars.add_statement(a)
     name_b = vars.add_statement(b)
-    assert Intersection(a, b).compile(vars) == f".{name_a}.{name_b}"
+    assert Intersection(a, b)._compile(vars) == f".{name_a}.{name_b}"
 
 def test_requires_variable():
     a = Statement()
     b = Statement()
     vars = VariableManager()
     vars.add_statement(a)
 
     with pytest.raises(KeyError):
-        Intersection(a, b).compile(vars)
+        Intersection(a, b)._compile(vars)
```

### Comparing `overpassforge-0.1/tests/test_statements.py` & `overpassforge-0.2/tests/test_statements.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from overpassforge.statements import Nodes, Ways, Relations, Areas, Difference, Union
-from overpassforge.variables import VariableManager
+from overpassforge._variables import VariableManager
 import pytest
 
 @pytest.fixture
 def no_sets():
     return VariableManager()
 
 def test_node_statement(no_sets):
-    assert Nodes().compile(no_sets) == "node;"
-    assert Nodes(ids=(42,43), bounding_box=(50.6,7.0,50.8,7.3)).compile(no_sets) == \
+    assert Nodes()._compile(no_sets) == "node;"
+    assert Nodes(ids=(42,43), bounding_box=(50.6,7.0,50.8,7.3))._compile(no_sets) == \
         "node(id:42,43)(50.6,7.0,50.8,7.3);"
 
 def test_way_statement(no_sets):
-    assert Ways().compile(no_sets) == "way;"
-    assert Ways(ids=(42,43), bounding_box=(50.6,7.0,50.8,7.3)).compile(no_sets) == \
+    assert Ways()._compile(no_sets) == "way;"
+    assert Ways(ids=(42,43), bounding_box=(50.6,7.0,50.8,7.3))._compile(no_sets) == \
         "way(id:42,43)(50.6,7.0,50.8,7.3);"
 
 def test_relation_statement(no_sets):
-    assert Relations().compile(no_sets) == "rel;"
-    assert Relations(ids=(42,43), bounding_box=(50.6,7.0,50.8,7.3)).compile(no_sets) == \
+    assert Relations()._compile(no_sets) == "rel;"
+    assert Relations(ids=(42,43), bounding_box=(50.6,7.0,50.8,7.3))._compile(no_sets) == \
         "rel(id:42,43)(50.6,7.0,50.8,7.3);"
 
 def test_area_statement(no_sets):
-    assert Areas().compile(no_sets) == "area;"
-    assert Areas(ids=(42,43), bounding_box=(50.6,7.0,50.8,7.3)).compile(no_sets) == \
+    assert Areas()._compile(no_sets) == "area;"
+    assert Areas(ids=(42,43), bounding_box=(50.6,7.0,50.8,7.3))._compile(no_sets) == \
         "area(id:42,43)(50.6,7.0,50.8,7.3);"
 
 def test_difference_statement(no_sets):
-    assert Difference(Nodes(ids=(42,43)), Nodes(ids=43)).compile(no_sets) == \
+    assert Difference(Nodes(ids=(42,43)), Nodes(ids=43))._compile(no_sets) == \
         "(node(id:42,43); - node(43););"
 
 def test_union_statement(no_sets):
-    assert Union(Nodes(ids=(42,43)), Nodes(ids=44)).compile(no_sets) == \
+    assert Union(Nodes(ids=(42,43)), Nodes(ids=44))._compile(no_sets) == \
         "(node(id:42,43); node(44););"
```

### Comparing `overpassforge-0.1/tests/test_tag_filter.py` & `overpassforge-0.2/tests/test_tag_filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from overpassforge.filters import Tag, K, V
 
 def test_equal(no_vars):
-    assert (K("amenity") == V("cinema")).compile(no_vars) == """["amenity"="cinema"]"""
-    assert (K("tourism") == "yes").compile(no_vars) == """["tourism"="yes"]"""
+    assert (K("amenity") == V("cinema"))._compile(no_vars) == """["amenity"="cinema"]"""
+    assert (K("tourism") == "yes")._compile(no_vars) == """["tourism"="yes"]"""
 
 def test_not_equal(no_vars):
-    assert (K("amenity") != V("cinema")).compile(no_vars) == """["amenity"!="cinema"]"""
-    assert (K("tourism") != "yes").compile(no_vars) == """["tourism"!="yes"]"""
+    assert (K("amenity") != V("cinema"))._compile(no_vars) == """["amenity"!="cinema"]"""
+    assert (K("tourism") != "yes")._compile(no_vars) == """["tourism"!="yes"]"""
 
 def test_has_key(no_vars):
-    assert Tag.has("opening_hours").compile(no_vars) == """["opening_hours"]"""
+    assert Tag.has("opening_hours")._compile(no_vars) == """["opening_hours"]"""
 
 def test_has_not_key(no_vars):
-    assert Tag.hasnot("opening_hours").compile(no_vars) == """[!"opening_hours"]"""
+    assert Tag.hasnot("opening_hours")._compile(no_vars) == """[!"opening_hours"]"""
 
 def test_value_matches(no_vars):
-    assert (K("name") == V("^Foo$", True)).compile(no_vars) == """["name"~"^Foo$"]"""
+    assert (K("name") == V("^Foo$", True))._compile(no_vars) == """["name"~"^Foo$"]"""
 
 def test_value_not_matches(no_vars):
-    assert (K("name") != V("^Foo$", True)).compile(no_vars) == """["name"!~"^Foo$"]"""
+    assert (K("name") != V("^Foo$", True))._compile(no_vars) == """["name"!~"^Foo$"]"""
 
 def test_key_value_match(no_vars):
-    assert (K("^addr:.*$", True) == V("^Foo$", True)).compile(no_vars) == """[~"^addr:.*$"~"^Foo$"]"""
+    assert (K("^addr:.*$", True) == V("^Foo$", True))._compile(no_vars) == """[~"^addr:.*$"~"^Foo$"]"""
 
 def test_case_insensitive(no_vars):
     tag = K("amenity") == V("cinema")
     tag.case_sensitive = False
-    assert tag.compile(no_vars) == """["amenity"="cinema",i]"""
+    assert tag._compile(no_vars) == """["amenity"="cinema",i]"""
```

### Comparing `overpassforge-0.1/tests/test_visitors.py` & `overpassforge-0.2/tests/test_visitors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from overpassforge.statements import Nodes, Union, Difference
-from overpassforge.visitors import CycleDetector, CircularDependencyError, DependencyRetriever, traverse_statement
+from overpassforge._visitors import CycleDetector, CircularDependencyError, DependencyRetriever, traverse_statement
 import pytest
 
 def test_no_cycles():
     a = Nodes()
     b = Nodes()
     c = Union(a, b)
     d = Union(a, b, c)
```

### Comparing `overpassforge-0.1/.gitignore` & `overpassforge-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `overpassforge-0.1/LICENSE` & `overpassforge-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `overpassforge-0.1/README.md` & `overpassforge-0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Overpass Forge: a query builder for the Overpass query language
 
 An object-oriented model to build Overpass queries in Python. Primarly intended
 to generate complex queries in Python.
 
-Requires **Python 3.10 or higher**.
+## Install
+
+Requires **Python 3.10 or higher**. Install with:
+
+```cmd
+pip install overpassforge
+```
 
 ## Example
 
 ```python
 from overpassforge import Areas, Nodes, Ways, build, beautify
 
 # Find both cinema nodes and ways in Bonn, which
@@ -65,15 +71,15 @@
   - [x] *newer*
   - [x] By date of change (*changed*)
   - [x] By user (*user, uid*)
   - [x] By area (*area*)
   - [x] Area pivot (*pivot*)
   - [ ] Conditional query filter (*if:*)
 
-## Contribute
+## Contributing
 
 ### Setup the development environment
 
 #### Windows
 
 ```cmd
 python -m venv .venv
@@ -85,14 +91,14 @@
 
 ```cmd
 python -m venv .venv
 source .venv/bin/activate
 python -m pip install -r requirements.txt
 ```
 
-## Unit tests
+### Unit tests
 
 Run all the tests with:
 
 ```cmd
 python -m pytest ./tests
 ```
```

### Comparing `overpassforge-0.1/pyproject.toml` & `overpassforge-0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 exclude = ["examples/"]
 
 [project]
 name = "overpassforge"
-version = "0.1"
+version = "0.2"
 authors = [
   { name="Krafpy", email="krafpy@gmail.com" },
 ]
 description = "A library for generating OpenStreetMap's Overpass QL queries from Python objects."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `overpassforge-0.1/PKG-INFO` & `overpassforge-0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overpassforge
-Version: 0.1
+Version: 0.2
 Summary: A library for generating OpenStreetMap's Overpass QL queries from Python objects.
 Project-URL: Homepage, https://github.com/Krafpy/Overpass-Forge
 Project-URL: Bug Tracker, https://github.com/Krafpy/Overpass-Forge/issues
 Author-email: Krafpy <krafpy@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,21 @@
 Description-Content-Type: text/markdown
 
 # Overpass Forge: a query builder for the Overpass query language
 
 An object-oriented model to build Overpass queries in Python. Primarly intended
 to generate complex queries in Python.
 
-Requires **Python 3.10 or higher**.
+## Install
+
+Requires **Python 3.10 or higher**. Install with:
+
+```cmd
+pip install overpassforge
+```
 
 ## Example
 
 ```python
 from overpassforge import Areas, Nodes, Ways, build, beautify
 
 # Find both cinema nodes and ways in Bonn, which
@@ -79,15 +85,15 @@
   - [x] *newer*
   - [x] By date of change (*changed*)
   - [x] By user (*user, uid*)
   - [x] By area (*area*)
   - [x] Area pivot (*pivot*)
   - [ ] Conditional query filter (*if:*)
 
-## Contribute
+## Contributing
 
 ### Setup the development environment
 
 #### Windows
 
 ```cmd
 python -m venv .venv
@@ -99,14 +105,14 @@
 
 ```cmd
 python -m venv .venv
 source .venv/bin/activate
 python -m pip install -r requirements.txt
 ```
 
-## Unit tests
+### Unit tests
 
 Run all the tests with:
 
 ```cmd
 python -m pytest ./tests
 ```
```

