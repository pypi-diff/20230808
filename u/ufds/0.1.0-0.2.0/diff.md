# Comparing `tmp/ufds-0.1.0.tar.gz` & `tmp/ufds-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufds-0.1.0.tar", last modified: Sun Aug  6 14:53:37 2023, max compression
+gzip compressed data, was "ufds-0.2.0.tar", last modified: Tue Aug  8 20:25:23 2023, max compression
```

## Comparing `ufds-0.1.0.tar` & `ufds-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:53:37.595399 ufds-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)    11372 2023-08-06 14:53:19.000000 ufds-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    15866 2023-08-06 14:53:37.595399 ufds-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1922 2023-08-06 14:53:19.000000 ufds-0.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2633 2023-08-06 14:53:19.000000 ufds-0.1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-06 14:53:19.000000 ufds-0.1.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 14:53:37.595399 ufds-0.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:53:37.593400 ufds-0.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:53:37.594400 ufds-0.1.0/src/ufds.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15866 2023-08-06 14:53:37.000000 ufds-0.1.0/src/ufds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      208 2023-08-06 14:53:37.000000 ufds-0.1.0/src/ufds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 14:53:37.000000 ufds-0.1.0/src/ufds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-08-06 14:53:37.000000 ufds-0.1.0/src/ufds.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     3712 2023-08-06 14:53:19.000000 ufds-0.1.0/src/ufds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:53:37.594400 ufds-0.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1364 2023-08-06 14:53:19.000000 ufds-0.1.0/tests/test_ufds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 20:25:23.724084 ufds-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11372 2023-08-08 20:25:08.000000 ufds-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15866 2023-08-08 20:25:23.724084 ufds-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1922 2023-08-08 20:25:08.000000 ufds-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2633 2023-08-08 20:25:08.000000 ufds-0.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 20:25:08.000000 ufds-0.2.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 20:25:23.724084 ufds-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 20:25:23.721084 ufds-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 20:25:23.723084 ufds-0.2.0/src/ufds/
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-08-08 20:25:08.000000 ufds-0.2.0/src/ufds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-08-08 20:25:08.000000 ufds-0.2.0/src/ufds/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2569 2023-08-08 20:25:08.000000 ufds-0.2.0/src/ufds/disjoint_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2023-08-08 20:25:08.000000 ufds-0.2.0/src/ufds/native_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 20:25:23.724084 ufds-0.2.0/src/ufds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15866 2023-08-08 20:25:23.000000 ufds-0.2.0/src/ufds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      287 2023-08-08 20:25:23.000000 ufds-0.2.0/src/ufds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 20:25:23.000000 ufds-0.2.0/src/ufds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-08 20:25:23.000000 ufds-0.2.0/src/ufds.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 20:25:23.724084 ufds-0.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1364 2023-08-08 20:25:08.000000 ufds-0.2.0/tests/test_ufds.py
```

### Comparing `ufds-0.1.0/LICENSE` & `ufds-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ufds-0.1.0/PKG-INFO` & `ufds-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufds
-Version: 0.1.0
+Version: 0.2.0
 Summary: Union-Find (Disjoint Set) Data Structure
 Author-email: Louis Cochen <louis.cochen@protonmail.ch>
 Maintainer-email: Louis Cochen <louis.cochen@protonmail.ch>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ufds-0.1.0/README.md` & `ufds-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ufds-0.1.0/pyproject.toml` & `ufds-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ufds-0.1.0/src/ufds.egg-info/PKG-INFO` & `ufds-0.2.0/src/ufds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufds
-Version: 0.1.0
+Version: 0.2.0
 Summary: Union-Find (Disjoint Set) Data Structure
 Author-email: Louis Cochen <louis.cochen@protonmail.ch>
 Maintainer-email: Louis Cochen <louis.cochen@protonmail.ch>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ufds-0.1.0/src/ufds.py` & `ufds-0.2.0/src/ufds/native_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,28 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""ufds.py: Union-Find Data Structure implementation."""
+"""base.py: Union-Find Data Structure base implementation."""
 
 from __future__ import annotations
 
-from collections import defaultdict
-from collections.abc import Iterable, Iterator
-from typing import Any, Generic, TypeVar
+from typing import Generic, TypeVar
 
 T = TypeVar("T")
 
 
-__version__ = "0.1.0"
-
-
 class BaseDisjointSet(Generic[T]):
     """BaseDisjointSet implementation exposes unsafe primitives."""
 
     parent: dict[T, T]
     rank: dict[T, int]
 
     def __init__(self) -> None:
@@ -66,57 +61,7 @@
         d = self.rank[x] - self.rank[y]
         if d < 0:
             self.parent[x] = y
         else:
             self.parent[y] = x
             if d == 0:
                 self.rank[x] += 1
-
-
-class DisjointSet(BaseDisjointSet[T]):
-    """Concrete DisjointSet implementation with safe methods."""
-
-    def __init__(self, seeds: Iterable[T | tuple[T, T]] = ()) -> None:
-        super().__init__()
-        for s in seeds:
-            if not isinstance(s, tuple):
-                s = s, s
-            self.union(*s)
-
-    def find(self, x: T) -> T:
-        """Find root or create tree containing x."""
-        if x not in self.parent:
-            return self._make_set(x)
-        return self._find_set(x)
-
-    def union(self, x: T, y: T) -> None:
-        """Link (optionally create) trees containing x and y."""
-        px, py = self.find(x), self.find(y)
-        if px == py:
-            return
-        self._union(px, py)
-
-    @property
-    def _branches(self) -> Iterator[tuple[T, T]]:
-        """Iterate over branches in trees."""
-        for x in self.parent.keys():
-            yield self._find_set(x), x
-
-    def __bool__(self) -> bool:  # pragma: no cover
-        """Alias to self.parent.__bool__ method."""
-        return bool(self.parent)
-
-    def __eq__(self, other: Any) -> bool:
-        """Evaluate if forests are equivalent."""
-        if not isinstance(other, type(self)):  # pragma: no cover
-            return NotImplemented
-        return sorted(tuple(self._branches)) == sorted(tuple(other._branches))
-
-    def __iter__(self) -> Iterator[set[T]]:
-        """Iterator over the trees in the forest."""
-        trees: defaultdict[T, set[T]] = defaultdict(set)
-        for p, c in self._branches:
-            trees[p].add(c)
-        yield from trees.values()
-
-    def __repr__(self) -> str:
-        return f"{type(self).__name__}({tuple(self._branches)!r})"
```

### Comparing `ufds-0.1.0/tests/test_ufds.py` & `ufds-0.2.0/tests/test_ufds.py`

 * *Files identical despite different names*

