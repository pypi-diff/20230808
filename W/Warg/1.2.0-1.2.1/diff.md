# Comparing `tmp/Warg-1.2.0.tar.gz` & `tmp/Warg-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Warg-1.2.0.tar", last modified: Tue Aug  8 07:30:58 2023, max compression
+gzip compressed data, was "Warg-1.2.1.tar", last modified: Tue Aug  8 07:47:25 2023, max compression
```

## Comparing `Warg-1.2.0.tar` & `Warg-1.2.1.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.210534 Warg-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.194534 Warg-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-08-08 07:30:52.000000 Warg-1.2.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:52.000000 Warg-1.2.0/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-08 07:30:52.000000 Warg-1.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 07:30:53.000000 Warg-1.2.0/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-08-08 07:30:53.000000 Warg-1.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-08 07:30:53.000000 Warg-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-08-08 07:30:58.210534 Warg-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-08-08 07:30:53.000000 Warg-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-08 07:30:53.000000 Warg-1.2.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.194534 Warg-1.2.0/Warg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-08-08 07:30:58.000000 Warg-1.2.0/Warg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-08 07:30:58.000000 Warg-1.2.0/Warg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:30:58.000000 Warg-1.2.0/Warg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-08 07:30:58.000000 Warg-1.2.0/Warg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 07:30:58.000000 Warg-1.2.0/Warg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.194534 Warg-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-08 07:30:53.000000 Warg-1.2.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-08 07:30:53.000000 Warg-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 07:30:53.000000 Warg-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-08 07:30:58.210534 Warg-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-08-08 07:30:53.000000 Warg-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.198534 Warg-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-08 07:30:53.000000 Warg-1.2.0/tests/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-08 07:30:53.000000 Warg-1.2.0/tests/test_ast_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-08 07:30:53.000000 Warg-1.2.0/tests/test_auto_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-08 07:30:53.000000 Warg-1.2.0/tests/test_collective.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-08 07:30:53.000000 Warg-1.2.0/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-08 07:30:53.000000 Warg-1.2.0/tests/test_gdkc.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-08 07:30:53.000000 Warg-1.2.0/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-08-08 07:30:53.000000 Warg-1.2.0/tests/test_kw_passing.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-08 07:30:53.000000 Warg-1.2.0/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-08-08 07:30:53.000000 Warg-1.2.0/tests/test_nod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-08 07:30:53.000000 Warg-1.2.0/tests/test_post_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-08 07:30:53.000000 Warg-1.2.0/tests/test_singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.198534 Warg-1.2.0/warg/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.198534 Warg-1.2.0/warg/ast_ops/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/ast_ops/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/ast_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/ast_ops/arg_indentifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/ast_ops/first_arg_identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.202534 Warg-1.2.0/warg/bases/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/bases/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/bases/property_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/boolean_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/business.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.202534 Warg-1.2.0/warg/colors/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/colors/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/colors/color_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/colors/css_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/colors/label_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/config_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/context_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/contexts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.202534 Warg-1.2.0/warg/data_structures/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/data_structures/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/data_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/data_structures/auto_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/data_structures/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16665 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/data_structures/named_ordered_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    28783 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/data_structures/ordered_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/data_structures/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/datetimes.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.202534 Warg-1.2.0/warg/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/decorators/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.202534 Warg-1.2.0/warg/decorators/caching/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/decorators/caching/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/decorators/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/decorators/caching/look_up_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/decorators/caching/property_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/decorators/exporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/decorators/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/decorators/kw_passing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/decorators/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/decorators/wrapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/gdkc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.206534 Warg-1.2.0/warg/generators/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/generators/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/generators/cyclic_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/generators/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/generators/mapping_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/generators/numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/generators/zipping_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/map_itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.206534 Warg-1.2.0/warg/math_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/math_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/math_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/math_utilities/multiples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/math_utilities/ordinals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/math_utilities/powers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.206534 Warg-1.2.0/warg/metas/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/metas/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/metas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/metas/post_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/metas/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.206534 Warg-1.2.0/warg/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/mixins/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/mixins/dict_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/mixins/ordinal_index_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/mixins/private.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/ode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.206534 Warg-1.2.0/warg/os_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/os_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/os_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/os_utilities/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/os_utilities/os_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/os_utilities/path_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/os_utilities/path_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/os_utilities/platform_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:30:58.210534 Warg-1.2.0/warg/packages/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/packages/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/packages/editable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/packages/pip_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/packages/reloading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/replication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/styling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-08 07:30:53.000000 Warg-1.2.0/warg/typing_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.248236 Warg-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.224235 Warg-1.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-08-08 07:47:15.000000 Warg-1.2.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:15.000000 Warg-1.2.1/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-08 07:47:15.000000 Warg-1.2.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 07:47:15.000000 Warg-1.2.1/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-08-08 07:47:15.000000 Warg-1.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-08 07:47:15.000000 Warg-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-08-08 07:47:25.248236 Warg-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-08-08 07:47:15.000000 Warg-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-08 07:47:15.000000 Warg-1.2.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.228235 Warg-1.2.1/Warg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-08-08 07:47:25.000000 Warg-1.2.1/Warg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-08 07:47:25.000000 Warg-1.2.1/Warg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:47:25.000000 Warg-1.2.1/Warg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-08 07:47:25.000000 Warg-1.2.1/Warg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 07:47:25.000000 Warg-1.2.1/Warg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.228235 Warg-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-08 07:47:15.000000 Warg-1.2.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-08 07:47:15.000000 Warg-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 07:47:15.000000 Warg-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-08 07:47:25.252236 Warg-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-08-08 07:47:15.000000 Warg-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.232235 Warg-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-08 07:47:15.000000 Warg-1.2.1/tests/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-08 07:47:15.000000 Warg-1.2.1/tests/test_ast_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-08 07:47:15.000000 Warg-1.2.1/tests/test_auto_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-08 07:47:15.000000 Warg-1.2.1/tests/test_collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-08 07:47:15.000000 Warg-1.2.1/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-08 07:47:15.000000 Warg-1.2.1/tests/test_gdkc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-08 07:47:15.000000 Warg-1.2.1/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-08-08 07:47:15.000000 Warg-1.2.1/tests/test_kw_passing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-08 07:47:15.000000 Warg-1.2.1/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-08-08 07:47:15.000000 Warg-1.2.1/tests/test_nod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-08 07:47:15.000000 Warg-1.2.1/tests/test_post_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-08 07:47:15.000000 Warg-1.2.1/tests/test_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.236235 Warg-1.2.1/warg/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.236235 Warg-1.2.1/warg/ast_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/ast_ops/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/ast_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/ast_ops/arg_indentifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/ast_ops/first_arg_identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.236235 Warg-1.2.1/warg/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/bases/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/bases/property_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/boolean_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/business.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.236235 Warg-1.2.1/warg/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/colors/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/colors/color_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/colors/css_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/colors/label_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/config_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/context_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/contexts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.240235 Warg-1.2.1/warg/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/data_structures/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/data_structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/data_structures/auto_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/data_structures/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16665 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/data_structures/named_ordered_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28783 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/data_structures/ordered_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/data_structures/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/datetimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.240235 Warg-1.2.1/warg/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/decorators/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.244235 Warg-1.2.1/warg/decorators/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/decorators/caching/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/decorators/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/decorators/caching/look_up_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/decorators/caching/property_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/decorators/exporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/decorators/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/decorators/kw_passing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/decorators/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/decorators/wrapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/gdkc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.244235 Warg-1.2.1/warg/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/generators/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/generators/cyclic_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/generators/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/generators/mapping_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/generators/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/generators/zipping_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/map_itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.244235 Warg-1.2.1/warg/math_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/math_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/math_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/math_utilities/multiples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/math_utilities/ordinals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/math_utilities/powers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.244235 Warg-1.2.1/warg/metas/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/metas/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/metas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/metas/post_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/metas/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.248236 Warg-1.2.1/warg/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/mixins/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/mixins/dict_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/mixins/ordinal_index_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/mixins/private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/ode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.248236 Warg-1.2.1/warg/os_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/os_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/os_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/os_utilities/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/os_utilities/os_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/os_utilities/path_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/os_utilities/path_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/os_utilities/platform_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:25.248236 Warg-1.2.1/warg/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/packages/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/packages/editable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/packages/pip_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/packages/reloading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/styling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-08 07:47:15.000000 Warg-1.2.1/warg/typing_extension.py
```

### Comparing `Warg-1.2.0/.github/CODE_OF_CONDUCT.md` & `Warg-1.2.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/LICENSE.md` & `Warg-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/PKG-INFO` & `Warg-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Warg
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/warg
 Download-URL: https://github.com/pything/warg/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
```

### Comparing `Warg-1.2.0/README.md` & `Warg-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/SECURITY.md` & `Warg-1.2.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/Warg.egg-info/PKG-INFO` & `Warg-1.2.1/Warg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Warg
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/warg
 Download-URL: https://github.com/pything/warg/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
```

### Comparing `Warg-1.2.0/Warg.egg-info/SOURCES.txt` & `Warg-1.2.1/Warg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/Warg.egg-info/requires.txt` & `Warg-1.2.1/Warg.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 setuptools>=60.9.3
 
 [all]
-pytest>=4.3.0
+pytest-runner
+tox
+warg
+sphinxcontrib-programoutput
 wheel>=0.33.0
 setuptools>=60.9.3
-tox
+sphinx
 pip>=19.0.3
-twine>=1.13.0
 coveralls>=1.6.0
-apppath
-sphinx
-sphinxcontrib-programoutput
-pytest-runner
-warg
-black>=18.9b0
 pytest-cov>=2.6.1
+black>=18.9b0
+twine>=1.13.0
+pytest>=4.3.0
+apppath
 
 [dev]
-pytest>=4.3.0
 wheel>=0.33.0
-pip>=19.0.3
-twine>=1.13.0
 tox
-coveralls>=1.6.0
-apppath
-sphinx
-sphinxcontrib-programoutput
-black>=18.9b0
 setuptools>=60.9.3
+sphinxcontrib-programoutput
+warg
 pytest-runner
+sphinx
+pip>=19.0.3
+coveralls>=1.6.0
 pytest-cov>=2.6.1
-warg
+black>=18.9b0
+twine>=1.13.0
+pytest>=4.3.0
+apppath
 
 [docs]
-apppath
-sphinx
-sphinxcontrib-programoutput
 warg
+sphinxcontrib-programoutput
+sphinx
+apppath
 
 [setup]
 pytest-runner
 
 [tests]
-pytest-cov>=2.6.1
-pytest>=4.3.0
 tox
+pytest>=4.3.0
+pytest-cov>=2.6.1
```

### Comparing `Warg-1.2.0/pyproject.toml` & `Warg-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/setup.py` & `Warg-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/tests/test_arguments.py` & `Warg-1.2.1/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/tests/test_ast_ops.py` & `Warg-1.2.1/tests/test_ast_ops.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/tests/test_auto_dict.py` & `Warg-1.2.1/tests/test_auto_dict.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/tests/test_collective.py` & `Warg-1.2.1/tests/test_collective.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/tests/test_gdkc.py` & `Warg-1.2.1/tests/test_gdkc.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/tests/test_imports.py` & `Warg-1.2.1/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/tests/test_kw_passing.py` & `Warg-1.2.1/tests/test_kw_passing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/tests/test_nod.py` & `Warg-1.2.1/tests/test_nod.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/tests/test_post_init.py` & `Warg-1.2.1/tests/test_post_init.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/tests/test_singleton.py` & `Warg-1.2.1/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/__init__.py` & `Warg-1.2.1/warg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from importlib import resources
 from importlib.metadata import Distribution, PackageNotFoundError
 from warnings import warn
 
 __project__ = "Warg"
 
 __author__ = "Christian Heider Nielsen"
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 __doc__ = r"""
 Created on 27/04/2019
 
 @author: cnheider
 
 """
```

### Comparing `Warg-1.2.0/warg/arguments.py` & `Warg-1.2.1/warg/arguments.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/ast_ops/arg_indentifier.py` & `Warg-1.2.1/warg/ast_ops/arg_indentifier.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/ast_ops/first_arg_identifier.py` & `Warg-1.2.1/warg/ast_ops/first_arg_identifier.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/bases/property_settings.py` & `Warg-1.2.1/warg/bases/property_settings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/boolean_tests.py` & `Warg-1.2.1/warg/boolean_tests.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/business.py` & `Warg-1.2.1/warg/business.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/colors/color_conversion.py` & `Warg-1.2.1/warg/colors/color_conversion.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/colors/css_colors.py` & `Warg-1.2.1/warg/colors/css_colors.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/colors/label_colors.py` & `Warg-1.2.1/warg/colors/label_colors.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/config_shell.py` & `Warg-1.2.1/warg/config_shell.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/context_wrapper.py` & `Warg-1.2.1/warg/context_wrapper.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/contexts.py` & `Warg-1.2.1/warg/contexts.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/data_structures/auto_dict.py` & `Warg-1.2.1/warg/data_structures/auto_dict.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/data_structures/mappings.py` & `Warg-1.2.1/warg/data_structures/mappings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/data_structures/named_ordered_dictionary.py` & `Warg-1.2.1/warg/data_structures/named_ordered_dictionary.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/data_structures/ordered_set.py` & `Warg-1.2.1/warg/data_structures/ordered_set.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/data_structures/sequences.py` & `Warg-1.2.1/warg/data_structures/sequences.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/datetimes.py` & `Warg-1.2.1/warg/datetimes.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/debug.py` & `Warg-1.2.1/warg/debug.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/decorators/caching/look_up_table.py` & `Warg-1.2.1/warg/decorators/caching/look_up_table.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/decorators/caching/property_caching.py` & `Warg-1.2.1/warg/decorators/caching/property_caching.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/decorators/exporting.py` & `Warg-1.2.1/warg/decorators/exporting.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/decorators/hashing.py` & `Warg-1.2.1/warg/decorators/hashing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/decorators/kw_passing.py` & `Warg-1.2.1/warg/decorators/kw_passing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/decorators/timing.py` & `Warg-1.2.1/warg/decorators/timing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/decorators/wrapping.py` & `Warg-1.2.1/warg/decorators/wrapping.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/exceptions.py` & `Warg-1.2.1/warg/exceptions.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/functions.py` & `Warg-1.2.1/warg/functions.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/gdkc.py` & `Warg-1.2.1/warg/gdkc.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/generators/cyclic_generators.py` & `Warg-1.2.1/warg/generators/cyclic_generators.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/generators/filtering.py` & `Warg-1.2.1/warg/generators/filtering.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/generators/mapping_generator.py` & `Warg-1.2.1/warg/generators/mapping_generator.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/generators/numbers.py` & `Warg-1.2.1/warg/generators/numbers.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/generators/zipping_generator.py` & `Warg-1.2.1/warg/generators/zipping_generator.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/iteration.py` & `Warg-1.2.1/warg/iteration.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/manipulation.py` & `Warg-1.2.1/warg/manipulation.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/map_itertools.py` & `Warg-1.2.1/warg/map_itertools.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/math_utilities/ordinals.py` & `Warg-1.2.1/warg/math_utilities/ordinals.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/math_utilities/powers.py` & `Warg-1.2.1/warg/math_utilities/powers.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/metas/post_init.py` & `Warg-1.2.1/warg/metas/post_init.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/metas/singleton.py` & `Warg-1.2.1/warg/metas/singleton.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/mixins/dict_mixins.py` & `Warg-1.2.1/warg/mixins/dict_mixins.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/mixins/ordinal_index_mixin.py` & `Warg-1.2.1/warg/mixins/ordinal_index_mixin.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/ode.py` & `Warg-1.2.1/warg/ode.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/os_utilities/filtering.py` & `Warg-1.2.1/warg/os_utilities/filtering.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/os_utilities/os_platform.py` & `Warg-1.2.1/warg/os_utilities/os_platform.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/os_utilities/path_functions.py` & `Warg-1.2.1/warg/os_utilities/path_functions.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/os_utilities/path_utilities.py` & `Warg-1.2.1/warg/os_utilities/path_utilities.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/os_utilities/platform_selection.py` & `Warg-1.2.1/warg/os_utilities/platform_selection.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/packages/editable.py` & `Warg-1.2.1/warg/packages/editable.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,31 +17,34 @@
     """
     top_level = dist.read_text("top_level.txt")
 
     top_level_name = None
     if top_level:
         top_level_name = top_level.split("\n")[0].strip()
     else:  # assume top level namespace is the same as dist
-        if isinstance(dist, Distribution):
-            top_level_name = dist.name
-        elif isinstance(dist, PathDistribution):
+        if isinstance(dist, PathDistribution):
             top_level_name = dist._normalized_name
+        elif isinstance(dist, Distribution):
+            if hasattr(dist, "name"):
+                top_level_name = dist.name
 
     if top_level_name:
-        if dist._read_files_egginfo() is not None:
-            if top_level_name == dist._path.parent.stem:
-                return True
-
-    if dist._read_files_distinfo() is not None:
-        direct_url_str = dist.read_text("direct_url.json")
-        if direct_url_str is not None:
-            direct_url_json = json.loads(direct_url_str)
-            if "dir_info" in direct_url_json:
-                if "editable" in direct_url_json["dir_info"]:
-                    return direct_url_json["dir_info"]["editable"]
+        if hasattr(dist, "_read_files_egginfo"):
+            if dist._read_files_egginfo() is not None:
+                if top_level_name == dist._path.parent.stem:
+                    return True
+
+    if hasattr(dist, "_read_files_distinfo"):
+        if dist._read_files_distinfo() is not None:
+            direct_url_str = dist.read_text("direct_url.json")
+            if direct_url_str is not None:
+                direct_url_json = json.loads(direct_url_str)
+                if "dir_info" in direct_url_json:
+                    if "editable" in direct_url_json["dir_info"]:
+                        return direct_url_json["dir_info"]["editable"]
 
     return False
 
 
 def package_is_editable(package_name: str) -> bool:
     """
     Return True if given Package is an editable installation.
```

### Comparing `Warg-1.2.0/warg/packages/pip_parsing.py` & `Warg-1.2.1/warg/packages/pip_parsing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/packages/reloading.py` & `Warg-1.2.1/warg/packages/reloading.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/plugin.py` & `Warg-1.2.1/warg/plugin.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/replication.py` & `Warg-1.2.1/warg/replication.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/strings.py` & `Warg-1.2.1/warg/strings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/styling.py` & `Warg-1.2.1/warg/styling.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/text.py` & `Warg-1.2.1/warg/text.py`

 * *Files identical despite different names*

### Comparing `Warg-1.2.0/warg/typing_extension.py` & `Warg-1.2.1/warg/typing_extension.py`

 * *Files identical despite different names*

