# Comparing `tmp/sqlconstructor-1.0.26.tar.gz` & `tmp/sqlconstructor-1.0.27.tar.gz`

## Comparing `sqlconstructor-1.0.26.tar` & `sqlconstructor-1.0.27.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/pytest.ini
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/src/sqlconstructor/__init__.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/src/sqlconstructor/cols.py
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/src/sqlconstructor/constants.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/src/sqlconstructor/helpers.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/src/sqlconstructor/sql_container.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/src/sqlconstructor/sql_cte.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/src/sqlconstructor/sql_enum.py
--rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/src/sqlconstructor/sql_query.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/src/sqlconstructor/sql_section.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/src/sqlconstructor/vals.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/fixtures/simple_query_dict.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/fixtures/expected_examples/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/fixtures/expected_examples/insert_into_inline_using_cols.sql
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/fixtures/expected_examples/insert_into_inline_using_sqlenum.sql
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/fixtures/expected_examples/insert_into_multiline_using_cols.sql
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/fixtures/expected_examples/insert_into_multiline_using_sqlenum.sql
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/fixtures/expected_examples/select_section_of_simple_query.sql
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/fixtures/expected_examples/simple_query.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_container/__init__.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_container/test_bool.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_container/test_container_filled_by_section_call.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_container/test_del_vars.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_container/test_init.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_container/test_json_variable.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_container/test_reset_vars.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_container/test_set_vars.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_container/test_unwrap.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_container/test_wrap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_cte/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_cte/test_call.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_cte/test_clear.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_cte/test_delitem.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_cte/test_getitem.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_cte/test_init.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_cte/test_iter.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_cte/test_pop.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_cte/test_reg.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_cte/test_setitem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_query/__init__.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_query/test_add.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_query/test_bool.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_query/test_building_process.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_query/test_call.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_query/test_init.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_query/test_iter.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_query/test_len.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_query/test_sections_pop.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_query/test_cases/__init__.py
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_query/test_cases/test_insert_into.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_section/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_section/test_bool.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_section/test_call.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_section/test_init.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/tests/test_sql_section/test_upper_sql_keywords.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/LICENSE
--rw-r--r--   0        0        0    10627 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/pyproject.toml
--rw-r--r--   0        0        0    11428 2020-02-02 00:00:00.000000 sqlconstructor-1.0.26/PKG-INFO
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/pytest.ini
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/src/sqlconstructor/__init__.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/src/sqlconstructor/cols.py
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/src/sqlconstructor/constants.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/src/sqlconstructor/helpers.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/src/sqlconstructor/sql_container.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/src/sqlconstructor/sql_cte.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/src/sqlconstructor/sql_enum.py
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/src/sqlconstructor/sql_query.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/src/sqlconstructor/sql_section.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/src/sqlconstructor/vals.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/fixtures/simple_query_dict.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/fixtures/expected_examples/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/fixtures/expected_examples/insert_into_inline_using_cols.sql
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/fixtures/expected_examples/insert_into_inline_using_sqlenum.sql
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/fixtures/expected_examples/insert_into_multiline_using_cols.sql
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/fixtures/expected_examples/insert_into_multiline_using_sqlenum.sql
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/fixtures/expected_examples/select_section_of_simple_query.sql
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/fixtures/expected_examples/simple_query.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_container/__init__.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_container/test_bool.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_container/test_container_filled_by_section_call.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_container/test_del_vars.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_container/test_init.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_container/test_json_variable.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_container/test_reset_vars.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_container/test_set_vars.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_container/test_unwrap.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_container/test_wrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_cte/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_cte/test_call.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_cte/test_clear.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_cte/test_delitem.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_cte/test_getitem.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_cte/test_init.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_cte/test_iter.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_cte/test_pop.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_cte/test_reg.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_cte/test_setitem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_query/__init__.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_query/test_add.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_query/test_bool.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_query/test_building_process.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_query/test_call.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_query/test_init.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_query/test_iter.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_query/test_len.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_query/test_sections_pop.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_query/test_cases/__init__.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_query/test_cases/test_insert_into.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_section/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_section/test_bool.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_section/test_call.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_section/test_init.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/tests/test_sql_section/test_upper_sql_keywords.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/LICENSE
+-rw-r--r--   0        0        0    10632 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/pyproject.toml
+-rw-r--r--   0        0        0    11433 2020-02-02 00:00:00.000000 sqlconstructor-1.0.27/PKG-INFO
```

### Comparing `sqlconstructor-1.0.26/src/sqlconstructor/cols.py` & `sqlconstructor-1.0.27/src/sqlconstructor/cols.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/src/sqlconstructor/constants.py` & `sqlconstructor-1.0.27/src/sqlconstructor/constants.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/src/sqlconstructor/helpers.py` & `sqlconstructor-1.0.27/src/sqlconstructor/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/src/sqlconstructor/sql_container.py` & `sqlconstructor-1.0.27/src/sqlconstructor/sql_container.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/src/sqlconstructor/sql_cte.py` & `sqlconstructor-1.0.27/src/sqlconstructor/sql_cte.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/src/sqlconstructor/sql_enum.py` & `sqlconstructor-1.0.27/src/sqlconstructor/sql_enum.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/src/sqlconstructor/sql_query.py` & `sqlconstructor-1.0.27/src/sqlconstructor/sql_query.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/src/sqlconstructor/sql_section.py` & `sqlconstructor-1.0.27/src/sqlconstructor/sql_section.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/src/sqlconstructor/vals.py` & `sqlconstructor-1.0.27/src/sqlconstructor/vals.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/fixtures/simple_query_dict.py` & `sqlconstructor-1.0.27/tests/fixtures/simple_query_dict.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/fixtures/expected_examples/__init__.py` & `sqlconstructor-1.0.27/tests/fixtures/expected_examples/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/test_sql_container/test_bool.py` & `sqlconstructor-1.0.27/tests/test_sql_container/test_bool.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/test_sql_container/test_del_vars.py` & `sqlconstructor-1.0.27/tests/test_sql_container/test_del_vars.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/test_sql_container/test_init.py` & `sqlconstructor-1.0.27/tests/test_sql_container/test_init.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/test_sql_container/test_reset_vars.py` & `sqlconstructor-1.0.27/tests/test_sql_container/test_reset_vars.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/test_sql_container/test_set_vars.py` & `sqlconstructor-1.0.27/tests/test_sql_container/test_set_vars.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/test_sql_cte/test_call.py` & `sqlconstructor-1.0.27/tests/test_sql_cte/test_call.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/test_sql_cte/test_iter.py` & `sqlconstructor-1.0.27/tests/test_sql_cte/test_iter.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/test_sql_cte/test_pop.py` & `sqlconstructor-1.0.27/tests/test_sql_cte/test_pop.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/test_sql_query/test_add.py` & `sqlconstructor-1.0.27/tests/test_sql_query/test_add.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/test_sql_query/test_building_process.py` & `sqlconstructor-1.0.27/tests/test_sql_query/test_building_process.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/test_sql_query/test_call.py` & `sqlconstructor-1.0.27/tests/test_sql_query/test_call.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/test_sql_query/test_init.py` & `sqlconstructor-1.0.27/tests/test_sql_query/test_init.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/test_sql_query/test_sections_pop.py` & `sqlconstructor-1.0.27/tests/test_sql_query/test_sections_pop.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/test_sql_query/test_cases/test_insert_into.py` & `sqlconstructor-1.0.27/tests/test_sql_query/test_cases/test_insert_into.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/test_sql_section/test_init.py` & `sqlconstructor-1.0.27/tests/test_sql_section/test_init.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/tests/test_sql_section/test_upper_sql_keywords.py` & `sqlconstructor-1.0.27/tests/test_sql_section/test_upper_sql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/LICENSE` & `sqlconstructor-1.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.26/README.md` & `sqlconstructor-1.0.27/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -403,15 +403,15 @@
 VALUES
   (
     1,
     'phone',
     '82611533-25c4-4cbd-8497-3f5024ca29a1'
   )
 ```
-If you would like to do not add double quotes to columns then you could use SqlEnum class. Any of this class(SqlEnum, Vals, Cols) has inline and multiline method (return SqlContainer which you could wrap by 'wrap' method or do not wrap) in release >= 1.0.24.
+If you would like to do not add double quotes to columns then you could use SqlEnum class. Any of this class (SqlEnum, Vals, Cols) has 'inline' and 'multiline' method (return SqlContainer which you could wrap by 'wrap' method or do not wrap) in release >= 1.0.24.
 Example:
 ```python
 import uuid
 from sqlconstructor import SqlQuery, SqlEnum, Vals
 
 
 q = SqlQuery()
```

### Comparing `sqlconstructor-1.0.26/pyproject.toml` & `sqlconstructor-1.0.27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sqlconstructor"
-version = "1.0.26"
+version = "1.0.27"
 authors = [
   { name="Andrey Smirnov", email="abc-sm@yandex.ru" },
 ]
 description = "Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sqlconstructor-1.0.26/PKG-INFO` & `sqlconstructor-1.0.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlconstructor
-Version: 1.0.26
+Version: 1.0.27
 Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!
 Project-URL: Homepage, https://github.com/akvilary/sqlconstructor
 Project-URL: Bug Tracker, https://github.com/akvilary/sqlconstructor/issues
 Project-URL: Telegram, https://t.me/sqlconstructor
 Author-email: Andrey Smirnov <abc-sm@yandex.ru>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -418,15 +418,15 @@
 VALUES
   (
     1,
     'phone',
     '82611533-25c4-4cbd-8497-3f5024ca29a1'
   )
 ```
-If you would like to do not add double quotes to columns then you could use SqlEnum class. Any of this class(SqlEnum, Vals, Cols) has inline and multiline method (return SqlContainer which you could wrap by 'wrap' method or do not wrap) in release >= 1.0.24.
+If you would like to do not add double quotes to columns then you could use SqlEnum class. Any of this class (SqlEnum, Vals, Cols) has 'inline' and 'multiline' method (return SqlContainer which you could wrap by 'wrap' method or do not wrap) in release >= 1.0.24.
 Example:
 ```python
 import uuid
 from sqlconstructor import SqlQuery, SqlEnum, Vals
 
 
 q = SqlQuery()
```

