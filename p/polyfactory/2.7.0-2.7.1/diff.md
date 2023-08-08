# Comparing `tmp/polyfactory-2.7.0.tar.gz` & `tmp/polyfactory-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.7.0.tar", max compression
+gzip compressed data, was "polyfactory-2.7.1.tar", max compression
```

## Comparing `polyfactory-2.7.0.tar` & `polyfactory-2.7.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1092 2023-07-28 17:24:54.344977 polyfactory-2.7.0/LICENSE
--rw-r--r--   0        0        0    24136 2023-07-28 17:24:54.344977 polyfactory-2.7.0/docs/PYPI_README.md
--rw-r--r--   0        0        0      425 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/__init__.py
--rw-r--r--   0        0        0     2525 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/collection_extender.py
--rw-r--r--   0        0        0      912 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/constants.py
--rw-r--r--   0        0        0     1037 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/decorators.py
--rw-r--r--   0        0        0      591 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0     2147 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/attrs_factory.py
--rw-r--r--   0        0        0    33713 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2758 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1912 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     2751 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/msgspec_factory.py
--rw-r--r--   0        0        0     2192 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0    14595 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1699 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     8697 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3317 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/fields.py
--rw-r--r--   0        0        0     1192 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/py.typed
--rw-r--r--   0        0        0     2850 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     3909 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3764 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     1948 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1885 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1125 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13429 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0      433 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/constrained_path.py
--rw-r--r--   0        0        0     3846 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0      440 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/constrained_url.py
--rw-r--r--   0        0        0      446 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/constrained_uuid.py
--rw-r--r--   0        0        0     3635 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6172 2023-07-28 17:24:54.348977 polyfactory-2.7.0/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     6875 2023-07-28 17:24:54.348977 polyfactory-2.7.0/pyproject.toml
--rw-r--r--   0        0        0    26133 1970-01-01 00:00:00.000000 polyfactory-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-08-08 17:05:45.637106 polyfactory-2.7.1/LICENSE
+-rw-r--r--   0        0        0    24136 2023-08-08 17:05:45.637106 polyfactory-2.7.1/docs/PYPI_README.md
+-rw-r--r--   0        0        0      425 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/__init__.py
+-rw-r--r--   0        0        0     2525 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/collection_extender.py
+-rw-r--r--   0        0        0      912 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/constants.py
+-rw-r--r--   0        0        0     1037 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/decorators.py
+-rw-r--r--   0        0        0      591 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0     2147 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/factories/attrs_factory.py
+-rw-r--r--   0        0        0    33755 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2758 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1912 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     2751 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/factories/msgspec_factory.py
+-rw-r--r--   0        0        0     2192 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0    15948 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1699 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     8697 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3317 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/fields.py
+-rw-r--r--   0        0        0     1192 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/py.typed
+-rw-r--r--   0        0        0     2850 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     3885 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3758 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     1948 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1885 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1125 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13429 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0      433 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/value_generators/constrained_path.py
+-rw-r--r--   0        0        0     3846 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0      440 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/value_generators/constrained_url.py
+-rw-r--r--   0        0        0      446 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/value_generators/constrained_uuid.py
+-rw-r--r--   0        0        0     3678 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6172 2023-08-08 17:05:45.641106 polyfactory-2.7.1/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6907 2023-08-08 17:05:45.641106 polyfactory-2.7.1/pyproject.toml
+-rw-r--r--   0        0        0    26133 1970-01-01 00:00:00.000000 polyfactory-2.7.1/PKG-INFO
```

### Comparing `polyfactory-2.7.0/LICENSE` & `polyfactory-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/docs/PYPI_README.md` & `polyfactory-2.7.1/docs/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/collection_extender.py` & `polyfactory-2.7.1/polyfactory/collection_extender.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/constants.py` & `polyfactory-2.7.1/polyfactory/constants.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/decorators.py` & `polyfactory-2.7.1/polyfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/exceptions.py` & `polyfactory-2.7.1/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/factories/attrs_factory.py` & `polyfactory-2.7.1/polyfactory/factories/attrs_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/factories/base.py` & `polyfactory-2.7.1/polyfactory/factories/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     IPv6Network,
     ip_address,
     ip_interface,
     ip_network,
 )
 from os.path import realpath
 from pathlib import Path
+from random import Random
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
     Collection,
     Generic,
@@ -52,15 +53,15 @@
 )
 from polyfactory.fields import Fixture, Ignore, PostGenerated, Require, Use
 from polyfactory.utils.helpers import unwrap_annotation, unwrap_args, unwrap_optional
 from polyfactory.utils.predicates import (
     get_type_origin,
     is_any,
     is_literal,
-    is_optional_union,
+    is_optional,
     is_safe_subclass,
     is_union,
 )
 from polyfactory.value_generators.complex_types import handle_collection_type
 from polyfactory.value_generators.constrained_collections import handle_constrained_collection
 from polyfactory.value_generators.constrained_dates import handle_constrained_date
 from polyfactory.value_generators.constrained_numbers import (
@@ -75,16 +76,14 @@
 from polyfactory.value_generators.primitives import (
     create_random_boolean,
     create_random_bytes,
     create_random_string,
 )
 
 if TYPE_CHECKING:
-    from random import Random
-
     from typing_extensions import TypeGuard
 
     from polyfactory.field_meta import Constraints, FieldMeta
     from polyfactory.persistence import AsyncPersistenceProtocol, SyncPersistenceProtocol
 
 
 def _create_pydantic_type_map(cls: type[BaseFactory[Any]]) -> dict[type, Callable[[], Any]]:
@@ -251,15 +250,16 @@
                     raise ConfigurationException(
                         f"Model type {model.__name__} is not supported. "
                         "To support it, register an appropriate base factory and subclass it for your factory."
                     )
         else:
             BaseFactory._base_factories.append(cls)
 
-        if random_seed := getattr(cls, "__random_seed__", None) is not None:
+        random_seed = getattr(cls, "__random_seed__", None)
+        if random_seed is not None:
             cls.seed_random(random_seed)
 
         if cls.__set_as_default_factory_for_type__:
             BaseFactory._factory_type_mapping[cls.__model__] = cls
 
     @classmethod
     def _get_sync_persistence(cls) -> SyncPersistenceProtocol[T]:
@@ -397,16 +397,19 @@
     def seed_random(cls, seed: int) -> None:
         """Seed faker and random with the given integer.
 
         :param seed: An integer to set as seed.
         :returns: 'None'
 
         """
-        cls.__random__.seed(seed, version=3)
-        cls.__faker__.seed_instance(seed)
+        cls.__random__ = Random(seed)
+
+        faker = Faker()
+        faker.seed_instance(seed)
+        cls.__faker__ = faker
 
     @classmethod
     def is_ignored_type(cls, value: Any) -> bool:
         """Check whether a given value is an ignored type.
 
         :param value: An arbitrary value.
 
@@ -671,15 +674,15 @@
             - This method is distinct to allow overriding.
 
         :returns: A boolean determining whether 'None' should be set for the given field_meta.
 
         """
         return (
             cls.__allow_none_optionals__
-            and is_optional_union(field_meta.annotation)
+            and is_optional(field_meta.annotation)
             and create_random_boolean(random=cls.__random__)
         )
 
     @classmethod
     def should_set_field_value(cls, field_meta: FieldMeta, **kwargs: Any) -> bool:
         """Determine whether to set a value for a given field_name.
```

### Comparing `polyfactory-2.7.0/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.7.1/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.7.1/polyfactory/factories/dataclass_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/factories/msgspec_factory.py` & `polyfactory-2.7.1/polyfactory/factories/msgspec_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.7.1/polyfactory/factories/odmantic_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/factories/pydantic_factory.py` & `polyfactory-2.7.1/polyfactory/factories/pydantic_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,40 +22,61 @@
     MIN_COLLECTION_LENGTH,
     RANDOMIZE_COLLECTION_LENGTH,
 )
 from polyfactory.exceptions import MissingDependencyException
 from polyfactory.factories.base import BaseFactory
 from polyfactory.field_meta import Constraints, FieldMeta, Null
 from polyfactory.utils.helpers import unwrap_new_type, unwrap_optional
-from polyfactory.utils.predicates import is_optional_union, is_safe_subclass, is_union
+from polyfactory.utils.predicates import is_optional, is_safe_subclass, is_union
 
 try:
-    from pydantic import VERSION, BaseModel
+    from pydantic import VERSION, BaseModel, Json
     from pydantic.fields import FieldInfo
+    from pydantic_core import to_json
 except ImportError as e:
     raise MissingDependencyException("pydantic is not installed") from e
 
 try:
     from pydantic.fields import ModelField  # type: ignore[attr-defined]
 
 except ImportError:
     ModelField = Any
     from pydantic_core import PydanticUndefined as Undefined
 
 if TYPE_CHECKING:
     from random import Random
 
-    from typing_extensions import TypeGuard
+    from typing_extensions import NotRequired, TypeGuard
 
 T = TypeVar("T", bound=BaseModel)
 
 
+class PydanticConstraints(Constraints):
+    """Metadata regarding a Pydantic type constraints, if any"""
+
+    json: NotRequired[bool]
+
+
 class PydanticFieldMeta(FieldMeta):
     """Field meta subclass capable of handling pydantic ModelFields"""
 
+    def __init__(
+        self,
+        *,
+        name: str,
+        annotation: type,
+        random: Random | None = None,
+        default: Any = ...,
+        children: list[FieldMeta] | None = None,
+        constraints: PydanticConstraints | None = None,
+    ) -> None:
+        super().__init__(
+            name=name, annotation=annotation, random=random, default=default, children=children, constraints=constraints
+        )
+
     @classmethod
     def from_field_info(
         cls,
         field_name: str,
         field_info: FieldInfo,
         use_alias: bool,
         random: Random | None,
@@ -81,16 +102,16 @@
             default_value = field_info.default if field_info.default is not Undefined else Null
 
         annotation = unwrap_new_type(field_info.annotation)
         children: list[FieldMeta,] | None = None
         constraints: Constraints = {}
         name = field_info.alias if field_info.alias and use_alias else field_name
 
-        # pydantic v2 do not propagate metadata for Union types
-        if is_optional_union(annotation):
+        # pydantic v2 does not always propagate metadata for Union types
+        if not field_info.metadata and is_optional(annotation):
             field_info = FieldInfo.from_annotation(unwrap_optional(annotation))
         elif is_union(annotation):
             children = [
                 cls.from_field_info(
                     field_info=FieldInfo.from_annotation(arg),
                     field_name=field_name,
                     max_collection_length=max_collection_length,
@@ -98,21 +119,31 @@
                     random=random,
                     randomize_collection_length=randomize_collection_length,
                     use_alias=use_alias,
                 )
                 for arg in get_args(annotation)
             ]
 
-        if metadata := [v for v in field_info.metadata if v is not None]:
-            constraints = cls.parse_constraints(metadata=metadata)
+        metadata, is_json = [], False
+        for m in field_info.metadata:
+            if not is_json and isinstance(m, Json):  # type: ignore[misc]
+                is_json = True
+            elif m is not None:
+                metadata.append(m)
+
+        constraints = cls.parse_constraints(metadata=metadata) if metadata else {}
+        constraints = cast(PydanticConstraints, constraints)
 
         if "url" in constraints:
             # pydantic uses a sentinel value for url constraints
             annotation = str
 
+        if is_json:
+            constraints["json"] = True
+
         return PydanticFieldMeta.from_type(
             annotation=annotation,
             children=children,
             constraints=cast("Constraints", {k: v for k, v in constraints.items() if v is not None}) or None,
             default=default_value,
             max_collection_length=max_collection_length,
             min_collection_length=min_collection_length,
@@ -241,15 +272,15 @@
 
         return PydanticFieldMeta(
             name=name,
             random=random or DEFAULT_RANDOM,
             annotation=annotation,
             children=children or None,
             default=default_value,
-            constraints=cast("Constraints", {k: v for k, v in constraints.items() if v is not None}) or None,
+            constraints=cast("PydanticConstraints", {k: v for k, v in constraints.items() if v is not None}) or None,
         )
 
 
 class ModelFactory(Generic[T], BaseFactory[T]):
     """Base factory for pydantic models"""
 
     __forward_ref_resolution_type_mapping__: ClassVar[Mapping[str, type]] = {}
@@ -308,14 +339,23 @@
                         max_collection_length=cls.__max_collection_length__,
                     )
                     for field_name, field_info in cls.__model__.model_fields.items()
                 ]
         return cls._fields_metadata
 
     @classmethod
+    def get_constrained_field_value(cls, annotation: Any, field_meta: FieldMeta) -> Any:
+        constraints = cast(PydanticConstraints, field_meta.constraints)
+        if constraints.pop("json", None):
+            value = cls.get_field_value(field_meta)
+            return to_json(value)
+
+        return super().get_constrained_field_value(annotation, field_meta)
+
+    @classmethod
     def build(cls, factory_use_construct: bool = False, **kwargs: Any) -> T:
         """Build an instance of the factory's __model__
 
         :param factory_use_construct: A boolean that determines whether validations will be made when instantiating the
                 model. This is supported only for pydantic models.
         :param kwargs: Any kwargs. If field_meta names are set in kwargs, their values will be used.
```

### Comparing `polyfactory-2.7.0/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.7.1/polyfactory/factories/typed_dict_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/field_meta.py` & `polyfactory-2.7.1/polyfactory/field_meta.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/fields.py` & `polyfactory-2.7.1/polyfactory/fields.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/persistence.py` & `polyfactory-2.7.1/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/pytest_plugin.py` & `polyfactory-2.7.1/polyfactory/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/utils/helpers.py` & `polyfactory-2.7.1/polyfactory/utils/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from typing_extensions import get_args, get_origin
 
 from polyfactory.constants import TYPE_MAPPING
 from polyfactory.utils.predicates import (
     is_annotated,
     is_new_type,
-    is_optional_union,
+    is_optional,
     is_union,
 )
 
 if TYPE_CHECKING:
     from random import Random
 
 
@@ -46,32 +46,32 @@
 def unwrap_optional(annotation: Any) -> Any:
     """Unwraps optional union types - recursively.
 
     :param annotation: A type annotation, possibly an optional union.
 
     :returns: A type annotation
     """
-    while is_optional_union(annotation):
+    while is_optional(annotation):
         annotation = next(arg for arg in get_args(annotation) if arg not in (type(None), None))
     return annotation
 
 
 def unwrap_annotation(annotation: Any, random: Random) -> Any:
     """Unwraps an annotation.
 
     :param annotation: A type annotation.
     :param random: An instance of random.Random.
 
     :returns: The unwrapped annotation.
 
     """
-    while is_optional_union(annotation) or is_union(annotation) or is_new_type(annotation) or is_annotated(annotation):
+    while is_optional(annotation) or is_union(annotation) or is_new_type(annotation) or is_annotated(annotation):
         if is_new_type(annotation):
             annotation = unwrap_new_type(annotation)
-        elif is_optional_union(annotation):
+        elif is_optional(annotation):
             annotation = unwrap_optional(annotation)
         elif is_annotated(annotation):
             annotation = unwrap_annotated(annotation, random=random)[0]
         else:
             annotation = unwrap_union(annotation, random=random)
     return annotation
```

### Comparing `polyfactory-2.7.0/polyfactory/utils/predicates.py` & `polyfactory-2.7.1/polyfactory/utils/predicates.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     :param annotation: A type annotation.
 
     :returns: A typeguard.
     """
     return get_type_origin(annotation) in UNION_TYPES
 
 
-def is_optional_union(annotation: Any) -> "TypeGuard[Any | None]":
+def is_optional(annotation: Any) -> "TypeGuard[Any | None]":
     """Determine whether a given annotation is 'typing.Optional'.
 
     :param annotation: A type annotation.
 
     :returns: A typeguard.
     """
     origin = get_type_origin(annotation)
```

### Comparing `polyfactory-2.7.0/polyfactory/value_generators/complex_types.py` & `polyfactory-2.7.1/polyfactory/value_generators/complex_types.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.7.1/polyfactory/value_generators/constrained_collections.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.7.1/polyfactory/value_generators/constrained_dates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.7.1/polyfactory/value_generators/constrained_numbers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.7.1/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/polyfactory/value_generators/primitives.py` & `polyfactory-2.7.1/polyfactory/value_generators/primitives.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 from binascii import hexlify
 from decimal import Decimal
-from os import urandom
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from random import Random
 
 
 def create_random_float(
@@ -76,15 +75,15 @@
     """
     if min_length is None:
         min_length = 0
     if max_length is None:
         max_length = min_length + 1 * 2
 
     length = random.randint(min_length, max_length)
-    result = hexlify(urandom(length))
+    result = b"" if length == 0 else hexlify(random.getrandbits(length * 8).to_bytes(length, "little"))
 
     if lower_case:
         result = result.lower()
     elif upper_case:
         result = result.upper()
 
     if max_length and len(result) > max_length:
```

### Comparing `polyfactory-2.7.0/polyfactory/value_generators/regex.py` & `polyfactory-2.7.1/polyfactory/value_generators/regex.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.7.0/pyproject.toml` & `polyfactory-2.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.7.0"
+version = "2.7.1"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
 ]
@@ -111,14 +111,15 @@
 [tool.pyright]
 include = ["polyfactory", "tests", "examples"]
 
 [tool.coverage.run]
 omit = ["*/tests/*"]
 
 [tool.pytest.ini_options]
+addopts = "tests docs/examples"
 asyncio_mode = "auto"
 filterwarnings = [
     "ignore:.*pkg_resources.declare_namespace\\('sphinxcontrib'\\).*:DeprecationWarning",
     "ignore:pkg_resources is deprecated as an API:DeprecationWarning",
     # Get rid those above once sphinxcontrib-mermaid doesn't use pkg_resources anymore
     # https://github.com/mgaitan/sphinxcontrib-mermaid/issues/119
 ]
```

### Comparing `polyfactory-2.7.0/PKG-INFO` & `polyfactory-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyfactory
-Version: 2.7.0
+Version: 2.7.1
 Summary: Mock data generation factories
 Home-page: https://github.com/litestar-org/polyfactory
 License: MIT
 Keywords: dataclasses,factory,msgspec,pydantic,testing
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
```

