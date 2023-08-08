# Comparing `tmp/artigraph-0.0.5.tar.gz` & `tmp/artigraph-0.0.6.tar.gz`

## Comparing `artigraph-0.0.5.tar` & `artigraph-0.0.6.tar`

### file list

```diff
@@ -1,54 +1,66 @@
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 artigraph-0.0.5/_temp.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 artigraph-0.0.5/mkdocs.yml
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 artigraph-0.0.5/docs/index.md
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 artigraph-0.0.5/docs/serializers.md
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 artigraph-0.0.5/docs/storage.md
--rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 artigraph-0.0.5/docs/usage.md
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/__init__.py
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/db.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/py.typed
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/api/__init__.py
--rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/api/artifact.py
--rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/api/artifact_model.py
--rw-r--r--   0        0        0     7317 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/api/node.py
--rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/api/span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/orm/__init__.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/orm/artifact.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/orm/base.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/orm/node.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/orm/span.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/serializer/__init__.py
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/serializer/core.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/serializer/datetime.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/serializer/json.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/serializer/numpy.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/serializer/pandas.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/serializer/polars.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/serializer/pyarrow.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/storage/__init__.py
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/storage/aws.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/storage/core.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 artigraph-0.0.5/src/artigraph/storage/file.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/conftest.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_db.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_storage.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_api/__init__.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_api/test_artifact.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_api/test_artifact_model.py
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_api/test_node.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_api/test_span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_serializer/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_serializer/test_core.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_serializer/test_json.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_serializer/test_numpy.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_serializer/test_pandas.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_serializer/test_polars.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 artigraph-0.0.5/tests/test_serializer/test_pyarrow.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 artigraph-0.0.5/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 artigraph-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 artigraph-0.0.5/README.md
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 artigraph-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 artigraph-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 artigraph-0.0.6/Untitled.ipynb
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 artigraph-0.0.6/_temp.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 artigraph-0.0.6/mkdocs.yml
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 artigraph-0.0.6/.github/workflows/.hatch-run.yml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 artigraph-0.0.6/.github/workflows/check.yml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 artigraph-0.0.6/.github/workflows/publish-docs.yml
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 artigraph-0.0.6/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 artigraph-0.0.6/docs/index.md
+-rw-r--r--   0        0        0     8559 2020-02-02 00:00:00.000000 artigraph-0.0.6/docs/schema.md
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 artigraph-0.0.6/docs/serializers.md
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 artigraph-0.0.6/docs/storage.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 artigraph-0.0.6/docs/style.css
+-rw-r--r--   0        0        0    13407 2020-02-02 00:00:00.000000 artigraph-0.0.6/docs/usage.md
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/__init__.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/db.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/py.typed
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/api/__init__.py
+-rw-r--r--   0        0        0     8865 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/api/artifact.py
+-rw-r--r--   0        0        0    11001 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/api/node.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/model/__init__.py
+-rw-r--r--   0        0        0    10465 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/model/base.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/model/builtins.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/model/data.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/orm/__init__.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/orm/artifact.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/orm/base.py
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/orm/node.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/serializer/__init__.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/serializer/core.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/serializer/datetime.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/serializer/json.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/serializer/numpy.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/serializer/pandas.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/serializer/polars.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/serializer/pyarrow.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/storage/__init__.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/storage/aws.py
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/storage/core.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 artigraph-0.0.6/src/artigraph/storage/file.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/conftest.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_db.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_orm.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_storage.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_api/__init__.py
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_api/test_artifact.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_api/test_artifact_model.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_api/test_node.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_model/__init__.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_model/test_base.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_model/test_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_serializer/__init__.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_serializer/test_core.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_serializer/test_datetime.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_serializer/test_json.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_serializer/test_numpy.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_serializer/test_pandas.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_serializer/test_polars.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 artigraph-0.0.6/tests/test_serializer/test_pyarrow.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 artigraph-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 artigraph-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 artigraph-0.0.6/README.md
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 artigraph-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 artigraph-0.0.6/PKG-INFO
```

### Comparing `artigraph-0.0.5/_temp.py` & `artigraph-0.0.6/_temp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import asyncio
 from dataclasses import dataclass
 
 from sqlalchemy.ext.asyncio import create_async_engine
 
-from artigraph import ArtifactModel
+from artigraph import DataModel
 from artigraph.db import set_engine
 
 # configure what engine artigraph will use
 set_engine(create_async_engine("sqlite+aiosqlite:///example.db"), create_tables=True)
 
 
 # define a model of your data
 @dataclass(frozen=True)
-class MyData(ArtifactModel, version=1):
+class MyData(DataModel, version=1):
     some_value: int
     another_value: dict[str, str]
 
 
 async def main():
     # construct an artifact
     artifact = MyData(some_value=42, another_value={"foo": "bar"})
```

### Comparing `artigraph-0.0.5/docs/index.md` & `artigraph-0.0.6/docs/index.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 # Artigraph
 
 A library for describing and relating artifacts.
 
 Artigraph is built atop [SQLAlchemy](https://www.sqlalchemy.org/) and supports most
-major databases including PostgreSQL, MySQL, and SQLite. It is designed to be used
-in conjunction with existing data pipeline tools like [Prefect](https://www.prefect.io/)
-or [Dask](https://dask.org/).
+major databases including PostgreSQL, MySQL, and SQLite. It is designed to be used in
+conjunction with existing data pipeline tools like [Prefect](https://www.prefect.io/) or
+[Dask](https://dask.org/).
 
 ## Installation
 
 ```
 pip install "artigraph[all]"
 ```
 
 To install only a select set of dependencies replace `all` with any of:
 
-- `aws`
-- `pandas`
-- `numpy`
-- `polars`
-- `pyarrow`
+-   `aws`
+-   `pandas`
+-   `numpy`
+-   `polars`
+-   `pyarrow`
 
-# At a Glance
+## At a Glance
 
 Below is a script that creates an artifact in a local SQLite database and reads it back.
 
 ```python
 import asyncio
-from dataclasses import dataclass
 
-from artigraph import ArtifactModel
+from artigraph import DataModel
 from artigraph.db import set_engine
 
 # configure what engine artigraph will use
 set_engine("sqlite+aiosqlite:///example.db", create_tables=True)
 
 
 # define a model of your data
-@dataclass(frozen=True)
-class MyData(ArtifactModel, version=1):
+class MyData(DataModel, version=1):
     some_value: int
     another_value: dict[str, str]
 
 
 async def main():
     # construct an artifact
     artifact = MyData(some_value=42, another_value={"foo": "bar"})
```

### Comparing `artigraph-0.0.5/docs/serializers.md` & `artigraph-0.0.6/docs/serializers.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 Artifacts are serialized before being stored in the database. This allows you to store
 arbitrary data types in your artifacts. By default, `artigraph` will do its best to
 infer how to serialize a value based on its type. However, you can also specify a
 serializer explicitly.
 
 ## Built-in Serializers
 
--   `artigraph.serializer.json.json_serializer` - JSON
--   `artigraph.serializer.numpy.array_serializer` - 1d and 2d
-    [Numpy](https://numpy.org/) Arrays
--   `artigraph.serializer.pandas.dataframe_serializer` -
-    [Pandas](https://pandas.pydata.org/) DataFrames
--   `artigraph.serializer.polars.dataframe_serializer` -
-    [Polars](https://pola-rs.github.io/) DataFrames
--   `artigraph.serializer.pyarrow.feather_serializer` -
-    [PyArrow](https://arrow.apache.org/docs/python/index.html) Feather Files
--   `artigraph.serializer.pyarrow.parquet_serializer` -
-    [PyArrow](https://arrow.apache.org/docs/python/index.html) Parquet Files
+All built-in serializers can be found under `artigraph.serializer`:
+
+| Serializer                      | Description                                                              |
+| ------------------------------- | ------------------------------------------------------------------------ |
+| `datetime.datetime_serializer`  | Date Times                                                               |
+| `datetime.timedelta_serializer` | Time Deltas                                                              |
+| `json.json_serializer`          | JSON                                                                     |
+| `json.json_sorted_serializer`   | JSON with sorted keys                                                    |
+| `numpy.array_serializer`        | 1d and 2d [Numpy](https://numpy.org/) Arrays                             |
+| `pandas.dataframe_serializer`   | [Pandas](https://pandas.pydata.org/) DataFrames                          |
+| `polars.dataframe_serializer`   | [Polars](https://pola-rs.github.io/) DataFrames                          |
+| `pyarrow.feather_serializer`    | [PyArrow](https://arrow.apache.org/docs/python/index.html) Feather Files |
+| `pyarrow.parquet_serializer`    | [PyArrow](https://arrow.apache.org/docs/python/index.html) Parquet Files |
 
 ## Custom Serializers
 
 You can create your own serializer by subclassing `artigraph.serializer.Serializer`:
 
 ```python
 from typing import TypeVar
@@ -29,16 +31,20 @@
 from artigraph.serializer import Serializer
 
 T = TypeVar("T")
 
 
 class CustomSerializer(Serializer[T]):
 
-    name = "custom-serializer"  # this must be globally unique and stable across versions
-    types = (SomeType,)  # the types that this serializer can handle
+    def __init__(self):
+        # This must be GLOBALLY unique and stable across versions!
+        self.name = "custom-serializer"
 
     def serialize(self, value: T) -> bytes:
         """serialize the value to bytes"""
 
     def deserialize(self, value: bytes) -> T:
         """deserialize the value from bytes"""
+
+
+CustomSerializer().register()
 ```
```

### Comparing `artigraph-0.0.5/docs/storage.md` & `artigraph-0.0.6/docs/storage.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,28 +2,34 @@
 
 Artifacts can be stored in a variety of locations. By default, artifacts are stored in
 the database itself. However, you can also store artifacts in a local filesystem or in
 AWS S3.
 
 # Built-in Storage Backends
 
--   `artigraph.storage.file.FileSystem` - Local filesystem
--   `artigraph.storage.aws.S3Storage` - AWS [S3](https://aws.amazon.com/s3/)
+All built-in serializers can be found under `artigraph.storage`:
+
+| Storage                             | Description                          |
+| ----------------------------------- | ------------------------------------ |
+| `artigraph.storage.file.FileSystem` | Local filesystem                     |
+| `artigraph.storage.aws.S3Storage`   | AWS [S3](https://aws.amazon.com/s3/) |
 
 # Custom Storage Backends
 
 You can create your own storage backend by subclassing `artigraph.storage.Storage`:
 
 ```python
 from artigraph.storage import Storage
 
 
 class CustomStorage(Storage):
 
-    name = "custom-storage"  # this must be globally unique and stable across versions
+    def __init__(self):
+        # This must be GLOBALLY unique and stable across versions!
+        self.name = "custom-storage"
 
     async def create(self, data: bytes) -> str:
         """Create the artifact data and return its location."""
 
     async def read(self, location: str) -> bytes:
         """Read artifact data from the given location."""
```

### Comparing `artigraph-0.0.5/src/artigraph/db.py` & `artigraph-0.0.6/src/artigraph/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from contextlib import asynccontextmanager, contextmanager
 from contextvars import ContextVar
 from typing import Any, AsyncIterator, Callable, Iterator, TypeVar
 
 from sqlalchemy.ext.asyncio import (
     AsyncEngine,
     AsyncSession,
@@ -24,16 +26,15 @@
 @contextmanager
 def engine_context(
     engine: AsyncEngine | str,
     *,
     create_tables: bool = False,
 ) -> Iterator[AsyncEngine]:
     """Define which engine to use in the context."""
-    if isinstance(engine, str):
-        engine = create_async_engine(engine)
+    engine = create_async_engine(engine) if isinstance(engine, str) else engine
     reset = set_engine(engine, create_tables=create_tables)
     try:
         yield engine
     finally:
         reset()
 
 
@@ -65,34 +66,33 @@
         except Exception:
             await session.rollback()
             raise
 
 
 def set_engine(engine: AsyncEngine | str, *, create_tables: bool = False) -> Callable[[], None]:
     """Set the current engine and whether to try creating tables if they don't exist."""
-    if isinstance(engine, str):
-        engine = create_async_engine(engine)
+    engine = create_async_engine(engine) if isinstance(engine, str) else engine
     current_engine_token = _CURRENT_ENGINE.set(engine)
     create_tables_token = _CREATE_TABLES.set(create_tables)
 
     def reset() -> None:
         _CURRENT_ENGINE.reset(current_engine_token)
         _CREATE_TABLES.reset(create_tables_token)
 
     return reset
 
 
-async def get_engine() -> AsyncEngine:
+async def get_engine(*, create_tables: bool = False) -> AsyncEngine:
     """Get the current engine."""
     try:
         engine = _CURRENT_ENGINE.get()
     except LookupError:  # nocov
         msg = "No current asynchronous engine"
         raise LookupError(msg) from None
-    if _CREATE_TABLES.get():
+    if create_tables or _CREATE_TABLES.get():  # nocov (FIXME: actually covered but not detected)
         async with engine.begin() as conn:
             await conn.run_sync(Base.metadata.create_all)
     return engine
 
 
 def set_session(session: AsyncSession) -> Callable[[], None]:
     """Set the current session."""
```

### Comparing `artigraph-0.0.5/src/artigraph/api/artifact.py` & `artigraph-0.0.6/src/artigraph/api/artifact.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,132 @@
-import asyncio
-from typing import Any, Coroutine, Sequence, TypeVar
+from __future__ import annotations
+
+from typing import Any, Sequence, TypeVar, overload
 
 from sqlalchemy import select
 from typing_extensions import TypeAlias
 
-from artigraph.api.node import delete_nodes, is_node_type, read_children, read_descendants
-from artigraph.db import current_session
+from artigraph.api.node import (
+    delete_node,
+    is_node_type,
+    read_child_nodes,
+    read_descendant_nodes,
+    read_node,
+)
+from artigraph.db import current_session, session_context
 from artigraph.orm.artifact import BaseArtifact, DatabaseArtifact, RemoteArtifact
 from artigraph.orm.node import Node
-from artigraph.serializer import get_serialize_by_name
-from artigraph.storage.core import get_storage_by_name
+from artigraph.serializer import get_serializer_by_name
+from artigraph.serializer.core import Serializer
+from artigraph.storage.core import Storage, get_storage_by_name
+from artigraph.utils import TaskBatch
 
 T = TypeVar("T")
 N = TypeVar("N", bound=Node)
 
-QualifiedArtifact: TypeAlias = tuple[RemoteArtifact | DatabaseArtifact, Any]
+QualifiedArtifact: TypeAlias = "tuple[RemoteArtifact | DatabaseArtifact, Any]"
 """An artifact with its value."""
 
 
+@overload
+def new_artifact(
+    label: str,
+    value: Any,
+    serializer: Serializer,
+    *,
+    detail: str = ...,
+    storage: Storage,
+    parent_id: int | None = ...,
+) -> tuple[RemoteArtifact, Any]:
+    ...
+
+
+@overload
+def new_artifact(
+    label: str,
+    value: Any,
+    serializer: Serializer,
+    *,
+    detail: str = ...,
+    storage: Storage | None,
+    parent_id: int | None = ...,
+) -> tuple[DatabaseArtifact | RemoteArtifact, Any]:
+    ...
+
+
+@overload
+def new_artifact(
+    label: str,
+    value: Any,
+    serializer: Serializer,
+    *,
+    detail: str = ...,
+    storage: None = ...,
+    parent_id: int | None = ...,
+) -> tuple[DatabaseArtifact, Any]:
+    ...
+
+
+def new_artifact(
+    label: str,
+    value: Any,
+    serializer: Serializer,
+    *,
+    detail: str = "",
+    storage: Storage | None = None,
+    parent_id: int | None = None,
+) -> QualifiedArtifact:
+    """Construct a new artifact and its value"""
+    return (
+        DatabaseArtifact(
+            node_parent_id=parent_id,
+            artifact_label=label,
+            artifact_serializer=serializer.name,
+            artifact_detail=detail,
+            database_artifact_value=serializer.serialize(value),
+        )
+        if storage is None
+        else RemoteArtifact(
+            node_parent_id=parent_id,
+            artifact_label=label,
+            artifact_detail=detail,
+            artifact_serializer=serializer.name,
+            remote_artifact_storage=storage.name,
+        ),
+        value,
+    )
+
+
 def group_artifacts_by_parent_id(
     qualified_artifacts: Sequence[QualifiedArtifact],
 ) -> dict[int | None, list[QualifiedArtifact]]:
     """Group artifacts by their parent id."""
     artifacts_by_parent_id: dict[int | None, list[QualifiedArtifact]] = {}
     for artifact, value in qualified_artifacts:
         artifacts_by_parent_id.setdefault(artifact.node_parent_id, []).append((artifact, value))
     return artifacts_by_parent_id
 
 
-async def create_artifact(artifact: RemoteArtifact | DatabaseArtifact, value: Any) -> int:
+async def write_artifact(artifact: RemoteArtifact | DatabaseArtifact, value: Any) -> int:
     """Save the artifact to the database."""
-    result = await create_artifacts([(artifact, value)])
+    result = await write_artifacts([(artifact, value)])
     return result[0]
 
 
 async def read_artifact_by_id(artifact_id: int) -> QualifiedArtifact:
     """Load the artifact from the database."""
     cmd = select(Node.node_type).where(Node.node_id == artifact_id)
     async with current_session() as session:
         result = await session.execute(cmd)
         artifact_type = _get_artifact_type_by_name(result.scalar_one())
         cmd = select(artifact_type).where(artifact_type.node_id == artifact_id)
         result = await session.execute(cmd)
         artifact = result.scalar_one()
 
-    serializer = get_serialize_by_name(artifact.artifact_serializer)
+    serializer = get_serializer_by_name(artifact.artifact_serializer)
     if isinstance(artifact, RemoteArtifact):
         storage = get_storage_by_name(artifact.remote_artifact_storage)
         value = serializer.deserialize(await storage.read(artifact.remote_artifact_location))
     elif isinstance(artifact, DatabaseArtifact):
         value = (
             None
             if artifact.database_artifact_value is None
@@ -57,80 +135,80 @@
     else:  # nocov
         msg = f"Unknown artifact type: {artifact}"
         raise RuntimeError(msg)
 
     return artifact, value
 
 
-async def create_artifacts(qualified_artifacts: Sequence[QualifiedArtifact]) -> Sequence[int]:
+async def write_artifacts(qualified_artifacts: Sequence[QualifiedArtifact]) -> Sequence[int]:
     """Save the artifacts to the database."""
     qualified_storage_artifacts: list[tuple[RemoteArtifact, Any]] = []
     database_artifacts: list[DatabaseArtifact] = []
 
     for artifact, value in qualified_artifacts:
         if isinstance(artifact, RemoteArtifact):
             qualified_storage_artifacts.append((artifact, value))
         else:
-            serializer = get_serialize_by_name(artifact.artifact_serializer)
+            serializer = get_serializer_by_name(artifact.artifact_serializer)
             artifact.database_artifact_value = serializer.serialize(value)
             database_artifacts.append(artifact)
 
     # Save values to storage first
     remote_artifacts: list[RemoteArtifact] = []
-    storage_create_coros: list[Coroutine[None, None, str]] = []
+    storage_locations: TaskBatch[str] = TaskBatch()
     for artifact, value in qualified_storage_artifacts:
         storage = get_storage_by_name(artifact.remote_artifact_storage)
-        serializer = get_serialize_by_name(artifact.artifact_serializer)
+        serializer = get_serializer_by_name(artifact.artifact_serializer)
         remote_artifacts.append(artifact)
-        storage_create_coros.append(storage.create(serializer.serialize(value)))
-
-    storage_locations = await asyncio.gather(*storage_create_coros)
+        storage_locations.add(storage.create, serializer.serialize(value))
 
-    for artifact, location in zip(remote_artifacts, storage_locations):
+    for artifact, location in zip(remote_artifacts, await storage_locations.gather()):
         artifact.remote_artifact_location = location
 
     # Save records in the database
-    async with current_session() as session:
+    async with session_context() as session:
         session.add_all(database_artifacts + remote_artifacts)
         await session.commit()
 
         # We can't do this in asyncio.gather() because of issues with concurrent connections:
         # https://docs.sqlalchemy.org/en/20/errors.html#illegalstatechangeerror-and-concurrency-exceptions
         artifact_ids: list[int] = []
         for a, _ in qualified_artifacts:
-            await session.refresh(a, ["node_id"])
+            await session.refresh(a)
             artifact_ids.append(a.node_id)
 
         return artifact_ids
 
 
-async def delete_artifacts(artifacts: Sequence[BaseArtifact]) -> None:
+async def delete_artifact(artifact_id: int, *, descendants: bool = True) -> None:
     """Delete the artifacts from the database."""
+    artifact = await read_node(artifact_id)
+
     remote_artifacts: list[RemoteArtifact] = []
-    for artifact in artifacts:
-        if isinstance(artifact, RemoteArtifact):
-            remote_artifacts.append(artifact)
+    if isinstance(artifact, RemoteArtifact):
+        remote_artifacts.append(artifact)
+    if descendants:  # nocov (FIXME: actually covered but not detected)
+        remote_artifacts.extend(await read_descendant_nodes(artifact_id, RemoteArtifact))
 
-    # Delete values from storage first
-    storage_delete_coros: list[Coroutine[None, None, None]] = []
-    for artifact in remote_artifacts:
-        storage = get_storage_by_name(artifact.remote_artifact_storage)
-        storage_delete_coros.append(storage.delete(artifact.remote_artifact_location))
+    remote_storage_deletions = TaskBatch()
+    for ra in remote_artifacts:
+        storage = get_storage_by_name(ra.remote_artifact_storage)
+        remote_storage_deletions.add(storage.delete, ra.remote_artifact_location)
+    await remote_storage_deletions.gather()
 
-    await asyncio.gather(*storage_delete_coros)
-    await delete_nodes([a.node_id for a in artifacts])
+    await delete_node(artifact_id, descendants=descendants)
 
 
 async def read_child_artifacts(root_node_id: int) -> Sequence[QualifiedArtifact]:
-    return await _read_qualified_artifacts(await read_children(root_node_id))
+    return await _read_qualified_artifacts(await read_child_nodes(root_node_id))
 
 
 async def read_descendant_artifacts(root_node_id: int) -> Sequence[QualifiedArtifact]:
     """Load the artifacts from the database."""
-    return await _read_qualified_artifacts(await read_descendants(root_node_id))
+    return await _read_qualified_artifacts(await read_descendant_nodes(root_node_id))
 
 
 async def _read_qualified_artifacts(all_artifacts: Sequence[Any]) -> Sequence[QualifiedArtifact]:
     remote_artifacts: list[RemoteArtifact] = []
     database_artifacts: list[DatabaseArtifact] = []
     for a in all_artifacts:
         if is_node_type(a, RemoteArtifact):
@@ -144,28 +222,26 @@
     qualified_artifacts: list[QualifiedArtifact] = []
 
     for d_artifact in database_artifacts:
         raw_value = d_artifact.database_artifact_value
         value = (
             None
             if raw_value is None
-            else get_serialize_by_name(d_artifact.artifact_serializer).deserialize(raw_value)
+            else get_serializer_by_name(d_artifact.artifact_serializer).deserialize(raw_value)
         )
         qualified_artifacts.append((d_artifact, value))
 
     # Load values from storage
-    storage_read_coros: list[Coroutine[None, None, Any]] = []
+    storage_data: TaskBatch[Any] = TaskBatch()
     for r_artifact in remote_artifacts:
         storage = get_storage_by_name(r_artifact.remote_artifact_storage)
-        storage_read_coros.append(storage.read(r_artifact.remote_artifact_location))
-
-    storage_data = await asyncio.gather(*storage_read_coros)
+        storage_data.add(storage.read, r_artifact.remote_artifact_location)
 
-    for r_artifact, data in zip(remote_artifacts, storage_data):
-        serializer = get_serialize_by_name(r_artifact.artifact_serializer)
+    for r_artifact, data in zip(remote_artifacts, await storage_data.gather()):
+        serializer = get_serializer_by_name(r_artifact.artifact_serializer)
         qualified_artifacts.append((r_artifact, serializer.deserialize(data)))
 
     return qualified_artifacts
 
 
 def _get_artifact_type_by_name(name: str) -> type[BaseArtifact]:
     """Get the artifact type by name."""
```

### Comparing `artigraph-0.0.5/src/artigraph/api/node.py` & `artigraph-0.0.6/src/artigraph/api/node.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,130 +1,234 @@
+from __future__ import annotations
+
 from collections.abc import Collection
+from contextlib import asynccontextmanager
+from contextvars import ContextVar
 from dataclasses import fields
-from typing import Any, Literal, Sequence, TypeGuard, TypeVar, overload
+from functools import wraps
+from typing import (
+    Any,
+    AsyncIterator,
+    Callable,
+    Iterable,
+    Literal,
+    Protocol,
+    Sequence,
+    TypeVar,
+    overload,
+)
 
-from sqlalchemy import Row, delete, join, select
+from sqlalchemy import Row, case, delete, join, select, update
 from sqlalchemy.orm import aliased
+from typing_extensions import ParamSpec, TypeGuard
 
-from artigraph.db import current_session
-from artigraph.orm.node import Node
+from artigraph.db import current_session, session_context
+from artigraph.orm.node import NODE_TYPE_BY_POLYMORPHIC_IDENTITY, Node
 
-T = TypeVar("T")
+P = ParamSpec("P")
+R_co = TypeVar("R_co", covariant=True)
 N = TypeVar("N", bound=Node)
 
+_CURRENT_NODE_ID: ContextVar[int | None] = ContextVar("CURRENT_NODE_ID", default=None)
+
+
+@overload
+def current_node_id(*, allow_none: Literal[True]) -> int | None:
+    ...
+
+
+@overload
+def current_node_id(*, allow_none: Literal[False] = ...) -> int:
+    ...
+
+
+def current_node_id(*, allow_none: bool = False) -> int | None:
+    """Get the current span ID."""
+    span_id = _CURRENT_NODE_ID.get()
+    if span_id is None and not allow_none:
+        msg = "No span is currently active."
+        raise RuntimeError(msg)
+    return span_id
+
+
+def with_current_node_id(func: _NodeFunc[P, R_co]) -> _CurrentNodeFunc[P, R_co]:
+    @wraps(func)
+    async def wrapper(node_id: int | Literal["current"], *args: P.args, **kwargs: P.kwargs) -> R_co:
+        return await func(
+            current_node_id() if node_id == "current" else node_id,
+            *args,
+            **kwargs,
+        )
+
+    return wrapper
+
+
+@asynccontextmanager
+async def create_current(
+    node_type: Callable[P, N],
+    *args: P.args,
+    **kwargs: P.kwargs,
+) -> AsyncIterator[N]:
+    """Create a new node and set it as the current node."""
+    kwargs.setdefault("node_parent_id", current_node_id(allow_none=True))
+    node = node_type(*args, **kwargs)
+    async with session_context(expire_on_commit=False) as session:
+        session.add(node)
+        await session.commit()
+        await session.refresh(node)
+    last_span_token = _CURRENT_NODE_ID.set(node.node_id)
+    try:
+        yield node
+    finally:
+        _CURRENT_NODE_ID.reset(last_span_token)
+
 
 def group_nodes_by_parent_id(nodes: Sequence[N]) -> dict[int | None, list[N]]:
     """Group nodes by their parent ID."""
     grouped_nodes: dict[int | None, list[N]] = {}
     for node in nodes:
         grouped_nodes.setdefault(node.node_parent_id, []).append(node)
     return grouped_nodes
 
 
 def is_node_type(node: Node, node_type: type[N]) -> TypeGuard[N]:
     """Check if a node is of a given type."""
     return node.node_type == node_type.polymorphic_identity
 
 
+async def read_node_exists(node_id: int) -> bool:
+    """Check if a node exists."""
+    return bool(await read_node(node_id, allow_none=True))
+
+
+async def read_nodes_exist(node_ids: Sequence[int]) -> bool:
+    """Check if nodes exist."""
+    return all(await read_nodes(node_ids, allow_none=True))
+
+
 @overload
-async def read_node(
-    node_id: int,
-    node_type: type[N] = Node,
-    *,
-    allow_none: Literal[True],
-) -> N | None:
+async def read_node(node_id: int, *, allow_none: bool) -> Node | None:
     ...
 
 
 @overload
-async def read_node(
-    node_id: int,
-    node_type: type[N] = Node,
-    *,
-    allow_none: Literal[False] = ...,
-) -> N:
+async def read_node(node_id: int, *, allow_none: Literal[False] = ...) -> Node:
     ...
 
 
-async def read_node(
-    node_id: int, node_type: type[N] = Node, *, allow_none: bool = False
-) -> N | None:
+async def read_node(node_id: int, *, allow_none: bool = False) -> Node | None:
     """Read a node by its ID."""
-    cmd = select(node_type).where(node_type.node_id == node_id)
-    async with current_session() as session:
-        result = await session.execute(cmd)
-        return result.scalar_one_or_none() if allow_none else result.scalar_one()
+    return (await read_nodes([node_id], allow_none=allow_none))[0]
 
 
-async def node_exists(node_id: int, node_type: type[Node] = Node) -> bool:
-    """Check if a node exists."""
-    cmd = select(node_type.node_id).where(node_type.node_id == node_id)
+@overload
+async def read_nodes(node_ids: Sequence[int], *, allow_none: bool) -> Sequence[Node | None]:
+    ...
+
+
+@overload
+async def read_nodes(
+    node_ids: Sequence[int], *, allow_none: Literal[False] = ...
+) -> Sequence[Node]:
+    ...
+
+
+async def read_nodes(node_ids: Sequence[int], *, allow_none: bool = False) -> Sequence[Node | None]:
+    """Read nodes by their IDs."""
+    cmd = select(Node.__table__).where(Node.node_id.in_(node_ids))
     async with current_session() as session:
         result = await session.execute(cmd)
-        return bool(result.one_or_none())
-
+        nodes_by_id = {n.node_id: n for n in load_nodes_from_rows(result.all())}
 
-async def delete_nodes(node_ids: Sequence[int]) -> None:
-    """Delete nodes."""
+    if not allow_none and len(nodes_by_id) != len(node_ids):
+        missing = set(node_ids) - set(nodes_by_id)
+        msg = f"Could not find node IDs: {list(missing)}"
+        raise ValueError(msg)
+
+    return [nodes_by_id.get(node_id) for node_id in node_ids]  # type: ignore
+
+
+async def delete_node(node_id: int, *, descendants: bool = True) -> None:
+    """Delete a node and optionally their descendants."""
+    nodes_ids = [node_id]
+    if descendants:  # nocov (FIXME: actually covered but not detected)
+        nodes_ids.extend(n.node_id for n in await read_descendant_nodes(node_id))
+    cmd = delete(Node).where(Node.node_id.in_(nodes_ids))
     async with current_session() as session:
-        cmd = delete(Node).where(Node.node_id.in_(node_ids))
         await session.execute(cmd)
         await session.commit()
 
 
-async def create_nodes(
-    nodes: Collection[Node], refresh_attributes: Sequence[str]
-) -> Collection[Node]:
+async def write_node(node: Node, *, refresh_attributes: Sequence[str] = ()) -> Node:
+    """Create a node."""
+    return (await write_nodes([node], refresh_attributes=refresh_attributes))[0]
+
+
+async def write_nodes(
+    nodes: Collection[Node], *, refresh_attributes: Sequence[str]
+) -> Sequence[Node]:
     """Create nodes and, if given, refresh their attributes."""
-    async with current_session() as session:
+    async with current_session() as session:  # nocov (FIXME: actually covered but not detected)
         session.add_all(nodes)
         await session.commit()
         if refresh_attributes:
             # We can't do this in asyncio.gather() because of issues with concurrent connections:
             # https://docs.sqlalchemy.org/en/20/errors.html#illegalstatechangeerror-and-concurrency-exceptions
             for n in nodes:
                 await session.refresh(n, refresh_attributes)
-    return nodes
+    return tuple(nodes)
 
 
-async def create_parent_child_relationships(
-    parent_child_pairs: Sequence[tuple[Node | None, Node]]
+async def write_parent_child_relationships(
+    parent_child_id_pairs: Iterable[tuple[int | None, int]]
 ) -> None:
-    """Create parent-to-child links between nodes."""
+    """Create parent-to-child links between nodes.
+
+    Updates the existing child node's node_parent_id.
+    """
+
+    # Build the CASE statement for the update query
+    parent_id_conditions = [
+        (Node.node_id == child_id, parent_id) for parent_id, child_id in parent_child_id_pairs
+    ]
+
+    # Build the update query
+    cmd = (
+        update(Node)
+        .where(Node.node_id.in_([child_id for _, child_id in parent_child_id_pairs]))
+        .values(node_parent_id=case(*parent_id_conditions))
+    )
+
     async with current_session() as session:
-        for parent, child in parent_child_pairs:
-            child.node_parent_id = None if parent is None else parent.node_id
-            session.add(child)
+        await session.execute(cmd)
         await session.commit()
 
 
-async def read_children(node_id: int, *node_types: type[N]) -> Sequence[N]:
+async def read_child_nodes(node_id: int, *node_types: type[N]) -> Sequence[N]:
     """Read the direct children of a node."""
-    cmd = select(Node).where(Node.node_parent_id == node_id)
+    cmd = select(Node.__table__).where(Node.node_parent_id == node_id)
     if node_types:
         cmd = cmd.where(Node.node_type.in_([n.polymorphic_identity for n in node_types]))
     async with current_session() as session:
         result = await session.execute(cmd)
-        children = result.scalars().all()
-    # we know we've filtered appropriately, so we can ignore the type check
-    return children  # type: ignore
+        return load_nodes_from_rows(result.all())
 
 
-async def read_parent(node_id: int, node_type: type[N] = Node) -> N | None:
+async def read_parent_node(node_id: int, node_type: type[N] = Node) -> N | None:
     """Read the direct parent of a node."""
     async with current_session() as session:
         node_cmd = select(node_type).where(node_type.node_id == node_id)
         result = await session.execute(node_cmd)
         node = result.scalar_one()
         parent_cmd = select(node_type).where(node_type.node_id == node.node_parent_id)
         result = await session.execute(parent_cmd)
         return result.scalar_one_or_none()
 
 
-async def read_descendants(node_id: int, *node_types: type[N]) -> Sequence[N]:
+async def read_descendant_nodes(node_id: int, *node_types: type[N]) -> Sequence[N]:
     """Read all descendants of this node."""
 
     # Create a CTE to get the descendants recursively
     node_cte = (
         select(Node.node_id.label("descendant_id"), Node.node_parent_id)
         .where(Node.node_id == node_id)
         .cte(name="descendants", recursive=True)
@@ -153,15 +257,15 @@
     async with current_session() as session:
         result = await session.execute(descendants_cmd)
         descendants = result.all()
 
     return load_nodes_from_rows(descendants)
 
 
-async def read_ancestors(node_id: int, *node_types: type[N]) -> Sequence[N]:
+async def read_ancestor_nodes(node_id: int, *node_types: type[N]) -> Sequence[N]:
     """Read all ancestors of this node."""
 
     # Create a CTE to get the ancestors recursively
     node_cte = (
         select(Node.node_id.label("ancestor_id"), Node.node_parent_id)
         .where(Node.node_id == node_id)
         .cte(name="ancestors", recursive=True)
@@ -178,15 +282,15 @@
     # Join the CTE with the actual Node table to get the ancestors
     ancestors_cmd = (
         select(Node.__table__)
         .select_from(join(Node, node_cte, Node.node_id == node_cte.c.ancestor_id))
         .where(node_cte.c.ancestor_id != node_id)  # Exclude the root node itself
     )
 
-    if node_types:
+    if node_types:  # nocov (FIXME: actually covered but not detected)
         ancestors_cmd = ancestors_cmd.where(
             Node.node_type.in_([n.polymorphic_identity for n in node_types])
         )
 
     async with current_session() as session:
         result = await session.execute(ancestors_cmd)
         ancestors = result.all()
@@ -194,19 +298,41 @@
     return load_nodes_from_rows(ancestors)
 
 
 def load_nodes_from_rows(rows: Sequence[Row[Any]]) -> Sequence[Any]:
     """Load the appropriate Node instances given a sequence of SQLAlchemy rows."""
     nodes: list[Any] = []
     for r in rows:
-        node_type = Node.polymorphic_identity_mapping[r.node_type]
+        node_type = NODE_TYPE_BY_POLYMORPHIC_IDENTITY[r.node_type]
         kwargs: dict[str, Any] = {}
         attrs: dict[str, Any] = {}
         for f in fields(node_type):
             if f.init:
                 kwargs[f.name] = getattr(r, f.name)
             else:
                 attrs[f.name] = getattr(r, f.name)
         node_obj = node_type(**kwargs)
         node_obj.__dict__.update(attrs)
         nodes.append(node_obj)
     return nodes
+
+
+class _NodeFunc(Protocol[P, R_co]):
+    async def __call__(
+        self,
+        node_id: int,
+        /,
+        *args: P.args,
+        **kwargs: P.kwargs,
+    ) -> R_co:
+        ...
+
+
+class _CurrentNodeFunc(Protocol[P, R_co]):
+    async def __call__(
+        self,
+        node_id: int | Literal["current"],
+        /,
+        *args: P.args,
+        **kwargs: P.kwargs,
+    ) -> R_co:
+        ...
```

### Comparing `artigraph-0.0.5/src/artigraph/orm/artifact.py` & `artigraph-0.0.6/src/artigraph/orm/artifact.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-from typing import Any, ClassVar
+from __future__ import annotations
+
+from typing import Any, ClassVar, Optional
 
 from sqlalchemy import UniqueConstraint
 from sqlalchemy.orm import Mapped, mapped_column
 
 from artigraph.orm.node import Node
 
 
 class BaseArtifact(Node):
     """A base class for artifacts."""
 
     __table_args__ = (UniqueConstraint("node_parent_id", "artifact_label"),)
     __mapper_args__: ClassVar[dict[str, Any]] = {"polymorphic_abstract": True}
 
-    artifact_label: Mapped[str] = mapped_column(use_existing_column=True, nullable=True)
-    """A label for the artifact."""
-
     artifact_serializer: Mapped[str] = mapped_column(nullable=True)
     """The name of the serializer used to serialize the artifact."""
 
+    artifact_detail: Mapped[str] = mapped_column(nullable=True)
+    """Extra information about the artifact"""
+
+    artifact_label: Mapped[str] = mapped_column(nullable=True)
+    """A label for the node."""
+
 
 class RemoteArtifact(BaseArtifact):
     """An artifact saved via a storage backend."""
 
     polymorphic_identity = "remote_artifact"
     __mapper_args__: ClassVar[dict[str, Any]] = {"polymorphic_identity": polymorphic_identity}
 
@@ -34,9 +39,9 @@
 
 class DatabaseArtifact(BaseArtifact):
     """An artifact saved directly in the database."""
 
     polymorphic_identity = "database_artifact"
     __mapper_args__: ClassVar[dict[str, Any]] = {"polymorphic_identity": polymorphic_identity}
 
-    database_artifact_value: Mapped[bytes | None] = mapped_column(default=None)
+    database_artifact_value: Mapped[Optional[bytes]] = mapped_column(default=None)
     """The data of the artifact."""
```

### Comparing `artigraph-0.0.5/src/artigraph/serializer/datetime.py` & `artigraph-0.0.6/src/artigraph/serializer/datetime.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from datetime import datetime, timedelta
 
 from artigraph.serializer import Serializer
 
 
 class DatetimeSerializer(Serializer):
     """Serializer for datetime.datetime."""
@@ -30,11 +32,12 @@
 
     def deserialize(self, value: bytes) -> timedelta:
         """Deserialize a string to a datetime.timedelta."""
         return timedelta(seconds=float(value.decode()))
 
 
 datetime_serializer = DatetimeSerializer().register()
-"""A serializer for datetime.datetime."""
+"""An iso8601 serializer for datetime objects."""
+
 
 timedelta_serializer = TimeDeltaSerializer().register()
 """A serializer for datetime.timedelta."""
```

### Comparing `artigraph-0.0.5/src/artigraph/serializer/json.py` & `artigraph-0.0.6/src/artigraph/serializer/json.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,30 @@
+from __future__ import annotations
+
 import json
 from typing import Any
 
 from artigraph.serializer import Serializer
 
 
 class JsonSerializer(Serializer[Any]):
     """A serializer for JSON."""
 
     types = (object,)
-    name = "artigraph-json"
+
+    def __init__(self, *, sort_keys: bool = False) -> None:
+        self.name = f"artigraph-json-{'sorted' if sort_keys else 'unsorted'}"
 
     def serialize(self, value: Any) -> bytes:
         """Serialize a value."""
-        return json.dumps(value).encode("utf-8")
+        return json.dumps(value, separators=(",", ":"), allow_nan=False).encode("utf-8")
 
     def deserialize(self, value: bytes) -> Any:
         """Deserialize a value."""
         return json.loads(value.decode("utf-8"))
 
 
 json_serializer = JsonSerializer().register()
 """A serializer for JSON."""
+
+json_sorted_serializer = JsonSerializer(sort_keys=True).register()
+"""A serializer for JSON with sorted keys"""
```

### Comparing `artigraph-0.0.5/src/artigraph/serializer/numpy.py` & `artigraph-0.0.6/src/artigraph/serializer/numpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 import pandas as pd
 
 from artigraph.serializer.core import Serializer
 from artigraph.serializer.pandas import dataframe_serializer
 
 NP_1D_SHAPE_LEN = 1
```

### Comparing `artigraph-0.0.5/src/artigraph/serializer/polars.py` & `artigraph-0.0.6/src/artigraph/serializer/polars.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import polars as pl
 
 from artigraph.serializer.core import Serializer
 from artigraph.serializer.pyarrow import ArrowSerializer, parquet_serializer
 
 
 class DataFrameSerializer(Serializer[pl.DataFrame]):
```

### Comparing `artigraph-0.0.5/src/artigraph/serializer/pyarrow.py` & `artigraph-0.0.6/src/artigraph/serializer/pyarrow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from io import BytesIO
 from typing import Literal
 
 import pyarrow as pa
 from pyarrow import feather, parquet
 
 from artigraph.serializer.core import Serializer
```

### Comparing `artigraph-0.0.5/src/artigraph/storage/aws.py` & `artigraph-0.0.6/src/artigraph/storage/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """S3 storage backend for Artigraph."""
+from __future__ import annotations
 
 import hashlib
 from contextlib import contextmanager
 from contextvars import ContextVar
 from typing import Callable, Iterator, TypeVar, cast
 
 from botocore.client import BaseClient
```

### Comparing `artigraph-0.0.5/src/artigraph/storage/core.py` & `artigraph-0.0.6/src/artigraph/storage/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+from __future__ import annotations
+
 import logging
 from abc import ABC, abstractmethod
 from typing import TypeVar
 
 from typing_extensions import Self
 
-B = TypeVar("B", bound=str | bytes)
+B = TypeVar("B", bound="str | bytes")
 S = TypeVar("S", bound="Storage")
 
 WRAPPER_VERSION = 1
-STORAGE_BY_NAME: dict[str, "Storage"] = {}
+STORAGE_BY_NAME: dict[str, Storage] = {}
 
 logger = logging.getLogger(__name__)
 
 
-def get_storage_by_name(name: str) -> "Storage":
+def get_storage_by_name(name: str) -> Storage:
     if name not in STORAGE_BY_NAME:  # nocov
         msg = f"No storage named {name!r} exists."
         raise ValueError(msg)
     return STORAGE_BY_NAME[name]
 
 
 class Storage(ABC):
```

### Comparing `artigraph-0.0.5/src/artigraph/storage/file.py` & `artigraph-0.0.6/src/artigraph/storage/file.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import atexit
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from uuid import uuid4
 
 from artigraph.storage import Storage
 from artigraph.utils import slugify
```

### Comparing `artigraph-0.0.5/tests/test_db.py` & `artigraph-0.0.6/tests/test_db.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+import asyncio
+
 import pytest
 from sqlalchemy import select
 
-from artigraph.db import current_session
+from artigraph.db import current_session, get_engine
 from artigraph.orm.node import Node
 
 
 async def test_current_session_auto_rollback():
     with pytest.raises(RuntimeError):
         async with current_session() as session:
-            node = Node(None)
+            node = Node(node_parent_id=None)
             session.add(node)
             await session.flush()
             result = await session.execute(select(Node))
             result.scalar_one()
             msg = "This should trigger a rollback"
             raise RuntimeError(msg)
 
     async with current_session() as session:
         result = await session.execute(select(Node))
         assert result.scalar_one_or_none() is None
+
+
+def test_get_engine_create_tables():
+    asyncio.run(get_engine(create_tables=True))
```

### Comparing `artigraph-0.0.5/tests/test_storage.py` & `artigraph-0.0.6/tests/test_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from contextlib import ExitStack, contextmanager
 from typing import ContextManager
 
 import pytest
 from boto3 import client
 
 from artigraph.storage import Storage
```

### Comparing `artigraph-0.0.5/tests/test_api/test_artifact_model.py` & `artigraph-0.0.6/tests/test_model/test_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,87 +1,81 @@
-from dataclasses import dataclass, field
-from typing import Any
+from __future__ import annotations
 
-from artigraph.api.artifact_model import (
-    ArtifactMapping,
-    ArtifactModel,
-    ArtifactSequence,
-    artifact_field,
-)
-from artigraph.serializer.json import json_serializer
+from dataclasses import fields
+from typing import Annotated, Any
+
+import pandas as pd
+
+from artigraph.api.node import create_current
+from artigraph.model.base import read_child_models, read_model, write_child_models, write_model
+from artigraph.model.data import DataModel
+from artigraph.orm import Node
+from artigraph.serializer.pandas import dataframe_serializer
 from artigraph.storage.file import temp_file_storage
 
+FileDataFrame = Annotated[pd.DataFrame, dataframe_serializer, temp_file_storage]
 
-@dataclass(frozen=True)
-class SimpleArtifactModel(ArtifactModel, version=1):
+
+class SampleModel(DataModel, version=1):
     """A simple artifact model that stores a few basic artifact."""
 
     some_value: str
-    remote_value: Any = artifact_field(serializer=json_serializer, storage=temp_file_storage)
-    inner_model: "None | SimpleArtifactModel" = None
+    remote_value: FileDataFrame
+    inner_model: None | SampleModel = None
+
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, SampleModel):
+            return False
+        for f in fields(self):
+            value = getattr(self, f.name)
+            if isinstance(value, pd.DataFrame):
+                if not value.equals(getattr(other, f.name)):
+                    return False
+            elif value != getattr(other, f.name):
+                return False
+        return True
 
 
 async def test_save_load_simple_artifact_model():
     """Test saving and loading a simple artifact model."""
-    artifact = SimpleArtifactModel(some_value="test-value", remote_value={"some": "data"})
-    artifact_id = await artifact.create(None)
-    loaded_artifact = await SimpleArtifactModel.read(artifact_id)
+    artifact = SampleModel(some_value="test-value", remote_value=pd.DataFrame())
+    artifact_id = await write_model("some-label", artifact)
+    loaded_artifact = await read_model(artifact_id)
     assert loaded_artifact == artifact
 
 
-async def test_save_load_simple_artifact_model_with_inner_model():
+async def test_read_write_simple_artifact_model_with_inner_model():
     """Test saving and loading a simple artifact model with an inner model."""
-    inner_inner_artifact = SimpleArtifactModel(
+    inner_inner_artifact = SampleModel(
         some_value="inner-inner-value",
-        remote_value={"inner-inner": "data"},
+        remote_value=pd.DataFrame(),
     )
-    inner_artifact = SimpleArtifactModel(
+    inner_artifact = SampleModel(
         some_value="inner-value",
-        remote_value={"inner": "data"},
+        remote_value=pd.DataFrame(),
         inner_model=inner_inner_artifact,
     )
-    artifact = SimpleArtifactModel(
+    artifact = SampleModel(
         some_value="test-value",
-        remote_value={"some": "data"},
+        remote_value=pd.DataFrame(),
         inner_model=inner_artifact,
     )
 
-    artifact_id = await artifact.create(None)
-    loaded_artifact = await SimpleArtifactModel.read(artifact_id)
+    artifact_id = await write_model("some-label", artifact)
+    loaded_artifact = await read_model(artifact_id)
     assert loaded_artifact == artifact
 
 
-@dataclass(frozen=True)
-class ComplexArtifactModel(ArtifactModel, version=1):
-    """A complex artifact model that stores a few basic artifact."""
-
-    simple: SimpleArtifactModel
-    mapping: ArtifactMapping["ComplexArtifactModel"] = field(default_factory=dict)
-    sequence: ArtifactSequence["ComplexArtifactModel"] = field(default_factory=dict)
-
-
-async def test_save_load_complex_artifact_model():
-    """Test saving and loading a complex artifact model."""
-    simple = SimpleArtifactModel(some_value="test-value", remote_value={"some": "data"})
-    artifact = ComplexArtifactModel(
-        simple=simple,
-        mapping=ArtifactMapping(
-            key1=ComplexArtifactModel(
-                simple=simple,
-                mapping=ArtifactMapping(key1=ComplexArtifactModel(simple=simple)),
-            ),
-            key2=ComplexArtifactModel(simple=simple),
-        ),
-        sequence=ArtifactSequence(
-            [
-                ComplexArtifactModel(simple=simple),
-                ComplexArtifactModel(
-                    simple=simple,
-                    mapping=ArtifactMapping(key3=ComplexArtifactModel(simple=simple)),
-                ),
-            ]
-        ),
-    )
-
-    artifact_id = await artifact.create(None)
-    loaded_artifact = await ComplexArtifactModel.read(artifact_id)
-    assert loaded_artifact == artifact
+async def test_read_write_child_artifact_models():
+    """Test saving and loading a simple artifact model with child models."""
+    async with create_current(Node):
+        models = {
+            "label": SampleModel(some_value="test-value", remote_value=pd.DataFrame()),
+            "other_label": SampleModel(some_value="other-value", remote_value=pd.DataFrame()),
+            "another_label": SampleModel(some_value="another-value", remote_value=pd.DataFrame()),
+        }
+        await write_child_models("current", models=models)
+        assert await read_child_models("current", labels=["label", "other_label"]) == {
+            "label": models["label"],
+            "other_label": models["other_label"],
+        }
+        assert await read_child_models("current", labels=["does_not_exist"]) == {}
```

### Comparing `artigraph-0.0.5/tests/test_api/test_node.py` & `artigraph-0.0.6/tests/test_api/test_node.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,21 @@
+from __future__ import annotations
+
+import pytest
+
 from artigraph.api.node import (
-    create_parent_child_relationships,
+    current_node_id,
     group_nodes_by_parent_id,
-    read_children,
-    read_descendants,
+    read_ancestor_nodes,
+    read_child_nodes,
+    read_descendant_nodes,
     read_node,
+    read_nodes,
+    read_parent_node,
+    write_parent_child_relationships,
 )
 from artigraph.db import current_session, session_context
 from artigraph.orm.node import Node
 
 
 class ThingOne(Node):
     polymorphic_identity = "thing_one"
@@ -15,77 +23,135 @@
 
 
 class ThingTwo(Node):
     polymorphic_identity = "thing_two"
     __mapper_args__ = {"polymorphic_identity": polymorphic_identity}  # noqa: RUF012
 
 
+def test_current_node_id_no_allow_none():
+    """Test that the current node ID is not None."""
+    with pytest.raises(RuntimeError):
+        current_node_id()
+
+
 async def test_read_direct_children():
     """Test reading the direct children of a node."""
     graph = await create_graph()
     root = graph.get_root()
-    children = await read_children(root.node_id)
+    children = await read_child_nodes(root.node_id)
     assert {n.node_id for n in children} == {n.node_id for n in graph.get_children(root.node_id)}
 
 
 async def test_read_direct_children_with_node_types():
     """Test reading the direct children of a node with node types."""
     graph = await create_graph()
     root = graph.get_root()
-    children = await read_children(root.node_id, ThingOne)
+    children = await read_child_nodes(root.node_id, ThingOne)
     expected_ids = {n.node_id for n in graph.get_children(root.node_id) if isinstance(n, ThingOne)}
     assert {n.node_id for n in children} == expected_ids
 
 
 async def test_read_recursive_children():
     """Test reading the recursive children of a node."""
     graph = await create_graph()
     root = graph.get_root()
-    children = await read_descendants(root.node_id)
+    children = await read_descendant_nodes(root.node_id)
     expected_descendant_ids = {n.node_id for n in graph.get_all_nodes()} - {root.node_id}
     assert {n.node_id for n in children} == expected_descendant_ids
 
 
 async def test_read_recursive_children_with_node_type():
     """Test reading the recursive children of a node with node types."""
     graph = await create_graph()
     root = graph.get_root()
-    children = await read_descendants(root.node_id, ThingOne)
+    children = await read_descendant_nodes(root.node_id, ThingOne)
     all_span_ids = {n.node_id for n in graph.get_all_nodes() if isinstance(n, ThingOne)}
     expected_descendant_ids = all_span_ids - {root.node_id}
     assert {n.node_id for n in children} == expected_descendant_ids
 
 
 async def test_create_parent_child_relationships():
     """Test creating parent-to-child relationships between nodes."""
     async with session_context(expire_on_commit=False):
         grandparent = await create_node()
         parent = await create_node(grandparent)
         child = await create_node(parent)
-        await create_parent_child_relationships([(grandparent, parent), (parent, child)])
+        grandchild = await create_node(child)
+        await write_parent_child_relationships(
+            [
+                (grandparent.node_id, parent.node_id),
+                (parent.node_id, child.node_id),
+                (child.node_id, grandchild.node_id),
+            ]
+        )
 
         db_parent = await read_node(parent.node_id)
         db_child = await read_node(child.node_id)
+        db_grandchild = await read_node(grandchild.node_id)
 
         assert db_parent.node_parent_id == grandparent.node_id
         assert db_child.node_parent_id == parent.node_id
+        assert db_grandchild.node_parent_id == child.node_id
+
+        assert {n.node_id for n in await read_descendant_nodes(grandparent.node_id)} == {
+            parent.node_id,
+            child.node_id,
+            grandchild.node_id,
+        }
+
+
+async def test_read_nodes_no_allow_none():
+    async with session_context(expire_on_commit=False):
+        node_exists_id = await create_node()
+
+        with pytest.raises(ValueError):
+            await read_nodes([node_exists_id.node_id, 123], allow_none=False)
+
+
+async def test_read_ancestor_nodes():
+    """Test reading the ancestor nodes of a node."""
+    async with session_context(expire_on_commit=False):
+        grandparent = await create_node()
+        parent = await create_node(grandparent)
+        child = await create_node(parent)
+        grandchild = await create_node(child)
+        await write_parent_child_relationships(
+            [
+                (grandparent.node_id, parent.node_id),
+                (parent.node_id, child.node_id),
+                (child.node_id, grandchild.node_id),
+            ]
+        )
+
+        assert {n.node_id for n in await read_ancestor_nodes(grandchild.node_id)} == {
+            grandparent.node_id,
+            parent.node_id,
+            child.node_id,
+        }
+
+
+async def test_read_parent_node():
+    async with session_context(expire_on_commit=False):
+        parent = await create_node()
+        child = await create_node(parent)
+    assert (await read_parent_node(child.node_id)).node_id == parent.node_id
 
 
 async def create_node(parent=None):
     node = Node(node_parent_id=parent.node_id if parent else None)
 
     async with current_session() as session:
         session.add(node)
         await session.commit()
         await session.refresh(node)
 
     return node
 
 
-async def create_graph() -> "Graph":
+async def create_graph() -> Graph:
     """Create a simple tree of nodes.
 
     The tree looks like this:
 
     ThingOne
     ├── ThingOne
     │   ├── ThingTwo
@@ -113,15 +179,15 @@
     """Simple graph for testing purposes."""
 
     def __init__(self, parent: Node | None):
         self.parent = parent
         self.children: list[Graph] = []
 
     def add_child(self, node_type: type[Node]):
-        node = node_type(None)
+        node = node_type(node_parent_id=None)
         graph = Graph(node)
         self.children.append(graph)
         return graph
 
     def get_root(self) -> Node:
         return self.parent if self.parent is not None else self.children[0].get_root()
```

### Comparing `artigraph-0.0.5/tests/test_serializer/test_numpy.py` & `artigraph-0.0.6/tests/test_serializer/test_numpy.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.5/tests/test_serializer/test_pyarrow.py` & `artigraph-0.0.6/tests/test_serializer/test_pyarrow.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.5/.gitignore` & `artigraph-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.5/LICENSE.txt` & `artigraph-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.5/pyproject.toml` & `artigraph-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 # --- Hatch ----------------------------------------------------------------------------------------
 
 [tool.hatch.version]
 path = "src/artigraph/__init__.py"
 
 [tool.hatch.envs.default]
+features = ["all"]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest>=7",
   "pytest-asyncio",
   "black>=23.1.0",
   "pyright>=1",
   "ruff>=0.0.243",
@@ -55,19 +56,23 @@
   "mkdocs-material>=9,<10",
 ]
 
 [tool.hatch.envs.default.scripts]
 cov = ["cov-test", "cov-report"]
 cov-report = ["- coverage combine", "coverage report"]
 cov-test = "coverage run -m pytest {args:tests}"
+docs-build = "mkdocs build"
+docs-serve = "mkdocs serve"
 format = ["black {args:.}", "ruff --fix {args:.}", "style"]
 lint = ["lint-style", "lint-typing"]
 lint-style = ["ruff {args:.}", "black --check --diff {args:.}"]
 lint-typing = "pyright {args:src}"
 test = "pytest {args:tests}"
+publish-docs = "mkdocs gh-deploy --force"
+publish-pypi = "hatch build && hatch publish"
 
 # --- Pytest ---------------------------------------------------------------------------------------
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 # --- Black ----------------------------------------------------------------------------------------
@@ -106,14 +111,16 @@
   "T",
   "TID",
   "UP",
   "W",
   "YTT",
 ]
 ignore = [
+  # SQLAlchemy in Python 3.9 does not support the newest typing syntax
+  "UP007",
   # Ignore function call in class definition (see: https://github.com/astral-sh/ruff/issues/4171)
   "RUF009",
   # Allow non-abstract empty methods in abstract base classes
   "B027",
   # Allow boolean positional values in function calls, like `dict.get(... True)`
   "FBT003",
   # Ignore checks for possible passwords
@@ -124,16 +131,18 @@
   "C901",
   "PLR0911",
   "PLR0912",
   "PLR0913",
   "PLR0915",
 ]
 unfixable = [
-  # Don't touch unused imports
-  "F401",
+  # Don't touch unused expressions
+  "F841",
+  # Leave unused loop variables
+  "B007",
 ]
 
 [tool.ruff.isort]
 known-first-party = ["artigraph"]
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
@@ -141,14 +150,15 @@
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 # --- Coverage -------------------------------------------------------------------------------------
 
 [tool.coverage.run]
+concurrency = ["greenlet", "thread"]
 source_pkgs = ["artigraph"]
 branch = true
 parallel = true
 
 [tool.coverage.paths]
 artigraph = ["src/artigraph"]
 
@@ -158,14 +168,15 @@
 skip_covered = true
 sort = "Name"
 exclude_lines = [
   "no ?cov",
   '\.\.\.',
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
+  'raise NotImplementedError\(\)',
 ]
 
 
 # --- PyRight -----------------------------------------------------------------------------------------
 
 [tool.pyright]
 include = ["src", "tests"]
```

### Comparing `artigraph-0.0.5/PKG-INFO` & `artigraph-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artigraph
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for interrelated graphs of artifacts.
 Project-URL: Documentation, https://github.com/rmorshea/artigraph#readme
 Project-URL: Issues, https://github.com/rmorshea/artigraph/issues
 Project-URL: Source, https://github.com/rmorshea/artigraph
 Author-email: "U.N. Owen" <void@some.where>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -43,8 +43,8 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/artigraph.svg)](https://pypi.org/project/artigraph)
 
 A library for creating interrelated graphs of artifacts.
 
 # Documentation
 
 Documentation is available at
-[ryanmorshead.com/artigraph/](https://ryanmorshead.com/artigraph/).
+[ryanmorshead.com/artigraph](https://ryanmorshead.com/artigraph/).
```

