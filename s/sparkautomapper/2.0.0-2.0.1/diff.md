# Comparing `tmp/sparkautomapper-2.0.0.tar.gz` & `tmp/sparkautomapper-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkautomapper-2.0.0.tar", last modified: Thu Jul 27 22:39:27 2023, max compression
+gzip compressed data, was "sparkautomapper-2.0.1.tar", last modified: Tue Aug  8 20:53:05 2023, max compression
```

## Comparing `sparkautomapper-2.0.0.tar` & `sparkautomapper-2.0.1.tar`

### file list

```diff
@@ -1,342 +1,342 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.563442 sparkautomapper-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-07-27 22:39:27.563442 sparkautomapper-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-27 22:39:27.000000 sparkautomapper-2.0.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-27 22:39:27.563442 sparkautomapper-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.523441 sparkautomapper-2.0.0/spark_auto_mapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.527441 sparkautomapper-2.0.0/spark_auto_mapper/automappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/automappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31339 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/automappers/automapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/automappers/automapper_analysis_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/automappers/automapper_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/automappers/automapper_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/automappers/check_schema_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/automappers/column_spec_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/automappers/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/automappers/complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/automappers/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/automappers/with_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/automappers/with_column_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.531441 sparkautomapper-2.0.0/spark_auto_mapper/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/array_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/array_distinct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/array_max.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/cast_to_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/coalesce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/column_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.531441 sparkautomapper-2.0.0/spark_auto_mapper/data_types/complex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/complex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/complex/complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/complex/complex_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/complex/struct_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/cross_column_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    41323 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/data_type_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/date_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/decimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/exists.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/first.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/first_valid_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/if_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/if_column_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/if_not.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/if_not_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/if_not_null_or_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/if_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/join_using_delimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/literal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/lpad.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.535441 sparkautomapper-2.0.0/spark_auto_mapper/data_types/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/nested_array_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/null_if_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/null_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/regex_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/regex_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/split_by_delimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/substring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/substring_by_delimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/text_like_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/to_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/trim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/data_types/unix_timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.535441 sparkautomapper-2.0.0/spark_auto_mapper/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29706 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/helpers/automapper_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/helpers/capture_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/helpers/expression_comparer.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/helpers/field_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/helpers/python_keyword_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/helpers/spark_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/helpers/value_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.535441 sparkautomapper-2.0.0/spark_auto_mapper/type_definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/type_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/type_definitions/defined_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/type_definitions/native_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/spark_auto_mapper/type_definitions/wrapper_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.535441 sparkautomapper-2.0.0/sparkautomapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-07-27 22:39:27.000000 sparkautomapper-2.0.0/sparkautomapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-07-27 22:39:27.000000 sparkautomapper-2.0.0/sparkautomapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:39:27.000000 sparkautomapper-2.0.0/sparkautomapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:39:27.000000 sparkautomapper-2.0.0/sparkautomapper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 22:39:27.000000 sparkautomapper-2.0.0/sparkautomapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 22:39:27.000000 sparkautomapper-2.0.0/sparkautomapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.535441 sparkautomapper-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.535441 sparkautomapper-2.0.0/tests/amount/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/amount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/amount/test_automapper_amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/amount/test_automapper_amount_typed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.535441 sparkautomapper-2.0.0/tests/array/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/array/test_automapper_array_typed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.539441 sparkautomapper-2.0.0/tests/array_distinct/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/array_distinct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/array_distinct/test_automapper_array_distinct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.539441 sparkautomapper-2.0.0/tests/array_max/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/array_max/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/array_max/test_automapper_array_max.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.539441 sparkautomapper-2.0.0/tests/base64/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/base64/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/base64/test_automapper_base64.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.539441 sparkautomapper-2.0.0/tests/boolean/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/boolean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/boolean/test_automapper_boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/boolean/test_automapper_boolean_typed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.539441 sparkautomapper-2.0.0/tests/cast/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/cast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/cast/test_cast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.539441 sparkautomapper-2.0.0/tests/cast_to_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/cast_to_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/cast_to_type/test_automapper_cast_to_type_typed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.539441 sparkautomapper-2.0.0/tests/checkpointing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/checkpointing/test_automapper_full_checkpointing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.539441 sparkautomapper-2.0.0/tests/coalesce/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/coalesce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/coalesce/test_automapper_coalesce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.539441 sparkautomapper-2.0.0/tests/columns/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/columns/test_automapper_columns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.539441 sparkautomapper-2.0.0/tests/complex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/complex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/complex/test_automapper_complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/complex/test_automapper_complex_with_defined_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/complex/test_automapper_complex_with_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/complex/test_automapper_complex_with_mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/complex/test_automapper_complex_with_skip_if_null.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.543442 sparkautomapper-2.0.0/tests/concat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/concat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/concat/test_automapper_add_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/concat/test_automapper_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/concat/test_automapper_concat_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/concat/test_automapper_concat_multiple_items_structs_different_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/concat/test_automapper_concat_multiple_items_structs_different_elements_with_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.543442 sparkautomapper-2.0.0/tests/copy_unmapped_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/copy_unmapped_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/copy_unmapped_properties/test_automapper_copy_unmapped_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.543442 sparkautomapper-2.0.0/tests/cross_column_filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/cross_column_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/cross_column_filter/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/cross_column_filter/test_cross_column_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.543442 sparkautomapper-2.0.0/tests/date/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/date/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/date/test_automapper_date_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/date/test_automapper_date_column_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/date/test_automapper_date_literal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.543442 sparkautomapper-2.0.0/tests/date_format/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/date_format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/date_format/test_automapper_date_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.543442 sparkautomapper-2.0.0/tests/decimal_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/decimal_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/decimal_type/test_automapper_decimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/decimal_type/test_automapper_decimal_typed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.543442 sparkautomapper-2.0.0/tests/duplicates_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/duplicates_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/duplicates_test/test_automapper_duplicates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.543442 sparkautomapper-2.0.0/tests/exists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/exists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/exists/test_automapper_exists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.543442 sparkautomapper-2.0.0/tests/field/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/field/test_automapper_field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.543442 sparkautomapper-2.0.0/tests/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/filter/test_automapper_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.543442 sparkautomapper-2.0.0/tests/first/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/first/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/first/test_automapper_first.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.543442 sparkautomapper-2.0.0/tests/first_valid_column/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/first_valid_column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/first_valid_column/test_automapper_first_valid_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/first_valid_column/test_automapper_first_valid_column_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.543442 sparkautomapper-2.0.0/tests/flatten/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/flatten/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/flatten/test_automapper_flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/flatten/test_automapper_flatten_with_null.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.547442 sparkautomapper-2.0.0/tests/hash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/hash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/hash/test_automapper_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.547442 sparkautomapper-2.0.0/tests/if_/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/if_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/if_/test_automapper_if_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/if_/test_automapper_if_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.547442 sparkautomapper-2.0.0/tests/if_column_exists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/if_column_exists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/if_column_exists/test_automapper_if_column_exists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.547442 sparkautomapper-2.0.0/tests/if_not/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/if_not/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/if_not/test_automapper_if_not.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/if_not/test_automapper_if_not_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.547442 sparkautomapper-2.0.0/tests/if_not_null/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/if_not_null/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/if_not_null/test_automapper_if_not_null.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.547442 sparkautomapper-2.0.0/tests/if_not_null_or_empty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/if_not_null_or_empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/if_not_null_or_empty/test_automapper_if_not_null_or_empty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.547442 sparkautomapper-2.0.0/tests/if_regex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/if_regex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/if_regex/test_automapper_if_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.547442 sparkautomapper-2.0.0/tests/join_using_delimiter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/join_using_delimiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/join_using_delimiter/test_automapper_join_using_delimiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.547442 sparkautomapper-2.0.0/tests/left/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/left/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/left/test_automapper_left.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.547442 sparkautomapper-2.0.0/tests/list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/list/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.551442 sparkautomapper-2.0.0/tests/list/addition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/list/addition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements_with_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/list/test_automapper_list_multiple_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/list/test_automapper_list_multiple_items_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/list/test_automapper_list_multiple_items_structs_different_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/list/test_automapper_list_multiple_items_structs_different_elements_with_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/list/test_automapper_list_multiple_items_with_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/list/test_automapper_list_single_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/list/test_automapper_list_single_item_with_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.551442 sparkautomapper-2.0.0/tests/lpad/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/lpad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/lpad/test_auto_mapper_lpad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.551442 sparkautomapper-2.0.0/tests/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/map/test_automapper_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/map/test_automapper_map_col_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/map/test_automapper_map_no_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/map/test_automapper_map_null.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.551442 sparkautomapper-2.0.0/tests/multiple_columns/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/multiple_columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/multiple_columns/test_automapper_multiple_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/multiple_columns/test_automapper_multiple_columns_simpler_syntax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.551442 sparkautomapper-2.0.0/tests/nested_array_filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/nested_array_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/nested_array_filter/location.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/nested_array_filter/schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.551442 sparkautomapper-2.0.0/tests/nested_array_filter/simple/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/nested_array_filter/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/nested_array_filter/simple/test_automapper_nested_array_filter_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.551442 sparkautomapper-2.0.0/tests/nested_array_filter/simple_with_array/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/nested_array_filter/simple_with_array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/nested_array_filter/simple_with_array/test_automapper_nested_array_filter_simple_with_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/nested_array_filter/test_automapper_nested_array_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/nested_array_filter/test_automapper_nested_array_filter_expression_only.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.551442 sparkautomapper-2.0.0/tests/null_if_empty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/null_if_empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/null_if_empty/test_automapper_null_if_empty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.551442 sparkautomapper-2.0.0/tests/null_remover/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/null_remover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/null_remover/test_automapper_null_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.551442 sparkautomapper-2.0.0/tests/number/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/number/test_automapper_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/number/test_automapper_number_typed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.551442 sparkautomapper-2.0.0/tests/regex_extract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/regex_extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/regex_extract/test_auto_mapper_regex_extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.555442 sparkautomapper-2.0.0/tests/regex_replace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/regex_replace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/regex_replace/test_auto_mapper_regex_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/regex_replace/test_auto_mapper_regex_replace_unicode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.555442 sparkautomapper-2.0.0/tests/right/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/right/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/right/test_automapper_right.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.555442 sparkautomapper-2.0.0/tests/sanitize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/sanitize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/sanitize/test_auto_mapper_sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.555442 sparkautomapper-2.0.0/tests/schema_pruning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/schema_pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/schema_pruning/test_automapper_schema_pruning_with_defined_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/schema_pruning/test_automapper_schema_pruning_with_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/schema_pruning/test_automapper_schema_pruning_with_extension_different_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.555442 sparkautomapper-2.0.0/tests/select_one/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/select_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/select_one/test_automapper_select_one.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.559442 sparkautomapper-2.0.0/tests/split_by_delimiter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/split_by_delimiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/split_by_delimiter/test_automapper_split_by_delimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/split_by_delimiter/test_automapper_split_by_delimiter_and_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/split_by_delimiter/test_automapper_split_by_delimiter_and_transform_fluent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.559442 sparkautomapper-2.0.0/tests/string_after_delimiter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/string_after_delimiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/string_after_delimiter/test_automapper_string_after_delimiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.559442 sparkautomapper-2.0.0/tests/string_before_delimiter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/string_before_delimiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/string_before_delimiter/test_automapper_string_before_delimiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.559442 sparkautomapper-2.0.0/tests/struct_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/struct_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/struct_type/test_automapper_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/struct_type/test_automapper_struct_with_mappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.559442 sparkautomapper-2.0.0/tests/substring_by_delimiter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/substring_by_delimiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/substring_by_delimiter/test_automapper_substring_by_delimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/test_automapper_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/test_automapper_full_no_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/test_automapper_full_no_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/test_automapper_full_view_exists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.559442 sparkautomapper-2.0.0/tests/to_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/to_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/to_json/test_automapper_to_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.559442 sparkautomapper-2.0.0/tests/transform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/transform/test_automapper_filter_and_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/transform/test_automapper_filter_and_transform_fluent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/transform/test_automapper_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.559442 sparkautomapper-2.0.0/tests/trim/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/trim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/trim/test_auto_mapper_trim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.563442 sparkautomapper-2.0.0/tests/unix_timestamp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/unix_timestamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/unix_timestamp/test_automapper_unix_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/unix_timestamp/test_automapper_unix_timestamp_literal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/unix_timestamp/test_automapper_unix_timestamp_string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:39:27.563442 sparkautomapper-2.0.0/tests/withColumn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/withColumn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/withColumn/test_automapper_with_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/withColumn/test_automapper_with_column_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/withColumn/test_automapper_with_column_literal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-27 22:38:18.000000 sparkautomapper-2.0.0/tests/withColumn/test_automapper_with_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.227529 sparkautomapper-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-08-08 20:53:05.227529 sparkautomapper-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 20:53:04.000000 sparkautomapper-2.0.1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-08 20:53:05.227529 sparkautomapper-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.171528 sparkautomapper-2.0.1/spark_auto_mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.175528 sparkautomapper-2.0.1/spark_auto_mapper/automappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/automappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31339 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/automappers/automapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/automappers/automapper_analysis_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/automappers/automapper_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/automappers/automapper_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/automappers/check_schema_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/automappers/column_spec_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/automappers/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/automappers/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/automappers/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/automappers/with_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/automappers/with_column_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.187528 sparkautomapper-2.0.1/spark_auto_mapper/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/array_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/array_distinct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/array_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/cast_to_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/coalesce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/column_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.187528 sparkautomapper-2.0.1/spark_auto_mapper/data_types/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/complex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/complex/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/complex/complex_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/complex/struct_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/cross_column_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41355 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/data_type_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/date_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/first_valid_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/if_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/if_column_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/if_not.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/if_not_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/if_not_null_or_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/if_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/join_using_delimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/lpad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.187528 sparkautomapper-2.0.1/spark_auto_mapper/data_types/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/nested_array_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/null_if_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/null_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/regex_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/regex_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/split_by_delimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/substring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/substring_by_delimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/text_like_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/to_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/trim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/data_types/unix_timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.187528 sparkautomapper-2.0.1/spark_auto_mapper/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29706 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/helpers/automapper_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/helpers/capture_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/helpers/expression_comparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/helpers/field_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/helpers/python_keyword_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/helpers/spark_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/helpers/value_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.191528 sparkautomapper-2.0.1/spark_auto_mapper/type_definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/type_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/type_definitions/defined_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/type_definitions/native_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/spark_auto_mapper/type_definitions/wrapper_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.191528 sparkautomapper-2.0.1/sparkautomapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-08-08 20:53:05.000000 sparkautomapper-2.0.1/sparkautomapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-08-08 20:53:05.000000 sparkautomapper-2.0.1/sparkautomapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:53:05.000000 sparkautomapper-2.0.1/sparkautomapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:53:05.000000 sparkautomapper-2.0.1/sparkautomapper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-08 20:53:05.000000 sparkautomapper-2.0.1/sparkautomapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 20:53:05.000000 sparkautomapper-2.0.1/sparkautomapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.191528 sparkautomapper-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.195528 sparkautomapper-2.0.1/tests/amount/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/amount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/amount/test_automapper_amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/amount/test_automapper_amount_typed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.195528 sparkautomapper-2.0.1/tests/array/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/array/test_automapper_array_typed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.195528 sparkautomapper-2.0.1/tests/array_distinct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/array_distinct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/array_distinct/test_automapper_array_distinct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.195528 sparkautomapper-2.0.1/tests/array_max/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/array_max/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/array_max/test_automapper_array_max.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.195528 sparkautomapper-2.0.1/tests/base64/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/base64/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/base64/test_automapper_base64.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.195528 sparkautomapper-2.0.1/tests/boolean/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/boolean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/boolean/test_automapper_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/boolean/test_automapper_boolean_typed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.195528 sparkautomapper-2.0.1/tests/cast/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/cast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/cast/test_cast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.195528 sparkautomapper-2.0.1/tests/cast_to_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/cast_to_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/cast_to_type/test_automapper_cast_to_type_typed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.195528 sparkautomapper-2.0.1/tests/checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/checkpointing/test_automapper_full_checkpointing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.195528 sparkautomapper-2.0.1/tests/coalesce/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/coalesce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/coalesce/test_automapper_coalesce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.199529 sparkautomapper-2.0.1/tests/columns/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/columns/test_automapper_columns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.199529 sparkautomapper-2.0.1/tests/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/complex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/complex/test_automapper_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/complex/test_automapper_complex_with_defined_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/complex/test_automapper_complex_with_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/complex/test_automapper_complex_with_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/complex/test_automapper_complex_with_skip_if_null.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.199529 sparkautomapper-2.0.1/tests/concat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/concat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/concat/test_automapper_add_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/concat/test_automapper_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/concat/test_automapper_concat_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/concat/test_automapper_concat_multiple_items_structs_different_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/concat/test_automapper_concat_multiple_items_structs_different_elements_with_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.199529 sparkautomapper-2.0.1/tests/copy_unmapped_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/copy_unmapped_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/copy_unmapped_properties/test_automapper_copy_unmapped_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.199529 sparkautomapper-2.0.1/tests/cross_column_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/cross_column_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/cross_column_filter/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/cross_column_filter/test_cross_column_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.203529 sparkautomapper-2.0.1/tests/date/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/date/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/date/test_automapper_date_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/date/test_automapper_date_column_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/date/test_automapper_date_literal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.203529 sparkautomapper-2.0.1/tests/date_format/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/date_format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/date_format/test_automapper_date_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.203529 sparkautomapper-2.0.1/tests/decimal_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/decimal_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/decimal_type/test_automapper_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/decimal_type/test_automapper_decimal_typed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.203529 sparkautomapper-2.0.1/tests/duplicates_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/duplicates_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/duplicates_test/test_automapper_duplicates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.203529 sparkautomapper-2.0.1/tests/exists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/exists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/exists/test_automapper_exists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.203529 sparkautomapper-2.0.1/tests/field/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/field/test_automapper_field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.203529 sparkautomapper-2.0.1/tests/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/filter/test_automapper_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.203529 sparkautomapper-2.0.1/tests/first/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/first/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/first/test_automapper_first.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.207528 sparkautomapper-2.0.1/tests/first_valid_column/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/first_valid_column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/first_valid_column/test_automapper_first_valid_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/first_valid_column/test_automapper_first_valid_column_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.207528 sparkautomapper-2.0.1/tests/flatten/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/flatten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/flatten/test_automapper_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/flatten/test_automapper_flatten_with_null.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.207528 sparkautomapper-2.0.1/tests/hash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/hash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/hash/test_automapper_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.207528 sparkautomapper-2.0.1/tests/if_/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/if_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/if_/test_automapper_if_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/if_/test_automapper_if_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.207528 sparkautomapper-2.0.1/tests/if_column_exists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/if_column_exists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/if_column_exists/test_automapper_if_column_exists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.207528 sparkautomapper-2.0.1/tests/if_not/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/if_not/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/if_not/test_automapper_if_not.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/if_not/test_automapper_if_not_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.207528 sparkautomapper-2.0.1/tests/if_not_null/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/if_not_null/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/if_not_null/test_automapper_if_not_null.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.211529 sparkautomapper-2.0.1/tests/if_not_null_or_empty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/if_not_null_or_empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/if_not_null_or_empty/test_automapper_if_not_null_or_empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.211529 sparkautomapper-2.0.1/tests/if_regex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/if_regex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/if_regex/test_automapper_if_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.211529 sparkautomapper-2.0.1/tests/join_using_delimiter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/join_using_delimiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/join_using_delimiter/test_automapper_join_using_delimiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.211529 sparkautomapper-2.0.1/tests/left/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/left/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/left/test_automapper_left.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.211529 sparkautomapper-2.0.1/tests/list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/list/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.211529 sparkautomapper-2.0.1/tests/list/addition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/list/addition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements_with_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/list/test_automapper_list_multiple_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/list/test_automapper_list_multiple_items_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/list/test_automapper_list_multiple_items_structs_different_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/list/test_automapper_list_multiple_items_structs_different_elements_with_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/list/test_automapper_list_multiple_items_with_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/list/test_automapper_list_single_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/list/test_automapper_list_single_item_with_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.215529 sparkautomapper-2.0.1/tests/lpad/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/lpad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/lpad/test_auto_mapper_lpad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.215529 sparkautomapper-2.0.1/tests/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/map/test_automapper_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/map/test_automapper_map_col_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/map/test_automapper_map_no_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/map/test_automapper_map_null.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.215529 sparkautomapper-2.0.1/tests/multiple_columns/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/multiple_columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/multiple_columns/test_automapper_multiple_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/multiple_columns/test_automapper_multiple_columns_simpler_syntax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.215529 sparkautomapper-2.0.1/tests/nested_array_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/nested_array_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/nested_array_filter/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/nested_array_filter/schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.215529 sparkautomapper-2.0.1/tests/nested_array_filter/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/nested_array_filter/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/nested_array_filter/simple/test_automapper_nested_array_filter_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.215529 sparkautomapper-2.0.1/tests/nested_array_filter/simple_with_array/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/nested_array_filter/simple_with_array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/nested_array_filter/simple_with_array/test_automapper_nested_array_filter_simple_with_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/nested_array_filter/test_automapper_nested_array_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/nested_array_filter/test_automapper_nested_array_filter_expression_only.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.215529 sparkautomapper-2.0.1/tests/null_if_empty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/null_if_empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/null_if_empty/test_automapper_null_if_empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.219529 sparkautomapper-2.0.1/tests/null_remover/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/null_remover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/null_remover/test_automapper_null_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.219529 sparkautomapper-2.0.1/tests/number/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/number/test_automapper_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/number/test_automapper_number_typed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.219529 sparkautomapper-2.0.1/tests/regex_extract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/regex_extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/regex_extract/test_auto_mapper_regex_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.219529 sparkautomapper-2.0.1/tests/regex_replace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/regex_replace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/regex_replace/test_auto_mapper_regex_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/regex_replace/test_auto_mapper_regex_replace_unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.219529 sparkautomapper-2.0.1/tests/right/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/right/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/right/test_automapper_right.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.219529 sparkautomapper-2.0.1/tests/sanitize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/sanitize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/sanitize/test_auto_mapper_sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.219529 sparkautomapper-2.0.1/tests/schema_pruning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/schema_pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/schema_pruning/test_automapper_schema_pruning_with_defined_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/schema_pruning/test_automapper_schema_pruning_with_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/schema_pruning/test_automapper_schema_pruning_with_extension_different_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.219529 sparkautomapper-2.0.1/tests/select_one/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/select_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/select_one/test_automapper_select_one.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.223528 sparkautomapper-2.0.1/tests/split_by_delimiter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/split_by_delimiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/split_by_delimiter/test_automapper_split_by_delimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/split_by_delimiter/test_automapper_split_by_delimiter_and_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/split_by_delimiter/test_automapper_split_by_delimiter_and_transform_fluent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.223528 sparkautomapper-2.0.1/tests/string_after_delimiter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/string_after_delimiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/string_after_delimiter/test_automapper_string_after_delimiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.223528 sparkautomapper-2.0.1/tests/string_before_delimiter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/string_before_delimiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/string_before_delimiter/test_automapper_string_before_delimiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.223528 sparkautomapper-2.0.1/tests/struct_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/struct_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/struct_type/test_automapper_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/struct_type/test_automapper_struct_with_mappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.223528 sparkautomapper-2.0.1/tests/substring_by_delimiter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/substring_by_delimiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/substring_by_delimiter/test_automapper_substring_by_delimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/test_automapper_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/test_automapper_full_no_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/test_automapper_full_no_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/test_automapper_full_view_exists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.223528 sparkautomapper-2.0.1/tests/to_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/to_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/to_json/test_automapper_to_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.227529 sparkautomapper-2.0.1/tests/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/transform/test_automapper_filter_and_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/transform/test_automapper_filter_and_transform_fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/transform/test_automapper_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.227529 sparkautomapper-2.0.1/tests/trim/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/trim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/trim/test_auto_mapper_trim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.227529 sparkautomapper-2.0.1/tests/unix_timestamp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/unix_timestamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/unix_timestamp/test_automapper_unix_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/unix_timestamp/test_automapper_unix_timestamp_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/unix_timestamp/test_automapper_unix_timestamp_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:53:05.227529 sparkautomapper-2.0.1/tests/withColumn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/withColumn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/withColumn/test_automapper_with_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/withColumn/test_automapper_with_column_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/withColumn/test_automapper_with_column_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-08-08 20:51:52.000000 sparkautomapper-2.0.1/tests/withColumn/test_automapper_with_filter.py
```

### Comparing `sparkautomapper-2.0.0/LICENSE` & `sparkautomapper-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/PKG-INFO` & `sparkautomapper-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkautomapper
-Version: 2.0.0
+Version: 2.0.1
 Summary: AutoMapper for Spark
 Home-page: https://github.com/imranq2/SparkAutoMapper
 Author: Imran Qureshi
 Author-email: imranq2@hotmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sparkautomapper-2.0.0/README.md` & `sparkautomapper-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/setup.py` & `sparkautomapper-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
 fix_setuptools()
 
 # classifiers list is here: https://pypi.org/classifiers/
 
 # create the package setup
 setup(
     install_requires=[
-        "pyspark>=3.1.1",
+        "pyspark==3.3.0",
         "logger>=1.4",
-        "sparkdataframecomparer>=1.0.6",
+        "sparkdataframecomparer>=2.0.2",
         "deprecated>=1.2.12",
         "numpy>=1.7",
     ],
     name=package_name,
     version=version,
     author="Imran Qureshi",
     author_email="imranq2@hotmail.com",
```

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/automappers/automapper.py` & `sparkautomapper-2.0.1/spark_auto_mapper/automappers/automapper.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/automappers/automapper_analysis_exception.py` & `sparkautomapper-2.0.1/spark_auto_mapper/automappers/automapper_analysis_exception.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/automappers/automapper_base.py` & `sparkautomapper-2.0.1/spark_auto_mapper/automappers/automapper_base.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/automappers/check_schema_result.py` & `sparkautomapper-2.0.1/spark_auto_mapper/automappers/check_schema_result.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/automappers/column_spec_wrapper.py` & `sparkautomapper-2.0.1/spark_auto_mapper/automappers/column_spec_wrapper.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/automappers/columns.py` & `sparkautomapper-2.0.1/spark_auto_mapper/automappers/columns.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/automappers/complex.py` & `sparkautomapper-2.0.1/spark_auto_mapper/automappers/complex.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/automappers/container.py` & `sparkautomapper-2.0.1/spark_auto_mapper/automappers/container.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/automappers/with_column.py` & `sparkautomapper-2.0.1/spark_auto_mapper/automappers/with_column.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/automappers/with_column_base.py` & `sparkautomapper-2.0.1/spark_auto_mapper/automappers/with_column_base.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/amount.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/amount.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/array.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/array.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/array_base.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/array_base.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/array_distinct.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/array_distinct.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/array_max.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/array_max.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/base64.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/base64.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/boolean.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/boolean.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/cast_to_type.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/cast_to_type.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/coalesce.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/coalesce.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/column.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/column.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/column_wrapper.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/column_wrapper.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/complex/complex.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/complex/complex.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/complex/complex_base.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/complex/complex_base.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/complex/struct_type.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/complex/struct_type.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/concat.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/concat.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/cross_column_filter.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/cross_column_filter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/data_type_base.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/data_type_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,26 +226,26 @@
                 "
                 )
         """
         from spark_auto_mapper.data_types.expression import AutoMapperDataTypeExpression
 
         return cast(_TAutoMapperDataType, AutoMapperDataTypeExpression(value))
 
-    def current(self) -> _TAutoMapperDataType:
+    def current(self) -> _TAutoMapperDataType:  # type: ignore
         """
         Specifies to use the current item
 
         :param self: Set by Python.  No need to pass.
         :return: A column automapper type
         :example: A.column("last_name").current()
         """
         return self.field("_")
 
     # noinspection PyMethodMayBeStatic
-    def field(self, value: str) -> _TAutoMapperDataType:
+    def field(self, value: str) -> _TAutoMapperDataType:  # type: ignore
         """
         Specifies that the value parameter should be used as a field name
 
         :param self: Set by Python.  No need to pass.
         :param value: name of field
         :return: A column automapper type
         :example: A.column("identifier").select_one(A.field("type.coding[0].code"))
```

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/date.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/date.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/date_format.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/date_format.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/datetime.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/datetime.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/decimal.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/decimal.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/exists.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/exists.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/expression.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/expression.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/field.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/field.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/filter.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/filter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/first.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/first.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/first_valid_column.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/first_valid_column.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/flatten.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/flatten.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/float.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/float.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/hash.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/hash.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/if_.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/if_.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/if_column_exists.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/if_column_exists.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/if_not.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/if_not.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/if_not_null.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/if_not_null.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/if_not_null_or_empty.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/if_not_null_or_empty.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/if_regex.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/if_regex.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/join_using_delimiter.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/join_using_delimiter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/list.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/list.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/literal.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/literal.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/lpad.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/lpad.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/map.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/map.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/nested_array_filter.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/nested_array_filter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/null_if_empty.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/null_if_empty.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/null_remover.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/null_remover.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/number.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/number.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/regex_extract.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/regex_extract.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/regex_replace.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/regex_replace.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/split_by_delimiter.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/split_by_delimiter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/substring.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/substring.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/substring_by_delimiter.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/substring_by_delimiter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/text_like_base.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/text_like_base.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/to_json.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/to_json.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/transform.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/transform.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/trim.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/trim.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/data_types/unix_timestamp.py` & `sparkautomapper-2.0.1/spark_auto_mapper/data_types/unix_timestamp.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/helpers/automapper_helpers.py` & `sparkautomapper-2.0.1/spark_auto_mapper/helpers/automapper_helpers.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/helpers/capture_arguments.py` & `sparkautomapper-2.0.1/spark_auto_mapper/helpers/capture_arguments.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/helpers/expression_comparer.py` & `sparkautomapper-2.0.1/spark_auto_mapper/helpers/expression_comparer.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/helpers/python_keyword_cleaner.py` & `sparkautomapper-2.0.1/spark_auto_mapper/helpers/python_keyword_cleaner.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/helpers/value_parser.py` & `sparkautomapper-2.0.1/spark_auto_mapper/helpers/value_parser.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/type_definitions/defined_types.py` & `sparkautomapper-2.0.1/spark_auto_mapper/type_definitions/defined_types.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/type_definitions/native_types.py` & `sparkautomapper-2.0.1/spark_auto_mapper/type_definitions/native_types.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/spark_auto_mapper/type_definitions/wrapper_types.py` & `sparkautomapper-2.0.1/spark_auto_mapper/type_definitions/wrapper_types.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/sparkautomapper.egg-info/PKG-INFO` & `sparkautomapper-2.0.1/sparkautomapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkautomapper
-Version: 2.0.0
+Version: 2.0.1
 Summary: AutoMapper for Spark
 Home-page: https://github.com/imranq2/SparkAutoMapper
 Author: Imran Qureshi
 Author-email: imranq2@hotmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sparkautomapper-2.0.0/sparkautomapper.egg-info/SOURCES.txt` & `sparkautomapper-2.0.1/sparkautomapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/amount/test_automapper_amount.py` & `sparkautomapper-2.0.1/tests/amount/test_automapper_amount.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/amount/test_automapper_amount_typed.py` & `sparkautomapper-2.0.1/tests/amount/test_automapper_amount_typed.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/array/test_automapper_array_typed.py` & `sparkautomapper-2.0.1/tests/array/test_automapper_array_typed.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/array_distinct/test_automapper_array_distinct.py` & `sparkautomapper-2.0.1/tests/array_distinct/test_automapper_array_distinct.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/array_max/test_automapper_array_max.py` & `sparkautomapper-2.0.1/tests/array_max/test_automapper_array_max.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/base64/test_automapper_base64.py` & `sparkautomapper-2.0.1/tests/base64/test_automapper_base64.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/boolean/test_automapper_boolean.py` & `sparkautomapper-2.0.1/tests/boolean/test_automapper_boolean.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/boolean/test_automapper_boolean_typed.py` & `sparkautomapper-2.0.1/tests/boolean/test_automapper_boolean_typed.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/cast/test_cast.py` & `sparkautomapper-2.0.1/tests/cast/test_cast.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/cast_to_type/test_automapper_cast_to_type_typed.py` & `sparkautomapper-2.0.1/tests/cast_to_type/test_automapper_cast_to_type_typed.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/checkpointing/test_automapper_full_checkpointing.py` & `sparkautomapper-2.0.1/tests/checkpointing/test_automapper_full_checkpointing.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/coalesce/test_automapper_coalesce.py` & `sparkautomapper-2.0.1/tests/coalesce/test_automapper_coalesce.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/columns/test_automapper_columns.py` & `sparkautomapper-2.0.1/tests/columns/test_automapper_columns.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/complex/test_automapper_complex.py` & `sparkautomapper-2.0.1/tests/complex/test_automapper_complex.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/complex/test_automapper_complex_with_defined_class.py` & `sparkautomapper-2.0.1/tests/complex/test_automapper_complex_with_defined_class.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/complex/test_automapper_complex_with_extension.py` & `sparkautomapper-2.0.1/tests/complex/test_automapper_complex_with_extension.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/complex/test_automapper_complex_with_mappers.py` & `sparkautomapper-2.0.1/tests/complex/test_automapper_complex_with_mappers.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/complex/test_automapper_complex_with_skip_if_null.py` & `sparkautomapper-2.0.1/tests/complex/test_automapper_complex_with_skip_if_null.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/concat/test_automapper_add_array.py` & `sparkautomapper-2.0.1/tests/concat/test_automapper_add_array.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/concat/test_automapper_concat.py` & `sparkautomapper-2.0.1/tests/concat/test_automapper_concat.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/concat/test_automapper_concat_array.py` & `sparkautomapper-2.0.1/tests/concat/test_automapper_concat_array.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/concat/test_automapper_concat_multiple_items_structs_different_elements.py` & `sparkautomapper-2.0.1/tests/concat/test_automapper_concat_multiple_items_structs_different_elements.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/concat/test_automapper_concat_multiple_items_structs_different_elements_with_schema.py` & `sparkautomapper-2.0.1/tests/concat/test_automapper_concat_multiple_items_structs_different_elements_with_schema.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/conftest.py` & `sparkautomapper-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/copy_unmapped_properties/test_automapper_copy_unmapped_properties.py` & `sparkautomapper-2.0.1/tests/copy_unmapped_properties/test_automapper_copy_unmapped_properties.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/cross_column_filter/location.py` & `sparkautomapper-2.0.1/tests/cross_column_filter/location.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/cross_column_filter/test_cross_column_filter.py` & `sparkautomapper-2.0.1/tests/cross_column_filter/test_cross_column_filter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/date/test_automapper_date_column.py` & `sparkautomapper-2.0.1/tests/date/test_automapper_date_column.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/date/test_automapper_date_column_typed.py` & `sparkautomapper-2.0.1/tests/date/test_automapper_date_column_typed.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/date/test_automapper_date_literal.py` & `sparkautomapper-2.0.1/tests/date/test_automapper_date_literal.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/date_format/test_automapper_date_format.py` & `sparkautomapper-2.0.1/tests/date_format/test_automapper_date_format.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/decimal_type/test_automapper_decimal.py` & `sparkautomapper-2.0.1/tests/decimal_type/test_automapper_decimal.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/decimal_type/test_automapper_decimal_typed.py` & `sparkautomapper-2.0.1/tests/decimal_type/test_automapper_decimal_typed.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/duplicates_test/test_automapper_duplicates.py` & `sparkautomapper-2.0.1/tests/duplicates_test/test_automapper_duplicates.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/exists/test_automapper_exists.py` & `sparkautomapper-2.0.1/tests/exists/test_automapper_exists.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/field/test_automapper_field.py` & `sparkautomapper-2.0.1/tests/field/test_automapper_field.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/filter/test_automapper_filter.py` & `sparkautomapper-2.0.1/tests/filter/test_automapper_filter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/first/test_automapper_first.py` & `sparkautomapper-2.0.1/tests/first/test_automapper_first.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/first_valid_column/test_automapper_first_valid_column.py` & `sparkautomapper-2.0.1/tests/first_valid_column/test_automapper_first_valid_column.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/first_valid_column/test_automapper_first_valid_column_expressions.py` & `sparkautomapper-2.0.1/tests/first_valid_column/test_automapper_first_valid_column_expressions.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/flatten/test_automapper_flatten.py` & `sparkautomapper-2.0.1/tests/flatten/test_automapper_flatten.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/flatten/test_automapper_flatten_with_null.py` & `sparkautomapper-2.0.1/tests/flatten/test_automapper_flatten_with_null.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/hash/test_automapper_hash.py` & `sparkautomapper-2.0.1/tests/hash/test_automapper_hash.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/if_/test_automapper_if_.py` & `sparkautomapper-2.0.1/tests/if_/test_automapper_if_.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/if_/test_automapper_if_list.py` & `sparkautomapper-2.0.1/tests/if_/test_automapper_if_list.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/if_column_exists/test_automapper_if_column_exists.py` & `sparkautomapper-2.0.1/tests/if_column_exists/test_automapper_if_column_exists.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/if_not/test_automapper_if_not.py` & `sparkautomapper-2.0.1/tests/if_not/test_automapper_if_not.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/if_not/test_automapper_if_not_list.py` & `sparkautomapper-2.0.1/tests/if_not/test_automapper_if_not_list.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/if_not_null/test_automapper_if_not_null.py` & `sparkautomapper-2.0.1/tests/if_not_null/test_automapper_if_not_null.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/if_not_null_or_empty/test_automapper_if_not_null_or_empty.py` & `sparkautomapper-2.0.1/tests/if_not_null_or_empty/test_automapper_if_not_null_or_empty.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/if_regex/test_automapper_if_regex.py` & `sparkautomapper-2.0.1/tests/if_regex/test_automapper_if_regex.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/join_using_delimiter/test_automapper_join_using_delimiter.py` & `sparkautomapper-2.0.1/tests/join_using_delimiter/test_automapper_join_using_delimiter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/left/test_automapper_left.py` & `sparkautomapper-2.0.1/tests/left/test_automapper_left.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements.py` & `sparkautomapper-2.0.1/tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements_with_schema.py` & `sparkautomapper-2.0.1/tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements_with_schema.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/list/test_automapper_list_multiple_items.py` & `sparkautomapper-2.0.1/tests/list/test_automapper_list_multiple_items.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/list/test_automapper_list_multiple_items_structs.py` & `sparkautomapper-2.0.1/tests/list/test_automapper_list_multiple_items_structs.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/list/test_automapper_list_multiple_items_structs_different_elements.py` & `sparkautomapper-2.0.1/tests/list/test_automapper_list_multiple_items_structs_different_elements.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/list/test_automapper_list_multiple_items_structs_different_elements_with_schema.py` & `sparkautomapper-2.0.1/tests/list/test_automapper_list_multiple_items_structs_different_elements_with_schema.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/list/test_automapper_list_multiple_items_with_null.py` & `sparkautomapper-2.0.1/tests/list/test_automapper_list_multiple_items_with_null.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/list/test_automapper_list_single_item.py` & `sparkautomapper-2.0.1/tests/list/test_automapper_list_single_item.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/list/test_automapper_list_single_item_with_mapper.py` & `sparkautomapper-2.0.1/tests/list/test_automapper_list_single_item_with_mapper.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/lpad/test_auto_mapper_lpad.py` & `sparkautomapper-2.0.1/tests/lpad/test_auto_mapper_lpad.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/map/test_automapper_map.py` & `sparkautomapper-2.0.1/tests/map/test_automapper_map.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/map/test_automapper_map_col_default.py` & `sparkautomapper-2.0.1/tests/map/test_automapper_map_col_default.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/map/test_automapper_map_no_default.py` & `sparkautomapper-2.0.1/tests/map/test_automapper_map_no_default.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/map/test_automapper_map_null.py` & `sparkautomapper-2.0.1/tests/map/test_automapper_map_null.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/multiple_columns/test_automapper_multiple_columns.py` & `sparkautomapper-2.0.1/tests/multiple_columns/test_automapper_multiple_columns.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/multiple_columns/test_automapper_multiple_columns_simpler_syntax.py` & `sparkautomapper-2.0.1/tests/multiple_columns/test_automapper_multiple_columns_simpler_syntax.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/nested_array_filter/location.py` & `sparkautomapper-2.0.1/tests/nested_array_filter/location.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/nested_array_filter/schedule.py` & `sparkautomapper-2.0.1/tests/nested_array_filter/schedule.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/nested_array_filter/simple/test_automapper_nested_array_filter_simple.py` & `sparkautomapper-2.0.1/tests/nested_array_filter/simple/test_automapper_nested_array_filter_simple.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/nested_array_filter/simple_with_array/test_automapper_nested_array_filter_simple_with_array.py` & `sparkautomapper-2.0.1/tests/nested_array_filter/simple_with_array/test_automapper_nested_array_filter_simple_with_array.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/nested_array_filter/test_automapper_nested_array_filter.py` & `sparkautomapper-2.0.1/tests/nested_array_filter/test_automapper_nested_array_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
                 struct(
                     l["name"].alias("name"),
                     transform(
                         filter(
                             col("b.schedule"),
                             lambda s: exists(
                                 s["actor"],
-                                lambda a: a["reference"] == l["name"],  # type: ignore
+                                lambda a: a["reference"] == l["name"],
                             ),
                         ),
                         lambda s: struct(s["name"].alias("name")),
                     )[0].alias("scheduling"),
                 )
             ),
         ).alias("___location"),
```

### Comparing `sparkautomapper-2.0.0/tests/nested_array_filter/test_automapper_nested_array_filter_expression_only.py` & `sparkautomapper-2.0.1/tests/nested_array_filter/test_automapper_nested_array_filter_expression_only.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             struct(
                 l["name"].alias("name"),
                 transform(
                     filter(
                         col("schedule"),
                         lambda s: exists(
                             s["actor"],
-                            lambda a: a["reference"] == l["name"],  # type: ignore
+                            lambda a: a["reference"] == l["name"],
                         ),
                     ),
                     lambda s: struct(s["name"].alias("name")),
                 )[0].alias("scheduling"),
             )
         ),
     )
```

### Comparing `sparkautomapper-2.0.0/tests/null_if_empty/test_automapper_null_if_empty.py` & `sparkautomapper-2.0.1/tests/null_if_empty/test_automapper_null_if_empty.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/null_remover/test_automapper_null_remover.py` & `sparkautomapper-2.0.1/tests/null_remover/test_automapper_null_remover.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/number/test_automapper_number.py` & `sparkautomapper-2.0.1/tests/number/test_automapper_number.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/number/test_automapper_number_typed.py` & `sparkautomapper-2.0.1/tests/number/test_automapper_number_typed.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/regex_extract/test_auto_mapper_regex_extract.py` & `sparkautomapper-2.0.1/tests/regex_extract/test_auto_mapper_regex_extract.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/regex_replace/test_auto_mapper_regex_replace.py` & `sparkautomapper-2.0.1/tests/regex_replace/test_auto_mapper_regex_replace.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/regex_replace/test_auto_mapper_regex_replace_unicode.py` & `sparkautomapper-2.0.1/tests/regex_replace/test_auto_mapper_regex_replace_unicode.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/right/test_automapper_right.py` & `sparkautomapper-2.0.1/tests/right/test_automapper_right.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/sanitize/test_auto_mapper_sanitize.py` & `sparkautomapper-2.0.1/tests/sanitize/test_auto_mapper_sanitize.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/schema_pruning/test_automapper_schema_pruning_with_defined_class.py` & `sparkautomapper-2.0.1/tests/schema_pruning/test_automapper_schema_pruning_with_defined_class.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/schema_pruning/test_automapper_schema_pruning_with_extension.py` & `sparkautomapper-2.0.1/tests/schema_pruning/test_automapper_schema_pruning_with_extension.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/schema_pruning/test_automapper_schema_pruning_with_extension_different_properties.py` & `sparkautomapper-2.0.1/tests/schema_pruning/test_automapper_schema_pruning_with_extension_different_properties.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/select_one/test_automapper_select_one.py` & `sparkautomapper-2.0.1/tests/select_one/test_automapper_select_one.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/split_by_delimiter/test_automapper_split_by_delimiter.py` & `sparkautomapper-2.0.1/tests/split_by_delimiter/test_automapper_split_by_delimiter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/split_by_delimiter/test_automapper_split_by_delimiter_and_transform.py` & `sparkautomapper-2.0.1/tests/split_by_delimiter/test_automapper_split_by_delimiter_and_transform.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/split_by_delimiter/test_automapper_split_by_delimiter_and_transform_fluent.py` & `sparkautomapper-2.0.1/tests/split_by_delimiter/test_automapper_split_by_delimiter_and_transform_fluent.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/string_after_delimiter/test_automapper_string_after_delimiter.py` & `sparkautomapper-2.0.1/tests/string_after_delimiter/test_automapper_string_after_delimiter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/string_before_delimiter/test_automapper_string_before_delimiter.py` & `sparkautomapper-2.0.1/tests/string_before_delimiter/test_automapper_string_before_delimiter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/struct_type/test_automapper_struct.py` & `sparkautomapper-2.0.1/tests/struct_type/test_automapper_struct.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/struct_type/test_automapper_struct_with_mappers.py` & `sparkautomapper-2.0.1/tests/struct_type/test_automapper_struct_with_mappers.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/substring_by_delimiter/test_automapper_substring_by_delimiter.py` & `sparkautomapper-2.0.1/tests/substring_by_delimiter/test_automapper_substring_by_delimiter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/test_automapper_full.py` & `sparkautomapper-2.0.1/tests/test_automapper_full.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/test_automapper_full_no_keys.py` & `sparkautomapper-2.0.1/tests/test_automapper_full_no_keys.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/test_automapper_full_no_views.py` & `sparkautomapper-2.0.1/tests/test_automapper_full_no_views.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/test_automapper_full_view_exists.py` & `sparkautomapper-2.0.1/tests/test_automapper_full_view_exists.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/to_json/test_automapper_to_json.py` & `sparkautomapper-2.0.1/tests/to_json/test_automapper_to_json.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/transform/test_automapper_filter_and_transform.py` & `sparkautomapper-2.0.1/tests/transform/test_automapper_filter_and_transform.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/transform/test_automapper_filter_and_transform_fluent.py` & `sparkautomapper-2.0.1/tests/transform/test_automapper_filter_and_transform_fluent.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/transform/test_automapper_transform.py` & `sparkautomapper-2.0.1/tests/transform/test_automapper_transform.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/trim/test_auto_mapper_trim.py` & `sparkautomapper-2.0.1/tests/trim/test_auto_mapper_trim.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/unix_timestamp/test_automapper_unix_timestamp.py` & `sparkautomapper-2.0.1/tests/unix_timestamp/test_automapper_unix_timestamp.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/unix_timestamp/test_automapper_unix_timestamp_literal.py` & `sparkautomapper-2.0.1/tests/unix_timestamp/test_automapper_unix_timestamp_literal.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/unix_timestamp/test_automapper_unix_timestamp_string.py` & `sparkautomapper-2.0.1/tests/unix_timestamp/test_automapper_unix_timestamp_string.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/withColumn/test_automapper_with_column.py` & `sparkautomapper-2.0.1/tests/withColumn/test_automapper_with_column.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/withColumn/test_automapper_with_column_expression.py` & `sparkautomapper-2.0.1/tests/withColumn/test_automapper_with_column_expression.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/withColumn/test_automapper_with_column_literal.py` & `sparkautomapper-2.0.1/tests/withColumn/test_automapper_with_column_literal.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.0/tests/withColumn/test_automapper_with_filter.py` & `sparkautomapper-2.0.1/tests/withColumn/test_automapper_with_filter.py`

 * *Files identical despite different names*

