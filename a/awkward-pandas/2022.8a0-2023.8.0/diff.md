# Comparing `tmp/awkward_pandas-2022.8a0.tar.gz` & `tmp/awkward_pandas-2023.8.0.tar.gz`

## Comparing `awkward_pandas-2022.8a0.tar` & `awkward_pandas-2023.8.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 awkward_pandas-2022.8a0/src/awkward_pandas/__init__.py
--rw-r--r--   0        0        0     6871 2020-02-02 00:00:00.000000 awkward_pandas-2022.8a0/src/awkward_pandas/accessor.py
--rw-r--r--   0        0        0     5772 2020-02-02 00:00:00.000000 awkward_pandas-2022.8a0/src/awkward_pandas/array.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 awkward_pandas-2022.8a0/src/awkward_pandas/dtype.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 awkward_pandas-2022.8a0/src/awkward_pandas/io.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 awkward_pandas-2022.8a0/src/awkward_pandas/py.typed
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 awkward_pandas-2022.8a0/src/awkward_pandas/strings.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 awkward_pandas-2022.8a0/src/awkward_pandas/version.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 awkward_pandas-2022.8a0/.gitignore
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 awkward_pandas-2022.8a0/LICENSE
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 awkward_pandas-2022.8a0/README.md
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 awkward_pandas-2022.8a0/pyproject.toml
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 awkward_pandas-2022.8a0/PKG-INFO
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 awkward_pandas-2023.8.0/src/awkward_pandas/__init__.py
+-rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 awkward_pandas-2023.8.0/src/awkward_pandas/accessor.py
+-rw-r--r--   0        0        0     5219 2020-02-02 00:00:00.000000 awkward_pandas-2023.8.0/src/awkward_pandas/array.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 awkward_pandas-2023.8.0/src/awkward_pandas/dtype.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 awkward_pandas-2023.8.0/src/awkward_pandas/io.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 awkward_pandas-2023.8.0/src/awkward_pandas/lib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 awkward_pandas-2023.8.0/src/awkward_pandas/py.typed
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 awkward_pandas-2023.8.0/src/awkward_pandas/strings.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 awkward_pandas-2023.8.0/src/awkward_pandas/version.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 awkward_pandas-2023.8.0/.gitignore
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 awkward_pandas-2023.8.0/LICENSE
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 awkward_pandas-2023.8.0/README.md
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 awkward_pandas-2023.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 awkward_pandas-2023.8.0/PKG-INFO
```

### Comparing `awkward_pandas-2022.8a0/src/awkward_pandas/accessor.py` & `awkward_pandas-2023.8.0/src/awkward_pandas/accessor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import functools
 import inspect
 
-import awkward._v2 as ak
+import awkward as ak
 import pandas as pd
 
 from awkward_pandas.array import AwkwardExtensionArray
 from awkward_pandas.dtype import AwkwardDtype
 from awkward_pandas.strings import (
     all_bytes,
     all_strings,
@@ -23,15 +23,15 @@
     def __init__(self, pandas_obj):
         if not self._validate(pandas_obj):
             raise AttributeError("ak accessor called on incompatible data")
         self._obj = pandas_obj
         self._arr = None
 
     @property
-    def arr(self):
+    def extarray(self):
         if self._arr is None:
             if isinstance(self._obj, AwkwardExtensionArray):
                 self._arr = self._obj
             elif isinstance(self._obj.dtype, AwkwardDtype) and isinstance(
                 self._obj, pd.Series
             ):
                 # this is a pandas Series that contains an Awkward
@@ -40,88 +40,137 @@
                 # a dask series - figure out what to do here
                 raise NotImplementedError
             else:
                 # this recreates series, possibly by iteration
                 self._arr = AwkwardExtensionArray(self._obj)
         return self._arr
 
-    def __getitem__(self, *items):
-        ds = self.arr._data.__getitem__(*items)
-        return pd.Series(AwkwardExtensionArray(ds))
+    @property
+    def array(self):
+        """Get underlying awkward array"""
+        return self.extarray._data
+
+    def __getitem__(self, items):
+        """Extract components using awkward indexing"""
+        ds = self.array.__getitem__(items)
+        index = None
+        if items[0]:
+            if not isinstance(items[0], str) and not (
+                isinstance(items[0], list) and isinstance(items[0][0], str)
+            ):
+                index = self._obj.index[items[0]]
+        return pd.Series(AwkwardExtensionArray(ds), index=index)
 
     def to_column(self):
-        data = self.arr._data
+        """Convert awkward series to regular pandas type
+
+        Will convert to numpy or string[pyarrow] if appropriate.
+        May fail if the conversion cannot be done.
+        """
+        data = self.array
         if data.ndim > 1:
             raise ValueError
         # TODO: if all_strings(data) - accept ?str
         if data.layout.parameter("__array__") == "string":
             from pandas.core.arrays.string_arrow import ArrowStringArray
 
-            return pd.Series(
-                ArrowStringArray(
-                    ak.to_arrow(data, extensionarray=False, string_to32=True)
-                )
+            new_ak_array = ak.to_arrow(
+                data,
+                string_to32=True,
+                extensionarray=False,
             )
+            return pd.Series(ArrowStringArray(new_ak_array))
         else:
             return pd.Series(ak.to_numpy(data))
 
-    def to_columns(self, cull=True):
+    def to_columns(self, cull=True, extract_all=False, awkward_name="awkward-data"):
+        """Extract columns from an awkward series
+
+        Where the series is a record type, each field may become a regular
+        pandas column.
+
+        Parameters
+        ----------
+        cull: bool
+            For those columns that we convert into regular ones, remove them
+            from the original awkward series if True
+        extract_all: bool
+            If False (default), only extract columns that can turn into normal
+            pandas columns. If True, all columns will be extracted, but those
+            that cannot be converted retain "awkward" type
+        awkward_name: str
+            If there are leftover columns in the original series, in the
+            resultant dataframe, these leftovers will get this column name
+
+        Returns
+        -------
+        pd.DataFrame
+        """
         s = self._obj
-        fields = self.arr._data.fields
+        fields = self.array.fields
         out = {}
         for field in fields:
             try:
                 out[field] = s.ak[field].ak.to_column()
             except Exception:
-                pass
-        if cull:
-            out[s.name] = s.ak[[_ for _ in fields if _ not in out]]
+                if extract_all:
+                    out[field] = s.ak[field]
+        if cull and extract_all:
+            pass
+        elif cull:
+            n = s.name or awkward_name
+            outfields = [_ for _ in fields if _ not in out]
+            if outfields:
+                out[n] = s.ak[outfields]
         else:
             out[s.name] = s
         return pd.DataFrame(out)
 
     def encode(self, encoding="utf-8"):
-        return pd.Series(AwkwardExtensionArray(encode(self.arr._data)))
+        """bytes -> string"""
+        return pd.Series(AwkwardExtensionArray(encode(self.array)))
 
     def decode(self, encoding="utf-8"):
-        return pd.Series(AwkwardExtensionArray(decode(self.arr._data)))
+        """string -> bytes"""
+        return pd.Series(AwkwardExtensionArray(decode(self.array)))
 
     @staticmethod
     def _validate(obj):
         return isinstance(
             obj, (AwkwardExtensionArray, ak.Array, ak.Record)
         ) or isinstance(obj.values, AwkwardExtensionArray)
 
     # def to_arrow(self):
-    #    return self.arr._data.to_arrow()
+    #    return self.array.to_arrow()
 
     # def cartesian(self, other, **kwargs):
     #    if isinstance(other, AwkwardExtensionArray):
     #        other = other._data
-    #    return AwkwardExtensionArray(ak.cartesian([self.arr._data, other], **kwargs))
+    #    return AwkwardExtensionArray(ak.cartesian([self.array, other], **kwargs))
 
     def __getattr__(self, item):
+        """Call awkward namespace function on a series"""
         # replace with concrete implementations of all top-level ak functions
         if item not in dir(self):
             raise AttributeError
         func = getattr(ak, item, None)
 
-        utf8 = all_strings(self.arr._data.layout)
-        byte = all_bytes(self.arr._data.layout)
+        utf8 = all_strings(self.array.layout)
+        byte = all_bytes(self.array.layout)
         if func:
 
             @functools.wraps(func)
             def f(*others, **kwargs):
                 others = [
                     other._data
                     if isinstance(getattr(other, "_data", None), ak.Array)
                     else other
                     for other in others
                 ]
-                ak_arr = func(self.arr._data, *others, **kwargs)
+                ak_arr = func(self.array, *others, **kwargs)
                 # TODO: special case to carry over index and name information where output
                 #  is similar to input, e.g., has same length
                 if isinstance(ak_arr, ak.Array):
                     # TODO: perhaps special case here if the output can be represented
                     #  as a regular num/cupy array
                     return pd.Series(
                         AwkwardExtensionArray(ak_arr), index=self._obj.index
@@ -137,15 +186,15 @@
             def f(*args, **kwargs):
                 import pyarrow
 
                 if utf8:
                     data = pyarrow.chunked_array(
                         [
                             ak.to_arrow(
-                                self.arr._data,
+                                self.array,
                                 extensionarray=False,
                                 string_to32=True,
                                 bytestring_to32=True,
                             )
                         ]
                     )
                 else:
@@ -177,18 +226,25 @@
                 return ak_arr
 
         else:
             raise AttributeError
 
         return f
 
+    def apply(self, fn):
+        """Perform function on all the values of the series"""
+        result = fn(self.array)
+        if isinstance(result, ak.Array):
+            return pd.Series(AwkwardExtensionArray(result))
+        return result
+
     def __dir__(self):
-        if self.arr._data.layout.parameters.get("__array__") == "bytestring":
+        if self.array.layout.parameters.get("__array__") == "bytestring":
             extra = dir_str(utf8=False)
-        elif self.arr._data.layout.parameters.get("__array__") == "string":
+        elif self.array.layout.parameters.get("__array__") == "string":
             extra = dir_str(utf8=True)
         else:
             extra = []
         return (
             [
                 _
                 for _ in (dir(ak))
```

### Comparing `awkward_pandas-2022.8a0/src/awkward_pandas/array.py` & `awkward_pandas-2023.8.0/src/awkward_pandas/array.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import operator
 from collections.abc import Iterable
 from typing import TYPE_CHECKING, Any, Literal
 
-import awkward._v2 as ak
+import awkward as ak
 import numpy as np
 import pandas as pd
 from pandas.core.arrays.base import (
     ExtensionArray,
     ExtensionScalarOpsMixin,
     set_function_name,
 )
@@ -21,14 +21,24 @@
 
 
 class AwkwardExtensionArray(ExtensionArray, ExtensionScalarOpsMixin):
     _dtype: AwkwardDtype
     _data: ak.Array
 
     def __init__(self, data: Any) -> None:
+        """
+
+        Parameters
+        ----------
+        data : awkward array, dict, JSON string, iterable
+            Construct extension array from this data. If an iterable or dict,
+            pass to awkward to generate the internal array. If a JSON string,
+            parse it using awkward.
+        """
+
         self._dtype = AwkwardDtype()
         if isinstance(data, type(self)):
             self._data = data._data
         elif isinstance(data, ak.Array):
             self._data = data
         elif isinstance(data, dict):
             self._data = ak.Array(data)
@@ -131,65 +141,37 @@
         dtype = np.dtype(object) if dtype is None else np.dtype(dtype)
 
         if dtype == np.dtype("O"):
             return np.asarray(self._data.tolist(), dtype=dtype)
 
         return np.asarray(self._data, dtype=dtype)
 
-    def __arrow_array__(self):
+    def __arrow_array__(self, type=None):
         import pyarrow as pa
 
-        return pa.chunked_array(ak.to_arrow(self._data))
+        return pa.chunked_array(ak.to_arrow(self._data), type=type)
 
     def tolist(self) -> list:
         return self._data.tolist()
 
     def __array_ufunc__(self, *inputs, **kwargs):
         return type(self)(self._data.__array_ufunc__(*inputs, **kwargs))
 
     def max(self, **kwargs):
+        print("max?")
         return ak.max(self._data, **kwargs)
 
     def min(self, **kwargs):
         return ak.min(self._data, **kwargs)
 
     def mean(self, **kwargs):
         return ak.mean(self._data, **kwargs)
 
     def std(self, **kwargs):
         return ak.std(self._data, **kwargs)
 
     def sum(self, axis=None, **kwargs):
         return ak.sum(self._data, axis=axis, **kwargs)
 
-    # def __repr__(self) -> str:
-    #     return f"pandas: {self._data.__repr__()}"
-
-    # def __str__(self) -> str:
-    #     return str(self._data)
-
 
 AwkwardExtensionArray._add_arithmetic_ops()
 AwkwardExtensionArray._add_comparison_ops()
-
-# for k in ["mean", "var", "std", "sum", "prod"]:
-#     setattr(AwkwardExtensionArray, k, getattr(ak, k))
-
-
-def merge(dataframe, name=None):
-    """Create a single awkward series by merging the columns of a dataframe.
-
-    Parameters
-    ----------
-    dataframe: pd.DataFrame
-        Containing columns of simple numpy type, object type (e.g.,
-        srtings, lists or dicts) or existing awkward columns.
-    name: str or None
-        Name of the output series.
-    """
-    out = {}
-    for c in dataframe.columns:
-        if dataframe[c].dtype in ["awkward", "string[pyarrow]"]:
-            out[c] = dataframe[c].values._data
-        else:
-            out[c] = dataframe[c].values
-    return pd.Series(AwkwardExtensionArray(ak.Array(out)), name=name)
```

### Comparing `awkward_pandas-2022.8a0/src/awkward_pandas/dtype.py` & `awkward_pandas-2023.8.0/src/awkward_pandas/dtype.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
-import awkward._v2 as ak
+import awkward as ak
 import numpy as np
 from pandas.core.dtypes.base import ExtensionDtype, register_extension_dtype
 
 if TYPE_CHECKING:
     from awkward_pandas.array import AwkwardExtensionArray
```

### Comparing `awkward_pandas-2022.8a0/src/awkward_pandas/strings.py` & `awkward_pandas-2023.8.0/src/awkward_pandas/strings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-import awkward._v2 as ak
+from __future__ import annotations
+
+import awkward as ak
 
 string_methods = {}
 
 
 def _make_string_methods(utf8=True):
     try:
         import pyarrow.compute
@@ -79,63 +81,63 @@
         name = "binary_" + item
     elif item in string_methods["standard"]:
         name = item
     return getattr(pyarrow.compute, name, None)
 
 
 def _encode(layout):
-    if layout.is_RecordType:
+    if layout.is_record:
         [_encode(_) for _ in layout._contents]
-    elif layout.is_ListType and layout.parameter("__array__") == "string":
+    elif layout.is_list and layout.parameter("__array__") == "string":
         layout._parameters["__array__"] = "bytestring"
-        layout.content._parameters["__array__"] = ("byte",)
-    elif layout.is_OptionType or layout.is_ListType:
+        layout.content._parameters["__array__"] = "byte"
+    elif layout.is_option or layout.is_list:
         _encode(layout.content)
 
 
 def encode(arr, encoding="utf-8"):
     if encoding.lower() not in ["utf-8", "utf8"]:
         raise NotImplementedError
     arr2 = ak.copy(arr)
     _encode(arr2.layout)
     return ak.Array(arr2)
 
 
 def _decode(layout):
-    if layout.is_RecordType:
+    if layout.is_record:
         [_decode(_) for _ in layout._contents]
-    elif layout.is_ListType and layout.parameter("__array__") == "bytestring":
+    elif layout.is_list and layout.parameter("__array__") == "bytestring":
         layout._parameters["__array__"] = "string"
-        layout.content._parameters["__array__"] = ("char",)
-    elif layout.is_OptionType or layout.is_ListType:
+        layout.content._parameters["__array__"] = "char"
+    elif layout.is_option or layout.is_list:
         _decode(layout.content)
 
 
 def decode(arr, encoding="utf-8"):
     if encoding.lower() not in ["utf-8", "utf8"]:
         raise NotImplementedError
     arr2 = ak.copy(arr)  # to be mutated on creation
     _decode(arr2.layout)
     return ak.Array(arr2)
 
 
 def all_strings(layout):
-    if layout.is_RecordType:
+    if layout.is_record:
         return all(all_strings(layout[field]) for field in layout.fields)
-    if layout.is_ListType or layout.is_OptionType:
+    if layout.is_list or layout.is_option:
         if layout.parameter("__array__") == "string":
             return True
         return all_strings(layout.content)
     return layout.parameter("__array__") == "string"
 
 
 def all_bytes(layout):
-    if layout.is_RecordType:
+    if layout.is_record:
         return all(all_strings(layout[field]) for field in layout.fields)
-    if layout.is_ListType or layout.is_OptionType:
+    if layout.is_list or layout.is_option:
         if layout.parameter("__array__") == "bytestring":
             return True
         return all_strings(layout.content)
     return layout.parameter("__array__") == "bytestring"
 
 
 def get_split(utf8=True):
```

### Comparing `awkward_pandas-2022.8a0/.gitignore` & `awkward_pandas-2023.8.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
+docs/generated
 
 # PyBuilder
 .pybuilder/
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `awkward_pandas-2022.8a0/LICENSE` & `awkward_pandas-2023.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awkward_pandas-2022.8a0/pyproject.toml` & `awkward_pandas-2023.8.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -6,36 +6,57 @@
 name = "awkward-pandas"
 description = "Awkward Array Pandas Extension"
 readme = "README.md"
 license = "BSD-3-Clause"
 requires-python = ">=3.8"
 authors = [
     { name = "Doug Davis", email = "ddavis@ddavis.io" },
+    { name = "Martin Durant", email = "mdurant@anaconda.com" },
+]
+maintainers = [
+    { name = "Doug Davis", email = "ddavis@ddavis.io" },
+    { name = "Martin Durant", email = "mdurant@anaconda.com" },
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
-    "awkward>=1.9.0rc10",
+    "awkward>=2.0.0",
     "pandas>=1.2",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 complete = [
-    "pyarrow",
-    "pytest >=6.0",
-    "pytest-cov >=3.0.0",
+  "awkward-pandas[strings,parquet]",
+]
+parquet = [
+  "pyarrow",
+]
+strings = [
+  "pyarrow >=7.0.0",
+]
+test = [
+  "awkward-pandas[complete]",
+  "pytest >=6.0",
+  "pytest-cov >=3.0.0",
+]
+docs = [
+  "sphinx",
+  "furo",
+  "nbsphinx",
+  "ipython",
 ]
 
 [project.urls]
 Homepage = "https://github.com/intake/awkward-pandas"
 "Bug Tracker" = "https://github.com/intake/awkward-pandas/issues"
 
 [tool.hatch.version]
@@ -82,7 +103,25 @@
 module = ["awkward.*"]
 ignore_missing_imports = true
 
 [tool.pyright]
 include = ["src"]
 pythonVersion = "3.8"
 reportPrivateImportUsage = false
+
+[tool.coverage.report]
+exclude_lines = [
+    "pragma: no cover",
+    "if TYPE_CHECKING:",
+    "except ImportError:",
+    "NotImplementedError",
+    "_ipython_key_completions_",
+]
+fail_under = 75
+show_missing = true
+
+[tool.coverage.run]
+omit = ["src/awkward_pandas/version.py"]
+source = ["src/awkward_pandas"]
+
+[tool.ruff]
+ignore = ["E501"]
```

### Comparing `awkward_pandas-2022.8a0/PKG-INFO` & `awkward_pandas-2023.8.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 Metadata-Version: 2.1
 Name: awkward-pandas
-Version: 2022.8a0
+Version: 2023.8.0
 Summary: Awkward Array Pandas Extension
 Project-URL: Homepage, https://github.com/intake/awkward-pandas
 Project-URL: Bug Tracker, https://github.com/intake/awkward-pandas/issues
-Author-email: Doug Davis <ddavis@ddavis.io>
+Author-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
+Maintainer-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
+License-Expression: BSD-3-Clause
+License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
-Requires-Dist: awkward>=1.9.0rc10
+Requires-Dist: awkward>=2.0.0
 Requires-Dist: pandas>=1.2
 Provides-Extra: complete
-Requires-Dist: pyarrow; extra == 'complete'
-Requires-Dist: pytest-cov>=3.0.0; extra == 'complete'
-Requires-Dist: pytest>=6.0; extra == 'complete'
+Requires-Dist: awkward-pandas[parquet,strings]; extra == 'complete'
+Provides-Extra: docs
+Requires-Dist: furo; extra == 'docs'
+Requires-Dist: ipython; extra == 'docs'
+Requires-Dist: nbsphinx; extra == 'docs'
+Requires-Dist: sphinx; extra == 'docs'
+Provides-Extra: parquet
+Requires-Dist: pyarrow; extra == 'parquet'
+Provides-Extra: strings
+Requires-Dist: pyarrow>=7.0.0; extra == 'strings'
+Provides-Extra: test
+Requires-Dist: awkward-pandas[complete]; extra == 'test'
+Requires-Dist: pytest-cov>=3.0.0; extra == 'test'
+Requires-Dist: pytest>=6.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # awkward-pandas
 
 > Awkward Array extension for use in pandas.
 
 [![Tests](https://github.com/intake/awkward-pandas/actions/workflows/pypi.yml/badge.svg)](https://github.com/intake/awkward-pandas/actions/workflows/pypi.yml)
+[![Documentation Status](https://readthedocs.org/projects/awkward-pandas/badge/?version=latest)](https://awkward-pandas.readthedocs.io/en/latest/?badge=latest)
 
-This project is affiliated with awkward-array's v1 to v2 transition.
-[Read more about that
-here](https://github.com/scikit-hep/awkward/wiki).
+See the [quick
+start](https://awkward-pandas.readthedocs.io/en/latest/quickstart.html)
+in the documentation for an introduction to awkward-pandas.
```

