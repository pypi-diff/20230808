# Comparing `tmp/Warg-1.1.8.tar.gz` & `tmp/Warg-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Warg-1.1.8.tar", last modified: Tue Aug  1 06:11:34 2023, max compression
+gzip compressed data, was "Warg-1.1.9.tar", last modified: Tue Aug  8 07:18:50 2023, max compression
```

## Comparing `Warg-1.1.8.tar` & `Warg-1.1.9.tar`

### file list

```diff
@@ -1,134 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.234342 Warg-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.218341 Warg-1.1.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-08-01 06:11:28.000000 Warg-1.1.8/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:28.000000 Warg-1.1.8/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 06:11:28.000000 Warg-1.1.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:11:28.000000 Warg-1.1.8/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-08-01 06:11:28.000000 Warg-1.1.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-01 06:11:28.000000 Warg-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-08-01 06:11:34.234342 Warg-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-08-01 06:11:28.000000 Warg-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-01 06:11:28.000000 Warg-1.1.8/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.218341 Warg-1.1.8/Warg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-08-01 06:11:34.000000 Warg-1.1.8/Warg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-08-01 06:11:34.000000 Warg-1.1.8/Warg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:11:34.000000 Warg-1.1.8/Warg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-01 06:11:34.000000 Warg-1.1.8/Warg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 06:11:34.000000 Warg-1.1.8/Warg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.218341 Warg-1.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 06:11:28.000000 Warg-1.1.8/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-01 06:11:28.000000 Warg-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 06:11:28.000000 Warg-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-01 06:11:34.234342 Warg-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-08-01 06:11:28.000000 Warg-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.222341 Warg-1.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_ast_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_auto_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_collective.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_gdkc.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_kw_passing.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_nod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_post_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.222341 Warg-1.1.8/warg/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.226342 Warg-1.1.8/warg/ast_ops/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/ast_ops/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/ast_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/ast_ops/arg_indentifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/ast_ops/first_arg_identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.226342 Warg-1.1.8/warg/bases/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/bases/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/bases/property_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/boolean_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/business.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.226342 Warg-1.1.8/warg/colors/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/colors/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/colors/color_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/colors/css_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/colors/label_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/config_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/context_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/contexts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.226342 Warg-1.1.8/warg/data_structures/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/data_structures/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/data_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/data_structures/auto_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/data_structures/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16665 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/data_structures/named_ordered_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    28783 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/data_structures/ordered_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/data_structures/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/datetimes.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.226342 Warg-1.1.8/warg/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.230342 Warg-1.1.8/warg/decorators/caching/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/caching/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/caching/look_up_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/caching/property_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/exporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/kw_passing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/wrapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/gdkc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.230342 Warg-1.1.8/warg/generators/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/generators/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/generators/cyclic_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/generators/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/generators/mapping_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/generators/numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/generators/zipping_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/map_itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.230342 Warg-1.1.8/warg/math_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/math_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/math_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/math_utilities/multiples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/math_utilities/ordinals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/math_utilities/powers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.230342 Warg-1.1.8/warg/metas/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/metas/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/metas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/metas/post_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/metas/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.230342 Warg-1.1.8/warg/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/mixins/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/mixins/dict_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/mixins/ordinal_index_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/mixins/private.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/ode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.234342 Warg-1.1.8/warg/os_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/os_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/os_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/os_utilities/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/os_utilities/os_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/os_utilities/path_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/os_utilities/path_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/os_utilities/platform_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.234342 Warg-1.1.8/warg/packages/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/packages/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/packages/editable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/packages/pip_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/packages/reloading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/replication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/styling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/typing_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.892087 Warg-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.868086 Warg-1.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-08-08 07:18:41.000000 Warg-1.1.9/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:41.000000 Warg-1.1.9/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-08 07:18:41.000000 Warg-1.1.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 07:18:42.000000 Warg-1.1.9/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-08-08 07:18:42.000000 Warg-1.1.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-08 07:18:42.000000 Warg-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-08-08 07:18:50.892087 Warg-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-08-08 07:18:42.000000 Warg-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-08 07:18:42.000000 Warg-1.1.9/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.872086 Warg-1.1.9/Warg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-08-08 07:18:50.000000 Warg-1.1.9/Warg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-08 07:18:50.000000 Warg-1.1.9/Warg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:18:50.000000 Warg-1.1.9/Warg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-08 07:18:50.000000 Warg-1.1.9/Warg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 07:18:50.000000 Warg-1.1.9/Warg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.872086 Warg-1.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-08 07:18:42.000000 Warg-1.1.9/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-08 07:18:42.000000 Warg-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 07:18:42.000000 Warg-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-08 07:18:50.892087 Warg-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-08-08 07:18:42.000000 Warg-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.872086 Warg-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-08 07:18:42.000000 Warg-1.1.9/tests/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-08 07:18:42.000000 Warg-1.1.9/tests/test_ast_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-08 07:18:42.000000 Warg-1.1.9/tests/test_auto_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-08 07:18:42.000000 Warg-1.1.9/tests/test_collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-08 07:18:42.000000 Warg-1.1.9/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-08 07:18:42.000000 Warg-1.1.9/tests/test_gdkc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-08 07:18:42.000000 Warg-1.1.9/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-08-08 07:18:42.000000 Warg-1.1.9/tests/test_kw_passing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-08 07:18:42.000000 Warg-1.1.9/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-08-08 07:18:42.000000 Warg-1.1.9/tests/test_nod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-08 07:18:42.000000 Warg-1.1.9/tests/test_post_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-08 07:18:42.000000 Warg-1.1.9/tests/test_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.880086 Warg-1.1.9/warg/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.880086 Warg-1.1.9/warg/ast_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/ast_ops/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/ast_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/ast_ops/arg_indentifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/ast_ops/first_arg_identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.880086 Warg-1.1.9/warg/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/bases/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/bases/property_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/boolean_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/business.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.880086 Warg-1.1.9/warg/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/colors/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/colors/color_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/colors/css_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/colors/label_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/config_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/context_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/contexts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.880086 Warg-1.1.9/warg/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/data_structures/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/data_structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/data_structures/auto_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/data_structures/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16665 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/data_structures/named_ordered_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28783 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/data_structures/ordered_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/data_structures/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/datetimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.884086 Warg-1.1.9/warg/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/decorators/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.884086 Warg-1.1.9/warg/decorators/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/decorators/caching/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/decorators/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/decorators/caching/look_up_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/decorators/caching/property_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/decorators/exporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/decorators/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/decorators/kw_passing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/decorators/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/decorators/wrapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/gdkc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.888086 Warg-1.1.9/warg/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/generators/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/generators/cyclic_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/generators/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/generators/mapping_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/generators/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/generators/zipping_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/map_itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.888086 Warg-1.1.9/warg/math_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/math_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/math_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/math_utilities/multiples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/math_utilities/ordinals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/math_utilities/powers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.888086 Warg-1.1.9/warg/metas/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/metas/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/metas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/metas/post_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/metas/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.888086 Warg-1.1.9/warg/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/mixins/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/mixins/dict_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/mixins/ordinal_index_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/mixins/private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/ode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.892087 Warg-1.1.9/warg/os_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/os_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/os_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/os_utilities/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/os_utilities/os_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/os_utilities/path_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/os_utilities/path_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/os_utilities/platform_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:18:50.892087 Warg-1.1.9/warg/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/packages/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/packages/editable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/packages/pip_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/packages/reloading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/styling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-08 07:18:42.000000 Warg-1.1.9/warg/typing_extension.py
```

### Comparing `Warg-1.1.8/.github/CODE_OF_CONDUCT.md` & `Warg-1.1.9/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/LICENSE.md` & `Warg-1.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/PKG-INFO` & `Warg-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Warg
-Version: 1.1.8
+Version: 1.1.9
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/warg
 Download-URL: https://github.com/pything/warg/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -19,18 +19,18 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: setup
+Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![warg](.github/images/warg.svg)-->
 
 <p align="center">
   <img src=".github/images/warg.svg" alt='Warg' />
```

### Comparing `Warg-1.1.8/README.md` & `Warg-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/SECURITY.md` & `Warg-1.1.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/Warg.egg-info/PKG-INFO` & `Warg-1.1.9/Warg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Warg
-Version: 1.1.8
+Version: 1.1.9
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/warg
 Download-URL: https://github.com/pything/warg/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -19,18 +19,18 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: setup
+Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![warg](.github/images/warg.svg)-->
 
 <p align="center">
   <img src=".github/images/warg.svg" alt='Warg' />
```

### Comparing `Warg-1.1.8/Warg.egg-info/SOURCES.txt` & `Warg-1.1.9/Warg.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 warg/context_wrapper.py
 warg/contexts.py
 warg/datetimes.py
 warg/debug.py
 warg/exceptions.py
 warg/functions.py
 warg/gdkc.py
+warg/iteration.py
 warg/manipulation.py
 warg/map_itertools.py
 warg/ode.py
 warg/plugin.py
 warg/replication.py
 warg/strings.py
 warg/styling.py
```

### Comparing `Warg-1.1.8/Warg.egg-info/requires.txt` & `Warg-1.1.9/Warg.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 setuptools>=60.9.3
 
 [all]
-pytest>=4.3.0
-sphinx
-tox
-sphinxcontrib-programoutput
 pytest-cov>=2.6.1
+apppath
+twine>=1.13.0
+black>=18.9b0
+tox
 pip>=19.0.3
-coveralls>=1.6.0
+pytest>=4.3.0
 wheel>=0.33.0
 pytest-runner
 setuptools>=60.9.3
-twine>=1.13.0
-black>=18.9b0
-apppath
 warg
-
-[dev]
-pytest>=4.3.0
 sphinx
-tox
-pip>=19.0.3
-warg
 coveralls>=1.6.0
-wheel>=0.33.0
+sphinxcontrib-programoutput
+
+[dev]
+pytest-cov>=2.6.1
 apppath
-pytest-runner
-setuptools>=60.9.3
 twine>=1.13.0
 black>=18.9b0
+pip>=19.0.3
+tox
+pytest>=4.3.0
+wheel>=0.33.0
+setuptools>=60.9.3
+pytest-runner
+warg
+sphinx
+coveralls>=1.6.0
 sphinxcontrib-programoutput
-pytest-cov>=2.6.1
 
 [docs]
-sphinx
-sphinxcontrib-programoutput
 apppath
 warg
+sphinx
+sphinxcontrib-programoutput
 
 [setup]
 pytest-runner
 
 [tests]
-pytest>=4.3.0
-tox
 pytest-cov>=2.6.1
+tox
+pytest>=4.3.0
```

### Comparing `Warg-1.1.8/pyproject.toml` & `Warg-1.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/setup.py` & `Warg-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/tests/test_arguments.py` & `Warg-1.1.9/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/tests/test_ast_ops.py` & `Warg-1.1.9/tests/test_ast_ops.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/tests/test_auto_dict.py` & `Warg-1.1.9/tests/test_auto_dict.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/tests/test_collective.py` & `Warg-1.1.9/tests/test_collective.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/tests/test_gdkc.py` & `Warg-1.1.9/tests/test_gdkc.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/tests/test_imports.py` & `Warg-1.1.9/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/tests/test_kw_passing.py` & `Warg-1.1.9/tests/test_kw_passing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/tests/test_nod.py` & `Warg-1.1.9/tests/test_nod.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/tests/test_post_init.py` & `Warg-1.1.9/tests/test_post_init.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/tests/test_singleton.py` & `Warg-1.1.9/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/__init__.py` & `Warg-1.1.9/warg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from importlib import resources
 from importlib.metadata import Distribution, PackageNotFoundError
 from warnings import warn
 
 __project__ = "Warg"
 
 __author__ = "Christian Heider Nielsen"
-__version__ = "1.1.8"
+__version__ = "1.1.9"
 __doc__ = r"""
 Created on 27/04/2019
 
 @author: cnheider
 
 """
 
@@ -57,14 +57,15 @@
     from .replication import *
     from .styling import *
     from .strings import *
     from .contexts import *
     from .config_shell import *
     from .colors import *
     from .packages import *
+    from .iteration import *
 except ImportError as ix:
     this_package_name = Path(__file__).parent.name
     this_package_reqs = Path(__file__).parent.parent / f"requirements.txt"
     if this_package_reqs.exists():
         print(
             f"Make sure requirements is installed for {this_package_name}, see {this_package_reqs}"
         )  # TODO: PARSE WHAT is missing and print
```

### Comparing `Warg-1.1.8/warg/arguments.py` & `Warg-1.1.9/warg/arguments.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/ast_ops/arg_indentifier.py` & `Warg-1.1.9/warg/ast_ops/arg_indentifier.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/ast_ops/first_arg_identifier.py` & `Warg-1.1.9/warg/ast_ops/first_arg_identifier.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/bases/property_settings.py` & `Warg-1.1.9/warg/bases/property_settings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/boolean_tests.py` & `Warg-1.1.9/warg/boolean_tests.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/business.py` & `Warg-1.1.9/warg/business.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/colors/color_conversion.py` & `Warg-1.1.9/warg/colors/color_conversion.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/colors/css_colors.py` & `Warg-1.1.9/warg/colors/css_colors.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/colors/label_colors.py` & `Warg-1.1.9/warg/colors/label_colors.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/config_shell.py` & `Warg-1.1.9/warg/config_shell.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/context_wrapper.py` & `Warg-1.1.9/warg/context_wrapper.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/contexts.py` & `Warg-1.1.9/warg/contexts.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/data_structures/auto_dict.py` & `Warg-1.1.9/warg/data_structures/auto_dict.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/data_structures/mappings.py` & `Warg-1.1.9/warg/data_structures/mappings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/data_structures/named_ordered_dictionary.py` & `Warg-1.1.9/warg/data_structures/named_ordered_dictionary.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/data_structures/ordered_set.py` & `Warg-1.1.9/warg/data_structures/ordered_set.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/data_structures/sequences.py` & `Warg-1.1.9/warg/data_structures/sequences.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/datetimes.py` & `Warg-1.1.9/warg/datetimes.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/debug.py` & `Warg-1.1.9/warg/debug.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/decorators/caching/look_up_table.py` & `Warg-1.1.9/warg/decorators/caching/look_up_table.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/decorators/caching/property_caching.py` & `Warg-1.1.9/warg/decorators/caching/property_caching.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/decorators/exporting.py` & `Warg-1.1.9/warg/decorators/exporting.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/decorators/hashing.py` & `Warg-1.1.9/warg/decorators/hashing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/decorators/kw_passing.py` & `Warg-1.1.9/warg/decorators/kw_passing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/decorators/timing.py` & `Warg-1.1.9/warg/decorators/timing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/decorators/wrapping.py` & `Warg-1.1.9/warg/decorators/wrapping.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/exceptions.py` & `Warg-1.1.9/warg/exceptions.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/functions.py` & `Warg-1.1.9/warg/functions.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/gdkc.py` & `Warg-1.1.9/warg/gdkc.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/generators/cyclic_generators.py` & `Warg-1.1.9/warg/generators/cyclic_generators.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/generators/filtering.py` & `Warg-1.1.9/warg/generators/filtering.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/generators/mapping_generator.py` & `Warg-1.1.9/warg/generators/mapping_generator.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/generators/numbers.py` & `Warg-1.1.9/warg/generators/numbers.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/generators/zipping_generator.py` & `Warg-1.1.9/warg/generators/zipping_generator.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/manipulation.py` & `Warg-1.1.9/warg/manipulation.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/map_itertools.py` & `Warg-1.1.9/warg/map_itertools.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/math_utilities/ordinals.py` & `Warg-1.1.9/warg/math_utilities/ordinals.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/math_utilities/powers.py` & `Warg-1.1.9/warg/math_utilities/powers.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/metas/post_init.py` & `Warg-1.1.9/warg/metas/post_init.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/metas/singleton.py` & `Warg-1.1.9/warg/metas/singleton.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/mixins/dict_mixins.py` & `Warg-1.1.9/warg/mixins/dict_mixins.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/mixins/ordinal_index_mixin.py` & `Warg-1.1.9/warg/mixins/ordinal_index_mixin.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/ode.py` & `Warg-1.1.9/warg/ode.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/os_utilities/filtering.py` & `Warg-1.1.9/warg/os_utilities/filtering.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/os_utilities/os_platform.py` & `Warg-1.1.9/warg/os_utilities/os_platform.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/os_utilities/path_functions.py` & `Warg-1.1.9/warg/os_utilities/path_functions.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/os_utilities/path_utilities.py` & `Warg-1.1.9/warg/os_utilities/path_utilities.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/os_utilities/platform_selection.py` & `Warg-1.1.9/warg/os_utilities/platform_selection.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/packages/editable.py` & `Warg-1.1.9/warg/packages/editable.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from importlib.metadata import Distribution
+from importlib.metadata import Distribution, PackageNotFoundError
 
 __all__ = [
     "dist_is_editable",
     "package_is_editable",
     "get_dist_package_location",
     "get_package_location",
 ]
@@ -11,16 +11,20 @@
 from pathlib import Path
 
 
 def dist_is_editable(dist: Distribution) -> bool:
     """
     Return True if given Distribution is an editable installation.
     """
+    top_level = dist.read_text("top_level.txt")
 
-    top_level_name = dist.read_text("top_level.txt").split("\n")[0].strip()
+    if top_level:
+        top_level_name = top_level.split("\n")[0].strip()
+    else:  # assume top level namespace is the same as dist
+        top_level_name = dist.name
 
     if dist._read_files_egginfo() is not None:
         if top_level_name == dist._path.parent.stem:
             return True
 
     if dist._read_files_distinfo() is not None:
         direct_url_str = dist.read_text("direct_url.json")
@@ -33,21 +37,29 @@
     return False
 
 
 def package_is_editable(package_name: str) -> bool:
     """
     Return True if given Package is an editable installation.
     """
-    return dist_is_editable(Distribution.from_name(package_name))
+    try:
+        dist = Distribution.from_name(package_name)
+
+        return dist_is_editable(dist)
+    except PackageNotFoundError as p:
+        print(p)
 
 
 def get_package_location(package_name: str) -> Path:
-    dist = Distribution.from_name(package_name)
-    if dist:
-        return get_dist_package_location(dist)
+    try:
+        dist = Distribution.from_name(package_name)
+        if dist:
+            return get_dist_package_location(dist)
+    except PackageNotFoundError as p:
+        print(p)
 
 
 def get_dist_package_location(dist: Distribution) -> Path:
     """
     FULL OF ASSUMPTIONS!
 
     :param dist:
```

### Comparing `Warg-1.1.8/warg/packages/reloading.py` & `Warg-1.1.9/warg/packages/reloading.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/plugin.py` & `Warg-1.1.9/warg/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,23 @@
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
           Plugin
 
            Created on 13/06/2020
            """
 
-from importlib.metadata import entry_points, EntryPoint
-from typing import Tuple, Any, Generator, Union
+import sys
+
+if sys.version_info[:2] >= (3, 10):
+    # pylint: disable=no-name-in-module
+    from importlib.metadata import entry_points, EntryPoint
+else:
+    from importlib_metadata import entry_points, EntryPoint
+
+from typing import Tuple, Generator, Any
 
 __all__ = ["get_plugins", "get_static_plugins", "get_dynamic_plugins"]
 
 
 def get_plugins(package_name: str) -> Tuple:
     """Returns a list specifying all known plugins.
 
@@ -38,24 +45,25 @@
     if v in globals():
         return globals()[v][:]
     return ()
 
 
 def get_dynamic_plugins(
     package_name: str,
-) -> Generator[Union[str, EntryPoint], Any, None]:
+) -> Generator[EntryPoint, Any, None]:
     """Returns a list specifying dynamically loaded plugins.
 
     Returns:
       The list of dynamic plugins.
 
     [1]: https://packaging.python.org/specifications/entry-points/
     """
 
-    # .load() method to import and load that entry point (module or object).
-    # from importlib import metadata # new method!
-    # return [      entry_point.load()      for entry_point in metadata.entry_points()[f'{package_name}_plugins']      ]
-    return (entry_point for entry_point in entry_points(group="console_scripts", name=package_name))
+    return (
+        entry_point.load() for entry_point in entry_points(group=f"{package_name}_plugins", name=package_name)
+    )
 
 
 if __name__ == "__main__":
     print(get_plugins("warg"))
+
+    print(entry_points())
```

### Comparing `Warg-1.1.8/warg/replication.py` & `Warg-1.1.9/warg/replication.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/strings.py` & `Warg-1.1.9/warg/strings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/styling.py` & `Warg-1.1.9/warg/styling.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/text.py` & `Warg-1.1.9/warg/text.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.8/warg/typing_extension.py` & `Warg-1.1.9/warg/typing_extension.py`

 * *Files identical despite different names*

