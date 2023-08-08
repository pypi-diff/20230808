# Comparing `tmp/linkml_owl-0.2.8.tar.gz` & `tmp/linkml_owl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_owl-0.2.8.tar", max compression
+gzip compressed data, was "linkml_owl-0.3.0.tar", max compression
```

## Comparing `linkml_owl-0.2.8.tar` & `linkml_owl-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      141 2023-04-04 00:54:58.089051 linkml_owl-0.2.8/README.md
--rw-r--r--   0        0        0      301 2023-04-04 00:54:58.097051 linkml_owl-0.2.8/linkml_owl/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 00:54:58.097051 linkml_owl-0.2.8/linkml_owl/crossproducts/__init__.py
--rw-r--r--   0        0        0     5407 2023-04-04 00:54:58.097051 linkml_owl-0.2.8/linkml_owl/crossproducts/cross_product_generator.py
--rw-r--r--   0        0        0        0 2023-04-04 00:54:58.097051 linkml_owl-0.2.8/linkml_owl/dumpers/__init__.py
--rw-r--r--   0        0        0    36936 2023-04-04 00:54:58.097051 linkml_owl-0.2.8/linkml_owl/dumpers/owl_dumper.py
--rw-r--r--   0        0        0        0 2023-04-04 00:54:58.097051 linkml_owl-0.2.8/linkml_owl/util/__init__.py
--rw-r--r--   0        0        0      659 2023-04-04 00:54:58.097051 linkml_owl-0.2.8/linkml_owl/util/csv_converter.py
--rw-r--r--   0        0        0     7763 2023-04-04 00:54:58.097051 linkml_owl-0.2.8/linkml_owl/util/loader_wrapper.py
--rw-r--r--   0        0        0      454 2023-04-04 00:54:58.097051 linkml_owl-0.2.8/linkml_owl/util/trim_yaml.py
--rw-r--r--   0        0        0     1401 2023-04-04 00:55:17.637385 linkml_owl-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 linkml_owl-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-08-08 17:56:59.660513 linkml_owl-0.3.0/README.md
+-rw-r--r--   0        0        0      301 2023-08-08 17:56:59.668514 linkml_owl-0.3.0/linkml_owl/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 17:56:59.668514 linkml_owl-0.3.0/linkml_owl/crossproducts/__init__.py
+-rw-r--r--   0        0        0     5407 2023-08-08 17:56:59.668514 linkml_owl-0.3.0/linkml_owl/crossproducts/cross_product_generator.py
+-rw-r--r--   0        0        0        0 2023-08-08 17:56:59.668514 linkml_owl-0.3.0/linkml_owl/dumpers/__init__.py
+-rw-r--r--   0        0        0    37629 2023-08-08 17:56:59.668514 linkml_owl-0.3.0/linkml_owl/dumpers/owl_dumper.py
+-rw-r--r--   0        0        0        0 2023-08-08 17:56:59.668514 linkml_owl-0.3.0/linkml_owl/util/__init__.py
+-rw-r--r--   0        0        0      659 2023-08-08 17:56:59.668514 linkml_owl-0.3.0/linkml_owl/util/csv_converter.py
+-rw-r--r--   0        0        0     7763 2023-08-08 17:56:59.668514 linkml_owl-0.3.0/linkml_owl/util/loader_wrapper.py
+-rw-r--r--   0        0        0      454 2023-08-08 17:56:59.668514 linkml_owl-0.3.0/linkml_owl/util/trim_yaml.py
+-rw-r--r--   0        0        0     1410 2023-08-08 17:57:18.965875 linkml_owl-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 linkml_owl-0.3.0/PKG-INFO
```

### Comparing `linkml_owl-0.2.8/linkml_owl/crossproducts/cross_product_generator.py` & `linkml_owl-0.3.0/linkml_owl/crossproducts/cross_product_generator.py`

 * *Files identical despite different names*

### Comparing `linkml_owl-0.2.8/linkml_owl/dumpers/owl_dumper.py` & `linkml_owl-0.3.0/linkml_owl/dumpers/owl_dumper.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,20 @@
                 logging.debug(f"set subj from {slot.name}={v} asURI: {subj}")
         if AnonymousIndividual.__name__ in cls_interps or (subj is None and "Individual" in cls_interps):
             subj = AnonymousIndividual()
             logging.debug(f"No identifier slot; Creating anon individual for element = {subj}")
         else:
             for obj_type in [ObjectProperty, DataProperty, AnnotationProperty, NamedIndividual, Class, Datatype]:
                 if obj_type.__name__ in cls_interps:
-                    decl = Declaration(obj_type(subj))
+                    if not subj:
+                        raise ValueError(f"Cannot create {obj_type} without an identifier for {element}")
+                    if not isinstance(subj, URIRef):
+                        raise ValueError(f"Cannot create {obj_type} with non-URI identifier for {element}")
+                    di = obj_type(subj)
+                    decl = Declaration(di)
                     logging.debug(f"Inferred {decl} based on {obj_type.__name__} in {cls_interps}")
                     o.axioms.append(decl)
         logging.info(f"Subject={subj}")
         expression_termset = {"IntersectionOf", "UnionOf", "ComplementOf", "OneOf", "SomeValuesFrom", "AllValuesFrom"}
         is_returns_expression = len(expression_termset.intersection(cls_interps)) > 0
         # iterate through all slot-value assignments for element;
         # generate axioms or add axioms to EntityAxiomIndex for each
@@ -438,15 +443,15 @@
                     elif axiom_type == ObjectPropertyDomain:
                         axiom = ObjectPropertyDomain(subj, parent)
                     elif axiom_type == ObjectPropertyRange:
                         axiom = ObjectPropertyRange(subj, parent)
                     elif axiom_type == AnnotationAssertion:
                         axiom = AnnotationAssertion(slot_uri, subj, parent)
                     else:
-                        raise Exception(f'Unknown: {axiom_type}')
+                        raise ValueError(f'Unknown axiom type: {axiom_type}')
                     if axiom is not None:
                         self.add_axiom(axiom, o, axiom_annotations)
                     else:
                         unprocessed_parents.append(parent)
         # all per-slot axioms have been processed; axioms that span
         # multiple slots are now processed
         if "IntersectionOf" in cls_interps:
@@ -554,16 +559,26 @@
                 if ann_key == 'owl':
                     vals.update([v.strip() for v in s.annotations[ann_key].value.split(',')])
                 else:
                     vals.add(s.annotations[ann_key].value)
         return list(vals)
 
     def _get_inferred_class_annotations(self, cls: ClassDefinition, ann_key: str) -> List[str]:
+        """
+        Retrieve owl annotations for a class, including those inherited from ancestors.
+
+        OWL annotations are specified in LinkML using the annotations slot, where the
+        key is "owl" or something in the owl namespace.
+
+        :param cls: class to query
+        :param ann_key: annotation key to query
+        :return:
+        """
         vals = set()
-        anc_classes = [cls]
+        anc_classes = []
         sv = self.schemaview
         for anc_c in sv.class_ancestors(cls.name, reflexive=True):
             anc_classes.append(sv.get_class(anc_c))
         for s in anc_classes:
             if ann_key in s.annotations:
                 if ann_key == 'owl':
                     vals.update([v.strip() for v in s.annotations[ann_key].value.split(',')])
```

### Comparing `linkml_owl-0.2.8/linkml_owl/util/csv_converter.py` & `linkml_owl-0.3.0/linkml_owl/util/csv_converter.py`

 * *Files identical despite different names*

### Comparing `linkml_owl-0.2.8/linkml_owl/util/loader_wrapper.py` & `linkml_owl-0.3.0/linkml_owl/util/loader_wrapper.py`

 * *Files identical despite different names*

### Comparing `linkml_owl-0.2.8/pyproject.toml` & `linkml_owl-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml_owl"
-version = "0.2.8"
+version = "0.3.0"
 description = "OWL mappings for Linked Open Data Modeling Language"
 authors = ["Chris Mungall <cjmungall@lbl.gov>"]
 
 readme = "README.md"
 
 homepage = "https://github.com/linkml/linkml-owl"
 repository = "https://github.com/linkml/linkml-owl"
@@ -33,22 +33,22 @@
 [tool.poetry.scripts]
 linkml-data2owl = "linkml_owl.dumpers.owl_dumper:cli"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 click = "*"
-funowl = "0.1.12"
-Jinja2 = "^3.0.3"
-linkml = "^1.3.0"
-linkml-runtime = "^1.3.4"
+funowl = ">=0.2.3"
+Jinja2 = ">=3.0.3"
+linkml = ">=1.3.0"
+linkml-runtime = ">=1.3.4"
 
 [tool.poetry.dev-dependencies]
-tox = "^3.24.5"
-pytest = "^6.2.5"
-pytest-cov = "^3.0.0"
-mkdocs = "^1.2.3"
-black = "^22.10.0"
+tox = ">=3.24.5"
+pytest = ">=6.2.5"
+pytest-cov = ">=3.0.0"
+mkdocs = ">=1.2.3"
+black = ">=22.10.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `linkml_owl-0.2.8/PKG-INFO` & `linkml_owl-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml-owl
-Version: 0.2.8
+Version: 0.3.0
 Summary: OWL mappings for Linked Open Data Modeling Language
 Home-page: https://github.com/linkml/linkml-owl
 Keywords: linkml,owl
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -16,21 +16,19 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Jinja2 (>=3.0.3,<4.0.0)
+Requires-Dist: Jinja2 (>=3.0.3)
 Requires-Dist: click
-Requires-Dist: funowl (==0.1.12)
-Requires-Dist: linkml (>=1.3.0,<2.0.0)
-Requires-Dist: linkml-runtime (>=1.3.4,<2.0.0)
+Requires-Dist: funowl (>=0.2.3)
+Requires-Dist: linkml (>=1.3.0)
+Requires-Dist: linkml-runtime (>=1.3.4)
 Project-URL: Documentation, https://github.com/linkml/linkml-owl
 Project-URL: Repository, https://github.com/linkml/linkml-owl
 Description-Content-Type: text/markdown
 
 # linkml-owl
 
 Translates between LinkML instance data to OWL (TBoxes and ABoxes)
```

