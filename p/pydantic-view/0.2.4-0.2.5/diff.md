# Comparing `tmp/pydantic_view-0.2.4.tar.gz` & `tmp/pydantic_view-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_view-0.2.4.tar", max compression
+gzip compressed data, was "pydantic_view-0.2.5.tar", max compression
```

## Comparing `pydantic_view-0.2.4.tar` & `pydantic_view-0.2.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-04-22 16:35:00.949673 pydantic_view-0.2.4/LICENSE
--rw-r--r--   0        0        0     5704 2023-05-07 10:28:55.636831 pydantic_view-0.2.4/README.md
--rw-r--r--   0        0        0      183 2023-08-03 13:00:41.628542 pydantic_view-0.2.4/pydantic_view/__init__.py
--rw-r--r--   0        0        0     9259 2023-08-06 14:58:24.557644 pydantic_view-0.2.4/pydantic_view/pydantic_view.py
--rw-r--r--   0        0        0      876 2023-08-06 14:58:24.558011 pydantic_view-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     6638 1970-01-01 00:00:00.000000 pydantic_view-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-22 16:35:00.949673 pydantic_view-0.2.5/LICENSE
+-rw-r--r--   0        0        0     5704 2023-05-07 10:28:55.636831 pydantic_view-0.2.5/README.md
+-rw-r--r--   0        0        0      183 2023-08-03 13:00:41.628542 pydantic_view-0.2.5/pydantic_view/__init__.py
+-rw-r--r--   0        0        0     9273 2023-08-07 21:09:16.791719 pydantic_view-0.2.5/pydantic_view/pydantic_view.py
+-rw-r--r--   0        0        0      876 2023-08-07 21:24:04.397023 pydantic_view-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     6638 1970-01-01 00:00:00.000000 pydantic_view-0.2.5/PKG-INFO
```

### Comparing `pydantic_view-0.2.4/LICENSE` & `pydantic_view-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_view-0.2.4/README.md` & `pydantic_view-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_view-0.2.4/pydantic_view/pydantic_view.py` & `pydantic_view-0.2.5/pydantic_view/pydantic_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                 if issubclass(item, BaseModel):
                     item = item.__class__
                 if item not in metaclass_bases:
                     metaclass_bases.append(item)
 
             class Metaclass(*metaclass_bases):
                 def __subclasscheck__(self, subclass):
-                    if getattr(subclass, "__view_name__", None) == name:
+                    if getattr(subclass, "__view_name__", None) == self.__view_name__:
                         return cls.__subclasscheck__(subclass.__view_root_cls__)
                     return super().__subclasscheck__(subclass)
 
             __cls_kwargs__ = {"metaclass": Metaclass}
 
         else:
             __cls_kwargs__ = {}
```

### Comparing `pydantic_view-0.2.4/pyproject.toml` & `pydantic_view-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-view"
-version = "0.2.4"
+version = "0.2.5"
 description = "View decorator to create the child pydantic models from the root model."
 authors = ["Roman Koshel <roma.koshel@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pydantic", "model", "view", "utils"]
 packages = [{include = "pydantic_view"}]
 classifiers = [
```

### Comparing `pydantic_view-0.2.4/PKG-INFO` & `pydantic_view-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-view
-Version: 0.2.4
+Version: 0.2.5
 Summary: View decorator to create the child pydantic models from the root model.
 License: MIT
 Keywords: pydantic,model,view,utils
 Author: Roman Koshel
 Author-email: roma.koshel@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

