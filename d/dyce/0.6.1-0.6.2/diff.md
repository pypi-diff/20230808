# Comparing `tmp/dyce-0.6.1-py3-none-any.whl.zip` & `tmp/dyce-0.6.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 65384 bytes, number of entries: 15
--rw-r--r--  2.0 unx     1197 b- defN 23-Aug-03 16:02 dyce/__init__.py
--rw-r--r--  2.0 unx       48 b- defN 23-Aug-03 16:03 dyce/_version.py
--rw-r--r--  2.0 unx    33687 b- defN 23-Aug-03 16:02 dyce/evaluation.py
--rw-r--r--  2.0 unx    69614 b- defN 23-Aug-03 16:02 dyce/h.py
--rw-r--r--  2.0 unx     2038 b- defN 23-Aug-03 16:02 dyce/lifecycle.py
--rw-r--r--  2.0 unx    42284 b- defN 23-Aug-03 16:02 dyce/p.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-03 16:02 dyce/py.typed
--rw-r--r--  2.0 unx    93666 b- defN 23-Aug-03 16:02 dyce/r.py
--rw-r--r--  2.0 unx     4684 b- defN 23-Aug-03 16:02 dyce/rng.py
--rw-r--r--  2.0 unx     2461 b- defN 23-Aug-03 16:02 dyce/types.py
--rw-r--r--  2.0 unx     2132 b- defN 23-Aug-03 16:03 dyce-0.6.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    20484 b- defN 23-Aug-03 16:03 dyce-0.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 16:03 dyce-0.6.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Aug-03 16:03 dyce-0.6.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1071 b- defN 23-Aug-03 16:03 dyce-0.6.1.dist-info/RECORD
-15 files, 273463 bytes uncompressed, 63672 bytes compressed:  76.7%
+Zip file size: 66036 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     1161 b- defN 23-Aug-07 23:35 dyce/__init__.py
+-rw-r--r--  2.0 unx       48 b- defN 23-Aug-07 23:36 dyce/_version.py
+-rw-r--r--  2.0 unx    33651 b- defN 23-Aug-07 23:35 dyce/evaluation.py
+-rw-r--r--  2.0 unx    72954 b- defN 23-Aug-07 23:35 dyce/h.py
+-rw-r--r--  2.0 unx     2002 b- defN 23-Aug-07 23:35 dyce/lifecycle.py
+-rw-r--r--  2.0 unx    41921 b- defN 23-Aug-07 23:35 dyce/p.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-07 23:35 dyce/py.typed
+-rw-r--r--  2.0 unx    93838 b- defN 23-Aug-07 23:35 dyce/r.py
+-rw-r--r--  2.0 unx     4648 b- defN 23-Aug-07 23:35 dyce/rng.py
+-rw-r--r--  2.0 unx     2425 b- defN 23-Aug-07 23:35 dyce/types.py
+-rw-r--r--  2.0 unx     2132 b- defN 23-Aug-07 23:36 dyce-0.6.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    20484 b- defN 23-Aug-07 23:36 dyce-0.6.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 23:36 dyce-0.6.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Aug-07 23:36 dyce-0.6.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1071 b- defN 23-Aug-07 23:36 dyce-0.6.2.dist-info/RECORD
+15 files, 276432 bytes uncompressed, 64324 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: dyce/rng.py
 Comment: 
 
 Filename: dyce/types.py
 Comment: 
 
-Filename: dyce-0.6.1.dist-info/LICENSE
+Filename: dyce-0.6.2.dist-info/LICENSE
 Comment: 
 
-Filename: dyce-0.6.1.dist-info/METADATA
+Filename: dyce-0.6.2.dist-info/METADATA
 Comment: 
 
-Filename: dyce-0.6.1.dist-info/WHEEL
+Filename: dyce-0.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: dyce-0.6.1.dist-info/top_level.txt
+Filename: dyce-0.6.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dyce-0.6.1.dist-info/RECORD
+Filename: dyce-0.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dyce/__init__.py

```diff
@@ -2,16 +2,14 @@
 # Copyright and other protections apply. Please see the accompanying LICENSE file for
 # rights and restrictions governing use of this software. All rights not expressly
 # waived or licensed are reserved. If that file is missing or appears to be modified
 # from its original, then please contact the author before viewing or using this
 # software in any capacity.
 # ======================================================================================
 
-from __future__ import annotations
-
 from typing import Union
 
 from .evaluation import *  # noqa: F401,F403
 from .h import *  # noqa: F401,F403
 from .p import *  # noqa: F401,F403
 from .r import *  # noqa: F401,F403
 from .types import *  # noqa: F401,F403
```

## dyce/_version.py

```diff
@@ -1,3 +1,3 @@
-__vers_str__ = "0.6.1"
-__version__ = (0, 6, 1)
+__vers_str__ = "0.6.2"
+__version__ = (0, 6, 2)
```

## dyce/evaluation.py

```diff
@@ -2,16 +2,14 @@
 # Copyright and other protections apply. Please see the accompanying LICENSE file for
 # rights and restrictions governing use of this software. All rights not expressly
 # waived or licensed are reserved. If that file is missing or appears to be modified
 # from its original, then please contact the author before viewing or using this
 # software in any capacity.
 # ======================================================================================
 
-from __future__ import annotations
-
 import sys
 from contextvars import ContextVar
 from fractions import Fraction
 from functools import wraps
 from itertools import chain, product
 from math import prod
 from typing import (
```

## dyce/h.py

```diff
@@ -2,19 +2,18 @@
 # Copyright and other protections apply. Please see the accompanying LICENSE file for
 # rights and restrictions governing use of this software. All rights not expressly
 # waived or licensed are reserved. If that file is missing or appears to be modified
 # from its original, then please contact the author before viewing or using this
 # software in any capacity.
 # ======================================================================================
 
-from __future__ import annotations
-
 import os
 import warnings
 from abc import abstractmethod
+from collections import Counter
 from collections.abc import Iterable as IterableC
 from fractions import Fraction
 from itertools import chain, product, repeat
 from math import comb, gcd, sqrt
 from operator import (
     __abs__,
     __add__,
@@ -102,15 +101,15 @@
     _ROW_WIDTH = 65
 
 
 # ---- Functions -----------------------------------------------------------------------
 
 
 @deprecated
-def coalesce_replace(h: H, outcome: RealLike) -> H:
+def coalesce_replace(h: "H", outcome: RealLike) -> "H":
     r"""
     !!! warning "Deprecated"
 
         This function has been deprecated and will be removed in a future release. See
         the [``expandable`` decorator][dyce.evaluation.expandable] and
         [``foreach`` function][dyce.evaluation.foreach] for more flexible alternatives.
 
@@ -385,18 +384,14 @@
     def __init__(self, items: _SourceT) -> None:
         r"Initializer."
         super().__init__()
         self._h: _MappingT
 
         if isinstance(items, H):
             self._h = items._h
-        elif isinstance(items, Mapping):
-            self._h = dict(
-                (outcome, as_int(count)) for outcome, count in sorted(items.items())
-            )
         elif isinstance(items, SupportsInt):
             if items == 0:
                 self._h = {}
             else:
                 simple_init = as_int(items)
                 outcome_range = range(
                     simple_init if simple_init < 0 else 1,
@@ -410,14 +405,17 @@
                 #     self._h = {i: 1 for i in outcome_range}
                 assert isinstance(items, RealLike)
                 outcome_type = type(items)
                 self._h = {outcome_type(i): 1 for i in outcome_range}
         elif isinstance(items, HableT):
             self._h = items.h()._h
         elif isinstance(items, IterableC):
+            if isinstance(items, Mapping):
+                items = items.items()
+
             # items is either an Iterable[RealLike] or an Iterable[tuple[RealLike,
             # SupportsInt]] (although this technically supports Iterable[RealLike |
             # tuple[RealLike, SupportsInt]])
             self._h = {}
             sorted_items = list(items)
 
             try:
@@ -430,14 +428,17 @@
                 if isinstance(item, tuple):
                     outcome, count = item
                     count = as_int(count)
                 else:
                     outcome = item
                     count = 1
 
+                if count < 0:
+                    raise ValueError(f"count for {outcome} cannot be negative")
+
                 if outcome not in self._h:
                     self._h[outcome] = 0
 
                 self._h[outcome] += count
         else:
             raise TypeError(f"unrecognized initializer type {items!r}")
 
@@ -508,195 +509,195 @@
         return reversed(self._h)
 
     @beartype
     def __contains__(self, key: RealLike) -> bool:  # type: ignore [override]
         return key in self._h
 
     @beartype
-    def __add__(self, other: _OperandT) -> H:
+    def __add__(self, other: _OperandT) -> "H":
         try:
             return self.map(__add__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __radd__(self, other: RealLike) -> H:
+    def __radd__(self, other: RealLike) -> "H":
         try:
             return self.rmap(other, __add__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __sub__(self, other: _OperandT) -> H:
+    def __sub__(self, other: _OperandT) -> "H":
         try:
             return self.map(__sub__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rsub__(self, other: RealLike) -> H:
+    def __rsub__(self, other: RealLike) -> "H":
         try:
             return self.rmap(other, __sub__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __mul__(self, other: _OperandT) -> H:
+    def __mul__(self, other: _OperandT) -> "H":
         try:
             return self.map(__mul__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rmul__(self, other: RealLike) -> H:
+    def __rmul__(self, other: RealLike) -> "H":
         try:
             return self.rmap(other, __mul__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __matmul__(self, other: SupportsInt) -> H:
+    def __matmul__(self, other: SupportsInt) -> "H":
         try:
             other = as_int(other)
         except TypeError:
             return NotImplemented
 
         if other < 0:
             raise ValueError("argument cannot be negative")
         else:
             return sum_h(repeat(self, other))
 
     @beartype
-    def __rmatmul__(self, other: SupportsInt) -> H:
+    def __rmatmul__(self, other: SupportsInt) -> "H":
         return self.__matmul__(other)
 
     @beartype
-    def __truediv__(self, other: _OperandT) -> H:
+    def __truediv__(self, other: _OperandT) -> "H":
         try:
             return self.map(__truediv__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rtruediv__(self, other: RealLike) -> H:
+    def __rtruediv__(self, other: RealLike) -> "H":
         try:
             return self.rmap(other, __truediv__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __floordiv__(self, other: _OperandT) -> H:
+    def __floordiv__(self, other: _OperandT) -> "H":
         try:
             return self.map(__floordiv__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rfloordiv__(self, other: RealLike) -> H:
+    def __rfloordiv__(self, other: RealLike) -> "H":
         try:
             return self.rmap(other, __floordiv__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __mod__(self, other: _OperandT) -> H:
+    def __mod__(self, other: _OperandT) -> "H":
         try:
             return self.map(__mod__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rmod__(self, other: RealLike) -> H:
+    def __rmod__(self, other: RealLike) -> "H":
         try:
             return self.rmap(other, __mod__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __pow__(self, other: _OperandT) -> H:
+    def __pow__(self, other: _OperandT) -> "H":
         try:
             return self.map(__pow__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rpow__(self, other: RealLike) -> H:
+    def __rpow__(self, other: RealLike) -> "H":
         try:
             return self.rmap(other, __pow__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
     # TODO(posita): See <https://github.com/beartype/beartype/issues/152>
-    def __and__(self, other: Union[SupportsInt, "H", "HableT"]) -> H:
+    def __and__(self, other: Union[SupportsInt, "H", "HableT"]) -> "H":
         try:
             if isinstance(other, SupportsInt):
                 other = as_int(other)
 
             return self.map(__and__, other)
         except (NotImplementedError, TypeError):
             return NotImplemented
 
     @beartype
-    def __rand__(self, other: SupportsInt) -> H:
+    def __rand__(self, other: SupportsInt) -> "H":
         try:
             return self.rmap(as_int(other), __and__)
         except (NotImplementedError, TypeError):
             return NotImplemented
 
     @beartype
     # TODO(posita): See <https://github.com/beartype/beartype/issues/152>
-    def __xor__(self, other: Union[SupportsInt, "H", "HableT"]) -> H:
+    def __xor__(self, other: Union[SupportsInt, "H", "HableT"]) -> "H":
         try:
             if isinstance(other, SupportsInt):
                 other = as_int(other)
 
             return self.map(__xor__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rxor__(self, other: SupportsInt) -> H:
+    def __rxor__(self, other: SupportsInt) -> "H":
         try:
             return self.rmap(as_int(other), __xor__)
         except (NotImplementedError, TypeError):
             return NotImplemented
 
     @beartype
     # TODO(posita): See <https://github.com/beartype/beartype/issues/152>
-    def __or__(self, other: Union[SupportsInt, "H", "HableT"]) -> H:
+    def __or__(self, other: Union[SupportsInt, "H", "HableT"]) -> "H":
         try:
             if isinstance(other, SupportsInt):
                 other = as_int(other)
 
             return self.map(__or__, other)
         except (NotImplementedError, TypeError):
             return NotImplemented
 
     @beartype
-    def __ror__(self, other: SupportsInt) -> H:
+    def __ror__(self, other: SupportsInt) -> "H":
         try:
             return self.rmap(as_int(other), __or__)
         except (NotImplementedError, TypeError):
             return NotImplemented
 
     @beartype
-    def __neg__(self) -> H:
+    def __neg__(self) -> "H":
         return self.umap(__neg__)
 
     @beartype
-    def __pos__(self) -> H:
+    def __pos__(self) -> "H":
         return self.umap(__pos__)
 
     @beartype
-    def __abs__(self) -> H:
+    def __abs__(self) -> "H":
         return self.umap(__abs__)
 
     @beartype
-    def __invert__(self) -> H:
+    def __invert__(self) -> "H":
         return self.umap(__invert__)
 
     @beartype
     def counts(self) -> ValuesView[int]:
         r"""
         More descriptive synonym for the [``values`` method][dyce.h.H.values].
         """
@@ -744,15 +745,15 @@
     @classmethod
     @deprecated
     @beartype
     def foreach(
         cls,
         dependent_term: Callable[..., HOrOutcomeT],
         **independent_sources: _SourceT,
-    ) -> H:
+    ) -> "H":
         r"""
         !!! warning "Deprecated"
 
             This method has been deprecated and will be removed in a future release. See
             the [``expandable`` decorator][dyce.evaluation.expandable] and
             [``foreach`` function][dyce.evaluation.foreach] for more flexible
             alternatives.
@@ -812,15 +813,15 @@
                 outcome_kw[key] = roll[0]
 
             return dependent_term(**outcome_kw)
 
         return P.foreach(_dependent_term, **independent_sources)
 
     @beartype
-    def map(self, bin_op: _BinaryOperatorT, right_operand: _OperandT) -> H:
+    def map(self, bin_op: _BinaryOperatorT, right_operand: _OperandT) -> "H":
         r"""
         Applies *bin_op* to each outcome of the histogram as the left operand and
         *right_operand* as the right. Shorthands exist for many arithmetic operators and
         comparators.
 
         ``` python
         >>> import operator
@@ -859,15 +860,15 @@
         else:
             return type(self)(
                 (bin_op(outcome, right_operand), count)
                 for outcome, count in self.items()
             )
 
     @beartype
-    def rmap(self, left_operand: RealLike, bin_op: _BinaryOperatorT) -> H:
+    def rmap(self, left_operand: RealLike, bin_op: _BinaryOperatorT) -> "H":
         r"""
         Analogous to the [``map`` method][dyce.h.H.map], but where the caller supplies
         *left_operand*.
 
         ``` python
         >>> import operator
         >>> d6 = H(6)
@@ -885,15 +886,15 @@
             of operand ordering.
         """
         return type(self)(
             (bin_op(left_operand, outcome), count) for outcome, count in self.items()
         )
 
     @beartype
-    def umap(self, un_op: _UnaryOperatorT) -> H:
+    def umap(self, un_op: _UnaryOperatorT) -> "H":
         r"""
         Applies *un_op* to each outcome of the histogram.
 
         ``` python
         >>> import operator
         >>> H(6).umap(operator.__neg__)
         H({-6: 1, -5: 1, -4: 1, -3: 1, -2: 1, -1: 1})
@@ -905,149 +906,234 @@
         H({-27: 1, -1: 1, 4: 1, 256: 1})
 
         ```
         """
         return type(self)((un_op(outcome), count) for outcome, count in self.items())
 
     @beartype
-    def lt(self, other: _OperandT) -> H:
+    def lt(self, other: _OperandT) -> "H":
         r"""
         Shorthand for ``#!python self.map(operator.__lt__, other).umap(bool)``.
 
         ``` python
         >>> H(6).lt(3)
         H({False: 4, True: 2})
 
         ```
 
         See the [``map``][dyce.h.H.map] and [``umap``][dyce.h.H.umap] methods.
         """
         return self.map(__lt__, other).umap(bool)
 
     @beartype
-    def le(self, other: _OperandT) -> H:
+    def le(self, other: _OperandT) -> "H":
         r"""
         Shorthand for ``#!python self.map(operator.__le__, other).umap(bool)``.
 
         ``` python
         >>> H(6).le(3)
         H({False: 3, True: 3})
 
         ```
 
         See the [``map``][dyce.h.H.map] and [``umap``][dyce.h.H.umap] methods.
         """
         return self.map(__le__, other).umap(bool)
 
     @beartype
-    def eq(self, other: _OperandT) -> H:
+    def eq(self, other: _OperandT) -> "H":
         r"""
         Shorthand for ``#!python self.map(operator.__eq__, other).umap(bool)``.
 
         ``` python
         >>> H(6).eq(3)
         H({False: 5, True: 1})
 
         ```
 
         See the [``map``][dyce.h.H.map] and [``umap``][dyce.h.H.umap] methods.
         """
         return self.map(__eq__, other).umap(bool)
 
     @beartype
-    def ne(self, other: _OperandT) -> H:
+    def ne(self, other: _OperandT) -> "H":
         r"""
         Shorthand for ``#!python self.map(operator.__ne__, other).umap(bool)``.
 
         ``` python
         >>> H(6).ne(3)
         H({False: 1, True: 5})
 
         ```
 
         See the [``map``][dyce.h.H.map] and [``umap``][dyce.h.H.umap] methods.
         """
         return self.map(__ne__, other).umap(bool)
 
     @beartype
-    def gt(self, other: _OperandT) -> H:
+    def gt(self, other: _OperandT) -> "H":
         r"""
         Shorthand for ``#!python self.map(operator.__gt__, other).umap(bool)``.
 
         ``` python
         >>> H(6).gt(3)
         H({False: 3, True: 3})
 
         ```
 
         See the [``map``][dyce.h.H.map] and [``umap``][dyce.h.H.umap] methods.
         """
         return self.map(__gt__, other).umap(bool)
 
     @beartype
-    def ge(self, other: _OperandT) -> H:
+    def ge(self, other: _OperandT) -> "H":
         r"""
         Shorthand for ``#!python self.map(operator.__ge__, other).umap(bool)``.
 
         ``` python
         >>> H(6).ge(3)
         H({False: 2, True: 4})
 
         ```
 
         See the [``map``][dyce.h.H.map] and [``umap``][dyce.h.H.umap] methods.
         """
         return self.map(__ge__, other).umap(bool)
 
     @beartype
-    def is_even(self) -> H:
+    def is_even(self) -> "H":
         r"""
         Equivalent to ``#!python self.umap(dyce.types.is_even)``.
 
         ``` python
         >>> H((-4, -2, 0, 1, 2, 3)).is_even()
         H({False: 2, True: 4})
 
         ```
 
         See the [``umap`` method][dyce.h.H.umap].
         """
         return self.umap(is_even)
 
     @beartype
-    def is_odd(self) -> H:
+    def is_odd(self) -> "H":
         r"""
         Equivalent to ``#!python self.umap(dyce.types.is_odd)``.
 
         ``` python
         >>> H((-4, -2, 0, 1, 2, 3)).is_odd()
         H({False: 4, True: 2})
 
         ```
 
         See the [``umap`` method][dyce.h.H.umap].
         """
         return self.umap(is_odd)
 
     @beartype
-    def accumulate(self, other: _SourceT) -> H:
+    def accumulate(self, other: _SourceT) -> "H":
         r"""
         Accumulates counts.
 
         ``` python
         >>> H(4).accumulate(H(6))
         H({1: 2, 2: 2, 3: 2, 4: 2, 5: 1, 6: 1})
 
         ```
         """
         if not isinstance(other, H):
             other = H(other)
 
         return type(self)(cast(_SourceT, chain(self.items(), other.items())))
 
+    @beartype
+    def draw(
+        self,
+        outcomes: Optional[Union[RealLike, Iterable[RealLike], _MappingT]] = None,
+    ) -> "H":
+        r"""
+        !!! warning "Experimental"
+
+            This property should be considered experimental and may change or disappear
+            in future versions.
+
+        Returns a new [``H`` object][dyce.h.H] where the counts associated with
+        *outcomes* has been updated. This may be useful for using histograms to model
+        decks of cards (rather than dice). If *outcome* is ``#!python None``, this is
+        equivalent to ``#!python self.draw(self.roll())``.
+
+        If *outcomes* is a single value, that value’s count is decremented by one. If
+        *outcomes* is an iterable of values, those values’ outcomes are decremented by
+        one for each time that outcome appears. If *outcomes* is a mapping of outcomes
+        to counts, those outcomes are decremented by the respective counts.
+
+        Counts are not reduced and zero counts are preserved. To reduce, call the
+        [``lowest_terms`` method][dyce.h.H.lowest_terms].
+
+        <!-- BEGIN MONKEY PATCH --
+        For deterministic outcomes.
+
+        >>> import random
+        >>> from dyce import rng
+        >>> rng.RNG = random.Random(1691413956)
+
+          -- END MONKEY PATCH -->
+
+        ``` python
+        >>> H(6).draw()
+        H({1: 1, 2: 1, 3: 1, 4: 0, 5: 1, 6: 1})
+
+        >>> H(6).draw(2)
+        H({1: 1, 2: 0, 3: 1, 4: 1, 5: 1, 6: 1})
+
+        >>> H(6).draw((2, 3, 4, 5)).lowest_terms()
+        H({1: 1, 6: 1})
+
+        >>> h = H(6).accumulate(H(4)) ; h
+        H({1: 2, 2: 2, 3: 2, 4: 2, 5: 1, 6: 1})
+        >>> h.draw({1: 2, 4: 1, 6: 1})
+        H({1: 0, 2: 2, 3: 2, 4: 1, 5: 1, 6: 0})
+
+        ```
+
+        !!! tip "Negative counts can be used to increase counts"
+
+            Where *outcomes* is a mapping of outcomes to counts, negative counts can be
+            used to *increase* or “add” outcomes’ counts.
+
+            ``` python
+            >>> H(4).draw({5: -1})
+            H({1: 1, 2: 1, 3: 1, 4: 1, 5: 1})
+
+            ```
+        """
+        if outcomes is None:
+            return self.draw(self.roll())
+
+        if isinstance(outcomes, RealLike):
+            outcomes = (outcomes,)
+
+        to_draw_outcome_counts = Counter(outcomes)
+        self_outcome_counts = Counter(self)
+        # This approach is necessary because Counter.__sub__ does not preserve negative
+        # counts and Counter.subtract modifies the counter in-place
+        new_outcome_counts = Counter(self_outcome_counts)
+        new_outcome_counts.subtract(to_draw_outcome_counts)
+        would_go_negative = set(+to_draw_outcome_counts) - set(+self_outcome_counts)
+
+        if would_go_negative:
+            raise ValueError(f"outcomes to be drawn {would_go_negative} not in {self}")
+
+        zeros = set(self_outcome_counts) - set(new_outcome_counts)
+
+        for outcome in zeros:
+            new_outcome_counts[outcome] = 0
+
+        return type(self)(new_outcome_counts)
+
     @experimental
     @beartype
     def exactly_k_times_in_n(
         self,
         outcome: RealLike,
         n: SupportsInt,
         k: SupportsInt,
@@ -1080,49 +1166,49 @@
         return comb(n, k) * c_outcome**k * (self.total - c_outcome) ** (n - k)
 
     @overload
     def explode(
         self,
         max_depth: IntegralLike,
         precision_limit: None = None,
-    ) -> H:
+    ) -> "H":
         ...
 
     @overload
     def explode(
         self,
         max_depth: None,
         precision_limit: Union[RationalLikeMixedU, RealLike],
-    ) -> H:
+    ) -> "H":
         ...
 
     @overload
     def explode(
         self,
         max_depth: None = None,
         *,
         precision_limit: Union[RationalLikeMixedU, RealLike],
-    ) -> H:
+    ) -> "H":
         ...
 
     @overload
     def explode(
         self,
         max_depth: None = None,
         precision_limit: None = None,
-    ) -> H:
+    ) -> "H":
         ...
 
     @deprecated
     @beartype
     def explode(
         self,
         max_depth: Optional[IntegralLike] = None,
         precision_limit: Optional[Union[RationalLikeMixedU, RealLike]] = None,
-    ) -> H:
+    ) -> "H":
         r"""
         !!! warning "Deprecated"
 
             This method has been deprecated and will be removed in a future release. See
             the [``explode`` function][dyce.evaluation.explode] for a more flexible
             alternative.
 
@@ -1150,15 +1236,15 @@
             return self.substitute(_explode, __add__, max_depth)
         elif precision_limit is not None:
             return self.substitute(_explode, __add__, precision_limit=precision_limit)
         else:
             return self.substitute(_explode, __add__)
 
     @beartype
-    def lowest_terms(self) -> H:
+    def lowest_terms(self) -> "H":
         r"""
         Computes and returns a histogram whose nonzero counts share a greatest
         common divisor of 1.
 
         ``` python
         >>> df_obscured = H({-2: 0, -1: 2, 0: 2, 1: 2, 2: 0})
         >>> df_obscured.lowest_terms()
@@ -1178,15 +1264,15 @@
                     if count != 0
                 )
 
         return self._lowest_terms
 
     @experimental
     @beartype
-    def order_stat_for_n_at_pos(self, n: SupportsInt, pos: SupportsInt) -> H:
+    def order_stat_for_n_at_pos(self, n: SupportsInt, pos: SupportsInt) -> "H":
         r"""
         !!! warning "Experimental"
 
             This method should be considered experimental and may change or disappear in
             future versions.
 
         Computes the probability distribution for each outcome appearing in at *pos* for
@@ -1236,104 +1322,104 @@
 
         if pos < 0:
             pos = n + pos
 
         return self._order_stat_funcs_by_n[n](pos)
 
     @beartype
-    def remove(self, outcome: RealLike) -> H:
+    def remove(self, outcome: RealLike) -> "H":
         if outcome not in self:
             return self
 
         return type(self)(
             (orig_outcome, count)
             for orig_outcome, count in self.items()
             if orig_outcome != outcome
         )
 
     @overload
     def substitute(
         self,
         expand: _SubstituteExpandCallbackT,
         coalesce: _SubstituteCoalesceCallbackT = coalesce_replace,
-    ) -> H:
+    ) -> "H":
         ...
 
     @overload
     def substitute(
         self,
         expand: _SubstituteExpandCallbackT,
         coalesce: _SubstituteCoalesceCallbackT = coalesce_replace,
         *,
         max_depth: IntegralLike,
         precision_limit: None = None,
-    ) -> H:
+    ) -> "H":
         ...
 
     @overload
     def substitute(
         self,
         expand: _SubstituteExpandCallbackT,
         coalesce: _SubstituteCoalesceCallbackT,
         max_depth: IntegralLike,
         precision_limit: None = None,
-    ) -> H:
+    ) -> "H":
         ...
 
     @overload
     def substitute(
         self,
         expand: _SubstituteExpandCallbackT,
         coalesce: _SubstituteCoalesceCallbackT = coalesce_replace,
         *,
         max_depth: None,
         precision_limit: Union[RationalLikeMixedU, RealLike],
-    ) -> H:
+    ) -> "H":
         ...
 
     @overload
     def substitute(
         self,
         expand: _SubstituteExpandCallbackT,
         coalesce: _SubstituteCoalesceCallbackT,
         max_depth: None,
         precision_limit: Union[RationalLikeMixedU, RealLike],
-    ) -> H:
+    ) -> "H":
         ...
 
     @overload
     def substitute(
         self,
         expand: _SubstituteExpandCallbackT,
         coalesce: _SubstituteCoalesceCallbackT = coalesce_replace,
         max_depth: None = None,
         *,
         precision_limit: Union[RationalLikeMixedU, RealLike],
-    ) -> H:
+    ) -> "H":
         ...
 
     @overload
     def substitute(
         self,
         expand: _SubstituteExpandCallbackT,
         coalesce: _SubstituteCoalesceCallbackT = coalesce_replace,
         max_depth: None = None,
         precision_limit: None = None,
-    ) -> H:
+    ) -> "H":
         ...
 
     @deprecated
     @beartype
     def substitute(
         self,
         expand: _SubstituteExpandCallbackT,
         coalesce: _SubstituteCoalesceCallbackT = coalesce_replace,
         max_depth: Optional[IntegralLike] = None,
         precision_limit: Optional[Union[RationalLikeMixedU, RealLike]] = None,
-    ) -> H:
+    ) -> "H":
         r"""
         !!! warning "Deprecated"
 
             This method has been deprecated and will be removed in a future release. See
             the [``expandable`` decorator][dyce.evaluation.expandable] and
             [``foreach`` function][dyce.evaluation.foreach] for more flexible
             alternatives.
@@ -1380,15 +1466,15 @@
             res = expand(result.h, result.outcome)
 
             return coalesce(_expand(res), result.outcome) if isinstance(res, H) else res
 
         return _expand(self, limit=limit)
 
     @beartype
-    def vs(self, other: _OperandT) -> H:
+    def vs(self, other: _OperandT) -> "H":
         r"""
         Compares the histogram with *other*. -1 represents where *other* is greater. 0
         represents where they are equal. 1 represents where *other* is less.
 
         Shorthand for ``#!python self.within(0, 0, other)``.
 
         ``` python
@@ -1400,15 +1486,15 @@
         ```
 
         See the [``within`` method][dyce.h.H.within].
         """
         return self.within(0, 0, other)
 
     @beartype
-    def within(self, lo: RealLike, hi: RealLike, other: _OperandT = 0) -> H:
+    def within(self, lo: RealLike, hi: RealLike, other: _OperandT = 0) -> "H":
         r"""
         Computes the difference between the histogram and *other*. -1 represents where that
         difference is less than *lo*. 0 represents where that difference between *lo*
         and *hi* (inclusive). 1 represents where that difference is greater than *hi*.
 
         ``` python
         >>> d6_2 = 2@H(6)
@@ -1437,15 +1523,15 @@
           1 |  50.00% |#########################
 
         ```
         """
         return self.map(_within(lo, hi), other)
 
     @beartype
-    def zero_fill(self, outcomes: Iterable[RealLike]) -> H:
+    def zero_fill(self, outcomes: Iterable[RealLike]) -> "H":
         r"""
         Shorthand for ``#!python self.accumulate({outcome: 0 for outcome in
         outcomes})``.
 
         ``` python
         >>> H(4).zero_fill(H(8).outcomes())
         H({1: 1, 2: 1, 3: 1, 4: 1, 5: 0, 6: 0, 7: 0, 8: 0})
@@ -1633,14 +1719,19 @@
 
         If *scaled* is ``#!python True``, horizontal bars are scaled to *width*.
 
         ``` python
         >>> h = (2@H(6)).ge(7)
         >>> print(f"{' 65 chars wide -->|':->65}")
         ---------------------------------------------- 65 chars wide -->|
+        >>> print(H(1).format(scaled=False))
+        avg |    1.00
+        std |    0.00
+        var |    0.00
+          1 | 100.00% |##################################################
         >>> print(h.format(scaled=False))
         avg |    0.58
         std |    0.49
         var |    0.24
           0 |  41.67% |####################
           1 |  58.33% |#############################
         >>> print(h.format(scaled=True))
@@ -1747,27 +1838,27 @@
         # more efficient E[X**2] - E[X]**2. See
         # <https://dlsun.github.io/probability/variance.html>.
         return numerator / (denominator or 1) - mu**2
 
     @beartype
     def roll(self) -> RealLike:
         r"""
-        Returns a (weighted) random outcome, sorted.
+        Returns a (weighted) random outcome.
         """
         return (
             rng.RNG.choices(
                 population=tuple(self.outcomes()),
                 weights=tuple(self.counts()),
                 k=1,
             )[0]
             if self
             else 0
         )
 
-    def _order_stat_func_for_n(self, n: int) -> Callable[[int], H]:
+    def _order_stat_func_for_n(self, n: int) -> Callable[[int], "H"]:
         betas_by_outcome: dict[RealLike, tuple[H, H]] = {}
 
         for outcome in self.outcomes():
             betas_by_outcome[outcome] = (
                 n @ self.le(outcome),
                 n @ self.lt(outcome),
             )
@@ -1776,15 +1867,15 @@
             for outcome, (h_le, h_lt) in betas_by_outcome.items():
                 yield (
                     outcome,
                     h_le.gt(pos).get(True, 0) - h_lt.gt(pos).get(True, 0),
                 )
 
         @beartype
-        def order_stat_for_n_at_pos(pos: int) -> H:
+        def order_stat_for_n_at_pos(pos: int) -> "H":
             return type(self)(_gen_h_items_at_pos(pos))
 
         return order_stat_for_n_at_pos
 
 
 @runtime_checkable
 class HableT(Protocol, metaclass=CachingProtocolMeta):
```

## dyce/lifecycle.py

```diff
@@ -2,16 +2,14 @@
 # Copyright and other protections apply. Please see the accompanying LICENSE file for
 # rights and restrictions governing use of this software. All rights not expressly
 # waived or licensed are reserved. If that file is missing or appears to be modified
 # from its original, then please contact the author before viewing or using this
 # software in any capacity.
 # ======================================================================================
 
-from __future__ import annotations
-
 import warnings
 from functools import wraps
 from typing import Any, Callable, Type, TypeVar, cast
 
 __all__ = ()
```

## dyce/p.py

```diff
@@ -2,19 +2,17 @@
 # Copyright and other protections apply. Please see the accompanying LICENSE file for
 # rights and restrictions governing use of this software. All rights not expressly
 # waived or licensed are reserved. If that file is missing or appears to be modified
 # from its original, then please contact the author before viewing or using this
 # software in any capacity.
 # ======================================================================================
 
-from __future__ import annotations
-
-from collections import Counter, defaultdict
+from collections import Counter
 from fractions import Fraction
-from functools import wraps
+from functools import cache
 from itertools import chain, groupby, product, repeat
 from math import prod
 from operator import __eq__, __index__, __ne__
 from typing import (
     Any,
     Callable,
     Iterable,
@@ -288,42 +286,42 @@
         return len(self._hs)
 
     @overload
     def __getitem__(self, key: SupportsIndex) -> H:
         ...
 
     @overload
-    def __getitem__(self, key: slice) -> P:
+    def __getitem__(self, key: slice) -> "P":
         ...
 
     @beartype
     def __getitem__(self, key: _GetItemT) -> Union[H, "P"]:
         if isinstance(key, slice):
             return P(*self._hs[key])
         else:
             return self._hs[__index__(key)]
 
     @beartype
     def __iter__(self) -> Iterator[H]:
         return iter(self._hs)
 
     @beartype
-    def __matmul__(self, other: SupportsInt) -> P:
+    def __matmul__(self, other: SupportsInt) -> "P":
         try:
             other = as_int(other)
         except TypeError:
             return NotImplemented
 
         if other < 0:
             raise ValueError("argument cannot be negative")
         else:
             return P(*chain.from_iterable(repeat(self, other)))
 
     @beartype
-    def __rmatmul__(self, other: SupportsInt) -> P:
+    def __rmatmul__(self, other: SupportsInt) -> "P":
         return self.__matmul__(other)
 
     @beartype
     def h(self, *which: _GetItemT) -> H:
         r"""
         Roughly equivalent to ``#!python H((sum(roll), count) for roll, count in
         self.rolls_with_counts(*which))`` with some short-circuit optimizations.
@@ -921,15 +919,15 @@
                 taken_outcomes = tuple(getitems(sorted_outcomes_for_roll, which))
             else:
                 taken_outcomes = sorted_outcomes_for_roll
 
             yield taken_outcomes, roll_count
 
     @beartype
-    def map(self, op: _BinaryOperatorT, right_operand: _OperandT) -> P:
+    def map(self, op: _BinaryOperatorT, right_operand: _OperandT) -> "P":
         r"""
         Shorthand for ``#!python P(*(h.map(op, right_operand) for h in self))``. See the
         [``H.map`` method][dyce.h.H.map].
 
         ``` python
         >>> import operator
         >>> p_3d6 = 3@P(H((-3, -1, 2, 4)))
@@ -937,15 +935,15 @@
         3@P(H({-4: 1, -2: 1, 1: 1, 3: 1}))
 
         ```
         """
         return P(*(h.map(op, right_operand) for h in self))
 
     @beartype
-    def rmap(self, left_operand: RealLike, op: _BinaryOperatorT) -> P:
+    def rmap(self, left_operand: RealLike, op: _BinaryOperatorT) -> "P":
         r"""
         Shorthand for ``#!python P(*(h.rmap(left_operand, op) for h in self))``. See the
         [``H.rmap`` method][dyce.h.H.rmap].
 
         ``` python
         >>> import operator
         >>> from fractions import Fraction
@@ -954,15 +952,15 @@
         2@P(H({Fraction(-1, 1): 1, Fraction(-1, 3): 1, Fraction(1, 4): 1, Fraction(1, 2): 1}))
 
         ```
         """
         return P(*(h.rmap(left_operand, op) for h in self))
 
     @beartype
-    def umap(self, op: _UnaryOperatorT) -> P:
+    def umap(self, op: _UnaryOperatorT) -> "P":
         r"""
         Shorthand for ``#!python P(*(h.umap(op) for h in self))``. See the
         [``H.umap`` method][dyce.h.H.umap].
 
         ``` python
         >>> import operator
         >>> p_3d6 = 3@P(H((-3, -1, 2, 4)))
@@ -1107,45 +1105,52 @@
     >>> sorted(_rwc_homogeneous_n_h_using_partial_selection(3, H(6), -2, fill=0))
     [((0, 1, 1), 1), ((0, 1, 2), 3), ((0, 1, 3), 3), ..., ((0, 5, 5), 13), ((0, 5, 6), 27), ((0, 6, 6), 16)]
 
     ```
     """
     n = as_int(n)
     k = as_int(k)
-    from_upper = k < 0
+    from_right = k < 0
     k = abs(k)
 
     if k == 0 or k > n:
         # Maintain consistency with comb(n, k) == 0 where k > n
         return iter(())
 
-    def _memoize(f: _SelectCallableT) -> _SelectCallableT:
-        cache: defaultdict[tuple[H, int, int], list[_RollProbT]] = defaultdict(list)
+    total_count = h.total**n
 
-        @wraps(f)
-        def _wrapped(h: H, n: int, k: int) -> Iterator[_RollProbT]:
-            if (h, n, k) not in cache:
-                cache[h, n, k].extend(f(h, n, k))
+    for outcomes, prob_nmr8r, prob_dnmn8r in _selected_distros_memoized(
+        h, n, k, from_right
+    ):
+        count = total_count * prob_nmr8r // prob_dnmn8r
 
-            return iter(cache[h, n, k])
+        if fill is not None:
+            outcomes = (
+                (fill,) * (n - k) + outcomes
+                if from_right
+                else outcomes + (fill,) * (n - k)
+            )
+
+        yield (outcomes, count)
 
-        return _wrapped
 
-    @_memoize
-    def _selected_distributions(h: H, n: int, k: int) -> Iterator[_RollProbT]:
+@cache
+def _selected_distros_memoized(
+    h: H,
+    n: int,
+    k: int,
+    from_right: bool,
+) -> tuple[_RollProbT, ...]:
+    def _selected_distros_gen() -> Iterator[_RollProbT]:
         if len(h) <= 1:
             whole = tuple(h) * k
             yield whole, 1, 1
         else:
             this_total = h.total**n
-
-            if from_upper:
-                this_outcome = max(h)
-            else:
-                this_outcome = min(h)
+            this_outcome = max(h) if from_right else min(h)
 
             next_h = type(h)(
                 (outcome, count)
                 for outcome, count in h.items()
                 if outcome != this_outcome
             )
             cumulative_p = Fraction(0)
@@ -1153,39 +1158,23 @@
             for i in range(0, k + 1):
                 head = i * (this_outcome,)
 
                 if i < k:
                     head_count = h.exactly_k_times_in_n(this_outcome, n, i)
                     cumulative_p += Fraction(head_count, this_total)
 
-                    for tail, tail_num, tail_denom in _selected_distributions(
-                        next_h, n - i, k - i
+                    for tail, tail_nmr8r, tail_dnmn8r in _selected_distros_memoized(
+                        next_h, n - i, k - i, from_right
                     ):
-                        if from_upper:
-                            whole = tail + head
-                        else:
-                            whole = head + tail
-
-                        whole_num = head_count * tail_num
-                        whole_denom = this_total * tail_denom
-                        yield whole, whole_num, whole_denom
+                        whole = tail + head if from_right else head + tail
+                        whole_nmr8r = head_count * tail_nmr8r
+                        whole_dnmn8r = this_total * tail_dnmn8r
+                        yield whole, whole_nmr8r, whole_dnmn8r
                 else:
                     # This optimization exploits the fact that the probability of all
                     # rolls comprising [k, n] of outcome is the probability of all rolls
                     # (i.e., 1) minus the cumulative probabilities of all rolls
                     # comprising [0, k) of outcome (computed above)
                     remaining_p = Fraction(1) - cumulative_p
                     yield head, remaining_p.numerator, remaining_p.denominator
 
-    total_count = h.total**n
-
-    for outcomes, num, denom in _selected_distributions(h, n, k):
-        count = total_count * num // denom
-
-        if fill is not None:
-            outcomes = (
-                (fill,) * (n - k) + outcomes
-                if from_upper
-                else outcomes + (fill,) * (n - k)
-            )
-
-        yield (outcomes, count)
+    return tuple(_selected_distros_gen())
```

## dyce/r.py

```diff
@@ -2,16 +2,14 @@
 # Copyright and other protections apply. Please see the accompanying LICENSE file for
 # rights and restrictions governing use of this software. All rights not expressly
 # waived or licensed are reserved. If that file is missing or appears to be modified
 # from its original, then please contact the author before viewing or using this
 # software in any capacity.
 # ======================================================================================
 
-from __future__ import annotations
-
 import enum
 import warnings
 from abc import abstractmethod
 from collections import defaultdict, deque
 from copy import copy
 from itertools import chain
 from operator import (
@@ -309,196 +307,196 @@
     def __ne__(self, other) -> bool:
         if isinstance(other, R):
             return not __eq__(self, other)
         else:
             return super().__ne__(other)
 
     @beartype
-    def __add__(self, other: _ROperandT) -> BinarySumOpRoller:
+    def __add__(self, other: _ROperandT) -> "BinarySumOpRoller":
         try:
             return self.map(__add__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __radd__(self, other: RealLike) -> BinarySumOpRoller:
+    def __radd__(self, other: RealLike) -> "BinarySumOpRoller":
         try:
             return self.rmap(other, __add__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __sub__(self, other: _ROperandT) -> BinarySumOpRoller:
+    def __sub__(self, other: _ROperandT) -> "BinarySumOpRoller":
         try:
             return self.map(__sub__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rsub__(self, other: RealLike) -> BinarySumOpRoller:
+    def __rsub__(self, other: RealLike) -> "BinarySumOpRoller":
         try:
             return self.rmap(other, __sub__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __mul__(self, other: _ROperandT) -> BinarySumOpRoller:
+    def __mul__(self, other: _ROperandT) -> "BinarySumOpRoller":
         try:
             return self.map(__mul__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rmul__(self, other: RealLike) -> BinarySumOpRoller:
+    def __rmul__(self, other: RealLike) -> "BinarySumOpRoller":
         try:
             return self.rmap(other, __mul__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __matmul__(self, other: SupportsInt) -> R:
+    def __matmul__(self, other: SupportsInt) -> "R":
         try:
             other = as_int(other)
         except TypeError:
             return NotImplemented
 
         if other < 0:
             raise ValueError("argument cannot be negative")
         else:
             return RepeatRoller(other, self)
 
     @beartype
-    def __rmatmul__(self, other: SupportsInt) -> R:
+    def __rmatmul__(self, other: SupportsInt) -> "R":
         return self.__matmul__(other)
 
     @beartype
-    def __truediv__(self, other: _ROperandT) -> BinarySumOpRoller:
+    def __truediv__(self, other: _ROperandT) -> "BinarySumOpRoller":
         try:
             return self.map(__truediv__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rtruediv__(self, other: RealLike) -> BinarySumOpRoller:
+    def __rtruediv__(self, other: RealLike) -> "BinarySumOpRoller":
         try:
             return self.rmap(other, __truediv__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __floordiv__(self, other: _ROperandT) -> BinarySumOpRoller:
+    def __floordiv__(self, other: _ROperandT) -> "BinarySumOpRoller":
         try:
             return self.map(__floordiv__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rfloordiv__(self, other: RealLike) -> BinarySumOpRoller:
+    def __rfloordiv__(self, other: RealLike) -> "BinarySumOpRoller":
         try:
             return self.rmap(other, __floordiv__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __mod__(self, other: _ROperandT) -> BinarySumOpRoller:
+    def __mod__(self, other: _ROperandT) -> "BinarySumOpRoller":
         try:
             return self.map(__mod__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rmod__(self, other: RealLike) -> BinarySumOpRoller:
+    def __rmod__(self, other: RealLike) -> "BinarySumOpRoller":
         try:
             return self.rmap(other, __mod__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __pow__(self, other: _ROperandT) -> BinarySumOpRoller:
+    def __pow__(self, other: _ROperandT) -> "BinarySumOpRoller":
         try:
             return self.map(__pow__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rpow__(self, other: RealLike) -> BinarySumOpRoller:
+    def __rpow__(self, other: RealLike) -> "BinarySumOpRoller":
         try:
             return self.rmap(other, __pow__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __and__(self, other: Union[_SourceT, SupportsInt]) -> BinarySumOpRoller:
+    def __and__(self, other: Union[_SourceT, SupportsInt]) -> "BinarySumOpRoller":
         try:
             if isinstance(other, R):
                 return self.map(__and__, other)
             else:
                 return self.map(__and__, as_int(other))
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rand__(self, other: SupportsInt) -> BinarySumOpRoller:
+    def __rand__(self, other: SupportsInt) -> "BinarySumOpRoller":
         try:
             return self.rmap(as_int(other), __and__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __xor__(self, other: Union[_SourceT, SupportsInt]) -> BinarySumOpRoller:
+    def __xor__(self, other: Union[_SourceT, SupportsInt]) -> "BinarySumOpRoller":
         try:
             if isinstance(other, R):
                 return self.map(__xor__, other)
             else:
                 return self.map(__xor__, as_int(other))
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rxor__(self, other: SupportsInt) -> BinarySumOpRoller:
+    def __rxor__(self, other: SupportsInt) -> "BinarySumOpRoller":
         try:
             return self.rmap(as_int(other), __xor__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __or__(self, other: Union[_SourceT, SupportsInt]) -> BinarySumOpRoller:
+    def __or__(self, other: Union[_SourceT, SupportsInt]) -> "BinarySumOpRoller":
         try:
             if isinstance(other, R):
                 return self.map(__or__, other)
             else:
                 return self.map(__or__, as_int(other))
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __ror__(self, other: SupportsInt) -> BinarySumOpRoller:
+    def __ror__(self, other: SupportsInt) -> "BinarySumOpRoller":
         try:
             return self.rmap(as_int(other), __or__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __neg__(self) -> UnarySumOpRoller:
+    def __neg__(self) -> "UnarySumOpRoller":
         return self.umap(__neg__)
 
     @beartype
-    def __pos__(self) -> UnarySumOpRoller:
+    def __pos__(self) -> "UnarySumOpRoller":
         return self.umap(__pos__)
 
     @beartype
-    def __abs__(self) -> UnarySumOpRoller:
+    def __abs__(self) -> "UnarySumOpRoller":
         return self.umap(__abs__)
 
     @beartype
-    def __invert__(self) -> UnarySumOpRoller:
+    def __invert__(self) -> "UnarySumOpRoller":
         return self.umap(__invert__)
 
     @abstractmethod
-    def roll(self) -> Roll:
+    def roll(self) -> "Roll":
         r"""
         Sub-classes should implement this method to return a new
         [``Roll`` object][dyce.r.Roll] taking into account any
         [sources][dyce.r.R.sources].
 
         !!! note
 
@@ -634,29 +632,29 @@
 
     @classmethod
     @beartype
     def from_sources(
         cls,
         *sources: _SourceT,
         annotation: Any = "",
-    ) -> PoolRoller:
+    ) -> "PoolRoller":
         r"""
         Shorthand for ``#!python cls.from_sources_iterable(rs, annotation=annotation)``.
 
         See the [``from_sources_iterable`` method][dyce.r.R.from_sources_iterable].
         """
         return cls.from_sources_iterable(sources, annotation=annotation)
 
     @classmethod
     @beartype
     def from_sources_iterable(
         cls,
         sources: Iterable[_SourceT],
         annotation: Any = "",
-    ) -> PoolRoller:
+    ) -> "PoolRoller":
         r"""
         Creates and returns a roller for “pooling” zero or more *sources*.
 
         <!-- BEGIN MONKEY PATCH --
         For deterministic outcomes.
 
         >>> import random
@@ -696,15 +694,15 @@
 
     @classmethod
     @beartype
     def from_value(
         cls,
         value: _ValueT,
         annotation: Any = "",
-    ) -> ValueRoller:
+    ) -> "ValueRoller":
         r"""
         Creates and returns a [``ValueRoller``][dyce.r.ValueRoller] from *value*.
 
         ``` python
         >>> R.from_value(6)
         ValueRoller(value=6, annotation='')
 
@@ -726,29 +724,29 @@
 
     @classmethod
     @beartype
     def from_values(
         cls,
         *values: _ValueT,
         annotation: Any = "",
-    ) -> PoolRoller:
+    ) -> "PoolRoller":
         r"""
         Shorthand for ``#!python cls.from_values_iterable(values, annotation=annotation)``.
 
         See the [``from_values_iterable`` method][dyce.r.R.from_values_iterable].
         """
         return cls.from_values_iterable(values, annotation=annotation)
 
     @classmethod
     @beartype
     def from_values_iterable(
         cls,
         values: Iterable[_ValueT],
         annotation: Any = "",
-    ) -> PoolRoller:
+    ) -> "PoolRoller":
         r"""
         Shorthand for ``#!python cls.from_sources_iterable((cls.from_value(value) for value
         in values), annotation=annotation)``.
 
         See the [``from_value``][dyce.r.R.from_value] and
         [``from_sources_iterable``][dyce.r.R.from_sources_iterable] methods.
         """
@@ -760,15 +758,15 @@
     @classmethod
     @beartype
     def filter_from_sources(
         cls,
         predicate: _PredicateT,
         *sources: _SourceT,
         annotation: Any = "",
-    ) -> FilterRoller:
+    ) -> "FilterRoller":
         r"""
         Shorthand for ``#!python cls.filter_from_sources_iterable(predicate, sources,
         annotation=annotation)``.
 
         See the [``filter_from_sources_iterable``
         method][dyce.r.R.filter_from_sources_iterable].
         """
@@ -779,15 +777,15 @@
     @classmethod
     @beartype
     def filter_from_sources_iterable(
         cls,
         predicate: _PredicateT,
         sources: Iterable[_SourceT],
         annotation: Any = "",
-    ) -> FilterRoller:
+    ) -> "FilterRoller":
         r"""
         Creates and returns a [``FilterRoller``][dyce.r.FilterRoller] for applying filterion
         *predicate* to sorted outcomes from *sources*.
 
         ``` python
         >>> r_filter = R.filter_from_sources_iterable(
         ...   lambda outcome: bool(outcome.is_even().value),
@@ -814,15 +812,15 @@
     @classmethod
     @beartype
     def filter_from_values(
         cls,
         predicate: _PredicateT,
         *values: _ValueT,
         annotation: Any = "",
-    ) -> FilterRoller:
+    ) -> "FilterRoller":
         r"""
         Shorthand for ``#!python cls.filter_from_values_iterable(predicate, values,
         annotation=annotation)``.
 
         See the
         [``filter_from_values_iterable`` method][dyce.r.R.filter_from_values_iterable].
         """
@@ -831,15 +829,15 @@
     @classmethod
     @beartype
     def filter_from_values_iterable(
         cls,
         predicate: _PredicateT,
         values: Iterable[_ValueT],
         annotation: Any = "",
-    ) -> FilterRoller:
+    ) -> "FilterRoller":
         r"""
         Shorthand for ``#!python cls.filter_from_sources_iterable((cls.from_value(value) for
         value in values), annotation=annotation)``.
 
         See the [``from_value``][dyce.r.R.from_value] and
         [``filter_from_sources_iterable``][dyce.r.R.filter_from_sources_iterable]
         methods.
@@ -853,15 +851,15 @@
     @classmethod
     @beartype
     def select_from_sources(
         cls,
         which: Iterable[_GetItemT],
         *sources: _SourceT,
         annotation: Any = "",
-    ) -> SelectionRoller:
+    ) -> "SelectionRoller":
         r"""
         Shorthand for ``#!python cls.select_from_sources_iterable(which, sources,
         annotation=annotation)``.
 
         See the [``select_from_sources_iterable``
         method][dyce.r.R.select_from_sources_iterable].
         """
@@ -870,15 +868,15 @@
     @classmethod
     @beartype
     def select_from_sources_iterable(
         cls,
         which: Iterable[_GetItemT],
         sources: Iterable[_SourceT],
         annotation: Any = "",
-    ) -> SelectionRoller:
+    ) -> "SelectionRoller":
         r"""
         Creates and returns a [``SelectionRoller``][dyce.r.SelectionRoller] for applying
         selection *which* to sorted outcomes from *sources*.
 
         ``` python
         >>> r_select = R.select_from_sources_iterable(
         ...   (0, -1, slice(3, 6), slice(6, 3, -1), -1, 0),
@@ -905,15 +903,15 @@
     @classmethod
     @beartype
     def select_from_values(
         cls,
         which: Iterable[_GetItemT],
         *values: _ValueT,
         annotation: Any = "",
-    ) -> SelectionRoller:
+    ) -> "SelectionRoller":
         r"""
         Shorthand for ``#!python cls.select_from_values_iterable(which, values,
         annotation=annotation)``.
 
         See the
         [``select_from_values_iterable`` method][dyce.r.R.select_from_values_iterable].
         """
@@ -922,15 +920,15 @@
     @classmethod
     @beartype
     def select_from_values_iterable(
         cls,
         which: Iterable[_GetItemT],
         values: Iterable[_ValueT],
         annotation: Any = "",
-    ) -> SelectionRoller:
+    ) -> "SelectionRoller":
         r"""
         Shorthand for ``#!python cls.select_from_sources_iterable((cls.from_value(value) for
         value in values), annotation=annotation)``.
 
         See the [``from_value``][dyce.r.R.from_value] and
         [``select_from_sources_iterable``][dyce.r.R.select_from_sources_iterable]
         methods.
@@ -946,15 +944,15 @@
         r"""
         Generates new rolls from all [``sources``][dyce.r.R.sources].
         """
         for source in self.sources:
             yield source.roll()
 
     @beartype
-    def annotate(self, annotation: Any = "") -> R:
+    def annotate(self, annotation: Any = "") -> "R":
         r"""
         Generates a copy of the roller with the desired annotation.
 
         ``` python
         >>> r_just_the_n_of_us = R.from_value(5, annotation="But I'm 42!") ; r_just_the_n_of_us
         ValueRoller(value=5, annotation="But I'm 42!")
         >>> r_just_the_n_of_us.annotate("I'm a 42-year-old investment banker!")
@@ -969,15 +967,15 @@
 
     @beartype
     def map(
         self,
         bin_op: _RollOutcomeBinaryOperatorT,
         right_operand: _ROperandT,
         annotation: Any = "",
-    ) -> BinarySumOpRoller:
+    ) -> "BinarySumOpRoller":
         r"""
         Creates and returns a [``BinarySumOpRoller``][dyce.r.BinarySumOpRoller] for applying
         *bin_op* to this roller and *right_operand* as its sources. Shorthands exist for
         many arithmetic operators and comparators.
 
         ``` python
         >>> import operator
@@ -1004,15 +1002,15 @@
     @beartype
     def rmap(
         self,
         # TODO(posita): See <https://github.com/beartype/beartype/issues/152>
         left_operand: Union[RealLike, "RollOutcome"],
         bin_op: _RollOutcomeBinaryOperatorT,
         annotation: Any = "",
-    ) -> BinarySumOpRoller:
+    ) -> "BinarySumOpRoller":
         r"""
         Analogous to the [``map`` method][dyce.r.R.map], but where the caller supplies
         *left_operand*.
 
         ``` python
         >>> import operator
         >>> r_bin_op = R.from_value(H(6)).rmap(2, operator.__pow__) ; r_bin_op
@@ -1043,15 +1041,15 @@
             raise NotImplementedError
 
     @beartype
     def umap(
         self,
         un_op: _RollOutcomeUnaryOperatorT,
         annotation: Any = "",
-    ) -> UnarySumOpRoller:
+    ) -> "UnarySumOpRoller":
         r"""
         Creates and returns a [``UnarySumOpRoller``][dyce.r.UnarySumOpRoller] roller for
         applying *un_op* to this roller as its source.
 
         ``` python
         >>> import operator
         >>> r_un_op = R.from_value(H(6)).umap(operator.__neg__) ; r_un_op
@@ -1064,106 +1062,106 @@
         True
 
         ```
         """
         return UnarySumOpRoller(un_op, self, annotation=annotation)
 
     @beartype
-    def lt(self, other: _ROperandT) -> BinarySumOpRoller:
+    def lt(self, other: _ROperandT) -> "BinarySumOpRoller":
         r"""
         Shorthand for ``#!python self.map(lambda left, right: left.lt(right), other)``.
 
         See the [``map`` method][dyce.r.R.map].
         """
 
         def _lt(left_operand: RollOutcome, right_operand: RollOutcome) -> RollOutcome:
             return left_operand.lt(right_operand)
 
         return self.map(_lt, other)
 
     @beartype
-    def le(self, other: _ROperandT) -> BinarySumOpRoller:
+    def le(self, other: _ROperandT) -> "BinarySumOpRoller":
         r"""
         Shorthand for ``#!python self.map(lambda left, right: left.le(right), other)``.
 
         See the [``map`` method][dyce.r.R.map].
         """
 
         def _le(left_operand: RollOutcome, right_operand: RollOutcome) -> RollOutcome:
             return left_operand.le(right_operand)
 
         return self.map(_le, other)
 
     @beartype
-    def eq(self, other: _ROperandT) -> BinarySumOpRoller:
+    def eq(self, other: _ROperandT) -> "BinarySumOpRoller":
         r"""
         Shorthand for ``#!python self.map(lambda left, right: left.eq(right), other)``.
 
         See the [``map`` method][dyce.r.R.map].
         """
 
         def _eq(left_operand: RollOutcome, right_operand: RollOutcome) -> RollOutcome:
             return left_operand.eq(right_operand)
 
         return self.map(_eq, other)
 
     @beartype
-    def ne(self, other: _ROperandT) -> BinarySumOpRoller:
+    def ne(self, other: _ROperandT) -> "BinarySumOpRoller":
         r"""
         Shorthand for ``#!python self.map(lambda left, right: left.ne(right), other)``.
 
         See the [``map`` method][dyce.r.R.map].
         """
 
         def _ne(left_operand: RollOutcome, right_operand: RollOutcome) -> RollOutcome:
             return left_operand.ne(right_operand)
 
         return self.map(_ne, other)
 
     @beartype
-    def gt(self, other: _ROperandT) -> BinarySumOpRoller:
+    def gt(self, other: _ROperandT) -> "BinarySumOpRoller":
         r"""
         Shorthand for ``#!python self.map(lambda left, right: left.gt(right), other)``.
 
         See the [``map`` method][dyce.r.R.map].
         """
 
         def _gt(left_operand: RollOutcome, right_operand: RollOutcome) -> RollOutcome:
             return left_operand.gt(right_operand)
 
         return self.map(_gt, other)
 
     @beartype
-    def ge(self, other: _ROperandT) -> BinarySumOpRoller:
+    def ge(self, other: _ROperandT) -> "BinarySumOpRoller":
         r"""
         Shorthand for ``#!python self.map(lambda left, right: left.ge(right), other)``.
 
         See the [``map`` method][dyce.r.R.map].
         """
 
         def _ge(left_operand: RollOutcome, right_operand: RollOutcome) -> RollOutcome:
             return left_operand.ge(right_operand)
 
         return self.map(_ge, other)
 
     @beartype
-    def is_even(self) -> UnarySumOpRoller:
+    def is_even(self) -> "UnarySumOpRoller":
         r"""
         Shorthand for: ``#!python self.umap(lambda operand: operand.is_even())``.
 
         See the [``umap`` method][dyce.r.R.umap].
         """
 
         def _is_even(operand: RollOutcome) -> RollOutcome:
             return operand.is_even()
 
         return self.umap(_is_even)
 
     @beartype
-    def is_odd(self) -> UnarySumOpRoller:
+    def is_odd(self) -> "UnarySumOpRoller":
         r"""
         Shorthand for: ``#!python self.umap(lambda operand: operand.is_odd())``.
 
         See the [``umap`` method][dyce.r.R.umap].
         """
 
         def _is_odd(operand: RollOutcome) -> RollOutcome:
@@ -1172,42 +1170,42 @@
         return self.umap(_is_odd)
 
     @beartype
     def filter(
         self,
         predicate: _PredicateT,
         annotation: Any = "",
-    ) -> FilterRoller:
+    ) -> "FilterRoller":
         r"""
         Shorthand for ``#!python type(self).filter_from_sources(predicate, self,
         annotation=annotation)``.
 
         See the [``filter_from_sources`` method][dyce.r.R.filter_from_sources].
         """
         return type(self).filter_from_sources(predicate, self, annotation=annotation)
 
     @beartype
     def select(
         self,
         *which: _GetItemT,
         annotation: Any = "",
-    ) -> SelectionRoller:
+    ) -> "SelectionRoller":
         r"""
         Shorthand for ``#!python self.select_iterable(which, annotation=annotation)``.
 
         See the [``select_iterable`` method][dyce.r.R.select_iterable].
         """
         return self.select_iterable(which, annotation=annotation)
 
     @beartype
     def select_iterable(
         self,
         which: Iterable[_GetItemT],
         annotation: Any = "",
-    ) -> SelectionRoller:
+    ) -> "SelectionRoller":
         r"""
         Shorthand for ``#!python type(self).select_from_sources(which, self,
         annotation=annotation)``.
 
         See the [``select_from_sources`` method][dyce.r.R.select_from_sources].
         """
         return type(self).select_from_sources(which, self, annotation=annotation)
@@ -1245,15 +1243,15 @@
     # ---- Overrides -------------------------------------------------------------------
 
     @beartype
     def __repr__(self) -> str:
         return f"{type(self).__name__}(value={self.value!r}, annotation={self.annotation!r})"
 
     @beartype
-    def roll(self) -> Roll:
+    def roll(self) -> "Roll":
         r""""""
         if isinstance(self.value, P):
             return Roll(
                 self,
                 roll_outcomes=(RollOutcome(outcome) for outcome in self.value.roll()),
             )
         elif isinstance(self.value, H):
@@ -1334,15 +1332,15 @@
     ```
     """
     __slots__: Any = ()
 
     # ---- Overrides -------------------------------------------------------------------
 
     @beartype
-    def roll(self) -> Roll:
+    def roll(self) -> "Roll":
         r""""""
         source_rolls = list(self.source_rolls())
 
         return Roll(
             self,
             roll_outcomes=(
                 roll_outcome
@@ -1402,15 +1400,15 @@
 )"""
 
     @beartype
     def __eq__(self, other) -> bool:
         return super().__eq__(other) and self.n == other.n
 
     @beartype
-    def roll(self) -> Roll:
+    def roll(self) -> "Roll":
         r""""""
         source_rolls: list[Roll] = []
 
         for _ in range(self.n):
             source_rolls.extend(self.source_rolls())
 
         return Roll(
@@ -1466,15 +1464,15 @@
 )"""
 
     @beartype
     def __eq__(self, other) -> bool:
         return super().__eq__(other) and (_callable_cmp(self.op, other.op))
 
     @beartype
-    def roll(self) -> Roll:
+    def roll(self) -> "Roll":
         r""""""
         source_rolls = list(self.source_rolls())
         res = self.op(
             self,
             (
                 roll_outcome
                 for roll_outcome in chain.from_iterable(source_rolls)
@@ -1505,15 +1503,15 @@
     grouped by each of *sources*.
     """
     __slots__: Any = ()
 
     # ---- Overrides -------------------------------------------------------------------
 
     @beartype
-    def roll(self) -> Roll:
+    def roll(self) -> "Roll":
         r""""""
         source_rolls = list(self.source_rolls())
 
         def _sum_roll_outcomes_by_rolls() -> Iterator[RollOutcome]:
             for source_roll in source_rolls:
                 if len(source_roll) == 1 and source_roll[0].value is not None:
                     yield from source_roll
@@ -1771,15 +1769,15 @@
 )"""
 
     @beartype
     def __eq__(self, other) -> bool:
         return super().__eq__(other) and _callable_cmp(self.predicate, other.predicate)
 
     @beartype
-    def roll(self) -> Roll:
+    def roll(self) -> "Roll":
         r""""""
         source_rolls = list(self.source_rolls())
 
         def _filtered_roll_outcomes() -> Iterator[RollOutcome]:
             for roll_outcome in chain.from_iterable(source_rolls):
                 if roll_outcome.value is not None:
                     if self.predicate(roll_outcome):
@@ -1910,15 +1908,15 @@
 )"""
 
     @beartype
     def __eq__(self, other) -> bool:
         return super().__eq__(other) and self.which == other.which
 
     @beartype
-    def roll(self) -> Roll:
+    def roll(self) -> "Roll":
         r""""""
         source_rolls = list(self.source_rolls())
         roll_outcomes = list(
             roll_outcome
             for roll_outcome in chain.from_iterable(source_rolls)
             if roll_outcome.value is not None
         )
@@ -2048,15 +2046,15 @@
             super().__eq__(other)
             and _callable_cmp(self.expansion_op, other.expansion_op)
             and self.coalesce_mode == other.coalesce_mode
             and self.max_depth == other.max_depth
         )
 
     @beartype
-    def roll(self) -> Roll:
+    def roll(self) -> "Roll":
         r""""""
         (source_roll,) = self.source_rolls()
         source_rolls: list[Roll] = []
 
         def _expanded_roll_outcomes(
             roll: Roll,
             depth: int = 0,
@@ -2223,179 +2221,179 @@
             and other.value is not None
         ):
             return bool(__ge__(self.value, other.value))
         else:
             return NotImplemented
 
     @beartype
-    def __add__(self, other: _RollOutcomeOperandT) -> RollOutcome:
+    def __add__(self, other: _RollOutcomeOperandT) -> "RollOutcome":
         try:
             return self.map(__add__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __radd__(self, other: RealLike) -> RollOutcome:
+    def __radd__(self, other: RealLike) -> "RollOutcome":
         try:
             return self.rmap(other, __add__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __sub__(self, other: _RollOutcomeOperandT) -> RollOutcome:
+    def __sub__(self, other: _RollOutcomeOperandT) -> "RollOutcome":
         try:
             return self.map(__sub__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rsub__(self, other: RealLike) -> RollOutcome:
+    def __rsub__(self, other: RealLike) -> "RollOutcome":
         try:
             return self.rmap(other, __sub__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __mul__(self, other: _RollOutcomeOperandT) -> RollOutcome:
+    def __mul__(self, other: _RollOutcomeOperandT) -> "RollOutcome":
         try:
             return self.map(__mul__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rmul__(self, other: RealLike) -> RollOutcome:
+    def __rmul__(self, other: RealLike) -> "RollOutcome":
         try:
             return self.rmap(other, __mul__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __truediv__(self, other: _RollOutcomeOperandT) -> RollOutcome:
+    def __truediv__(self, other: _RollOutcomeOperandT) -> "RollOutcome":
         try:
             return self.map(__truediv__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rtruediv__(self, other: RealLike) -> RollOutcome:
+    def __rtruediv__(self, other: RealLike) -> "RollOutcome":
         try:
             return self.rmap(other, __truediv__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __floordiv__(self, other: _RollOutcomeOperandT) -> RollOutcome:
+    def __floordiv__(self, other: _RollOutcomeOperandT) -> "RollOutcome":
         try:
             return self.map(__floordiv__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rfloordiv__(self, other: RealLike) -> RollOutcome:
+    def __rfloordiv__(self, other: RealLike) -> "RollOutcome":
         try:
             return self.rmap(other, __floordiv__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __mod__(self, other: _RollOutcomeOperandT) -> RollOutcome:
+    def __mod__(self, other: _RollOutcomeOperandT) -> "RollOutcome":
         try:
             return self.map(__mod__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rmod__(self, other: RealLike) -> RollOutcome:
+    def __rmod__(self, other: RealLike) -> "RollOutcome":
         try:
             return self.rmap(other, __mod__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __pow__(self, other: _RollOutcomeOperandT) -> RollOutcome:
+    def __pow__(self, other: _RollOutcomeOperandT) -> "RollOutcome":
         try:
             return self.map(__pow__, other)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
-    def __rpow__(self, other: RealLike) -> RollOutcome:
+    def __rpow__(self, other: RealLike) -> "RollOutcome":
         try:
             return self.rmap(other, __pow__)
         except NotImplementedError:
             return NotImplemented
 
     @beartype
     # TODO(posita): See <https://github.com/beartype/beartype/issues/152>
-    def __and__(self, other: Union["RollOutcome", SupportsInt]) -> RollOutcome:
+    def __and__(self, other: Union["RollOutcome", SupportsInt]) -> "RollOutcome":
         try:
             if isinstance(other, SupportsInt):
                 other = as_int(other)
 
             return self.map(__and__, other)
         except (NotImplementedError, TypeError):
             return NotImplemented
 
     @beartype
-    def __rand__(self, other: SupportsInt) -> RollOutcome:
+    def __rand__(self, other: SupportsInt) -> "RollOutcome":
         try:
             return self.rmap(as_int(other), __and__)
         except (NotImplementedError, TypeError):
             return NotImplemented
 
     @beartype
     # TODO(posita): See <https://github.com/beartype/beartype/issues/152>
-    def __xor__(self, other: Union["RollOutcome", SupportsInt]) -> RollOutcome:
+    def __xor__(self, other: Union["RollOutcome", SupportsInt]) -> "RollOutcome":
         try:
             if isinstance(other, SupportsInt):
                 other = as_int(other)
 
             return self.map(__xor__, other)
         except (NotImplementedError, TypeError):
             return NotImplemented
 
     @beartype
-    def __rxor__(self, other: SupportsInt) -> RollOutcome:
+    def __rxor__(self, other: SupportsInt) -> "RollOutcome":
         try:
             return self.rmap(as_int(other), __xor__)
         except (NotImplementedError, TypeError):
             return NotImplemented
 
     @beartype
     # TODO(posita): See <https://github.com/beartype/beartype/issues/152>
-    def __or__(self, other: Union["RollOutcome", SupportsInt]) -> RollOutcome:
+    def __or__(self, other: Union["RollOutcome", SupportsInt]) -> "RollOutcome":
         try:
             if isinstance(other, SupportsInt):
                 other = as_int(other)
 
             return self.map(__or__, other)
         except (NotImplementedError, TypeError):
             return NotImplemented
 
     @beartype
-    def __ror__(self, other: SupportsInt) -> RollOutcome:
+    def __ror__(self, other: SupportsInt) -> "RollOutcome":
         try:
             return self.rmap(as_int(other), __or__)
         except (NotImplementedError, TypeError):
             return NotImplemented
 
     @beartype
-    def __neg__(self) -> RollOutcome:
+    def __neg__(self) -> "RollOutcome":
         return self.umap(__neg__)
 
     @beartype
-    def __pos__(self) -> RollOutcome:
+    def __pos__(self) -> "RollOutcome":
         return self.umap(__pos__)
 
     @beartype
-    def __abs__(self) -> RollOutcome:
+    def __abs__(self) -> "RollOutcome":
         return self.umap(__abs__)
 
     @beartype
-    def __invert__(self) -> RollOutcome:
+    def __invert__(self) -> "RollOutcome":
         return self.umap(__invert__)
 
     # ---- Properties ------------------------------------------------------------------
 
     @property
     def annotation(self) -> Any:
         r"""
@@ -2413,15 +2411,15 @@
 
         See the [``source_roll``][dyce.r.RollOutcome.source_roll] and
         [``Roll.r``][dyce.r.Roll.r] properties.
         """
         return self.source_roll.r
 
     @property
-    def source_roll(self) -> Roll:
+    def source_roll(self) -> "Roll":
         r"""
         Returns the roll if one has been associated with this roll outcome. Usually that
         happens by submitting the roll outcome to the
         [``Roll.__init__`` method][dyce.r.Roll.__init__] inside a
         [``R.roll`` method][dyce.r.R.roll] implementation. Accessing this property
         before the roll outcome has been associated with a roll is considered a
         programming error.
@@ -2451,15 +2449,15 @@
         assert (
             self._roll is not None
         ), "RollOutcome.source_roll accessed before associating the roll outcome with a roll (usually via Roll.__init__)"
 
         return self._roll
 
     @property
-    def sources(self) -> tuple[RollOutcome, ...]:
+    def sources(self) -> tuple["RollOutcome", ...]:
         r"""
         The source roll outcomes from which this roll outcome was generated.
         """
         return self._sources
 
     @property
     def value(self) -> Optional[RealLike]:
@@ -2472,15 +2470,15 @@
     # ---- Methods ---------------------------------------------------------------------
 
     @beartype
     def map(
         self,
         bin_op: _BinaryOperatorT,
         right_operand: _RollOutcomeOperandT,
-    ) -> RollOutcome:
+    ) -> "RollOutcome":
         r"""
         Applies *bin_op* to the value of this roll outcome as the left operand and
         *right_operand* as the right. Shorthands exist for many arithmetic operators and
         comparators.
 
         ``` python
         >>> import operator
@@ -2509,15 +2507,15 @@
 
         if isinstance(right_operand_value, RealLike):
             return type(self)(bin_op(self.value, right_operand_value), sources)
         else:
             raise NotImplementedError
 
     @beartype
-    def rmap(self, left_operand: RealLike, bin_op: _BinaryOperatorT) -> RollOutcome:
+    def rmap(self, left_operand: RealLike, bin_op: _BinaryOperatorT) -> "RollOutcome":
         r"""
         Analogous to the [``map`` method][dyce.r.RollOutcome.map], but where the caller
         supplies *left_operand*.
 
         ``` python
         >>> import operator
         >>> two = RollOutcome(2)
@@ -2547,15 +2545,15 @@
         else:
             raise NotImplementedError
 
     @beartype
     def umap(
         self,
         un_op: _UnaryOperatorT,
-    ) -> RollOutcome:
+    ) -> "RollOutcome":
         r"""
         Applies *un_op* to the value of this roll outcome. Shorthands exist for many
         arithmetic operators and comparators.
 
         ``` python
         >>> import operator
         >>> two_neg = RollOutcome(-2)
@@ -2573,89 +2571,89 @@
         True
 
         ```
         """
         return type(self)(un_op(self.value), sources=(self,))
 
     @beartype
-    def lt(self, other: _RollOutcomeOperandT) -> RollOutcome:
+    def lt(self, other: _RollOutcomeOperandT) -> "RollOutcome":
         if isinstance(other, RollOutcome):
             return type(self)(bool(__lt__(self, other)), sources=(self, other))
         elif self.value is not None:
             return type(self)(bool(__lt__(self.value, other)), sources=(self,))
         else:
             raise ValueError(f"unable to compare {self} to {other}")
 
     @beartype
-    def le(self, other: _RollOutcomeOperandT) -> RollOutcome:
+    def le(self, other: _RollOutcomeOperandT) -> "RollOutcome":
         if isinstance(other, RollOutcome):
             return type(self)(bool(__le__(self, other)), sources=(self, other))
         elif self.value is not None:
             return type(self)(bool(__le__(self.value, other)), sources=(self,))
         else:
             raise ValueError(f"unable to compare {self} to {other}")
 
     @beartype
-    def eq(self, other: _RollOutcomeOperandT) -> RollOutcome:
+    def eq(self, other: _RollOutcomeOperandT) -> "RollOutcome":
         if isinstance(other, RollOutcome):
             return type(self)(bool(__eq__(self, other)), sources=(self, other))
         elif self.value is not None:
             return type(self)(bool(__eq__(self.value, other)), sources=(self,))
         else:
             raise ValueError(f"unable to compare {self} to {other}")
 
     @beartype
-    def ne(self, other: _RollOutcomeOperandT) -> RollOutcome:
+    def ne(self, other: _RollOutcomeOperandT) -> "RollOutcome":
         if isinstance(other, RollOutcome):
             return type(self)(bool(__ne__(self, other)), sources=(self, other))
         else:
             return type(self)(bool(__ne__(self.value, other)), sources=(self,))
 
     @beartype
-    def gt(self, other: _RollOutcomeOperandT) -> RollOutcome:
+    def gt(self, other: _RollOutcomeOperandT) -> "RollOutcome":
         if isinstance(other, RollOutcome):
             return type(self)(bool(__gt__(self, other)), sources=(self, other))
         elif self.value is not None:
             return type(self)(bool(__gt__(self.value, other)), sources=(self,))
         else:
             raise ValueError(f"unable to compare {self} to {other}")
 
     @beartype
-    def ge(self, other: _RollOutcomeOperandT) -> RollOutcome:
+    def ge(self, other: _RollOutcomeOperandT) -> "RollOutcome":
         if isinstance(other, RollOutcome):
             return type(self)(bool(__ge__(self, other)), sources=(self, other))
         elif self.value is not None:
             return type(self)(bool(__ge__(self.value, other)), sources=(self,))
         else:
             raise ValueError(f"unable to compare {self} to {other}")
 
     @beartype
-    def is_even(self) -> RollOutcome:
+    def is_even(self) -> "RollOutcome":
         r"""
         Shorthand for: ``#!python self.umap(dyce.types.is_even)``.
 
         See the [``umap`` method][dyce.r.RollOutcome.umap].
         """
         return self.umap(is_even)
 
     @beartype
-    def is_odd(self) -> RollOutcome:
+    def is_odd(self) -> "RollOutcome":
         r"""
         Shorthand for: ``#!python self.umap(dyce.types.is_even)``.
 
         See the [``umap`` method][dyce.r.RollOutcome.umap].
         """
         return self.umap(is_odd)
 
     @beartype
     def adopt(
         self,
         sources: Iterable["RollOutcome"] = (),
         coalesce_mode: CoalesceMode = CoalesceMode.REPLACE,
-    ) -> RollOutcome:
+    ) -> "RollOutcome":
         r"""
         Creates and returns a new roll outcome identical to this roll outcome, but with
         *sources* replacing or appended to this roll outcome’s sources in accordance
         with *coalesce_mode*.
 
         ``` python
         >>> from dyce.r import CoalesceMode
@@ -2705,15 +2703,15 @@
 
         adopted_roll_outcome = type(self)(self.value, adopted_sources)
         adopted_roll_outcome._roll = self._roll
 
         return adopted_roll_outcome
 
     @beartype
-    def euthanize(self) -> RollOutcome:
+    def euthanize(self) -> "RollOutcome":
         r"""
         Shorthand for ``#!python self.umap(lambda operand: None)``.
 
         ``` python
         >>> two = RollOutcome(2)
         >>> two.euthanize()
         RollOutcome(
@@ -2868,28 +2866,28 @@
     def r(self) -> R:
         r"""
         The roller that generated the roll.
         """
         return self._r
 
     @property
-    def source_rolls(self) -> tuple[Roll, ...]:
+    def source_rolls(self) -> tuple["Roll", ...]:
         r"""
         The source rolls from which this roll was generated.
         """
         return self._source_rolls
 
     # ---- Methods ---------------------------------------------------------------------
 
     @beartype
     def adopt(
         self,
         sources: Iterable["RollOutcome"] = (),
         coalesce_mode: CoalesceMode = CoalesceMode.REPLACE,
-    ) -> Roll:
+    ) -> "Roll":
         r"""
         Shorthand for ``#!python Roll(self.r, (roll_outcome.adopt(sources,
         coalesce_mode) for roll_outcome in self), self.source_rolls)``.
         """
         return type(self)(
             self.r,
             (roll_outcome.adopt(sources, coalesce_mode) for roll_outcome in self),
```

## dyce/rng.py

```diff
@@ -2,16 +2,14 @@
 # Copyright and other protections apply. Please see the accompanying LICENSE file for
 # rights and restrictions governing use of this software. All rights not expressly
 # waived or licensed are reserved. If that file is missing or appears to be modified
 # from its original, then please contact the author before viewing or using this
 # software in any capacity.
 # ======================================================================================
 
-from __future__ import annotations
-
 from abc import ABC
 from random import Random
 from sys import version_info
 from typing import Any, Type
 
 from numerary.bt import beartype
```

## dyce/types.py

```diff
@@ -2,16 +2,14 @@
 # Copyright and other protections apply. Please see the accompanying LICENSE file for
 # rights and restrictions governing use of this software. All rights not expressly
 # waived or licensed are reserved. If that file is missing or appears to be modified
 # from its original, then please contact the author before viewing or using this
 # software in any capacity.
 # ======================================================================================
 
-from __future__ import annotations
-
 import re
 from operator import __getitem__, __index__
 from typing import Any, Callable, Iterable, Iterator, Sequence, TypeVar, Union
 
 from numerary.bt import beartype
 from numerary.types import SupportsIndex, SupportsInt
```

## Comparing `dyce-0.6.1.dist-info/LICENSE` & `dyce-0.6.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dyce-0.6.1.dist-info/METADATA` & `dyce-0.6.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyce
-Version: 0.6.1
+Version: 0.6.2
 Summary: Simple Python tools for exploring dice outcomes and other finite discrete probabilities
 Home-page: https://posita.github.io/dyce/
 Author: Matt Bogosian
 Author-email: matt@bogosian.net
 License: MIT License
 Project-URL: Source Repository, https://github.com/posita/dyce/
 Classifier: Topic :: Education
@@ -52,26 +52,26 @@
 
 *Copyright and other protections apply.
 Please see the accompanying ``LICENSE`` file for rights and restrictions governing use of this software.
 All rights not expressly waived or licensed are reserved.
 If that file is missing or appears to be modified from its original, then please contact the author before viewing or using this software in any capacity.*
 
 [![Tests](https://github.com/posita/dyce/actions/workflows/on-push.yaml/badge.svg)](https://github.com/posita/dyce/actions/workflows/on-push.yaml)
-[![Version](https://img.shields.io/pypi/v/dyce/0.6.1.svg)](https://pypi.org/project/dyce/0.6.1/)
-[![Development Stage](https://img.shields.io/pypi/status/dyce/0.6.1.svg)](https://pypi.org/project/dyce/0.6.1/)
-[![License](https://img.shields.io/pypi/l/dyce/0.6.1.svg)](http://opensource.org/licenses/MIT)
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/dyce/0.6.1.svg)](https://pypi.org/project/dyce/0.6.1/)
-[![Supported Python Implementations](https://img.shields.io/pypi/implementation/dyce/0.6.1.svg)](https://pypi.org/project/dyce/0.6.1/)
+[![Version](https://img.shields.io/pypi/v/dyce/0.6.2.svg)](https://pypi.org/project/dyce/0.6.2/)
+[![Development Stage](https://img.shields.io/pypi/status/dyce/0.6.2.svg)](https://pypi.org/project/dyce/0.6.2/)
+[![License](https://img.shields.io/pypi/l/dyce/0.6.2.svg)](http://opensource.org/licenses/MIT)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/dyce/0.6.2.svg)](https://pypi.org/project/dyce/0.6.2/)
+[![Supported Python Implementations](https://img.shields.io/pypi/implementation/dyce/0.6.2.svg)](https://pypi.org/project/dyce/0.6.2/)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![``numerary``-encumbered](https://raw.githubusercontent.com/posita/numerary/latest/docs/numerary-encumbered.svg)](https://posita.github.io/numerary/)
 [![Bear-ified™](https://raw.githubusercontent.com/beartype/beartype-assets/main/badge/bear-ified.svg)](https://beartype.rtfd.io/)
 
 Now you’re playing with …
 
-<img style="float: right; padding: 0 1.0em 0 1.0em;" src="https://raw.githubusercontent.com/posita/dyce/v0.6.1/docs/dyce.svg" alt="dyce logo">
+<img style="float: right; padding: 0 1.0em 0 1.0em;" src="https://raw.githubusercontent.com/posita/dyce/v0.6.2/docs/dyce.svg" alt="dyce logo">
 
 # ``dyce`` – simple Python tools for exploring dice outcomes and other finite discrete probabilities
 
 **💥 _Now 100% [Bear-ified™](https://beartype.rtfd.io/)!_ 👌🏾🐻**
 ([Details](#requirements) below.)
 
 
@@ -178,25 +178,25 @@
 ```
 
 [``H`` objects](https://posita.github.io/dyce/0.6/dyce/#dyce.h.H) provide a [``distribution`` method](https://posita.github.io/dyce/0.6/dyce/#dyce.h.H.distribution) and a [``distribution_xy`` method](https://posita.github.io/dyce/0.6/dyce/#dyce.h.H.distribution_xy) to ease integration with plotting packages
 [``anydyce``](https://github.com/posita/anydyce/), for example, makes use of these to integrate with [``matplotlib``](https://matplotlib.org/stable/api/index.html).
 
 <!-- Should match any title of the corresponding plot title -->
 <picture>
-  <source srcset="https://raw.githubusercontent.com/posita/dyce/v0.6.1/docs/assets/plot_2d6_lo_hi_dark.png" media="(prefers-color-scheme: dark)">
-  <img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/dyce/v0.6.1/docs/assets/plot_2d6_lo_hi_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/dyce/v0.6.1/docs/assets/plot_2d6_lo_hi_dark.png#gh-dark-mode-only"></span>
+  <source srcset="https://raw.githubusercontent.com/posita/dyce/v0.6.2/docs/assets/plot_2d6_lo_hi_dark.png" media="(prefers-color-scheme: dark)">
+  <img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/dyce/v0.6.2/docs/assets/plot_2d6_lo_hi_light.png#gh-light-mode-only"><span style="display: none"><img alt="Plot: Taking the lowest or highest die of 2d6" src="https://raw.githubusercontent.com/posita/dyce/v0.6.2/docs/assets/plot_2d6_lo_hi_dark.png#gh-dark-mode-only"></span>
 </picture>
 <!-- The above is a ridiculous work-around for GitHub's braindead, proprietary
 light/dark image rendering dumpster fire. See
 [https://github.community/t/support-theme-context-for-images-in-light-vs-dark-mode/147981/87].
 -->
 
 <details>
 <summary>
-  Source: <a href="https://github.com/posita/dyce/blob/v0.6.1/docs/assets/plot_2d6_lo_hi.py"><code>plot_2d6_lo_hi.py</code></a><br>
+  Source: <a href="https://github.com/posita/dyce/blob/v0.6.2/docs/assets/plot_2d6_lo_hi.py"><code>plot_2d6_lo_hi.py</code></a><br>
   Interactive version: <a href="https://posita.github.io/dyce/0.6/jupyter/lab/?path=2d6_lo_hi.ipynb"><img src="https://jupyterlite.readthedocs.io/en/latest/_static/badge.svg" alt="Try dyce"></a>
 </summary>
 
 ``` python
 --8<-- "docs/assets/plot_2d6_lo_hi.py"
 ```
 </details>
```

