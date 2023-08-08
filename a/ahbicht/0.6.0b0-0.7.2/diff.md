# Comparing `tmp/ahbicht-0.6.0b0.tar.gz` & `tmp/ahbicht-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahbicht-0.6.0b0.tar", last modified: Mon Jan 16 12:27:23 2023, max compression
+gzip compressed data, was "ahbicht-0.7.2.tar", last modified: Tue Aug  8 07:53:59 2023, max compression
```

## Comparing `ahbicht-0.6.0b0.tar` & `ahbicht-0.7.2.tar`

### file list

```diff
@@ -1,157 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.303480 ahbicht-0.6.0b0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.287481 ahbicht-0.6.0b0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.287481 ahbicht-0.6.0b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/json_schemas.yml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/typescript_from_json_schemas.yml
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-01-16 12:27:23.303480 ahbicht-0.6.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    54198 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/definition-of-terms.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.287481 ahbicht-0.6.0b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.291481 ahbicht-0.6.0b0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/_static/ahbicht-favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)  2076200 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/_static/ahbicht-logo-raw.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21244 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/_static/ahbicht-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    12394 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/_static/ahbicht-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)  2025509 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/_static/ahbicht_uml.svg
--rw-r--r--   0 runner    (1001) docker     (123)    41431 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/_static/wim_ahb_screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.295481 ahbicht-0.6.0b0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/api/ahbicht.content_evaluation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/api/ahbicht.expressions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/api/ahbicht.json_serialization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/api/ahbicht.rst
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/api/ahbicht.validation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9533 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.295481 ahbicht-0.6.0b0/json_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/AhbExpressionEvaluationResultSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/CategorizedKeyExtractSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/ConditionKeyConditionTextMappingSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/ContentEvaluationResultSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/EvaluatedFormatConstraintSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/FormatConstraintEvaluationResultSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/PackageKeyConditionExpressionMappingSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/RequirementConstraintEvaluationResultSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/TokenSchema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/json_schemas/generate_json_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    26252 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/minimal_working_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-01-16 12:27:23.303480 ahbicht-0.6.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.287481 ahbicht-0.6.0b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.295481 ahbicht-0.6.0b0/src/ahbicht/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/condition_node_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/condition_node_distinction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.295481 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)   136061 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/EvaluatingConditions.png
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/categorized_key_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/content_evaluation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/evaluationdatatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/evaluator_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/fc_evaluators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/german_strom_and_gas_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/rc_evaluators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/content_evaluation/token_logic_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/evaluation_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.299481 ahbicht-0.6.0b0/src/ahbicht/expressions/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/ahb_expression_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/ahb_expression_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/condition_expression_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/condition_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)   171830 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/condition_structure_with_more_than_one_condition.png
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    11182 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/expression_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/expression_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/format_constraint_expression_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/hints_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/package_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/expressions/requirement_constraint_expression_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.299481 ahbicht-0.6.0b0/src/ahbicht/json_serialization/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/json_serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/json_serialization/concise_condition_key_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/json_serialization/concise_tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/json_serialization/tree_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/mapping_results.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.299481 ahbicht-0.6.0b0/src/ahbicht/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22516 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/validation/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/validation/validation_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/src/ahbicht/validation/validation_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.295481 ahbicht-0.6.0b0/src/ahbicht.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-01-16 12:27:23.000000 ahbicht-0.6.0b0/src/ahbicht.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-01-16 12:27:23.000000 ahbicht-0.6.0b0/src/ahbicht.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 12:27:23.000000 ahbicht-0.6.0b0/src/ahbicht.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 12:27:23.000000 ahbicht-0.6.0b0/src/ahbicht.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-16 12:27:23.000000 ahbicht-0.6.0b0/src/ahbicht.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-16 12:27:23.000000 ahbicht-0.6.0b0/src/ahbicht.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.303480 ahbicht-0.6.0b0/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.303480 ahbicht-0.6.0b0/unittests/content_evaluation_result_generation/
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/content_evaluation_result_generation/example0.json
--rw-r--r--   0 runner    (1001) docker     (123)    42249 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/content_evaluation_result_generation/example1.json
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 12:27:23.303480 ahbicht-0.6.0b0/unittests/provider_test_files/
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/provider_test_files/example_hints_file.json
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/provider_test_files/example_package_mapping_dict.json
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/provider_test_files/example_package_mapping_list.json
--rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_ahb_expression_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_ahb_expression_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_categorized_key_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_cer_based_fc_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_cer_based_hints_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_cer_based_package_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_cer_based_rc_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_condition_node_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_condition_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_condition_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_dict_based_fc_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_dict_based_rc_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_evaluator_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_evaluator_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_expression_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_expression_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_format_constraint_expression_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_format_constraints_context_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_german_strom_and_gas_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_hints_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_integration_mwe.py
--rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_json_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_mixed_sync_async_rc_fc_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_package_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_requirement_constraint_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18294 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_requirement_constraint_expression_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_time_condition_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    25322 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_tree_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_utility_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    47895 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_validation_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_validity_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-01-16 12:27:17.000000 ahbicht-0.6.0b0/unittests/test_warning_when_using_inject_attr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.188638 ahbicht-0.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.168638 ahbicht-0.7.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-08 07:53:38.000000 ahbicht-0.7.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.168638 ahbicht-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-08 07:53:38.000000 ahbicht-0.7.2/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-08-08 07:53:38.000000 ahbicht-0.7.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-08 07:53:38.000000 ahbicht-0.7.2/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-08 07:53:38.000000 ahbicht-0.7.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-08-08 07:53:38.000000 ahbicht-0.7.2/.github/workflows/json_schemas.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-08 07:53:38.000000 ahbicht-0.7.2/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-08-08 07:53:38.000000 ahbicht-0.7.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-08 07:53:38.000000 ahbicht-0.7.2/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-08 07:53:38.000000 ahbicht-0.7.2/.github/workflows/typescript_from_json_schemas.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-08 07:53:38.000000 ahbicht-0.7.2/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-08-08 07:53:38.000000 ahbicht-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-08 07:53:38.000000 ahbicht-0.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-08 07:53:38.000000 ahbicht-0.7.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-08 07:53:38.000000 ahbicht-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    54975 2023-08-08 07:53:59.188638 ahbicht-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    54198 2023-08-08 07:53:38.000000 ahbicht-0.7.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-08-08 07:53:38.000000 ahbicht-0.7.2/definition-of-terms.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.172638 ahbicht-0.7.2/dev_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-08 07:53:38.000000 ahbicht-0.7.2/dev_requirements/requirements-coverage.in
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-08 07:53:38.000000 ahbicht-0.7.2/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 07:53:38.000000 ahbicht-0.7.2/dev_requirements/requirements-docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-08-08 07:53:38.000000 ahbicht-0.7.2/dev_requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-08 07:53:38.000000 ahbicht-0.7.2/dev_requirements/requirements-formatting.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-08 07:53:38.000000 ahbicht-0.7.2/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-08 07:53:38.000000 ahbicht-0.7.2/dev_requirements/requirements-json_schemas.in
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-08 07:53:38.000000 ahbicht-0.7.2/dev_requirements/requirements-json_schemas.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-08 07:53:38.000000 ahbicht-0.7.2/dev_requirements/requirements-linting.in
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-08 07:53:38.000000 ahbicht-0.7.2/dev_requirements/requirements-linting.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-08 07:53:38.000000 ahbicht-0.7.2/dev_requirements/requirements-test_packaging.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-08-08 07:53:38.000000 ahbicht-0.7.2/dev_requirements/requirements-test_packaging.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-08 07:53:38.000000 ahbicht-0.7.2/dev_requirements/requirements-tests.in
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-08 07:53:38.000000 ahbicht-0.7.2/dev_requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-08 07:53:38.000000 ahbicht-0.7.2/dev_requirements/requirements-type_check.in
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-08 07:53:38.000000 ahbicht-0.7.2/dev_requirements/requirements-type_check.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.172638 ahbicht-0.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-08 07:53:38.000000 ahbicht-0.7.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.176638 ahbicht-0.7.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-08 07:53:38.000000 ahbicht-0.7.2/docs/_static/ahbicht-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2076200 2023-08-08 07:53:38.000000 ahbicht-0.7.2/docs/_static/ahbicht-logo-raw.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21244 2023-08-08 07:53:38.000000 ahbicht-0.7.2/docs/_static/ahbicht-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12394 2023-08-08 07:53:38.000000 ahbicht-0.7.2/docs/_static/ahbicht-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  2025509 2023-08-08 07:53:38.000000 ahbicht-0.7.2/docs/_static/ahbicht_uml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41431 2023-08-08 07:53:38.000000 ahbicht-0.7.2/docs/_static/wim_ahb_screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.176638 ahbicht-0.7.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-08 07:53:38.000000 ahbicht-0.7.2/docs/api/ahbicht.content_evaluation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-08-08 07:53:38.000000 ahbicht-0.7.2/docs/api/ahbicht.expressions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-08 07:53:38.000000 ahbicht-0.7.2/docs/api/ahbicht.json_serialization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-08-08 07:53:38.000000 ahbicht-0.7.2/docs/api/ahbicht.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-08 07:53:38.000000 ahbicht-0.7.2/docs/api/ahbicht.validation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-08 07:53:38.000000 ahbicht-0.7.2/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9533 2023-08-08 07:53:38.000000 ahbicht-0.7.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-08 07:53:38.000000 ahbicht-0.7.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-08 07:53:38.000000 ahbicht-0.7.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.180638 ahbicht-0.7.2/json_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-08-08 07:53:38.000000 ahbicht-0.7.2/json_schemas/AhbExpressionEvaluationResultSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-08-08 07:53:38.000000 ahbicht-0.7.2/json_schemas/CategorizedKeyExtractSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-08-08 07:53:38.000000 ahbicht-0.7.2/json_schemas/ConditionKeyConditionTextMappingSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-08-08 07:53:38.000000 ahbicht-0.7.2/json_schemas/ContentEvaluationResultSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-08 07:53:38.000000 ahbicht-0.7.2/json_schemas/EvaluatedFormatConstraintSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-08 07:53:38.000000 ahbicht-0.7.2/json_schemas/FormatConstraintEvaluationResultSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-08-08 07:53:38.000000 ahbicht-0.7.2/json_schemas/PackageKeyConditionExpressionMappingSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-08 07:53:38.000000 ahbicht-0.7.2/json_schemas/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-08 07:53:38.000000 ahbicht-0.7.2/json_schemas/RequirementConstraintEvaluationResultSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-08-08 07:53:38.000000 ahbicht-0.7.2/json_schemas/TokenSchema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-08-08 07:53:38.000000 ahbicht-0.7.2/json_schemas/generate_json_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26272 2023-08-08 07:53:38.000000 ahbicht-0.7.2/minimal_working_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-08 07:53:38.000000 ahbicht-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-08 07:53:38.000000 ahbicht-0.7.2/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-08 07:53:38.000000 ahbicht-0.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-08 07:53:59.192638 ahbicht-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-08 07:53:38.000000 ahbicht-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.164638 ahbicht-0.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.180638 ahbicht-0.7.2/src/ahbicht/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/condition_node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/condition_node_distinction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.180638 ahbicht-0.7.2/src/ahbicht/content_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)   136061 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/content_evaluation/EvaluatingConditions.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/content_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/content_evaluation/categorized_key_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/content_evaluation/content_evaluation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/content_evaluation/evaluationdatatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/content_evaluation/evaluator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/content_evaluation/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/content_evaluation/fc_evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/content_evaluation/german_strom_and_gas_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/content_evaluation/rc_evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/content_evaluation/token_logic_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/evaluation_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.184638 ahbicht-0.7.2/src/ahbicht/expressions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/expressions/ahb_expression_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/expressions/ahb_expression_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/expressions/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/expressions/condition_expression_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/expressions/condition_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171830 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/expressions/condition_structure_with_more_than_one_condition.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/expressions/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/expressions/expression_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/expressions/expression_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/expressions/format_constraint_expression_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/expressions/hints_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/expressions/package_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/expressions/requirement_constraint_expression_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.184638 ahbicht-0.7.2/src/ahbicht/json_serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/json_serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/json_serialization/concise_condition_key_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/json_serialization/concise_tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/json_serialization/tree_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/mapping_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.184638 ahbicht-0.7.2/src/ahbicht/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23606 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/validation/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/validation/validation_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-08 07:53:38.000000 ahbicht-0.7.2/src/ahbicht/validation/validation_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.180638 ahbicht-0.7.2/src/ahbicht.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    54975 2023-08-08 07:53:59.000000 ahbicht-0.7.2/src/ahbicht.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-08-08 07:53:59.000000 ahbicht-0.7.2/src/ahbicht.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:53:59.000000 ahbicht-0.7.2/src/ahbicht.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:53:58.000000 ahbicht-0.7.2/src/ahbicht.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-08 07:53:59.000000 ahbicht-0.7.2/src/ahbicht.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 07:53:59.000000 ahbicht-0.7.2/src/ahbicht.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-08-08 07:53:38.000000 ahbicht-0.7.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.188638 ahbicht-0.7.2/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.188638 ahbicht-0.7.2/unittests/content_evaluation_result_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/content_evaluation_result_generation/example0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42249 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/content_evaluation_result_generation/example1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:53:59.188638 ahbicht-0.7.2/unittests/provider_test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/provider_test_files/example_hints_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/provider_test_files/example_package_mapping_dict.json
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/provider_test_files/example_package_mapping_list.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20179 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_ahb_expression_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_ahb_expression_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_categorized_key_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_cer_based_fc_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_cer_based_hints_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_cer_based_package_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_cer_based_rc_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_condition_node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_condition_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_condition_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_dict_based_fc_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_dict_based_rc_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_evaluator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_evaluator_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_expression_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_expression_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_format_constraint_expression_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_format_constraints_context_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_german_strom_and_gas_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_hints_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_integration_mwe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_json_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_mixed_sync_async_rc_fc_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_package_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_requirement_constraint_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18294 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_requirement_constraint_expression_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_time_condition_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25322 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_tree_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_utility_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48598 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12765 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_validation_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_validity_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-08-08 07:53:38.000000 ahbicht-0.7.2/unittests/test_warning_when_using_inject_attr.py
```

### Comparing `ahbicht-0.6.0b0/.github/dependabot.yml` & `ahbicht-0.7.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/.github/workflows/codeql-analysis.yml` & `ahbicht-0.7.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/.github/workflows/coverage.yml` & `ahbicht-0.7.2/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/.github/workflows/docs.yml` & `ahbicht-0.7.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/.github/workflows/json_schemas.yml` & `ahbicht-0.7.2/.github/workflows/json_schemas.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/.github/workflows/packaging_test.yml` & `ahbicht-0.7.2/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/.github/workflows/python-publish.yml` & `ahbicht-0.7.2/.github/workflows/python-publish.yml`

 * *Files 9% similar despite different names*

```diff
@@ -24,32 +24,34 @@
           python-version: ${{ matrix.python-version }}
       - name: Install tox
         run: |
           python -m pip install --upgrade pip
           pip install tox
       - name: Run tox
         run: |
-          tox
+          tox -e tests
 
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to PyPI and TestPyPI
     runs-on: ubuntu-latest
     needs: tests
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install setuptools setuptools-scm wheel twine
+          pip install tox
+          tox -e test_packaging
       - name: Build a binary wheel and a source tarball
         run: |
           python setup.py sdist bdist_wheel
       - name: Publish distribution 📦 to PyPI
         if: startsWith(github.ref, 'refs/tags/v')
-        uses: pypa/gh-action-pypi-publish@release/v1
+        uses: pypa/gh-action-pypi-publish@v1.8.8
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
+          skip-existing: true
```

### Comparing `ahbicht-0.6.0b0/.github/workflows/pythonlint.yml` & `ahbicht-0.7.2/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/.github/workflows/typescript_from_json_schemas.yml` & `ahbicht-0.7.2/.github/workflows/typescript_from_json_schemas.yml`

 * *Files 10% similar despite different names*

```diff
@@ -20,17 +20,19 @@
         run: json2ts -i 'json_schemas/**.json' -o ts_models/
       - name: Upload TypeScript Files
         uses: actions/upload-artifact@master
         with:
           name: TypeScriptClasses
           path: ts_models
       - name: Push ts_models content to type script models repo
-        uses: cpina/github-action-push-to-another-repository@v1.5.1
+        uses: cpina/github-action-push-to-another-repository@v1.7.2
         env:
-          API_TOKEN_GITHUB: ${{ secrets.TS_MODELS_PUSH_TOKEN }} # this token expires on 2023-05-01
+          API_TOKEN_GITHUB: ${{ secrets.TS_MODELS_PUSH_TOKEN }} # this token expires on 2024-08-01
+          # it's a Personal Access Token (PAT) with repo scope
+          # https://github.com/Hochfrequenz/ahbicht/settings/secrets/actions/TS_MODELS_PUSH_TOKEN
         with:
           source-directory: "ts_models"
           target-directory: "src"
           destination-github-username: "Hochfrequenz"
           destination-repository-name: "ahbicht-ts-models"
           user-email: ahbicht@hochfrequenz.de
           target-branch: main
```

### Comparing `ahbicht-0.6.0b0/.github/workflows/unittests.yml` & `ahbicht-0.7.2/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/.gitignore` & `ahbicht-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/.pre-commit-config.yaml` & `ahbicht-0.7.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/.readthedocs.yaml` & `ahbicht-0.7.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/LICENSE` & `ahbicht-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/PKG-INFO` & `ahbicht-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahbicht
-Version: 0.6.0b0
+Version: 0.7.2
 Summary: Python Library to parse AHB expressions.
 Home-page: https://github.com/Hochfrequenz/ahbicht
 Author: Annika Schlögl
 Author-email: annika.schloegl@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://ahbicht.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Hochfrequenz/ahbicht/
@@ -421,9 +421,7 @@
 
 .. |Unittests status badge| image:: https://github.com/Hochfrequenz/ahbicht/workflows/Unittests/badge.svg
 .. |Coverage status badge| image:: https://github.com/Hochfrequenz/ahbicht/workflows/Coverage/badge.svg
 .. |Linting status badge| image:: https://github.com/Hochfrequenz/ahbicht/workflows/Linting/badge.svg
 .. |Black status badge| image:: https://github.com/Hochfrequenz/ahbicht/workflows/Black/badge.svg
 .. |pypy status badge| image:: https://img.shields.io/pypi/v/ahbicht
 .. |UTILMD_AHB_WiM_3_1b_20201016.pdf page 90| image:: ./docs/_static/wim_ahb_screenshot.png
-
-
```

### Comparing `ahbicht-0.6.0b0/README.rst` & `ahbicht-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/definition-of-terms.csv` & `ahbicht-0.7.2/definition-of-terms.csv`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/docs/Makefile` & `ahbicht-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/docs/_static/ahbicht-favicon.png` & `ahbicht-0.7.2/docs/_static/ahbicht-favicon.png`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/docs/_static/ahbicht-logo-raw.svg` & `ahbicht-0.7.2/docs/_static/ahbicht-logo-raw.svg`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/docs/_static/ahbicht-logo.png` & `ahbicht-0.7.2/docs/_static/ahbicht-logo.png`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/docs/_static/ahbicht-logo.svg` & `ahbicht-0.7.2/docs/_static/ahbicht-logo.svg`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/docs/_static/ahbicht_uml.svg` & `ahbicht-0.7.2/docs/_static/ahbicht_uml.svg`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/docs/_static/wim_ahb_screenshot.png` & `ahbicht-0.7.2/docs/_static/wim_ahb_screenshot.png`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/docs/api/ahbicht.content_evaluation.rst` & `ahbicht-0.7.2/docs/api/ahbicht.content_evaluation.rst`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/docs/api/ahbicht.expressions.rst` & `ahbicht-0.7.2/docs/api/ahbicht.expressions.rst`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/docs/api/ahbicht.json_serialization.rst` & `ahbicht-0.7.2/docs/api/ahbicht.json_serialization.rst`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/docs/api/ahbicht.rst` & `ahbicht-0.7.2/docs/api/ahbicht.rst`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/docs/api/ahbicht.validation.rst` & `ahbicht-0.7.2/docs/api/ahbicht.validation.rst`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/docs/conf.py` & `ahbicht-0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/docs/make.bat` & `ahbicht-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/json_schemas/AhbExpressionEvaluationResultSchema.json` & `ahbicht-0.7.2/json_schemas/AhbExpressionEvaluationResultSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/json_schemas/CategorizedKeyExtractSchema.json` & `ahbicht-0.7.2/json_schemas/CategorizedKeyExtractSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/json_schemas/ConditionKeyConditionTextMappingSchema.json` & `ahbicht-0.7.2/json_schemas/ConditionKeyConditionTextMappingSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/json_schemas/ContentEvaluationResultSchema.json` & `ahbicht-0.7.2/json_schemas/ContentEvaluationResultSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/json_schemas/EvaluatedFormatConstraintSchema.json` & `ahbicht-0.7.2/json_schemas/EvaluatedFormatConstraintSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/json_schemas/FormatConstraintEvaluationResultSchema.json` & `ahbicht-0.7.2/json_schemas/FormatConstraintEvaluationResultSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/json_schemas/PackageKeyConditionExpressionMappingSchema.json` & `ahbicht-0.7.2/json_schemas/PackageKeyConditionExpressionMappingSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/json_schemas/README.md` & `ahbicht-0.7.2/json_schemas/README.md`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/json_schemas/RequirementConstraintEvaluationResultSchema.json` & `ahbicht-0.7.2/json_schemas/RequirementConstraintEvaluationResultSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/json_schemas/TokenSchema.json` & `ahbicht-0.7.2/json_schemas/TokenSchema.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/json_schemas/generate_json_schemas.py` & `ahbicht-0.7.2/json_schemas/generate_json_schemas.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/minimal_working_example.ipynb` & `ahbicht-0.7.2/minimal_working_example.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999517882187938%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(13, '\\n')]}}, 8: {'source': {insert: [(4, '\\n')]}}}"}*

```diff
@@ -189,14 +189,15 @@
                 "    \"\"\"\n",
                 "    Format Constraint (FC) Evaluator answers questions of the kind: \"Does the data provided obey format specified in condition <condition_number>?\"\n",
                 "    Any format constraint evaluator has to inherit from FcEvaluator.\n",
                 "    \"\"\"\n",
                 "\n",
                 "    edifact_format = EdifactFormat.UTILMD\n",
                 "    edifact_format_version = EdifactFormatVersion.FV2104  # valid since 2021-04-01\n",
+                "\n",
                 "    # note that format constraint evaluation methods can also be async, if necessary\n",
                 "    def evaluate_901(self, entered_input):\n",
                 "        \"\"\"\n",
                 "        This method checks if the entered_input fulfills the constraints of condition 901.\n",
                 "        This could be f.e. if entered_input is a valid OBIS, a valid Marktlokations-ID etc.\n",
                 "        For this MWE we check if the input is all lower case.\n",
                 "        The methods can be either sync or async.\n",
@@ -305,14 +306,15 @@
             "outputs": [],
             "source": [
                 "from ahbicht.content_evaluation.token_logic_provider import SingletonTokenLogicProvider, TokenLogicProvider\n",
                 "import inject\n",
                 "from ahbicht.content_evaluation.evaluationdatatypes import EvaluatableDataProvider\n",
                 "from ahbicht.expressions.ahb_expression_evaluation import evaluate_ahb_expression_tree\n",
                 "\n",
+                "\n",
                 "# We use dependency injection to get the evaluators in place:\n",
                 "def provide_evaluatable_data():\n",
                 "    # place your own dynamic(!) data provision method here\n",
                 "    # in web applications it's recommended to access a context variable here that is set in the request handler\n",
                 "    return EvaluatableData(\n",
                 "        edifact_seed=hardcoded_content_evaluations,\n",
                 "        edifact_format=EdifactFormat.UTILMD,\n",
```

### Comparing `ahbicht-0.6.0b0/pyproject.toml` & `ahbicht-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/requirements.txt` & `ahbicht-0.7.2/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
-# by the following command:
+# This file is autogenerated by pip-compile with python 3.10
+# To update, run:
 #
 #    pip-compile requirements.in
 #
-attrs==22.2.0
+attrs==23.1.0
     # via
     #   -r requirements.in
     #   maus
-inject==4.3.1
+inject==5.0.0
     # via -r requirements.in
-lark==1.1.5
+lark==1.1.7
     # via -r requirements.in
-marshmallow==3.19.0
+marshmallow==3.20.1
     # via
     #   -r requirements.in
     #   marshmallow-enum
     #   maus
 marshmallow-enum==1.5.1
     # via -r requirements.in
-maus==0.3.1a0
+maus==0.2.9
     # via -r requirements.in
 more-itertools==9.0.0
     # via maus
-packaging==21.3
+packaging==23.0
     # via marshmallow
-pyparsing==3.0.8
-    # via packaging
-pytz==2022.7
+pytz==2023.3
     # via -r requirements.in
```

### Comparing `ahbicht-0.6.0b0/setup.cfg` & `ahbicht-0.7.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 python_requires = >=3.8
 install_requires = 
 	attrs>=21.4.0
 	lark>=1.1.4
 	inject
 	marshmallow
 	marshmallow_enum
-	maus>=0.3.1a
+	maus>=0.1.24
 	pytz
 
 [options.packages.find]
 where = src
 exclude = 
 	unittests
```

### Comparing `ahbicht-0.6.0b0/src/ahbicht/__init__.py` & `ahbicht-0.7.2/src/ahbicht/__init__.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/condition_node_builder.py` & `ahbicht-0.7.2/src/ahbicht/condition_node_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ahbicht.content_evaluation.token_logic_provider import TokenLogicProvider
 from ahbicht.expressions.condition_expression_parser import extract_categorized_keys_from_tree
 from ahbicht.expressions.condition_nodes import Hint, RequirementConstraint, UnevaluatedFormatConstraint
 
 # TRCTransformerArgument is a union of nodes that are already evaluated from a Requirement Constraint (RC) perspective.
 # The Format Constraints (FC) might still be unevaluated. That's why the return type used in the
 # RequirementConstraintTransformer is always an EvaluatedComposition.
-TRCTransformerArgument = Union[RequirementConstraint, UnevaluatedFormatConstraint, Hint]
+TRCTransformerArgument = Union[RequirementConstraint, UnevaluatedFormatConstraint, Hint]  # pylint:disable=invalid-name
 
 
 # pylint: disable=no-member, too-few-public-methods
 
 
 class ConditionNodeBuilder:
     """
```

### Comparing `ahbicht-0.6.0b0/src/ahbicht/condition_node_distinction.py` & `ahbicht-0.7.2/src/ahbicht/condition_node_distinction.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/EvaluatingConditions.png` & `ahbicht-0.7.2/src/ahbicht/content_evaluation/EvaluatingConditions.png`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/__init__.py` & `ahbicht-0.7.2/src/ahbicht/content_evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/categorized_key_extract.py` & `ahbicht-0.7.2/src/ahbicht/content_evaluation/categorized_key_extract.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/content_evaluation_result.py` & `ahbicht-0.7.2/src/ahbicht/content_evaluation/content_evaluation_result.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/evaluationdatatypes.py` & `ahbicht-0.7.2/src/ahbicht/content_evaluation/evaluationdatatypes.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/evaluator_factory.py` & `ahbicht-0.7.2/src/ahbicht/content_evaluation/evaluator_factory.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/evaluators.py` & `ahbicht-0.7.2/src/ahbicht/content_evaluation/evaluators.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/fc_evaluators.py` & `ahbicht-0.7.2/src/ahbicht/content_evaluation/fc_evaluators.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/german_strom_and_gas_tag.py` & `ahbicht-0.7.2/src/ahbicht/content_evaluation/german_strom_and_gas_tag.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/rc_evaluators.py` & `ahbicht-0.7.2/src/ahbicht/content_evaluation/rc_evaluators.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/content_evaluation/token_logic_provider.py` & `ahbicht-0.7.2/src/ahbicht/content_evaluation/token_logic_provider.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/evaluation_results.py` & `ahbicht-0.7.2/src/ahbicht/evaluation_results.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,21 @@
 @attrs.define(auto_attribs=True, kw_only=True)
 class RequirementConstraintEvaluationResult:
     """
     A class for the result of the requirement constraint evaluation.
     """
 
     #: true if condition expression in regard to requirement constraints evaluates to true
-    requirement_constraints_fulfilled: bool = attrs.field(validator=attrs.validators.instance_of(bool))
-    #: true if it is dependent on requirement constraints
-    requirement_is_conditional: bool = attrs.field(validator=attrs.validators.instance_of(bool))
+    requirement_constraints_fulfilled: Optional[bool] = attrs.field(
+        validator=attrs.validators.optional(attrs.validators.instance_of(bool))
+    )
+    #: true if it is dependent on requirement constraints; None if there are unknown condition nodes left
+    requirement_is_conditional: Optional[bool] = attrs.field(
+        validator=attrs.validators.optional(attrs.validators.instance_of(bool))
+    )
 
     format_constraints_expression: Optional[str] = attrs.field(
         default=None, validator=attrs.validators.optional(attrs.validators.instance_of(str))
     )
     #: Hint text that should be displayed in the frontend, e.g. "[501] Hinweis: 'ID der Messlokation'"
     hints: Optional[str] = attrs.field(
         default=None, validator=attrs.validators.optional(attrs.validators.instance_of(str))
```

### Comparing `ahbicht-0.6.0b0/src/ahbicht/expressions/__init__.py` & `ahbicht-0.7.2/src/ahbicht/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/expressions/ahb_expression_evaluation.py` & `ahbicht-0.7.2/src/ahbicht/expressions/ahb_expression_evaluation.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/expressions/ahb_expression_parser.py` & `ahbicht-0.7.2/src/ahbicht/expressions/ahb_expression_parser.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/expressions/base_transformer.py` & `ahbicht-0.7.2/src/ahbicht/expressions/base_transformer.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/expressions/condition_expression_parser.py` & `ahbicht-0.7.2/src/ahbicht/expressions/condition_expression_parser.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/expressions/condition_nodes.py` & `ahbicht-0.7.2/src/ahbicht/expressions/condition_nodes.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/expressions/condition_structure_with_more_than_one_condition.png` & `ahbicht-0.7.2/src/ahbicht/expressions/condition_structure_with_more_than_one_condition.png`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/expressions/enums.py` & `ahbicht-0.7.2/src/ahbicht/expressions/enums.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/expressions/expression_builder.py` & `ahbicht-0.7.2/src/ahbicht/expressions/expression_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,26 +57,26 @@
         connects the expression with an exclusive or (XOR)
         :param other: condition or expression to be connected to the expression
         :return:
         """
         raise NotImplementedError("Has to be implemented by inheriting class.")
 
 
-TEffectiveFCExpressionBuilderArguments = Union[
+TEffectiveFCExpressionBuilderArguments = Union[  # pylint:disable=invalid-name
     EvaluatedComposition, UnevaluatedFormatConstraint, Optional[str]
 ]  # node types that have an effect on the built format constraint expression
 
-TUneffectiveFCExpressionBuilderArguments = Union[
+TUneffectiveFCExpressionBuilderArguments = Union[  # pylint:disable=invalid-name
     RequirementConstraint, EvaluatedComposition, Hint, Type[ConditionNode]
 ]  # node types that are formally accepted as argument but don't
 # have any effect. Instead of checking which nodes contain format constraints all are put into the
 # FormatConstraintExpressionBuilder, but it only has an effect on those with format constraints.
 # Note that EvaluatedComposition is in both classes since they can have format constraints but don't have to.
 
-TSupportedFCExpressionBuilderArguments = Union[
+TSupportedFCExpressionBuilderArguments = Union[  # pylint:disable=invalid-name
     TEffectiveFCExpressionBuilderArguments, TUneffectiveFCExpressionBuilderArguments
 ]
 
 
 class FormatConstraintExpressionBuilder(ExpressionBuilder[TSupportedFCExpressionBuilderArguments]):
     """
     Class to create expressions that consist of FormatConstraints
```

### Comparing `ahbicht-0.6.0b0/src/ahbicht/expressions/expression_resolver.py` & `ahbicht-0.7.2/src/ahbicht/expressions/expression_resolver.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/expressions/format_constraint_expression_evaluation.py` & `ahbicht-0.7.2/src/ahbicht/expressions/format_constraint_expression_evaluation.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/expressions/hints_provider.py` & `ahbicht-0.7.2/src/ahbicht/expressions/hints_provider.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/expressions/package_expansion.py` & `ahbicht-0.7.2/src/ahbicht/expressions/package_expansion.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/expressions/requirement_constraint_expression_evaluation.py` & `ahbicht-0.7.2/src/ahbicht/expressions/requirement_constraint_expression_evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module evaluates the parsed condition expression tree regarding the requirement constraints using ConditionNodes.
 The RequirementConstraintTransformer defines the rules how the different parts and nodes
 of the condition expression tree are handled.
 
 The used terms are defined in the README_conditions.md.
 """
 
-from typing import List, Literal, Mapping, Type, Union
+from typing import List, Literal, Mapping, Optional, Type, Union
 
 from lark import Token, Tree, v_args
 from lark.exceptions import VisitError
 
 from ahbicht.condition_node_builder import ConditionNodeBuilder, TRCTransformerArgument
 from ahbicht.evaluation_results import RequirementConstraintEvaluationResult
 from ahbicht.expressions import InvalidExpressionError
@@ -259,31 +259,32 @@
         t.value for t in parsed_tree_rc.scan_values(lambda v: isinstance(v, Token))  # type: ignore[attr-defined]
     ]
     condition_node_builder = ConditionNodeBuilder(all_condition_keys)
     input_nodes = await condition_node_builder.requirement_content_evaluation_for_all_condition_keys()
 
     resulting_condition_node: EvaluatedComposition = evaluate_requirement_constraint_tree(parsed_tree_rc, input_nodes)
 
-    requirement_constraints_fulfilled: bool = (
+    requirement_constraints_fulfilled: Optional[bool] = (
         resulting_condition_node.conditions_fulfilled == ConditionFulfilledValue.FULFILLED
     )
-    requirement_is_conditional = True
+    requirement_is_conditional: Optional[bool] = True
     if resulting_condition_node.conditions_fulfilled == ConditionFulfilledValue.NEUTRAL:  # pylint:disable=no-member
         requirement_constraints_fulfilled = True
         requirement_is_conditional = False
     if resulting_condition_node.conditions_fulfilled == ConditionFulfilledValue.UNKNOWN:  # pylint:disable=no-member
-        unknown_keys = [
-            node_key
-            for node_key, node_value in input_nodes.items()
-            if isinstance(node_value, RequirementConstraint)
-            and node_value.conditions_fulfilled == ConditionFulfilledValue.UNKNOWN
-        ]
-        raise NotImplementedError(
-            f"It is unknown if the conditions ({','.join(unknown_keys)}) are fulfilled due to missing information."
-        )
+        # unknown_keys = [
+        #    node_key
+        #    for node_key, node_value in input_nodes.items()
+        #    if isinstance(node_value, RequirementConstraint)
+        #    and node_value.conditions_fulfilled == ConditionFulfilledValue.UNKNOWN
+        # ]
+        # a NotImplementedError was raised here in ahbicht<=v0.5.11
+        # https://github.com/Hochfrequenz/ahbicht/issues/275
+        requirement_constraints_fulfilled = None
+        requirement_is_conditional = None
 
     format_constraints_expression = getattr(resulting_condition_node, "format_constraints_expression", None)
     if isinstance(resulting_condition_node, UnevaluatedFormatConstraint):
         format_constraints_expression = f"[{resulting_condition_node.condition_key}]"
     hints = getattr(resulting_condition_node, "hint", None)
 
     requirement_constraint_evaluation_result = RequirementConstraintEvaluationResult(
```

### Comparing `ahbicht-0.6.0b0/src/ahbicht/json_serialization/concise_condition_key_tree_schema.py` & `ahbicht-0.7.2/src/ahbicht/json_serialization/concise_condition_key_tree_schema.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/json_serialization/concise_tree_schema.py` & `ahbicht-0.7.2/src/ahbicht/json_serialization/concise_tree_schema.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/json_serialization/tree_schema.py` & `ahbicht-0.7.2/src/ahbicht/json_serialization/tree_schema.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/mapping_results.py` & `ahbicht-0.7.2/src/ahbicht/mapping_results.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/utility_functions.py` & `ahbicht-0.7.2/src/ahbicht/utility_functions.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht/validation/validation.py` & `ahbicht-0.7.2/src/ahbicht/validation/validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -274,15 +274,15 @@
             validation_result=DataElementValidationResult(
                 requirement_validation=RequirementValidationValue.IS_OPTIONAL,
                 format_validation_fulfilled=True,
                 format_error_message=None,
                 hints=invalid_expr_error.error_message,
                 data_element_data_type=DataElementDataType.TEXT,
             ),
-            discriminator=data_element.discriminator,
+            discriminator=data_element.discriminator,  # type:ignore[arg-type]
         )
 
     # requirement constraints
     requirement_validation_without_input_without_hierarchy = map_requirement_validation_values(
         evaluation_result.requirement_constraint_evaluation_result.requirement_constraints_fulfilled,
         evaluation_result.requirement_indicator,
         soll_is_required,
@@ -307,15 +307,15 @@
     validation_logger.debug(
         "The validation of expression '%s' for the data element with discriminator '%s' resulted in %s",
         data_element.ahb_expression,
         data_element.discriminator,
         str(result),
     )
     return ValidationResultInContext(
-        discriminator=data_element.discriminator,
+        discriminator=data_element.discriminator,  # type:ignore[arg-type]
         validation_result=result,
     )
 
 
 async def validate_data_element_valuepool(
     data_element: DataElementValuePool,
     segment_requirement: RequirementValidationValue,
@@ -397,21 +397,21 @@
     )
     validation_logger.debug(
         "The validation for the data element with discriminator '%s' resulted in %s",
         data_element.discriminator,
         str(result),
     )
     return ValidationResultInContext(
-        discriminator=data_element.discriminator,
+        discriminator=data_element.discriminator,  # type:ignore[arg-type]
         validation_result=result,
     )
 
 
 def map_requirement_validation_values(
-    requirement_constraints_are_fulfilled: bool,
+    requirement_constraints_are_fulfilled: Optional[bool],
     requirement_indicator: RequirementIndicator,
     soll_is_required: bool = True,
 ) -> RequirementValidationValue:
     """
     Returns requirement validation value according to the requirement indicator
     and whether the requirements constraints are fulfilled.
     :param requirement_constraints_are_fulfilled: true if requirement constraints are fulfilled
@@ -423,17 +423,29 @@
     # sets soll according to soll_is_required
     if requirement_indicator is ModalMark.SOLL:
         if soll_is_required:
             requirement_indicator = ModalMark.MUSS
         else:
             requirement_indicator = ModalMark.KANN
 
-    if not requirement_constraints_are_fulfilled:
+    if requirement_constraints_are_fulfilled is False:
         requirement_validation = RequirementValidationValue.IS_FORBIDDEN
-    else:
+    elif requirement_constraints_are_fulfilled is None:
+        if requirement_indicator is ModalMark.MUSS or isinstance(requirement_indicator, PrefixOperator):
+            # This error is basically the postponed former RequirementEvaluationFailedBecauseOfUnknownNodesError.
+            # Raising this error here allows the users to use ConditionFulfilledValue.UNKNOWN in the evaluation module
+            # and only care about it again, if they're also using the validation module.
+            # https://github.com/Hochfrequenz/ahbicht/issues/275
+            raise NotImplementedError(
+                # pylint:disable=line-too-long
+                "It's unknown if the requirement constraints are met (most likely because at least one node evaluated to UNKNONW. A validation is meaningless in this case."
+            )
+        if requirement_indicator is ModalMark.KANN or requirement_indicator is ModalMark.SOLL:
+            requirement_validation = RequirementValidationValue.IS_OPTIONAL
+    else:  # True
         if requirement_indicator is ModalMark.MUSS or isinstance(requirement_indicator, PrefixOperator):
             requirement_validation = RequirementValidationValue.IS_REQUIRED
         elif requirement_indicator is ModalMark.KANN:
             requirement_validation = RequirementValidationValue.IS_OPTIONAL
 
     return requirement_validation
```

### Comparing `ahbicht-0.6.0b0/src/ahbicht/validation/validation_results.py` & `ahbicht-0.7.2/src/ahbicht/validation/validation_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
 @attrs.define(auto_attribs=True, kw_only=True)
 class ValidationResultInContext:
     """
     Class to set validation result in context, for example with its discriminator.
     """
 
-    discriminator: Optional[str] = attrs.field(validator=attrs.validators.optional(attrs.validators.instance_of(str)))
+    discriminator: str = attrs.field(validator=attrs.validators.instance_of(str))
     validation_result: ValidationResult = attrs.field(validator=attrs.validators.instance_of(ValidationResult))
 
 
 class ValidationResultInContextSchema(Schema):
     """
     A schema to serialize ValidationResultInContext
     """
@@ -193,15 +193,15 @@
 
         :param edi_domain_to_application_domain_mappings: dictionary with edi domain paths as keys
             and application domain paths as values, for example ediseed to bo4e mapping:
             "$[Dokument][0]['Transaktionsgrund']": "$['transaktionsdaten']['transaktionsgrund']"
         :return:
         """
         for validation_result in self.validation_results:
-            if validation_result.discriminator is not None and validation_result.discriminator.startswith("$"):
+            if validation_result.discriminator.startswith("$"):
                 edi_seed_path = validation_result.discriminator
                 if edi_seed_path in edi_domain_to_application_domain_mappings:
                     bo4e_path = edi_domain_to_application_domain_mappings[edi_seed_path]
                     validation_result.discriminator = bo4e_path
 
     def filter_for_data_element_validation_results(self) -> None:
         """
@@ -210,16 +210,15 @@
         self.validation_results = list(
             filter(lambda vr: isinstance(vr.validation_result, DataElementValidationResult), self.validation_results)
         )
 
     @staticmethod
     def _is_boneycomb_path_result(validation_result_in_context: ValidationResultInContext) -> bool:
         return (
-            validation_result_in_context.discriminator is None
-            or "stammdaten" in validation_result_in_context.discriminator
+            "stammdaten" in validation_result_in_context.discriminator
             or "transaktionsdaten" in validation_result_in_context.discriminator
         )
 
     def filter_for_boneycomb_path_results(self) -> None:
         """
         Filters the list of validation results for those that have a boneycomb path as discriminator
         """
```

### Comparing `ahbicht-0.6.0b0/src/ahbicht/validation/validation_values.py` & `ahbicht-0.7.2/src/ahbicht/validation/validation_values.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/src/ahbicht.egg-info/PKG-INFO` & `ahbicht-0.7.2/src/ahbicht.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahbicht
-Version: 0.6.0b0
+Version: 0.7.2
 Summary: Python Library to parse AHB expressions.
 Home-page: https://github.com/Hochfrequenz/ahbicht
 Author: Annika Schlögl
 Author-email: annika.schloegl@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://ahbicht.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Hochfrequenz/ahbicht/
@@ -421,9 +421,7 @@
 
 .. |Unittests status badge| image:: https://github.com/Hochfrequenz/ahbicht/workflows/Unittests/badge.svg
 .. |Coverage status badge| image:: https://github.com/Hochfrequenz/ahbicht/workflows/Coverage/badge.svg
 .. |Linting status badge| image:: https://github.com/Hochfrequenz/ahbicht/workflows/Linting/badge.svg
 .. |Black status badge| image:: https://github.com/Hochfrequenz/ahbicht/workflows/Black/badge.svg
 .. |pypy status badge| image:: https://img.shields.io/pypi/v/ahbicht
 .. |UTILMD_AHB_WiM_3_1b_20201016.pdf page 90| image:: ./docs/_static/wim_ahb_screenshot.png
-
-
```

### Comparing `ahbicht-0.6.0b0/src/ahbicht.egg-info/SOURCES.txt` & `ahbicht-0.7.2/src/ahbicht.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -18,14 +18,30 @@
 .github/workflows/docs.yml
 .github/workflows/json_schemas.yml
 .github/workflows/packaging_test.yml
 .github/workflows/python-publish.yml
 .github/workflows/pythonlint.yml
 .github/workflows/typescript_from_json_schemas.yml
 .github/workflows/unittests.yml
+dev_requirements/requirements-coverage.in
+dev_requirements/requirements-coverage.txt
+dev_requirements/requirements-docs.in
+dev_requirements/requirements-docs.txt
+dev_requirements/requirements-formatting.in
+dev_requirements/requirements-formatting.txt
+dev_requirements/requirements-json_schemas.in
+dev_requirements/requirements-json_schemas.txt
+dev_requirements/requirements-linting.in
+dev_requirements/requirements-linting.txt
+dev_requirements/requirements-test_packaging.in
+dev_requirements/requirements-test_packaging.txt
+dev_requirements/requirements-tests.in
+dev_requirements/requirements-tests.txt
+dev_requirements/requirements-type_check.in
+dev_requirements/requirements-type_check.txt
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/_static/ahbicht-favicon.png
 docs/_static/ahbicht-logo-raw.svg
 docs/_static/ahbicht-logo.png
```

### Comparing `ahbicht-0.6.0b0/tox.ini` & `ahbicht-0.7.2/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -11,96 +11,98 @@
 [testenv]
 commands = python -m pip install --upgrade pip
 
 [testenv:tests]
 # the tests environment is called by the Github action that runs the unit tests
 usedevelop = True
 deps =
-    -rrequirements.txt
-    pytest
-    pytest_mock
-    pytest-asyncio
-    pytest-datafiles
+    -r requirements.txt
+    -r dev_requirements/requirements-tests.txt
 commands = python -m pytest --basetemp={envtmpdir} {posargs}
 
 [testenv:linting]
 # the linting environment is called by the Github Action that runs the linter
 deps =
     {[testenv:json_schemas]deps}
     -rrequirements.txt
-    pylint
+    -r dev_requirements/requirements-linting.txt
 # add your fixtures like e.g. pytest_datafiles here
 commands =
     pylint src/ahbicht
     pylint json_schemas/generate_json_schemas.py
 # add single files (ending with .py) or packages here
 
 [testenv:type_check]
+usedevelop=True
 # the type_check environment is called by the Github Action that runs the static type check (mypy)
+# because we type-check the tests it's good to install e.g. pytest in the type_check env
 deps =
     {[testenv:json_schemas]deps}
-    -rrequirements.txt
-    types-pytz
-    mypy
+    {[testenv:tests]deps}
+    -r requirements.txt
+    -r dev_requirements/requirements-type_check.txt
 commands =
     mypy --show-error-codes src/ahbicht
     mypy --show-error-codes unittests
     mypy --show-error-codes json_schemas/generate_json_schemas.py
 # add single files (ending with .py) or packages here
 
 [testenv:coverage]
 # the coverage environment is called by the Github Action that runs the coverage measurement
 usedevelop = True
 deps =
     {[testenv:tests]deps}
-    coverage
+    -r dev_requirements/requirements-coverage.txt
 commands =
     coverage run -m pytest --basetemp={envtmpdir} {posargs}
     coverage html --omit .tox/*,unittests/*
     coverage report --fail-under 95 --omit .tox/*,unittests/*
 
+[testenv:formatting]
+deps =
+    -r dev_requirements/requirements-formatting.txt
+commands =
+    black . --check
+    isort . --check
+
 [testenv:dev]
 # the dev environment contains everything you need to start developing on your local machine.
 deps =
     {[testenv:tests]deps}
     {[testenv:linting]deps}
     {[testenv:type_check]deps}
     {[testenv:coverage]deps}
     {[testenv:json_schemas]deps}
-    black
-    black[jupyter]
+    {[testenv:formatting]deps}
     nest_asyncio
-    isort
     pip-tools
     pre-commit
 commands =
     python -m pip install --upgrade pip
     pip-compile requirements.in
     pip install -r requirements.txt
     pre-commit install
 
 [testenv:test_packaging]
 skip_install = true
 deps =
-    build
-    twine
+    -r dev_requirements/requirements-test_packaging.txt
 commands =
     python -m build
     twine check dist/*
 
 [testenv:docs]
 deps =
-    -rrequirements.txt
-    Sphinx
-    sphinx_rtd_theme
+    -r requirements.txt
+    -r dev_requirements/requirements-docs.txt
 commands =
     sphinx-build -W -b html -d {envtmpdir}/doctrees docs {envtmpdir}/html
     sphinx-build -n -T -W -b doctest -d {envtmpdir}/doctrees docs docs/_build/html
     python -m doctest README.rst
 
 [testenv:json_schemas]
 usedevelop = True
 deps =
-    -rrequirements.txt
-    marshmallow_jsonschema
+    -r requirements.txt
+    -r dev_requirements/requirements-json_schemas.txt
 commands =
     python json_schemas/generate_json_schemas.py
```

### Comparing `ahbicht-0.6.0b0/unittests/conftest.py` & `ahbicht-0.7.2/unittests/conftest.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/content_evaluation_result_generation/example0.json` & `ahbicht-0.7.2/unittests/content_evaluation_result_generation/example0.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/content_evaluation_result_generation/example1.json` & `ahbicht-0.7.2/unittests/content_evaluation_result_generation/example1.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/defaults.py` & `ahbicht-0.7.2/unittests/defaults.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/provider_test_files/example_hints_file.json` & `ahbicht-0.7.2/unittests/provider_test_files/example_hints_file.json`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_ahb_expression_evaluation.py` & `ahbicht-0.7.2/unittests/test_ahb_expression_evaluation.py`

 * *Files 14% similar despite different names*

```diff
@@ -346,7 +346,80 @@
                 edifact_format=default_test_format,
                 edifact_format_version=default_test_version,
             )
             evaluation_result = await evaluate_ahb_expression_tree(tree)
             assert evaluation_result is not None
         finally:
             inject.clear()
+
+    @pytest.mark.parametrize(
+        "ahb_expression, content_evaluation_result, expected",
+        [
+            pytest.param(
+                "Soll [1]",
+                ContentEvaluationResult(
+                    hints={},
+                    format_constraints={},
+                    requirement_constraints={
+                        "1": ConditionFulfilledValue.UNKNOWN,
+                    },
+                    id=uuid.UUID("9bdc494b-8e61-440b-a15d-eb5630916969"),
+                    packages={},
+                ),
+                AhbExpressionEvaluationResult(
+                    requirement_indicator=ModalMark.SOLL,
+                    requirement_constraint_evaluation_result=RequirementConstraintEvaluationResult(
+                        requirement_constraints_fulfilled=None,
+                        requirement_is_conditional=None,
+                        format_constraints_expression=None,
+                        hints=None,
+                    ),
+                    format_constraint_evaluation_result=FormatConstraintEvaluationResult(
+                        format_constraints_fulfilled=True
+                    ),
+                ),
+            ),
+            pytest.param(
+                "Muss [1]",
+                ContentEvaluationResult(
+                    hints={},
+                    format_constraints={},
+                    requirement_constraints={
+                        "1": ConditionFulfilledValue.UNKNOWN,
+                    },
+                    id=uuid.UUID("ba79e51c-6b74-44ed-ad53-66fba828b1b8"),
+                    packages={},
+                ),
+                AhbExpressionEvaluationResult(
+                    requirement_indicator=ModalMark.MUSS,
+                    requirement_constraint_evaluation_result=RequirementConstraintEvaluationResult(
+                        requirement_constraints_fulfilled=None,
+                        requirement_is_conditional=None,
+                        format_constraints_expression=None,
+                        hints=None,
+                    ),
+                    format_constraint_evaluation_result=FormatConstraintEvaluationResult(
+                        format_constraints_fulfilled=True
+                    ),
+                ),
+            ),
+        ],
+    )
+    async def test_no_not_implemented_error_is_raised_for_unknown_nodes(
+        self,
+        ahb_expression: str,
+        content_evaluation_result: ContentEvaluationResult,
+        expected: AhbExpressionEvaluationResult,
+    ):
+        tree = parse_ahb_expression_to_single_requirement_indicator_expressions(ahb_expression)
+        try:
+            create_and_inject_hardcoded_evaluators(
+                content_evaluation_result,
+                evaluatable_data_provider=return_empty_dummy_evaluatable_data,
+                edifact_format=default_test_format,
+                edifact_format_version=default_test_version,
+            )
+            evaluation_result = await evaluate_ahb_expression_tree(tree)
+            assert evaluation_result is not None
+            assert evaluation_result == expected
+        finally:
+            inject.clear()
```

### Comparing `ahbicht-0.6.0b0/unittests/test_ahb_expression_parser.py` & `ahbicht-0.7.2/unittests/test_ahb_expression_parser.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_caching.py` & `ahbicht-0.7.2/unittests/test_caching.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
             len(tree_instances)
             * len(tree_instances)
             / len([1 for x, y in product(tree_instances, tree_instances) if x is y])
         )
         assert number_of_distinct_instances == number_of_calls
 
     async def test_ahb_expression_cache_async(self, mocker):
-
         ahb_expression = "Muss [5] U [6]"
         parse_spy = mocker.spy(ahb_expr_parser, "parse")
 
         async def parsing_task():
             parse_ahb_expression_to_single_requirement_indicator_expressions(ahb_expression)
 
         tasks = [parsing_task() for _ in range(100)]
```

### Comparing `ahbicht-0.6.0b0/unittests/test_categorized_key_extraction.py` & `ahbicht-0.7.2/unittests/test_categorized_key_extraction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ Tests for the parsing of the conditions tests (Mussfeldprüfung) """
 
 import json
+from pathlib import Path
 from typing import List
 
 import pytest  # type:ignore[import]
 
 from ahbicht.content_evaluation.categorized_key_extract import CategorizedKeyExtract, CategorizedKeyExtractSchema
 from ahbicht.content_evaluation.content_evaluation_result import ContentEvaluationResult, ContentEvaluationResultSchema
 from ahbicht.expressions.condition_expression_parser import extract_categorized_keys
@@ -186,16 +187,17 @@
         "test_file_path",
         [
             pytest.param("example0.json", id="0 FC, 3 RC"),
             pytest.param("example1.json", id="2 FC, 3 RC"),
         ],
     )
     @ALL_LARGE_TEST_CASES
-    def test_possible_cer_generation_large_results(self, test_file_path, datafiles):
-        file_content = json.load(datafiles / test_file_path)
+    def test_possible_cer_generation_large_results(self, test_file_path: str, datafiles):
+        with open(datafiles / Path(test_file_path), "r", encoding="utf-8") as infile:
+            file_content = json.load(infile)
         categorized_keys = CategorizedKeyExtractSchema().load(file_content["categorizedKeyExtract"])
         expected_result = ContentEvaluationResultSchema(many=True).load(file_content["expected_result"])
         actual = categorized_keys.generate_possible_content_evaluation_results()
         # json_string = ContentEvaluationResultSchema(many=True).dumps(actual)
         assert actual == expected_result
 
     @pytest.mark.parametrize(
```

### Comparing `ahbicht-0.6.0b0/unittests/test_cer_based_fc_evaluator.py` & `ahbicht-0.7.2/unittests/test_cer_based_fc_evaluator.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_cer_based_hints_provider.py` & `ahbicht-0.7.2/unittests/test_cer_based_hints_provider.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_cer_based_package_resolver.py` & `ahbicht-0.7.2/unittests/test_cer_based_package_resolver.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_cer_based_rc_evaluator.py` & `ahbicht-0.7.2/unittests/test_cer_based_rc_evaluator.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_condition_node_builder.py` & `ahbicht-0.7.2/unittests/test_condition_node_builder.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_condition_nodes.py` & `ahbicht-0.7.2/unittests/test_condition_nodes.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_condition_parser.py` & `ahbicht-0.7.2/unittests/test_condition_parser.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_dict_based_fc_evaluator.py` & `ahbicht-0.7.2/unittests/test_dict_based_fc_evaluator.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_dict_based_rc_evaluator.py` & `ahbicht-0.7.2/unittests/test_dict_based_rc_evaluator.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_evaluator_factory.py` & `ahbicht-0.7.2/unittests/test_evaluator_factory.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_evaluator_provider.py` & `ahbicht-0.7.2/unittests/test_evaluator_provider.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_expression_builder.py` & `ahbicht-0.7.2/unittests/test_expression_builder.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_expression_resolver.py` & `ahbicht-0.7.2/unittests/test_expression_resolver.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_format_constraint_expression_evaluation.py` & `ahbicht-0.7.2/unittests/test_format_constraint_expression_evaluation.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_format_constraints_context_var.py` & `ahbicht-0.7.2/unittests/test_format_constraints_context_var.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_german_strom_and_gas_tag.py` & `ahbicht-0.7.2/unittests/test_german_strom_and_gas_tag.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_hints_provider.py` & `ahbicht-0.7.2/unittests/test_hints_provider.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_integration_mwe.py` & `ahbicht-0.7.2/unittests/test_integration_mwe.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 from contextvars import ContextVar
 from logging import LogRecord
 from typing import List
 
 import inject
 import pytest  # type:ignore[import]
 import pytest_asyncio  # type:ignore[import]
-from maus.models.anwendungshandbuch import AhbMetaInformation, DeepAnwendungshandbuch
-from maus.models.edifact_components import (
+from maus import (
     DataElementFreeText,
     DataElementValuePool,
+    DeepAnwendungshandbuch,
     Segment,
     SegmentGroup,
     ValuePoolEntry,
 )
+from maus.models.anwendungshandbuch import AhbMetaInformation
 
 from ahbicht.content_evaluation.evaluationdatatypes import EvaluatableData, EvaluatableDataProvider
 from ahbicht.content_evaluation.token_logic_provider import SingletonTokenLogicProvider, TokenLogicProvider
 from ahbicht.expressions.condition_nodes import ConditionFulfilledValue, EvaluatedFormatConstraint
 from ahbicht.validation.validation import validate_deep_anwendungshandbuch
 from unittests.defaults import (
     DefaultHintsProvider,
```

### Comparing `ahbicht-0.6.0b0/unittests/test_json_serialization.py` & `ahbicht-0.7.2/unittests/test_json_serialization.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_mixed_sync_async_rc_fc_evaluation.py` & `ahbicht-0.7.2/unittests/test_mixed_sync_async_rc_fc_evaluation.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_package_resolver.py` & `ahbicht-0.7.2/unittests/test_package_resolver.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_requirement_constraint_evaluation.py` & `ahbicht-0.7.2/unittests/test_requirement_constraint_evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,21 +137,14 @@
             # no value for [2]
             pytest.param(
                 "[1]U[2]",
                 {"1": RequirementConstraint(condition_key="1", conditions_fulfilled=ConditionFulfilledValue.FULFILLED)},
                 ValueError,
                 "Please make sure that the input values contain all necessary condition_keys.",
             ),
-            # unknown value as result
-            pytest.param(
-                "[101]",
-                _input_values,
-                NotImplementedError,
-                "It is unknown if the conditions (101) are fulfilled due to missing information.",
-            ),
         ],
     )
     async def test_evaluate_condition_expression_with_invalid_values(
         self,
         mocker,
         condition_expression: str,
         input_values: dict,
```

### Comparing `ahbicht-0.6.0b0/unittests/test_requirement_constraint_expression_evaluation.py` & `ahbicht-0.7.2/unittests/test_requirement_constraint_expression_evaluation.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_time_condition_resolver.py` & `ahbicht-0.7.2/unittests/test_time_condition_resolver.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_tree_schemas.py` & `ahbicht-0.7.2/unittests/test_tree_schemas.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_utility_functions.py` & `ahbicht-0.7.2/unittests/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_validation.py` & `ahbicht-0.7.2/unittests/test_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -972,33 +972,52 @@
                 RequirementValidationValue.IS_REQUIRED,
             ),
             pytest.param(
                 False,
                 ModalMark.MUSS,
                 RequirementValidationValue.IS_FORBIDDEN,
             ),
+            pytest.param(
+                None,
+                ModalMark.SOLL,
+                RequirementValidationValue.IS_OPTIONAL,
+            ),
+            pytest.param(
+                None,
+                ModalMark.KANN,
+                RequirementValidationValue.IS_OPTIONAL,
+            ),
         ],
     )
     def test_map_requirement_validation_values_soll_not_required(
         self, requirement_constraints_are_fulfilled, requirement_indicator, expected_requirement_validation_value
     ):
         requirement_validation_value = map_requirement_validation_values(
             requirement_constraints_are_fulfilled, requirement_indicator, soll_is_required=False
         )
         assert requirement_validation_value == expected_requirement_validation_value
 
+    def test_map_requirement_validation_values_muss_with_unknown_rcs(self):
+        with pytest.raises(NotImplementedError):
+            _ = map_requirement_validation_values(None, ModalMark.MUSS, soll_is_required=False)
+
     def test_map_requirement_validation_values_all_cases_are_covered(self):
         """
         A fuzzing test to make sure all possible input values are mapped
         """
         requirement_indicators: List[RequirementIndicator] = [x for x in ModalMark] + [x for x in PrefixOperator]
         for rcs_fulfilled, requirement_indicator, soll_is_required in product(
-            [True, False], requirement_indicators, [True, False]
+            [True, None, False], requirement_indicators, [True, False]
         ):
-            result = map_requirement_validation_values(rcs_fulfilled, requirement_indicator, soll_is_required)
+            try:
+                result = map_requirement_validation_values(rcs_fulfilled, requirement_indicator, soll_is_required)
+            except NotImplementedError:
+                if rcs_fulfilled is None:
+                    continue  # this case is ok
+                raise
             assert result is not None
             assert isinstance(result, RequirementValidationValue)
 
     @pytest.mark.parametrize(
         "parent_level_requirement, child_level_requirement, expected_requirement",
         [
             pytest.param(
```

### Comparing `ahbicht-0.6.0b0/unittests/test_validation_results.py` & `ahbicht-0.7.2/unittests/test_validation_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,9 +243,9 @@
                 ),
             ),
         ],
     )
     async def test_lovric_remove_absender_and_empfaenger_path_results(
         self, lovric_actual: ListOfValidationResultInContext, lovric_expected: ListOfValidationResultInContext
     ):
-        lovric_actual.remove_absender_and_empfaenger_path_results()
+        lovric_actual.remove_absender_and_empfaenger_path_results()  # type:ignore[attr-defined]
         assert lovric_actual == lovric_expected
```

### Comparing `ahbicht-0.6.0b0/unittests/test_validity_check.py` & `ahbicht-0.7.2/unittests/test_validity_check.py`

 * *Files identical despite different names*

### Comparing `ahbicht-0.6.0b0/unittests/test_warning_when_using_inject_attr.py` & `ahbicht-0.7.2/unittests/test_warning_when_using_inject_attr.py`

 * *Files identical despite different names*

