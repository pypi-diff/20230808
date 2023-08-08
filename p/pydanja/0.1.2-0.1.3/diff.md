# Comparing `tmp/pydanja-0.1.2.tar.gz` & `tmp/pydanja-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydanja-0.1.2.tar", last modified: Sun Aug  6 10:58:53 2023, max compression
+gzip compressed data, was "pydanja-0.1.3.tar", last modified: Tue Aug  8 14:04:28 2023, max compression
```

## Comparing `pydanja-0.1.2.tar` & `pydanja-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2684 2023-08-06 10:16:20.525826 pydanja-0.1.2/README.md
--rw-r--r--   0        0        0     1100 2023-08-06 10:58:53.324333 pydanja-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5488 2023-08-06 05:42:49.879483 pydanja-0.1.2/src/pydanja/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 04:57:14.398442 pydanja-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     3708 1970-01-01 00:00:00.000000 pydanja-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4151 2023-08-08 13:14:29.532782 pydanja-0.1.3/README.md
+-rw-r--r--   0        0        0     1100 2023-08-08 14:04:28.665922 pydanja-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5488 2023-08-06 05:42:49.879483 pydanja-0.1.3/src/pydanja/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 04:57:14.398442 pydanja-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     5175 1970-01-01 00:00:00.000000 pydanja-0.1.3/PKG-INFO
```

### Comparing `pydanja-0.1.2/pyproject.toml` & `pydanja-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydanja"
-version = "0.1.2"
+version = "0.1.3"
 description = "JSON:API Support for Pydantic"
 authors = [
     { name = "Chris Read", email = "centurix@gmail.com" },
 ]
 dependencies = [
     "pydantic>=2.1.1",
 ]
```

### Comparing `pydanja-0.1.2/src/pydanja/__init__.py` & `pydanja-0.1.3/src/pydanja/__init__.py`

 * *Files identical despite different names*

### Comparing `pydanja-0.1.2/PKG-INFO` & `pydanja-0.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: pydanja
-Version: 0.1.2
-Summary: JSON:API Support for Pydantic
-Keywords: pydantic jsonapi json:api openapi fastapi
-Home-page: https://github.com/Centurix/pydanja
-Author-Email: Chris Read <centurix@gmail.com>
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: File Formats :: JSON
-Classifier: Topic :: File Formats :: JSON :: JSON Schema
-Classifier: Topic :: Software Development :: Documentation
-Classifier: Topic :: Software Development :: Libraries
-Project-URL: Homepage, https://github.com/Centurix/pydanja
-Project-URL: Repository, https://github.com/Centurix/pydanja
-Requires-Python: >=3.8
-Requires-Dist: pydantic>=2.1.1
-Description-Content-Type: text/markdown
-
 # PyDANJA
 
 [JSON:API](https://jsonapi.org/format/) Suport for [Pydantic](https://docs.pydantic.dev/latest/)
 
 This is a series of classes that can be included into your [Pydantic](https://docs.pydantic.dev/latest/) project that act as a container format for outputting and verifying [JSON:API](https://jsonapi.org/format/) compliant content.
 
 This library makes use of BaseModel generics to contain either a single resource or a list of resources as further BaseModels.
@@ -38,14 +12,16 @@
 
 ## Requirements
 
 This will support the oldest non-EOL Python (3.8 as of the writing of this document)
 
 ## Usage
 
+With pydantic
+
 ```
 from pydanja import DANJAResource
 
 
 class TestType(BaseModel):
     # A simple Pydantic BaseModel
     testtype_id: Optional[int] = Field(alias="id", default=None)
@@ -92,14 +68,62 @@
   "meta": null,
   "included": null
 }
 ```
 
 Note that all [JSON:API](https://jsonapi.org/format/) fields are included in the output of the model dump. If you are using an API framework like [FastAPI](https://fastapi.tiangolo.com/), you use the `response_model_exclude_none` to suppress fields with no values.
 
+### FastAPI example
+
+```
+from typing import Optional, Union
+from pydantic import BaseModel, Field
+from fastapi import FastAPI
+from pydanja import DANJAResource, DANJAResourceList, DANJAError
+
+
+app = FastAPI()
+
+
+# Example BaseModel
+class TestType(BaseModel):
+    # If we use ID, then we must alias it to avoid clashes with Python
+    testtype_id: Optional[int] = Field(alias="id", default=None)
+    name: str
+    description: str
+
+    class Config:
+        # Declare the resource ID field name
+        resource_id: str = "testtype_id"
+
+
+@app.post("/", response_model_exclude_none=True)
+async def test_func(payload: DANJAResource[TestType]) -> Union[DANJAResource[TestType], DANJAError]:
+    """
+    payload will be verified correctly for inbound JSON:API content
+    The Union includes a reference to the JSON:API error object that this could throw
+    """
+    res = TestType(
+        id=1,
+        name="Stuff!",
+        description="This is description!"
+    )
+    return DANJAResource.from_basemodel(res)
+
+@app.get("/", response_model_exclude_none=True)
+async def test_get() -> Union[DANJAResourceList[TestType], DANJAError]:
+    values = [
+        TestType(id=1, name="One", description="Desc One"),
+        TestType(id=2, name="Two", description="Desc Two"),
+        TestType(id=3, name="Three", description="Desc Three"),
+        TestType(id=4, name="Four", description="Desc Four"),
+    ]
+    return DANJAResourceList.from_basemodel(values)
+```
+
 This library supports:
 
 * Single resources (`DANJAResource`)
 * Lists of resources (`DANJAResourceList`)
 * Error objects (`DANJAErrorList`/`DANJAError`)
 * Link objects (`DANJALink`)
```

