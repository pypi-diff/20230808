# Comparing `tmp/forestadmin_datasource_toolkit-1.0.0b5.tar.gz` & `tmp/forestadmin_datasource_toolkit-1.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_datasource_toolkit-1.0.0b5.tar", max compression
+gzip compressed data, was "forestadmin_datasource_toolkit-1.0.0b6.tar", max compression
```

## Comparing `forestadmin_datasource_toolkit-1.0.0b5.tar` & `forestadmin_datasource_toolkit-1.0.0b6.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/README.md
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/__init__.py
--rw-r--r--   0        0        0     2276 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/collections.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/context/__init__.py
--rw-r--r--   0        0        0      678 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/context/agent_context.py
--rw-r--r--   0        0        0      658 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/context/collection_context.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/context/relaxed_wrappers/__init__.py
--rw-r--r--   0        0        0     7105 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py
--rw-r--r--   0        0        0     4741 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py
--rw-r--r--   0        0        0     1608 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py
--rw-r--r--   0        0        0     1536 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/datasources.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/__init__.py
--rw-r--r--   0        0        0     5369 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/collections.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/context/__init__.py
--rw-r--r--   0        0        0     2127 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/context/base.py
--rw-r--r--   0        0        0      664 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/context/bulk.py
--rw-r--r--   0        0        0      907 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/context/single.py
--rw-r--r--   0        0        0     2167 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/result_builder.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/types/__init__.py
--rw-r--r--   0        0        0     1688 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/types/actions.py
--rw-r--r--   0        0        0    14435 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/types/fields.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/chart/__init__.py
--rw-r--r--   0        0        0     1941 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py
--rw-r--r--   0        0        0     2133 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py
--rw-r--r--   0        0        0     1549 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py
--rw-r--r--   0        0        0     3484 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/chart/result_builder.py
--rw-r--r--   0        0        0      557 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/chart/types.py
--rw-r--r--   0        0        0     4972 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/collection_decorator.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/computed/__init__.py
--rw-r--r--   0        0        0     4690 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/computed/collections.py
--rw-r--r--   0        0        0      154 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/computed/exceptions.py
--rw-r--r--   0        0        0     3886 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/computed/helpers.py
--rw-r--r--   0        0        0      651 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/computed/types.py
--rw-r--r--   0        0        0     2812 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/computed/utils.py
--rw-r--r--   0        0        0      902 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/datasource_decorator.py
--rw-r--r--   0        0        0     4074 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/decorator_stack.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/empty/__init__.py
--rw-r--r--   0        0        0     4495 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/empty/collection.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/operators_emulate/__init__.py
--rw-r--r--   0        0        0     6398 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py
--rw-r--r--   0        0        0      320 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/operators_emulate/types.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/operators_equivalence/__init__.py
--rw-r--r--   0        0        0     3855 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/publication_field/__init__.py
--rw-r--r--   0        0        0     3015 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/publication_field/collections.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/rename_field/__init__.py
--rw-r--r--   0        0        0     9761 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/rename_field/collections.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/schema/__init__.py
--rw-r--r--   0        0        0      671 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/schema/collection.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/search/__init__.py
--rw-r--r--   0        0        0     6200 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/search/collections.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/segments/__init__.py
--rw-r--r--   0        0        0     2651 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/segments/collections.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/validation/__init__.py
--rw-r--r--   0        0        0     4142 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/validation/collection.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/write/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/write/create_relations/__init__.py
--rw-r--r--   0        0        0     5102 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/write/update_relations/__init__.py
--rw-r--r--   0        0        0     4845 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py
--rw-r--r--   0        0        0     1020 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/write/write_replace/__init__.py
--rw-r--r--   0        0        0      258 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/write/write_replace/types.py
--rw-r--r--   0        0        0     1045 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py
--rw-r--r--   0        0        0     6327 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py
--rw-r--r--   0        0        0      376 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/exceptions.py
--rw-r--r--   0        0        0     6148 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/.DS_Store
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/__init__.py
--rw-r--r--   0        0        0     1933 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/actions.py
--rw-r--r--   0        0        0      954 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/chart.py
--rw-r--r--   0        0        0     2591 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/collections.py
--rw-r--r--   0        0        0     5323 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/fields.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/models/__init__.py
--rw-r--r--   0        0        0     1420 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/models/collections.py
--rw-r--r--   0        0        0     6148 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/.DS_Store
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/__init__.py
--rw-r--r--   0        0        0     7775 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/aggregation.py
--rw-r--r--   0        0        0     6148 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/__init__.py
--rw-r--r--   0        0        0     4506 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py
--rw-r--r--   0        0        0     5377 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/__init__.py
--rw-r--r--   0        0        0     2572 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py
--rw-r--r--   0        0        0     4647 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py
--rw-r--r--   0        0        0     9798 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py
--rw-r--r--   0        0        0     1270 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/__init__.py
--rw-r--r--   0        0        0     3941 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py
--rw-r--r--   0        0        0     1688 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py
--rw-r--r--   0        0        0     7660 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/filter/__init__.py
--rw-r--r--   0        0        0     6832 2023-08-01 13:27:18.813669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py
--rw-r--r--   0        0        0     2877 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py
--rw-r--r--   0        0        0     3213 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py
--rw-r--r--   0        0        0      875 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/page.py
--rw-r--r--   0        0        0     4511 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py
--rw-r--r--   0        0        0      902 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py
--rw-r--r--   0        0        0     2619 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py
--rw-r--r--   0        0        0      595 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py
--rw-r--r--   0        0        0      118 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/records.py
--rw-r--r--   0        0        0       73 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     7235 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/utils/collections.py
--rw-r--r--   0        0        0     1169 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/utils/records.py
--rw-r--r--   0        0        0     1658 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/utils/schema.py
--rw-r--r--   0        0        0        0 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/validations/__init__.py
--rw-r--r--   0        0        0     4788 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/validations/condition_tree.py
--rw-r--r--   0        0        0     3581 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/validations/field.py
--rw-r--r--   0        0        0      393 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/validations/projection.py
--rw-r--r--   0        0        0     1542 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/validations/records.py
--rw-r--r--   0        0        0     4536 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/validations/rules.py
--rw-r--r--   0        0        0      469 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/validations/sort.py
--rw-r--r--   0        0        0     4352 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/validations/type_getter.py
--rw-r--r--   0        0        0      372 2023-08-01 13:27:18.817669 forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/validations/types.py
--rw-r--r--   0        0        0     1758 2023-08-01 13:27:37.186033 forestadmin_datasource_toolkit-1.0.0b5/pyproject.toml
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-1.0.0b5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/README.md
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/__init__.py
+-rw-r--r--   0        0        0     2276 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/collections.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/context/__init__.py
+-rw-r--r--   0        0        0      678 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/context/agent_context.py
+-rw-r--r--   0        0        0      658 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/context/collection_context.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/context/relaxed_wrappers/__init__.py
+-rw-r--r--   0        0        0     7105 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py
+-rw-r--r--   0        0        0     4741 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py
+-rw-r--r--   0        0        0     1608 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py
+-rw-r--r--   0        0        0     1536 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/datasources.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/__init__.py
+-rw-r--r--   0        0        0     5369 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/collections.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/context/__init__.py
+-rw-r--r--   0        0        0     2127 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/context/base.py
+-rw-r--r--   0        0        0      664 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/context/bulk.py
+-rw-r--r--   0        0        0      907 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/context/single.py
+-rw-r--r--   0        0        0     2167 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/result_builder.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/types/__init__.py
+-rw-r--r--   0        0        0     1688 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/types/actions.py
+-rw-r--r--   0        0        0    14435 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/types/fields.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/chart/__init__.py
+-rw-r--r--   0        0        0     1941 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py
+-rw-r--r--   0        0        0     2133 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py
+-rw-r--r--   0        0        0     1549 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py
+-rw-r--r--   0        0        0     3484 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/chart/result_builder.py
+-rw-r--r--   0        0        0      557 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/chart/types.py
+-rw-r--r--   0        0        0     4972 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/collection_decorator.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/computed/__init__.py
+-rw-r--r--   0        0        0     4690 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/computed/collections.py
+-rw-r--r--   0        0        0      154 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/computed/exceptions.py
+-rw-r--r--   0        0        0     3886 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/computed/helpers.py
+-rw-r--r--   0        0        0      651 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/computed/types.py
+-rw-r--r--   0        0        0     2812 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/computed/utils.py
+-rw-r--r--   0        0        0      902 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/datasource_decorator.py
+-rw-r--r--   0        0        0     4074 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/decorator_stack.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/empty/__init__.py
+-rw-r--r--   0        0        0     4495 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/empty/collection.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/operators_emulate/__init__.py
+-rw-r--r--   0        0        0     6398 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py
+-rw-r--r--   0        0        0      320 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/operators_emulate/types.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/operators_equivalence/__init__.py
+-rw-r--r--   0        0        0     3855 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/publication_field/__init__.py
+-rw-r--r--   0        0        0     3015 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/publication_field/collections.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/rename_field/__init__.py
+-rw-r--r--   0        0        0     9761 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/rename_field/collections.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/schema/__init__.py
+-rw-r--r--   0        0        0      671 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/schema/collection.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/search/__init__.py
+-rw-r--r--   0        0        0     6200 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/search/collections.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/segments/__init__.py
+-rw-r--r--   0        0        0     2651 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/segments/collections.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/validation/__init__.py
+-rw-r--r--   0        0        0     4142 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/validation/collection.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/write/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/write/create_relations/__init__.py
+-rw-r--r--   0        0        0     5102 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/write/update_relations/__init__.py
+-rw-r--r--   0        0        0     4845 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py
+-rw-r--r--   0        0        0     1020 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/write/write_replace/__init__.py
+-rw-r--r--   0        0        0      258 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/write/write_replace/types.py
+-rw-r--r--   0        0        0     1045 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py
+-rw-r--r--   0        0        0     6327 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py
+-rw-r--r--   0        0        0      376 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/exceptions.py
+-rw-r--r--   0        0        0     6148 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/.DS_Store
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/__init__.py
+-rw-r--r--   0        0        0     1933 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/actions.py
+-rw-r--r--   0        0        0      954 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/chart.py
+-rw-r--r--   0        0        0     2591 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/collections.py
+-rw-r--r--   0        0        0     5323 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/fields.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/models/__init__.py
+-rw-r--r--   0        0        0     1420 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/models/collections.py
+-rw-r--r--   0        0        0     6148 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/.DS_Store
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/__init__.py
+-rw-r--r--   0        0        0     7775 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/aggregation.py
+-rw-r--r--   0        0        0     6148 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/__init__.py
+-rw-r--r--   0        0        0     4506 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py
+-rw-r--r--   0        0        0     5377 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/__init__.py
+-rw-r--r--   0        0        0     2572 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py
+-rw-r--r--   0        0        0     4647 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py
+-rw-r--r--   0        0        0     9798 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py
+-rw-r--r--   0        0        0     1270 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/__init__.py
+-rw-r--r--   0        0        0     3941 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py
+-rw-r--r--   0        0        0     1688 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py
+-rw-r--r--   0        0        0     7660 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/filter/__init__.py
+-rw-r--r--   0        0        0     6832 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py
+-rw-r--r--   0        0        0     2877 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py
+-rw-r--r--   0        0        0     3213 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py
+-rw-r--r--   0        0        0      875 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/page.py
+-rw-r--r--   0        0        0     4511 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py
+-rw-r--r--   0        0        0      902 2023-08-08 13:36:21.143791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py
+-rw-r--r--   0        0        0     2619 2023-08-08 13:36:21.147791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py
+-rw-r--r--   0        0        0      595 2023-08-08 13:36:21.147791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py
+-rw-r--r--   0        0        0      118 2023-08-08 13:36:21.147791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/records.py
+-rw-r--r--   0        0        0       73 2023-08-08 13:36:21.147791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     7255 2023-08-08 13:36:21.147791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/utils/collections.py
+-rw-r--r--   0        0        0     1169 2023-08-08 13:36:21.147791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/utils/records.py
+-rw-r--r--   0        0        0     1658 2023-08-08 13:36:21.147791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/utils/schema.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:36:21.147791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/validations/__init__.py
+-rw-r--r--   0        0        0     4788 2023-08-08 13:36:21.147791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/validations/condition_tree.py
+-rw-r--r--   0        0        0     3581 2023-08-08 13:36:21.147791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/validations/field.py
+-rw-r--r--   0        0        0      393 2023-08-08 13:36:21.147791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/validations/projection.py
+-rw-r--r--   0        0        0     1542 2023-08-08 13:36:21.147791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/validations/records.py
+-rw-r--r--   0        0        0     4536 2023-08-08 13:36:21.147791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/validations/rules.py
+-rw-r--r--   0        0        0      469 2023-08-08 13:36:21.147791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/validations/sort.py
+-rw-r--r--   0        0        0     4352 2023-08-08 13:36:21.147791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/validations/type_getter.py
+-rw-r--r--   0        0        0      372 2023-08-08 13:36:21.147791 forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/validations/types.py
+-rw-r--r--   0        0        0     1758 2023-08-08 13:36:37.976026 forestadmin_datasource_toolkit-1.0.0b6/pyproject.toml
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-1.0.0b6/PKG-INFO
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/collections.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/context/agent_context.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/context/agent_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/context/collection_context.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/context/collection_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/datasources.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/datasources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/collections.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/context/base.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/context/base.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/context/bulk.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/context/bulk.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/context/single.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/context/single.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/result_builder.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/result_builder.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/types/actions.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/types/actions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/action/types/fields.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/action/types/fields.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/chart/result_builder.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/chart/result_builder.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/chart/types.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/chart/types.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/collection_decorator.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/collection_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/computed/collections.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/computed/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/computed/helpers.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/computed/helpers.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/computed/types.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/computed/types.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/computed/utils.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/computed/utils.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/datasource_decorator.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/datasource_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/decorator_stack.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/decorator_stack.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/empty/collection.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/empty/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/publication_field/collections.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/publication_field/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/rename_field/collections.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/rename_field/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/schema/collection.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/schema/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/search/collections.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/search/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/segments/collections.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/segments/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/validation/collection.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/validation/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/.DS_Store` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/actions.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/actions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/chart.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/chart.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/collections.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/fields.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/fields.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/models/collections.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/models/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/.DS_Store` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/aggregation.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/aggregation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/page.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/page.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/utils/collections.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/utils/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,22 +77,22 @@
         foreign_collection: Collection,
         relation: Union[ManyToMany, OneToMany],
         foreign_filter: PaginatedFilter,
         projection: Projection,
     ) -> List[RecordsDataAlias]:
         from forestadmin.datasource_toolkit.interfaces.query.filter.factory import FilterFactory
 
-        if is_many_to_many(relation) and relation["foreign_relation"] and foreign_filter.is_nestable:
+        if is_many_to_many(relation) and relation.get("foreign_relation") and foreign_filter.is_nestable:
             through = collection.datasource.get_collection(relation["through_collection"])
             records = await through.list(
                 caller,
-                await FilterFactory.make_through_filter(collection, id, relation, foreign_filter),
-                projection.nest(relation["foreign_relation"]),
+                await FilterFactory.make_through_filter(caller, collection, id, relation, foreign_filter),
+                projection.nest(relation.get("foreign_relation")),
             )
-            return [record[relation["foreign_relation"]] for record in records]
+            return [record[relation.get("foreign_relation")] for record in records]
         return await foreign_collection.list(
             caller,
             await FilterFactory.make_foreign_filter(caller, collection, id, relation, foreign_filter),
             projection,
         )
 
     @staticmethod
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/utils/records.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/utils/records.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/utils/schema.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/utils/schema.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/validations/condition_tree.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/validations/condition_tree.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/validations/field.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/validations/field.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/validations/records.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/validations/records.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/validations/rules.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/validations/rules.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/forestadmin/datasource_toolkit/validations/type_getter.py` & `forestadmin_datasource_toolkit-1.0.0b6/forestadmin/datasource_toolkit/validations/type_getter.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,20 +16,20 @@
     @classmethod
     def get(cls, value: Any, type_context: Optional[PrimitiveType]) -> Union[PrimitiveType, ValidationType]:
         if isinstance(value, list):
             value = cast(List[Any], value)
             return cls._get_array_type(value, type_context)
         elif isinstance(value, str):
             return cls._get_type_from_string(value, type_context)
+        elif isinstance(value, bool):
+            return PrimitiveType.BOOLEAN
         elif isinstance(value, float) or isinstance(value, int):
             return PrimitiveType.NUMBER
         elif isinstance(value, datetime):
             return PrimitiveType.DATE
-        elif isinstance(value, bool):
-            return PrimitiveType.BOOLEAN
         elif isinstance(value, dict) and type_context == PrimitiveType.JSON:
             return PrimitiveType.JSON
 
         return ValidationPrimaryType.NULL
 
     @staticmethod
     def _get_date_type(value: str) -> PrimitiveType:
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/pyproject.toml` & `forestadmin_datasource_toolkit-1.0.0b6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-datasource-toolkit"
-version = "1.0.0-beta.5"
+version = "1.0.0-beta.6"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.semantic_release]
```

### Comparing `forestadmin_datasource_toolkit-1.0.0b5/PKG-INFO` & `forestadmin_datasource_toolkit-1.0.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forestadmin-datasource-toolkit
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: 
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

